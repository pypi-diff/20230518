# Comparing `tmp/deeplake-3.5.0.tar.gz` & `tmp/deeplake-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.5.0.tar", last modified: Wed May 17 18:24:43 2023, max compression
+gzip compressed data, was "deeplake-3.5.1.tar", last modified: Thu May 18 16:29:42 2023, max compression
```

## Comparing `deeplake-3.5.0.tar` & `deeplake-3.5.1.tar`

### file list

```diff
@@ -1,394 +1,394 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.832152 deeplake-3.5.0/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-05-17 18:22:26.000000 deeplake-3.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-17 18:22:26.000000 deeplake-3.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    25286 2023-05-17 18:24:43.832152 deeplake-3.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24579 2023-05-17 18:22:26.000000 deeplake-3.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.802152 deeplake-3.5.0/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2662 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.802152 deeplake-3.5.0/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94061 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    80238 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    23071 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     6352 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    17730 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7389 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     6666 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    12440 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12937 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19270 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     6262 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   109420 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   170718 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    14805 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11464 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    19800 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    11242 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    15953 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.812152 deeplake-3.5.0/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13344 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    19976 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    22849 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      441 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    19080 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    25667 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    49384 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7404 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    11475 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51192 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    29318 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5860 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/vectorstore/
--rw-r--r--   0 root         (0) root         (0)      509 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11423 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/deeplake_vectorstore.py
--rw-r--r--   0 root         (0) root         (0)     4958 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/test_deeplake_vectorstore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8020 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)     7799 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 root         (0) root         (0)      237 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3147 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 root         (0) root         (0)     3352 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/indra_vector_search.py
--rw-r--r--   0 root         (0) root         (0)     3309 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 root         (0) root         (0)      541 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/remote_engine_search.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 root         (0) root         (0)      275 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      721 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5964 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 root         (0) root         (0)     3703 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 root         (0) root         (0)     2184 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/vectorstore/vector_search/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     3069 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19869 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6781 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    29584 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    25905 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22441 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5463 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.822152 deeplake-3.5.0/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62754 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.832152 deeplake-3.5.0/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9772 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7140 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     6919 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.832152 deeplake-3.5.0/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.832152 deeplake-3.5.0/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.832152 deeplake-3.5.0/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      304 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.832152 deeplake-3.5.0/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     4072 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     3573 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    15328 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.832152 deeplake-3.5.0/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5623 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4477 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4597 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5381 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    34711 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37497 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.832152 deeplake-3.5.0/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4206 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.832152 deeplake-3.5.0/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    25208 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31615 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.832152 deeplake-3.5.0/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-05-17 18:22:26.000000 deeplake-3.5.0/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:24:43.802152 deeplake-3.5.0/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25286 2023-05-17 18:24:43.000000 deeplake-3.5.0/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12524 2023-05-17 18:24:43.000000 deeplake-3.5.0/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 18:24:43.000000 deeplake-3.5.0/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-17 18:24:43.000000 deeplake-3.5.0/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 18:24:43.000000 deeplake-3.5.0/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      978 2023-05-17 18:24:43.000000 deeplake-3.5.0/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-17 18:24:43.000000 deeplake-3.5.0/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-17 18:24:43.842152 deeplake-3.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3289 2023-05-17 18:22:26.000000 deeplake-3.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.413784 deeplake-3.5.1/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-05-18 16:18:26.000000 deeplake-3.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-18 16:18:26.000000 deeplake-3.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    25286 2023-05-18 16:29:42.413784 deeplake-3.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24579 2023-05-18 16:18:26.000000 deeplake-3.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94609 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    80238 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    23071 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     6352 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    17730 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7389 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    12440 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19270 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     6262 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   109420 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   170718 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14805 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11464 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    19800 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    11242 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    15953 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13344 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    19976 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    19080 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25686 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    49384 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7485 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    11475 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51192 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    29318 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5860 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/vectorstore/
+-rw-r--r--   0 root         (0) root         (0)      509 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11517 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/deeplake_vectorstore.py
+-rw-r--r--   0 root         (0) root         (0)     4993 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8071 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     7799 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 root         (0) root         (0)     3352 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/indra_vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     3309 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 root         (0) root         (0)      541 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/remote_engine_search.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      721 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19869 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6781 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    25905 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22441 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5463 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.402951 deeplake-3.5.1/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9772 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.413784 deeplake-3.5.1/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.413784 deeplake-3.5.1/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.413784 deeplake-3.5.1/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      304 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.413784 deeplake-3.5.1/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    15328 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.413784 deeplake-3.5.1/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5623 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4477 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5381 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    34711 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37497 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.413784 deeplake-3.5.1/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.413784 deeplake-3.5.1/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    25208 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31615 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.413784 deeplake-3.5.1/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-05-18 16:18:26.000000 deeplake-3.5.1/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:42.392118 deeplake-3.5.1/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25286 2023-05-18 16:29:42.000000 deeplake-3.5.1/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12524 2023-05-18 16:29:42.000000 deeplake-3.5.1/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 16:29:42.000000 deeplake-3.5.1/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-18 16:29:42.000000 deeplake-3.5.1/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 16:29:42.000000 deeplake-3.5.1/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      978 2023-05-18 16:29:42.000000 deeplake-3.5.1/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-18 16:29:42.000000 deeplake-3.5.1/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-18 16:29:42.413784 deeplake-3.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-05-18 16:18:26.000000 deeplake-3.5.1/setup.py
```

### Comparing `deeplake-3.5.0/LICENSE` & `deeplake-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/PKG-INFO` & `deeplake-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.5.0
+Version: 3.5.1
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.5.0 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.5.1 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
 Provides-Extra: enterprise Provides-Extra: gcp Provides-Extra: gdrive Provides-
