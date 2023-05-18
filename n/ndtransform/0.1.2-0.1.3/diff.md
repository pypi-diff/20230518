# Comparing `tmp/ndtransform-0.1.2.tar.gz` & `tmp/ndtransform-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndtransform-0.1.2.tar", max compression
+gzip compressed data, was "ndtransform-0.1.3.tar", max compression
```

## Comparing `ndtransform-0.1.2.tar` & `ndtransform-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-05-09 18:11:01.209245 ndtransform-0.1.2/ndtransform/__init__.py
--rw-r--r--   0        0        0     3319 2023-05-15 16:42:44.989556 ndtransform-0.1.2/ndtransform/nDtransform_lib.py
--rw-r--r--   0        0        0      299 2023-05-15 17:22:11.567582 ndtransform-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1001 2023-05-15 17:13:32.639084 ndtransform-0.1.2/README.md
--rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 ndtransform-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-09 18:11:01.209245 ndtransform-0.1.3/ndtransform/__init__.py
+-rw-r--r--   0        0        0     3673 2023-05-18 16:28:57.385772 ndtransform-0.1.3/ndtransform/nDtransform_lib.py
+-rw-r--r--   0        0        0      299 2023-05-18 16:29:03.806236 ndtransform-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      999 2023-05-18 15:46:00.840221 ndtransform-0.1.3/README.md
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 ndtransform-0.1.3/PKG-INFO
```

### Comparing `ndtransform-0.1.2/ndtransform/nDtransform_lib.py` & `ndtransform-0.1.3/ndtransform/nDtransform_lib.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
+from typing import List
 from dataclasses import dataclass
 
 @dataclass
 class Tensor:
     '''This class provides basic framework for inputing tensors. Simple enforsment of type on input'''
-    tensor_2d: list[list[float]]
+    tensor_2d: List[List[float]]
 
 @dataclass
 class TimeSeries:
     '''Time series needs to have multiple inputs, 2 of which(shift and stride) need to have a default
     of 1. This class is used as enforcement of types. array and size must be provided in input.
     '''
     array: list|np.ndarray
@@ -23,49 +24,65 @@
     matrix: np.ndarray
     kernel: np.ndarray
     stride: int = 1
 
 def transpose2d(tensor):
     '''This function transposes provided tensor using 2 for loops, by going through provided list.'''
     Tensor.tensor_2d = tensor
-    transposed_row = [[Tensor.tensor_2d[row][value] 
+    transposed_row = [[float(Tensor.tensor_2d[row][value]) 
                         for row in range(len(Tensor.tensor_2d))] 
                         for value in range(len(Tensor.tensor_2d[0]))]
     return transposed_row
 
 
 def window1d(array, size, *args) -> list[list | np.ndarray]:
     '''window1d function uses TimeSeries class and calculates window of provided array akin to TensorFlow
         tf.data.Dataset.range(n).window(m) function.
     '''
     input_seq = TimeSeries(array,size,*args)
     result_win = []
-    start = [i for i in range(0,len(input_seq.array),input_seq.shift)]
-    for position in range(len(start)):
-        value = input_seq.array[start[position]:start[position] + input_seq.size*input_seq.stride: input_seq.stride ]
+    starting_positions = [i for i in range(0,len(input_seq.array),input_seq.shift)]
+
+    for position in range(len(starting_positions)):
+        value = input_seq.array[starting_positions[position]
+                                :starting_positions[position] + input_seq.size * input_seq.stride
+                                : input_seq.stride ]
         result_win.append(value)
     return result_win
                 
 
 def convolution2d(matrix, kernel, *args) -> np.ndarray:
     '''convolution2d takes in 2 arrays and 1 optional argument of stride and calculates cross-correlation operation
     it utilizes 2 for loops to iterate through target matrix and calculate sums of each iterations multiplications.
     Stride argument is there in case there is a need to iterate only on matrices after some steps.
     '''
     input_args = Convolution(matrix, kernel, *args)
 
+
+    '''Here will be stored all relevant values as a higher dimensional overview. Source is class Convolution.'''
+    stride = input_args.stride
+
+    matrix_full = input_args.matrix
+    kernel_full = input_args.kernel
+
+    matrix_1d_shape = input_args.matrix.shape[0]
+    kernel_1d_shape = input_args.kernel.shape[0]
+    matrix_2d_shape = input_args.matrix.shape[1]
+    kernel_2d_shape = input_args.kernel.shape[1]
+
+
     result = []
-    for point_1 in range(0,input_args.matrix.shape[0] - input_args.kernel.shape[0] + 1, input_args.stride):
-            for point_2 in range(0,input_args.matrix.shape[1] - input_args.kernel.shape[1] + 1, input_args.stride):
+    for point_1 in range(0,matrix_1d_shape - kernel_1d_shape + 1, stride):
+            for point_2 in range(0,matrix_2d_shape - kernel_2d_shape + 1, stride):
                 value = 0
-                gen_matrix = input_args.matrix[point_1:point_1 + np.size(input_args.kernel,0) 
-                                                 ,point_2:point_2 + np.size(input_args.kernel,1) 
+                gen_matrix = matrix_full[point_1:point_1 + np.size(kernel_full, 0) 
+                                                 ,point_2:point_2 + np.size(kernel_full, 1) 
                                                  ] 
-                if gen_matrix.shape == input_args.kernel.shape :
-                    for i in range(len(input_args.kernel)):
-                        value = value + sum(gen_matrix[i] * np.array(input_args.kernel[i]))
+                if gen_matrix.shape == kernel_full.shape :
+                    value = np.sum(np.multiply(gen_matrix, kernel_full))
+
                     result.append(value)
 
-    return np.ndarray(shape=((input_args.matrix.shape[0] - input_args.kernel.shape[0])//input_args.stride + 1, 
-                             (input_args.matrix.shape[1] - input_args.kernel.shape[1])//input_args.stride + 1)
+    return np.ndarray(shape=((matrix_1d_shape - kernel_1d_shape)//stride + 1, 
+                             (matrix_2d_shape - kernel_2d_shape)//stride + 1)
                              ,buffer = np.array(result), dtype=int)
```

### Comparing `ndtransform-0.1.2/README.md` & `ndtransform-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 This library contains 3 functions that are meant to be used for tensor transformations. 
 Mostly they are built using standard python library with some functionalities of numpy.
 
 The 3 functions in question:
-
 -transpose2d(tensor): takes a tensor in the format "list[list[float]]". This tensor will
 then be transposed. Returns a list.
 
 -window1d(array, size, *shift, *stride): "array" takes an array in format list or np.ndarray;
 "size", of which size you want to get your windows; "shift" (default = 1) optional argument, which 
 determines step in between window calculations; "stride" (default = 1) optional argument, which 
 represents the step size. Returns a list.
```

### Comparing `ndtransform-0.1.2/PKG-INFO` & `ndtransform-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: ndtransform
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: sevolek
 Author-email: ale.sev@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 This library contains 3 functions that are meant to be used for tensor transformations. 
 Mostly they are built using standard python library with some functionalities of numpy.
 
 The 3 functions in question:
-
 -transpose2d(tensor): takes a tensor in the format "list[list[float]]". This tensor will
 then be transposed. Returns a list.
 
 -window1d(array, size, *shift, *stride): "array" takes an array in format list or np.ndarray;
 "size", of which size you want to get your windows; "shift" (default = 1) optional argument, which 
 determines step in between window calculations; "stride" (default = 1) optional argument, which 
 represents the step size. Returns a list.
```

