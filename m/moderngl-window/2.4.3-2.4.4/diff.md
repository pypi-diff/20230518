# Comparing `tmp/moderngl-window-2.4.3.tar.gz` & `tmp/moderngl-window-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moderngl-window-2.4.3.tar", last modified: Fri Mar  3 12:02:44 2023, max compression
+gzip compressed data, was "moderngl-window-2.4.4.tar", last modified: Thu May 18 11:08:07 2023, max compression
```

## Comparing `moderngl-window-2.4.3.tar` & `moderngl-window-2.4.4.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.424526 moderngl-window-2.4.3/
--rw-rw-rw-   0        0        0     1111 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/LICENSE
--rw-rw-rw-   0        0        0      153 2021-07-23 20:25:43.000000 moderngl-window-2.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7784 2023-03-03 12:02:44.425525 moderngl-window-2.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     6456 2022-06-18 19:36:00.000000 moderngl-window-2.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.329435 moderngl-window-2.4.3/moderngl_window/
--rw-rw-rw-   0        0        0    10375 2023-03-03 11:56:03.000000 moderngl-window-2.4.3/moderngl_window/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.340436 moderngl-window-2.4.3/moderngl_window/atlas/
--rw-rw-rw-   0        0        0     1890 2022-06-18 19:36:00.000000 moderngl-window-2.4.3/moderngl_window/atlas/base.py
--rw-rw-rw-   0        0        0     5195 2022-06-18 19:36:00.000000 moderngl-window-2.4.3/moderngl_window/atlas/simple_atlas.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.342434 moderngl-window-2.4.3/moderngl_window/capture/
--rw-rw-rw-   0        0        0       87 2022-06-18 19:36:00.000000 moderngl-window-2.4.3/moderngl_window/capture/__init__.py
--rw-rw-rw-   0        0        0     4715 2022-06-18 19:36:00.000000 moderngl-window-2.4.3/moderngl_window/capture/base.py
--rw-rw-rw-   0        0        0     3333 2022-06-18 19:36:00.000000 moderngl-window-2.4.3/moderngl_window/capture/ffmpeg.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.344434 moderngl-window-2.4.3/moderngl_window/conf/
--rw-rw-rw-   0        0        0    10728 2020-08-22 11:45:34.000000 moderngl-window-2.4.3/moderngl_window/conf/__init__.py
--rw-rw-rw-   0        0        0     1502 2020-08-22 11:45:09.000000 moderngl-window-2.4.3/moderngl_window/conf/default.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.315435 moderngl-window-2.4.3/moderngl_window/context/
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.346436 moderngl-window-2.4.3/moderngl_window/context/base/
--rw-rw-rw-   0        0        0      160 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/context/base/__init__.py
--rw-rw-rw-   0        0        0     2128 2021-05-13 09:43:41.000000 moderngl-window-2.4.3/moderngl_window/context/base/keys.py
--rw-rw-rw-   0        0        0    48854 2022-09-17 17:49:27.000000 moderngl-window-2.4.3/moderngl_window/context/base/window.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.348436 moderngl-window-2.4.3/moderngl_window/context/glfw/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/context/glfw/__init__.py
--rw-rw-rw-   0        0        0     2387 2021-07-23 20:25:43.000000 moderngl-window-2.4.3/moderngl_window/context/glfw/keys.py
--rw-rw-rw-   0        0        0    13120 2022-09-17 17:48:16.000000 moderngl-window-2.4.3/moderngl_window/context/glfw/window.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.350438 moderngl-window-2.4.3/moderngl_window/context/headless/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/context/headless/__init__.py
--rw-rw-rw-   0        0        0       88 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/context/headless/keys.py
--rw-rw-rw-   0        0        0     2650 2022-09-17 16:15:36.000000 moderngl-window-2.4.3/moderngl_window/context/headless/window.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.352436 moderngl-window-2.4.3/moderngl_window/context/pygame2/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/context/pygame2/__init__.py
--rw-rw-rw-   0        0        0     2391 2020-08-23 14:24:53.000000 moderngl-window-2.4.3/moderngl_window/context/pygame2/keys.py
--rw-rw-rw-   0        0        0    10243 2022-09-17 16:53:28.000000 moderngl-window-2.4.3/moderngl_window/context/pygame2/window.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.355435 moderngl-window-2.4.3/moderngl_window/context/pyglet/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/context/pyglet/__init__.py
--rw-rw-rw-   0        0        0     2203 2020-08-23 14:15:48.000000 moderngl-window-2.4.3/moderngl_window/context/pyglet/keys.py
--rw-rw-rw-   0        0        0    12084 2022-09-17 16:13:06.000000 moderngl-window-2.4.3/moderngl_window/context/pyglet/window.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.357436 moderngl-window-2.4.3/moderngl_window/context/pyqt5/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/context/pyqt5/__init__.py
--rw-rw-rw-   0        0        0     2263 2020-08-23 14:28:19.000000 moderngl-window-2.4.3/moderngl_window/context/pyqt5/keys.py
--rw-rw-rw-   0        0        0    11931 2022-09-17 16:59:34.000000 moderngl-window-2.4.3/moderngl_window/context/pyqt5/window.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.359436 moderngl-window-2.4.3/moderngl_window/context/pyside2/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/context/pyside2/__init__.py
--rw-rw-rw-   0        0        0     2217 2020-08-23 14:28:38.000000 moderngl-window-2.4.3/moderngl_window/context/pyside2/keys.py
--rw-rw-rw-   0        0        0    11907 2022-09-17 17:01:54.000000 moderngl-window-2.4.3/moderngl_window/context/pyside2/window.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.362436 moderngl-window-2.4.3/moderngl_window/context/sdl2/
--rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/context/sdl2/__init__.py
--rw-rw-rw-   0        0        0     2473 2020-08-23 14:33:13.000000 moderngl-window-2.4.3/moderngl_window/context/sdl2/keys.py
--rw-rw-rw-   0        0        0    10430 2022-09-17 17:08:24.000000 moderngl-window-2.4.3/moderngl_window/context/sdl2/window.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.364438 moderngl-window-2.4.3/moderngl_window/context/tk/
--rw-rw-rw-   0        0        0      120 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/context/tk/__init__.py
--rw-rw-rw-   0        0        0     2153 2020-08-23 14:35:15.000000 moderngl-window-2.4.3/moderngl_window/context/tk/keys.py
--rw-rw-rw-   0        0        0     9364 2022-09-17 17:02:40.000000 moderngl-window-2.4.3/moderngl_window/context/tk/window.py
--rw-rw-rw-   0        0        0      137 2020-08-23 13:56:44.000000 moderngl-window-2.4.3/moderngl_window/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.367436 moderngl-window-2.4.3/moderngl_window/finders/
--rw-rw-rw-   0        0        0     3309 2020-08-22 11:47:29.000000 moderngl-window-2.4.3/moderngl_window/finders/base.py
--rw-rw-rw-   0        0        0      328 2020-08-22 11:47:29.000000 moderngl-window-2.4.3/moderngl_window/finders/data.py
--rw-rw-rw-   0        0        0      340 2020-08-22 11:47:29.000000 moderngl-window-2.4.3/moderngl_window/finders/program.py
--rw-rw-rw-   0        0        0      333 2020-08-22 11:47:29.000000 moderngl-window-2.4.3/moderngl_window/finders/scene.py
--rw-rw-rw-   0        0        0      341 2020-08-22 11:47:29.000000 moderngl-window-2.4.3/moderngl_window/finders/texture.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.372438 moderngl-window-2.4.3/moderngl_window/geometry/
--rw-rw-rw-   0        0        0      312 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/geometry/__init__.py
--rw-rw-rw-   0        0        0     2305 2020-08-23 13:52:57.000000 moderngl-window-2.4.3/moderngl_window/geometry/attributes.py
--rw-rw-rw-   0        0        0     2058 2020-08-23 13:52:38.000000 moderngl-window-2.4.3/moderngl_window/geometry/bbox.py
--rw-rw-rw-   0        0        0     5375 2020-08-23 13:52:07.000000 moderngl-window-2.4.3/moderngl_window/geometry/cube.py
--rw-rw-rw-   0        0        0     2552 2023-03-03 11:50:20.000000 moderngl-window-2.4.3/moderngl_window/geometry/quad.py
--rw-rw-rw-   0        0        0     2656 2020-08-23 13:48:13.000000 moderngl-window-2.4.3/moderngl_window/geometry/sphere.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.373437 moderngl-window-2.4.3/moderngl_window/integrations/
--rw-rw-rw-   0        0        0     9890 2023-03-03 11:50:20.000000 moderngl-window-2.4.3/moderngl_window/integrations/imgui.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.374436 moderngl-window-2.4.3/moderngl_window/loaders/
--rw-rw-rw-   0        0        0     3739 2021-05-13 09:43:41.000000 moderngl-window-2.4.3/moderngl_window/loaders/base.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.376434 moderngl-window-2.4.3/moderngl_window/loaders/data/
--rw-rw-rw-   0        0        0      759 2020-08-23 13:54:00.000000 moderngl-window-2.4.3/moderngl_window/loaders/data/binary.py
--rw-rw-rw-   0        0        0      811 2020-08-23 13:54:00.000000 moderngl-window-2.4.3/moderngl_window/loaders/data/json.py
--rw-rw-rw-   0        0        0      803 2020-08-23 13:54:00.000000 moderngl-window-2.4.3/moderngl_window/loaders/data/text.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.378436 moderngl-window-2.4.3/moderngl_window/loaders/program/
--rw-rw-rw-   0        0        0     3339 2020-08-23 13:54:00.000000 moderngl-window-2.4.3/moderngl_window/loaders/program/separate.py
--rw-rw-rw-   0        0        0     2390 2020-08-23 13:54:00.000000 moderngl-window-2.4.3/moderngl_window/loaders/program/single.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.380435 moderngl-window-2.4.3/moderngl_window/loaders/scene/
--rw-rw-rw-   0        0        0    28338 2020-10-24 12:28:27.000000 moderngl-window-2.4.3/moderngl_window/loaders/scene/gltf2.py
--rw-rw-rw-   0        0        0     1648 2021-11-04 20:22:25.000000 moderngl-window-2.4.3/moderngl_window/loaders/scene/stl.py
--rw-rw-rw-   0        0        0     5710 2020-08-23 13:54:00.000000 moderngl-window-2.4.3/moderngl_window/loaders/scene/wavefront.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.384437 moderngl-window-2.4.3/moderngl_window/loaders/texture/
--rw-rw-rw-   0        0        0     1443 2020-08-23 13:54:00.000000 moderngl-window-2.4.3/moderngl_window/loaders/texture/array.py
--rw-rw-rw-   0        0        0     2908 2020-08-23 13:54:00.000000 moderngl-window-2.4.3/moderngl_window/loaders/texture/cube.py
--rw-rw-rw-   0        0        0      709 2020-08-23 13:54:00.000000 moderngl-window-2.4.3/moderngl_window/loaders/texture/icon.py
--rw-rw-rw-   0        0        0     3826 2020-08-23 13:54:00.000000 moderngl-window-2.4.3/moderngl_window/loaders/texture/pillow.py
--rw-rw-rw-   0        0        0     1037 2020-08-23 13:54:00.000000 moderngl-window-2.4.3/moderngl_window/loaders/texture/t2d.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.388434 moderngl-window-2.4.3/moderngl_window/meta/
--rw-rw-rw-   0        0        0      186 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/meta/__init__.py
--rw-rw-rw-   0        0        0     2915 2020-08-22 11:48:01.000000 moderngl-window-2.4.3/moderngl_window/meta/base.py
--rw-rw-rw-   0        0        0     1345 2020-10-24 12:28:35.000000 moderngl-window-2.4.3/moderngl_window/meta/data.py
--rw-rw-rw-   0        0        0     4415 2021-07-23 20:25:43.000000 moderngl-window-2.4.3/moderngl_window/meta/program.py
--rw-rw-rw-   0        0        0     1960 2020-10-24 12:29:08.000000 moderngl-window-2.4.3/moderngl_window/meta/scene.py
--rw-rw-rw-   0        0        0     5301 2020-08-23 12:37:41.000000 moderngl-window-2.4.3/moderngl_window/meta/texture.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.391437 moderngl-window-2.4.3/moderngl_window/opengl/
--rw-rw-rw-   0        0        0    15473 2021-07-23 20:25:43.000000 moderngl-window-2.4.3/moderngl_window/opengl/program.py
--rw-rw-rw-   0        0        0     2780 2020-08-22 11:50:55.000000 moderngl-window-2.4.3/moderngl_window/opengl/projection.py
--rw-rw-rw-   0        0        0     4878 2020-10-24 12:28:52.000000 moderngl-window-2.4.3/moderngl_window/opengl/types.py
--rw-rw-rw-   0        0        0    13379 2020-08-22 11:50:56.000000 moderngl-window-2.4.3/moderngl_window/opengl/vao.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.398442 moderngl-window-2.4.3/moderngl_window/resources/
--rw-rw-rw-   0        0        0     3211 2021-05-13 09:43:41.000000 moderngl-window-2.4.3/moderngl_window/resources/__init__.py
--rw-rw-rw-   0        0        0     4035 2020-08-23 13:56:01.000000 moderngl-window-2.4.3/moderngl_window/resources/base.py
--rw-rw-rw-   0        0        0      644 2020-08-23 13:56:01.000000 moderngl-window-2.4.3/moderngl_window/resources/data.py
--rw-rw-rw-   0        0        0      482 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/resources/decorators.py
--rw-rw-rw-   0        0        0     1087 2020-08-23 13:56:01.000000 moderngl-window-2.4.3/moderngl_window/resources/programs.py
--rw-rw-rw-   0        0        0      671 2020-08-23 13:56:01.000000 moderngl-window-2.4.3/moderngl_window/resources/scenes.py
--rw-rw-rw-   0        0        0      860 2021-05-13 09:43:41.000000 moderngl-window-2.4.3/moderngl_window/resources/textures.py
--rw-rw-rw-   0        0        0      650 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/resources/tracks.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.403443 moderngl-window-2.4.3/moderngl_window/scene/
--rw-rw-rw-   0        0        0      317 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/scene/__init__.py
--rw-rw-rw-   0        0        0    18806 2023-03-03 11:50:20.000000 moderngl-window-2.4.3/moderngl_window/scene/camera.py
--rw-rw-rw-   0        0        0     2547 2020-08-22 11:49:55.000000 moderngl-window-2.4.3/moderngl_window/scene/material.py
--rw-rw-rw-   0        0        0     4868 2020-08-22 11:49:55.000000 moderngl-window-2.4.3/moderngl_window/scene/mesh.py
--rw-rw-rw-   0        0        0     5946 2020-08-22 11:49:55.000000 moderngl-window-2.4.3/moderngl_window/scene/node.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.320437 moderngl-window-2.4.3/moderngl_window/scene/programs/
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.411444 moderngl-window-2.4.3/moderngl_window/scene/programs/scene_default/
--rw-rw-rw-   0        0        0      476 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/scene/programs/scene_default/bbox.glsl
--rw-rw-rw-   0        0        0     1139 2020-06-06 23:23:21.000000 moderngl-window-2.4.3/moderngl_window/scene/programs/scene_default/color_light.glsl
--rw-rw-rw-   0        0        0      365 2020-01-10 17:44:38.000000 moderngl-window-2.4.3/moderngl_window/scene/programs/scene_default/fallback.glsl
--rw-rw-rw-   0        0        0      458 2020-06-07 01:31:46.000000 moderngl-window-2.4.3/moderngl_window/scene/programs/scene_default/texture.glsl
--rw-rw-rw-   0        0        0      796 2020-06-06 22:55:31.000000 moderngl-window-2.4.3/moderngl_window/scene/programs/scene_default/texture_light.glsl
--rw-rw-rw-   0        0        0      426 2020-06-07 01:12:04.000000 moderngl-window-2.4.3/moderngl_window/scene/programs/scene_default/vertex_color.glsl
--rw-rw-rw-   0        0        0      559 2020-06-07 01:51:45.000000 moderngl-window-2.4.3/moderngl_window/scene/programs/scene_default/vertex_color_texture.glsl
--rw-rw-rw-   0        0        0      500 2020-06-06 23:25:16.000000 moderngl-window-2.4.3/moderngl_window/scene/programs/scene_default/wireframe.glsl
--rw-rw-rw-   0        0        0     8516 2020-08-22 11:49:55.000000 moderngl-window-2.4.3/moderngl_window/scene/programs.py
--rw-rw-rw-   0        0        0     9744 2020-08-22 11:49:55.000000 moderngl-window-2.4.3/moderngl_window/scene/scene.py
--rw-rw-rw-   0        0        0     2590 2020-08-23 13:56:52.000000 moderngl-window-2.4.3/moderngl_window/screenshot.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.320437 moderngl-window-2.4.3/moderngl_window/text/
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.414528 moderngl-window-2.4.3/moderngl_window/text/bitmapped/
--rw-rw-rw-   0        0        0       43 2021-06-22 07:43:02.000000 moderngl-window-2.4.3/moderngl_window/text/bitmapped/__init__.py
--rw-rw-rw-   0        0        0     1954 2021-06-22 07:43:02.000000 moderngl-window-2.4.3/moderngl_window/text/bitmapped/base.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.321437 moderngl-window-2.4.3/moderngl_window/text/bitmapped/bitmapped/
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.415527 moderngl-window-2.4.3/moderngl_window/text/bitmapped/bitmapped/programs/
--rw-rw-rw-   0        0        0     1696 2021-06-22 07:43:02.000000 moderngl-window-2.4.3/moderngl_window/text/bitmapped/bitmapped/programs/text_2d.glsl
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.416526 moderngl-window-2.4.3/moderngl_window/text/bitmapped/bitmapped/text/
--rw-rw-rw-   0        0        0      262 2021-06-22 07:43:02.000000 moderngl-window-2.4.3/moderngl_window/text/bitmapped/bitmapped/text/meta.json
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.417528 moderngl-window-2.4.3/moderngl_window/text/bitmapped/bitmapped/textures/
--rw-rw-rw-   0        0        0   318186 2021-06-22 07:43:02.000000 moderngl-window-2.4.3/moderngl_window/text/bitmapped/bitmapped/textures/VeraMono.png
--rw-rw-rw-   0        0        0     2804 2022-06-18 19:36:00.000000 moderngl-window-2.4.3/moderngl_window/text/bitmapped/text_2d.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.420528 moderngl-window-2.4.3/moderngl_window/timers/
--rw-rw-rw-   0        0        0     1792 2020-08-22 11:46:40.000000 moderngl-window-2.4.3/moderngl_window/timers/base.py
--rw-rw-rw-   0        0        0     2805 2021-05-13 09:43:41.000000 moderngl-window-2.4.3/moderngl_window/timers/clock.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.424526 moderngl-window-2.4.3/moderngl_window/utils/
--rw-rw-rw-   0        0        0       42 2020-10-19 05:57:32.000000 moderngl-window-2.4.3/moderngl_window/utils/__init__.py
--rw-rw-rw-   0        0        0      747 2023-03-03 11:50:20.000000 moderngl-window-2.4.3/moderngl_window/utils/keymaps.py
--rw-rw-rw-   0        0        0      837 2020-08-22 11:46:20.000000 moderngl-window-2.4.3/moderngl_window/utils/module_loading.py
--rw-rw-rw-   0        0        0     5381 2020-10-24 12:29:20.000000 moderngl-window-2.4.3/moderngl_window/utils/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-03-03 12:02:44.338436 moderngl-window-2.4.3/moderngl_window.egg-info/
--rw-rw-rw-   0        0        0     7784 2023-03-03 12:02:43.000000 moderngl-window-2.4.3/moderngl_window.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4458 2023-03-03 12:02:44.000000 moderngl-window-2.4.3/moderngl_window.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 12:02:43.000000 moderngl-window-2.4.3/moderngl_window.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2023-03-03 12:02:43.000000 moderngl-window-2.4.3/moderngl_window.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-03 12:02:43.000000 moderngl-window-2.4.3/moderngl_window.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-03 12:02:44.429523 moderngl-window-2.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1952 2023-03-03 12:01:19.000000 moderngl-window-2.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.893470 moderngl-window-2.4.4/
+-rw-rw-rw-   0        0        0     1111 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/LICENSE
+-rw-rw-rw-   0        0        0      153 2021-07-23 20:25:43.000000 moderngl-window-2.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     7785 2023-05-18 11:08:07.893470 moderngl-window-2.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6456 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.765136 moderngl-window-2.4.4/moderngl_window/
+-rw-rw-rw-   0        0        0    10564 2023-05-18 11:00:51.000000 moderngl-window-2.4.4/moderngl_window/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.773368 moderngl-window-2.4.4/moderngl_window/atlas/
+-rw-rw-rw-   0        0        0     1890 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/moderngl_window/atlas/base.py
+-rw-rw-rw-   0        0        0     5195 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/moderngl_window/atlas/simple_atlas.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.775879 moderngl-window-2.4.4/moderngl_window/capture/
+-rw-rw-rw-   0        0        0       87 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/moderngl_window/capture/__init__.py
+-rw-rw-rw-   0        0        0     4715 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/moderngl_window/capture/base.py
+-rw-rw-rw-   0        0        0     3333 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/moderngl_window/capture/ffmpeg.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.777886 moderngl-window-2.4.4/moderngl_window/conf/
+-rw-rw-rw-   0        0        0    10728 2020-08-22 11:45:34.000000 moderngl-window-2.4.4/moderngl_window/conf/__init__.py
+-rw-rw-rw-   0        0        0     1502 2020-08-22 11:45:09.000000 moderngl-window-2.4.4/moderngl_window/conf/default.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.749621 moderngl-window-2.4.4/moderngl_window/context/
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.780884 moderngl-window-2.4.4/moderngl_window/context/base/
+-rw-rw-rw-   0        0        0      160 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/base/__init__.py
+-rw-rw-rw-   0        0        0     2128 2021-05-13 09:43:41.000000 moderngl-window-2.4.4/moderngl_window/context/base/keys.py
+-rw-rw-rw-   0        0        0    49412 2023-05-18 09:43:10.000000 moderngl-window-2.4.4/moderngl_window/context/base/window.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.782885 moderngl-window-2.4.4/moderngl_window/context/glfw/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/glfw/__init__.py
+-rw-rw-rw-   0        0        0     2387 2021-07-23 20:25:43.000000 moderngl-window-2.4.4/moderngl_window/context/glfw/keys.py
+-rw-rw-rw-   0        0        0    13168 2023-05-18 08:48:42.000000 moderngl-window-2.4.4/moderngl_window/context/glfw/window.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.785393 moderngl-window-2.4.4/moderngl_window/context/headless/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/headless/__init__.py
+-rw-rw-rw-   0        0        0       88 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/headless/keys.py
+-rw-rw-rw-   0        0        0     2925 2023-05-18 09:50:27.000000 moderngl-window-2.4.4/moderngl_window/context/headless/window.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.788401 moderngl-window-2.4.4/moderngl_window/context/pygame2/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/pygame2/__init__.py
+-rw-rw-rw-   0        0        0     2391 2020-08-23 14:24:53.000000 moderngl-window-2.4.4/moderngl_window/context/pygame2/keys.py
+-rw-rw-rw-   0        0        0    10311 2023-05-18 08:48:42.000000 moderngl-window-2.4.4/moderngl_window/context/pygame2/window.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.791400 moderngl-window-2.4.4/moderngl_window/context/pyglet/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/pyglet/__init__.py
+-rw-rw-rw-   0        0        0     2203 2020-08-23 14:15:48.000000 moderngl-window-2.4.4/moderngl_window/context/pyglet/keys.py
+-rw-rw-rw-   0        0        0    12218 2023-05-18 08:48:42.000000 moderngl-window-2.4.4/moderngl_window/context/pyglet/window.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.793399 moderngl-window-2.4.4/moderngl_window/context/pyqt5/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/pyqt5/__init__.py
+-rw-rw-rw-   0        0        0     2263 2020-08-23 14:28:19.000000 moderngl-window-2.4.4/moderngl_window/context/pyqt5/keys.py
+-rw-rw-rw-   0        0        0    11967 2023-05-18 08:48:42.000000 moderngl-window-2.4.4/moderngl_window/context/pyqt5/window.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.796607 moderngl-window-2.4.4/moderngl_window/context/pyside2/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/pyside2/__init__.py
+-rw-rw-rw-   0        0        0     2217 2020-08-23 14:28:38.000000 moderngl-window-2.4.4/moderngl_window/context/pyside2/keys.py
+-rw-rw-rw-   0        0        0    11943 2023-05-18 08:48:42.000000 moderngl-window-2.4.4/moderngl_window/context/pyside2/window.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.798605 moderngl-window-2.4.4/moderngl_window/context/sdl2/
+-rw-rw-rw-   0        0        0       68 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/sdl2/__init__.py
+-rw-rw-rw-   0        0        0     2473 2020-08-23 14:33:13.000000 moderngl-window-2.4.4/moderngl_window/context/sdl2/keys.py
+-rw-rw-rw-   0        0        0    10499 2023-05-18 08:48:42.000000 moderngl-window-2.4.4/moderngl_window/context/sdl2/window.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.801606 moderngl-window-2.4.4/moderngl_window/context/tk/
+-rw-rw-rw-   0        0        0      120 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/context/tk/__init__.py
+-rw-rw-rw-   0        0        0     2153 2020-08-23 14:35:15.000000 moderngl-window-2.4.4/moderngl_window/context/tk/keys.py
+-rw-rw-rw-   0        0        0     9364 2022-09-17 17:02:40.000000 moderngl-window-2.4.4/moderngl_window/context/tk/window.py
+-rw-rw-rw-   0        0        0      137 2020-08-23 13:56:44.000000 moderngl-window-2.4.4/moderngl_window/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.805113 moderngl-window-2.4.4/moderngl_window/finders/
+-rw-rw-rw-   0        0        0     3309 2020-08-22 11:47:29.000000 moderngl-window-2.4.4/moderngl_window/finders/base.py
+-rw-rw-rw-   0        0        0      328 2020-08-22 11:47:29.000000 moderngl-window-2.4.4/moderngl_window/finders/data.py
+-rw-rw-rw-   0        0        0      340 2020-08-22 11:47:29.000000 moderngl-window-2.4.4/moderngl_window/finders/program.py
+-rw-rw-rw-   0        0        0      333 2020-08-22 11:47:29.000000 moderngl-window-2.4.4/moderngl_window/finders/scene.py
+-rw-rw-rw-   0        0        0      341 2020-08-22 11:47:29.000000 moderngl-window-2.4.4/moderngl_window/finders/texture.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.811121 moderngl-window-2.4.4/moderngl_window/geometry/
+-rw-rw-rw-   0        0        0      312 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/geometry/__init__.py
+-rw-rw-rw-   0        0        0     2305 2020-08-23 13:52:57.000000 moderngl-window-2.4.4/moderngl_window/geometry/attributes.py
+-rw-rw-rw-   0        0        0     2058 2020-08-23 13:52:38.000000 moderngl-window-2.4.4/moderngl_window/geometry/bbox.py
+-rw-rw-rw-   0        0        0     5375 2020-08-23 13:52:07.000000 moderngl-window-2.4.4/moderngl_window/geometry/cube.py
+-rw-rw-rw-   0        0        0     2552 2023-03-03 11:50:20.000000 moderngl-window-2.4.4/moderngl_window/geometry/quad.py
+-rw-rw-rw-   0        0        0     2656 2020-08-23 13:48:13.000000 moderngl-window-2.4.4/moderngl_window/geometry/sphere.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.813120 moderngl-window-2.4.4/moderngl_window/integrations/
+-rw-rw-rw-   0        0        0     9890 2023-03-03 11:50:20.000000 moderngl-window-2.4.4/moderngl_window/integrations/imgui.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.814119 moderngl-window-2.4.4/moderngl_window/loaders/
+-rw-rw-rw-   0        0        0     3739 2021-05-13 09:43:41.000000 moderngl-window-2.4.4/moderngl_window/loaders/base.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.816301 moderngl-window-2.4.4/moderngl_window/loaders/data/
+-rw-rw-rw-   0        0        0      759 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/data/binary.py
+-rw-rw-rw-   0        0        0      811 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/data/json.py
+-rw-rw-rw-   0        0        0      803 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/data/text.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.818304 moderngl-window-2.4.4/moderngl_window/loaders/program/
+-rw-rw-rw-   0        0        0     3339 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/program/separate.py
+-rw-rw-rw-   0        0        0     2390 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/program/single.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.821303 moderngl-window-2.4.4/moderngl_window/loaders/scene/
+-rw-rw-rw-   0        0        0    28338 2020-10-24 12:28:27.000000 moderngl-window-2.4.4/moderngl_window/loaders/scene/gltf2.py
+-rw-rw-rw-   0        0        0     1648 2021-11-04 20:22:25.000000 moderngl-window-2.4.4/moderngl_window/loaders/scene/stl.py
+-rw-rw-rw-   0        0        0     5710 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/scene/wavefront.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.825301 moderngl-window-2.4.4/moderngl_window/loaders/texture/
+-rw-rw-rw-   0        0        0     1443 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/texture/array.py
+-rw-rw-rw-   0        0        0     2908 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/texture/cube.py
+-rw-rw-rw-   0        0        0      709 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/texture/icon.py
+-rw-rw-rw-   0        0        0     3826 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/texture/pillow.py
+-rw-rw-rw-   0        0        0     1037 2020-08-23 13:54:00.000000 moderngl-window-2.4.4/moderngl_window/loaders/texture/t2d.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.859784 moderngl-window-2.4.4/moderngl_window/meta/
+-rw-rw-rw-   0        0        0      186 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/meta/__init__.py
+-rw-rw-rw-   0        0        0     2915 2020-08-22 11:48:01.000000 moderngl-window-2.4.4/moderngl_window/meta/base.py
+-rw-rw-rw-   0        0        0     1345 2020-10-24 12:28:35.000000 moderngl-window-2.4.4/moderngl_window/meta/data.py
+-rw-rw-rw-   0        0        0     4415 2021-07-23 20:25:43.000000 moderngl-window-2.4.4/moderngl_window/meta/program.py
+-rw-rw-rw-   0        0        0     1960 2020-10-24 12:29:08.000000 moderngl-window-2.4.4/moderngl_window/meta/scene.py
+-rw-rw-rw-   0        0        0     5301 2020-08-23 12:37:41.000000 moderngl-window-2.4.4/moderngl_window/meta/texture.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.862780 moderngl-window-2.4.4/moderngl_window/opengl/
+-rw-rw-rw-   0        0        0    15473 2021-07-23 20:25:43.000000 moderngl-window-2.4.4/moderngl_window/opengl/program.py
+-rw-rw-rw-   0        0        0     2780 2020-08-22 11:50:55.000000 moderngl-window-2.4.4/moderngl_window/opengl/projection.py
+-rw-rw-rw-   0        0        0     4878 2020-10-24 12:28:52.000000 moderngl-window-2.4.4/moderngl_window/opengl/types.py
+-rw-rw-rw-   0        0        0    13379 2020-08-22 11:50:56.000000 moderngl-window-2.4.4/moderngl_window/opengl/vao.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.869302 moderngl-window-2.4.4/moderngl_window/resources/
+-rw-rw-rw-   0        0        0     3211 2021-05-13 09:43:41.000000 moderngl-window-2.4.4/moderngl_window/resources/__init__.py
+-rw-rw-rw-   0        0        0     4035 2020-08-23 13:56:01.000000 moderngl-window-2.4.4/moderngl_window/resources/base.py
+-rw-rw-rw-   0        0        0      644 2020-08-23 13:56:01.000000 moderngl-window-2.4.4/moderngl_window/resources/data.py
+-rw-rw-rw-   0        0        0      482 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/resources/decorators.py
+-rw-rw-rw-   0        0        0     1087 2020-08-23 13:56:01.000000 moderngl-window-2.4.4/moderngl_window/resources/programs.py
+-rw-rw-rw-   0        0        0      671 2020-08-23 13:56:01.000000 moderngl-window-2.4.4/moderngl_window/resources/scenes.py
+-rw-rw-rw-   0        0        0      860 2021-05-13 09:43:41.000000 moderngl-window-2.4.4/moderngl_window/resources/textures.py
+-rw-rw-rw-   0        0        0      650 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/resources/tracks.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.875300 moderngl-window-2.4.4/moderngl_window/scene/
+-rw-rw-rw-   0        0        0      317 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/scene/__init__.py
+-rw-rw-rw-   0        0        0    18808 2023-05-18 08:47:55.000000 moderngl-window-2.4.4/moderngl_window/scene/camera.py
+-rw-rw-rw-   0        0        0     2547 2020-08-22 11:49:55.000000 moderngl-window-2.4.4/moderngl_window/scene/material.py
+-rw-rw-rw-   0        0        0     4868 2020-08-22 11:49:55.000000 moderngl-window-2.4.4/moderngl_window/scene/mesh.py
+-rw-rw-rw-   0        0        0     5946 2020-08-22 11:49:55.000000 moderngl-window-2.4.4/moderngl_window/scene/node.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.755125 moderngl-window-2.4.4/moderngl_window/scene/programs/
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.882340 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/
+-rw-rw-rw-   0        0        0      476 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/bbox.glsl
+-rw-rw-rw-   0        0        0     1139 2020-06-06 23:23:21.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/color_light.glsl
+-rw-rw-rw-   0        0        0      365 2020-01-10 17:44:38.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/fallback.glsl
+-rw-rw-rw-   0        0        0      458 2020-06-07 01:31:46.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/texture.glsl
+-rw-rw-rw-   0        0        0      796 2020-06-06 22:55:31.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/texture_light.glsl
+-rw-rw-rw-   0        0        0      426 2020-06-07 01:12:04.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/vertex_color.glsl
+-rw-rw-rw-   0        0        0      559 2020-06-07 01:51:45.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/vertex_color_texture.glsl
+-rw-rw-rw-   0        0        0      500 2020-06-06 23:25:16.000000 moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/wireframe.glsl
+-rw-rw-rw-   0        0        0     8516 2020-08-22 11:49:55.000000 moderngl-window-2.4.4/moderngl_window/scene/programs.py
+-rw-rw-rw-   0        0        0     9744 2020-08-22 11:49:55.000000 moderngl-window-2.4.4/moderngl_window/scene/scene.py
+-rw-rw-rw-   0        0        0     2590 2020-08-23 13:56:52.000000 moderngl-window-2.4.4/moderngl_window/screenshot.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.756131 moderngl-window-2.4.4/moderngl_window/text/
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.885339 moderngl-window-2.4.4/moderngl_window/text/bitmapped/
+-rw-rw-rw-   0        0        0       43 2021-06-22 07:43:02.000000 moderngl-window-2.4.4/moderngl_window/text/bitmapped/__init__.py
+-rw-rw-rw-   0        0        0     1954 2021-06-22 07:43:02.000000 moderngl-window-2.4.4/moderngl_window/text/bitmapped/base.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.757131 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.885339 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/programs/
+-rw-rw-rw-   0        0        0     1696 2021-06-22 07:43:02.000000 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/programs/text_2d.glsl
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.886471 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/text/
+-rw-rw-rw-   0        0        0      262 2021-06-22 07:43:02.000000 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/text/meta.json
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.887470 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/textures/
+-rw-rw-rw-   0        0        0   318186 2021-06-22 07:43:02.000000 moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/textures/VeraMono.png
+-rw-rw-rw-   0        0        0     2804 2022-06-18 19:36:00.000000 moderngl-window-2.4.4/moderngl_window/text/bitmapped/text_2d.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.890470 moderngl-window-2.4.4/moderngl_window/timers/
+-rw-rw-rw-   0        0        0     1792 2020-08-22 11:46:40.000000 moderngl-window-2.4.4/moderngl_window/timers/base.py
+-rw-rw-rw-   0        0        0     2805 2021-05-13 09:43:41.000000 moderngl-window-2.4.4/moderngl_window/timers/clock.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.893470 moderngl-window-2.4.4/moderngl_window/utils/
+-rw-rw-rw-   0        0        0       42 2020-10-19 05:57:32.000000 moderngl-window-2.4.4/moderngl_window/utils/__init__.py
+-rw-rw-rw-   0        0        0      755 2023-05-18 08:47:36.000000 moderngl-window-2.4.4/moderngl_window/utils/keymaps.py
+-rw-rw-rw-   0        0        0      837 2020-08-22 11:46:20.000000 moderngl-window-2.4.4/moderngl_window/utils/module_loading.py
+-rw-rw-rw-   0        0        0     5381 2020-10-24 12:29:20.000000 moderngl-window-2.4.4/moderngl_window/utils/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-05-18 11:08:07.772367 moderngl-window-2.4.4/moderngl_window.egg-info/
+-rw-rw-rw-   0        0        0     7785 2023-05-18 11:08:07.000000 moderngl-window-2.4.4/moderngl_window.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4458 2023-05-18 11:08:07.000000 moderngl-window-2.4.4/moderngl_window.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 11:08:07.000000 moderngl-window-2.4.4/moderngl_window.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2023-05-18 11:08:07.000000 moderngl-window-2.4.4/moderngl_window.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-18 11:08:07.000000 moderngl-window-2.4.4/moderngl_window.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-18 11:08:07.898991 moderngl-window-2.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1953 2023-05-18 08:50:47.000000 moderngl-window-2.4.4/setup.py
```

### Comparing `moderngl-window-2.4.3/LICENSE` & `moderngl-window-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/PKG-INFO` & `moderngl-window-2.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moderngl-window
-Version: 2.4.3
+Version: 2.4.4
 Summary: A cross platform helper library for ModernGL making window creation and resource loading simple
 Home-page: https://github.com/moderngl/moderngl_window
 Author: Einar Forselv
 Author-email: eforselv@gmail.com
 License: MIT
 Project-URL: Documentation, https://moderngl-window.readthedocs.io
 Project-URL: ModernGL, https://github.com/moderngl/moderngl
