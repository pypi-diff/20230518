# Comparing `tmp/raya-3.4.1.dev0.tar.gz` & `tmp/raya-3.4.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raya-3.4.1.dev0.tar", last modified: Wed May 17 16:00:15 2023, max compression
+gzip compressed data, was "raya-3.4.1.dev3.tar", last modified: Thu May 18 03:48:42 2023, max compression
```

## Comparing `raya-3.4.1.dev0.tar` & `raya-3.4.1.dev3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-17 16:00:15.378730 raya-3.4.1.dev0/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1074 2023-01-29 19:45:42.000000 raya-3.4.1.dev0/LICENSE
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      579 2023-05-17 16:00:15.378730 raya-3.4.1.dev0/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      150 2023-05-15 19:14:17.000000 raya-3.4.1.dev0/README.md
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      103 2023-01-29 19:45:42.000000 raya-3.4.1.dev0/pyproject.toml
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       38 2023-05-17 16:00:15.378730 raya-3.4.1.dev0/setup.cfg
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     3091 2023-05-17 16:00:13.000000 raya-3.4.1.dev0/setup.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-17 16:00:15.374730 raya-3.4.1.dev0/src/
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-17 16:00:15.378730 raya-3.4.1.dev0/src/raya/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       38 2023-05-15 19:14:17.000000 raya-3.4.1.dev0/src/raya/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       27 2023-05-17 15:58:17.000000 raya-3.4.1.dev0/src/raya/_version.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     3183 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/application_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      664 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/constants.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-17 16:00:15.378730 raya-3.4.1.dev0/src/raya/controllers/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev0/src/raya/controllers/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      260 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/controllers/analytics_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)    17375 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/controllers/arms_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      620 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/controllers/base_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       90 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/controllers/base_pseudo_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1222 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/controllers/cameras_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      425 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/controllers/communication_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2838 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/controllers/cv_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1387 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/controllers/fleet_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      523 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/controllers/grasping_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      924 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/controllers/interactions_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1298 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/controllers/leds_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1171 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/controllers/lidar_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     3127 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/controllers/manipulation_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2042 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/controllers/motion_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     7148 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/controllers/navigation_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     1367 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/controllers/sensors_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      808 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/controllers/skills_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2282 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/controllers/sound_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6988 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/controllers/ui_controller.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       59 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/entry_point.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     4681 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/enumerations.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)    12950 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/exceptions.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     6274 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/exceptions_handler.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-17 16:00:15.378730 raya-3.4.1.dev0/src/raya/handlers/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev0/src/raya/handlers/__init__.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-17 16:00:15.378730 raya-3.4.1.dev0/src/raya/handlers/cv/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev0/src/raya/handlers/cv/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      877 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/classifier_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      844 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/detector_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      743 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/estimator_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      302 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/faces_detector_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      831 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/faces_recognizer_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      305 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/hand_estimator_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      183 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/model_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      790 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/objects_classifier_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      782 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/objects_detector_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      794 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/objects_segmentator_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      783 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/planes_segmentator_handler.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      862 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/recognizer_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      871 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/segmentator_handler_base.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      703 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/cv/tags_detector_handler.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-17 16:00:15.378730 raya-3.4.1.dev0/src/raya/handlers/general/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev0/src/raya/handlers/general/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      330 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/handlers/general/callback_handler.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-17 16:00:15.378730 raya-3.4.1.dev0/src/raya/listeners/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev0/src/raya/listeners/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)       77 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/listeners/lidar_listeners.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      160 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/listeners/sensors_listeners.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      352 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/logger.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2055 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/raya_interface.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      257 2023-05-17 15:58:37.000000 raya-3.4.1.dev0/src/raya/standalone_handler.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-17 16:00:15.378730 raya-3.4.1.dev0/src/raya/tools/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev0/src/raya/tools/__init__.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/tools/filesystem.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      984 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/tools/fsm.py
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      152 2023-05-17 15:58:38.000000 raya-3.4.1.dev0/src/raya/tools/image.py
-drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-17 16:00:15.378730 raya-3.4.1.dev0/src/raya.egg-info/
--rw-rw-r--   0 camilo    (1000) camilo    (1000)      579 2023-05-17 16:00:15.000000 raya-3.4.1.dev0/src/raya.egg-info/PKG-INFO
--rw-rw-r--   0 camilo    (1000) camilo    (1000)     2314 2023-05-17 16:00:15.000000 raya-3.4.1.dev0/src/raya.egg-info/SOURCES.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-17 16:00:15.000000 raya-3.4.1.dev0/src/raya.egg-info/dependency_links.txt
--rw-rw-r--   0 camilo    (1000) camilo    (1000)        5 2023-05-17 16:00:15.000000 raya-3.4.1.dev0/src/raya.egg-info/top_level.txt
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:48:42.152766 raya-3.4.1.dev3/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1074 2023-01-29 19:45:42.000000 raya-3.4.1.dev3/LICENSE
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      579 2023-05-18 03:48:42.152766 raya-3.4.1.dev3/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      150 2023-05-15 19:14:17.000000 raya-3.4.1.dev3/README.md
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      103 2023-01-29 19:45:42.000000 raya-3.4.1.dev3/pyproject.toml
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       38 2023-05-18 03:48:42.152766 raya-3.4.1.dev3/setup.cfg
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3094 2023-05-18 03:48:39.000000 raya-3.4.1.dev3/setup.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:48:42.148766 raya-3.4.1.dev3/src/
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:48:42.148766 raya-3.4.1.dev3/src/raya/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       38 2023-05-15 19:14:17.000000 raya-3.4.1.dev3/src/raya/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       27 2023-05-18 03:47:52.000000 raya-3.4.1.dev3/src/raya/_version.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3183 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/application_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      664 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/constants.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:48:42.148766 raya-3.4.1.dev3/src/raya/controllers/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev3/src/raya/controllers/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      260 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/analytics_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)    17375 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/arms_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      620 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/base_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       90 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/base_pseudo_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1222 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/cameras_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      425 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/communication_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2838 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/cv_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1387 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/fleet_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      523 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/grasping_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      924 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/interactions_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1298 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/leds_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1171 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/lidar_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     3127 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/manipulation_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2042 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/motion_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     7148 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/navigation_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     1367 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/sensors_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      808 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/skills_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2590 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/sound_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6988 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/controllers/ui_controller.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       59 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/entry_point.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     4681 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/enumerations.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)    13019 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/exceptions.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     6274 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/exceptions_handler.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:48:42.148766 raya-3.4.1.dev3/src/raya/handlers/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev3/src/raya/handlers/__init__.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:48:42.152766 raya-3.4.1.dev3/src/raya/handlers/cv/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev3/src/raya/handlers/cv/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      877 2023-05-18 03:48:05.000000 raya-3.4.1.dev3/src/raya/handlers/cv/classifier_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      844 2023-05-18 03:48:05.000000 raya-3.4.1.dev3/src/raya/handlers/cv/detector_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      743 2023-05-18 03:48:05.000000 raya-3.4.1.dev3/src/raya/handlers/cv/estimator_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      302 2023-05-18 03:48:05.000000 raya-3.4.1.dev3/src/raya/handlers/cv/faces_detector_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      831 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/handlers/cv/faces_recognizer_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      305 2023-05-18 03:48:05.000000 raya-3.4.1.dev3/src/raya/handlers/cv/hand_estimator_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      183 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/handlers/cv/model_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      790 2023-05-18 03:48:05.000000 raya-3.4.1.dev3/src/raya/handlers/cv/objects_classifier_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      782 2023-05-18 03:48:05.000000 raya-3.4.1.dev3/src/raya/handlers/cv/objects_detector_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      794 2023-05-18 03:48:05.000000 raya-3.4.1.dev3/src/raya/handlers/cv/objects_segmentator_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      783 2023-05-18 03:48:05.000000 raya-3.4.1.dev3/src/raya/handlers/cv/planes_segmentator_handler.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      862 2023-05-18 03:48:05.000000 raya-3.4.1.dev3/src/raya/handlers/cv/recognizer_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      871 2023-05-18 03:48:05.000000 raya-3.4.1.dev3/src/raya/handlers/cv/segmentator_handler_base.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      703 2023-05-18 03:48:05.000000 raya-3.4.1.dev3/src/raya/handlers/cv/tags_detector_handler.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:48:42.152766 raya-3.4.1.dev3/src/raya/handlers/general/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-05-15 19:15:31.000000 raya-3.4.1.dev3/src/raya/handlers/general/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      330 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/handlers/general/callback_handler.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:48:42.152766 raya-3.4.1.dev3/src/raya/listeners/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev3/src/raya/listeners/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)       77 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/listeners/lidar_listeners.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      160 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/listeners/sensors_listeners.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      352 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/logger.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2055 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/raya_interface.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      257 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/standalone_handler.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:48:42.152766 raya-3.4.1.dev3/src/raya/tools/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        0 2023-01-29 19:45:42.000000 raya-3.4.1.dev3/src/raya/tools/__init__.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      399 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/tools/filesystem.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      984 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/tools/fsm.py
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      152 2023-05-18 03:48:04.000000 raya-3.4.1.dev3/src/raya/tools/image.py
+drwxrwxr-x   0 camilo    (1000) camilo    (1000)        0 2023-05-18 03:48:42.148766 raya-3.4.1.dev3/src/raya.egg-info/
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)      579 2023-05-18 03:48:42.000000 raya-3.4.1.dev3/src/raya.egg-info/PKG-INFO
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)     2314 2023-05-18 03:48:42.000000 raya-3.4.1.dev3/src/raya.egg-info/SOURCES.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        1 2023-05-18 03:48:42.000000 raya-3.4.1.dev3/src/raya.egg-info/dependency_links.txt
+-rw-rw-r--   0 camilo    (1000) camilo    (1000)        5 2023-05-18 03:48:42.000000 raya-3.4.1.dev3/src/raya.egg-info/top_level.txt
```

### Comparing `raya-3.4.1.dev0/LICENSE` & `raya-3.4.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/PKG-INFO` & `raya-3.4.1.dev3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raya
-Version: 3.4.1.dev0
+Version: 3.4.1.dev3
 Summary: Unlimited Robotics - Ra-Ya Python Library
 Home-page: https://documentation.unlimited-robotics.com/
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Platform: UNKNOWN
```

### Comparing `raya-3.4.1.dev0/setup.py` & `raya-3.4.1.dev3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 import pathlib
 import re
 from pathlib import Path
 
 from setuptools import setup, find_packages
 from setuptools.command.build_py import build_py as _build_py
 
