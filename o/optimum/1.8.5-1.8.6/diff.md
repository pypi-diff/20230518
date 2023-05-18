# Comparing `tmp/optimum-1.8.5.tar.gz` & `tmp/optimum-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-1.8.5.tar", last modified: Thu May 11 09:41:53 2023, max compression
+gzip compressed data, was "optimum-1.8.6.tar", last modified: Thu May 18 08:09:20 2023, max compression
```

## Comparing `optimum-1.8.5.tar` & `optimum-1.8.6.tar`

### file list

```diff
@@ -1,152 +1,149 @@
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.065360 optimum-1.8.5/
--rw-rw-r--   0 regis     (1000) regis     (1000)    11357 2023-03-22 09:54:58.000000 optimum-1.8.5/LICENSE
--rw-rw-r--   0 regis     (1000) regis     (1000)      651 2023-03-22 09:54:58.000000 optimum-1.8.5/MANIFEST.in
--rw-rw-r--   0 regis     (1000) regis     (1000)    11475 2023-05-11 09:41:53.065360 optimum-1.8.5/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)     9876 2023-05-11 09:35:27.000000 optimum-1.8.5/README.md
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.057360 optimum-1.8.5/optimum/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.057360 optimum-1.8.5/optimum/bettertransformer/
--rw-rw-r--   0 regis     (1000) regis     (1000)      707 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/bettertransformer/__init__.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/bettertransformer/models/
--rw-rw-r--   0 regis     (1000) regis     (1000)     8420 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/bettertransformer/models/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    21474 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/bettertransformer/models/attention.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     8092 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/bettertransformer/models/base.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    12222 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/bettertransformer/models/decoder_models.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    60023 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/bettertransformer/models/encoder_models.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    17127 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/bettertransformer/transformation.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/commands/
--rw-rw-r--   0 regis     (1000) regis     (1000)      952 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/commands/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     5872 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/commands/base.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     2475 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/commands/env.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/commands/export/
--rw-rw-r--   0 regis     (1000) regis     (1000)      716 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/commands/export/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     1340 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/commands/export/base.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     8554 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/commands/export/onnx.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     9016 2023-04-21 16:45:52.000000 optimum-1.8.5/optimum/commands/export/tflite.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/commands/onnxruntime/
--rw-rw-r--   0 regis     (1000) regis     (1000)      759 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/commands/onnxruntime/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     1374 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/commands/onnxruntime/base.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     3885 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/commands/onnxruntime/optimize.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     4011 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/commands/onnxruntime/quantize.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     6871 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/commands/optimum_cli.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/commands/register/
--rw-rw-r--   0 regis     (1000) regis     (1000)      621 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/commands/register/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    17957 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/configuration_utils.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     1454 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/conftest.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/exporters/
--rw-rw-r--   0 regis     (1000) regis     (1000)      688 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/exporters/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)      707 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/exporters/base.py
--rw-rw-r--   0 regis     (1000) regis     (1000)      903 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/exporters/error_utils.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/exporters/onnx/
--rw-rw-r--   0 regis     (1000) regis     (1000)     1918 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/exporters/onnx/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    17290 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/exporters/onnx/__main__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    44198 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/exporters/onnx/base.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    16221 2023-04-21 16:45:52.000000 optimum-1.8.5/optimum/exporters/onnx/config.py
--rw-rw-r--   0 regis     (1000) regis     (1000)      865 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/exporters/onnx/constants.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    31628 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/exporters/onnx/convert.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    37124 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/exporters/onnx/model_configs.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     7326 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/exporters/onnx/model_patcher.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     9950 2023-05-03 12:04:20.000000 optimum-1.8.5/optimum/exporters/onnx/utils.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    60556 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/exporters/tasks.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/exporters/tflite/
--rw-rw-r--   0 regis     (1000) regis     (1000)     1209 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/exporters/tflite/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     5256 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/exporters/tflite/__main__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    15507 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/exporters/tflite/base.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     1397 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/exporters/tflite/config.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    16963 2023-04-21 16:45:52.000000 optimum-1.8.5/optimum/exporters/tflite/convert.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     3588 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/exporters/tflite/model_configs.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/fx/
--rw-rw-r--   0 regis     (1000) regis     (1000)      672 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/fx/__init__.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/fx/optimization/
--rw-rw-r--   0 regis     (1000) regis     (1000)      866 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/fx/optimization/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    32725 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/fx/optimization/transformations.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/fx/quantization/
--rw-rw-r--   0 regis     (1000) regis     (1000)      675 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/fx/quantization/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    13591 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/fx/quantization/functions.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     1450 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/fx/utils.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    15117 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/modeling_base.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/onnx/
--rw-rw-r--   0 regis     (1000) regis     (1000)     1276 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnx/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     3830 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnx/configuration.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    11198 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/onnx/graph_transformations.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     4316 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnx/modeling_seq2seq.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    13025 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/onnx/transformations_utils.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     3307 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnx/utils.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/onnxruntime/
--rw-rw-r--   0 regis     (1000) regis     (1000)     4279 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    32544 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/onnxruntime/base.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    45434 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/onnxruntime/configuration.py
--rw-rw-r--   0 regis     (1000) regis     (1000)      901 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/onnxruntime/constants.py
--rw-rw-r--   0 regis     (1000) regis     (1000)      955 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/graph.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/onnxruntime/io_binding/
--rw-rw-r--   0 regis     (1000) regis     (1000)      675 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/io_binding/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     7767 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/io_binding/io_binding_helper.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     3915 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/model.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    30965 2023-04-21 16:45:52.000000 optimum-1.8.5/optimum/onnxruntime/modeling_decoder.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    17940 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/modeling_diffusion.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    83591 2023-04-21 16:45:52.000000 optimum-1.8.5/optimum/onnxruntime/modeling_ort.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    58316 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/onnxruntime/modeling_seq2seq.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    15083 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/optimization.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.061360 optimum-1.8.5/optimum/onnxruntime/preprocessors/
--rw-rw-r--   0 regis     (1000) regis     (1000)      686 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/preprocessors/__init__.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.065360 optimum-1.8.5/optimum/onnxruntime/preprocessors/passes/
--rw-rw-r--   0 regis     (1000) regis     (1000)      760 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/preprocessors/passes/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     3048 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/preprocessors/passes/excluders.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     1377 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/preprocessors/passes/fully_connected.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     1415 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/preprocessors/passes/gelu.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     1580 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/preprocessors/passes/layernorm.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     2350 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/preprocessors/quantization.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    23448 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/onnxruntime/quantization.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.065360 optimum-1.8.5/optimum/onnxruntime/runs/
--rw-rw-r--   0 regis     (1000) regis     (1000)     8001 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/runs/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     4070 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/runs/calibrator.py
--rw-rw-r--   0 regis     (1000) regis     (1000)      625 2023-04-21 16:45:52.000000 optimum-1.8.5/optimum/onnxruntime/runs/utils.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    88945 2023-04-21 16:45:52.000000 optimum-1.8.5/optimum/onnxruntime/trainer.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    38387 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/onnxruntime/trainer_seq2seq.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    17122 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/onnxruntime/training_args.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     1362 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/onnxruntime/training_args_seq2seq.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    11746 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/onnxruntime/utils.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.065360 optimum-1.8.5/optimum/pipelines/
--rw-rw-r--   0 regis     (1000) regis     (1000)      770 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/pipelines/__init__.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.065360 optimum-1.8.5/optimum/pipelines/diffusers/
--rw-rw-r--   0 regis     (1000) regis     (1000)    11266 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/pipelines/diffusers/pipeline_stable_diffusion.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     2211 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/pipelines/diffusers/pipeline_utils.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    13522 2023-05-03 18:22:21.000000 optimum-1.8.5/optimum/pipelines/pipelines_base.py
--rw-rw-r--   0 regis     (1000) regis     (1000)      948 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/quantization_base.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    10268 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/runs_base.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.065360 optimum-1.8.5/optimum/utils/
--rw-rw-r--   0 regis     (1000) regis     (1000)     1989 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/utils/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)      845 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/utils/constant.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     2001 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/utils/doc.py
--rw-rw-r--   0 regis     (1000) regis     (1000)      953 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/utils/dummy_diffusers_objects.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     3747 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/utils/file_utils.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     6181 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/utils/import_utils.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    23612 2023-05-11 09:35:27.000000 optimum-1.8.5/optimum/utils/input_generators.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     7836 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/utils/logging.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     1295 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/utils/modeling_utils.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     9323 2023-04-21 16:45:52.000000 optimum-1.8.5/optimum/utils/normalized_config.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.065360 optimum-1.8.5/optimum/utils/preprocessing/
--rw-rw-r--   0 regis     (1000) regis     (1000)      977 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/utils/preprocessing/__init__.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    10271 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/utils/preprocessing/base.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     4263 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/utils/preprocessing/image_classification.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     3995 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/utils/preprocessing/question_answering.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     2169 2023-04-21 16:45:52.000000 optimum-1.8.5/optimum/utils/preprocessing/task_processors_manager.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     4436 2023-04-21 16:45:52.000000 optimum-1.8.5/optimum/utils/preprocessing/text_classification.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     3940 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/utils/preprocessing/token_classification.py
--rw-rw-r--   0 regis     (1000) regis     (1000)    11609 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/utils/runs.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     2364 2023-03-22 09:54:58.000000 optimum-1.8.5/optimum/utils/save_utils.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     5762 2023-04-07 08:20:06.000000 optimum-1.8.5/optimum/utils/testing_utils.py
--rw-rw-r--   0 regis     (1000) regis     (1000)      639 2023-05-11 09:37:00.000000 optimum-1.8.5/optimum/version.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.057360 optimum-1.8.5/optimum.egg-info/
--rw-rw-r--   0 regis     (1000) regis     (1000)    11475 2023-05-11 09:41:52.000000 optimum-1.8.5/optimum.egg-info/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)     4333 2023-05-11 09:41:53.000000 optimum-1.8.5/optimum.egg-info/SOURCES.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)        1 2023-05-11 09:41:52.000000 optimum-1.8.5/optimum.egg-info/dependency_links.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       66 2023-05-11 09:41:52.000000 optimum-1.8.5/optimum.egg-info/entry_points.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)        1 2023-05-03 12:05:20.000000 optimum-1.8.5/optimum.egg-info/not-zip-safe
--rw-rw-r--   0 regis     (1000) regis     (1000)     1089 2023-05-11 09:41:52.000000 optimum-1.8.5/optimum.egg-info/requires.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)        8 2023-05-11 09:41:52.000000 optimum-1.8.5/optimum.egg-info/top_level.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)     1212 2023-03-22 09:54:58.000000 optimum-1.8.5/pyproject.toml
--rw-rw-r--   0 regis     (1000) regis     (1000)      423 2023-05-11 09:41:53.065360 optimum-1.8.5/setup.cfg
--rw-rw-r--   0 regis     (1000) regis     (1000)     3564 2023-05-11 09:36:05.000000 optimum-1.8.5/setup.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-11 09:41:53.065360 optimum-1.8.5/tests/
--rw-rw-r--   0 regis     (1000) regis     (1000)     3432 2023-05-11 09:35:27.000000 optimum-1.8.5/tests/test_configuration_utils.py
--rw-rw-r--   0 regis     (1000) regis     (1000)     1936 2023-03-22 09:54:58.000000 optimum-1.8.5/tests/test_modeling_base.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.803465 optimum-1.8.6/
+-rw-rw-r--   0 regis     (1000) regis     (1000)    11357 2023-03-22 09:54:58.000000 optimum-1.8.6/LICENSE
+-rw-rw-r--   0 regis     (1000) regis     (1000)      651 2023-03-22 09:54:58.000000 optimum-1.8.6/MANIFEST.in
+-rw-rw-r--   0 regis     (1000) regis     (1000)    11475 2023-05-18 08:09:20.803465 optimum-1.8.6/PKG-INFO
+-rw-rw-r--   0 regis     (1000) regis     (1000)     9876 2023-05-18 08:00:17.000000 optimum-1.8.6/README.md
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.795465 optimum-1.8.6/optimum/
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.795465 optimum-1.8.6/optimum/bettertransformer/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      707 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/bettertransformer/__init__.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/bettertransformer/models/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     8420 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/bettertransformer/models/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    21474 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/bettertransformer/models/attention.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     8092 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/bettertransformer/models/base.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    12222 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/bettertransformer/models/decoder_models.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    60023 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/bettertransformer/models/encoder_models.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    17127 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/bettertransformer/transformation.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/commands/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      952 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/commands/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     5872 2023-05-17 18:19:10.000000 optimum-1.8.6/optimum/commands/base.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     2475 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/commands/env.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/commands/export/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      716 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/commands/export/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1340 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/commands/export/base.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     8554 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/commands/export/onnx.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     9100 2023-05-18 08:02:07.000000 optimum-1.8.6/optimum/commands/export/tflite.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/commands/onnxruntime/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      759 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/commands/onnxruntime/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1374 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/commands/onnxruntime/base.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3885 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/commands/onnxruntime/optimize.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4011 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/commands/onnxruntime/quantize.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     6871 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/commands/optimum_cli.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/commands/register/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      621 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/commands/register/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    17957 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/configuration_utils.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1454 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/conftest.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/exporters/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      688 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/exporters/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)      707 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/exporters/base.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)      903 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/exporters/error_utils.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/exporters/onnx/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1918 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/exporters/onnx/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    17290 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/exporters/onnx/__main__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    44198 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/exporters/onnx/base.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    16221 2023-04-21 16:45:52.000000 optimum-1.8.6/optimum/exporters/onnx/config.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)      865 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/exporters/onnx/constants.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    31628 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/exporters/onnx/convert.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    37124 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/exporters/onnx/model_configs.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     7326 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/exporters/onnx/model_patcher.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     9950 2023-05-18 08:01:38.000000 optimum-1.8.6/optimum/exporters/onnx/utils.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    60556 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/exporters/tasks.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/exporters/tflite/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1209 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/exporters/tflite/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     5256 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/exporters/tflite/__main__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    15507 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/exporters/tflite/base.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1397 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/exporters/tflite/config.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    16963 2023-04-21 16:45:52.000000 optimum-1.8.6/optimum/exporters/tflite/convert.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3588 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/exporters/tflite/model_configs.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/fx/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      672 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/fx/__init__.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/fx/optimization/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      866 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/fx/optimization/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    32725 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/fx/optimization/transformations.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/fx/quantization/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      675 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/fx/quantization/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    13591 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/fx/quantization/functions.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1450 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/fx/utils.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    15117 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/modeling_base.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/onnx/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1276 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnx/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3830 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnx/configuration.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    11198 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/onnx/graph_transformations.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4316 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnx/modeling_seq2seq.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    13025 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/onnx/transformations_utils.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3307 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnx/utils.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/onnxruntime/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4279 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    32544 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/onnxruntime/base.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    45434 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/onnxruntime/configuration.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)      901 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/onnxruntime/constants.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)      955 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/graph.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/onnxruntime/io_binding/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      675 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/io_binding/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     7767 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/io_binding/io_binding_helper.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3915 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/model.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    30965 2023-04-21 16:45:52.000000 optimum-1.8.6/optimum/onnxruntime/modeling_decoder.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    17940 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/modeling_diffusion.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    83591 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/onnxruntime/modeling_ort.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    58316 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/onnxruntime/modeling_seq2seq.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    15083 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/optimization.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.799465 optimum-1.8.6/optimum/onnxruntime/preprocessors/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      686 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/preprocessors/__init__.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.803465 optimum-1.8.6/optimum/onnxruntime/preprocessors/passes/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      760 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/preprocessors/passes/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3048 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/preprocessors/passes/excluders.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1377 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/preprocessors/passes/fully_connected.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1415 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/preprocessors/passes/gelu.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1580 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/preprocessors/passes/layernorm.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     2350 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/preprocessors/quantization.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    23448 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/onnxruntime/quantization.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.803465 optimum-1.8.6/optimum/onnxruntime/runs/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     8001 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/runs/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4070 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/runs/calibrator.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)      625 2023-04-21 16:45:52.000000 optimum-1.8.6/optimum/onnxruntime/runs/utils.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    88945 2023-04-21 16:45:52.000000 optimum-1.8.6/optimum/onnxruntime/trainer.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    38387 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/onnxruntime/trainer_seq2seq.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    17122 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/onnxruntime/training_args.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1362 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/onnxruntime/training_args_seq2seq.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    11746 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/onnxruntime/utils.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.803465 optimum-1.8.6/optimum/pipelines/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      770 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/pipelines/__init__.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.803465 optimum-1.8.6/optimum/pipelines/diffusers/
+-rw-rw-r--   0 regis     (1000) regis     (1000)    11266 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/pipelines/diffusers/pipeline_stable_diffusion.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     2211 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/pipelines/diffusers/pipeline_utils.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    13522 2023-05-03 18:22:21.000000 optimum-1.8.6/optimum/pipelines/pipelines_base.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)      948 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/quantization_base.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    10268 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/runs_base.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.803465 optimum-1.8.6/optimum/utils/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1989 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/utils/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)      845 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/utils/constant.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     2001 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/utils/doc.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)      953 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/utils/dummy_diffusers_objects.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3747 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/utils/file_utils.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     6181 2023-05-18 08:01:38.000000 optimum-1.8.6/optimum/utils/import_utils.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    23612 2023-05-18 08:00:17.000000 optimum-1.8.6/optimum/utils/input_generators.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     7836 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/utils/logging.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1295 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/utils/modeling_utils.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     9323 2023-04-21 16:45:52.000000 optimum-1.8.6/optimum/utils/normalized_config.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.803465 optimum-1.8.6/optimum/utils/preprocessing/
+-rw-rw-r--   0 regis     (1000) regis     (1000)      977 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/utils/preprocessing/__init__.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    10271 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/utils/preprocessing/base.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4263 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/utils/preprocessing/image_classification.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3995 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/utils/preprocessing/question_answering.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     2169 2023-04-21 16:45:52.000000 optimum-1.8.6/optimum/utils/preprocessing/task_processors_manager.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4436 2023-04-21 16:45:52.000000 optimum-1.8.6/optimum/utils/preprocessing/text_classification.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3940 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/utils/preprocessing/token_classification.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)    11609 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/utils/runs.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     2364 2023-03-22 09:54:58.000000 optimum-1.8.6/optimum/utils/save_utils.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)     5762 2023-04-07 08:20:06.000000 optimum-1.8.6/optimum/utils/testing_utils.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)      639 2023-05-18 08:03:22.000000 optimum-1.8.6/optimum/version.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-18 08:09:20.795465 optimum-1.8.6/optimum.egg-info/
+-rw-rw-r--   0 regis     (1000) regis     (1000)    11475 2023-05-18 08:09:20.000000 optimum-1.8.6/optimum.egg-info/PKG-INFO
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4271 2023-05-18 08:09:20.000000 optimum-1.8.6/optimum.egg-info/SOURCES.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)        1 2023-05-18 08:09:20.000000 optimum-1.8.6/optimum.egg-info/dependency_links.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)       66 2023-05-18 08:09:20.000000 optimum-1.8.6/optimum.egg-info/entry_points.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)        1 2023-05-18 08:09:13.000000 optimum-1.8.6/optimum.egg-info/not-zip-safe
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1089 2023-05-18 08:09:20.000000 optimum-1.8.6/optimum.egg-info/requires.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)        8 2023-05-18 08:09:20.000000 optimum-1.8.6/optimum.egg-info/top_level.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)     1212 2023-03-22 09:54:58.000000 optimum-1.8.6/pyproject.toml
+-rw-rw-r--   0 regis     (1000) regis     (1000)      423 2023-05-18 08:09:20.803465 optimum-1.8.6/setup.cfg
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3564 2023-05-18 08:01:38.000000 optimum-1.8.6/setup.py
```

### Comparing `optimum-1.8.5/LICENSE` & `optimum-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/MANIFEST.in` & `optimum-1.8.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/PKG-INFO` & `optimum-1.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum
-Version: 1.8.5
+Version: 1.8.6
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://github.com/huggingface/optimum
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-1.8.5/README.md` & `optimum-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/bettertransformer/__init__.py` & `optimum-1.8.6/optimum/bettertransformer/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/bettertransformer/models/__init__.py` & `optimum-1.8.6/optimum/bettertransformer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/bettertransformer/models/attention.py` & `optimum-1.8.6/optimum/bettertransformer/models/attention.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/bettertransformer/models/base.py` & `optimum-1.8.6/optimum/bettertransformer/models/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/bettertransformer/models/decoder_models.py` & `optimum-1.8.6/optimum/bettertransformer/models/decoder_models.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/bettertransformer/models/encoder_models.py` & `optimum-1.8.6/optimum/bettertransformer/models/encoder_models.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/bettertransformer/transformation.py` & `optimum-1.8.6/optimum/bettertransformer/transformation.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/commands/__init__.py` & `optimum-1.8.6/optimum/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/commands/base.py` & `optimum-1.8.6/optimum/commands/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/commands/env.py` & `optimum-1.8.6/optimum/commands/env.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/commands/export/__init__.py` & `optimum-1.8.6/optimum/commands/export/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/commands/export/base.py` & `optimum-1.8.6/optimum/commands/export/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/commands/export/onnx.py` & `optimum-1.8.6/optimum/commands/export/onnx.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/commands/export/tflite.py` & `optimum-1.8.6/optimum/commands/export/tflite.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,20 +220,21 @@
         help=("The name of the column containing the image in the dataset. Only for image-classification."),
     )
 
 
 class TFLiteExportCommand(BaseOptimumCLICommand):
     def __init__(
         self,
-        parser: "_SubParsersAction",
+        subparsers: Optional["_SubParsersAction"],
         args: Optional["Namespace"] = None,
         command: Optional["CommandInfo"] = None,
         from_defaults_factory: bool = False,
+        parser: Optional["ArgumentParser"] = None,
     ):