@@ -13,18 +13,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: PySide2
 Provides-Extra: pyqt5
 Provides-Extra: glfw
 Provides-Extra: PySDL2
 Provides-Extra: pywavefront
```

### Comparing `moderngl-window-2.4.3/README.md` & `moderngl-window-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/__init__.py` & `moderngl-window-2.4.4/moderngl_window/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from typing import List, Type
 
 import moderngl
 from moderngl_window.context.base import WindowConfig, BaseWindow
 from moderngl_window.timers.clock import Timer
 from moderngl_window.conf import settings
 from moderngl_window.utils.module_loading import import_string
-from moderngl_window.utils.keymaps import KeyMapFactory, KeyMap, QWERTY, AZERTY
+from moderngl_window.utils.keymaps import KeyMapFactory, KeyMap, QWERTY, AZERTY  # noqa
 
-__version__ = "2.4.3"
+__version__ = "2.4.4"
 
 IGNORE_DIRS = [
     "__pycache__",
     "base",
 ]
 
 # Add new windows classes here to be recognized by the command line option --window
@@ -200,14 +200,15 @@
         if values.resizable is not None
         else config_cls.resizable,
         gl_version=config_cls.gl_version,
         aspect_ratio=config_cls.aspect_ratio,
         vsync=values.vsync if values.vsync is not None else config_cls.vsync,
         samples=values.samples if values.samples is not None else config_cls.samples,
         cursor=show_cursor if show_cursor is not None else True,