-if 'bdist_wheel' in sys.argv:
-    # from Cython.Build import cythonize
-    # BUILD_WHEEL = True
-    BUILD_WHEEL = False
-else:
-    BUILD_WHEEL = False
+# if 'bdist_wheel' in sys.argv:
+#     from Cython.Build import cythonize
+#     BUILD_WHEEL = True
+# else:
+#     BUILD_WHEEL = False
+
+BUILD_WHEEL = False
 
 
 def get_lib_version():
     VERSIONFILE = 'src/raya/_version.py'
     verstrline = open(VERSIONFILE, "rt").read()
     VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
     mo = re.search(VSRE, verstrline, re.M)
```

### Comparing `raya-3.4.1.dev0/src/raya/application_base.py` & `raya-3.4.1.dev3/src/raya/application_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/constants.py` & `raya-3.4.1.dev3/src/raya/constants.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/arms_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/arms_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/base_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/cameras_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/cameras_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/cv_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/cv_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/fleet_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/fleet_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/grasping_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/grasping_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/interactions_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/interactions_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/leds_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/leds_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/lidar_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/lidar_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/manipulation_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/manipulation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/motion_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/motion_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/navigation_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/navigation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/sensors_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/sensors_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/skills_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/skills_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/controllers/sound_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/sound_controller.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import typing
 import pasimple
 from typing import List, Any
 from rclpy.node import Node
 from raya.controllers.base_controller import BaseController
 
 SIZE = 20
 
