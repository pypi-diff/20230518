# Comparing `tmp/mokkari-2.3.3.tar.gz` & `tmp/mokkari-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mokkari-2.3.3.tar", max compression
+gzip compressed data, was "mokkari-2.4.0.tar", max compression
```

## Comparing `mokkari-2.3.3.tar` & `mokkari-2.4.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0    35149 2022-10-23 14:33:42.067151 mokkari-2.3.3/LICENSE
--rw-r--r--   0        0        0     1946 2022-10-23 14:33:42.067151 mokkari-2.3.3/README.rst
--rw-r--r--   0        0        0      992 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/__init__.py
--rw-r--r--   0        0        0     2803 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/arc.py
--rw-r--r--   0        0        0     3396 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/character.py
--rw-r--r--   0        0        0     3183 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/creator.py
--rw-r--r--   0        0        0      750 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/exceptions.py
--rw-r--r--   0        0        0     1148 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/genre.py
--rw-r--r--   0        0        0     9004 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/issue.py
--rw-r--r--   0        0        0     3100 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/publisher.py
--rw-r--r--   0        0        0     1148 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/rating.py
--rw-r--r--   0        0        0     1213 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/reprint.py
--rw-r--r--   0        0        0     7345 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/series.py
--rw-r--r--   0        0        0    14156 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/session.py
--rw-r--r--   0        0        0     2103 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/sqlite_cache.py
--rw-r--r--   0        0        0     2986 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/team.py
--rw-r--r--   0        0        0     1259 2022-10-23 14:33:42.067151 mokkari-2.3.3/mokkari/variant.py
--rw-r--r--   0        0        0     2334 2022-10-23 14:33:42.067151 mokkari-2.3.3/pyproject.toml
--rw-r--r--   0        0        0      544 2022-10-23 14:33:42.067151 mokkari-2.3.3/tests/README.md
--rw-r--r--   0        0        0       25 2022-10-23 14:33:42.067151 mokkari-2.3.3/tests/__init__.py
--rw-r--r--   0        0        0      734 2022-10-23 14:33:42.067151 mokkari-2.3.3/tests/conftest.py
--rw-r--r--   0        0        0     2590 2022-10-23 14:33:42.067151 mokkari-2.3.3/tests/test_arcs.py
--rw-r--r--   0        0        0     2075 2022-10-23 14:33:42.067151 mokkari-2.3.3/tests/test_cache.py
--rw-r--r--   0        0        0     3087 2022-10-23 14:33:42.071151 mokkari-2.3.3/tests/test_characters.py
--rw-r--r--   0        0        0     2594 2022-10-23 14:33:42.071151 mokkari-2.3.3/tests/test_creator.py
--rw-r--r--   0        0        0      659 2022-10-23 14:33:42.071151 mokkari-2.3.3/tests/test_init.py
--rw-r--r--   0        0        0    10082 2022-10-23 14:33:42.071151 mokkari-2.3.3/tests/test_issues.py
--rw-r--r--   0        0        0     2476 2022-10-23 14:33:42.071151 mokkari-2.3.3/tests/test_publishers.py
--rw-r--r--   0        0        0      714 2022-10-23 14:33:42.071151 mokkari-2.3.3/tests/test_role.py
--rw-r--r--   0        0        0     4091 2022-10-23 14:33:42.071151 mokkari-2.3.3/tests/test_series.py
--rw-r--r--   0        0        0      734 2022-10-23 14:33:42.071151 mokkari-2.3.3/tests/test_series_type.py
--rw-r--r--   0        0        0     2648 2022-10-23 14:33:42.071151 mokkari-2.3.3/tests/test_teams.py
--rw-r--r--   0        0        0   544768 2022-10-23 14:33:42.071151 mokkari-2.3.3/tests/testing_mock.sqlite
--rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 mokkari-2.3.3/setup.py
--rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 mokkari-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-18 12:27:13.789870 mokkari-2.4.0/LICENSE
+-rw-r--r--   0        0        0     1946 2023-05-18 12:27:13.789870 mokkari-2.4.0/README.rst
+-rw-r--r--   0        0        0      992 2023-05-18 12:27:13.789870 mokkari-2.4.0/mokkari/__init__.py
+-rw-r--r--   0        0        0     2960 2023-05-18 12:27:13.789870 mokkari-2.4.0/mokkari/arc.py
+-rw-r--r--   0        0        0     3553 2023-05-18 12:27:13.789870 mokkari-2.4.0/mokkari/character.py
+-rw-r--r--   0        0        0     3338 2023-05-18 12:27:13.789870 mokkari-2.4.0/mokkari/creator.py
+-rw-r--r--   0        0        0      750 2023-05-18 12:27:13.789870 mokkari-2.4.0/mokkari/exceptions.py
+-rw-r--r--   0        0        0     1148 2023-05-18 12:27:13.789870 mokkari-2.4.0/mokkari/genre.py
+-rw-r--r--   0        0        0     9157 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/issue.py
+-rw-r--r--   0        0        0     3257 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/publisher.py
+-rw-r--r--   0        0        0     1148 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/rating.py
+-rw-r--r--   0        0        0     1213 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/reprint.py
+-rw-r--r--   0        0        0     7499 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/series.py
+-rw-r--r--   0        0        0    14156 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/session.py
+-rw-r--r--   0        0        0     2103 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/sqlite_cache.py
+-rw-r--r--   0        0        0     3138 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/team.py
+-rw-r--r--   0        0        0     1259 2023-05-18 12:27:13.793870 mokkari-2.4.0/mokkari/variant.py
+-rw-r--r--   0        0        0     2334 2023-05-18 12:27:13.793870 mokkari-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      544 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/README.md
+-rw-r--r--   0        0        0       25 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      734 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     2590 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_arcs.py
+-rw-r--r--   0        0        0     2075 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_cache.py
+-rw-r--r--   0        0        0     3087 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_characters.py
+-rw-r--r--   0        0        0     2594 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_creator.py
+-rw-r--r--   0        0        0      659 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_init.py
+-rw-r--r--   0        0        0    10082 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_issues.py
+-rw-r--r--   0        0        0     2476 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_publishers.py
+-rw-r--r--   0        0        0      714 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_role.py
+-rw-r--r--   0        0        0     4091 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_series.py
+-rw-r--r--   0        0        0      734 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_series_type.py
+-rw-r--r--   0        0        0     2648 2023-05-18 12:27:13.793870 mokkari-2.4.0/tests/test_teams.py
+-rw-r--r--   0        0        0   544768 2023-05-18 12:27:13.797870 mokkari-2.4.0/tests/testing_mock.sqlite
+-rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 mokkari-2.4.0/PKG-INFO
```

### Comparing `mokkari-2.3.3/LICENSE` & `mokkari-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/README.rst` & `mokkari-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/mokkari/__init__.py` & `mokkari-2.4.0/mokkari/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Project entry file."""
 
 # Keep this at beginning of file to prevent circular import with session
-__version__ = "2.3.3"
+__version__ = "2.4.0"
 
 from typing import Optional
 
 from mokkari import exceptions, session, sqlite_cache
 
 
 def api(
```

### Comparing `mokkari-2.3.3/mokkari/arc.py` & `mokkari-2.4.0/mokkari/arc.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         **kwargs (Any): The keyword arguments is used for setting arc data from Metron.
 
     Attributes:
         id (int): The Metron identification number for the story arc.
         name (str): The name of the story arc.
         desc (str): The description of the story arc.
         image (url): The url for an image associated with the story arc.
+        cv_id (int): Comic Vine ID for the story arc.
         resource_url (url): The url for the resource.
         modified (datetime): The date/time the story arc was last changed.
     """
 
     def __init__(self, **kwargs):
         """Initialize a new Arc."""
         for k, v in kwargs.items():