+        backend=values.backend,
     )
     window.print_context_info()
     activate_context(window=window)
     timer = timer or Timer()
     config = config_cls(ctx=window.ctx, wnd=window, timer=timer)
     # Avoid the event assigning in the property setter for now
     # We want the even assigning to happen in WindowConfig.__init__
@@ -288,14 +289,18 @@
     )
     parser.add_argument(
         "--size_mult",
         type=valid_window_size_multiplier,
         default=1.0,
         help="Multiplier for the window size making it easy scale the window",
     )
+    parser.add_argument(
+        "--backend",
+        help="Specify context backend. This is mostly used to enable EGL in headless mode",
+    )
     return parser
 
 
 def parse_args(args=None, parser=None):
     """Parse arguments from sys.argv
 
     Passing in your own argparser can be user to extend the parser.
```

### Comparing `moderngl-window-2.4.3/moderngl_window/atlas/base.py` & `moderngl-window-2.4.4/moderngl_window/atlas/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/atlas/simple_atlas.py` & `moderngl-window-2.4.4/moderngl_window/atlas/simple_atlas.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/capture/base.py` & `moderngl-window-2.4.4/moderngl_window/capture/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/capture/ffmpeg.py` & `moderngl-window-2.4.4/moderngl_window/capture/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/conf/__init__.py` & `moderngl-window-2.4.4/moderngl_window/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/conf/default.py` & `moderngl-window-2.4.4/moderngl_window/conf/default.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/context/base/keys.py` & `moderngl-window-2.4.4/moderngl_window/context/base/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/context/base/window.py` & `moderngl-window-2.4.4/moderngl_window/context/base/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from argparse import ArgumentParser, Namespace
+from argparse import ArgumentParser
 from functools import wraps
 from pathlib import Path
 import logging
 import sys
 import weakref
-from typing import Any, Tuple, Type, List
+from typing import Any, Tuple, Type, List, Optional
 
 import moderngl
 from moderngl_window.context.base import KeyModifiers, BaseKeys
 from moderngl_window.timers.base import BaseTimer
 from moderngl_window import resources
 from moderngl_window.geometry.attributes import AttributeNames
 from moderngl_window.meta import (
@@ -83,14 +83,15 @@
         size=(1280, 720),
         resizable=True,
         fullscreen=False,
         vsync=True,
         aspect_ratio: float = None,
         samples=0,
         cursor=True,
+        backend: Optional[str] = None,
         **kwargs
     ):
         """Initialize a window instance.
 
         Args:
             title (str): The window title
             gl_version (tuple): Major and minor version of the opengl context to create
