# Comparing `tmp/sports2d-0.1.0.tar.gz` & `tmp/sports2d-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports2d-0.1.0.tar", last modified: Tue May  9 15:10:26 2023, max compression
+gzip compressed data, was "sports2d-0.1.2.tar", last modified: Thu May 18 08:20:03 2023, max compression
```

## Comparing `sports2d-0.1.0.tar` & `sports2d-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:26.635247 sports2d-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-09 15:10:16.000000 sports2d-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-09 15:10:26.635247 sports2d-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12773 2023-05-09 15:10:16.000000 sports2d-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:26.631247 sports2d-0.1.0/Sports2D/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:26.631247 sports2d-0.1.0/Sports2D/Demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Demo/Config_demo.toml
--rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Demo/demo.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Sports2D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:26.635247 sports2d-0.1.0/Sports2D/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Utilities/Blazepose_runsave.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Utilities/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Utilities/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Utilities/skeletons.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/Utilities/test_with_blazepose.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/compute_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    23753 2023-05-09 15:10:16.000000 sports2d-0.1.0/Sports2D/detect_pose.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-09 15:10:16.000000 sports2d-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-09 15:10:26.635247 sports2d-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-09 15:10:16.000000 sports2d-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:10:26.635247 sports2d-0.1.0/sports2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-09 15:10:26.000000 sports2d-0.1.0/sports2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-09 15:10:26.000000 sports2d-0.1.0/sports2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:10:26.000000 sports2d-0.1.0/sports2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:10:26.000000 sports2d-0.1.0/sports2d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 15:10:26.000000 sports2d-0.1.0/sports2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 15:10:26.000000 sports2d-0.1.0/sports2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:03.880555 sports2d-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-18 08:19:50.000000 sports2d-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-05-18 08:20:03.880555 sports2d-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-05-18 08:19:50.000000 sports2d-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:03.872554 sports2d-0.1.2/Sports2D/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:03.872554 sports2d-0.1.2/Sports2D/Demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-18 08:19:50.000000 sports2d-0.1.2/Sports2D/Demo/Config_demo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-05-18 08:19:50.000000 sports2d-0.1.2/Sports2D/Demo/demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-18 08:19:50.000000 sports2d-0.1.2/Sports2D/Sports2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:03.876554 sports2d-0.1.2/Sports2D/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-18 08:19:50.000000 sports2d-0.1.2/Sports2D/Utilities/Blazepose_runsave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 08:19:50.000000 sports2d-0.1.2/Sports2D/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-18 08:19:50.000000 sports2d-0.1.2/Sports2D/Utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-18 08:19:50.000000 sports2d-0.1.2/Sports2D/Utilities/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-05-18 08:19:50.000000 sports2d-0.1.2/Sports2D/Utilities/skeletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-18 08:19:50.000000 sports2d-0.1.2/Sports2D/Utilities/test_with_blazepose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 08:19:50.000000 sports2d-0.1.2/Sports2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-05-18 08:19:50.000000 sports2d-0.1.2/Sports2D/compute_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23913 2023-05-18 08:19:50.000000 sports2d-0.1.2/Sports2D/detect_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-18 08:19:50.000000 sports2d-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-18 08:20:03.880555 sports2d-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-18 08:19:50.000000 sports2d-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 08:20:03.880555 sports2d-0.1.2/sports2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-05-18 08:20:03.000000 sports2d-0.1.2/sports2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-18 08:20:03.000000 sports2d-0.1.2/sports2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:20:03.000000 sports2d-0.1.2/sports2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 08:20:03.000000 sports2d-0.1.2/sports2d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-18 08:20:03.000000 sports2d-0.1.2/sports2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 08:20:03.000000 sports2d-0.1.2/sports2d.egg-info/top_level.txt
```

### Comparing `sports2d-0.1.0/LICENSE` & `sports2d-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sports2d-0.1.0/PKG-INFO` & `sports2d-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.1.0
+Version: 0.1.2
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
@@ -23,25 +23,25 @@
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
 Requires-Python: <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