@@ -41,20 +42,25 @@
     .. versionchanged:: 1.0.0
 
         - Added ``modified`` field
 
     .. versionchanged:: 2.3.3
 
         - Added ``resource_url`` field.
+
+    .. versionadded:: 2.4.0
+
+        - Added ``cv_id`` field.
     """
 
     id = fields.Int()
     name = fields.Str()
     desc = fields.Str()
     image = fields.Url(allow_none=True)
+    cv_id = fields.Int(allow_none=True)
     resource_url = fields.URL()
     modified = fields.DateTime()
 
     class Meta:
         """Any unknown fields will be excluded."""
 
         unknown = EXCLUDE
```

### Comparing `mokkari-2.3.3/mokkari/character.py` & `mokkari-2.4.0/mokkari/character.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         id (int): The Metron identification number for the character.
         name (str): The name of the character.
         alias (list[str]): List of aliases the character may have.
         desc (str): The description of the character.
         image (url): The url for an image associated with the character.
         creators (list[Creator]): A list of creators for the character.
         teams (list[Team]): A list of teams the character is a member of.
+        cv_id (int): Comic Vine ID for the Character.
         resource_url (url): The url for the resource.
         modified (datetime): The date/time the character was last changed.
     """
 
     def __init__(self, **kwargs):
         """Initialize a new Character."""
         for k, v in kwargs.items():