@@ -110,14 +111,17 @@
         self._resizable = resizable
         self._buffer_width, self._buffer_height = size
         self._fullscreen = fullscreen
         self._vsync = vsync
         self._fixed_aspect_ratio = aspect_ratio
         self._samples = samples
         self._cursor = cursor
+        self._backend = backend
+        self._headless = False
+
         self._exit_key = self.keys.ESCAPE
         self._fs_key = self.keys.F11
 
         # Callback functions
         self._render_func = dummy_func
         self._resize_func = dummy_func
         self._close_func = dummy_func
@@ -170,14 +174,30 @@
 
     @property
     def ctx(self) -> moderngl.Context:
         """moderngl.Context: The ModernGL context for the window"""
         return self._ctx
 
     @property
+    def backend(self) -> Optional[str]:
+        """
+        Name of the context backend.
+
+        This is ``None`` unless a backend is explicitly specified
+        during context creation. The main use case for this is to
+        enable EGL in headless mode.
+        """
+        return self._backend
+
+    @property
+    def headless(self) -> bool:
+        """bool: Is the window headless?"""
+        return self._headless
+
+    @property
     def fbo(self) -> moderngl.Framebuffer:
         """moderngl.Framebuffer: The default framebuffer"""
         return self._ctx.screen
 
     @property
     def title(self) -> str:
         """str: Window title.
```

### Comparing `moderngl-window-2.4.3/moderngl_window/context/glfw/keys.py` & `moderngl-window-2.4.4/moderngl_window/context/glfw/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/context/glfw/window.py` & `moderngl-window-2.4.4/moderngl_window/context/glfw/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         glfw.window_hint(glfw.CONTEXT_VERSION_MAJOR, self.gl_version[0])
         glfw.window_hint(glfw.CONTEXT_VERSION_MINOR, self.gl_version[1])
         glfw.window_hint(glfw.OPENGL_PROFILE, glfw.OPENGL_CORE_PROFILE)
         glfw.window_hint(glfw.OPENGL_FORWARD_COMPAT, True)
         glfw.window_hint(glfw.RESIZABLE, self.resizable)
         glfw.window_hint(glfw.DOUBLEBUFFER, True)
         glfw.window_hint(glfw.DEPTH_BITS, 24)
+        glfw.window_hint(glfw.STENCIL_BITS, 8)
         glfw.window_hint(glfw.SAMPLES, self.samples)
         glfw.window_hint(glfw.SCALE_TO_MONITOR, glfw.TRUE)
 
         monitor = None
 
         self._window = glfw.create_window(
             self.width, self.height, self.title, monitor, None
```

### Comparing `moderngl-window-2.4.3/moderngl_window/context/headless/window.py` & `moderngl-window-2.4.4/moderngl_window/context/headless/window.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,25 +16,35 @@
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._fbo = None
         self._vsync = False  # We don't care about vsync in headless mode
         self._resizable = False  # headless window is not resizable
         self._cursor = False  # Headless don't have a cursor
+        self._headless = True
         self.init_mgl_context()
         self.set_default_viewport()
 
     @property
     def fbo(self) -> moderngl.Framebuffer:
         """moderngl.Framebuffer: The default framebuffer"""
         return self._fbo
 
     def init_mgl_context(self) -> None:
         """Create an standalone context and framebuffer"""
-        self._ctx = moderngl.create_standalone_context(require=self.gl_version_code)
+        if self._backend:
+            self._ctx = moderngl.create_standalone_context(
+                require=self.gl_version_code,
+                backend=self._backend,
+            )
+        else:
+            self._ctx = moderngl.create_standalone_context(
+                require=self.gl_version_code,
+            )
+
         self._fbo = self.ctx.framebuffer(
             color_attachments=self.ctx.texture(self.size, 4, samples=self._samples),
             depth_attachment=self.ctx.depth_texture(self.size, samples=self._samples),
         )
         self.use()
 
     def use(self):
```

### Comparing `moderngl-window-2.4.3/moderngl_window/context/pygame2/keys.py` & `moderngl-window-2.4.4/moderngl_window/context/pygame2/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/context/pygame2/window.py` & `moderngl-window-2.4.4/moderngl_window/context/pygame2/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         )
         pygame.display.gl_set_attribute(
             pygame.GL_CONTEXT_PROFILE_MASK, pygame.GL_CONTEXT_PROFILE_CORE
         )
         pygame.display.gl_set_attribute(pygame.GL_CONTEXT_FORWARD_COMPATIBLE_FLAG, 1)
         pygame.display.gl_set_attribute(pygame.GL_DOUBLEBUFFER, 1)
         pygame.display.gl_set_attribute(pygame.GL_DEPTH_SIZE, 24)
+        pygame.display.gl_set_attribute(pygame.GL_STENCIL_SIZE, 8)
 
         if self.samples > 1:
             pygame.display.gl_set_attribute(pygame.GL_MULTISAMPLEBUFFERS, 1)
             pygame.display.gl_set_attribute(pygame.GL_MULTISAMPLESAMPLES, self.samples)
 
         self._depth = 24
         self._flags = pygame.OPENGL | pygame.DOUBLEBUF
```

### Comparing `moderngl-window-2.4.3/moderngl_window/context/pyglet/keys.py` & `moderngl-window-2.4.4/moderngl_window/context/pyglet/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/context/pyglet/window.py` & `moderngl-window-2.4.4/moderngl_window/context/pyglet/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,19 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         config = pyglet.gl.Config(
             major_version=self.gl_version[0],
             minor_version=self.gl_version[1],
             forward_compatible=True,
+            red_size=8,
+            green_size=8,
+            blue_size=8,
+            alpha_size=8,
+            stencil_size=8,
             depth_size=24,
             double_buffer=True,
             sample_buffers=1 if self.samples > 1 else 0,
             samples=self.samples,
         )
 
         if self.fullscreen:
```

### Comparing `moderngl-window-2.4.3/moderngl_window/context/pyqt5/keys.py` & `moderngl-window-2.4.4/moderngl_window/context/pyqt5/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/context/pyqt5/window.py` & `moderngl-window-2.4.4/moderngl_window/context/pyqt5/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         super().__init__(**kwargs)
 
         # Specify OpenGL context parameters
         gl = QtOpenGL.QGLFormat()
         gl.setVersion(self.gl_version[0], self.gl_version[1])
         gl.setProfile(QtOpenGL.QGLFormat.CoreProfile)
         gl.setDepthBufferSize(24)
+        gl.setStencilBufferSize(8)
         gl.setDoubleBuffer(True)
         gl.setSwapInterval(1 if self._vsync else 0)
 
         # Configure multisampling if needed
         if self.samples > 1:
             gl.setSampleBuffers(True)
             gl.setSamples(int(self.samples))
```

### Comparing `moderngl-window-2.4.3/moderngl_window/context/pyside2/keys.py` & `moderngl-window-2.4.4/moderngl_window/context/pyside2/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/context/pyside2/window.py` & `moderngl-window-2.4.4/moderngl_window/context/pyside2/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         super().__init__(**kwargs)
 
         # Specify OpenGL context parameters
         gl = QtOpenGL.QGLFormat()
         gl.setVersion(self.gl_version[0], self.gl_version[1])
         gl.setProfile(QtOpenGL.QGLFormat.CoreProfile)
         gl.setDepthBufferSize(24)
+        gl.setStencilBufferSize(8)
         gl.setDoubleBuffer(True)
         gl.setSwapInterval(1 if self.vsync else 0)
 
         # Configure multisampling if needed
         if self.samples > 1:
             gl.setSampleBuffers(True)
             gl.setSamples(self.samples)
```

### Comparing `moderngl-window-2.4.3/moderngl_window/context/sdl2/keys.py` & `moderngl-window-2.4.4/moderngl_window/context/sdl2/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/context/sdl2/window.py` & `moderngl-window-2.4.4/moderngl_window/context/sdl2/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         )
         sdl2.video.SDL_GL_SetAttribute(
             sdl2.SDL_GL_CONTEXT_PROFILE_MASK, sdl2.SDL_GL_CONTEXT_PROFILE_CORE
         )
         sdl2.video.SDL_GL_SetAttribute(sdl2.SDL_GL_CONTEXT_FORWARD_COMPATIBLE_FLAG, 1)
         sdl2.video.SDL_GL_SetAttribute(sdl2.SDL_GL_DOUBLEBUFFER, 1)
         sdl2.video.SDL_GL_SetAttribute(sdl2.SDL_GL_DEPTH_SIZE, 24)
+        sdl2.video.SDL_GL_SetAttribute(sdl2.SDL_GL_STENCIL_SIZE, 8)
 
         self.cursor = self._cursor
 
         if self.samples > 1:
             sdl2.video.SDL_GL_SetAttribute(sdl2.SDL_GL_MULTISAMPLEBUFFERS, 1)
             sdl2.video.SDL_GL_SetAttribute(sdl2.SDL_GL_MULTISAMPLESAMPLES, self.samples)
```

### Comparing `moderngl-window-2.4.3/moderngl_window/context/tk/keys.py` & `moderngl-window-2.4.4/moderngl_window/context/tk/keys.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/context/tk/window.py` & `moderngl-window-2.4.4/moderngl_window/context/tk/window.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/finders/base.py` & `moderngl-window-2.4.4/moderngl_window/finders/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/geometry/attributes.py` & `moderngl-window-2.4.4/moderngl_window/geometry/attributes.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/geometry/bbox.py` & `moderngl-window-2.4.4/moderngl_window/geometry/bbox.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/geometry/cube.py` & `moderngl-window-2.4.4/moderngl_window/geometry/cube.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/geometry/quad.py` & `moderngl-window-2.4.4/moderngl_window/geometry/quad.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/geometry/sphere.py` & `moderngl-window-2.4.4/moderngl_window/geometry/sphere.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/integrations/imgui.py` & `moderngl-window-2.4.4/moderngl_window/integrations/imgui.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/base.py` & `moderngl-window-2.4.4/moderngl_window/loaders/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/data/binary.py` & `moderngl-window-2.4.4/moderngl_window/loaders/data/binary.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/data/json.py` & `moderngl-window-2.4.4/moderngl_window/loaders/data/json.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/data/text.py` & `moderngl-window-2.4.4/moderngl_window/loaders/data/text.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/program/separate.py` & `moderngl-window-2.4.4/moderngl_window/loaders/program/separate.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/program/single.py` & `moderngl-window-2.4.4/moderngl_window/loaders/program/single.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/scene/gltf2.py` & `moderngl-window-2.4.4/moderngl_window/loaders/scene/gltf2.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/scene/stl.py` & `moderngl-window-2.4.4/moderngl_window/loaders/scene/stl.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/scene/wavefront.py` & `moderngl-window-2.4.4/moderngl_window/loaders/scene/wavefront.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/texture/array.py` & `moderngl-window-2.4.4/moderngl_window/loaders/texture/array.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/texture/cube.py` & `moderngl-window-2.4.4/moderngl_window/loaders/texture/cube.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/texture/icon.py` & `moderngl-window-2.4.4/moderngl_window/loaders/texture/icon.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/texture/pillow.py` & `moderngl-window-2.4.4/moderngl_window/loaders/texture/pillow.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/loaders/texture/t2d.py` & `moderngl-window-2.4.4/moderngl_window/loaders/texture/t2d.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/meta/base.py` & `moderngl-window-2.4.4/moderngl_window/meta/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/meta/data.py` & `moderngl-window-2.4.4/moderngl_window/meta/data.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/meta/program.py` & `moderngl-window-2.4.4/moderngl_window/meta/program.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/meta/scene.py` & `moderngl-window-2.4.4/moderngl_window/meta/scene.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/meta/texture.py` & `moderngl-window-2.4.4/moderngl_window/meta/texture.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/opengl/program.py` & `moderngl-window-2.4.4/moderngl_window/opengl/program.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/opengl/projection.py` & `moderngl-window-2.4.4/moderngl_window/opengl/projection.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/opengl/types.py` & `moderngl-window-2.4.4/moderngl_window/opengl/types.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/opengl/vao.py` & `moderngl-window-2.4.4/moderngl_window/opengl/vao.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/resources/__init__.py` & `moderngl-window-2.4.4/moderngl_window/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/resources/base.py` & `moderngl-window-2.4.4/moderngl_window/resources/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/resources/data.py` & `moderngl-window-2.4.4/moderngl_window/resources/data.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/resources/programs.py` & `moderngl-window-2.4.4/moderngl_window/resources/programs.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/resources/scenes.py` & `moderngl-window-2.4.4/moderngl_window/resources/scenes.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/resources/textures.py` & `moderngl-window-2.4.4/moderngl_window/resources/textures.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/resources/tracks.py` & `moderngl-window-2.4.4/moderngl_window/resources/tracks.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/scene/camera.py` & `moderngl-window-2.4.4/moderngl_window/scene/camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         # Update aspect ratio
         camera.projection.update(aspect_ratio=1.0)
 
         # Get projection matrix in bytes (f4)
         camera.projection.tobytes()
     """
 
