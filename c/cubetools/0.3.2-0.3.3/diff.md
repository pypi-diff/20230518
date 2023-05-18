# Comparing `tmp/cubetools-0.3.2.tar.gz` & `tmp/cubetools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubetools-0.3.2.tar", last modified: Thu May 18 04:09:20 2023, max compression
+gzip compressed data, was "dist/cubetools-0.3.3.tar", last modified: Thu May 18 05:05:10 2023, max compression
```

## Comparing `cubetools-0.3.2.tar` & `cubetools-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 04:09:20.000000 cubetools-0.3.2/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2109 2023-05-18 04:09:20.000000 cubetools-0.3.2/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1033 2023-04-03 13:20:28.000000 cubetools-0.3.2/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 04:09:20.000000 cubetools-0.3.2/cubetools/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.3.2/cubetools/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.3.2/cubetools/image_tools.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.3.2/cubetools/mindspore_lite_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.3.2/cubetools/onnx_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.3.2/cubetools/openvino_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.3.2/cubetools/paddle_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     7514 2023-05-18 04:07:01.000000 cubetools-0.3.2/cubetools/python_video_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.3.2/cubetools/video_capture.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3726 2023-03-23 06:14:20.000000 cubetools-0.3.2/cubetools/video_predict.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 04:09:20.000000 cubetools-0.3.2/cubetools.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2109 2023-05-18 04:09:20.000000 cubetools-0.3.2/cubetools.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      474 2023-05-18 04:09:20.000000 cubetools-0.3.2/cubetools.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-18 04:09:20.000000 cubetools-0.3.2/cubetools.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-05-18 04:09:20.000000 cubetools-0.3.2/cubetools.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-05-18 04:09:20.000000 cubetools-0.3.2/cubetools.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-05-18 04:09:20.000000 cubetools-0.3.2/cubetools.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-18 04:09:20.000000 cubetools-0.3.2/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-05-18 04:09:16.000000 cubetools-0.3.2/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 05:05:10.000000 cubetools-0.3.3/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2186 2023-05-18 05:05:10.000000 cubetools-0.3.3/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1094 2023-05-18 05:05:06.000000 cubetools-0.3.3/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 05:05:10.000000 cubetools-0.3.3/cubetools/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.3.3/cubetools/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.3.3/cubetools/image_tools.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.3.3/cubetools/mindspore_lite_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.3.3/cubetools/onnx_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.3.3/cubetools/openvino_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.3.3/cubetools/paddle_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     7514 2023-05-18 04:59:48.000000 cubetools-0.3.3/cubetools/python_video_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.3.3/cubetools/video_capture.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3726 2023-03-23 06:14:20.000000 cubetools-0.3.3/cubetools/video_predict.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 05:05:10.000000 cubetools-0.3.3/cubetools.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2186 2023-05-18 05:05:10.000000 cubetools-0.3.3/cubetools.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      474 2023-05-18 05:05:10.000000 cubetools-0.3.3/cubetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-18 05:05:10.000000 cubetools-0.3.3/cubetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-05-18 05:05:10.000000 cubetools-0.3.3/cubetools.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-05-18 05:05:10.000000 cubetools-0.3.3/cubetools.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-05-18 05:05:10.000000 cubetools-0.3.3/cubetools.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-18 05:05:10.000000 cubetools-0.3.3/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-05-18 05:05:06.000000 cubetools-0.3.3/setup.py
```

### Comparing `cubetools-0.3.2/PKG-INFO` & `cubetools-0.3.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.3.2
+Version: 0.3.3
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
         
         [CubeAI智立方](https://openi.pcl.ac.cn/OpenI/cubeai) 模型和应用开发常用工具集。
         
         目前主要包括：
         
         - 图像前处理、后处理常用函数封装。
         - 支持多路视频流媒体在线AI流式服务的通用SDK组件。
+        - 基于Gradio的视频流媒体类Python前端SDK组件。
         - 基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装的通用OpenVino模型推理器。
         - 基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装的通用ONNX模型推理器。
         - 基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装的通用PaddlePaddle模型推理器。
         - 基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装的通用MindSporeLite推理器。
         
+        
         ## 开源主页
         
         - https://openi.pcl.ac.cn/cubeai/cubetools
         
         ## 依赖包主页 
         
         - https://pypi.org/project/cubetools
```

### Comparing `cubetools-0.3.2/README.md` & `cubetools-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 [CubeAI智立方](https://openi.pcl.ac.cn/OpenI/cubeai) 模型和应用开发常用工具集。
 
 目前主要包括：
 
 - 图像前处理、后处理常用函数封装。
 - 支持多路视频流媒体在线AI流式服务的通用SDK组件。
+- 基于Gradio的视频流媒体类Python前端SDK组件。
 - 基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装的通用OpenVino模型推理器。
 - 基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装的通用ONNX模型推理器。
 - 基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装的通用PaddlePaddle模型推理器。
 - 基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装的通用MindSporeLite推理器。
 
+
 ## 开源主页
 
 - https://openi.pcl.ac.cn/cubeai/cubetools
 
 ## 依赖包主页 
 
 - https://pypi.org/project/cubetools
```

### Comparing `cubetools-0.3.2/cubetools/image_tools.py` & `cubetools-0.3.3/cubetools/image_tools.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.2/cubetools/mindspore_lite_predict.py` & `cubetools-0.3.3/cubetools/mindspore_lite_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.2/cubetools/onnx_predict.py` & `cubetools-0.3.3/cubetools/onnx_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.2/cubetools/openvino_predict.py` & `cubetools-0.3.3/cubetools/openvino_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.2/cubetools/paddle_predict.py` & `cubetools-0.3.3/cubetools/paddle_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.2/cubetools/python_video_frontend.py` & `cubetools-0.3.3/cubetools/python_video_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.2/cubetools/video_capture.py` & `cubetools-0.3.3/cubetools/video_capture.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.2/cubetools/video_predict.py` & `cubetools-0.3.3/cubetools/video_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.2/cubetools.egg-info/PKG-INFO` & `cubetools-0.3.3/cubetools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.3.2
+Version: 0.3.3
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
         
         [CubeAI智立方](https://openi.pcl.ac.cn/OpenI/cubeai) 模型和应用开发常用工具集。
         
         目前主要包括：
         
         - 图像前处理、后处理常用函数封装。
         - 支持多路视频流媒体在线AI流式服务的通用SDK组件。
+        - 基于Gradio的视频流媒体类Python前端SDK组件。
         - 基于 [OpenVino Runtime](https://pypi.org/project/openvino/) 封装的通用OpenVino模型推理器。
         - 基于 [ONNX Runtime](https://pypi.org/project/onnxruntime-gpu/) 封装的通用ONNX模型推理器。
         - 基于 [Paddle Inference](https://www.paddlepaddle.org.cn/paddle/paddleinference) 推理引擎封装的通用PaddlePaddle模型推理器。
         - 基于 [MindSpore Lite](https://www.mindspore.cn/lite) 推理引擎封装的通用MindSporeLite推理器。
         
+        
         ## 开源主页
         
         - https://openi.pcl.ac.cn/cubeai/cubetools
         
         ## 依赖包主页 
         
         - https://pypi.org/project/cubetools
```

### Comparing `cubetools-0.3.2/setup.py` & `cubetools-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='cubetools',
-    version='0.3.2',
+    version='0.3.3',
     author='cubeai',
     author_email='cubeai@163.com',
     description='CubeAI模型开发常用工具集',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

