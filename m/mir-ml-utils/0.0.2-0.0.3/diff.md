# Comparing `tmp/mir_ml_utils-0.0.2.tar.gz` & `tmp/mir_ml_utils-0.0.3.tar.gz`

## Comparing `mir_ml_utils-0.0.2.tar` & `mir_ml_utils-0.0.3.tar`

### file list

```diff
@@ -1,195 +1,195 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/requirements.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/.idea/.gitignore
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/.idea/modules.xml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/.idea/src.iml
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/.idea/vcs.xml
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/.idea/workspace.xml
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/config.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/data_handlers/__init__.py
--rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/data_handlers/dataset_with_masks.py
--rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/data_handlers/images_dataset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/__init__.py
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/utils.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/__init__.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/cub.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/danish_fungi.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/default_configs.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/easy_set.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/few_shot_dataset.py
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/mini_imagenet.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/support_set_folder.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/tiered_imagenet.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/__init__.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/bd_cspn.py
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/few_shot_classifier.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/finetune.py
--rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/matching_networks.py
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/prototypical_networks.py
--rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/relation_networks.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/tim.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/transductive_finetuning.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/utils.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/modules/__init__.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/modules/predesigned_modules.py
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/modules/resnet.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/samplers/__init__.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/samplers/task_sampler.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/factories/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/factories/loss_function_factory.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/factories/model_adaptor_factory.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/factories/model_builder_factory.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/factories/optimzer_factory.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/loss_functions/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/loss_functions/loss_function_result.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/loss_functions/loss_function_wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/examples/python/README.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/__init__.py
--rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/plot_optical_flow.py
--rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/plot_repurposing_annotations.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/plot_scripted_tensor_transforms.py
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/plot_transforms.py
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/plot_video_api.py
--rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/plot_visualization_utils.py
--rw-r--r--   0        0        0   316358 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054.png
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054_mask.png
--rw-r--r--   0        0        0    40344 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/astronaut.jpg
--rw-r--r--   0        0        0   771052 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/basketball.mp4
--rw-r--r--   0        0        0    97422 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/dog1.jpg
--rw-r--r--   0        0        0    90796 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/dog2.jpg
--rw-r--r--   0        0        0    35364 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/imagenet_class_index.json
--rw-r--r--   0        0        0    70126 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/person1.jpg
--rw-r--r--   0        0        0   858575 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/repurposing_annotations_thumbnail.png
--rw-r--r--   0        0        0   632918 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/transforms_thumbnail.png
--rw-r--r--   0        0        0   300404 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/visualization_utils_thumbnail2.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/__init__.py
--rw-r--r--   0        0        0    16652 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/__init__.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/presets.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/sampler.py
--rw-r--r--   0        0        0    22550 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/train.py
--rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/train_quantization.py
--rw-r--r--   0        0        0     6780 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/transforms.py
--rw-r--r--   0        0        0    15769 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/__init__.py
--rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/__init__.py
--rw-r--r--   0        0        0    11905 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/cascade_evaluation.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/parsing.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/presets.py
--rw-r--r--   0        0        0    33426 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/train.py
--rw-r--r--   0        0        0    25981 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/transforms.py
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/vizualization.py
--rw-r--r--   0        0        0   273008 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/Loss.jpg
--rw-r--r--   0        0        0  1343300 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-background-mode-collapse.jpg
--rw-r--r--   0        0        0  1781352 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-domain-drift.jpg
--rw-r--r--   0        0        0   321833 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/gradient-norm-removal.jpg
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/__init__.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/distributed.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/logger.py
--rw-r--r--   0        0        0    17472 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/losses.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/metrics.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/norm.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/padder.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/__init__.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/coco_eval.py
--rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/coco_utils.py
--rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/engine.py
--rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/group_by_aspect_ratio.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/presets.py
--rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/train.py
--rw-r--r--   0        0        0    23337 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/transforms.py
--rw-r--r--   0        0        0     9265 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/utils.py
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/optical_flow/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/optical_flow/__init__.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/optical_flow/presets.py
--rw-r--r--   0        0        0    15501 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/optical_flow/train.py
--rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/optical_flow/transforms.py
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/optical_flow/utils.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/__init__.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/coco_utils.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/presets.py
--rw-r--r--   0        0        0    12665 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/train.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/transforms.py
--rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/utils.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/similarity/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/similarity/__init__.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/similarity/loss.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/similarity/model.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/similarity/sampler.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/similarity/test.py
--rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/similarity/train.py
--rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/video_classification/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/video_classification/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/video_classification/datasets.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/video_classification/presets.py
--rw-r--r--   0        0        0    18245 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/video_classification/train.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/video_classification/transforms.py
--rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/video_classification/utils.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/scripts/README.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/scripts/__init__.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/scripts/collect_model_urls.py
--rwxr-xr-x   0        0        0     1147 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/scripts/fbcode_to_main_sync.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/scripts/release_notes/__init__.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/scripts/release_notes/classify_prs.py
--rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/scripts/release_notes/retrieve_prs_data.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/models/__init__.py
--rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/models/easyfsl_proto_net_classifier.py
--rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/models/linear_regressor_model_tester.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/models/model_adaptor.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/models/model_adaptor_type_enum.py
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/models/model_loaders.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/models/models_enum.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/models/resnet_model_predictor_wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/pytorch_util_modules/__init__.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/pytorch_util_modules/flatten_module.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/pytorch_util_modules/pytorch_hooks.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/pytorch_util_modules/utils.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/testers/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/testers/inference_enum_types.py
--rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/testers/test_wrapper.py
--rw-r--r--   0        0        0    23901 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/testers/two_class_model_tester_wrapper.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/trainers/__init__.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/trainers/model_trainer_type_enum.py
--rw-r--r--   0        0        0    20312 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/trainers/pytorch_trainer.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/trainers/trainer_info.py
--rw-r--r--   0        0        0    13573 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/trainers/trainer_wrapper.py
--rw-r--r--   0        0        0    39818 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/trainers/trainer_wrapper_pimpl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/utils/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/utils/array_utils.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/utils/exceptions.py
--rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/utils/file_utils.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/utils/function_wrappers.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/utils/math_ops.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/src/mir_ml_utils/utils/mode_enum.py
--rw-r--r--   0        0        0   142798 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/testing_data/corrosion_4.png
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/testing_data/highres_raw_train_two_classes.csv
--rw-r--r--   0        0        0   195177 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/testing_data/hull001_label.jpg
--rw-r--r--   0        0        0   462993 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/testing_data/prototypical_net_test_data/best_model.pth
--rw-r--r--   0        0        0   166635 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/testing_data/prototypical_net_test_data/train_prototypes.pth
--rw-r--r--   0        0        0   151371 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/testing_data/prototypical_net_test_data/inference/corrosion_1.png
--rw-r--r--   0        0        0   162210 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/testing_data/prototypical_net_test_data/inference/corrosion_2.png
--rw-r--r--   0        0        0   140763 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/testing_data/prototypical_net_test_data/inference/corrosion_3.png
--rw-r--r--   0        0        0   142798 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/testing_data/prototypical_net_test_data/inference/corrosion_4.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/tests/test_images_dataset.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/tests/test_img_pipeline.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/tests/test_img_utils.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/tests/test_math_ops.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/tests/test_prototypical_loss.py
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/tests/test_pytorch_trainer.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/tests/test_suite.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/trainer_wrapper_config_template/config.json
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/LICENSE
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/README.md
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/.idea/.gitignore
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/.idea/modules.xml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/.idea/src.iml
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/.idea/vcs.xml
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/.idea/workspace.xml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/config.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/data_handlers/__init__.py
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/data_handlers/dataset_with_masks.py
+-rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/data_handlers/images_dataset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/__init__.py
+-rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/utils.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/__init__.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/cub.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/danish_fungi.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/default_configs.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/easy_set.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/few_shot_dataset.py
+-rw-r--r--   0        0        0     6137 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/mini_imagenet.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/support_set_folder.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/tiered_imagenet.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/__init__.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/bd_cspn.py
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/few_shot_classifier.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/finetune.py
+-rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/matching_networks.py
+-rw-r--r--   0        0        0     7666 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/prototypical_networks.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/relation_networks.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/tim.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/transductive_finetuning.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/utils.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/modules/__init__.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/modules/predesigned_modules.py
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/modules/resnet.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/samplers/__init__.py
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/samplers/task_sampler.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/factories/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/factories/loss_function_factory.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/factories/model_adaptor_factory.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/factories/model_builder_factory.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/factories/optimzer_factory.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/loss_functions/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/loss_functions/loss_function_result.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/loss_functions/loss_function_wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/examples/python/README.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/__init__.py
+-rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/plot_optical_flow.py
+-rw-r--r--   0        0        0     7485 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/plot_repurposing_annotations.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/plot_scripted_tensor_transforms.py
+-rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/plot_transforms.py
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/plot_video_api.py
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/plot_visualization_utils.py
+-rw-r--r--   0        0        0   316358 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054.png
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054_mask.png
+-rw-r--r--   0        0        0    40344 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/astronaut.jpg
+-rw-r--r--   0        0        0   771052 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/basketball.mp4
+-rw-r--r--   0        0        0    97422 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/dog1.jpg
+-rw-r--r--   0        0        0    90796 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/dog2.jpg
+-rw-r--r--   0        0        0    35364 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/imagenet_class_index.json
+-rw-r--r--   0        0        0    70126 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/person1.jpg
+-rw-r--r--   0        0        0   858575 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/repurposing_annotations_thumbnail.png
+-rw-r--r--   0        0        0   632918 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/transforms_thumbnail.png
+-rw-r--r--   0        0        0   300404 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/visualization_utils_thumbnail2.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/__init__.py
+-rw-r--r--   0        0        0    16652 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/__init__.py
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/presets.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/sampler.py
+-rw-r--r--   0        0        0    22550 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/train.py
+-rw-r--r--   0        0        0    11093 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/train_quantization.py
+-rw-r--r--   0        0        0     6780 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/transforms.py
+-rw-r--r--   0        0        0    15769 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/__init__.py
+-rw-r--r--   0        0        0     9976 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/__init__.py
+-rw-r--r--   0        0        0    11905 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/cascade_evaluation.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/parsing.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/presets.py
+-rw-r--r--   0        0        0    33426 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/train.py
+-rw-r--r--   0        0        0    25981 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/transforms.py
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/vizualization.py
+-rw-r--r--   0        0        0   273008 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/Loss.jpg
+-rw-r--r--   0        0        0  1343300 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-background-mode-collapse.jpg
+-rw-r--r--   0        0        0  1781352 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-domain-drift.jpg
+-rw-r--r--   0        0        0   321833 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/gradient-norm-removal.jpg
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/__init__.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/distributed.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/logger.py
+-rw-r--r--   0        0        0    17472 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/losses.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/metrics.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/norm.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/padder.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/__init__.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/coco_eval.py
+-rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/coco_utils.py
+-rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/engine.py
+-rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/group_by_aspect_ratio.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/presets.py
+-rw-r--r--   0        0        0    12595 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/train.py
+-rw-r--r--   0        0        0    23337 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/transforms.py
+-rw-r--r--   0        0        0     9265 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/utils.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/optical_flow/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/optical_flow/__init__.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/optical_flow/presets.py
+-rw-r--r--   0        0        0    15501 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/optical_flow/train.py
+-rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/optical_flow/transforms.py
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/optical_flow/utils.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/__init__.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/coco_utils.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/presets.py
+-rw-r--r--   0        0        0    12665 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/train.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/transforms.py
+-rw-r--r--   0        0        0     9136 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/utils.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/similarity/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/similarity/__init__.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/similarity/loss.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/similarity/model.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/similarity/sampler.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/similarity/test.py
+-rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/similarity/train.py
+-rw-r--r--   0        0        0     5900 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/video_classification/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/video_classification/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/video_classification/datasets.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/video_classification/presets.py
+-rw-r--r--   0        0        0    18245 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/video_classification/train.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/video_classification/transforms.py
+-rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/video_classification/utils.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/scripts/README.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/scripts/__init__.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/scripts/collect_model_urls.py
+-rwxr-xr-x   0        0        0     1147 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/scripts/fbcode_to_main_sync.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/scripts/release_notes/__init__.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/scripts/release_notes/classify_prs.py
+-rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/scripts/release_notes/retrieve_prs_data.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/models/__init__.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/models/easyfsl_proto_net_classifier.py
+-rw-r--r--   0        0        0     6777 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/models/linear_regressor_model_tester.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/models/model_adaptor.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/models/model_adaptor_type_enum.py
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/models/model_loaders.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/models/models_enum.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/models/resnet_model_predictor_wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/pytorch_util_modules/__init__.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/pytorch_util_modules/flatten_module.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/pytorch_util_modules/pytorch_hooks.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/pytorch_util_modules/utils.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/testers/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/testers/inference_enum_types.py
+-rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/testers/test_wrapper.py
+-rw-r--r--   0        0        0    23901 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/testers/two_class_model_tester_wrapper.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/trainers/__init__.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/trainers/model_trainer_type_enum.py
+-rw-r--r--   0        0        0    20312 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/trainers/pytorch_trainer.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/trainers/trainer_info.py
+-rw-r--r--   0        0        0    13573 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/trainers/trainer_wrapper.py
+-rw-r--r--   0        0        0    39818 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/trainers/trainer_wrapper_pimpl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/utils/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/utils/array_utils.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/utils/exceptions.py
+-rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/utils/file_utils.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/utils/function_wrappers.py
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/utils/math_ops.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/src/mir_ml_utils/utils/mode_enum.py
+-rw-r--r--   0        0        0   142798 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/testing_data/corrosion_4.png
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/testing_data/highres_raw_train_two_classes.csv
+-rw-r--r--   0        0        0   195177 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/testing_data/hull001_label.jpg
+-rw-r--r--   0        0        0   462993 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/testing_data/prototypical_net_test_data/best_model.pth
+-rw-r--r--   0        0        0   166635 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/testing_data/prototypical_net_test_data/train_prototypes.pth
+-rw-r--r--   0        0        0   151371 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/testing_data/prototypical_net_test_data/inference/corrosion_1.png
+-rw-r--r--   0        0        0   162210 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/testing_data/prototypical_net_test_data/inference/corrosion_2.png
+-rw-r--r--   0        0        0   140763 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/testing_data/prototypical_net_test_data/inference/corrosion_3.png
+-rw-r--r--   0        0        0   142798 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/testing_data/prototypical_net_test_data/inference/corrosion_4.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/tests/test_images_dataset.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/tests/test_img_pipeline.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/tests/test_img_utils.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/tests/test_math_ops.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/tests/test_prototypical_loss.py
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/tests/test_pytorch_trainer.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/tests/test_suite.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/trainer_wrapper_config_template/config.json
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/README.md
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 mir_ml_utils-0.0.3/PKG-INFO
```