@@ -47,23 +48,28 @@
 
     .. versionchanged:: 2.0.2
         - Removed ``wikipedia`` field
 
     .. versionchanged:: 2.3.3
 
         - Added ``resource_url`` field.
+
+    .. versionadded:: 2.4.0
+
+        - Added ``cv_id`` field.
     """
 
     id = fields.Int()
     name = fields.Str()
     alias = fields.List(fields.Str)
     desc = fields.Str()
     image = fields.Url(allow_none=True)
     creators = fields.Nested(creator.CreatorSchema, many=True)
     teams = fields.Nested(team.TeamSchema, many=True)
+    cv_id = fields.Int(allow_none=True)
     resource_url = fields.URL()
     modified = fields.DateTime()
 
     class Meta:
         """Any unknown fields will be excluded."""
 
         unknown = EXCLUDE
```

### Comparing `mokkari-2.3.3/mokkari/creator.py` & `mokkari-2.4.0/mokkari/creator.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     Attributes:
         id (int): The Metron identification number for the creator.
         name (str): The name of the creator.
         birth (date): The date of birth for the creator.
         death (date): The date of death for the creator.
         desc (str): The description of the creator.
         image (url): The url for an image associated with the creator.
+        cv_id (int): Comic Vine ID for the Creator.
         resource_url (url): The url for the resource.
         modified (datetime): The date/time the creator was last changed.
     """
 
     def __init__(self, **kwargs):
         """Initialize a new Creator."""
         for k, v in kwargs.items():
@@ -47,22 +48,27 @@
     .. versionchanged:: 2.0.2
 
         - Removed ``wikipedia`` field
 
     .. versionchanged:: 2.3.3
 
         - Added ``resource_url`` field.
+
+    .. versionadded:: 2.4.0
+
+        - Added ``cv_id`` field.
     """
 
     id = fields.Int()
     name = fields.Str()
     birth = fields.Date(allow_none=True)
     death = fields.Date(allow_none=True)
     desc = fields.Str()
     image = fields.Url(allow_none=True)
+    cv_id = fields.Int(allow_none=True)
     resource_url = fields.URL()
     modified = fields.DateTime()
 
     class Meta:
         """Any unknown fields will be excluded."""
 
         unknown = EXCLUDE
```

### Comparing `mokkari-2.3.3/mokkari/exceptions.py` & `mokkari-2.4.0/mokkari/exceptions.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/mokkari/genre.py` & `mokkari-2.4.0/mokkari/genre.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/mokkari/issue.py` & `mokkari-2.4.0/mokkari/issue.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,15 @@
         arcs (list[:obj:`Arc`]): A list of story arcs.
         credits (list[:obj:`Credit`]): A list of creator credits for the issue.
         characters (list[:obj:`Character`]): A list of characters who appear in the issue.
         teams (list[:obj:`Team`]): A list of teams who appear in the issue.
         reprints (list[:obj:`Reprint`]): A list of reprinted issue contained in the issue.
         issue_name (str): The name used to identified the issue.
         variants (list[:obj:`Variant`]): A list of variant covers for the issue.
+        cv_id (int): Comic Vine ID for the issue.
         resource_url (url): The url for the resource.
         modified (datetime): The date/time the issue was last changed.
     """
 
     def __init__(self, **kwargs):
         """Initialize a new Issue."""
         for k, v in kwargs.items():
@@ -223,14 +224,18 @@
     .. versionchanged:: 2.3.2
 
         - Added ``rating`` field.
 
     .. versionchanged:: 2.3.3
 
         - Added ``resource_url`` field.
