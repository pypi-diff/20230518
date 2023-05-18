# Comparing `tmp/funasr-0.5.2.tar.gz` & `tmp/funasr-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.5.2.tar", last modified: Thu May 18 03:24:35 2023, max compression
+gzip compressed data, was "funasr-0.5.3.tar", last modified: Thu May 18 03:46:27 2023, max compression
```

## Comparing `funasr-0.5.2.tar` & `funasr-0.5.3.tar`

### file list

```diff
@@ -1,426 +1,426 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.576406 funasr-0.5.2/
--rw-r--r--   0 zhifu      (502) staff       (20)     1063 2023-02-07 07:13:38.000000 funasr-0.5.2/LICENSE
--rw-r--r--   0 zhifu      (502) staff       (20)     8468 2023-05-18 03:24:35.576094 funasr-0.5.2/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     7446 2023-05-18 02:19:50.000000 funasr-0.5.2/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.393138 funasr-0.5.2/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.409180 funasr-0.5.2/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21913 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/asr_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11106 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/asr_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    25965 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/asr_inference_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40504 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/asr_inference_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26713 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/asr_inference_paraformer_streaming.py
--rw-r--r--   0 zhifu      (502) staff       (20)    24956 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/asr_inference_rnnt.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23949 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/asr_inference_uniasr.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1068 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1027 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/asr_train_paraformer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1036 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/asr_train_transducer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1024 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/asr_train_uniasr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5382 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-18 02:19:38.000000 funasr-0.5.2/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5327 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1010 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/diar_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    14137 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/eend_ola_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     6814 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/lm_calc_perplexity.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14544 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/lm_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3816 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1019 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/lm_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3049 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/modelscope_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3593 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/punc_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11940 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/punctuation_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11101 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/punctuation_infer_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23328 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/sa_asr_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1071 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/sa_asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20700 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/sond_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    14841 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/sv_inference.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     4718 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.5.2/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13304 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/tp_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3874 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/tp_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19679 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/vad_inference.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4282 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/vad_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11618 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/bin/vad_inference_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.411927 funasr-0.5.2/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.5.2/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.5.2/funasr/datasets/iterable_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12671 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/datasets/iterable_dataset_modelscope.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.413345 funasr-0.5.2/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3488 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.414770 funasr-0.5.2/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.5.2/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9294 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.417614 funasr-0.5.2/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.5.2/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.5.2/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.5.2/funasr/datasets/large_datasets/utils/hotword_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.5.2/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2583 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-18 02:19:38.000000 funasr-0.5.2/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.5.2/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.418041 funasr-0.5.2/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.2/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10699 2023-05-12 02:41:22.000000 funasr-0.5.2/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.426028 funasr-0.5.2/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.5.2/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.435100 funasr-0.5.2/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.2/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.5.2/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.5.2/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.437260 funasr-0.5.2/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.2/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.5.2/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.5.2/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.439709 funasr-0.5.2/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.2/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.5.2/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.5.2/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.5.2/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.440388 funasr-0.5.2/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.2/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.5.2/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.442655 funasr-0.5.2/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      966 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.443067 funasr-0.5.2/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.2/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.5.2/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.444738 funasr-0.5.2/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3539 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.446150 funasr-0.5.2/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.449716 funasr-0.5.2/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      359 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3503 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      349 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.5.2/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.450906 funasr-0.5.2/funasr/lm/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/lm/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5436 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/lm/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5904 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/lm/seq_rnn_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4243 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/lm/transformer_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.451408 funasr-0.5.2/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.5.2/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.453037 funasr-0.5.2/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5610 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5029 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.460240 funasr-0.5.2/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.5.2/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5298 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.466102 funasr-0.5.2/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.5.2/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75199 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.5.2/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16707 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.5.2/funasr/models/e2e_asr_contextual_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11630 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)    74013 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    34796 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10238 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20581 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19501 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/e2e_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10098 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6710 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51737 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31100 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.472749 funasr-0.5.2/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      503 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43608 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20993 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.5.2/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.5.2/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.5.2/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17514 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.475058 funasr-0.5.2/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.5.2/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.5.2/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.5.2/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41077 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3634 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    54458 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.477890 funasr-0.5.2/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      400 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9106 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5759 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4990 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20471 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6322 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2817 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.478912 funasr-0.5.2/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.5.2/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.5.2/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.479805 funasr-0.5.2/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.5.2/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.481221 funasr-0.5.2/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.481804 funasr-0.5.2/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35684 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.482804 funasr-0.5.2/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/preencoder/sinc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.483455 funasr-0.5.2/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4661 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4715 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.490409 funasr-0.5.2/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.5.2/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.492104 funasr-0.5.2/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/beam_search/beam_search.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-09 03:02:42.000000 funasr-0.5.2/funasr/modules/beam_search/beam_search_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.5.2/funasr/modules/beam_search/beam_search_transducer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.495849 funasr-0.5.2/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.5.2/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.498463 funasr-0.5.2/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.5.2/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/modules/eend_ola/encoder_decoder_attractor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.5.2/funasr/modules/embedding.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.500657 funasr-0.5.2/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.5.2/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.5.2/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.5.2/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.5.2/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.503305 funasr-0.5.2/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.505633 funasr-0.5.2/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.506911 funasr-0.5.2/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21441 2023-04-25 03:22:30.000000 funasr-0.5.2/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.507772 funasr-0.5.2/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.5.2/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.508028 funasr-0.5.2/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.2/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.508188 funasr-0.5.2/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.2/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.509189 funasr-0.5.2/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.5.2/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.509960 funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.511831 funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.514441 funasr-0.5.2/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.520179 funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13093 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.529517 funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1580 2023-05-12 03:39:34.000000 funasr-0.5.2/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.532205 funasr-0.5.2/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.533350 funasr-0.5.2/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.5.2/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.536527 funasr-0.5.2/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    74340 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    60814 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.5.2/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32463 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6782 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8029 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21378 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/tasks/sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18814 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12527 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.538932 funasr-0.5.2/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.545041 funasr-0.5.2/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.5.2/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.547092 funasr-0.5.2/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1764 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/train/abs_espnet_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7280 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.5.2/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    37188 2023-05-18 03:24:03.000000 funasr-0.5.2/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.573300 funasr-0.5.2/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.5.2/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.5.2/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.5.2/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.5.2/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.5.2/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-13 04:23:50.000000 funasr-0.5.2/funasr/utils/modelscope_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.5.2/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.5.2/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-12 01:37:03.000000 funasr-0.5.2/funasr/utils/vad_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.5.2/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.5.2/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-05-18 03:24:17.000000 funasr-0.5.2/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.394664 funasr-0.5.2/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     8468 2023-05-18 03:24:35.000000 funasr-0.5.2/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    13412 2023-05-18 03:24:35.000000 funasr-0.5.2/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-05-18 03:24:35.000000 funasr-0.5.2/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      864 2023-05-18 03:24:35.000000 funasr-0.5.2/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-05-18 03:24:35.000000 funasr-0.5.2/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-05-18 03:24:35.576472 funasr-0.5.2/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     4641 2023-05-18 02:15:48.000000 funasr-0.5.2/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:24:35.575606 funasr-0.5.2/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    26162 2023-05-08 08:26:24.000000 funasr-0.5.2/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.5.2/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.5.2/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.5.2/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.5.2/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.5.2/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.224642 funasr-0.5.3/
+-rw-r--r--   0 zhifu      (502) staff       (20)     1063 2023-02-07 07:13:38.000000 funasr-0.5.3/LICENSE
+-rw-r--r--   0 zhifu      (502) staff       (20)     8468 2023-05-18 03:46:27.224154 funasr-0.5.3/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     7446 2023-05-18 02:19:50.000000 funasr-0.5.3/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.586757 funasr-0.5.3/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.645149 funasr-0.5.3/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21913 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11106 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    25965 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40504 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26713 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference_paraformer_streaming.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    24956 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference_rnnt.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23949 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_inference_uniasr.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1068 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1027 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_train_paraformer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1036 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_train_transducer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1024 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/asr_train_uniasr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5382 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-18 02:19:38.000000 funasr-0.5.3/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5327 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1010 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/diar_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    14137 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/eend_ola_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     6814 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/lm_calc_perplexity.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14544 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/lm_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3816 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1019 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/lm_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3049 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/modelscope_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3593 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/punc_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11940 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/punctuation_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11101 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/punctuation_infer_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23328 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/sa_asr_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1071 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/sa_asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20700 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/sond_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    14841 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/sv_inference.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     4718 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.5.3/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13304 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/tp_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3874 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/tp_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19679 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/vad_inference.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4282 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/vad_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11618 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/bin/vad_inference_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.649952 funasr-0.5.3/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.5.3/funasr/datasets/iterable_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12671 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/datasets/iterable_dataset_modelscope.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.655228 funasr-0.5.3/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3488 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.657845 funasr-0.5.3/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9294 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.668058 funasr-0.5.3/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2583 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-18 02:19:38.000000 funasr-0.5.3/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.5.3/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.669732 funasr-0.5.3/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10699 2023-05-12 02:41:22.000000 funasr-0.5.3/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.677597 funasr-0.5.3/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.5.3/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.679060 funasr-0.5.3/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.5.3/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.5.3/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.691431 funasr-0.5.3/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.5.3/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.5.3/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.695413 funasr-0.5.3/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.5.3/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.5.3/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.696512 funasr-0.5.3/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.5.3/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.698593 funasr-0.5.3/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      966 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.699101 funasr-0.5.3/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.5.3/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.711222 funasr-0.5.3/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3539 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.713464 funasr-0.5.3/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.718080 funasr-0.5.3/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      359 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3503 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      349 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.5.3/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.719241 funasr-0.5.3/funasr/lm/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/lm/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5436 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/lm/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5904 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/lm/seq_rnn_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4243 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/lm/transformer_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.724737 funasr-0.5.3/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.5.3/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.727056 funasr-0.5.3/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5610 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5029 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.755169 funasr-0.5.3/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.5.3/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5298 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.758931 funasr-0.5.3/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.5.3/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75199 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.5.3/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16707 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.5.3/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11630 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    74013 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    34796 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10238 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20581 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19501 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10098 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6710 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51737 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31100 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.766377 funasr-0.5.3/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      503 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43608 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20993 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.5.3/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.5.3/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.5.3/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17514 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.775833 funasr-0.5.3/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.5.3/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.5.3/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.5.3/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41077 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3634 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    54458 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.778546 funasr-0.5.3/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      400 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9106 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5759 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4990 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20471 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6322 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2817 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.779206 funasr-0.5.3/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.5.3/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.5.3/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.801946 funasr-0.5.3/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.5.3/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.803537 funasr-0.5.3/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.804074 funasr-0.5.3/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35684 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.805815 funasr-0.5.3/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/preencoder/sinc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.840666 funasr-0.5.3/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4661 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4715 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.858248 funasr-0.5.3/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.5.3/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.861741 funasr-0.5.3/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/beam_search/beam_search.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-09 03:02:42.000000 funasr-0.5.3/funasr/modules/beam_search/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.5.3/funasr/modules/beam_search/beam_search_transducer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.875203 funasr-0.5.3/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.5.3/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.876397 funasr-0.5.3/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.5.3/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/modules/eend_ola/encoder_decoder_attractor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.5.3/funasr/modules/embedding.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.878418 funasr-0.5.3/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.5.3/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.5.3/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.5.3/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.5.3/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.880688 funasr-0.5.3/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.882676 funasr-0.5.3/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.885276 funasr-0.5.3/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21441 2023-04-25 03:22:30.000000 funasr-0.5.3/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/modules/subsampling_without_posenc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.886171 funasr-0.5.3/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.886451 funasr-0.5.3/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.3/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.886687 funasr-0.5.3/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.3/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.887584 funasr-0.5.3/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.5.3/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.888289 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.890005 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.892782 funasr-0.5.3/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.893946 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13093 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.896272 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1580 2023-05-12 03:39:34.000000 funasr-0.5.3/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.056012 funasr-0.5.3/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.059494 funasr-0.5.3/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.081951 funasr-0.5.3/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    74340 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    60814 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32463 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6782 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8029 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21378 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18814 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12527 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.088644 funasr-0.5.3/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.137542 funasr-0.5.3/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.5.3/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.172652 funasr-0.5.3/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1764 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/train/abs_espnet_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7280 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.5.3/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    37188 2023-05-18 03:45:34.000000 funasr-0.5.3/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.218835 funasr-0.5.3/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.5.3/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.5.3/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.5.3/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.5.3/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.5.3/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-13 04:23:50.000000 funasr-0.5.3/funasr/utils/modelscope_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.5.3/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.5.3/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-12 01:37:03.000000 funasr-0.5.3/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.5.3/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.5.3/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-05-18 03:46:00.000000 funasr-0.5.3/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:26.587836 funasr-0.5.3/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8468 2023-05-18 03:46:26.000000 funasr-0.5.3/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    13412 2023-05-18 03:46:26.000000 funasr-0.5.3/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-05-18 03:46:26.000000 funasr-0.5.3/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      857 2023-05-18 03:46:26.000000 funasr-0.5.3/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-05-18 03:46:26.000000 funasr-0.5.3/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-05-18 03:46:27.224818 funasr-0.5.3/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     4634 2023-05-18 03:45:59.000000 funasr-0.5.3/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-05-18 03:46:27.223356 funasr-0.5.3/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    26162 2023-05-08 08:26:24.000000 funasr-0.5.3/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.5.3/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.5.3/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.5.3/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.5.3/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.5.3/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.5.2/LICENSE` & `funasr-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/PKG-INFO` & `funasr-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.5.2
+Version: 0.5.3
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.5.2 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.5.3 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
```

### Comparing `funasr-0.5.2/README.md` & `funasr-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.5.3/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/asr_inference.py` & `funasr-0.5.3/funasr/bin/asr_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/asr_inference_launch.py` & `funasr-0.5.3/funasr/bin/asr_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/asr_inference_mfcca.py` & `funasr-0.5.3/funasr/bin/asr_inference_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/asr_inference_paraformer.py` & `funasr-0.5.3/funasr/bin/asr_inference_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/asr_inference_paraformer_streaming.py` & `funasr-0.5.3/funasr/bin/asr_inference_paraformer_streaming.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/asr_inference_rnnt.py` & `funasr-0.5.3/funasr/bin/asr_inference_rnnt.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/asr_inference_uniasr.py` & `funasr-0.5.3/funasr/bin/asr_inference_uniasr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/asr_train.py` & `funasr-0.5.3/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/asr_train_paraformer.py` & `funasr-0.5.3/funasr/bin/asr_train_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/asr_train_transducer.py` & `funasr-0.5.3/funasr/bin/asr_train_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/asr_train_uniasr.py` & `funasr-0.5.3/funasr/bin/asr_train_uniasr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/build_trainer.py` & `funasr-0.5.3/funasr/bin/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/data2vec_train.py` & `funasr-0.5.3/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/diar_inference_launch.py` & `funasr-0.5.3/funasr/bin/diar_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/diar_train.py` & `funasr-0.5.3/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/eend_ola_inference.py` & `funasr-0.5.3/funasr/bin/eend_ola_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/lm_calc_perplexity.py` & `funasr-0.5.3/funasr/bin/lm_calc_perplexity.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/lm_inference.py` & `funasr-0.5.3/funasr/bin/lm_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/lm_inference_launch.py` & `funasr-0.5.3/funasr/bin/lm_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/lm_train.py` & `funasr-0.5.3/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/modelscope_infer.py` & `funasr-0.5.3/funasr/bin/modelscope_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/punc_inference_launch.py` & `funasr-0.5.3/funasr/bin/punc_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/punc_train.py` & `funasr-0.5.3/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/punctuation_infer.py` & `funasr-0.5.3/funasr/bin/punctuation_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/punctuation_infer_vadrealtime.py` & `funasr-0.5.3/funasr/bin/punctuation_infer_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/sa_asr_inference.py` & `funasr-0.5.3/funasr/bin/sa_asr_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/sa_asr_train.py` & `funasr-0.5.3/funasr/bin/sa_asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/sond_inference.py` & `funasr-0.5.3/funasr/bin/sond_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/sv_inference.py` & `funasr-0.5.3/funasr/bin/sv_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/sv_inference_launch.py` & `funasr-0.5.3/funasr/bin/sv_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/tokenize_text.py` & `funasr-0.5.3/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/tp_inference.py` & `funasr-0.5.3/funasr/bin/tp_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/tp_inference_launch.py` & `funasr-0.5.3/funasr/bin/tp_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/vad_inference.py` & `funasr-0.5.3/funasr/bin/vad_inference.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/vad_inference_launch.py` & `funasr-0.5.3/funasr/bin/vad_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/bin/vad_inference_online.py` & `funasr-0.5.3/funasr/bin/vad_inference_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/collate_fn.py` & `funasr-0.5.3/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/dataset.py` & `funasr-0.5.3/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/iterable_dataset.py` & `funasr-0.5.3/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/iterable_dataset_modelscope.py` & `funasr-0.5.3/funasr/datasets/iterable_dataset_modelscope.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.5.3/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.5.3/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.5.3/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/large_datasets/dataset.py` & `funasr-0.5.3/funasr/datasets/large_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.5.3/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.5.3/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/large_datasets/utils/hotword_utils.py` & `funasr-0.5.3/funasr/datasets/large_datasets/utils/hotword_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.5.3/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.5.3/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.5.3/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/ms_dataset.py` & `funasr-0.5.3/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/datasets/preprocessor.py` & `funasr-0.5.3/funasr/datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/export_model.py` & `funasr-0.5.3/funasr/export/export_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/CT_Transformer.py` & `funasr-0.5.3/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/__init__.py` & `funasr-0.5.3/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.5.3/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.5.3/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.5.3/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/e2e_vad.py` & `funasr-0.5.3/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.5.3/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.5.3/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.5.3/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/modules/decoder_layer.py` & `funasr-0.5.3/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/modules/encoder_layer.py` & `funasr-0.5.3/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/modules/feedforward.py` & `funasr-0.5.3/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/modules/multihead_att.py` & `funasr-0.5.3/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/models/predictor/cif.py` & `funasr-0.5.3/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/test/test_onnx.py` & `funasr-0.5.3/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/test/test_onnx_punc.py` & `funasr-0.5.3/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.5.3/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/test/test_onnx_vad.py` & `funasr-0.5.3/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/export/utils/torch_function.py` & `funasr-0.5.3/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/fileio/datadir_writer.py` & `funasr-0.5.3/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/fileio/npy_scp.py` & `funasr-0.5.3/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/fileio/rand_gen_dataset.py` & `funasr-0.5.3/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/fileio/read_text.py` & `funasr-0.5.3/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/fileio/sound_scp.py` & `funasr-0.5.3/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/iterators/chunk_iter_factory.py` & `funasr-0.5.3/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/iterators/multiple_iter_factory.py` & `funasr-0.5.3/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/iterators/sequence_iter_factory.py` & `funasr-0.5.3/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/layers/complex_utils.py` & `funasr-0.5.3/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/layers/global_mvn.py` & `funasr-0.5.3/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/layers/label_aggregation.py` & `funasr-0.5.3/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/layers/log_mel.py` & `funasr-0.5.3/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/layers/mask_along_axis.py` & `funasr-0.5.3/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/layers/sinc_conv.py` & `funasr-0.5.3/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/layers/stft.py` & `funasr-0.5.3/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/layers/time_warp.py` & `funasr-0.5.3/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/layers/utterance_mvn.py` & `funasr-0.5.3/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/lm/abs_model.py` & `funasr-0.5.3/funasr/lm/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/lm/seq_rnn_lm.py` & `funasr-0.5.3/funasr/lm/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/lm/transformer_lm.py` & `funasr-0.5.3/funasr/lm/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/losses/label_smoothing_loss.py` & `funasr-0.5.3/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/main_funcs/average_nbest_models.py` & `funasr-0.5.3/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.5.3/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/main_funcs/collect_stats.py` & `funasr-0.5.3/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/main_funcs/pack_funcs.py` & `funasr-0.5.3/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/ctc.py` & `funasr-0.5.3/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/data2vec.py` & `funasr-0.5.3/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/decoder/contextual_decoder.py` & `funasr-0.5.3/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/decoder/rnn_decoder.py` & `funasr-0.5.3/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.5.3/funasr/models/decoder/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/decoder/sanm_decoder.py` & `funasr-0.5.3/funasr/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/decoder/sv_decoder.py` & `funasr-0.5.3/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/decoder/transformer_decoder.py` & `funasr-0.5.3/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_asr.py` & `funasr-0.5.3/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_asr_common.py` & `funasr-0.5.3/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_asr_contextual_paraformer.py` & `funasr-0.5.3/funasr/models/e2e_asr_contextual_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_asr_mfcca.py` & `funasr-0.5.3/funasr/models/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_asr_paraformer.py` & `funasr-0.5.3/funasr/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_asr_transducer.py` & `funasr-0.5.3/funasr/models/e2e_asr_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.5.3/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_diar_sond.py` & `funasr-0.5.3/funasr/models/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_sa_asr.py` & `funasr-0.5.3/funasr/models/e2e_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_sv.py` & `funasr-0.5.3/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_tp.py` & `funasr-0.5.3/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_uni_asr.py` & `funasr-0.5.3/funasr/models/e2e_uni_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/e2e_vad.py` & `funasr-0.5.3/funasr/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/conformer_encoder.py` & `funasr-0.5.3/funasr/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.5.3/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.5.3/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.5.3/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.5.3/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.5.3/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.5.3/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.5.3/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.5.3/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.5.3/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.5.3/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/rnn_encoder.py` & `funasr-0.5.3/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/sanm_encoder.py` & `funasr-0.5.3/funasr/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/encoder/transformer_encoder.py` & `funasr-0.5.3/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/frontend/default.py` & `funasr-0.5.3/funasr/models/frontend/default.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.5.3/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/frontend/fused.py` & `funasr-0.5.3/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/frontend/s3prl.py` & `funasr-0.5.3/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/frontend/wav_frontend.py` & `funasr-0.5.3/funasr/models/frontend/wav_frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.5.3/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/frontend/windowing.py` & `funasr-0.5.3/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/joint_net/joint_network.py` & `funasr-0.5.3/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/pooling/statistic_pooling.py` & `funasr-0.5.3/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.5.3/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/predictor/cif.py` & `funasr-0.5.3/funasr/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/preencoder/linear.py` & `funasr-0.5.3/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/preencoder/sinc.py` & `funasr-0.5.3/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/specaug/specaug.py` & `funasr-0.5.3/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/target_delay_transformer.py` & `funasr-0.5.3/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/models/vad_realtime_transformer.py` & `funasr-0.5.3/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/add_sos_eos.py` & `funasr-0.5.3/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/attention.py` & `funasr-0.5.3/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.5.3/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.5.3/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/beam_search/beam_search.py` & `funasr-0.5.3/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/beam_search/beam_search_sa_asr.py` & `funasr-0.5.3/funasr/modules/beam_search/beam_search_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.5.3/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/data2vec/data_utils.py` & `funasr-0.5.3/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/data2vec/ema_module.py` & `funasr-0.5.3/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.5.3/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/data2vec/quant_noise.py` & `funasr-0.5.3/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/data2vec/utils.py` & `funasr-0.5.3/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.5.3/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/dynamic_conv.py` & `funasr-0.5.3/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/dynamic_conv2d.py` & `funasr-0.5.3/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/e2e_asr_common.py` & `funasr-0.5.3/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/eend_ola/encoder.py` & `funasr-0.5.3/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.5.3/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/embedding.py` & `funasr-0.5.3/funasr/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/frontends/beamformer.py` & `funasr-0.5.3/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.5.3/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.5.3/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/frontends/feature_transform.py` & `funasr-0.5.3/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/frontends/frontend.py` & `funasr-0.5.3/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/frontends/mask_estimator.py` & `funasr-0.5.3/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/layer_norm.py` & `funasr-0.5.3/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/lightconv.py` & `funasr-0.5.3/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/lightconv2d.py` & `funasr-0.5.3/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/mask.py` & `funasr-0.5.3/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/multi_layer_conv.py` & `funasr-0.5.3/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/nets_utils.py` & `funasr-0.5.3/funasr/modules/nets_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/positionwise_feed_forward.py` & `funasr-0.5.3/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/repeat.py` & `funasr-0.5.3/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/rnn/argument.py` & `funasr-0.5.3/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/rnn/attentions.py` & `funasr-0.5.3/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/rnn/decoders.py` & `funasr-0.5.3/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/rnn/encoders.py` & `funasr-0.5.3/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/scorers/ctc.py` & `funasr-0.5.3/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.5.3/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/scorers/length_bonus.py` & `funasr-0.5.3/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/scorers/scorer_interface.py` & `funasr-0.5.3/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.5.3/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.5.3/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/streaming_utils/utils.py` & `funasr-0.5.3/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/subsampling.py` & `funasr-0.5.3/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/modules/subsampling_without_posenc.py` & `funasr-0.5.3/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/optimizers/fairseq_adam.py` & `funasr-0.5.3/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/optimizers/sgd.py` & `funasr-0.5.3/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/libtorch/demo.py` & `funasr-0.5.3/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.5.3/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/libtorch/setup.py` & `funasr-0.5.3/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.5.3/funasr/runtime/python/onnxruntime/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/samplers/build_batch_sampler.py` & `funasr-0.5.3/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/samplers/folded_batch_sampler.py` & `funasr-0.5.3/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/samplers/length_batch_sampler.py` & `funasr-0.5.3/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.5.3/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.5.3/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.5.3/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/schedulers/abs_scheduler.py` & `funasr-0.5.3/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/schedulers/noam_lr.py` & `funasr-0.5.3/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.5.3/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/schedulers/warmup_lr.py` & `funasr-0.5.3/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/tasks/abs_task.py` & `funasr-0.5.3/funasr/tasks/abs_task.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/tasks/asr.py` & `funasr-0.5.3/funasr/tasks/asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/tasks/data2vec.py` & `funasr-0.5.3/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/tasks/diar.py` & `funasr-0.5.3/funasr/tasks/diar.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/tasks/lm.py` & `funasr-0.5.3/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/tasks/punctuation.py` & `funasr-0.5.3/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/tasks/sa_asr.py` & `funasr-0.5.3/funasr/tasks/sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/tasks/sv.py` & `funasr-0.5.3/funasr/tasks/sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/tasks/vad.py` & `funasr-0.5.3/funasr/tasks/vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/text/build_tokenizer.py` & `funasr-0.5.3/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/text/char_tokenizer.py` & `funasr-0.5.3/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/text/cleaner.py` & `funasr-0.5.3/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/text/korean_cleaner.py` & `funasr-0.5.3/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/text/phoneme_tokenizer.py` & `funasr-0.5.3/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.5.3/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/text/token_id_converter.py` & `funasr-0.5.3/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/text/word_tokenizer.py` & `funasr-0.5.3/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.5.3/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/torch_utils/device_funcs.py` & `funasr-0.5.3/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/torch_utils/forward_adaptor.py` & `funasr-0.5.3/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/torch_utils/initialize.py` & `funasr-0.5.3/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.5.3/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/torch_utils/model_summary.py` & `funasr-0.5.3/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/torch_utils/recursive_op.py` & `funasr-0.5.3/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/train/abs_espnet_model.py` & `funasr-0.5.3/funasr/train/abs_espnet_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/train/abs_model.py` & `funasr-0.5.3/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/train/class_choices.py` & `funasr-0.5.3/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/train/distributed_utils.py` & `funasr-0.5.3/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/train/reporter.py` & `funasr-0.5.3/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/train/trainer.py` & `funasr-0.5.3/funasr/train/trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/asr_env_checking.py` & `funasr-0.5.3/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/asr_utils.py` & `funasr-0.5.3/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/build_dataclass.py` & `funasr-0.5.3/funasr/utils/build_dataclass.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/cli_utils.py` & `funasr-0.5.3/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/compute_eer.py` & `funasr-0.5.3/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/compute_min_dcf.py` & `funasr-0.5.3/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/compute_wer.py` & `funasr-0.5.3/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/config_argparse.py` & `funasr-0.5.3/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/get_default_kwargs.py` & `funasr-0.5.3/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/griffin_lim.py` & `funasr-0.5.3/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/job_runner.py` & `funasr-0.5.3/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/misc.py` & `funasr-0.5.3/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/modelscope_param.py` & `funasr-0.5.3/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/modelscope_utils.py` & `funasr-0.5.3/funasr/utils/modelscope_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/nested_dict_action.py` & `funasr-0.5.3/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/postprocess_utils.py` & `funasr-0.5.3/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/sized_dict.py` & `funasr-0.5.3/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/timestamp_tools.py` & `funasr-0.5.3/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/types.py` & `funasr-0.5.3/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/vad_utils.py` & `funasr-0.5.3/funasr/utils/vad_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr/utils/wav_utils.py` & `funasr-0.5.3/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr.egg-info/PKG-INFO` & `funasr-0.5.3/funasr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.5.2
+Version: 0.5.3
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.5.2 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.5.3 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
```

### Comparing `funasr-0.5.2/funasr.egg-info/SOURCES.txt` & `funasr-0.5.3/funasr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/funasr.egg-info/requires.txt` & `funasr-0.5.3/funasr.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 setuptools>=38.5.1
 typeguard==2.13.3
 humanfriendly
 scipy>=1.4.1