### Comparing `mir_ml_utils-0.0.2/src/.idea/workspace.xml` & `mir_ml_utils-0.0.3/src/.idea/workspace.xml`

 * *Files 17% similar despite different names*

#### Comparing `mir_ml_utils-0.0.2/src/.idea/workspace.xml` & `mir_ml_utils-0.0.3/src/.idea/workspace.xml`

```diff
@@ -47,8 +47,19 @@
           <value>
             <State/>
           </value>
         </entry>
       </map>
     </option>
   </component>
+  <component name="XDebuggerManager">
+    <breakpoint-manager>
+      <breakpoints>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/mir_ml_utils/easyfsl/methods/relation_networks.py</url>
+          <line>5</line>
+          <option name="timeStamp" value="1"/>
+        </line-breakpoint>
+      </breakpoints>
+    </breakpoint-manager>
+  </component>
 </project>
```

### Comparing `mir_ml_utils-0.0.2/src/.idea/inspectionProfiles/Project_Default.xml` & `mir_ml_utils-0.0.3/src/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/data_handlers/dataset_with_masks.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/data_handlers/dataset_with_masks.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/data_handlers/images_dataset.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/data_handlers/images_dataset.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/utils.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/cub.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/tiered_imagenet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from pathlib import Path
 
-from src.easyfsl.datasets.easy_set import EasySet
-from src.easyfsl.datasets.few_shot_dataset import FewShotDataset
+from mir_ml_utils.easyfsl.datasets.easy_set import EasySet
+from mir_ml_utils.easyfsl.datasets.few_shot_dataset import FewShotDataset
 
