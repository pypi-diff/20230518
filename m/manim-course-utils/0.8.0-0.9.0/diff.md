# Comparing `tmp/manim_course_utils-0.8.0.tar.gz` & `tmp/manim_course_utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_course_utils-0.8.0.tar", max compression
+gzip compressed data, was "manim_course_utils-0.9.0.tar", max compression
```

## Comparing `manim_course_utils-0.8.0.tar` & `manim_course_utils-0.9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      112 2023-05-11 22:31:16.319862 manim_course_utils-0.8.0/manim_course_utils/__init__.py
--rw-r--r--   0        0        0     2971 2023-05-18 15:00:51.357510 manim_course_utils-0.8.0/manim_course_utils/animation_description.py
--rw-r--r--   0        0        0      296 2023-05-18 15:05:19.239167 manim_course_utils-0.8.0/manim_course_utils/markdown_tex_template.py
--rw-r--r--   0        0        0     2082 2023-05-18 15:00:22.904911 manim_course_utils-0.8.0/manim_course_utils/mobject_description.py
--rw-r--r--   0        0        0      520 2023-05-18 15:05:42.893530 manim_course_utils-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-05-11 16:15:04.015818 manim_course_utils-0.8.0/README.md
--rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 manim_course_utils-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-05-11 22:31:16.319862 manim_course_utils-0.9.0/manim_course_utils/__init__.py
+-rw-r--r--   0        0        0     2971 2023-05-18 15:00:51.357510 manim_course_utils-0.9.0/manim_course_utils/animation_description.py
+-rw-r--r--   0        0        0      318 2023-05-18 15:11:19.800699 manim_course_utils-0.9.0/manim_course_utils/markdown_tex_template.py
+-rw-r--r--   0        0        0     2082 2023-05-18 15:00:22.904911 manim_course_utils-0.9.0/manim_course_utils/mobject_description.py
+-rw-r--r--   0        0        0      520 2023-05-18 15:11:29.768456 manim_course_utils-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-11 16:15:04.015818 manim_course_utils-0.9.0/README.md
+-rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 manim_course_utils-0.9.0/PKG-INFO
```

### Comparing `manim_course_utils-0.8.0/manim_course_utils/animation_description.py` & `manim_course_utils-0.9.0/manim_course_utils/animation_description.py`

 * *Files identical despite different names*

### Comparing `manim_course_utils-0.8.0/manim_course_utils/mobject_description.py` & `manim_course_utils-0.9.0/manim_course_utils/mobject_description.py`

 * *Files identical despite different names*

### Comparing `manim_course_utils-0.8.0/pyproject.toml` & `manim_course_utils-0.9.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "manim-course-utils"
-version = "0.8.0"
+version = "0.9.0"
 description = "Para el curso de ManimCE de MathLike"
 homepage = "https://github.com/MathLike/manim-course-utils"
 repository = "https://github.com/MathLike/manim-course-utils"
 authors = ["MathLike <benjamin.ubilla@uc.cl>"]
 readme = "README.md"
 packages = [{include = "manim_course_utils"}]
```

### Comparing `manim_course_utils-0.8.0/PKG-INFO` & `manim_course_utils-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-course-utils
-Version: 0.8.0
+Version: 0.9.0
 Summary: Para el curso de ManimCE de MathLike
 Home-page: https://github.com/MathLike/manim-course-utils
 Author: MathLike
 Author-email: benjamin.ubilla@uc.cl
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

