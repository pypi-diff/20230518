# Comparing `tmp/raya-0.9.1.tar.gz` & `tmp/raya-3.4.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raya-0.9.1.tar", last modified: Tue Sep 20 14:52:31 2022, max compression
+gzip compressed data, was "raya-3.4.1.dev5.tar", last modified: Thu May 18 04:39:49 2023, max compression
```

## Comparing `raya-0.9.1.tar` & `raya-3.4.1.dev5.tar`

### file list

```diff
@@ -1,13 +1,76 @@
-drwxrwxr-x   0 ofir      (1000) ofir      (1000)        0 2022-09-20 14:52:31.484438 raya-0.9.1/
--rw-rw-r--   0 ofir      (1000) ofir      (1000)     1069 2022-08-02 15:33:11.000000 raya-0.9.1/LICENSE
--rw-rw-r--   0 ofir      (1000) ofir      (1000)       35 2022-08-02 15:31:45.000000 raya-0.9.1/MANIFEST.in
--rw-rw-r--   0 ofir      (1000) ofir      (1000)      401 2022-09-20 14:52:31.484438 raya-0.9.1/PKG-INFO
--rw-rw-r--   0 ofir      (1000) ofir      (1000)      145 2022-08-28 05:55:25.000000 raya-0.9.1/README.md
-drwxrwxr-x   0 ofir      (1000) ofir      (1000)        0 2022-09-20 14:52:31.484438 raya-0.9.1/raya.egg-info/
--rw-rw-r--   0 ofir      (1000) ofir      (1000)      401 2022-09-20 14:52:31.000000 raya-0.9.1/raya.egg-info/PKG-INFO
--rw-rw-r--   0 ofir      (1000) ofir      (1000)      187 2022-09-20 14:52:31.000000 raya-0.9.1/raya.egg-info/SOURCES.txt
--rw-rw-r--   0 ofir      (1000) ofir      (1000)        1 2022-09-20 14:52:31.000000 raya-0.9.1/raya.egg-info/dependency_links.txt
--rw-rw-r--   0 ofir      (1000) ofir      (1000)        8 2022-09-20 14:52:31.000000 raya-0.9.1/raya.egg-info/requires.txt
--rw-rw-r--   0 ofir      (1000) ofir      (1000)        1 2022-09-20 14:52:31.000000 raya-0.9.1/raya.egg-info/top_level.txt
--rw-rw-r--   0 ofir      (1000) ofir      (1000)       38 2022-09-20 14:52:31.484438 raya-0.9.1/setup.cfg
--rw-rw-r--   0 ofir      (1000) ofir      (1000)      469 2022-09-20 14:52:26.000000 raya-0.9.1/setup.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:39:49.826545 raya-3.4.1.dev5/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1074 2023-01-29 19:45:42.000000 raya-3.4.1.dev5/LICENSE
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      579 2023-05-18 04:39:49.826545 raya-3.4.1.dev5/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      150 2023-05-15 19:14:17.000000 raya-3.4.1.dev5/README.md
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      103 2023-01-29 19:45:42.000000 raya-3.4.1.dev5/pyproject.toml
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       38 2023-05-18 04:39:49.826545 raya-3.4.1.dev5/setup.cfg
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3095 2023-05-18 04:39:36.000000 raya-3.4.1.dev5/setup.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:39:49.822545 raya-3.4.1.dev5/src/
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:39:49.822545 raya-3.4.1.dev5/src/raya/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       38 2023-05-15 19:14:17.000000 raya-3.4.1.dev5/src/raya/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       27 2023-05-18 04:15:49.000000 raya-3.4.1.dev5/src/raya/_version.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3183 2023-05-18 04:39:15.000000 raya-3.4.1.dev5/src/raya/application_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      664 2023-05-18 04:39:15.000000 raya-3.4.1.dev5/src/raya/constants.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:39:49.822545 raya-3.4.1.dev5/src/raya/controllers/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev5/src/raya/controllers/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      260 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/analytics_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)    17375 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/arms_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      620 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/base_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       90 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/base_pseudo_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1222 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/cameras_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      425 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/communication_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2838 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/cv_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1387 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/fleet_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      523 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/grasping_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      924 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/interactions_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1298 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/leds_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1171 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/lidar_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3127 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/manipulation_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2042 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/motion_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     7148 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/navigation_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1367 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/sensors_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      808 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/skills_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2590 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/sound_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6988 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/controllers/ui_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       59 2023-05-18 04:39:15.000000 raya-3.4.1.dev5/src/raya/entry_point.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     4681 2023-05-18 04:39:15.000000 raya-3.4.1.dev5/src/raya/enumerations.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)    13019 2023-05-18 04:39:15.000000 raya-3.4.1.dev5/src/raya/exceptions.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6274 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/exceptions_handler.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:39:49.822545 raya-3.4.1.dev5/src/raya/handlers/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev5/src/raya/handlers/__init__.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:39:49.826545 raya-3.4.1.dev5/src/raya/handlers/cv/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev5/src/raya/handlers/cv/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      877 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/classifier_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      844 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/detector_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      743 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/estimator_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      302 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/faces_detector_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      831 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/faces_recognizer_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      305 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/hand_estimator_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      183 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/model_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      790 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/objects_classifier_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      782 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/objects_detector_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      794 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/objects_segmentator_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      783 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/planes_segmentator_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      862 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/recognizer_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      871 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/segmentator_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      703 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/cv/tags_detector_handler.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:39:49.826545 raya-3.4.1.dev5/src/raya/handlers/general/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev5/src/raya/handlers/general/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      330 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/handlers/general/callback_handler.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:39:49.826545 raya-3.4.1.dev5/src/raya/listeners/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev5/src/raya/listeners/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       77 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/listeners/lidar_listeners.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      160 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/listeners/sensors_listeners.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      352 2023-05-18 04:39:15.000000 raya-3.4.1.dev5/src/raya/logger.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2055 2023-05-18 04:39:15.000000 raya-3.4.1.dev5/src/raya/raya_interface.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      257 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/standalone_handler.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:39:49.826545 raya-3.4.1.dev5/src/raya/tools/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev5/src/raya/tools/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/tools/filesystem.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      984 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/tools/fsm.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      152 2023-05-18 04:39:16.000000 raya-3.4.1.dev5/src/raya/tools/image.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 04:39:49.822545 raya-3.4.1.dev5/src/raya.egg-info/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      579 2023-05-18 04:39:49.000000 raya-3.4.1.dev5/src/raya.egg-info/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2314 2023-05-18 04:39:49.000000 raya-3.4.1.dev5/src/raya.egg-info/SOURCES.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-18 04:39:49.000000 raya-3.4.1.dev5/src/raya.egg-info/dependency_links.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        5 2023-05-18 04:39:49.000000 raya-3.4.1.dev5/src/raya.egg-info/top_level.txt
```

### Comparing `raya-0.9.1/LICENSE` & `raya-3.4.1.dev5/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-MIT License
-
-Copyright (c) [year] [fullname]
+Copyright (c) 2018 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

