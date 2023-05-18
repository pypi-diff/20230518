# Comparing `tmp/manim_course_utils-0.7.0.tar.gz` & `tmp/manim_course_utils-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_course_utils-0.7.0.tar", max compression
+gzip compressed data, was "manim_course_utils-0.8.0.tar", max compression
```

## Comparing `manim_course_utils-0.7.0.tar` & `manim_course_utils-0.8.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      112 2023-05-11 22:31:16.319862 manim_course_utils-0.7.0/manim_course_utils/__init__.py
--rw-r--r--   0        0        0     2817 2023-05-18 14:44:07.740116 manim_course_utils-0.7.0/manim_course_utils/animation_description.py
--rw-r--r--   0        0        0      273 2023-05-11 22:31:05.058757 manim_course_utils-0.7.0/manim_course_utils/markdown_tex_template.py
--rw-r--r--   0        0        0     1928 2023-05-18 14:50:58.336660 manim_course_utils-0.7.0/manim_course_utils/mobject_description.py
--rw-r--r--   0        0        0      520 2023-05-18 14:51:51.280532 manim_course_utils-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-05-11 16:15:04.015818 manim_course_utils-0.7.0/README.md
--rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 manim_course_utils-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-05-11 22:31:16.319862 manim_course_utils-0.8.0/manim_course_utils/__init__.py
+-rw-r--r--   0        0        0     2971 2023-05-18 15:00:51.357510 manim_course_utils-0.8.0/manim_course_utils/animation_description.py
+-rw-r--r--   0        0        0      296 2023-05-18 15:05:19.239167 manim_course_utils-0.8.0/manim_course_utils/markdown_tex_template.py
+-rw-r--r--   0        0        0     2082 2023-05-18 15:00:22.904911 manim_course_utils-0.8.0/manim_course_utils/mobject_description.py
+-rw-r--r--   0        0        0      520 2023-05-18 15:05:42.893530 manim_course_utils-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-11 16:15:04.015818 manim_course_utils-0.8.0/README.md
+-rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 manim_course_utils-0.8.0/PKG-INFO
```

### Comparing `manim_course_utils-0.7.0/manim_course_utils/animation_description.py` & `manim_course_utils-0.8.0/manim_course_utils/animation_description.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,16 +13,19 @@
         title: str | None = None,
         description: str | None = None,
         rec_config: dict | None = None
     ):
         super().__init__()
         self.mobject_to_animate = mobject_to_animate
         self.animation = animation
-        self.title = title or animation.__class__.__name__
+        self.title = animation.__class__.__name__ or title
         self.description = description or animation.__doc__
+        examples_idx = self.description.find("Examples")
+        if examples_idx != -1:
+            self.description = self.description[:examples_idx]
         self.rec_config = rec_config or {
             "stroke_color": WHITE,
             "stroke_width": 2,
             "fill_color": BLACK,
             "fill_opacity": 0.5,
             "buff": 0.2,
             "corner_radius": 0.2
@@ -48,15 +51,15 @@
         mobject_to_animate: Mobject,
         animation: Animation,
         description: str | None = None,
         title: str | None = None
     ):
         self[1].become(mobject_to_animate)
         self.set_description(description or animation.__doc__)
-        self.set_title(title or animation.__class__.__name__)
+        self.set_title(animation.__class__.__name__ or title)
         self.animation = animation
         return self
     
     def set_animation(self, animation: Animation, description: str | None = None, title: str | None = None):
         self.set_mobject_and_animation(self.mobject_to_animate, animation, description, title)
         return self
```

### Comparing `manim_course_utils-0.7.0/manim_course_utils/mobject_description.py` & `manim_course_utils-0.8.0/manim_course_utils/mobject_description.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,18 @@
         description: str | None = None,
         rec_config: dict | None = None,
         **kwargs
     ):
         super().__init__(**kwargs)
         self.mobject = mobject
         self.description = mobject.__doc__ if description is None else description
-        self.title = title or mobject.__class__.__name__
+        examples_idx = self.description.find("Examples")
+        if examples_idx != -1:
+            self.description = self.description[:examples_idx]
+        self.title = mobject.__class__.__name__ or title
         self.title_mobject = Tex(f"\\textbf{{{title}}}", font_size=36)
         self.description_mobject = Tex(self.description, font_size=24, tex_environment="markdown", tex_template=MarkdownTexTemplate())
         self.add(self.title_mobject, self.mobject, self.description_mobject)
         self.arrange(DOWN, buff=0.5)
         rec_config = rec_config or {
             "stroke_color": WHITE,
             "stroke_width": 2,
@@ -41,9 +44,9 @@
         self.title = title
         self[0].become(Tex(f"\\textbf{{{title}}}", font_size=36))
         return self
     
     def set_mobject(self, mobject: Mobject, description: str | None = None, title: str | None = None):
         self[1].become(mobject)
         self.set_description(mobject.__doc__ if description is None else description)
-        self.set_title(title or mobject.__class__.__name__)
+        self.set_title(mobject.__class__.__name__ or title)
         return self
```

### Comparing `manim_course_utils-0.7.0/pyproject.toml` & `manim_course_utils-0.8.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "manim-course-utils"
-version = "0.7.0"
+version = "0.8.0"
 description = "Para el curso de ManimCE de MathLike"
 homepage = "https://github.com/MathLike/manim-course-utils"
 repository = "https://github.com/MathLike/manim-course-utils"
 authors = ["MathLike <benjamin.ubilla@uc.cl>"]
 readme = "README.md"
 packages = [{include = "manim_course_utils"}]
```

### Comparing `manim_course_utils-0.7.0/PKG-INFO` & `manim_course_utils-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim-course-utils
-Version: 0.7.0
+Version: 0.8.0
 Summary: Para el curso de ManimCE de MathLike
 Home-page: https://github.com/MathLike/manim-course-utils
 Author: MathLike
 Author-email: benjamin.ubilla@uc.cl
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