+
+    .. versionadded:: 2.4.0
+
+        - Added ``cv_id`` field.
     """
 
     id = fields.Int()
     publisher = fields.Nested(PublisherSchema)
     series = fields.Nested(SeriesSchema)
     number = fields.Str()
     collection_title = fields.Str(allow_none=True, data_key="title")
@@ -247,14 +252,15 @@
     arcs = fields.Nested(ArcSchema, many=True)
     credits = fields.Nested(CreditsSchema, many=True)
     characters = fields.Nested(CharacterSchema, many=True)
     teams = fields.Nested(TeamSchema, many=True)
     reprints = fields.Nested(ReprintSchema, many=True)
     issue_name = fields.Str(data_key="issue")
     variants = fields.Nested(VariantSchema, many=True)
+    cv_id = fields.Int(allow_none=True)
     resource_url = fields.URL()
     modified = fields.DateTime()
 
     class Meta:
         """Any unknown fields will be excluded."""
 
         unknown = EXCLUDE
```

### Comparing `mokkari-2.3.3/mokkari/publisher.py` & `mokkari-2.4.0/mokkari/publisher.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
     Attributes:
         id (int): The Metron identification number for the publisher.
         name (str): The name of the publisher.
         founded (int): The year the publisher was founded.
         desc (str): A summary description about the publisher.
         image (url): The url for an image associated with the publisher.
+        cv_id (int): Comic Vine ID for the publisher.
         resource_url (url): The url for the resource.
         modified (datetime): The date/time the publisher was last changed.
     """
 
     def __init__(self, **kwargs):
         """Initialize a new Publisher."""
         for k, v in kwargs.items():
@@ -46,21 +47,26 @@
     .. versionchanged:: 2.0.2
 
         - Removed ``wikipedia`` field
 
     .. versionchanged:: 2.3.3
 
         - Added ``resource_url`` field.
+
+    .. versionadded:: 2.4.0
+
+        - Added ``cv_id`` field.
     """
 
     id = fields.Int()
     name = fields.Str()
     founded = fields.Int()
     desc = fields.Str()
     image = fields.Url(allow_none=True)
+    cv_id = fields.Int(allow_none=True)
     resource_url = fields.URL()
     modified = fields.DateTime()
 
     class Meta:
         """Any unknown fields will be excluded."""
 
         unknown = EXCLUDE
```

### Comparing `mokkari-2.3.3/mokkari/rating.py` & `mokkari-2.4.0/mokkari/rating.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/mokkari/reprint.py` & `mokkari-2.4.0/mokkari/reprint.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/mokkari/series.py` & `mokkari-2.4.0/mokkari/series.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         year_end (int, optional): The cover year in which the series ended.
         desc (str): A summary description of the series.
         issue_count (int): The number of issues the series contains.
         display_name (str): The display name for the series.
         genres (list[Genre]): A list of genres for the series.
         associated (list[AssociatedSeries]): A list of of series associated with the
         primary series.
+        cv_id (int): Comic Vine ID for the series.
         resource_url (url): The url for the resource.
         modified (datetime): The date/time the series was last changed.
     """
 
     def __init__(self, **kwargs):
         """Initialize a new Series."""
         for k, v in kwargs.items():
@@ -188,14 +189,18 @@
 
     .. versionchanged:: 2.1.1
         Added ``genres`` fields
 
     .. versionchanged:: 2.3.3
 
         - Added ``resource_url`` field.