-CUB_SPECS_DIR = Path("data/CUB")
+TIERED_IMAGENET_SPECS_DIR = Path("data/tiered_imagenet")
 
 
 # pylint: disable=invalid-name
-def CUB(split: str, **kwargs) -> FewShotDataset:
+def TieredImageNet(split: str, **kwargs) -> FewShotDataset:
     """
-    Build the CUB dataset for the specific split.
+    Build the tieredImageNet dataset for the specific split.
     Args:
         split: one of the available split (typically train, val, test).
 
     Returns:
         the constructed dataset using EasySet
 
     Raises:
         ValueError: if the specified split cannot be associated with a JSON spec file
-            from CUB's specs directory
+            from tieredImageNet's specs directory
     """
-    specs_file = CUB_SPECS_DIR / f"{split}.json"
+    specs_file = TIERED_IMAGENET_SPECS_DIR / f"{split}.json"
     if specs_file.is_file():
         return EasySet(specs_file=specs_file, **kwargs)
 
-    raise ValueError(f"Could not find specs file {specs_file.name} in {CUB_SPECS_DIR}")
+    raise ValueError(
+        f"Could not find specs file {specs_file.name} in {TIERED_IMAGENET_SPECS_DIR}"
+    )
 
 
 # pylint: enable=invalid-name
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/danish_fungi.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/danish_fungi.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import List, Union, Tuple, Callable
 
 import pandas as pd
 from pandas import DataFrame
 from PIL import Image
 from torch import Tensor
 