-        super().__init__(parser, args, command=command, from_defaults_factory=from_defaults_factory)
+        super().__init__(subparsers, args, command=command, from_defaults_factory=from_defaults_factory, parser=parser)
         # TODO: hack until TFLiteExportCommand does not use subprocess anymore.
         self.args_string = " ".join(sys.argv[3:])
 
     @staticmethod
     def parse_args(parser: "ArgumentParser"):
         return parse_args_tflite(parser)
```

### Comparing `optimum-1.8.5/optimum/commands/onnxruntime/__init__.py` & `optimum-1.8.6/optimum/commands/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/commands/onnxruntime/base.py` & `optimum-1.8.6/optimum/commands/onnxruntime/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/commands/onnxruntime/optimize.py` & `optimum-1.8.6/optimum/commands/onnxruntime/optimize.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/commands/onnxruntime/quantize.py` & `optimum-1.8.6/optimum/commands/onnxruntime/quantize.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/commands/optimum_cli.py` & `optimum-1.8.6/optimum/commands/optimum_cli.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/commands/register/__init__.py` & `optimum-1.8.6/optimum/commands/register/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/configuration_utils.py` & `optimum-1.8.6/optimum/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/conftest.py` & `optimum-1.8.6/optimum/conftest.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/__init__.py` & `optimum-1.8.6/optimum/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/base.py` & `optimum-1.8.6/optimum/exporters/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/error_utils.py` & `optimum-1.8.6/optimum/exporters/error_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/onnx/__init__.py` & `optimum-1.8.6/optimum/exporters/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/onnx/__main__.py` & `optimum-1.8.6/optimum/exporters/onnx/__main__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/onnx/base.py` & `optimum-1.8.6/optimum/exporters/onnx/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/onnx/config.py` & `optimum-1.8.6/optimum/exporters/onnx/config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/onnx/constants.py` & `optimum-1.8.6/optimum/exporters/onnx/constants.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/onnx/convert.py` & `optimum-1.8.6/optimum/exporters/onnx/convert.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/onnx/model_configs.py` & `optimum-1.8.6/optimum/exporters/onnx/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/onnx/model_patcher.py` & `optimum-1.8.6/optimum/exporters/onnx/model_patcher.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/onnx/utils.py` & `optimum-1.8.6/optimum/exporters/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/tasks.py` & `optimum-1.8.6/optimum/exporters/tasks.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/tflite/__init__.py` & `optimum-1.8.6/optimum/exporters/tflite/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/tflite/__main__.py` & `optimum-1.8.6/optimum/exporters/tflite/__main__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/tflite/base.py` & `optimum-1.8.6/optimum/exporters/tflite/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/tflite/config.py` & `optimum-1.8.6/optimum/exporters/tflite/config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/tflite/convert.py` & `optimum-1.8.6/optimum/exporters/tflite/convert.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/exporters/tflite/model_configs.py` & `optimum-1.8.6/optimum/exporters/tflite/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/fx/__init__.py` & `optimum-1.8.6/optimum/fx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/fx/optimization/__init__.py` & `optimum-1.8.6/optimum/fx/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/fx/optimization/transformations.py` & `optimum-1.8.6/optimum/fx/optimization/transformations.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/fx/quantization/__init__.py` & `optimum-1.8.6/optimum/fx/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/fx/quantization/functions.py` & `optimum-1.8.6/optimum/fx/quantization/functions.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/fx/utils.py` & `optimum-1.8.6/optimum/fx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/modeling_base.py` & `optimum-1.8.6/optimum/modeling_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnx/__init__.py` & `optimum-1.8.6/optimum/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnx/configuration.py` & `optimum-1.8.6/optimum/onnx/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnx/graph_transformations.py` & `optimum-1.8.6/optimum/onnx/graph_transformations.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnx/modeling_seq2seq.py` & `optimum-1.8.6/optimum/onnx/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnx/transformations_utils.py` & `optimum-1.8.6/optimum/onnx/transformations_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnx/utils.py` & `optimum-1.8.6/optimum/onnx/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/__init__.py` & `optimum-1.8.6/optimum/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/base.py` & `optimum-1.8.6/optimum/onnxruntime/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/configuration.py` & `optimum-1.8.6/optimum/onnxruntime/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/constants.py` & `optimum-1.8.6/optimum/onnxruntime/constants.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/graph.py` & `optimum-1.8.6/optimum/onnxruntime/graph.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/io_binding/__init__.py` & `optimum-1.8.6/optimum/onnxruntime/io_binding/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/io_binding/io_binding_helper.py` & `optimum-1.8.6/optimum/onnxruntime/io_binding/io_binding_helper.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/model.py` & `optimum-1.8.6/optimum/onnxruntime/model.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/modeling_decoder.py` & `optimum-1.8.6/optimum/onnxruntime/modeling_decoder.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/modeling_diffusion.py` & `optimum-1.8.6/optimum/onnxruntime/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/modeling_ort.py` & `optimum-1.8.6/optimum/onnxruntime/modeling_ort.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/modeling_seq2seq.py` & `optimum-1.8.6/optimum/onnxruntime/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/optimization.py` & `optimum-1.8.6/optimum/onnxruntime/optimization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/preprocessors/__init__.py` & `optimum-1.8.6/optimum/onnxruntime/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/preprocessors/passes/__init__.py` & `optimum-1.8.6/optimum/onnxruntime/preprocessors/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/preprocessors/passes/excluders.py` & `optimum-1.8.6/optimum/onnxruntime/preprocessors/passes/excluders.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/preprocessors/passes/fully_connected.py` & `optimum-1.8.6/optimum/onnxruntime/preprocessors/passes/fully_connected.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/preprocessors/passes/gelu.py` & `optimum-1.8.6/optimum/onnxruntime/preprocessors/passes/gelu.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/preprocessors/passes/layernorm.py` & `optimum-1.8.6/optimum/onnxruntime/preprocessors/passes/layernorm.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/preprocessors/quantization.py` & `optimum-1.8.6/optimum/onnxruntime/preprocessors/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/quantization.py` & `optimum-1.8.6/optimum/onnxruntime/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/runs/__init__.py` & `optimum-1.8.6/optimum/onnxruntime/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/runs/calibrator.py` & `optimum-1.8.6/optimum/onnxruntime/runs/calibrator.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/runs/utils.py` & `optimum-1.8.6/optimum/onnxruntime/runs/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/trainer.py` & `optimum-1.8.6/optimum/onnxruntime/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/trainer_seq2seq.py` & `optimum-1.8.6/optimum/onnxruntime/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/training_args.py` & `optimum-1.8.6/optimum/onnxruntime/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/training_args_seq2seq.py` & `optimum-1.8.6/optimum/onnxruntime/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/onnxruntime/utils.py` & `optimum-1.8.6/optimum/onnxruntime/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/pipelines/__init__.py` & `optimum-1.8.6/optimum/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/pipelines/diffusers/pipeline_stable_diffusion.py` & `optimum-1.8.6/optimum/pipelines/diffusers/pipeline_stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/pipelines/diffusers/pipeline_utils.py` & `optimum-1.8.6/optimum/pipelines/diffusers/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/pipelines/pipelines_base.py` & `optimum-1.8.6/optimum/pipelines/pipelines_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/quantization_base.py` & `optimum-1.8.6/optimum/quantization_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/runs_base.py` & `optimum-1.8.6/optimum/runs_base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/__init__.py` & `optimum-1.8.6/optimum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/constant.py` & `optimum-1.8.6/optimum/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/doc.py` & `optimum-1.8.6/optimum/utils/doc.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/dummy_diffusers_objects.py` & `optimum-1.8.6/optimum/utils/dummy_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/file_utils.py` & `optimum-1.8.6/optimum/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/import_utils.py` & `optimum-1.8.6/optimum/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/input_generators.py` & `optimum-1.8.6/optimum/utils/input_generators.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/logging.py` & `optimum-1.8.6/optimum/utils/logging.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/modeling_utils.py` & `optimum-1.8.6/optimum/utils/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/normalized_config.py` & `optimum-1.8.6/optimum/utils/normalized_config.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/preprocessing/__init__.py` & `optimum-1.8.6/optimum/utils/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/preprocessing/base.py` & `optimum-1.8.6/optimum/utils/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/preprocessing/image_classification.py` & `optimum-1.8.6/optimum/utils/preprocessing/image_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/preprocessing/question_answering.py` & `optimum-1.8.6/optimum/utils/preprocessing/question_answering.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/preprocessing/task_processors_manager.py` & `optimum-1.8.6/optimum/utils/preprocessing/task_processors_manager.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/preprocessing/text_classification.py` & `optimum-1.8.6/optimum/utils/preprocessing/text_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/preprocessing/token_classification.py` & `optimum-1.8.6/optimum/utils/preprocessing/token_classification.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/runs.py` & `optimum-1.8.6/optimum/utils/runs.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/save_utils.py` & `optimum-1.8.6/optimum/utils/save_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/utils/testing_utils.py` & `optimum-1.8.6/optimum/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/optimum/version.py` & `optimum-1.8.6/optimum/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "1.8.5"
+__version__ = "1.8.6"
```

### Comparing `optimum-1.8.5/optimum.egg-info/PKG-INFO` & `optimum-1.8.6/optimum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum
-Version: 1.8.5
+Version: 1.8.6
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://github.com/huggingface/optimum
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,optimization,training,inference,onnx,onnx runtime,intel,habana,graphcore,neural compressor,ipu,hpu
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-1.8.5/optimum.egg-info/SOURCES.txt` & `optimum-1.8.6/optimum.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -116,10 +116,8 @@
 optimum/utils/testing_utils.py
 optimum/utils/preprocessing/__init__.py
 optimum/utils/preprocessing/base.py
 optimum/utils/preprocessing/image_classification.py
 optimum/utils/preprocessing/question_answering.py
 optimum/utils/preprocessing/task_processors_manager.py
 optimum/utils/preprocessing/text_classification.py
-optimum/utils/preprocessing/token_classification.py
-tests/test_configuration_utils.py
-tests/test_modeling_base.py
+optimum/utils/preprocessing/token_classification.py
```

### Comparing `optimum-1.8.5/optimum.egg-info/requires.txt` & `optimum-1.8.6/optimum.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/pyproject.toml` & `optimum-1.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-1.8.5/setup.py` & `optimum-1.8.6/setup.py`

 * *Files identical despite different names*