-    def __init__(self, keys: BaseKeys, keymap: KeyMapFactory=QWERTY, fov=60.0, aspect_ratio=1.0, near=1.0, far=100.0):
+    def __init__(self, keys: BaseKeys, keymap: KeyMapFactory = QWERTY, fov=60.0, aspect_ratio=1.0, near=1.0, far=100.0):
         """Initialize the camera
 
         Args:
             keys (BaseKeys): The key constants for the current window type
         Keyword Args:
             keymap (KeyMapFactory) : The keymap to use. By default QWERTY.
             fov (float): Field of view
```

### Comparing `moderngl-window-2.4.3/moderngl_window/scene/material.py` & `moderngl-window-2.4.4/moderngl_window/scene/material.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/scene/mesh.py` & `moderngl-window-2.4.4/moderngl_window/scene/mesh.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/scene/node.py` & `moderngl-window-2.4.4/moderngl_window/scene/node.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/scene/programs/scene_default/color_light.glsl` & `moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/color_light.glsl`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/scene/programs/scene_default/texture_light.glsl` & `moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/texture_light.glsl`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/scene/programs/scene_default/vertex_color_texture.glsl` & `moderngl-window-2.4.4/moderngl_window/scene/programs/scene_default/vertex_color_texture.glsl`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/scene/programs.py` & `moderngl-window-2.4.4/moderngl_window/scene/programs.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/scene/scene.py` & `moderngl-window-2.4.4/moderngl_window/scene/scene.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/screenshot.py` & `moderngl-window-2.4.4/moderngl_window/screenshot.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/text/bitmapped/base.py` & `moderngl-window-2.4.4/moderngl_window/text/bitmapped/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/text/bitmapped/bitmapped/programs/text_2d.glsl` & `moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/programs/text_2d.glsl`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/text/bitmapped/bitmapped/textures/VeraMono.png` & `moderngl-window-2.4.4/moderngl_window/text/bitmapped/bitmapped/textures/VeraMono.png`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/text/bitmapped/text_2d.py` & `moderngl-window-2.4.4/moderngl_window/text/bitmapped/text_2d.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/timers/base.py` & `moderngl-window-2.4.4/moderngl_window/timers/base.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/timers/clock.py` & `moderngl-window-2.4.4/moderngl_window/timers/clock.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/utils/keymaps.py` & `moderngl-window-2.4.4/moderngl_window/utils/keymaps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from collections import namedtuple
 from typing import Callable
 
 from moderngl_window.context.base.keys import BaseKeys
 
 KeyMap = namedtuple("KeyMap", ["UP", "DOWN", "LEFT", "RIGHT", "FORWARD", "BACKWARD"])
 
-# A factory is used since we cannot deduce the keys format before run time, as they are induced by the window software used; 
+# A factory is used since we cannot deduce the keys format before run time, as they are
+# induced by the window software used.
 # Therefore, the factory takes as a parameter the keys used, and return a keymap instance.
 KeyMapFactory = Callable[[BaseKeys], KeyMap]
-AZERTY : KeyMapFactory = lambda keys : KeyMap(UP=keys.A, DOWN=keys.E, LEFT=keys.Q, RIGHT = keys.D, FORWARD=keys.Z, BACKWARD=keys.S)
-QWERTY : KeyMapFactory = lambda keys : KeyMap(UP=keys.Q, DOWN=keys.E, LEFT=keys.A, RIGHT = keys.D, FORWARD=keys.W, BACKWARD=keys.S)
-
+AZERTY: KeyMapFactory = lambda keys: KeyMap(
+    UP=keys.A, DOWN=keys.E, LEFT=keys.Q, RIGHT=keys.D, FORWARD=keys.Z, BACKWARD=keys.S
+)
+QWERTY: KeyMapFactory = lambda keys: KeyMap(
+    UP=keys.Q, DOWN=keys.E, LEFT=keys.A, RIGHT=keys.D, FORWARD=keys.W, BACKWARD=keys.S
+)
```

### Comparing `moderngl-window-2.4.3/moderngl_window/utils/module_loading.py` & `moderngl-window-2.4.4/moderngl_window/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window/utils/scheduler.py` & `moderngl-window-2.4.4/moderngl_window/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/moderngl_window.egg-info/PKG-INFO` & `moderngl-window-2.4.4/moderngl_window.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moderngl-window
-Version: 2.4.3
+Version: 2.4.4
 Summary: A cross platform helper library for ModernGL making window creation and resource loading simple
 Home-page: https://github.com/moderngl/moderngl_window
 Author: Einar Forselv
 Author-email: eforselv@gmail.com
 License: MIT
 Project-URL: Documentation, https://moderngl-window.readthedocs.io
 Project-URL: ModernGL, https://github.com/moderngl/moderngl
@@ -13,18 +13,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: PySide2
 Provides-Extra: pyqt5
 Provides-Extra: glfw
 Provides-Extra: PySDL2
 Provides-Extra: pywavefront
```

### Comparing `moderngl-window-2.4.3/moderngl_window.egg-info/SOURCES.txt` & `moderngl-window-2.4.4/moderngl_window.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moderngl-window-2.4.3/setup.py` & `moderngl-window-2.4.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="moderngl-window",
-    version="2.4.3",
+    version="2.4.4",
     description="A cross platform helper library for ModernGL making window creation and resource loading simple",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/moderngl/moderngl_window",
     author="Einar Forselv",
     author_email="eforselv@gmail.com",
     packages=find_namespace_packages(include=['moderngl_window', 'moderngl_window.*']),
@@ -19,18 +19,18 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Topic :: Games/Entertainment',
         'Topic :: Multimedia :: Graphics',
         'Topic :: Multimedia :: Graphics :: 3D Rendering',
         'Topic :: Scientific/Engineering :: Visualization',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     install_requires=[
         'moderngl<6',
         'pyglet>=2.0dev23',
         'numpy>=1.16,<2',
         'pyrr>=0.10.3,<1',
         'Pillow>=9,<10',
```

