# Comparing `tmp/pydantic_view-0.2.1.tar.gz` & `tmp/pydantic_view-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_view-0.2.1.tar", max compression
+gzip compressed data, was "pydantic_view-0.2.2.tar", max compression
```

## Comparing `pydantic_view-0.2.1.tar` & `pydantic_view-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.000000 pydantic_view-0.2.1/LICENSE
--rw-r--r--   0        0        0     5704 2023-05-07 10:28:55.000000 pydantic_view-0.2.1/README.md
--rw-r--r--   0        0        0      183 2023-05-10 12:31:33.000000 pydantic_view-0.2.1/pydantic_view/__init__.py
--rw-r--r--   0        0        0     8356 2023-05-15 11:56:56.000000 pydantic_view-0.2.1/pydantic_view/pydantic_view.py
--rw-r--r--   0        0        0      876 2023-05-15 11:59:13.000000 pydantic_view-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 pydantic_view-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.000000 pydantic_view-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5704 2023-05-07 10:28:55.000000 pydantic_view-0.2.2/README.md
+-rw-r--r--   0        0        0      183 2023-05-10 12:31:33.000000 pydantic_view-0.2.2/pydantic_view/__init__.py
+-rw-r--r--   0        0        0     8395 2023-05-18 11:21:26.000000 pydantic_view-0.2.2/pydantic_view/pydantic_view.py
+-rw-r--r--   0        0        0      876 2023-05-18 11:31:57.000000 pydantic_view-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 pydantic_view-0.2.2/PKG-INFO
```

### Comparing `pydantic_view-0.2.1/LICENSE` & `pydantic_view-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.2.1/README.md` & `pydantic_view-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.2.1/pydantic_view/pydantic_view.py` & `pydantic_view-0.2.2/pydantic_view/pydantic_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,27 +147,27 @@
 
         if recursive is True:
 
             def update_type(tp):
                 if isinstance(tp, _GenericAlias):
                     tp.__args__ = tuple(update_type(arg) for arg in tp.__args__)
                 elif isinstance(tp, type) and issubclass(tp, BaseModel):
-                    for _name in (name, *tp.__bases__):
-                        if hasattr(tp, name):
-                            tp = getattr(tp, name)
+                    for _name in (name, *(base or [])):
+                        if hasattr(tp, _name):
+                            tp = getattr(tp, _name)
                             break
                 return tp
 
             def update_field_type(field):
                 if field.sub_fields:
                     for sub_field in field.sub_fields:
                         update_field_type(sub_field)
-                else:
-                    field.type_ = update_type(field.type_)
-                    field.prepare()
+                field.type_ = update_type(field.type_)
+                field.outer_type_ = update_type(field.outer_type_)
+                field.prepare()
                 if (
                     isinstance(field.default_factory, type)
                     and issubclass(field.default_factory, BaseModel)
                     and hasattr(field.default_factory, name)
                 ):
                     field.default_factory = getattr(field.default_factory, name)
```

### Comparing `pydantic_view-0.2.1/pyproject.toml` & `pydantic_view-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-view"
-version = "0.2.1"
+version = "0.2.2"
 description = "View decorator to create the child pydantic models from the root model."
 authors = ["Roman Koshel <roma.koshel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pydantic", "model", "view", "utils"]
 packages = [{include = "pydantic_view"}]
 classifiers = [
```

### Comparing `pydantic_view-0.2.1/PKG-INFO` & `pydantic_view-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-view
-Version: 0.2.1
+Version: 0.2.2
 Summary: View decorator to create the child pydantic models from the root model.
 License: MIT
 Keywords: pydantic,model,view,utils
 Author: Roman Koshel
 Author-email: roma.koshel@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

