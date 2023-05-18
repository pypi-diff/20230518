# Comparing `tmp/unstructured_inference-0.4.4.tar.gz` & `tmp/unstructured_inference-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.4.4.tar", last modified: Fri May  5 01:59:27 2023, max compression
+gzip compressed data, was "unstructured_inference-0.5.0.tar", last modified: Thu May 18 20:00:21 2023, max compression
```

## Comparing `unstructured_inference-0.4.4.tar` & `unstructured_inference-0.5.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.276872 unstructured_inference-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-05 01:59:27.276872 unstructured_inference-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.264872 unstructured_inference-0.4.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-05 01:59:27.276872 unstructured_inference-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.264872 unstructured_inference-0.4.4/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.268872 unstructured_inference-0.4.4/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.276872 unstructured_inference-0.4.4/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/yolox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.276872 unstructured_inference-0.4.4/unstructured_inference/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/patches/pdfminer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.268872 unstructured_inference-0.4.4/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-05 01:59:26.000000 unstructured_inference-0.4.4/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-05 01:59:27.000000 unstructured_inference-0.4.4/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:59:26.000000 unstructured_inference-0.4.4/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-05 01:59:26.000000 unstructured_inference-0.4.4/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 01:59:26.000000 unstructured_inference-0.4.4/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.187327 unstructured_inference-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-18 20:00:21.187327 unstructured_inference-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.175327 unstructured_inference-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-18 20:00:21.187327 unstructured_inference-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.175327 unstructured_inference-0.5.0/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.179327 unstructured_inference-0.5.0/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/inference/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.187327 unstructured_inference-0.5.0/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/detectron2onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/models/yolox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.187327 unstructured_inference-0.5.0/unstructured_inference/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/patches/pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-18 19:58:25.000000 unstructured_inference-0.5.0/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:00:21.179327 unstructured_inference-0.5.0/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-18 20:00:21.000000 unstructured_inference-0.5.0/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-18 20:00:21.000000 unstructured_inference-0.5.0/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 20:00:21.000000 unstructured_inference-0.5.0/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-18 20:00:21.000000 unstructured_inference-0.5.0/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 20:00:21.000000 unstructured_inference-0.5.0/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.4.4/README.md` & `unstructured_inference-0.5.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ### Package
 
 Run `pip install unstructured-inference`.
 
 ### Detectron2
 