```

### Comparing `deeplake-3.5.0/README.md` & `deeplake-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/__init__.py` & `deeplake-3.5.1/deeplake/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.5.0"
+__version__ = "3.5.1"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.5.0/deeplake/api/dataset.py` & `deeplake-3.5.1/deeplake/api/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
         local_cache_size: int = DEFAULT_LOCAL_CACHE_SIZE,
         creds: Optional[Union[Dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         verbose: bool = True,
         access_method: str = "stream",
         reset: bool = False,
+        check_integrity: bool = True,
     ):
         """Returns a :class:`~deeplake.core.dataset.Dataset` object referencing either a new or existing dataset.
 
         Examples:
 
             >>> ds = deeplake.dataset("hub://username/dataset")
             >>> ds = deeplake.dataset("s3://mybucket/my_dataset")
@@ -152,14 +153,15 @@
                         - Downloads the dataset if it doesn't already exist, otherwise loads from local storage.
                         - Raises an exception if ``DEEPLAKE_DOWNLOAD_PATH`` environment variable is not set.
                         - The 'local' access method can be modified to specify num_workers and/or scheduler to be used in case dataset needs to be downloaded.
                           If dataset needs to be downloaded, 'local:2:processed' will use 2 workers and use processed scheduler, while 'local:3' will use 3 workers
                           and default scheduler (threaded), and 'local:processed' will use a single worker and use processed scheduler.
             reset (bool): If the specified dataset cannot be loaded due to a corrupted HEAD state of the branch being loaded,
                           setting ``reset=True`` will reset HEAD changes and load the previous version.
+            check_integrity (bool): If the param is True it will do integrity check during dataset loading otherwise the check is not performed
 
         ..
             # noqa: DAR101
 
         Returns:
             Dataset: Dataset created using the arguments provided.
 
@@ -254,15 +256,17 @@
                     "num_workers": num_workers,
                     "scheduler": scheduler,
                     "reset": reset,
                 }
             )
 
         try:
-            return dataset._load(dataset_kwargs, access_method, create)
+            return dataset._load(
+                dataset_kwargs, access_method, create, check_integrity=check_integrity
+            )
         except (AgreementError, CheckoutError, LockedException) as e:
             raise e from None
         except Exception as e:
             if create:
                 raise e
             if access_method == "stream":
                 if not reset:
@@ -432,14 +436,15 @@
         local_cache_size: int = DEFAULT_LOCAL_CACHE_SIZE,
         creds: Optional[Union[dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         verbose: bool = True,
         access_method: str = "stream",
         reset: bool = False,
+        check_integrity: bool = True,
     ) -> Dataset:
         """Loads an existing dataset
 
         Examples:
 
             >>> ds = deeplake.load("hub://username/dataset")
             >>> ds = deeplake.load("s3://mybucket/my_dataset")
@@ -495,14 +500,15 @@
                         - Downloads the dataset if it doesn't already exist, otherwise loads from local storage.
                         - Raises an exception if ``DEEPLAKE_DOWNLOAD_PATH`` environment variable is not set.
                         - The 'local' access method can be modified to specify num_workers and/or scheduler to be used in case dataset needs to be downloaded.
                           If dataset needs to be downloaded, 'local:2:processed' will use 2 workers and use processed scheduler, while 'local:3' will use 3 workers
                           and default scheduler (threaded), and 'local:processed' will use a single worker and use processed scheduler.
             reset (bool): If the specified dataset cannot be loaded due to a corrupted HEAD state of the branch being loaded,
                           setting ``reset=True`` will reset HEAD changes and load the previous version.
+            check_integrity (bool): If the param is True it will do integrity check during dataset loading otherwise the check is not performed
 
         ..
             # noqa: DAR101
 
         Returns:
             Dataset: Dataset loaded using the arguments provided.
 
@@ -577,15 +583,17 @@
                     "num_workers": num_workers,
                     "scheduler": scheduler,
                     "reset": reset,
                 }
             )
 
         try:
