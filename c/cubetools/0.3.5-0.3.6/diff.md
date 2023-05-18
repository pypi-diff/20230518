# Comparing `tmp/cubetools-0.3.5.tar.gz` & `tmp/cubetools-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubetools-0.3.5.tar", last modified: Thu May 18 06:41:49 2023, max compression
+gzip compressed data, was "dist/cubetools-0.3.6.tar", last modified: Thu May 18 07:08:58 2023, max compression
```

## Comparing `cubetools-0.3.5.tar` & `cubetools-0.3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 06:41:49.000000 cubetools-0.3.5/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2185 2023-05-18 06:41:49.000000 cubetools-0.3.5/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1093 2023-05-18 06:41:19.000000 cubetools-0.3.5/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 06:41:49.000000 cubetools-0.3.5/cubetools/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.3.5/cubetools/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.3.5/cubetools/image_tools.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.3.5/cubetools/mindspore_lite_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.3.5/cubetools/onnx_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.3.5/cubetools/openvino_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.3.5/cubetools/paddle_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     7513 2023-05-18 06:41:19.000000 cubetools-0.3.5/cubetools/python_video_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.3.5/cubetools/video_capture.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3726 2023-03-23 06:14:20.000000 cubetools-0.3.5/cubetools/video_predict.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 06:41:49.000000 cubetools-0.3.5/cubetools.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2185 2023-05-18 06:41:49.000000 cubetools-0.3.5/cubetools.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      474 2023-05-18 06:41:49.000000 cubetools-0.3.5/cubetools.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-18 06:41:49.000000 cubetools-0.3.5/cubetools.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-05-18 06:41:49.000000 cubetools-0.3.5/cubetools.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-05-18 06:41:49.000000 cubetools-0.3.5/cubetools.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-05-18 06:41:49.000000 cubetools-0.3.5/cubetools.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-18 06:41:49.000000 cubetools-0.3.5/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-05-18 06:41:19.000000 cubetools-0.3.5/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 07:08:58.000000 cubetools-0.3.6/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2185 2023-05-18 07:08:58.000000 cubetools-0.3.6/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1093 2023-05-18 06:45:24.000000 cubetools-0.3.6/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.3.6/cubetools/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.3.6/cubetools/image_tools.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.3.6/cubetools/mindspore_lite_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.3.6/cubetools/onnx_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.3.6/cubetools/openvino_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.3.6/cubetools/paddle_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     7658 2023-05-18 07:07:26.000000 cubetools-0.3.6/cubetools/python_video_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.3.6/cubetools/video_capture.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3726 2023-03-23 06:14:20.000000 cubetools-0.3.6/cubetools/video_predict.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2185 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      474 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        5 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       27 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       10 2023-05-18 07:08:58.000000 cubetools-0.3.6/cubetools.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-18 07:08:58.000000 cubetools-0.3.6/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2192 2023-05-18 07:07:27.000000 cubetools-0.3.6/setup.py
```

### Comparing `cubetools-0.3.5/PKG-INFO` & `cubetools-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.3.5
+Version: 0.3.6
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
```

### Comparing `cubetools-0.3.5/README.md` & `cubetools-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.5/cubetools/image_tools.py` & `cubetools-0.3.6/cubetools/image_tools.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.5/cubetools/mindspore_lite_predict.py` & `cubetools-0.3.6/cubetools/mindspore_lite_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.5/cubetools/onnx_predict.py` & `cubetools-0.3.6/cubetools/onnx_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.5/cubetools/openvino_predict.py` & `cubetools-0.3.6/cubetools/openvino_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.5/cubetools/paddle_predict.py` & `cubetools-0.3.6/cubetools/paddle_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.5/cubetools/python_video_frontend.py` & `cubetools-0.3.6/cubetools/python_video_frontend.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,20 @@
 
                     examples = [['rtsp://localhost:8554/stream'], ['rtmp://localhost/stream/live']]
                     for example in video_examples:
                         examples.append([example])
                     gr.Examples(label='URL示例', examples=examples, inputs=[self.url])
 
             gr.Markdown('<br/>')
-            api_text = gen_api_docs(self.predict, self.predict_video)
+            args = []
+            if local_image:
+                args.append(self.predict)
+            if streaming_video:
+                args.append(self.predict_video)
+            api_text = gen_api_docs(*args)
             btn_show_api = gr.Button(value='显示API文档')
             btn_hide_api = gr.Button(value='隐藏API文档', visible=False)
             api_docs = gr.Markdown(api_text, visible=False)
             btn_show_api.click(lambda: (btn_show_api.update(visible=False), btn_hide_api.update(visible=True), api_docs.update(visible=True)),
                                outputs=[btn_show_api, btn_hide_api, api_docs])
             btn_hide_api.click(lambda: (btn_show_api.update(visible=True), btn_hide_api.update(visible=False), api_docs.update(visible=False)),
                                outputs=[btn_show_api, btn_hide_api, api_docs])
```

### Comparing `cubetools-0.3.5/cubetools/video_capture.py` & `cubetools-0.3.6/cubetools/video_capture.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.5/cubetools/video_predict.py` & `cubetools-0.3.6/cubetools/video_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.3.5/cubetools.egg-info/PKG-INFO` & `cubetools-0.3.6/cubetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.3.5
+Version: 0.3.6
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
```

### Comparing `cubetools-0.3.5/setup.py` & `cubetools-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='cubetools',
-    version='0.3.5',
+    version='0.3.6',
     author='cubeai',
     author_email='cubeai@163.com',
     description='CubeAI模型开发常用工具集',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