-[Detectron2](https://github.com/facebookresearch/detectron2) is required for most inference tasks 
+[Detectron2](https://github.com/facebookresearch/detectron2) is required for using models from the [layoutparser model zoo](#using-models-from-the-layoutparser-model-zoo) 
 but is not automatically installed with this package. 
 For MacOS and Linux, build from source with:
 ```shell
 pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
 ```
 Other install options can be found in the 
 [Detectron2 installation guide](https://detectron2.readthedocs.io/en/latest/tutorials/install.html).
@@ -62,70 +62,38 @@
 print(layout.pages[0].elements)
 ```
 
 Once the model has detected the layout and OCR'd the document, the text extracted from the first 
 page of the sample document will be displayed.
 You can convert a given element to a `dict` by running the `.to_dict()` method.
 
-To build the Docker container, run `make docker-build`. Note that Apple hardware with an M1 chip 
-has trouble building `Detectron2` on Docker and for best results you should build it on Linux. To 
-run the API locally, use `make start-app-local`. You can stop the API with `make stop-app-local`. 
-The API will run at `http:/localhost:5000`. 
-You can then `POST` a PDF file to the API endpoint to see its layout with the command:
-```
-curl -X 'POST' 'http://localhost:5000/layout/default/pdf' -F 'file=@<your_pdf_file>' | jq -C . | less -R
-```
+## Models
 
-You can also choose the types of elements you want to return from the output of PDF parsing by 
-passing a list of types to the `include_elems` parameter. For example, if you only want to return 
-`Text` elements and `Title` elements, you can curl:
-```
-curl -X 'POST' 'http://localhost:5000/layout/default/pdf' \
--F 'file=@<your_pdf_file>' \
--F include_elems=Text \
--F include_elems=Title \
- | jq -C | less -R
-```
-If you are using an Apple M1 chip, use `make run-app-dev` instead of `make start-app-local` to 
-start the API with hot reloading. The API will run at `http:/localhost:8000`.
+The inference pipeline operates by finding text elements in a document page using a detection model, then extracting the contents of the elements using direct extraction (if available), OCR, and optionally table inference models.
 
-View the swagger documentation at `http://localhost:5000/docs`.
+We offer several detection models including [Detectron2](https://github.com/facebookresearch/detectron2) and [YOLOX](https://github.com/Megvii-BaseDetection/YOLOX).
 
-## YoloX model
+### Using a non-default model
 
-For using the YoloX model the endpoints are: 
-```
-http://localhost:8000/layout/yolox/pdf
-http://localhost:8000/layout/yolox/image
-```
-For example:
-```
-curl -X 'POST' 'http://localhost:8000/layout/yolox/image' \
--F 'file=@sample-docs/test-image.jpg' \
- | jq -C | less -R
-
-curl -X 'POST' 'http://localhost:8000/layout/yolox/pdf' \
--F 'file=@sample-docs/loremipsum.pdf' \
- | jq -C | less -R
-```
+When doing inference, an alternate model can be used by passing the model object to the ingestion method via the `model` parameter. The `get_model` function can be used to construct one of our out-of-the-box models from a keyword, e.g.:
+```python
+from unstructured_inference.models.base import get_model
+from unstructured_inference.inference.layout import DocumentLayout
 
-If your PDF file doesn't have text embedded you can force the use of OCR with
-the parameter force_ocr=True:
-```
-curl -X 'POST' 'http://localhost:8000/layout/yolox/pdf' \
--F 'file=@sample-docs/loremipsum-flat.pdf' \
--F force_ocr=true 
- | jq -C | less -R
+model = get_model("yolox")
+layout = DocumentLayout.from_file("sample-docs/layout-parser-paper.pdf", model=model)
 ```
 
-or in local:
+### Using models from the layoutparser model zoo
 
-```
-layout = yolox_local_inference(filename, type="pdf")
-```
+The `UnstructuredDetectronModel` class in `unstructured_inference.modelts.detectron2` uses the `faster_rcnn_R_50_FPN_3x` model pretrained on DocLayNet, but by using different construction parameters, any model in the `layoutparser` [model zoo](https://layout-parser.readthedocs.io/en/latest/notes/modelzoo.html) can be used. `UnstructuredDetectronModel` is a light wrapper around the `layoutparser` `Detectron2LayoutModel` object, and accepts the same arguments. See [layoutparser documentation](https://layout-parser.readthedocs.io/en/latest/api_doc/models.html#layoutparser.models.Detectron2LayoutModel) for details.
+
+### Using your own model
+
+Any detection model can be used for in the `unstructured_inference` pipeline by wrapping the model in the `UnstructuredObjectDetectionModel` class. To integrate with the `DocumentLayout` class, a subclass of `UnstructuredObjectDetectionModel` must have a `predict` method that accepts a `PIL.Image.Image` and returns a list of `LayoutElement`s, and an `initialize` method, which loads the model and prepares it for inference.
 
 ## Security Policy
 
 See our [security policy](https://github.com/Unstructured-IO/unstructured-inference/security/policy) for
 information on how to report security vulnerabilities.
 
 ## Learn more
```

### Comparing `unstructured_inference-0.4.4/setup.py` & `unstructured_inference-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from setuptools import setup, find_packages
+from typing import List
 
 from unstructured_inference.__version__ import __version__
 
 
 def load_requirements(file_list=None):
     if file_list is None:
         file_list = ["requirements/base.in"]
     if isinstance(file_list, str):
         file_list = [file_list]
-    requirements = []
+    requirements: List[str] = []
     for file in file_list:
-        if not file.startswith("#"):
-            with open(file, encoding="utf-8") as f:
-                requirements.extend(f.readlines())
+        with open(file, encoding="utf-8") as f:
+            requirements.extend(f.readlines())
+    requirements = [req for req in requirements if not req.startswith("#")]
     return requirements
 
 
 setup(
     name="unstructured_inference",
     description="A library for performing inference using trained models.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
```

### Comparing `unstructured_inference-0.4.4/unstructured_inference/inference/elements.py` & `unstructured_inference-0.5.0/unstructured_inference/inference/elements.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,24 @@
         return self.x2 - self.x1
 
     @property
     def height(self) -> Union[int, float]:
         """Height of rectangle"""
         return self.y2 - self.y1
 
+    @property
+    def x_midpoint(self) -> Union[int, float]:
+        """Finds the horizontal midpoint of the object."""
+        return (self.x2 + self.x1) / 2
+
+    @property
+    def y_midpoint(self) -> Union[int, float]:
+        """Finds the vertical midpoint of the object."""
+        return (self.y2 + self.y1) / 2
+
     def is_disjoint(self, other: Rectangle) -> bool:
         """Checks whether this rectangle is disjoint from another rectangle."""
         return not self.intersects(other)
 
     def intersects(self, other: Rectangle) -> bool:
         """Checks whether this rectangle intersects another rectangle."""
         return intersections(self, other)[0, 1]
```

### Comparing `unstructured_inference-0.4.4/unstructured_inference/inference/layout.py` & `unstructured_inference-0.5.0/unstructured_inference/inference/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from unstructured_inference.inference.elements import (
     TextRegion,
     EmbeddedTextRegion,
     ImageTextRegion,
 )
 from unstructured_inference.inference.layoutelement import LayoutElement
+from unstructured_inference.inference.ordering import order_layout
 from unstructured_inference.logger import logger
 from unstructured_inference.models.base import get_model
 from unstructured_inference.models.unstructuredmodel import UnstructuredModel
 from unstructured_inference.patches.pdfminer import parse_keyword
 
 # NOTE(alan): Patching this to fix a bug in pdfminer.six. Submitted this PR into pdfminer.six to fix
 # the bug: https://github.com/pdfminer/pdfminer.six/pull/885
@@ -99,15 +100,18 @@
         ocr_languages: str = "eng",
         fixed_layout: Optional[List[TextRegion]] = None,
         extract_tables: bool = False,
     ) -> DocumentLayout:
         """Creates a DocumentLayout from an image file."""
         logger.info(f"Reading image file: {filename} ...")
         try:
-            image = Image.open(filename).convert("RGB")
+            image = Image.open(filename)
+            format = image.format
+            image = image.convert("RGB")
+            image.format = format
         except Exception as e:
             if os.path.isdir(filename) or os.path.isfile(filename):
                 raise e
             else:
                 raise FileNotFoundError(f'File "{filename}" not found!') from e
         page = PageLayout.from_image(
             image,
@@ -163,17 +167,15 @@
             self.elements = elements
             return None
         return elements
 
     def get_elements_from_layout(self, layout: List[TextRegion]) -> List[LayoutElement]:
         """Uses the given Layout to separate the page text into elements, either extracting the
         text from the discovered layout blocks or from the image using OCR."""
-        # NOTE(robinson) - This orders the page from top to bottom. We'll need more
-        # sophisticated ordering logic for more complicated layouts.
-        layout.sort(key=lambda element: element.y1)
+        layout = order_layout(layout)
         elements = [
             get_element_from_block(
                 block=e,
                 image=self.image,
                 pdf_objects=self.layout,
                 ocr_strategy=self.ocr_strategy,
                 ocr_languages=self.ocr_languages,
```

### Comparing `unstructured_inference-0.4.4/unstructured_inference/inference/layoutelement.py` & `unstructured_inference-0.5.0/unstructured_inference/inference/layoutelement.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.4/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.5.0/unstructured_inference/models/detectron2.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 )
 from layoutparser.models.model_config import LayoutModelConfig
 from PIL import Image
 from huggingface_hub import hf_hub_download
 
 from unstructured_inference.logger import logger
 from unstructured_inference.inference.layoutelement import LayoutElement
-from unstructured_inference.models.unstructuredmodel import UnstructuredModel
+from unstructured_inference.models.unstructuredmodel import UnstructuredObjectDetectionModel
 from unstructured_inference.utils import LazyDict, LazyEvaluateInfo
 
 
 DETECTRON_CONFIG: Final = "lp://PubLayNet/faster_rcnn_R_50_FPN_3x/config"
 DEFAULT_LABEL_MAP: Final[Dict[int, str]] = {
     0: "Text",
     1: "Title",
@@ -25,15 +25,15 @@
 }
 DEFAULT_EXTRA_CONFIG: Final[List[Any]] = ["MODEL.ROI_HEADS.SCORE_THRESH_TEST", 0.8]
 
 
 # NOTE(alan): Entries are implemented as LazyDicts so that models aren't downloaded until they are
 # needed.
 MODEL_TYPES = {
-    None: LazyDict(
+    "detectron2_lp": LazyDict(
         model_path=LazyEvaluateInfo(
             hf_hub_download,
             "layoutparser/detectron2",
             "PubLayNet/faster_rcnn_R_50_FPN_3x/model_final.pth",
         ),
         config_path=LazyEvaluateInfo(
             hf_hub_download,
@@ -52,15 +52,15 @@
         ),
         label_map={0: "Unchecked", 1: "Checked"},
         extra_config=None,
     ),
 }
 
 
-class UnstructuredDetectronModel(UnstructuredModel):
+class UnstructuredDetectronModel(UnstructuredObjectDetectionModel):
     """Unstructured model wrapper for Detectron2LayoutModel."""
 
     def predict(self, x: Image):
         """Makes a prediction using detectron2 model."""
         super().predict(x)
         prediction = self.model.detect(x)
         return [LayoutElement.from_lp_textblock(block) for block in prediction]
```

### Comparing `unstructured_inference-0.4.4/unstructured_inference/models/donut.py` & `unstructured_inference-0.5.0/unstructured_inference/models/donut.py`

 * *Files 15% similar despite different names*

```diff
@@ -60,9 +60,13 @@
             eos_token_id=self.processor.tokenizer.eos_token_id,
             use_cache=True,
             num_beams=1,
             bad_words_ids=[[self.processor.tokenizer.unk_token_id]],
             return_dict_in_generate=True,
         )
         prediction = self.processor.batch_decode(outputs.sequences)[0]
+        # NOTE(alan): As of right now I think this would not work if passed in as the model to
+        # DocumentLayout.from_file and similar functions that take a model object as input. This
+        # produces image-to-text inferences rather than image-to-bboxes, so we actually need to
+        # hook it up in a different way.
         prediction = self.processor.token2json(prediction)
         return prediction
```

### Comparing `unstructured_inference-0.4.4/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.5.0/unstructured_inference/models/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.4/unstructured_inference/models/tables.py` & `unstructured_inference-0.5.0/unstructured_inference/models/tables.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.4/unstructured_inference/models/tesseract.py` & `unstructured_inference-0.5.0/unstructured_inference/models/tesseract.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.4/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.5.0/unstructured_inference/models/unstructuredmodel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+from __future__ import annotations
 from abc import ABC, abstractmethod
-from typing import Any
+from typing import TYPE_CHECKING, Any, List
+
+from PIL.Image import Image
+
+if TYPE_CHECKING:
+    from unstructured_inference.inference.layoutelement import LayoutElement
 
 
 class UnstructuredModel(ABC):
     """Wrapper class for the various models used by unstructured."""
 
     def __init__(self):
         """model should support inference of some sort, either by calling or by some method.
@@ -18,19 +24,33 @@
         if self.model is None:
             raise ModelNotInitializedError(
                 "Model has not been initialized. Please call the initialize method with the "
                 "appropriate arguments for loading the model."
             )
         pass  # pragma: no cover
 
-    def __call__(self, x: Any):
+    def __call__(self, x: Any) -> Any:
         """Inference using function call interface."""
         return self.predict(x)
 
     @abstractmethod
     def initialize(self, *args, **kwargs):
         """Load the model for inference."""
         pass  # pragma: no cover
 
 
+class UnstructuredObjectDetectionModel(UnstructuredModel):
+    """Wrapper class for object detection models used by unstructured."""
+
+    @abstractmethod
+    def predict(self, x: Image) -> List[LayoutElement]:
+        """Do inference using the wrapped model."""
+        super().predict(x)
+        return []  # pragma: no cover
+
+    def __call__(self, x: Image) -> List[LayoutElement]:
+        """Inference using function call interface."""
+        return super().__call__(x)
+
+
 class ModelNotInitializedError(Exception):
     pass
```

### Comparing `unstructured_inference-0.4.4/unstructured_inference/models/yolox.py` & `unstructured_inference-0.5.0/unstructured_inference/models/yolox.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.4/unstructured_inference/patches/pdfminer.py` & `unstructured_inference-0.5.0/unstructured_inference/patches/pdfminer.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.4/unstructured_inference/utils.py` & `unstructured_inference-0.5.0/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.4/unstructured_inference/visualize.py` & `unstructured_inference-0.5.0/unstructured_inference/visualize.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.4/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.5.0/unstructured_inference.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 requirements/base.in
 unstructured_inference/__init__.py
 unstructured_inference/__version__.py
-unstructured_inference/api.py
 unstructured_inference/logger.py
 unstructured_inference/utils.py
 unstructured_inference/visualize.py
 unstructured_inference.egg-info/PKG-INFO
 unstructured_inference.egg-info/SOURCES.txt
 unstructured_inference.egg-info/dependency_links.txt
 unstructured_inference.egg-info/requires.txt
 unstructured_inference.egg-info/top_level.txt
 unstructured_inference/inference/__init__.py
 unstructured_inference/inference/elements.py
 unstructured_inference/inference/layout.py
 unstructured_inference/inference/layoutelement.py
+unstructured_inference/inference/ordering.py
 unstructured_inference/models/__init__.py
 unstructured_inference/models/base.py
 unstructured_inference/models/detectron2.py
+unstructured_inference/models/detectron2onnx.py
 unstructured_inference/models/donut.py
 unstructured_inference/models/paddle_ocr.py
 unstructured_inference/models/table_postprocess.py
 unstructured_inference/models/tables.py
 unstructured_inference/models/tesseract.py
 unstructured_inference/models/unstructuredmodel.py
 unstructured_inference/models/yolox.py
```