-            return dataset._load(dataset_kwargs, access_method)
+            return dataset._load(
+                dataset_kwargs, access_method, check_integrity=check_integrity
+            )
         except (AgreementError, CheckoutError, LockedException) as e:
             raise e from None
         except Exception as e:
             if access_method == "stream":
                 if not reset:
                     if isinstance(e, DatasetCorruptError):
                         raise DatasetCorruptError(
@@ -644,23 +652,24 @@
         current_node = ds.version_state["commit_node_map"][ds.commit_id]
         verbose = dataset_kwargs.get("verbose")
         if verbose:
             logger.info(f"HEAD reset. Current version:\n{current_node}")
         return ds
 
     @staticmethod
-    def _load(dataset_kwargs, access_method=None, create=False):
+    def _load(dataset_kwargs, access_method=None, create=False, check_integrity=True):
         if access_method in ("stream", None):
             ret = dataset_factory(**dataset_kwargs)
             if create:
                 dataset_created(ret)
             else:
                 dataset_loaded(ret)
 
-            integrity_check(ret)
+            if check_integrity:
+                integrity_check(ret)
 
             verbose = dataset_kwargs.get("verbose")
             path = dataset_kwargs.get("path")
             if verbose:
                 logger.info(f"{path} loaded successfully.")
         else:
             ret = get_local_dataset(**dataset_kwargs)
```

### Comparing `deeplake-3.5.0/deeplake/api/info.py` & `deeplake-3.5.1/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/link.py` & `deeplake-3.5.1/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/link_tiled.py` & `deeplake-3.5.1/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/read.py` & `deeplake-3.5.1/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_access_method.py` & `deeplake-3.5.1/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_agreement.py` & `deeplake-3.5.1/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_api.py` & `deeplake-3.5.1/deeplake/api/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.5.1/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.5.1/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.5.1/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.5.1/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_dataset.py` & `deeplake-3.5.1/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_dicom.py` & `deeplake-3.5.1/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_downsample.py` & `deeplake-3.5.1/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_events.py` & `deeplake-3.5.1/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_grayscale.py` & `deeplake-3.5.1/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_info.py` & `deeplake-3.5.1/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.5.1/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_json.py` & `deeplake-3.5.1/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_link.py` & `deeplake-3.5.1/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.5.1/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_linking.py` & `deeplake-3.5.1/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_mesh.py` & `deeplake-3.5.1/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_meta.py` & `deeplake-3.5.1/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_nifti.py` & `deeplake-3.5.1/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_none.py` & `deeplake-3.5.1/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.5.1/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_pickle.py` & `deeplake-3.5.1/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.5.1/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_polygons.py` & `deeplake-3.5.1/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_pop.py` & `deeplake-3.5.1/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_readonly.py` & `deeplake-3.5.1/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_rechunk.py` & `deeplake-3.5.1/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_reset.py` & `deeplake-3.5.1/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_sample_info.py` & `deeplake-3.5.1/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_text.py` & `deeplake-3.5.1/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_update_samples.py` & `deeplake-3.5.1/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_video.py` & `deeplake-3.5.1/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tests/test_views.py` & `deeplake-3.5.1/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/api/tiled.py` & `deeplake-3.5.1/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/structured/base.py` & `deeplake-3.5.1/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/structured/dataframe.py` & `deeplake-3.5.1/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.5.1/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.5.1/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.5.1/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.5.1/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/unstructured/base.py` & `deeplake-3.5.1/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.5.1/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.5.1/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.5.1/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.5.1/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.5.1/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.5.1/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/unstructured/util.py` & `deeplake-3.5.1/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.5.1/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.5.1/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/cli/auth.py` & `deeplake-3.5.1/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/cli/test_cli.py` & `deeplake-3.5.1/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/client/client.py` & `deeplake-3.5.1/deeplake/client/client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/client/config.py` & `deeplake-3.5.1/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/client/log.py` & `deeplake-3.5.1/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/client/test_client.py` & `deeplake-3.5.1/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/client/utils.py` & `deeplake-3.5.1/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/compression.py` & `deeplake-3.5.1/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/constants.py` & `deeplake-3.5.1/deeplake/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/chunk/base_chunk.py` & `deeplake-3.5.1/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.5.1/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.5.1/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.5.1/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.5.1/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.5.1/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.5.1/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/chunk_engine.py` & `deeplake-3.5.1/deeplake/core/chunk_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -2535,15 +2535,15 @@
                 if self.tensor_meta.htype in ("text", "json"):
                     shape = (1,)
                 else:
                     if sample_shape_provider:
                         try:
                             shape = sample_shape_provider(idx)  # type: ignore
                             if isinstance(shape, tuple) and shape == ():
-                                shape = (1,)
+                                shape = (0,)
                             if self.is_sequence:
                                 if sample_index and not sample_index[0].subscriptable():
                                     shape = (1, *tuple(shape[sample_index[0].value].tolist()))  # type: ignore
                                 else:
                                     is_same = np.all(shape == shape[0, :], axis=0)  # type: ignore
                                     shape = (len(shape),) + (
                                         tuple(
```

### Comparing `deeplake-3.5.0/deeplake/core/compression.py` & `deeplake-3.5.1/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/compute/process.py` & `deeplake-3.5.1/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/compute/provider.py` & `deeplake-3.5.1/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/compute/ray.py` & `deeplake-3.5.1/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/compute/serial.py` & `deeplake-3.5.1/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/compute/thread.py` & `deeplake-3.5.1/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/dataset/__init__.py` & `deeplake-3.5.1/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/dataset/dataset.py` & `deeplake-3.5.1/deeplake/core/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.5.1/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.5.1/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.5.1/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/dataset/invalid_view.py` & `deeplake-3.5.1/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/dataset/view_entry.py` & `deeplake-3.5.1/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/fast_forwarding.py` & `deeplake-3.5.1/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/index/index.py` & `deeplake-3.5.1/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/io.py` & `deeplake-3.5.1/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/ipc.py` & `deeplake-3.5.1/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/link_creds.py` & `deeplake-3.5.1/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/linked_chunk_engine.py` & `deeplake-3.5.1/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/linked_sample.py` & `deeplake-3.5.1/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/linked_tiled_sample.py` & `deeplake-3.5.1/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/lock.py` & `deeplake-3.5.1/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/dataset_meta.py` & `deeplake-3.5.1/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.5.1/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.5.1/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.5.1/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/creds.py` & `deeplake-3.5.1/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/pad.py` & `deeplake-3.5.1/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/sequence.py` & `deeplake-3.5.1/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/shape.py` & `deeplake-3.5.1/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.5.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.5.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.5.1/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.5.1/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.5.1/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/encode/tile.py` & `deeplake-3.5.1/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/meta/tensor_meta.py` & `deeplake-3.5.1/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/partial_reader.py` & `deeplake-3.5.1/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/partial_sample.py` & `deeplake-3.5.1/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/polygon.py` & `deeplake-3.5.1/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/query/autocomplete.py` & `deeplake-3.5.1/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/query/filter.py` & `deeplake-3.5.1/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/query/query.py` & `deeplake-3.5.1/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/sample.py` & `deeplake-3.5.1/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/serialize.py` & `deeplake-3.5.1/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.5.1/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/storage/gcs.py` & `deeplake-3.5.1/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/storage/google_drive.py` & `deeplake-3.5.1/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/storage/local.py` & `deeplake-3.5.1/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/storage/lru_cache.py` & `deeplake-3.5.1/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/storage/memory.py` & `deeplake-3.5.1/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/storage/provider.py` & `deeplake-3.5.1/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/storage/s3.py` & `deeplake-3.5.1/deeplake/core/storage/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import deeplake
 from math import ceil
 import time
 import boto3
 import botocore  # type: ignore
 import posixpath
 from typing import Dict, Optional, Tuple, Type
-from datetime import datetime
+from datetime import datetime, timezone
 from botocore.session import ComponentLocator
 from deeplake.client.client import DeepLakeBackendClient
 from deeplake.core.storage.provider import StorageProvider
 from deeplake.util.exceptions import (
     S3GetAccessError,
     S3DeletionError,
     S3GetError,
@@ -502,15 +502,15 @@
         self._set_s3_client_and_resource()
 
     def _check_update_creds(self, force=False):
         """If the client has an expiration time, check if creds are expired and fetch new ones.
         This would only happen for datasets stored on Deep Lake storage for which temporary 12 hour credentials are generated.
         """
         if self.expiration and (
-            force or float(self.expiration) < datetime.utcnow().timestamp()
+            force or float(self.expiration) < datetime.now(timezone.utc).timestamp()
         ):
             client = DeepLakeBackendClient(self.token)
             org_id, ds_name = self.tag.split("/")
 
             mode = "r" if self.read_only else "a"
 
             url, creds, mode, expiration, repo = client.get_dataset_credentials(
```

### Comparing `deeplake-3.5.0/deeplake/core/tensor.py` & `deeplake-3.5.1/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tensor_link.py` & `deeplake-3.5.1/deeplake/core/tensor_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,17 @@
 def update_shape(new_sample, link_creds=None, tensor_meta=None):
     if new_sample is None:
         return np.zeros(1, dtype=np.int64)
     if isinstance(new_sample, deeplake.core.linked_sample.LinkedSample):
         new_sample = read_linked_sample(
             new_sample.path, new_sample.creds_key, link_creds, verify=False
         )
-    if np.isscalar(new_sample):
+    if np.isscalar(new_sample) or (
+        isinstance(new_sample, np.ndarray) and new_sample.shape == ()
+    ):
         ret = np.array([1], dtype=np.int64)
     else:
         ret = np.array(
             getattr(new_sample, "shape", None) or np.array(new_sample).shape,
             dtype=np.int64,
         )
```

### Comparing `deeplake-3.5.0/deeplake/core/test_serialize.py` & `deeplake-3.5.1/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tests/test_compression.py` & `deeplake-3.5.1/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tests/test_compute.py` & `deeplake-3.5.1/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.5.1/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tests/test_io.py` & `deeplake-3.5.1/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tests/test_locking.py` & `deeplake-3.5.1/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tests/test_readonly.py` & `deeplake-3.5.1/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tests/test_serialize.py` & `deeplake-3.5.1/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tiling/deserialize.py` & `deeplake-3.5.1/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tiling/optimizer.py` & `deeplake-3.5.1/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.5.1/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tiling/serialize.py` & `deeplake-3.5.1/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.5.1/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/tiling/test_serialize.py` & `deeplake-3.5.1/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/transform/test_transform.py` & `deeplake-3.5.1/deeplake/core/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/transform/transform.py` & `deeplake-3.5.1/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/transform/transform_dataset.py` & `deeplake-3.5.1/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/transform/transform_tensor.py` & `deeplake-3.5.1/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/deeplake_vectorstore.py` & `deeplake-3.5.1/deeplake/core/vectorstore/deeplake_vectorstore.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,24 +65,24 @@
         self.verbose = verbose
 
     def add(
         self,
         texts: Iterable[str],
         metadatas: Optional[List[dict]] = None,
         ids: Optional[List[str]] = None,
-        embeddings: Optional[np.ndarray] = None,
+        embeddings: Optional[Union[List[float], np.ndarray]] = None,
         total_samples_processed: int = 0,
     ) -> List[str]:
         """Adding elements to deeplake vector store
 
         Args:
             texts (Iterable[str]): texts to add to deeplake vector store
             metadatas (List[dict], optional): List of metadatas. Defaults to None.
             ids (List[str], optional): List of document IDs. Defaults to None.
-            embeddings (np.ndarray, optional): embedding of texts. Defaults to None.
+            embeddings (Union[List[float], np.ndarray], optional): embedding of texts. Defaults to None.
             total_samples_processed (int): Total number of samples processed before transforms stopped.
 
         Returns:
             List[str]: List of document IDs
         """
         elements, ids = dataset_utils.create_elements(
             ids=ids, texts=texts, metadatas=metadatas, embeddings=embeddings
@@ -102,25 +102,25 @@
         if self.verbose:
             self.dataset.summary()
         return ids
 
     def search(
         self,
         query: Optional[str] = None,
-        embedding: Optional[np.ndarray] = None,
+        embedding: Optional[Union[List[float], np.ndarray]] = None,
         k: int = 4,
         distance_metric: str = "L2",
         filter: Optional[Any] = None,
         exec_option: Optional[str] = None,
     ):
         """DeepLakeVectorStore search method
 
         Args:
             query (str, optional): String representation of the query to run. Defaults to None.
-            embedding (Optional[np.ndarray, optional): Embedding representation of the query to run. Defaults to None.
+            embedding (Union[np.ndarray, List[float]], optional): Embedding representation of the query to run. Defaults to None.
             k (int): Number of elements to return after running query. Defaults to 4.
             distance_metric (str): Type of distance metric to use for sorting the data. Avaliable options are: "L1", "L2", "COS", "MAX". Defaults to "L2".
             filter (Any, optional): Metadata dictionary for exact search. Defaults to None.
             exec_option (str, optional): Type of query execution. It could be either "python", "compute_engine" or "tensor_db". Defaults to "python".
                 - ``python`` - runs on the client and can be used for any data stored anywhere. WARNING: using this option with big datasets is discouraged, because it can lead to some memory issues.
                 - ``compute_engine`` - runs on the client and can be used for any data stored in or connected to Deep Lake.
                 - ``tensor_db`` - runs on the Deep Lake Managed Database and can be used for any data stored in the Deep Lake Managed.
@@ -158,15 +158,15 @@
         distance_metric: str = "L2",
     ):
         """Internal DeepLakeVectorStore search method
 
         Args:
             view (DeepLakeDataset): DeepLakeDataset object to run query inside.
             query (Optional[str], optional): String representation of the query to run. Defaults to None.
-            embedding (Optional[Union[List[float], np.ndarray]], optional): Embedding representation of the query to run. Defaults to None.
+            embedding (Union[List[float], np.ndarray], optional): Embedding representation of the query to run. Defaults to None.
             k (int): Number of elements to return after running query. Defaults to 4.
             distance_metric (str): Type of distance metric to use for sorting the data. Avaliable options are: "L1", "L2", "COS", "MAX". Defaults to "L2".
             exec_option (str): Type of query execution. It could be either "python", "compute_engine" or "tensor_db".
                 - ``python`` - Pure-python implementation that runs on the client and can be used for data stored anywhere. WARNING: using this option with big datasets is discouraged because it can lead to memory issues.
                 - ``compute_engine`` - C++ implementation of the Deep Lake Compute Engine that runs on the client and can be used for any data stored in or connected to Deep Lake. It cannot be used with in-memory or local data.
                 - ``tensor_db`` - Fully-hosted Managed Database that is responsible for storage and query execution. Only available for data stored in the Deep Lake Managed Database. This is achieved by specifying runtime = {"tensor_db": True} during dataset creation.
 
@@ -188,14 +188,15 @@
                 query_embedding=query_emb,
                 embedding=embeddings,
                 k=k,
                 distance_metric=distance_metric.lower(),
                 exec_option=exec_option,
                 deeplake_dataset=self.dataset,
             )
+            view = view[indices]
         return (view, indices, scores)
 
     def delete(
         self,
         ids: Optional[List[str]] = None,
         filter: Optional[Dict[str, str]] = None,
         delete_all: Optional[bool] = None,
```

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/test_deeplake_vectorstore.py` & `deeplake-3.5.1/deeplake/core/vectorstore/test_deeplake_vectorstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     k = 4
     query_embedding = np.random.randint(0, 255, (1, embedding_dim))
 
     # initialize vector store object:
     vector_store = DeepLakeVectorStore(
         dataset_path="./deeplake_vector_store",
         overwrite=True,
+        token=hub_cloud_dev_token,
     )
 
     # add data to the dataset:
     vector_store.add(embeddings=embeddings, texts=texts)
 
     # use python implementation to search the data
     python_view, python_indices, python_scores = vector_store.search(
```

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,15 +208,15 @@
             )
 
     if embedding_function is not None:
         if embedding is not None:
             always_warn("both embedding and embedding_function are specified. ")
         embedding = embedding_function(query)  # type: ignore
 
-    if embedding.dtype != "float32":
+    if isinstance(embedding, list) or embedding.dtype != "float32":
         embedding = np.array(embedding, dtype=np.float32)
 
     return embedding
 
 
 def preprocess_tensors(ids, texts, metadatas, embeddings):
     if ids is None:
@@ -241,15 +241,15 @@
     return processed_tensors, ids
 
 
 def create_elements(
     texts: Iterable[str],
     ids: Optional[List[str]] = None,
     metadatas: Optional[List[dict]] = None,
-    embeddings: Optional[np.ndarray] = None,
+    embeddings: Optional[Union[List[float], np.ndarray]] = None,
 ):
     processed_tensors, ids = preprocess_tensors(ids, texts, metadatas, embeddings)
     utils.check_length_of_each_tensor(processed_tensors)
 
     elements = [
         {
             "text": processed_tensors["texts"][i],
```

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/indra_vector_search.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/indra_vector_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 from typing import Union, List, Any, Optional, Tuple
 
+from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
+
 from deeplake.core.vectorstore.vector_search.indra import query
 from deeplake.core.vectorstore.vector_search import utils
 from deeplake.core.dataset import Dataset as DeepLakeDataset
 
 
 def vector_search(
     query_embedding: np.ndarray,
@@ -26,14 +28,14 @@
 
     Returns:
         Tuple[List, List]: tuple representing the indices of the returned embeddings and their respective scores.
     """
     from indra import api  # type: ignore
 
     tql_query = query.parse_query(distance_metric, k, query_embedding, embedding_tensor)
-    indra_ds = api.dataset(deeplake_dataset.path)
+    indra_ds = dataset_to_libdeeplake(deeplake_dataset)
 
     view = indra_ds.query(tql_query)
     indices = view.indexes
 
     scores = view.score.numpy()
     return indices, scores
```

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/remote_engine_search.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/remote_engine_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/python/vector_search.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/utils.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.5.1/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.5.1/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/version_control/commit_diff.py` & `deeplake-3.5.1/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/version_control/commit_node.py` & `deeplake-3.5.1/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.5.1/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/version_control/test_merge.py` & `deeplake-3.5.1/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/core/version_control/test_version_control.py` & `deeplake-3.5.1/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.5.1/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/enterprise/dataloader.py` & `deeplake-3.5.1/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.5.1/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.5.1/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/enterprise/test_pytorch.py` & `deeplake-3.5.1/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/enterprise/test_query.py` & `deeplake-3.5.1/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.5.1/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/enterprise/util.py` & `deeplake-3.5.1/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/hooks.py` & `deeplake-3.5.1/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/htype.py` & `deeplake-3.5.1/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.5.1/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.5.1/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.5.1/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.5.1/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/integrations/pytorch/common.py` & `deeplake-3.5.1/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.5.1/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.5.1/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.5.1/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/integrations/tf/common.py` & `deeplake-3.5.1/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.5.1/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.5.1/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/integrations/wandb/wandb.py` & `deeplake-3.5.1/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/tests/cache_fixtures.py` & `deeplake-3.5.1/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/tests/client_fixtures.py` & `deeplake-3.5.1/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/tests/common.py` & `deeplake-3.5.1/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/tests/dataset_fixtures.py` & `deeplake-3.5.1/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/tests/path_fixtures.py` & `deeplake-3.5.1/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/tests/storage_fixtures.py` & `deeplake-3.5.1/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/access_method.py` & `deeplake-3.5.1/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/agreement.py` & `deeplake-3.5.1/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/array_list.py` & `deeplake-3.5.1/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/assert_byte_indexes.py` & `deeplake-3.5.1/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/auto.py` & `deeplake-3.5.1/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/bugout_reporter.py` & `deeplake-3.5.1/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/cache_chain.py` & `deeplake-3.5.1/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/casting.py` & `deeplake-3.5.1/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/check_latest_version.py` & `deeplake-3.5.1/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/chunk_engine.py` & `deeplake-3.5.1/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/class_label.py` & `deeplake-3.5.1/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/compute.py` & `deeplake-3.5.1/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/connect_dataset.py` & `deeplake-3.5.1/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/dataset.py` & `deeplake-3.5.1/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/diff.py` & `deeplake-3.5.1/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/downsample.py` & `deeplake-3.5.1/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/encoder.py` & `deeplake-3.5.1/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/exceptions.py` & `deeplake-3.5.1/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/exif.py` & `deeplake-3.5.1/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/from_tfds.py` & `deeplake-3.5.1/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/htype.py` & `deeplake-3.5.1/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/image.py` & `deeplake-3.5.1/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/invalid_view_op.py` & `deeplake-3.5.1/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/iteration_warning.py` & `deeplake-3.5.1/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/json.py` & `deeplake-3.5.1/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/keys.py` & `deeplake-3.5.1/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/link.py` & `deeplake-3.5.1/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/logging.py` & `deeplake-3.5.1/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/merge.py` & `deeplake-3.5.1/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/modified.py` & `deeplake-3.5.1/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/notebook.py` & `deeplake-3.5.1/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/object_3d/mesh.py` & `deeplake-3.5.1/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.5.1/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.5.1/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.5.1/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.5.1/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.5.1/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.5.1/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.5.1/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.5.1/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.5.1/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/path.py` & `deeplake-3.5.1/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/pretty_print.py` & `deeplake-3.5.1/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/remove_cache.py` & `deeplake-3.5.1/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/scheduling.py` & `deeplake-3.5.1/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/shape_interval.py` & `deeplake-3.5.1/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/spinner.py` & `deeplake-3.5.1/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/split.py` & `deeplake-3.5.1/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/storage.py` & `deeplake-3.5.1/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/tag.py` & `deeplake-3.5.1/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/testing.py` & `deeplake-3.5.1/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/tests/test_auto.py` & `deeplake-3.5.1/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.5.1/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.5.1/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/tests/test_read.py` & `deeplake-3.5.1/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.5.1/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/tests/test_split.py` & `deeplake-3.5.1/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/tests/test_version_control.py` & `deeplake-3.5.1/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/transform.py` & `deeplake-3.5.1/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/version_control.py` & `deeplake-3.5.1/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/util/video.py` & `deeplake-3.5.1/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/visualizer/video_streaming.py` & `deeplake-3.5.1/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake/visualizer/visualizer.py` & `deeplake-3.5.1/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake.egg-info/PKG-INFO` & `deeplake-3.5.1/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.5.0
+Version: 3.5.1
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.5.0 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.5.1 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
 Provides-Extra: enterprise Provides-Extra: gcp Provides-Extra: gdrive Provides-
```

### Comparing `deeplake-3.5.0/deeplake.egg-info/SOURCES.txt` & `deeplake-3.5.1/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/deeplake.egg-info/requires.txt` & `deeplake-3.5.1/deeplake.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.0/setup.py` & `deeplake-3.5.1/setup.py`

 * *Files identical despite different names*