@@ -12,22 +13,14 @@
         self.FORMAT = pasimple.PA_SAMPLE_S16LE
         self.SAMPLE_WIDTH = pasimple.format2width(self.FORMAT)
         self.CHANNELS = 1
         self.SAMPLE_RATE = 8000
         self.MAX_DURATION_DATA = 60
         self.MAX_SIZE_DATA = (self.SAMPLE_RATE * self.MAX_DURATION_DATA)
 
-    async def play_predefined_sound(self,
-                                    sound_name: str,
-                                    volume: int = 100,
-                                    callback_feedback=None,
-                                    callback_finish=None,
-                                    wait=True) -> None:
-        return
-
     async def play_sound_from_file(self,
                                    filepath: str,
                                    volume: int = 100,
                                    callback_feedback=None,
                                    callback_finish=None,
                                    wait=True) -> None:
         return
@@ -36,32 +29,43 @@
                                    audio_raw,
                                    volume: int = 100,
                                    callback_feedback=None,
                                    callback_finish=None,
                                    wait=True) -> None:
         return
 
+    async def play_predefined_sound(self,
+                                    sound_name: str,
+                                    volume: int = 100,
+                                    callback_feedback=None,
+                                    callback_finish=None,
+                                    wait=True) -> None:
+        return
+
     def get_predefined_sounds(self) -> List[str]:
         return
 
     async def record_sound(self,
                            duration: float = 60.0,
                            path: str = '',
-                           callback_finish=None,
-                           wait=True) -> Any:
+                           callback_finish: typing.Callable = None,
+                           callback_finish_async: typing.Callable = None,
+                           wait: bool = True) -> Any:
         return
 
     def is_playing(self):
         return
 
     def is_recording(self):
         return
 
     async def play_sound(self,
                          name: str = None,
                          path: str = None,
-                         data: Any = None,
+                         data: list = None,
                          volume: int = 100,
-                         callback_feedback=None,
-                         callback_finish=None,
-                         wait=True) -> None:
+                         callback_finish: typing.Callable = None,
+                         callback_finish_async: typing.Callable = None,
+                         callback_feedback: typing.Callable = None,
+                         callback_feedback_async: typing.Callable = None,
+                         wait: bool = True) -> None:
         pass