+
+    .. versionadded:: 2.4.0
+
+        - Added ``cv_id`` field.
     """
 
     id = fields.Int()
     name = fields.Str()
     sort_name = fields.Str()
     volume = fields.Int()
     series_type = fields.Nested(SeriesTypeSchema)
@@ -204,14 +209,15 @@
     year_end = fields.Int(allow_none=True)
     desc = fields.Str()
     issue_count = fields.Int()
     image = fields.Url(allow_none=True)
     display_name = fields.Str(data_key="series")
     genres = fields.Nested(GenreSchema, many=True)
     associated = fields.Nested(AssociatedSeriesSchema, many=True)
+    cv_id = fields.Int(allow_none=True)
     resource_url = fields.URL()
     modified = fields.DateTime()
 
     class Meta:
         """Any unknown fields will be excluded."""
 
         unknown = EXCLUDE
```

### Comparing `mokkari-2.3.3/mokkari/session.py` & `mokkari-2.4.0/mokkari/session.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/mokkari/sqlite_cache.py` & `mokkari-2.4.0/mokkari/sqlite_cache.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/mokkari/team.py` & `mokkari-2.4.0/mokkari/team.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
     Attributes:
         id (int): The Metron identification number for the team.
         name (str): The name of the team.
         desc (str): The description of the team.
         image (url): The url for an image associated with the team.
         creators (list[:obj:`Creator`]): A list of creators for the team.
+        cv_id (int): Comic Vine ID for the team.
         resource_url (url): The url for the resource.
         modified (datetime): The date/time the team was last changed.
     """
 
     def __init__(self, **kwargs):
         """Initialize a new Team."""
         for k, v in kwargs.items():
@@ -45,21 +46,26 @@
 
     .. versionchanged:: 2.0.2
         - Removed ``wikipedia`` field
 
     .. versionchanged:: 2.3.3
 
         - Added ``resource_url`` field.
+
+    .. versionadded:: 2.4.0
+
+        - Added ``cv_id`` field.
     """
 
     id = fields.Int()
     name = fields.Str()
     desc = fields.Str()
     image = fields.Url(allow_none=True)
     creators = fields.Nested(creator.CreatorSchema, many=True)
+    cv_id = fields.Int(allow_none=True)
     resource_url = fields.URL()
     modified = fields.DateTime()
 
     class Meta:
         """Any unknown fields will be excluded."""
 
         unknown = EXCLUDE
```

### Comparing `mokkari-2.3.3/mokkari/variant.py` & `mokkari-2.4.0/mokkari/variant.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/pyproject.toml` & `mokkari-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mokkari"
-version = "2.3.3"
+version = "2.4.0"
 description = "Python wrapper for Metron API"
 authors = ["Brian Pepple <bdpepple@gmail.com>"]
 license = "GPL-3.0-or-later"
 maintainers = ["Brian Pepple <bdpepple@gmail.com>"]
 readme = "README.rst"
 packages = [
 	{ include = "mokkari" },
```

### Comparing `mokkari-2.3.3/tests/README.md` & `mokkari-2.4.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/conftest.py` & `mokkari-2.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/test_arcs.py` & `mokkari-2.4.0/tests/test_arcs.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/test_cache.py` & `mokkari-2.4.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/test_characters.py` & `mokkari-2.4.0/tests/test_characters.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/test_creator.py` & `mokkari-2.4.0/tests/test_creator.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/test_init.py` & `mokkari-2.4.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/test_issues.py` & `mokkari-2.4.0/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/test_publishers.py` & `mokkari-2.4.0/tests/test_publishers.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/test_role.py` & `mokkari-2.4.0/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/test_series.py` & `mokkari-2.4.0/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/test_series_type.py` & `mokkari-2.4.0/tests/test_series_type.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/test_teams.py` & `mokkari-2.4.0/tests/test_teams.py`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/tests/testing_mock.sqlite` & `mokkari-2.4.0/tests/testing_mock.sqlite`

 * *Files identical despite different names*

### Comparing `mokkari-2.3.3/PKG-INFO` & `mokkari-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mokkari
-Version: 2.3.3
+Version: 2.4.0
 Summary: Python wrapper for Metron API
 License: GPL-3.0-or-later
 Keywords: comics,comic,metadata
 Author: Brian Pepple
 Author-email: bdpepple@gmail.com
 Maintainer: Brian Pepple
 Maintainer-email: bdpepple@gmail.com
@@ -28,16 +28,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Provides-Extra: docs
 Requires-Dist: marshmallow (>=3.13.0,<4.0.0)
 Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
-Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0); extra == "docs"
-Requires-Dist: sphinxcontrib-napoleon (>=0.7,<0.8); extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0) ; extra == "docs"
+Requires-Dist: sphinxcontrib-napoleon (>=0.7,<0.8) ; extra == "docs"
 Project-URL: Bug Tracker, https://github.com/Metron-Project/mokkari/issues
 Project-URL: Homepage, https://github.com/Metron-Project/mokkari
 Description-Content-Type: text/x-rst
 
 =======
 Mokkari
 =======
```