-[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D)\
+[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D)
+[![Downloads](https://static.pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)\
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![DOI](https://zenodo.org/badge/634044634.svg)](https://zenodo.org/badge/latestdoi/634044634)\
 <a href="https://colab.research.google.com/github/davidpagnon/Sports2D/blob/main/Sports2D/Sports2D.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
-<!-- [![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
-[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
+<!-- [![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
 [![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
-[![DOI](https://zenodo.org/badge/501642916.svg)](https://zenodo.org/badge/latestdoi/501642916)
+[![status](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26/status.svg)](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26)
 -->
 
 
 # Sports2D
 
 **`Sports2D` lets you compute 2D joint and segment angles from a video.**
 
@@ -143,15 +143,15 @@
 Similarly, if you launch Sports2D in an other directory, specify the location of the config file this way: `Sports2D.detect_pose(<path_to_Config_demo.toml>)`\
 In `pose`, specify the use of BlazePose or OpenPose as joint detectors: this will be detailed in the next section.\
 In `compute_angles`, select your angles of interest.
 
 
 ### Use OpenPose for multi-person, more accurate analysis
 
-OpenPose is slower than OpenPose, but more accurate. It also allows for the detection of multiple persons, whose indices are consistent across frames. 
+OpenPose is slower than BlazePose, but usually more accurate. It also allows for the detection of multiple persons, whose indices are consistent across frames. 
 
 1. **Install OpenPose** (instructions [there](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md)). \
 *Windows portable demo works fine.*
 
 2. If you want even more accurate results, use the BODY_25B experimental model instead of the standard BODY_25 one. This requires manually [downloading the model](https://github.com/CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/README.md). You can optionally download from there the BODY_135 model which will let you compute wrist flexion and hand segment angle, however this will be much slower.
 
 3. In `Config_demo.toml` → `pose.OPENPOSE`, specify your OpenPose model, and the path where you downloaded OpenPose.
@@ -255,14 +255,15 @@
 - [ ] Full test on **MacOS**.
 - [ ] **GUI applications** for Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with [Kivy](https://kivy.org).
 - [ ] **Include OpenPose** in Sports2D executable files. [Dockerize](https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile) it? 
 - [ ] **Track other points and angles** with classic tracking methods (cf. [Kinovea](https://www.kinovea.org/features.html)), or by training a model (cf. [DeepLabCut](https://deeplabcut.github.io/DeepLabCut/README.html)).
 - [ ] **Pose refinement**. Click and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/watch?v=bEuBKB7eqmk) for inspiration.
 - [ ] **Constrain points** to OpenSim skeletal model for better angle estimation (like with [Pose2Sim](https://github.com/perfanalytics/pose2sim), but in 2D.
 - [ ] Add tools for annotating images, undistort them, take perspective into account, etc. (cf. [Kinovea](https://www.kinovea.org/features.html)).
+- [ ] Check other methods for sorting people across frames ([STAF](https://github.com/soulslicer/STAF/tree/staf) or [LivePoseTracker](https://github.com/ortegatron/liveposetracker).
 
 BSD 3-Clause License
 
 Copyright (c) 2022, perfanalytics
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sports2d Version: 0.1.0 Summary: Detect pose and
+Metadata-Version: 2.1 Name: sports2d Version: 0.1.2 Summary: Detect pose and
 compute 2D joint angles from a video. Home-page: https://github.com/
 davidpagnon/Sports2D Author: David Pagnon Author-email: contact@david-
 pagnon.com License: BSD 3-Clause License Project-URL: Bug Tracker, https://
 github.com/davidpagnon/Sports2D/issues Keywords:
 markerless,kinematics,OpenPose,BlazePose,joint
 angles,2D,biomechanics,sports,sports-analytics Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,16 @@
 Engineering :: Medical Science Apps. Classifier: Topic :: Multimedia ::
 Graphics Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling Requires-
 Python: <3.11 Description-Content-Type: text/markdown License-File: LICENSE [!
 [Continuous integration](https://github.com/davidpagnon/sports2d/actions/
 workflows/continuous-integration.yml/badge.svg?branch=main)](https://
 github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/
-py/Sports2D)\ [![Open Source? Yes!](https://badgen.net/badge/
+py/Sports2D) [![Downloads](https://static.pepy.tech/badge/sports2d)](https://
+pepy.tech/project/sports2d)\ [![Open Source? Yes!](https://badgen.net/badge/
 Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/
 badges/) [![License](https://img.shields.io/badge/License-BSD_3--Clause-
 blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![DOI](https://
 zenodo.org/badge/634044634.svg)](https://zenodo.org/badge/latestdoi/634044634)\
 [Open_In_Colab]  # Sports2D **`Sports2D` lets you compute 2D joint and segment
 angles from a video.** [Content/demo_gif.gif] `Warning:` Angle estimation is
 only as good as the pose estimation algorithm, i.e., it is not perfect.\
@@ -76,18 +77,18 @@
 *Optionally:* If your video is not in the same folder as `Config_demo.toml`,
 specify its location in `video_dir`.\ Similarly, if you launch Sports2D in an
 other directory, specify the location of the config file this way:
 `Sports2D.detect_pose(
 toml>)`\ In `pose`, specify the use of BlazePose or OpenPose as joint
 detectors: this will be detailed in the next section.\ In `compute_angles`,
 select your angles of interest. ### Use OpenPose for multi-person, more
-accurate analysis OpenPose is slower than OpenPose, but more accurate. It also
-allows for the detection of multiple persons, whose indices are consistent
-across frames. 1. **Install OpenPose** (instructions [there](https://
-github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/
+accurate analysis OpenPose is slower than BlazePose, but usually more accurate.
+It also allows for the detection of multiple persons, whose indices are
+consistent across frames. 1. **Install OpenPose** (instructions [there](https:/
+/github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/
 0_index.md)). \ *Windows portable demo works fine.* 2. If you want even more
 accurate results, use the BODY_25B experimental model instead of the standard
 BODY_25 one. This requires manually [downloading the model](https://github.com/
 CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/
 README.md). You can optionally download from there the BODY_135 model which
 will let you compute wrist flexion and hand segment angle, however this will be
 much slower. 3. In `Config_demo.toml` â `pose.OPENPOSE`, specify your
@@ -160,27 +161,30 @@
 features.html)), or by training a model (cf. [DeepLabCut](https://
 deeplabcut.github.io/DeepLabCut/README.html)). - [ ] **Pose refinement**. Click
 and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/
 watch?v=bEuBKB7eqmk) for inspiration. - [ ] **Constrain points** to OpenSim
 skeletal model for better angle estimation (like with [Pose2Sim](https://
 github.com/perfanalytics/pose2sim), but in 2D. - [ ] Add tools for annotating
 images, undistort them, take perspective into account, etc. (cf. [Kinovea]
-(https://www.kinovea.org/features.html)). BSD 3-Clause License Copyright (c)
-2022, perfanalytics All rights reserved. Redistribution and use in source and
-binary forms, with or without modification, are permitted provided that the
-following conditions are met: 1. Redistributions of source code must retain the
-above copyright notice, this list of conditions and the following disclaimer.
-2. Redistributions in binary form must reproduce the above copyright notice,
-this list of conditions and the following disclaimer in the documentation and/
-or other materials provided with the distribution. 3. Neither the name of the
-copyright holder nor the names of its contributors may be used to endorse or
-promote products derived from this software without specific prior written
-permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
-LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
-GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+(https://www.kinovea.org/features.html)). - [ ] Check other methods for sorting
+people across frames ([STAF](https://github.com/soulslicer/STAF/tree/staf) or
+[LivePoseTracker](https://github.com/ortegatron/liveposetracker). BSD 3-Clause
+License Copyright (c) 2022, perfanalytics All rights reserved. Redistribution
+and use in source and binary forms, with or without modification, are permitted
+provided that the following conditions are met: 1. Redistributions of source
+code must retain the above copyright notice, this list of conditions and the
+following disclaimer. 2. Redistributions in binary form must reproduce the
+above copyright notice, this list of conditions and the following disclaimer in
+the documentation and/or other materials provided with the distribution. 3.
+Neither the name of the copyright holder nor the names of its contributors may
+be used to endorse or promote products derived from this software without
+specific prior written permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT
+HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
+INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
+FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
+COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
+INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
+PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
+ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `sports2d-0.1.0/README.md` & `sports2d-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
 [![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
-[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D)\
+[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D)
+[![Downloads](https://static.pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)\
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![DOI](https://zenodo.org/badge/634044634.svg)](https://zenodo.org/badge/latestdoi/634044634)\
 <a href="https://colab.research.google.com/github/davidpagnon/Sports2D/blob/main/Sports2D/Sports2D.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
-<!-- [![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
-[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
+<!-- [![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
 [![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
-[![DOI](https://zenodo.org/badge/501642916.svg)](https://zenodo.org/badge/latestdoi/501642916)
+[![status](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26/status.svg)](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26)
 -->
 
 
 # Sports2D
 
 **`Sports2D` lets you compute 2D joint and segment angles from a video.**
 
@@ -116,15 +116,15 @@
 Similarly, if you launch Sports2D in an other directory, specify the location of the config file this way: `Sports2D.detect_pose(<path_to_Config_demo.toml>)`\
 In `pose`, specify the use of BlazePose or OpenPose as joint detectors: this will be detailed in the next section.\
 In `compute_angles`, select your angles of interest.
 
 
 ### Use OpenPose for multi-person, more accurate analysis
 
-OpenPose is slower than OpenPose, but more accurate. It also allows for the detection of multiple persons, whose indices are consistent across frames. 
+OpenPose is slower than BlazePose, but usually more accurate. It also allows for the detection of multiple persons, whose indices are consistent across frames. 
 
 1. **Install OpenPose** (instructions [there](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md)). \
 *Windows portable demo works fine.*
 
 2. If you want even more accurate results, use the BODY_25B experimental model instead of the standard BODY_25 one. This requires manually [downloading the model](https://github.com/CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/README.md). You can optionally download from there the BODY_135 model which will let you compute wrist flexion and hand segment angle, however this will be much slower.
 
 3. In `Config_demo.toml` → `pose.OPENPOSE`, specify your OpenPose model, and the path where you downloaded OpenPose.
@@ -228,7 +228,8 @@
 - [ ] Full test on **MacOS**.
 - [ ] **GUI applications** for Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with [Kivy](https://kivy.org).
 - [ ] **Include OpenPose** in Sports2D executable files. [Dockerize](https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile) it? 
 - [ ] **Track other points and angles** with classic tracking methods (cf. [Kinovea](https://www.kinovea.org/features.html)), or by training a model (cf. [DeepLabCut](https://deeplabcut.github.io/DeepLabCut/README.html)).
 - [ ] **Pose refinement**. Click and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/watch?v=bEuBKB7eqmk) for inspiration.
 - [ ] **Constrain points** to OpenSim skeletal model for better angle estimation (like with [Pose2Sim](https://github.com/perfanalytics/pose2sim), but in 2D.
 - [ ] Add tools for annotating images, undistort them, take perspective into account, etc. (cf. [Kinovea](https://www.kinovea.org/features.html)).
+- [ ] Check other methods for sorting people across frames ([STAF](https://github.com/soulslicer/STAF/tree/staf) or [LivePoseTracker](https://github.com/ortegatron/liveposetracker).
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
  [![Continuous integration](https://github.com/davidpagnon/sports2d/actions/
 workflows/continuous-integration.yml/badge.svg?branch=main)](https://
 github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/
-py/Sports2D)\ [![Open Source? Yes!](https://badgen.net/badge/
+py/Sports2D) [![Downloads](https://static.pepy.tech/badge/sports2d)](https://
+pepy.tech/project/sports2d)\ [![Open Source? Yes!](https://badgen.net/badge/
 Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/
 badges/) [![License](https://img.shields.io/badge/License-BSD_3--Clause-
 blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![DOI](https://
 zenodo.org/badge/634044634.svg)](https://zenodo.org/badge/latestdoi/634044634)\
 [Open_In_Colab]  # Sports2D **`Sports2D` lets you compute 2D joint and segment
 angles from a video.** [Content/demo_gif.gif] `Warning:` Angle estimation is
 only as good as the pose estimation algorithm, i.e., it is not perfect.\
@@ -60,18 +61,18 @@
 *Optionally:* If your video is not in the same folder as `Config_demo.toml`,
 specify its location in `video_dir`.\ Similarly, if you launch Sports2D in an
 other directory, specify the location of the config file this way:
 `Sports2D.detect_pose(
 toml>)`\ In `pose`, specify the use of BlazePose or OpenPose as joint
 detectors: this will be detailed in the next section.\ In `compute_angles`,
 select your angles of interest. ### Use OpenPose for multi-person, more
-accurate analysis OpenPose is slower than OpenPose, but more accurate. It also
-allows for the detection of multiple persons, whose indices are consistent
-across frames. 1. **Install OpenPose** (instructions [there](https://
-github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/
+accurate analysis OpenPose is slower than BlazePose, but usually more accurate.
+It also allows for the detection of multiple persons, whose indices are
+consistent across frames. 1. **Install OpenPose** (instructions [there](https:/
+/github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/
 0_index.md)). \ *Windows portable demo works fine.* 2. If you want even more
 accurate results, use the BODY_25B experimental model instead of the standard
 BODY_25 one. This requires manually [downloading the model](https://github.com/
 CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/
 README.md). You can optionally download from there the BODY_135 model which
 will let you compute wrist flexion and hand segment angle, however this will be
 much slower. 3. In `Config_demo.toml` â `pose.OPENPOSE`, specify your
@@ -144,8 +145,10 @@
 features.html)), or by training a model (cf. [DeepLabCut](https://
 deeplabcut.github.io/DeepLabCut/README.html)). - [ ] **Pose refinement**. Click
 and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/
 watch?v=bEuBKB7eqmk) for inspiration. - [ ] **Constrain points** to OpenSim
 skeletal model for better angle estimation (like with [Pose2Sim](https://
 github.com/perfanalytics/pose2sim), but in 2D. - [ ] Add tools for annotating
 images, undistort them, take perspective into account, etc. (cf. [Kinovea]
-(https://www.kinovea.org/features.html)).
+(https://www.kinovea.org/features.html)). - [ ] Check other methods for sorting
+people across frames ([STAF](https://github.com/soulslicer/STAF/tree/staf) or
+[LivePoseTracker](https://github.com/ortegatron/liveposetracker).
```

### Comparing `sports2d-0.1.0/Sports2D/Demo/Config_demo.toml` & `sports2d-0.1.2/Sports2D/Demo/Config_demo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 ## SPORTS2D PROJECT PARAMETERS                                               ##
 ###############################################################################
 
 # Configure your project parameters here
 
 
 [project]
-video_dir = '' # BETWEEN SINGLE QUOTES! # If empty, project dir is current dir
+video_dir = '' # BETWEEN SINGLE QUOTES! # If empty, result dir is current dir
 video_file = 'demo.mp4'
+result_dir = '' # BETWEEN SINGLE QUOTES! # If empty, project dir is current dir
 
 
 [pose]
 pose_algo = 'BLAZEPOSE' # 'OPENPOSE' or 'BLAZEPOSE' 
 # OpenPose is more accurate and supports multi-person detection, but needs to be installed separately	
 # Coming soon: 'deeplabcut', 'alphapose'
```

### Comparing `sports2d-0.1.0/Sports2D/Demo/demo.mp4` & `sports2d-0.1.2/Sports2D/Demo/demo.mp4`

 * *Files identical despite different names*

### Comparing `sports2d-0.1.0/Sports2D/Sports2D.py` & `sports2d-0.1.2/Sports2D/Sports2D.py`

 * *Files 13% similar despite different names*

```diff
@@ -103,18 +103,14 @@
 import toml
 import os
 import time
 import cv2
 from pathlib import Path
 import logging, logging.handlers
 
-with open(Path('logs.txt'), 'a+') as log_f: pass
-logging.basicConfig(format='%(message)s', level=logging.INFO, 
-    handlers = [logging.handlers.TimedRotatingFileHandler(Path('logs.txt'), when='D', interval=7), logging.StreamHandler()]) 
-
 
 ## AUTHORSHIP INFORMATION
 __author__ = "David Pagnon"
 __copyright__ = "Copyright 2023, Sports2D"
 __credits__ = ["David Pagnon"]
 __license__ = "BSD 3-Clause License"
 __version__ = "0.1"
@@ -137,38 +133,44 @@
     '''
     Retrieve sequence name and frames to be analyzed.
     '''
 
     video_dir = Path(config_dict.get('project').get('video_dir')).resolve()
     if video_dir == '': video_dir = os.getcwd()
     video_file = Path(config_dict.get('project').get('video_file'))
+    result_dir = Path(config_dict.get('project').get('result_dir')).resolve()
+    if result_dir == '': result_dir = os.getcwd()
     
     video = cv2.VideoCapture(str(video_dir / video_file))
     frame_rate = video.get(cv2.CAP_PROP_FPS)
     try:
         1/frame_rate
     except ZeroDivisionError:
         print('Frame rate could not be retrieved: check that your video exists at the correct path')
         raise
     video.release()
 
-    return video_dir, video_file, frame_rate
+    return video_dir, video_file, result_dir, frame_rate
 
 
 def detect_pose(config='Config_demo.toml'):
     '''
     Compute 2D pose from video.
     Save 2D csv file, and optionally json files, image files, and video file.
     Optionally interpolates missing data, filters them, and displays figures.
     '''
 
     from Sports2D.detect_pose import detect_pose_fun
     
     config_dict = read_config_file(config)
-    _, video_file, _ = base_params(config_dict)
+    _, video_file, result_dir, _ = base_params(config_dict)
+        
+    with open(result_dir / 'logs.txt', 'a+') as log_f: pass
+    logging.basicConfig(format='%(message)s', level=logging.INFO, force=True, 
+        handlers = [logging.handlers.TimedRotatingFileHandler(result_dir / 'logs.txt', when='D', interval=7), logging.StreamHandler()]) 
     
     logging.info("\n\n---------------------------------------------------------------------")
     logging.info(f"Detect pose for video {video_file}")
     logging.info("---------------------------------------------------------------------")
     start = time.time()
     
     detect_pose_fun(config_dict)
@@ -183,15 +185,20 @@
     Save csv file.
     Optionally interpolates missing data, filters them, and displays figures.
     '''
 
     from Sports2D.compute_angles import compute_angles_fun
 
     config_dict = read_config_file(config)
-    _, video_file, _ = base_params(config_dict)
+    _, video_file, result_dir, _ = base_params(config_dict)
+        
+    with open(result_dir / 'logs.txt', 'a+') as log_f: pass
+    logging.basicConfig(format='%(message)s', level=logging.INFO, force=True, 
+        handlers = [logging.handlers.TimedRotatingFileHandler(result_dir / 'logs.txt', when='D', interval=7), logging.StreamHandler()])
+        
     joint_angles = config_dict.get('compute_angles').get('joint_angles')
     segment_angles = config_dict.get('compute_angles').get('segment_angles')
 
     logging.info("\n\n---------------------------------------------------------------------")
     logging.info(f"Compute angles for video {video_file} ")
     logging.info(f"for {joint_angles}")
     logging.info(f"and {segment_angles}.")
```

### Comparing `sports2d-0.1.0/Sports2D/Utilities/Blazepose_runsave.py` & `sports2d-0.1.2/Sports2D/Utilities/Blazepose_runsave.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
                 try:
                     kpt = [[p.x*W, p.y*H, p.visibility] for p in results.pose_landmarks.landmark]
                     kpt = [item for sublist in kpt for item in sublist]  
 
                     mp_drawing.draw_landmarks(frame, results.pose_landmarks, mp_pose.POSE_CONNECTIONS, landmark_drawing_spec=mp_drawing_styles.get_default_pose_landmarks_style())
                 except:
                     print(f'No person detected by BlazePose on frame {count}')
-                    kpt=[np.nan*3*33]
+                    kpt=[np.nan]*3*33
 
                 # Display images
                 if display: 
                     cv2.imshow('frame', frame)
                     if cv2.waitKey(30) & 0xFF == ord('q'):
                         break
```

### Comparing `sports2d-0.1.0/Sports2D/Utilities/common.py` & `sports2d-0.1.2/Sports2D/Utilities/common.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.1.0/Sports2D/Utilities/filter.py` & `sports2d-0.1.2/Sports2D/Utilities/filter.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.1.0/Sports2D/Utilities/skeletons.py` & `sports2d-0.1.2/Sports2D/Utilities/skeletons.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.1.0/Sports2D/compute_angles.py` & `sports2d-0.1.2/Sports2D/compute_angles.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
     
     OUTPUTS:
     - one csv file for joint and segment angles per detected person
     - a logs.txt file 
     '''
     
     # Retrieve parameters
-    video_dir, video_file, frame_rate = base_params(config_dict)
+    video_dir, video_file, result_dir, frame_rate = base_params(config_dict)
     pose_algo = config_dict.get('pose').get('pose_algo')
     if pose_algo == 'OPENPOSE':
         pose_model = config_dict.get('pose').get('OPENPOSE').get('openpose_model')
     elif pose_algo == 'BLAZEPOSE':
         pose_model = 'BLAZEPOSE'
     joint_angles = config_dict.get('compute_angles').get('joint_angles')
     segment_angles = config_dict.get('compute_angles').get('segment_angles')
@@ -375,16 +375,16 @@
     median_filter_kernel = config_dict.get('compute_angles_advanced').get('median').get('kernel_size')
     filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
     
     show_angles_img = config_dict.get('compute_angles_advanced').get('save_img')
     show_angles_vid = config_dict.get('compute_angles_advanced').get('save_vid')
     
     # Find csv position files in video_dir, search pose_model and video_file.stem
-    logging.info(f'Retrieving csv position files in {video_dir}...')
-    csv_paths = sorted(video_dir.glob(f'*{video_file.stem}_{pose_model}_*points*.csv'))
+    logging.info(f'Retrieving csv position files in {result_dir}...')
+    csv_paths = list(result_dir.glob(f'*{video_file.stem}_{pose_model}_*points*.csv'))
     logging.info(f'{len(csv_paths)} persons found.')
 
     # Compute angles
     df_angles_list = []
     for i, c in enumerate(csv_paths):
         # Prepare angle csv header
         scorer = ['DavidPagnon']*angle_nb
@@ -448,27 +448,27 @@
                 display_figures_fun(df_angles)
 
             df_angles_list += [df_angles[-1]]
 
     # Add angles to vid and img
     if show_angles_img or show_angles_vid:
         video_base = Path(video_dir / video_file)
-        img_pose = video_base.parent / (video_base.stem + '_' + pose_model + '_img')
-        video_pose = video_base.parent / (video_base.stem + '_' + pose_model + '.mp4')
-        video_pose2 = video_base.parent / (video_base.stem + '_' + pose_model + '2.mp4')
+        img_pose = result_dir / (video_base.stem + '_' + pose_model + '_img')
+        video_pose = result_dir / (video_base.stem + '_' + pose_model + '.mp4')
+        video_pose2 = result_dir / (video_base.stem + '_' + pose_model + '2.mp4')
         
         if show_angles_vid:
             cap = [cv2.VideoCapture(str(video_pose)) if Path.exists(video_pose) else cv2.VideoCapture(str(video_base))][0]
             fps = cap.get(cv2.CAP_PROP_FPS)
             W, H = cap.get(cv2.CAP_PROP_FRAME_WIDTH), cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
             fourcc = cv2.VideoWriter_fourcc(*'mp4v')
             writer = cv2.VideoWriter(str(video_pose2), fourcc, fps, (int(W), int(H)))
         
         # Preferentially from pose image files
-        frames_img = sorted(img_pose.glob('*'))
+        frames_img = list(img_pose.glob('*'))
         if len(frames_img)>0:
             for frame_nb in range(df_angles_list[0].shape[0]):
                 df_angles_list_frame = [df_angles_list[n].iloc[frame_nb,:] for n in range(len(df_angles_list))]
                 frame = cv2.imread(str(frames_img[frame_nb]))
                 frame = overlay_angles(frame, df_angles_list_frame)
                 if show_angles_img:
                     cv2.imwrite(str(frames_img[frame_nb]), frame)
```

### Comparing `sports2d-0.1.0/Sports2D/detect_pose.py` & `sports2d-0.1.2/Sports2D/detect_pose.py`

 * *Files 3% similar despite different names*

```diff
@@ -284,15 +284,15 @@
     keypoints_ids = [node.id for _, _, node in RenderTree(model) if node.id!=None]
     keypoints_names = [node.name for _, _, node in RenderTree(model) if node.id!=None]
     keypoints_names_rearranged = [y for x,y in sorted(zip(keypoints_ids,keypoints_names))]
     keypoints_nb = len(keypoints_ids)
 
     # Retrieve coordinates
     logging.info('Sorting people across frames.')
-    json_fnames = sorted(json_path.glob('*.json'))
+    json_fnames = list(json_path.glob('*.json'))
     nb_persons_to_detect = max([len(json.load(open(json_fname))['people']) for json_fname in json_fnames])
     Coords = [np.array([]).reshape(0,keypoints_nb*3)] * nb_persons_to_detect
     for json_fname in json_fnames:    # for each frame
         with open(json_fname) as json_f:
             json_file = json.load(json_f)
             keypt = []
             # Retrieve coords for this frame 
@@ -434,15 +434,15 @@
             2)
             for i, n in enumerate(node_pairs)
             if not (np.isnan(x[n[0]]) or np.isnan(y[n[0]]) or np.isnan(x[n[1]]) or np.isnan(y[n[1]]))]
     
     return img
 
 
-def save_imgvid_reID(video_path, save_vid=1, save_img=1, *pose_model):
+def save_imgvid_reID(video_path, video_result_path, save_vid=1, save_img=1, *pose_model):
     '''
     Displays json 2d detections overlayed on original raw images.
     High confidence keypoints are green, low confidence ones are red.
      
     Note: See 'json_display_without_img.py' if you only want to display the
     json coordinates on an animated graph or if don't have the original raw
     images.
@@ -451,40 +451,40 @@
     json_display_with_img -j "<json_folder>" -i "<raw_img_folder>"
     json_display_with_img -j "<json_folder>" -i "<raw_img_folder>" -o "<output_img_folder>" -d True -s True
     import json_display_with_img; json_display_with_img.json_display_with_img_func(json_folder=r'<json_folder>', raw_img_folder=r'<raw_img_folder>')
     '''
             
    # Find csv position files, prepare video and image saving paths
     pose_model = pose_model[0]
-    csv_paths = sorted(video_path.parent.glob(f'*{video_path.stem}*{pose_model}*points*refined*.csv'))
+    csv_paths = list(video_result_path.parent.glob(f'*{video_result_path.stem}*{pose_model}*points*refined*.csv'))
     if csv_paths == []:
-        csv_paths = sorted(video_path.parent.glob(f'*{video_path.stem}*{pose_model}*points*.csv'))
+        csv_paths = list(video_result_path.parent.glob(f'*{video_result_path.stem}*{pose_model}*points*.csv'))
         
     # Open csv files
     coords = []
     for c in csv_paths:
         with open(c) as c_f:
             coords += [pd.read_csv(c_f, header=[0,1,2,3])]
 
     # Open video frame by frame
     cap = cv2.VideoCapture(str(video_path))
     W, H = cap.get(cv2.CAP_PROP_FRAME_WIDTH), cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
     fps = cap.get(cv2.CAP_PROP_FPS)
     if (cap.isOpened()== False): 
         print("Error opening video stream or file")
     if save_vid:
-        video_pose_path = video_path.parent / (video_path.stem + '_' + pose_model + '.mp4')
+        video_pose_path = video_result_path.parent / (video_result_path.stem + '_' + pose_model + '.mp4')
         fourcc = cv2.VideoWriter_fourcc(*'mp4v')
         writer = cv2.VideoWriter(str(video_pose_path), fourcc, fps, (int(W), int(H)))
     if save_img:
-        img_pose_path = video_path.parent / (video_path.stem + '_' + pose_model + '_img')
+        img_pose_path = video_result_path.parent / (video_result_path.stem + '_' + pose_model + '_img')
         img_pose_path.mkdir(parents=True, exist_ok=True)  
         
     f = 0
-    while(cap.isOpened() and f < len(coords[0])):
+    while(cap.isOpened()):
         ret, frame = cap.read()
         if ret == True:
             X = [np.array(coord.iloc[f,1::3]) for coord in coords]
             X = [np.where(x==0., np.nan, x) for x in X]
             Y = [np.array(coord.iloc[f,2::3]) for coord in coords]
             Y = [np.where(y==0., np.nan, y) for y in Y]
 
@@ -494,15 +494,15 @@
             # Draw keypoints and skeleton
             frame = draw_keypts_skel(X, Y, frame, pose_model)
             
             # Save video and images
             if save_vid:
                 writer.write(frame)
             if save_img:
-                cv2.imwrite(str( img_pose_path / (video_path.stem+'_'+pose_model+'.'+str(f).zfill(5)+'.png' )), frame)
+                cv2.imwrite(str( img_pose_path / (video_result_path.stem+'_'+pose_model+'.'+str(f).zfill(5)+'.png' )), frame)
 
         else: 
             break
         f += 1
     cap.release()
     writer.release()
 
@@ -537,15 +537,15 @@
     - one csv file of joint coordinates per detected person
     - optionally json directory, image directory, video
     - a logs.txt file 
     '''
     
     # Retrieve parameters
     root_dir = os.getcwd()
-    video_dir, video_file, frame_rate = base_params(config_dict)
+    video_dir, video_file, result_dir, frame_rate = base_params(config_dict)
     pose_algo = config_dict.get('pose').get('pose_algo')
     
     load_pose = config_dict.get('pose_advanced').get('load_pose')
     save_vid = config_dict.get('pose_advanced').get('save_vid')
     save_img = config_dict.get('pose_advanced').get('save_img')
     interp_gap_smaller_than = config_dict.get('pose_advanced').get('interp_gap_smaller_than')
     
@@ -556,19 +556,20 @@
     butterworth_filter_cutoff = config_dict.get('pose_advanced').get('butterworth').get('cut_off_frequency')
     gaussian_filter_kernel = config_dict.get('pose_advanced').get('gaussian').get('sigma_kernel')
     loess_filter_kernel = config_dict.get('pose_advanced').get('loess').get('nb_values_used')
     median_filter_kernel = config_dict.get('pose_advanced').get('median').get('kernel_size')
     filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
     
     video_file_stem = video_file.stem
-    video_path = (video_dir / video_file)
+    video_path = video_dir / video_file
+    video_result_path = result_dir / video_file
 
     if pose_algo == 'OPENPOSE':
         pose_model = config_dict.get('pose').get('OPENPOSE').get('openpose_model')
-        json_path = video_dir / '_'.join((video_file_stem,pose_model,'json'))
+        json_path = result_dir / '_'.join((video_file_stem,pose_model,'json'))
 
         # Pose detection skipped if load existing json files
         if load_pose and len(list(json_path.glob('*')))>0:
             pass
         else:
             logging.info(f'Detecting 2D joint positions with OpenPose model {pose_model}, for {video_file}.')
             json_path.mkdir(parents=True, exist_ok=True)
@@ -583,21 +584,21 @@
             os.chdir(root_dir)
         
     # Sort people and save to csv, optionally display plot
         json_to_csv(json_path, pose_model, interp_gap_smaller_than, filter_options, show_plots)
         
     # Save images and files after reindentification
         if save_img and save_vid:
-            logging.info(f'Saving images and video in {video_dir}.')
+            logging.info(f'Saving images and video in {result_dir}.')
         if save_img and not save_vid:
-            logging.info(f'Saving images in {video_dir}.')
+            logging.info(f'Saving images in {result_dir}.')
         if not save_img and save_vid:
-            logging.info(f'Saving video in {video_dir}.')
+            logging.info(f'Saving video in {result_dir}.')
         if save_vid or save_img:
-            save_imgvid_reID(video_path, save_vid, save_img, pose_model)
+            save_imgvid_reID(video_path, video_result_path, save_vid, save_img, pose_model)
    
      
     elif pose_algo == 'BLAZEPOSE':
         model_complexity = config_dict.get('pose').get('BLAZEPOSE').get('model_complexity')
-        Blazepose_runsave.blazepose_detec_func(input_file=video_path, save_images=save_img, to_json=True, save_video=save_vid, to_csv=True, model_complexity=model_complexity)
+        Blazepose_runsave.blazepose_detec_func(input_file=video_path, save_images=save_img, to_json=True, save_video=save_vid, to_csv=True, output_folder=result_dir, model_complexity=model_complexity)
 
     logging.info(f'Done.')
```

### Comparing `sports2d-0.1.0/setup.cfg` & `sports2d-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sports2d
-version = 0.1.0
+version = 0.1.2
 author = David Pagnon
 author_email = contact@david-pagnon.com
 description = Detect pose and compute 2D joint angles from a video.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/davidpagnon/Sports2D
 keywords = markerless, kinematics, OpenPose, BlazePose, joint angles, 2D, biomechanics, sports, sports-analytics
```

### Comparing `sports2d-0.1.0/sports2d.egg-info/PKG-INFO` & `sports2d-0.1.2/sports2d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.1.0
+Version: 0.1.2
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
@@ -23,25 +23,25 @@
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
 Requires-Python: <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![Continuous integration](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
-[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D)\
+[![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/py/Sports2D)
+[![Downloads](https://static.pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)\
 [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![DOI](https://zenodo.org/badge/634044634.svg)](https://zenodo.org/badge/latestdoi/634044634)\
 <a href="https://colab.research.google.com/github/davidpagnon/Sports2D/blob/main/Sports2D/Sports2D.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
-<!-- [![Downloads](https://pepy.tech/badge/sports2d)](https://pepy.tech/project/sports2d)
-[![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
+<!-- [![Stars](https://badgen.net/github/stars/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/stargazers)
 [![GitHub issues](https://img.shields.io/github/issues/davidpagnon/sports2d)](https://github.com/davidpagnon/sports2d/issues)
 [![GitHub issues-closed](https://img.shields.io/github/issues-closed/davidpagnon/sports2d)](https://GitHub.com/davidpagnon/sports2d/issues?q=is%3Aissue+is%3Aclosed) 
-[![DOI](https://zenodo.org/badge/501642916.svg)](https://zenodo.org/badge/latestdoi/501642916)
+[![status](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26/status.svg)](https://joss.theoj.org/papers/a31cb207a180f7ac9838d049e3a0de26)
 -->
 
 
 # Sports2D
 
 **`Sports2D` lets you compute 2D joint and segment angles from a video.**
 
@@ -143,15 +143,15 @@
 Similarly, if you launch Sports2D in an other directory, specify the location of the config file this way: `Sports2D.detect_pose(<path_to_Config_demo.toml>)`\
 In `pose`, specify the use of BlazePose or OpenPose as joint detectors: this will be detailed in the next section.\
 In `compute_angles`, select your angles of interest.
 
 
 ### Use OpenPose for multi-person, more accurate analysis
 
-OpenPose is slower than OpenPose, but more accurate. It also allows for the detection of multiple persons, whose indices are consistent across frames. 
+OpenPose is slower than BlazePose, but usually more accurate. It also allows for the detection of multiple persons, whose indices are consistent across frames. 
 
 1. **Install OpenPose** (instructions [there](https://github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/0_index.md)). \
 *Windows portable demo works fine.*
 
 2. If you want even more accurate results, use the BODY_25B experimental model instead of the standard BODY_25 one. This requires manually [downloading the model](https://github.com/CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/README.md). You can optionally download from there the BODY_135 model which will let you compute wrist flexion and hand segment angle, however this will be much slower.
 
 3. In `Config_demo.toml` → `pose.OPENPOSE`, specify your OpenPose model, and the path where you downloaded OpenPose.
@@ -255,14 +255,15 @@
 - [ ] Full test on **MacOS**.
 - [ ] **GUI applications** for Windows, Mac, and Linux, as well as for Android and iOS (minimal version on mobile device, with only BlazePose). Code with [Kivy](https://kivy.org).
 - [ ] **Include OpenPose** in Sports2D executable files. [Dockerize](https://github.com/stanfordnmbl/mobile-gaitlab/blob/master/demo/Dockerfile) it? 
 - [ ] **Track other points and angles** with classic tracking methods (cf. [Kinovea](https://www.kinovea.org/features.html)), or by training a model (cf. [DeepLabCut](https://deeplabcut.github.io/DeepLabCut/README.html)).
 - [ ] **Pose refinement**. Click and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/watch?v=bEuBKB7eqmk) for inspiration.
 - [ ] **Constrain points** to OpenSim skeletal model for better angle estimation (like with [Pose2Sim](https://github.com/perfanalytics/pose2sim), but in 2D.
 - [ ] Add tools for annotating images, undistort them, take perspective into account, etc. (cf. [Kinovea](https://www.kinovea.org/features.html)).
+- [ ] Check other methods for sorting people across frames ([STAF](https://github.com/soulslicer/STAF/tree/staf) or [LivePoseTracker](https://github.com/ortegatron/liveposetracker).
 
 BSD 3-Clause License
 
 Copyright (c) 2022, perfanalytics
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sports2d Version: 0.1.0 Summary: Detect pose and
+Metadata-Version: 2.1 Name: sports2d Version: 0.1.2 Summary: Detect pose and
 compute 2D joint angles from a video. Home-page: https://github.com/
 davidpagnon/Sports2D Author: David Pagnon Author-email: contact@david-
 pagnon.com License: BSD 3-Clause License Project-URL: Bug Tracker, https://
 github.com/davidpagnon/Sports2D/issues Keywords:
 markerless,kinematics,OpenPose,BlazePose,joint
 angles,2D,biomechanics,sports,sports-analytics Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,16 @@
 Engineering :: Medical Science Apps. Classifier: Topic :: Multimedia ::
 Graphics Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling Requires-
 Python: <3.11 Description-Content-Type: text/markdown License-File: LICENSE [!
 [Continuous integration](https://github.com/davidpagnon/sports2d/actions/
 workflows/continuous-integration.yml/badge.svg?branch=main)](https://
 github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/
-py/Sports2D)\ [![Open Source? Yes!](https://badgen.net/badge/
+py/Sports2D) [![Downloads](https://static.pepy.tech/badge/sports2d)](https://
+pepy.tech/project/sports2d)\ [![Open Source? Yes!](https://badgen.net/badge/
 Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/
 badges/) [![License](https://img.shields.io/badge/License-BSD_3--Clause-
 blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![DOI](https://
 zenodo.org/badge/634044634.svg)](https://zenodo.org/badge/latestdoi/634044634)\
 [Open_In_Colab]  # Sports2D **`Sports2D` lets you compute 2D joint and segment
 angles from a video.** [Content/demo_gif.gif] `Warning:` Angle estimation is
 only as good as the pose estimation algorithm, i.e., it is not perfect.\
@@ -76,18 +77,18 @@
 *Optionally:* If your video is not in the same folder as `Config_demo.toml`,
 specify its location in `video_dir`.\ Similarly, if you launch Sports2D in an
 other directory, specify the location of the config file this way:
 `Sports2D.detect_pose(
 toml>)`\ In `pose`, specify the use of BlazePose or OpenPose as joint
 detectors: this will be detailed in the next section.\ In `compute_angles`,
 select your angles of interest. ### Use OpenPose for multi-person, more
-accurate analysis OpenPose is slower than OpenPose, but more accurate. It also
-allows for the detection of multiple persons, whose indices are consistent
-across frames. 1. **Install OpenPose** (instructions [there](https://
-github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/
+accurate analysis OpenPose is slower than BlazePose, but usually more accurate.
+It also allows for the detection of multiple persons, whose indices are
+consistent across frames. 1. **Install OpenPose** (instructions [there](https:/
+/github.com/CMU-Perceptual-Computing-Lab/openpose/blob/master/doc/installation/
 0_index.md)). \ *Windows portable demo works fine.* 2. If you want even more
 accurate results, use the BODY_25B experimental model instead of the standard
 BODY_25 one. This requires manually [downloading the model](https://github.com/
 CMU-Perceptual-Computing-Lab/openpose_train/blob/master/experimental_models/
 README.md). You can optionally download from there the BODY_135 model which
 will let you compute wrist flexion and hand segment angle, however this will be
 much slower. 3. In `Config_demo.toml` â `pose.OPENPOSE`, specify your
@@ -160,27 +161,30 @@
 features.html)), or by training a model (cf. [DeepLabCut](https://
 deeplabcut.github.io/DeepLabCut/README.html)). - [ ] **Pose refinement**. Click
 and move badly estimated 2D points. See [DeepLabCut](https://www.youtube.com/
 watch?v=bEuBKB7eqmk) for inspiration. - [ ] **Constrain points** to OpenSim
 skeletal model for better angle estimation (like with [Pose2Sim](https://
 github.com/perfanalytics/pose2sim), but in 2D. - [ ] Add tools for annotating
 images, undistort them, take perspective into account, etc. (cf. [Kinovea]
-(https://www.kinovea.org/features.html)). BSD 3-Clause License Copyright (c)
-2022, perfanalytics All rights reserved. Redistribution and use in source and
-binary forms, with or without modification, are permitted provided that the
-following conditions are met: 1. Redistributions of source code must retain the
-above copyright notice, this list of conditions and the following disclaimer.
-2. Redistributions in binary form must reproduce the above copyright notice,
-this list of conditions and the following disclaimer in the documentation and/
-or other materials provided with the distribution. 3. Neither the name of the
-copyright holder nor the names of its contributors may be used to endorse or
-promote products derived from this software without specific prior written
-permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
-LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
-GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+(https://www.kinovea.org/features.html)). - [ ] Check other methods for sorting
+people across frames ([STAF](https://github.com/soulslicer/STAF/tree/staf) or
+[LivePoseTracker](https://github.com/ortegatron/liveposetracker). BSD 3-Clause
+License Copyright (c) 2022, perfanalytics All rights reserved. Redistribution
+and use in source and binary forms, with or without modification, are permitted
+provided that the following conditions are met: 1. Redistributions of source
+code must retain the above copyright notice, this list of conditions and the
+following disclaimer. 2. Redistributions in binary form must reproduce the
+above copyright notice, this list of conditions and the following disclaimer in
+the documentation and/or other materials provided with the distribution. 3.
+Neither the name of the copyright holder nor the names of its contributors may
+be used to endorse or promote products derived from this software without
+specific prior written permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT
+HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
+INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
+FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
+COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
+INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
+PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
+ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `sports2d-0.1.0/sports2d.egg-info/SOURCES.txt` & `sports2d-0.1.2/sports2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