```

### Comparing `raya-3.4.1.dev0/src/raya/controllers/ui_controller.py` & `raya-3.4.1.dev3/src/raya/controllers/ui_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/enumerations.py` & `raya-3.4.1.dev3/src/raya/enumerations.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/exceptions.py` & `raya-3.4.1.dev3/src/raya/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,14 +230,18 @@
     pass
 
 
 class RayaLidarInvalidAngleUnit(RayaApplicationException):
     pass
 
 
+class RayaLidarNotDataReceived(RayaApplicationException):
+    pass
+
+
 class RayaCamerasException(RayaControllerException):
     pass
 
 
 class RayaCameraInvalidName(RayaCamerasException):
     pass
```

### Comparing `raya-3.4.1.dev0/src/raya/exceptions_handler.py` & `raya-3.4.1.dev3/src/raya/exceptions_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/handlers/cv/classifier_handler_base.py` & `raya-3.4.1.dev3/src/raya/handlers/cv/classifier_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/handlers/cv/detector_handler_base.py` & `raya-3.4.1.dev3/src/raya/handlers/cv/detector_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/handlers/cv/estimator_handler_base.py` & `raya-3.4.1.dev3/src/raya/handlers/cv/estimator_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/handlers/cv/faces_recognizer_handler.py` & `raya-3.4.1.dev3/src/raya/handlers/cv/faces_recognizer_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/handlers/cv/objects_classifier_handler.py` & `raya-3.4.1.dev3/src/raya/handlers/cv/objects_classifier_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/handlers/cv/objects_detector_handler.py` & `raya-3.4.1.dev3/src/raya/handlers/cv/objects_detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/handlers/cv/objects_segmentator_handler.py` & `raya-3.4.1.dev3/src/raya/handlers/cv/objects_segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/handlers/cv/planes_segmentator_handler.py` & `raya-3.4.1.dev3/src/raya/handlers/cv/planes_segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/handlers/cv/recognizer_handler_base.py` & `raya-3.4.1.dev3/src/raya/handlers/cv/recognizer_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/handlers/cv/segmentator_handler_base.py` & `raya-3.4.1.dev3/src/raya/handlers/cv/segmentator_handler_base.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/handlers/cv/tags_detector_handler.py` & `raya-3.4.1.dev3/src/raya/handlers/cv/tags_detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/raya_interface.py` & `raya-3.4.1.dev3/src/raya/raya_interface.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya/tools/fsm.py` & `raya-3.4.1.dev3/src/raya/tools/fsm.py`

 * *Files identical despite different names*

### Comparing `raya-3.4.1.dev0/src/raya.egg-info/PKG-INFO` & `raya-3.4.1.dev3/src/raya.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raya
-Version: 3.4.1.dev0
+Version: 3.4.1.dev3
 Summary: Unlimited Robotics - Ra-Ya Python Library
 Home-page: https://documentation.unlimited-robotics.com/
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Platform: UNKNOWN
```

### Comparing `raya-3.4.1.dev0/src/raya.egg-info/SOURCES.txt` & `raya-3.4.1.dev3/src/raya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