-from src.easyfsl.datasets.few_shot_dataset import FewShotDataset
-from src.easyfsl.datasets.default_configs import default_transform
+from mir_ml_utils.easyfsl.datasets.few_shot_dataset import FewShotDataset
+from mir_ml_utils.easyfsl.datasets.default_configs import default_transform
 
 WHOLE_DANISH_FUNGI_SPECS_FILE = Path("data/fungi") / "DF20_metadata.csv"
 
 
 class DanishFungi(FewShotDataset):
     def __init__(
         self,
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/default_configs.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/default_configs.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/easy_set.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/easy_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import warnings
 from pathlib import Path
 from typing import List, Union, Set, Tuple, Callable
 
 from PIL import Image
 
-from src.easyfsl.datasets.few_shot_dataset import FewShotDataset
-from src.easyfsl.datasets.default_configs import default_transform, DEFAULT_IMAGE_FORMATS
+from mir_ml_utils.easyfsl.datasets.few_shot_dataset import FewShotDataset
+from mir_ml_utils.easyfsl.datasets.default_configs import default_transform, DEFAULT_IMAGE_FORMATS
 
 
 class EasySet(FewShotDataset):
     """
     A ready-to-use dataset. Will work for any dataset where the images are
     grouped in directories by class. It expects a JSON file defining the
     classes and where to find them. It must have the following shape:
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/few_shot_dataset.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/few_shot_dataset.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/mini_imagenet.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/mini_imagenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import pandas as pd
 from pandas import DataFrame
 from PIL import Image
 import torch
 from torch import Tensor
 from tqdm import tqdm
 
-from src.easyfsl.datasets.few_shot_dataset import FewShotDataset
-from src.easyfsl.datasets.default_configs import (
+from mir_ml_utils.easyfsl.datasets.few_shot_dataset import FewShotDataset
+from mir_ml_utils.easyfsl.datasets.default_configs import (
     default_mini_imagenet_loading_transform,
     default_mini_imagenet_serving_transform,
     default_transform,
 )
 
 MINI_IMAGENET_SPECS_DIR = Path("data/mini_imagenet")
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/support_set_folder.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/support_set_folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Union, Callable
 
 import torch
 from torch import Tensor
 from torchvision.datasets import ImageFolder
 
-from src.easyfsl.datasets.default_configs import default_transform
+from mir_ml_utils.easyfsl.datasets.default_configs import default_transform
 
 
 NOT_A_TENSOR_ERROR_MESSAGE = (
     "SupportSetFolder handles instances as tensors. "
     "Please ensure that the specific transform outputs a tensor."
 )
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/datasets/tiered_imagenet.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/datasets/cub.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from pathlib import Path
 
-from src.easyfsl.datasets.easy_set import EasySet
-from src.easyfsl.datasets.few_shot_dataset import FewShotDataset
+from mir_ml_utils.easyfsl.datasets.easy_set import EasySet
+from mir_ml_utils.easyfsl.datasets.few_shot_dataset import FewShotDataset
 
-TIERED_IMAGENET_SPECS_DIR = Path("data/tiered_imagenet")
+CUB_SPECS_DIR = Path("data/CUB")
 
 
 # pylint: disable=invalid-name
-def TieredImageNet(split: str, **kwargs) -> FewShotDataset:
+def CUB(split: str, **kwargs) -> FewShotDataset:
     """
-    Build the tieredImageNet dataset for the specific split.
+    Build the CUB dataset for the specific split.
     Args:
         split: one of the available split (typically train, val, test).
 
     Returns:
         the constructed dataset using EasySet
 
     Raises:
         ValueError: if the specified split cannot be associated with a JSON spec file
-            from tieredImageNet's specs directory
+            from CUB's specs directory
     """
-    specs_file = TIERED_IMAGENET_SPECS_DIR / f"{split}.json"
+    specs_file = CUB_SPECS_DIR / f"{split}.json"
     if specs_file.is_file():
         return EasySet(specs_file=specs_file, **kwargs)
 
-    raise ValueError(
-        f"Could not find specs file {specs_file.name} in {TIERED_IMAGENET_SPECS_DIR}"
-    )
+    raise ValueError(f"Could not find specs file {specs_file.name} in {CUB_SPECS_DIR}")
 
 
 # pylint: enable=invalid-name
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/bd_cspn.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/bd_cspn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from torch import Tensor, nn
 
-from src.easyfsl.methods.few_shot_classifier import FewShotClassifier
+from mir_ml_utils.easyfsl.methods.few_shot_classifier import FewShotClassifier
 
 
 class BDCSPN(FewShotClassifier):
 
     """
     Jinlu Liu, Liang Song, Yongqiang Qin
     "Prototype Rectification for Few-Shot Learning" (ECCV 2020)
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/few_shot_classifier.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/few_shot_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import abstractmethod
 
 import torch
 from torch import nn, Tensor
 
-from src.easyfsl.utils import compute_backbone_output_shape, compute_prototypes
+from mir_ml_utils.easyfsl.utils import compute_backbone_output_shape, compute_prototypes
 
 
 class FewShotClassifier(nn.Module):
     """
     Abstract class providing methods usable by all few-shot classification algorithms
     """
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/finetune.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/finetune.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 from torch import Tensor, nn
 
 
-from src.easyfsl.methods.few_shot_classifier import FewShotClassifier
+from mir_ml_utils.easyfsl.methods.few_shot_classifier import FewShotClassifier
 
 
 class Finetune(FewShotClassifier):
     """
     Wei-Yu Chen, Yen-Cheng Liu, Zsolt Kira, Yu-Chiang Frank Wang, Jia-Bin Huang
     A Closer Look at Few-shot Classification (ICLR 2019)
     https://arxiv.org/abs/1904.04232
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/matching_networks.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/matching_networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 See original implementation at
 https://github.com/facebookresearch/low-shot-shrink-hallucinate
 """
 
 import torch
 from torch import nn, Tensor
-from src.easyfsl.methods.few_shot_classifier import FewShotClassifier
-from src.easyfsl.modules.predesigned_modules import (
+from mir_ml_utils.easyfsl.methods.few_shot_classifier import FewShotClassifier
+from mir_ml_utils.easyfsl.modules.predesigned_modules import (
     default_matching_networks_support_encoder,
     default_matching_networks_query_encoder,
 )
 
 
 class MatchingNetworks(FewShotClassifier):
     """
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/prototypical_networks.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/prototypical_networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from typing import List
 import torch
 from torch import Tensor
 import torch.nn as nn
 from tqdm import tqdm
 
-from src.easyfsl.methods.few_shot_classifier import FewShotClassifier
-from src.easyfsl.utils import compute_prototypes
-from src.loss_functions.loss_function_wrapper import LossFunctionWrapper
+from mir_ml_utils.easyfsl.methods.few_shot_classifier import FewShotClassifier
+from mir_ml_utils.easyfsl.utils import compute_prototypes
+from mir_ml_utils.loss_functions.loss_function_wrapper import LossFunctionWrapper
 
 
 class PrototypicalNetworks(FewShotClassifier):
     """
     Jake Snell, Kevin Swersky, and Richard S. Zemel.
     "Prototypical networks for few-shot learning." (2017)
     https://arxiv.org/abs/1703.05175
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/relation_networks.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/relation_networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 See original implementation at
 https://github.com/floodsung/LearningToCompare_FSL
 """
 
 import torch
 from torch import nn, Tensor
-from src.easyfsl.methods.few_shot_classifier import FewShotClassifier
-from src.easyfsl.modules.predesigned_modules import default_relation_module
-from src.easyfsl.utils import compute_prototypes
+from mir_ml_utils.easyfsl.methods.few_shot_classifier import FewShotClassifier
+from mir_ml_utils.easyfsl.modules.predesigned_modules import default_relation_module
+from mir_ml_utils.easyfsl.utils import compute_prototypes
 
 
 class RelationNetworks(FewShotClassifier):
     """
     Sung, Flood, Yongxin Yang, Li Zhang, Tao Xiang, Philip HS Torr, and Timothy M. Hospedales.
     "Learning to compare: Relation network for few-shot learning." (2018)
     https://openaccess.thecvf.com/content_cvpr_2018/papers/Sung_Learning_to_Compare_CVPR_2018_paper.pdf
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/tim.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/tim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 from torch import Tensor, nn
 
-from src.easyfsl.methods.few_shot_classifier import FewShotClassifier
+from mir_ml_utils.easyfsl.methods.few_shot_classifier import FewShotClassifier
 
 
 class TIM(FewShotClassifier):
     """
     Malik Boudiaf, Ziko Imtiaz Masud, Jérôme Rony, José Dolz, Pablo Piantanida, Ismail Ben Ayed.
     "Transductive Information Maximization For Few-Shot Learning" (NeurIPS 2020)
     https://arxiv.org/abs/2008.11297
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/transductive_finetuning.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/transductive_finetuning.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 from torch import Tensor, nn
 
 
-from src.easyfsl.methods.few_shot_classifier import FewShotClassifier
-from src.easyfsl.utils import entropy
+from mir_ml_utils.easyfsl.methods.few_shot_classifier import FewShotClassifier
+from mir_ml_utils.easyfsl.utils import entropy
 
 
 class TransductiveFinetuning(FewShotClassifier):
     """
     Guneet S. Dhillon, Pratik Chaudhari, Avinash Ravichandran, Stefano Soatto.
     "A Baseline for Few-Shot Image Classification" (ICLR 2020)
     https://arxiv.org/abs/1909.02729
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/methods/utils.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/methods/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 from torch import Tensor
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
-from src.easyfsl.methods.few_shot_classifier import FewShotClassifier
+from mir_ml_utils.easyfsl.methods.few_shot_classifier import FewShotClassifier
 
 
 def evaluate_on_one_task(
     model: FewShotClassifier,
     support_images: Tensor,
     support_labels: Tensor,
     query_images: Tensor,
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/modules/predesigned_modules.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/modules/predesigned_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from torch import nn
 from torchvision.models.resnet import BasicBlock, Bottleneck
 
-from src.easyfsl.modules.resnet import ResNet
+from mir_ml_utils.easyfsl.modules.resnet import ResNet
 
 __all__ = [
     "resnet10",
     "resnet12",
     "resnet18",
     "resnet34",
     "resnet50",
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/modules/resnet.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/easyfsl/samplers/task_sampler.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/easyfsl/samplers/task_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 from typing import List, Tuple, Iterator
 
 import torch
 from torch import Tensor
 from torch.utils.data import Sampler
 
-from src.easyfsl.datasets.few_shot_dataset import FewShotDataset
+from mir_ml_utils.easyfsl.datasets.few_shot_dataset import FewShotDataset
 
 
 class TaskSampler(Sampler):
     """
     Samples batches in the shape of few-shot classification tasks. At each iteration, it will sample
     n_way classes, and then sample support and query images from these classes.
     Note that this class does not accept the batch size. This can be controlled
```

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/factories/model_adaptor_factory.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/factories/model_adaptor_factory.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/factories/model_builder_factory.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/factories/model_builder_factory.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/factories/optimzer_factory.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/factories/optimzer_factory.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/plot_optical_flow.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/plot_optical_flow.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/plot_repurposing_annotations.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/plot_repurposing_annotations.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/plot_scripted_tensor_transforms.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/plot_scripted_tensor_transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/plot_transforms.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/plot_transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/plot_video_api.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/plot_video_api.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/plot_visualization_utils.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/plot_visualization_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054.png` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054_mask.png` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/FudanPed00054_mask.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/astronaut.jpg` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/astronaut.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/basketball.mp4` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/basketball.mp4`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/dog1.jpg` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/dog1.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/dog2.jpg` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/dog2.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/imagenet_class_index.json` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/imagenet_class_index.json`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/person1.jpg` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/person1.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/repurposing_annotations_thumbnail.png` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/repurposing_annotations_thumbnail.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/transforms_thumbnail.png` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/transforms_thumbnail.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/gallery/assets/visualization_utils_thumbnail2.png` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/gallery/assets/visualization_utils_thumbnail2.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/README.md` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/presets.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/presets.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/sampler.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/sampler.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/train.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/train_quantization.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/train_quantization.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/transforms.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/classification/utils.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/classification/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/README.md` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/cascade_evaluation.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/cascade_evaluation.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/parsing.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/parsing.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/presets.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/presets.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/train.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/transforms.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/vizualization.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/vizualization.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/Loss.jpg` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/Loss.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-background-mode-collapse.jpg` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-background-mode-collapse.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-domain-drift.jpg` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/disparity-domain-drift.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/gradient-norm-removal.jpg` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/assets/gradient-norm-removal.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/distributed.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/logger.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/losses.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/losses.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/metrics.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/padder.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/depth/stereo/utils/padder.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/README.md` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/coco_eval.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/coco_eval.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/coco_utils.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/coco_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/engine.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/engine.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/group_by_aspect_ratio.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/group_by_aspect_ratio.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/presets.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/presets.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/train.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/transforms.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/detection/utils.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/detection/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/optical_flow/README.md` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/optical_flow/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/optical_flow/presets.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/optical_flow/presets.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/optical_flow/train.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/optical_flow/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/optical_flow/transforms.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/optical_flow/transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/optical_flow/utils.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/optical_flow/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/README.md` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/coco_utils.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/coco_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/presets.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/presets.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/train.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/transforms.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/transforms.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/segmentation/utils.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/similarity/README.md` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/similarity/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/similarity/loss.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/similarity/loss.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/similarity/sampler.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/similarity/sampler.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/similarity/test.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/similarity/test.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/similarity/train.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/similarity/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/video_classification/README.md` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/video_classification/README.md`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/video_classification/presets.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/video_classification/presets.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/video_classification/train.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/video_classification/train.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/references/video_classification/utils.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/references/video_classification/utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/scripts/README.rst` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/scripts/fbcode_to_main_sync.sh` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/scripts/fbcode_to_main_sync.sh`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/scripts/release_notes/classify_prs.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/scripts/release_notes/classify_prs.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/mir_vision/scripts/release_notes/retrieve_prs_data.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/mir_vision/scripts/release_notes/retrieve_prs_data.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/models/easyfsl_proto_net_classifier.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/models/easyfsl_proto_net_classifier.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/models/linear_regressor_model_tester.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/models/linear_regressor_model_tester.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/models/model_adaptor.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/models/model_adaptor.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/models/model_adaptor_type_enum.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/models/model_adaptor_type_enum.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/models/model_loaders.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/models/model_loaders.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/models/models_enum.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/models/models_enum.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/models/resnet_model_predictor_wrapper.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/models/resnet_model_predictor_wrapper.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/pytorch_util_modules/pytorch_hooks.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/pytorch_util_modules/pytorch_hooks.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/testers/test_wrapper.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/testers/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/testers/two_class_model_tester_wrapper.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/testers/two_class_model_tester_wrapper.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/trainers/pytorch_trainer.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/trainers/pytorch_trainer.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/trainers/trainer_info.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/trainers/trainer_info.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/trainers/trainer_wrapper.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/trainers/trainer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/trainers/trainer_wrapper_pimpl.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/trainers/trainer_wrapper_pimpl.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/utils/array_utils.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/utils/array_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/utils/exceptions.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/utils/file_utils.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/utils/function_wrappers.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/utils/function_wrappers.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/src/mir_ml_utils/utils/math_ops.py` & `mir_ml_utils-0.0.3/src/mir_ml_utils/utils/math_ops.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/testing_data/corrosion_4.png` & `mir_ml_utils-0.0.3/testing_data/corrosion_4.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/testing_data/hull001_label.jpg` & `mir_ml_utils-0.0.3/testing_data/hull001_label.jpg`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/testing_data/prototypical_net_test_data/best_model.pth` & `mir_ml_utils-0.0.3/testing_data/prototypical_net_test_data/best_model.pth`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/testing_data/prototypical_net_test_data/train_prototypes.pth` & `mir_ml_utils-0.0.3/testing_data/prototypical_net_test_data/train_prototypes.pth`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/testing_data/prototypical_net_test_data/inference/corrosion_1.png` & `mir_ml_utils-0.0.3/testing_data/prototypical_net_test_data/inference/corrosion_1.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/testing_data/prototypical_net_test_data/inference/corrosion_2.png` & `mir_ml_utils-0.0.3/testing_data/prototypical_net_test_data/inference/corrosion_2.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/testing_data/prototypical_net_test_data/inference/corrosion_3.png` & `mir_ml_utils-0.0.3/testing_data/prototypical_net_test_data/inference/corrosion_3.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/testing_data/prototypical_net_test_data/inference/corrosion_4.png` & `mir_ml_utils-0.0.3/testing_data/prototypical_net_test_data/inference/corrosion_4.png`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/tests/test_images_dataset.py` & `mir_ml_utils-0.0.3/tests/test_images_dataset.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/tests/test_img_pipeline.py` & `mir_ml_utils-0.0.3/tests/test_img_pipeline.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/tests/test_img_utils.py` & `mir_ml_utils-0.0.3/tests/test_img_utils.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/tests/test_prototypical_loss.py` & `mir_ml_utils-0.0.3/tests/test_prototypical_loss.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/tests/test_pytorch_trainer.py` & `mir_ml_utils-0.0.3/tests/test_pytorch_trainer.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/tests/test_suite.py` & `mir_ml_utils-0.0.3/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/trainer_wrapper_config_template/config.json` & `mir_ml_utils-0.0.3/trainer_wrapper_config_template/config.json`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/.gitignore` & `mir_ml_utils-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/LICENSE` & `mir_ml_utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mir_ml_utils-0.0.2/pyproject.toml` & `mir_ml_utils-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling", "torch", "torchvision", "numpy",
 	    "dataclasses", "Pillow", "matplotlib", "loguru", "opencv-python",
             "torchcam", "torch-summary",  "tqdm", "pycocotools", "navalmartin-mir-vision-utils"]
 build-backend = "hatchling.build"
 [project]
 name = "mir_ml_utils"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Alexandros Giavaras", email="a.giavaras@gmail.com" },
 ]
 description = "Various utilities for machine learning training in Python 3. for the mir project"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `mir_ml_utils-0.0.2/PKG-INFO` & `mir_ml_utils-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,48 @@
 Metadata-Version: 2.1
 Name: mir_ml_utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Various utilities for machine learning training in Python 3. for the mir project
 Project-URL: Homepage, https://github.com/Navalmartin/mir_ml_utils
 Project-URL: Bug Tracker, https://github.com/Navalmartin/mir_ml_utils/issues
 Author-email: Alexandros Giavaras <a.giavaras@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-[![mir (Marine Inspection by Remote)](https://github.com/pockerman/mir/actions/workflows/python-app.yml/badge.svg)](https://github.com/pockerman/mir/actions/workflows/python-app.yml)
 
-# mir-ml-engine
+
+# mir-ml-utils
 
 The ML engine for the mir (Marine Inspection by Remote) app.
 
+## Install
+
+You can install the utilities via ```pip```
+
+```
+pip install mir-ml-utils
+```
+
+For a specific version use
+
+```
+pip install mir-ml-utils==x.x.x
+```
+
+You can uninstall the project via
+
+```
+pip3 uninstall mir-ml-utils
+```
+
+
 ## Dependencies
 
 - PyTorch
 - Numpy
 - Pillow
 - matplolib
 
@@ -37,15 +58,15 @@
 
 - pytest
 - coverage
 - flake8
 
 In order to test locally, you can run the
 
-```commandline
+```
 local_test_pipeline.sh
 ```
 
 The script first runs ```flake8``` and then ```pytest``` with coverage. Finally, it produces
 a report ```coverage_report.txt```.
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: mir_ml_utils Version: 0.0.2 Summary: Various
+Metadata-Version: 2.1 Name: mir_ml_utils Version: 0.0.3 Summary: Various
 utilities for machine learning training in Python 3. for the mir project
 Project-URL: Homepage, https://github.com/Navalmartin/mir_ml_utils Project-URL:
 Bug Tracker, https://github.com/Navalmartin/mir_ml_utils/issues Author-email:
 Alexandros Giavaras
 giavaras@gmail.com> License-File: LICENSE Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-
-Type: text/markdown [![mir (Marine Inspection by Remote)](https://github.com/
-pockerman/mir/actions/workflows/python-app.yml/badge.svg)](https://github.com/
-pockerman/mir/actions/workflows/python-app.yml) # mir-ml-engine The ML engine
-for the mir (Marine Inspection by Remote) app. ## Dependencies - PyTorch -
-Numpy - Pillow - matplolib - sphinx (if you want to build the documentation)
-The project also gets benefited from easyfsl and easy-few-shot-learning.
-However, you don't need to install this as a fork is maintained within mir-
-engine ### Testing There are additional dependencies if you want to run the
-tests - pytest - coverage - flake8 In order to test locally, you can run the
-```commandline local_test_pipeline.sh ``` The script first runs ```flake8```
-and then ```pytest``` with coverage. Finally, it produces a report
-```coverage_report.txt```. ## Installation
+Type: text/markdown # mir-ml-utils The ML engine for the mir (Marine Inspection
+by Remote) app. ## Install You can install the utilities via ```pip``` ``` pip
+install mir-ml-utils ``` For a specific version use ``` pip install mir-ml-
+utils==x.x.x ``` You can uninstall the project via ``` pip3 uninstall mir-ml-
+utils ``` ## Dependencies - PyTorch - Numpy - Pillow - matplolib - sphinx (if
+you want to build the documentation) The project also gets benefited from
+easyfsl and easy-few-shot-learning. However, you don't need to install this as
+a fork is maintained within mir-engine ### Testing There are additional
+dependencies if you want to run the tests - pytest - coverage - flake8 In order
+to test locally, you can run the ``` local_test_pipeline.sh ``` The script
+first runs ```flake8``` and then ```pytest``` with coverage. Finally, it
+produces a report ```coverage_report.txt```. ## Installation
```