-librosa==0.8.1
+librosa
 jamo==0.4.1
 PyYAML>=5.1.2
 soundfile>=0.10.2
 h5py>=2.10.0
 kaldiio>=2.17.0
 torch_complex
 nltk>=3.4.5
```

### Comparing `funasr-0.5.2/setup.py` & `funasr-0.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "install": [
         "setuptools>=38.5.1",
         # "configargparse>=1.2.1",
         "typeguard==2.13.3",
         "humanfriendly",
         "scipy>=1.4.1",
         # "filelock",
-        "librosa==0.8.1",
+        "librosa",
         "jamo==0.4.1",  # For kss
         "PyYAML>=5.1.2",
         "soundfile>=0.10.2",
         "h5py>=2.10.0",
         "kaldiio>=2.17.0",
         "torch_complex",
         "nltk>=3.4.5",
```

### Comparing `funasr-0.5.2/tests/test_asr_inference_pipeline.py` & `funasr-0.5.3/tests/test_asr_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.5.3/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/tests/test_lm_pipeline.py` & `funasr-0.5.3/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/tests/test_punctuation_pipeline.py` & `funasr-0.5.3/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/tests/test_sv_inference_pipeline.py` & `funasr-0.5.3/tests/test_sv_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.5.2/tests/test_vad_inference_pipeline.py` & `funasr-0.5.3/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

