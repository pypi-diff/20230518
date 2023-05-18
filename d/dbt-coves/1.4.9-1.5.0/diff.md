# Comparing `tmp/dbt_coves-1.4.9.tar.gz` & `tmp/dbt_coves-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_coves-1.4.9.tar", max compression
+gzip compressed data, was "dbt_coves-1.5.0.tar", max compression
```

## Comparing `dbt_coves-1.4.9.tar` & `dbt_coves-1.5.0.tar`

### file list

```diff
@@ -1,51 +1,58 @@
--rw-r--r--   0        0        0    11357 2023-05-02 12:30:43.101203 dbt_coves-1.4.9/LICENSE
--rw-r--r--   0        0        0    21746 2023-05-02 12:30:43.101203 dbt_coves-1.4.9/README.md
--rw-r--r--   0        0        0       22 2023-05-02 12:31:38.381234 dbt_coves-1.4.9/dbt_coves/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 12:30:43.101203 dbt_coves-1.4.9/dbt_coves/config/__init__.py
--rw-r--r--   0        0        0     9689 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/config/config.py
--rw-r--r--   0        0        0        0 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/core/__init__.py
--rw-r--r--   0        0        0      650 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/core/exceptions.py
--rw-r--r--   0        0        0     4914 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/core/main.py
--rw-r--r--   0        0        0        0 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/__init__.py
--rw-r--r--   0        0        0     2956 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/base.py
--rw-r--r--   0        0        0     4994 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/dbt/main.py
--rw-r--r--   0        0        0        0 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/extract/__init__.py
--rw-r--r--   0        0        0    12100 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/extract/airbyte.py
--rw-r--r--   0        0        0      475 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/extract/base.py
--rw-r--r--   0        0        0     4512 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/extract/fivetran.py
--rw-r--r--   0        0        0      963 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/extract/main.py
--rw-r--r--   0        0        0        0 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/generate/__init__.py
--rw-r--r--   0        0        0    18472 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/generate/base.py
--rw-r--r--   0        0        0     1520 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/generate/main.py
--rw-r--r--   0        0        0    10562 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/generate/metadata.py
--rw-r--r--   0        0        0     8880 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/generate/properties.py
--rw-r--r--   0        0        0    13956 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/generate/sources.py
--rw-r--r--   0        0        0     2653 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/generate/templates.py
--rw-r--r--   0        0        0        0 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/load/__init__.py
--rw-r--r--   0        0        0    22617 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/load/airbyte.py
--rw-r--r--   0        0        0     2153 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/load/base.py
--rw-r--r--   0        0        0    17204 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/load/fivetran.py
--rw-r--r--   0        0        0      946 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/load/main.py
--rw-r--r--   0        0        0        0 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/setup/__init__.py
--rw-r--r--   0        0        0     1744 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/setup/all.py
--rw-r--r--   0        0        0     4215 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/setup/dbt.py
--rw-r--r--   0        0        0     6689 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/setup/git.py
--rw-r--r--   0        0        0     1183 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/setup/main.py
--rw-r--r--   0        0        0    10142 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/setup/ssh.py
--rw-r--r--   0        0        0      685 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/tasks/setup/utils.py
--rw-r--r--   0        0        0      255 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/templates/model_props.yml
--rw-r--r--   0        0        0      214 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/templates/source_props.yml
--rw-r--r--   0        0        0     1201 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/templates/staging_model.sql
--rw-r--r--   0        0        0      495 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/templates/staging_model_props.yml
--rw-r--r--   0        0        0        0 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/ui/__init__.py
--rw-r--r--   0        0        0     1202 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/ui/traceback.py
--rw-r--r--   0        0        0        0 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/utils/__init__.py
--rw-r--r--   0        0        0     4608 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/utils/airbyte_api.py
--rw-r--r--   0        0        0    12118 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/utils/api_caller.py
--rw-r--r--   0        0        0    13863 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/utils/flags.py
--rw-r--r--   0        0        0     1132 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/utils/jinja.py
--rw-r--r--   0        0        0      785 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/utils/log.py
--rw-r--r--   0        0        0      791 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/utils/shell.py
--rw-r--r--   0        0        0     1010 2023-05-02 12:30:43.105203 dbt_coves-1.4.9/dbt_coves/utils/yaml.py
--rw-r--r--   0        0        0     3520 2023-05-02 12:31:38.381234 dbt_coves-1.4.9/pyproject.toml
--rw-r--r--   0        0        0    23729 1970-01-01 00:00:00.000000 dbt_coves-1.4.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-11-12 20:16:42.866709 dbt_coves-1.5.0/LICENSE
+-rw-r--r--   0        0        0    21746 2023-05-02 13:59:26.100559 dbt_coves-1.5.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-18 12:04:27.911193 dbt_coves-1.5.0/dbt_coves/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-12 20:16:42.867324 dbt_coves-1.5.0/dbt_coves/config/__init__.py
+-rw-r--r--   0        0        0     9689 2023-04-25 20:50:24.122865 dbt_coves-1.5.0/dbt_coves/config/config.py
+-rw-r--r--   0        0        0        0 2022-11-12 20:16:42.867500 dbt_coves-1.5.0/dbt_coves/core/__init__.py
+-rw-r--r--   0        0        0      650 2022-11-12 20:16:42.867579 dbt_coves-1.5.0/dbt_coves/core/exceptions.py
+-rw-r--r--   0        0        0     7398 2023-05-18 12:03:26.474660 dbt_coves-1.5.0/dbt_coves/core/main.py
+-rw-r--r--   0        0        0        0 2022-11-12 20:16:42.867724 dbt_coves-1.5.0/dbt_coves/tasks/__init__.py
+-rw-r--r--   0        0        0     3008 2023-05-18 12:03:26.475205 dbt_coves-1.5.0/dbt_coves/tasks/base.py
+-rw-r--r--   0        0        0     4994 2023-05-02 13:59:26.103829 dbt_coves-1.5.0/dbt_coves/tasks/dbt/main.py
+-rw-r--r--   0        0        0        0 2022-11-12 20:16:42.867965 dbt_coves-1.5.0/dbt_coves/tasks/extract/__init__.py
+-rw-r--r--   0        0        0    12303 2023-05-15 17:37:04.477439 dbt_coves-1.5.0/dbt_coves/tasks/extract/airbyte.py
+-rw-r--r--   0        0        0      475 2023-03-23 11:02:15.327281 dbt_coves-1.5.0/dbt_coves/tasks/extract/base.py
+-rw-r--r--   0        0        0     4512 2023-03-23 11:02:15.327681 dbt_coves-1.5.0/dbt_coves/tasks/extract/fivetran.py
+-rw-r--r--   0        0        0      963 2023-03-23 11:02:15.328185 dbt_coves-1.5.0/dbt_coves/tasks/extract/main.py
+-rw-r--r--   0        0        0        0 2022-11-12 20:16:42.868244 dbt_coves-1.5.0/dbt_coves/tasks/generate/__init__.py
+-rw-r--r--   0        0        0    18472 2023-05-16 15:07:22.657626 dbt_coves-1.5.0/dbt_coves/tasks/generate/base.py
+-rw-r--r--   0        0        0     1520 2023-05-16 11:48:11.708991 dbt_coves-1.5.0/dbt_coves/tasks/generate/main.py
+-rw-r--r--   0        0        0    10562 2023-03-23 11:02:15.329609 dbt_coves-1.5.0/dbt_coves/tasks/generate/metadata.py
+-rw-r--r--   0        0        0     8880 2023-03-30 13:55:57.611879 dbt_coves-1.5.0/dbt_coves/tasks/generate/properties.py
+-rw-r--r--   0        0        0    13955 2023-05-18 12:03:26.475513 dbt_coves-1.5.0/dbt_coves/tasks/generate/sources.py
+-rw-r--r--   0        0        0     2653 2023-03-23 11:02:15.330706 dbt_coves-1.5.0/dbt_coves/tasks/generate/templates.py
+-rw-r--r--   0        0        0        0 2022-11-12 20:16:42.868885 dbt_coves-1.5.0/dbt_coves/tasks/load/__init__.py
+-rw-r--r--   0        0        0    25682 2023-05-15 17:37:04.477626 dbt_coves-1.5.0/dbt_coves/tasks/load/airbyte.py
+-rw-r--r--   0        0        0     2259 2023-05-05 11:02:21.127260 dbt_coves-1.5.0/dbt_coves/tasks/load/base.py
+-rw-r--r--   0        0        0    18390 2023-05-15 17:37:04.478119 dbt_coves-1.5.0/dbt_coves/tasks/load/fivetran.py
+-rw-r--r--   0        0        0      946 2023-03-23 11:02:15.332754 dbt_coves-1.5.0/dbt_coves/tasks/load/main.py
+-rw-r--r--   0        0        0        0 2022-11-12 20:16:42.869156 dbt_coves-1.5.0/dbt_coves/tasks/setup/__init__.py
+-rw-r--r--   0        0        0     1744 2023-03-23 11:02:15.333279 dbt_coves-1.5.0/dbt_coves/tasks/setup/all.py
+-rw-r--r--   0        0        0     4294 2023-05-18 12:03:26.475924 dbt_coves-1.5.0/dbt_coves/tasks/setup/dbt.py
+-rw-r--r--   0        0        0     6689 2023-03-23 11:02:15.334243 dbt_coves-1.5.0/dbt_coves/tasks/setup/git.py
+-rw-r--r--   0        0        0     1329 2023-05-08 19:28:33.430793 dbt_coves-1.5.0/dbt_coves/tasks/setup/main.py
+-rw-r--r--   0        0        0     1615 2023-05-08 19:28:33.431036 dbt_coves-1.5.0/dbt_coves/tasks/setup/pre_commit.py
+-rw-r--r--   0        0        0    10142 2023-03-23 11:02:15.335712 dbt_coves-1.5.0/dbt_coves/tasks/setup/ssh.py
+-rw-r--r--   0        0        0      845 2023-05-08 19:28:33.431214 dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/copier.yml
+-rw-r--r--   0        0        0     2110 2023-05-08 19:28:33.431340 dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja
+-rw-r--r--   0        0        0       75 2023-05-08 19:28:33.431660 dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluffignore{% endif %}
+-rw-r--r--   0        0        0     2743 2023-05-08 19:28:33.431853 dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja
+-rw-r--r--   0        0        0      668 2023-05-08 19:28:33.432263 dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}
+-rw-r--r--   0        0        0      102 2023-05-08 19:28:33.432386 dbt_coves-1.5.0/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{{ _copier_conf.answers_file }}-precommit.yaml.jinja
+-rw-r--r--   0        0        0     1371 2023-05-08 19:28:33.432813 dbt_coves-1.5.0/dbt_coves/tasks/setup/utils.py
+-rw-r--r--   0        0        0      255 2023-03-23 11:02:15.337399 dbt_coves-1.5.0/dbt_coves/templates/model_props.yml
+-rw-r--r--   0        0        0      214 2023-03-23 11:02:15.337740 dbt_coves-1.5.0/dbt_coves/templates/source_props.yml
+-rw-r--r--   0        0        0     1201 2023-03-23 11:02:15.338064 dbt_coves-1.5.0/dbt_coves/templates/staging_model.sql
+-rw-r--r--   0        0        0      495 2023-03-23 11:02:15.338292 dbt_coves-1.5.0/dbt_coves/templates/staging_model_props.yml
+-rw-r--r--   0        0        0        0 2022-11-12 20:16:42.870019 dbt_coves-1.5.0/dbt_coves/ui/__init__.py
+-rw-r--r--   0        0        0     1202 2022-11-12 20:16:42.870090 dbt_coves-1.5.0/dbt_coves/ui/traceback.py
+-rw-r--r--   0        0        0        0 2022-11-12 20:16:42.870149 dbt_coves-1.5.0/dbt_coves/utils/__init__.py
+-rw-r--r--   0        0        0    11270 2023-05-15 17:37:04.478455 dbt_coves-1.5.0/dbt_coves/utils/api_caller.py
+-rw-r--r--   0        0        0    14725 2023-05-18 12:03:26.476318 dbt_coves-1.5.0/dbt_coves/utils/flags.py
+-rw-r--r--   0        0        0     1132 2023-03-23 11:02:15.340252 dbt_coves-1.5.0/dbt_coves/utils/jinja.py
+-rw-r--r--   0        0        0      785 2023-03-23 11:02:15.340489 dbt_coves-1.5.0/dbt_coves/utils/log.py
+-rw-r--r--   0        0        0      791 2023-03-23 11:02:15.341162 dbt_coves-1.5.0/dbt_coves/utils/shell.py
+-rw-r--r--   0        0        0     1010 2023-03-23 11:02:15.341786 dbt_coves-1.5.0/dbt_coves/utils/yaml.py
+-rw-r--r--   0        0        0     3573 2023-05-18 12:04:23.598551 dbt_coves-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    24184 1970-01-01 00:00:00.000000 dbt_coves-1.5.0/setup.py
+-rw-r--r--   0        0        0    23804 1970-01-01 00:00:00.000000 dbt_coves-1.5.0/PKG-INFO
```

### Comparing `dbt_coves-1.4.9/LICENSE` & `dbt_coves-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/README.md` & `dbt_coves-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/config/config.py` & `dbt_coves-1.5.0/dbt_coves/config/config.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/core/exceptions.py` & `dbt_coves-1.5.0/dbt_coves/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/base.py` & `dbt_coves-1.5.0/dbt_coves/tasks/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,15 @@
-from dbt.adapters.factory import get_adapter
+from dbt.adapters.factory import get_adapter, register_adapter
+
+try:
+    from dbt.flags import set_flags
+
+    SET_FLAGS = True
+except ImportError:
+    SET_FLAGS = False
 from dbt.task.base import ConfiguredTask
 
 from dbt_coves.core.exceptions import MissingCommand
 
 
 class BaseTask:
     """
@@ -35,20 +42,26 @@
     """
 
     needs_config = True
     needs_dbt_project = True
 
     def __init__(self, args, config):
         super().__init__(args, config)
-        self.adapter = get_adapter(self.config)
+        try:
+            self.adapter = get_adapter(self.config)
+        except KeyError:
+            register_adapter(self.config)
+            self.adapter = get_adapter(self.config)
         self.coves_config = None
         self.coves_flags = None
 
     @classmethod
     def from_args(cls, args):
+        if SET_FLAGS:
+            set_flags(args)
         config = cls.ConfigType.from_args(args)
         try:
             return cls(args, config)
         # class cannot be instantiated with abstract methods.
         # that means a subcommand is missing.
         except TypeError:
             raise MissingCommand(cls.arg_parser)
@@ -71,19 +84,14 @@
 
     def __init__(self, args, config):
         super().__init__(args, config)
         self.coves_config = config
         self.coves_flags = None
 
     @classmethod
-    def from_args(cls, args):
-        config = cls.ConfigType.from_args(args)
-        return cls(args, config)
-
-    @classmethod
     def get_instance(cls, flags, coves_config):
         instance = cls(flags.args, coves_config)
         instance.coves_config = coves_config
         instance.coves_flags = flags
         return instance
 
     @classmethod
@@ -101,17 +109,12 @@
 
     def __init__(self, args, config):
         super().__init__(args, config)
         self.coves_config = config
         self.coves_flags = None
 
     @classmethod
-    def from_args(cls, args):
-        config = cls.ConfigType.from_args(args)
-        return cls(args, config)
-
-    @classmethod
     def get_instance(cls, flags, coves_config):
         instance = cls(flags.args, coves_config)
         instance.coves_config = coves_config
         instance.coves_flags = flags
         return instance
```

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/dbt/main.py` & `dbt_coves-1.5.0/dbt_coves/tasks/dbt/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/extract/airbyte.py` & `dbt_coves-1.5.0/dbt_coves/tasks/extract/airbyte.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dbt_coves.utils.api_caller import AirbyteApiCaller
 
 from .base import BaseExtractTask
 
 # from dbt_coves.utils import airbyte_api
 
 console = Console()
-NON_EXTRACT_KEYS = ["icon"]
+NON_EXTRACT_KEYS = ["icon", "breakingChange"]
 
 
 class AirbyteExtractorException(Exception):
     pass
 
 
 class ExtractAirbyteTask(BaseExtractTask):
@@ -118,15 +118,17 @@
 
     def _get_airbyte_destination_definition_from_id(self, definition_id):
         req_body = {
             "destinationDefinitionId": definition_id,
             "workspaceId": self.airbyte_api.airbyte_workspace_id,
         }
         return self.airbyte_api.api_call(
-            self.airbyte_api.airbyte_endpoint_get_destination_definition,
+            self.airbyte_api.api_endpoints["GET_OBJECTS"].format(
+                obj="destination_definition_specifications"
+            ),
             req_body,
         )
 
     def _get_airbyte_destination_from_id(self, destinationId):
         """
         Get the complete Destination object from it's ID
         """
@@ -166,15 +168,18 @@
 
     def _get_airbyte_source_definition_from_id(self, definition_id):
         req_body = {
             "sourceDefinitionId": definition_id,
             "workspaceId": self.airbyte_api.airbyte_workspace_id,
         }
         return self.airbyte_api.api_call(
-            self.airbyte_api.airbyte_endpoint_get_source_definition, req_body
+            self.airbyte_api.api_endpoints["GET_OBJECTS"].format(
+                obj="source_definition_specifications"
+            ),
+            req_body,
         )
 
     def _hide_configuration_secret_fields(self, connection_configuration, airbyte_secret_fields):
         for k, v in connection_configuration.items():
             if isinstance(v, dict):
                 self._hide_configuration_secret_fields(v, airbyte_secret_fields)
             elif k in airbyte_secret_fields:
@@ -239,14 +244,15 @@
         return json_object
 
     def _save_json(self, path, json_object):
         json_object = self._remove_unnecessary_fields(json_object)
         try:
             with open(path, "w") as json_file:
                 json.dump(json_object, json_file, indent=4)
+                json_file.write("\n")
         except OSError as e:
             raise AirbyteExtractorException(f"Couldn't write {path}: {e}")
 
     def _save_json_connection(self, connection):
         connection = copy(connection)
         connection.pop("connectionId")
```

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/extract/fivetran.py` & `dbt_coves-1.5.0/dbt_coves/tasks/extract/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/extract/main.py` & `dbt_coves-1.5.0/dbt_coves/tasks/extract/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/generate/base.py` & `dbt_coves-1.5.0/dbt_coves/tasks/generate/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/generate/main.py` & `dbt_coves-1.5.0/dbt_coves/tasks/generate/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/generate/metadata.py` & `dbt_coves-1.5.0/dbt_coves/tasks/generate/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/generate/properties.py` & `dbt_coves-1.5.0/dbt_coves/tasks/generate/properties.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/generate/sources.py` & `dbt_coves-1.5.0/dbt_coves/tasks/generate/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,14 @@
         self.get_metadata()
 
         # initiate connection
         with self.adapter.connection_named("master"):
             filtered_schemas = self.get_schemas()
             if not filtered_schemas:
                 return 0
-
             relations = self.get_relations(filtered_schemas)
             if relations:
                 selected_relations = self.select_relations(relations)
                 if selected_relations:
                     self.raise_duplicate_relations(selected_relations)
                     self.generate(selected_relations)
                 else:
```

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/generate/templates.py` & `dbt_coves-1.5.0/dbt_coves/tasks/generate/templates.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/load/airbyte.py` & `dbt_coves-1.5.0/dbt_coves/tasks/load/airbyte.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import json
 import os
 import pathlib
+from copy import copy
 from os import path
 
+import questionary
 from rich.console import Console
 from slugify import slugify
 
-from dbt_coves.utils.airbyte_api import AirbyteApiCaller, AirbyteApiCallerException
+from dbt_coves.utils.api_caller import AirbyteApiCaller, AirbyteApiCallerException
 
 from .base import BaseLoadTask
 
 console = Console()
 
 
 class AirbyteLoaderException(Exception):
@@ -100,15 +102,15 @@
                 f"Specified [b]load_destination[/b]: [u]{self.load_destination}[/u] does not exist"
             )
 
         self.connections_load_destination = os.path.abspath(path / "connections")
         self.destinations_load_destination = os.path.abspath(path / "destinations")
         self.sources_load_destination = os.path.abspath(path / "sources")
 
-        self.airbyte_api_caller = AirbyteApiCaller(self.airbyte_host, self.airbyte_port)
+        self.airbyte_api = AirbyteApiCaller(self.airbyte_host, self.airbyte_port)
 
         console.print(f"Loading DBT Sources into Airbyte from {os.path.abspath(path)}\n")
 
         # Load all exported
         extracted_sources = self.retrieve_all_jsons_from_path(self.sources_load_destination)
         # Create/update sources
         extracted_destinations = self.retrieve_all_jsons_from_path(
@@ -216,35 +218,30 @@
                     if not target_secret_data:
                         raise AirbyteLoaderException(
                             "Specified manager didn't provide secret information"
                             f"for[red]{secret_target_name}[/red]"
                         )
                     secret_data = target_secret_data["value"]
                 elif self.secrets_path:
-                    wildcard_keys = [
-                        str(k)
-                        for k, v in connection_configuration.items()
-                        if wildcard_pattern == str(v)
-                    ]
                     secret_target_name = slugify(exported_json_data["name"].lower())
                     # Get the secret file for that name
                     secret_file = os.path.join(
                         self.secrets_path,
                         directory,
                         secret_target_name + ".json",
                     )
 
                     if path.isfile(secret_file):
                         secret_data = json.load(open(secret_file))
                     else:
                         raise AirbyteLoaderException(
                             f"Secret file for {secret_target_name} not found\n"
-                            f"Please create secret for [bold red]{secret_target_name}[/bold red]"
-                            "with the following keys:"
-                            f"[bold red]{', '.join(k for k in wildcard_keys)}[/bold red]"
+                            f"Please create secret for [bold red]{secret_target_name}[/bold red] "
+                            "with the following keys: "
+                            f"[bold red]{', '.join(k for k in hidden_fields)}[/bold red]"
                         )
                 else:
                     raise AirbyteLoaderException(
                         "secrets_path or secrets_manager flag must be provided"
                     )
 
                 connection_configuration = self._update_connection_config_secret_fields(
@@ -252,227 +249,291 @@
                     wildcard_pattern,
                     secret_data,
                     secret_target_name,
                 )
             return exported_json_data
         except AirbyteLoaderException as e:
             raise AirbyteLoaderException(
-                f"There was an error loading secret data for {airbyte_object_type}"
+                f"There was an error loading secret data for {airbyte_object_type} "
                 f"[bold red]{exported_json_data['name']}[/bold red]: {e}"
             )
 
-    def _create_source(self, exported_json_data):
-        exported_json_data.pop("connectorVersion")
-        # Grab password from secret
-        exported_json_data = self._get_secrets(exported_json_data, "sources")
-        exported_json_data["workspaceId"] = self.airbyte_api_caller.airbyte_workspace_id
-        exported_json_data["sourceDefinitionId"] = self._get_source_definition_id_by_name(
-            exported_json_data.pop("sourceName")
-        )
-        try:
-            response = self.airbyte_api_caller.api_call(
-                self.airbyte_api_caller.airbyte_endpoint_create_sources,
-                exported_json_data,
+    def _update_source_or_destination(self, exported_data, object_type):
+        update = True
+        conn_status = self._test_update_connection(exported_data, object_type)
+        if conn_status.get("status", "").lower() != "succeeded":
+            console.print(
+                f"Connection test for {exported_data['name']} failed:\n {conn_status['message']}"
+            )
+            update = questionary.confirm("Would you like to continue updating it?").ask()
+        if update:
+            response = self.airbyte_api.api_call(
+                self.airbyte_api.api_endpoints["UPDATE_OBJECT"].format(obj=object_type),
+                exported_data,
             )
-            self.airbyte_api_caller.airbyte_sources_list.append(response)
-            self.loading_results["sources"]["created"].append(exported_json_data["name"])
-            return response["sourceId"]
 
-        except AirbyteApiCallerException as e:
-            raise AirbyteLoaderException(f"Could not create Airbyte Source: {e}")
+            self._add_update_result(object_type, exported_data["name"])
+            return response.get("sourceId", response.get("destinationId"))
 
-    def _update_source(self, exported_json_data, source_id):
-        exported_json_data["sourceId"] = source_id
-        exported_json_data.pop("sourceName")
-        exported_json_data.pop("connectorVersion")
+    def _create_source_or_destination(self, exported_data, object_type):
+        create = True
+        response = self.airbyte_api.api_call(
+            self.airbyte_api.api_endpoints["CREATE_OBJECT"].format(obj=object_type),
+            exported_data,
+        )
+        new_object_body = {}
+        if object_type == "sources":
+            new_object_body = {"sourceId": response["sourceId"]}
+        elif object_type == "destinations":
+            new_object_body = {"destinationId": response["destinationId"]}
 
-        exported_json_data = self._get_secrets(exported_json_data, "sources")
-        try:
-            response = self.airbyte_api_caller.api_call(
-                self.airbyte_api_caller.airbyte_endpoint_update_sources,
-                exported_json_data,
+        conn_status = self._test_created_object(new_object_body, object_type)
+        if conn_status.get("status", "").lower() != "succeeded":
+            console.print(
+                f"Connection test for {exported_data['name']} failed:\n {conn_status['message']}"
             )
-            self._add_update_result("sources", exported_json_data["name"])
-            return response["sourceId"]
-        except KeyError:
-            raise AirbyteLoaderException("Could not update source")
+            create = questionary.confirm("Would you like to continue creating it?").ask()
+        if create:
+            self.airbyte_api.airbyte_destinations_list.append(response)
+            self.loading_results[object_type]["created"].append(exported_data["name"])
+            return response[next(iter(new_object_body))]
+        else:
+            self.airbyte_api.api_call(
+                self.airbyte_api.api_endpoints["DELETE_OBJECT"].format(obj=object_type),
+                new_object_body,
+            )
+
+    def _create_source(self, exported_data):
+        exported_data.pop("connectorVersion")
+        exported_data = self._get_secrets(exported_data, "sources")
+        exported_data["workspaceId"] = self.airbyte_api.airbyte_workspace_id
+        exported_data["sourceDefinitionId"] = self._get_source_definition_id_by_name(
+            exported_data.pop("sourceName")
+        )
+        self._create_source_or_destination(exported_data, "sources")
+
+    def _test_update_connection(self, data, obj_type):
+        console.print(f"Testing update for [yellow]{data.get('name', 'object')}[/yellow]")
+        return self.airbyte_api.api_call(
+            self.airbyte_api.api_endpoints["TEST_UPDATE"].format(obj=obj_type), data, timeout=30
+        )
+
+    def _update_source(self, exported_data, source_id):
+        exported_data["sourceId"] = source_id
+        exported_data.pop("sourceName")
+        exported_data.pop("connectorVersion")
+
+        exported_data = self._get_secrets(exported_data, "sources")
+        self._update_source_or_destination(exported_data, "sources")
+
+    def _sources_are_equivalent(self, exported_source, current_source):
+        current_source_copy = copy(current_source)
+        exported_source_copy = copy(exported_source)
+        exported_source_copy.pop("connectorVersion")
+        current_source_copy.pop("icon")
+        current_source_copy.pop("sourceId")
+        current_source_copy.pop("sourceDefinitionId")
+        current_source_copy.pop("workspaceId")
+        return current_source_copy == exported_source_copy
 
     def _create_or_update_source(self, exported_json_data):
         """
         Decide whether creating or updating an existing source\
         (if it's name corresponds to an existing name in JSON exported configuration)
         """
         self._connector_versions_mismatch(exported_json_data, "source")
 
-        for src in self.airbyte_api_caller.airbyte_sources_list:
+        for src in self.airbyte_api.airbyte_sources_list:
             if exported_json_data["name"] == src["name"]:
-                return self._update_source(exported_json_data, src["sourceId"])
+                if self._sources_are_equivalent(exported_json_data, src):
+                    console.print(
+                        f"Source [green]{src['name']}[/green] already up to date. Skipping"
+                    )
+                    return
+                else:
+                    return self._update_source(exported_json_data, src["sourceId"])
 
         return self._create_source(exported_json_data)
 
     def _get_destination_definition_id_by_name(self, destination_type_name):
         """
         Get destination definition ID by it's name
         (File, Postgres, Snowflake, BigQuery, MariaDB, etc)
         """
-        for definition in self.airbyte_api_caller.destination_definitions:
+        for definition in self.airbyte_api.destination_definitions:
             if definition["name"] == destination_type_name:
                 return definition["destinationDefinitionId"]
         raise AirbyteLoaderException(
             f"There is no destination definition for {destination_type_name}."
             "Please review Airbyte's configuration"
         )
 
     def _get_destination_definition_by_name(self, destination_type_name):
         """
         Get destination definition ID by it's name
         (File, Postgres, Snowflake, BigQuery, MariaDB, etc)
         """
-        for definition in self.airbyte_api_caller.destination_definitions:
+        for definition in self.airbyte_api.destination_definitions:
             if definition["name"] == destination_type_name:
                 return definition
         raise AirbyteLoaderException(
             f"There is no destination definition for {destination_type_name}."
             "Please review Airbyte's configuration"
         )
 
     def _get_source_definition_id_by_name(self, source_type_name):
         """
         Get destination definition ID by it's name
         (File, Postgres, Snowflake, BigQuery, MariaDB, etc)
         """
-        for definition in self.airbyte_api_caller.source_definitions:
+        for definition in self.airbyte_api.source_definitions:
             if definition["name"] == source_type_name:
                 return definition["sourceDefinitionId"]
         raise AirbyteLoaderException(
             f"There is no source definition for {source_type_name}."
             "Please review Airbyte's configuration"
         )
 
     def _get_source_definition_by_name(self, source_type_name):
         """
         Get destination definition ID by it's name
         (File, Postgres, Snowflake, BigQuery, MariaDB, etc)
         """
-        for definition in self.airbyte_api_caller.source_definitions:
+        for definition in self.airbyte_api.source_definitions:
             if definition["name"] == source_type_name:
                 return definition
         raise AirbyteLoaderException(
             f"There is no source definition for {source_type_name}."
             "Please review Airbyte's configuration"
         )
 
+    def _test_created_object(self, test_body, obj_type):
+        console.print("Testing created object")
+        return self.airbyte_api.api_call(
+            self.airbyte_api.api_endpoints["TEST_CONNECTION"].format(obj=obj_type),
+            test_body,
+            timeout=30,
+        )
+
     def _create_destination(self, exported_data):
         exported_data.pop("connectorVersion")
         exported_data = self._get_secrets(exported_data, "destinations")
-        exported_data["workspaceId"] = self.airbyte_api_caller.airbyte_workspace_id
+        exported_data["workspaceId"] = self.airbyte_api.airbyte_workspace_id
         exported_data["destinationDefinitionId"] = self._get_destination_definition_id_by_name(
             exported_data.pop("destinationName")
         )
-        try:
-            response = self.airbyte_api_caller.api_call(
-                self.airbyte_api_caller.airbyte_endpoint_create_destinations,
-                exported_data,
-            )
-            self.airbyte_api_caller.airbyte_destinations_list.append(response)
-            self.loading_results["destinations"]["created"].append(exported_data["name"])
-            return response["destinationId"]
-        except AirbyteApiCallerException:
-            raise AirbyteApiCallerException("Could not create Airbyte destination")
+        self._create_source_or_destination(exported_data, "destinations")
 
-    def _update_destination(self, exported_json_data, destination_id):
-        exported_json_data.pop("destinationName")
-        exported_json_data["destinationId"] = destination_id
-        exported_json_data.pop("connectorVersion")
+    def _update_destination(self, exported_data, destination_id):
+        exported_data.pop("destinationName")
+        exported_data["destinationId"] = destination_id
+        exported_data.pop("connectorVersion")
 
-        exported_json_data = self._get_secrets(exported_json_data, "destinations")
+        exported_data = self._get_secrets(exported_data, "destinations")
+        self._update_source_or_destination(exported_data, "destinations")
 
-        try:
-            response = self.airbyte_api_caller.api_call(
-                self.airbyte_api_caller.airbyte_endpoint_update_destinations,
-                exported_json_data,
-            )
-            self._add_update_result("destinations", exported_json_data["name"])
-            return response["destinationId"]
-        except KeyError:
-            raise AirbyteLoaderException("Could not update destination")
+    def _destinations_are_equivalent(self, exported_destination, current_destination):
+        current_destination_copy = copy(current_destination)
+        exported_destination_copy = copy(exported_destination)
+        exported_destination_copy.pop("connectorVersion")
+        current_destination_copy.pop("destinationDefinitionId")
+        current_destination_copy.pop("destinationId")
+        current_destination_copy.pop("workspaceId")
+        current_destination_copy.pop("icon")
+        return current_destination_copy == exported_destination_copy
 
     def _create_or_update_destination(self, exported_json_data):
         """
         Decide whether creating or updating an existing destination
         (if it's name corresponds to an existing name in JSON exported configuration)
         """
         self._connector_versions_mismatch(exported_json_data, "destination")
 
-        for destination in self.airbyte_api_caller.airbyte_destinations_list:
+        for destination in self.airbyte_api.airbyte_destinations_list:
             if exported_json_data["name"] == destination["name"]:
-                return self._update_destination(exported_json_data, destination["destinationId"])
+                if self._destinations_are_equivalent(exported_json_data, destination):
+                    console.print(
+                        f"Destination [green]{destination['name']}[/green] already up to date. Skipping"
+                    )
+                    return
+                else:
+                    return self._update_destination(
+                        exported_json_data, destination["destinationId"]
+                    )
 
         return self._create_destination(exported_json_data)
 
     def _create_connection(self, exported_json_data, source_id, destination_id):
         exported_json_data["sourceId"] = source_id
         exported_json_data["destinationId"] = destination_id
         connection_name = (
             f"{exported_json_data['sourceName']}-{exported_json_data['destinationName']}"
         )
         exported_json_data.pop("sourceName")
         exported_json_data.pop("destinationName")
 
         try:
-            response = self.airbyte_api_caller.api_call(
-                self.airbyte_api_caller.airbyte_endpoint_create_connections,
+            response = self.airbyte_api.api_call(
+                self.airbyte_api.api_endpoints["CREATE_OBJECT"].format(obj="connections"),
                 exported_json_data,
             )
-            self.airbyte_api_caller.airbyte_connections_list.append(response)
-            if "connectionId" in response:
+            if response:
+                self.airbyte_api.airbyte_connections_list.append(response)
                 return connection_name
-            else:
-                raise AirbyteApiCallerException("Could not create Airbyte connection")
-        except AirbyteApiCallerException:
-            raise AirbyteApiCallerException("Could not create Airbyte connection")
+        except AirbyteApiCallerException as ex:
+            raise AirbyteApiCallerException(f"Could not create Airbyte connection: {ex}")
 
     def _delete_connection(self, connection_id):
         try:
             conn_delete_req_body = {"connectionId": connection_id}
-            self.airbyte_api_caller.api_call(
-                self.airbyte_api_caller.airbyte_endpoint_delete_connection,
+            self.airbyte_api.api_call(
+                self.airbyte_api.api_endpoints["DELETE_OBJECT"].format(obj="connections"),
                 conn_delete_req_body,
             )
         except AirbyteApiCallerException:
             raise AirbyteLoaderException("Could not delete Airbyte connection for re-creation")
 
     def _get_connection_id_by_table_name(self, table_name):
         """
         Given a table name, returns the corresponding airbyte connection
         """
-        for conn in self.airbyte_api_caller.airbyte_connections_list:
+        for conn in self.airbyte_api.airbyte_connections_list:
             for stream in conn["syncCatalog"]["streams"]:
                 if stream["stream"]["name"].lower() == table_name:
                     return conn["connectionId"]
         return False
 
     def _get_source_id_by_name(self, source_name):
-        for source in self.airbyte_api_caller.airbyte_sources_list:
+        for source in self.airbyte_api.airbyte_sources_list:
             if source["name"].lower() == source_name:
                 return source["sourceId"]
 
     def _get_destination_id_by_name(self, destination_name):
-        for destination in self.airbyte_api_caller.airbyte_destinations_list:
+        for destination in self.airbyte_api.airbyte_destinations_list:
             if destination["name"].lower() == destination_name:
                 return destination["destinationId"]
 
     def _get_connection_id_by_endpoints(self, source_id, destination_id):
-        for connection in self.airbyte_api_caller.airbyte_connections_list:
+        for connection in self.airbyte_api.airbyte_connections_list:
             if (
                 connection["sourceId"] == source_id
                 and connection["destinationId"] == destination_id
             ):
-                return connection["connectionId"]
-        pass
+                return connection
+
+    def _connection_already_updated(self, extracted_connection, current_connection):
+        extracted_copy = copy(extracted_connection)
+        current_copy = copy(current_connection)
+        extracted_copy.pop("sourceName")
+        extracted_copy.pop("destinationName")
+        current_copy.pop("connectionId")
+        current_copy.pop("sourceId")
+        current_copy.pop("destinationId")
+        current_copy.pop("breakingChange")
+        return extracted_copy == current_copy
 
     def _create_or_update_connection(self, connection_json):
         """
         Identify source_id and destination_id by their names
         Update or create connection
         """
         source_name = connection_json["sourceName"]
@@ -480,20 +541,27 @@
         source_id = self._get_source_id_by_name(source_name)
         destination_id = self._get_destination_id_by_name(destination_name)
         if not source_id or not destination_id:
             console.print(
                 f"No existent source-destination pair found for {connection_json['name']}"
             )
             return
-        connection_id = self._get_connection_id_by_endpoints(source_id, destination_id)
-        if connection_id:
+        connection = self._get_connection_id_by_endpoints(source_id, destination_id)
+        if connection:
             # Connection update
-            self._delete_connection(connection_id)
-            conn_name = self._create_connection(connection_json, source_id, destination_id)
-            self._add_update_result("connections", conn_name)
+            if self._connection_already_updated(connection_json, connection):
+                console.print(
+                    f"Connection [green]{connection['name']}[/green] already up to date. Skipping"
+                )
+                return
+            else:
+                connection_id = connection["connectionId"]
+                self._delete_connection(connection_id)
+                conn_name = self._create_connection(connection_json, source_id, destination_id)
+                self._add_update_result("connections", conn_name)
         else:
             # Connection creation
             conn_name = self._create_connection(connection_json, source_id, destination_id)
             self.loading_results["connections"]["created"].append(conn_name)
 
     def _add_update_result(self, obj_type, obj_name):
         if (obj_name not in self.loading_results[obj_type]["updated"]) and (
```

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/load/base.py` & `dbt_coves-1.5.0/dbt_coves/tasks/load/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,37 +26,40 @@
             filepath = Path(file)
             if filepath.stat().st_size > 0:
                 with open(filepath, "r") as json_file:
                     jsons.append(json.load(json_file))
         return jsons
 
     def _load_secret_data(self) -> dict:
-        # Contact the manager and retrieve Secrets
-        secrets_url = os.getenv("DBT_COVES_SECRETS_URL") or self.get_config_value("secrets_url")
-        secrets_token = os.getenv("DBT_COVES_SECRETS_TOKEN") or self.get_config_value(
-            "secrets_token"
-        )
-        if not (secrets_url and secrets_token):
-            raise LoadException(
-                "[b]secrets_url[/b] and [b]secrets_token[/b] must be provided"
-                "when using a Secrets Manager"
-            )
         payload = {}
-        if self.secrets_manager.lower() == "datacoves":
-            secrets_project = self.get_config_value("secrets_project")
-            if not secrets_project:
+        manager = self.secrets_manager.lower()
+        if manager == "datacoves":
+            # Contact the secrets manager and retrieve Secrets
+            secrets_url = os.getenv("DATACOVES__SECRETS_URL") or self.get_config_value(
+                "secrets_url"
+            )
+            secrets_token = os.getenv("DATACOVES__SECRETS_TOKEN") or self.get_config_value(
+                "secrets_token"
+            )
+            secrets_project = os.getenv("DATACOVES__SECRETS_PROJECT") or self.get_config_value(
+                "secrets_project"
+            )
+
+            if not (secrets_url and secrets_token and secrets_project):
                 raise LoadException(
-                    "[b]secrets_project[/b] must be provided when using 'datacoves'"
-                    "as your Secrets Manager "
+                    "[b]secrets_url[/b], [b]secrets_project[/b] and [b]secrets_token[/b] must "
+                    "be provided when using a Secrets Manager"
                 )
+
             secrets_url = f"{secrets_url}/api/v1/secrets/{secrets_project}"
             secrets_tags = self.get_config_value("secrets_tags")
             secrets_key = self.get_config_value("secrets_key")
             if secrets_tags:
                 payload["tags"] = set(secrets_tags)
             if secrets_key:
                 payload["key"] = secrets_key
+            headers = {"Authorization": f"token {secrets_token}"}
+            response = requests.get(secrets_url, headers=headers, verify=False, params=payload)
+            response.raise_for_status()
+            return response.json()
 
-        headers = {"Authorization": f"token {secrets_token}"}
-        response = requests.get(secrets_url, headers=headers, verify=False, params=payload)
-        response.raise_for_status()
-        return response.json()
+        raise LoadException(f"'{manager}' not recognized as a valid secrets manager.")
```

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/load/fivetran.py` & `dbt_coves-1.5.0/dbt_coves/tasks/load/fivetran.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,14 @@
 from dbt_coves.utils.api_caller import FivetranApiCaller
 from dbt_coves.utils.yaml import open_yaml
 
 from .base import BaseLoadTask
 
 console = Console()
 
-FIVETRAN_API_BASE_URL = "https://api.fivetran.com/v1"
-API_ENDPOINTS = {
-    "GROUP_DETAILS": FIVETRAN_API_BASE_URL + "/groups/{group}",
-    "GROUP_CREATE": FIVETRAN_API_BASE_URL + "/groups/",
-    "DESTINATION_LIST": FIVETRAN_API_BASE_URL + "/groups",
-    "DESTINATION_DETAILS": FIVETRAN_API_BASE_URL + "/destinations/{destination}",
-    "CONNECTOR_DESTINATION_LIST": FIVETRAN_API_BASE_URL + "/groups/{destination}/connectors",
-    "CONNECTOR_DETAILS": FIVETRAN_API_BASE_URL + "/connectors/{connector}",
-    "CONNECTOR_SCHEMAS": FIVETRAN_API_BASE_URL + "/connectors/{connector}/schemas",
-}
-FIVETRAN_SECRET_MASKING = "******"
-
 
 class FivetranLoaderException(Exception):
     pass
 
 
 class LoadFivetranTask(BaseLoadTask):
     @classmethod
@@ -72,19 +60,30 @@
         subparser.add_argument("--secrets-key", type=str, help="Secret credentials key")
         subparser.set_defaults(cls=cls, which="fivetran")
         return subparser
 
     def get_config_value(self, key):
         return self.coves_config.integrated["load"]["fivetran"][key]
 
+    def _print_load_results(self):
+        for obj_type, result_dict in self.load_results.items():
+            for activity, result in result_dict.items():
+                if len(result) > 0:
+                    console.print(
+                        f"{obj_type.capitalize()} {activity}: "
+                        f"[green]{', '.join(result)}[/green]"
+                    )
+
     def run(self) -> int:
         self.load_results = {
             "groups": {"created": set()},
             "destinations": {"created": set(), "updated": set()},
             "connectors": {"created": set(), "updated": set()},
+            "schemas": {"updated": set()},
+            "tables": {"updated": set()},
         }
 
         extract_destination = self.get_config_value("path")
         self.api_key = self.get_config_value("api_key")
         self.api_secret = self.get_config_value("api_secret")
         self.secrets_manager = self.get_config_value("secrets_manager")
         api_credentials_path = self.get_config_value("credentials")
@@ -123,14 +122,15 @@
         )
         if not self.extracted_destinations:
             raise FivetranLoaderException(
                 f"No Fivetran extracted data found on {self.extract_destination.absolute()}"
             )
 
         self.local_secrets = []
+        self.secret_manager_data = {}
 
         if secrets_path:
             self.secrets_path = Path(secrets_path)
             self.local_secrets = self.retrieve_all_jsons_from_path(
                 str(self.secrets_path.absolute())
             )
 
@@ -153,26 +153,16 @@
                     exported_group_id, exported_service_type
                 )
 
                 if target_group_id != exported_group_id:
                     self._update_group_id(fivetran_destination, target_group_id)
 
                 self._update_or_create_fivetran_destination(fivetran_destination, target_group_id)
+        self._print_load_results()
 
-        if (
-            len(self.load_results["destinations"]["updated"]) > 0
-            or len(self.load_results["destinations"]["created"]) > 0
-        ):
-            for obj_type, result_dict in self.load_results.items():
-                for activity, result in result_dict.items():
-                    if len(result) > 0:
-                        console.print(
-                            f"{obj_type.capitalize()} {activity}: "
-                            f"[green]{', '.join(result)}[/green]"
-                        )
         return 0
 
     def _connect_to_api_using_credentials_file(self, credentials_path):
         api_key = None
         api_secret = None
         credentials = open_yaml(credentials_path)
         if len(credentials) > 1:
@@ -185,55 +175,85 @@
         else:
             default_credentials = next(iter(credentials.values()))
             api_key = default_credentials["api_key"]
             api_secret = default_credentials["api_secret"]
 
         return FivetranApiCaller(api_key, api_secret)
 
+    def _fivetran_destination_updated(self, destination_details):
+        current_destination = self.fivetran_api._get_destination_details(destination_details["id"])
+        return destination_details == current_destination
+
     def _update_fivetran_destination(self, destination_details):
         destination_id = destination_details["id"]
         destination_name = self.fivetran_api.fivetran_groups[destination_details["group_id"]][
             "name"
         ]
-        updated_destination = self.fivetran_api.update_destination(
-            destination_id, destination_details
-        )
-        self.load_results["destinations"]["updated"].add(destination_name)
-        return updated_destination
+        if self._fivetran_destination_updated(destination_details):
+            console.print(
+                f"Destination [green]{destination_details['id']}[/green] already up to date. Skipping"
+            )
+        else:
+            destination_details["run_setup_tests"] = False
+            self.fivetran_api.update_destination(destination_id, destination_details)
+            self.load_results["destinations"]["updated"].add(destination_name)
 
     def _create_fivetran_destination(self, destination_details):
         created_destination = {}
         del destination_details["id"]
+        destination_details["run_setup_tests"] = False
         created_destination = self.fivetran_api.create_destination(destination_details)
         destination_name = self.fivetran_api.fivetran_groups[created_destination["group_id"]][
             "name"
         ]
         self.load_results["destinations"]["created"].add(destination_name)
         return created_destination
 
-    def _update_fivetran_connector(self, connector_details):
+    def _fivetran_connector_updated(self, connector_details):
+        current_connector = self.fivetran_api._get_connector_details(connector_details["id"])
+        return connector_details == current_connector
+
+    def _update_fivetran_connector(self, connector_details, group_name):
         connector_id = connector_details["id"]
+        if self._fivetran_connector_updated(connector_details):
+            console.print(f"Connector [green]{connector_id}[/green] already up to date. Skipping")
+            return connector_details
+        connector_details["run_setup_tests"] = False
+        self._fill_required_config_fields(connector_details, group_name)
         updated_connector = self.fivetran_api.update_connector(connector_id, connector_details)
         connector_schema = updated_connector["schema"]
         self.load_results["connectors"]["updated"].add(connector_schema)
         return updated_connector
 
     def _create_fivetran_connector(self, connector_details):
         del connector_details["id"]
         console.print("Creating Fivetran connector")
+        connector_details["run_setup_tests"] = False
         created_connector = self.fivetran_api.create_connector(connector_details)
         connector_schema = created_connector["schema"]
         self.load_results["connectors"]["created"].add(connector_schema)
         return created_connector
 
-    def _update_target_connector_schema_config(self, connector, schemas):
+    def _update_target_connector_schema_config(self, connector, extracted_schemas):
         connector_id = connector["id"]
         connector_schemas = self.fivetran_api._get_connector_schemas(connector_id)
         if connector_schemas:
-            self.fivetran_api.update_connector_schema_config(connector_id, schemas)
+            self.fivetran_api.update_connector_schema_config(connector_id, extracted_schemas)
+            for extracted_schema in extracted_schemas.values():
+                schema_name_in_destination = extracted_schema["name_in_destination"]
+                self.load_results["schemas"]["updated"].add(schema_name_in_destination)
+                for table_config in extracted_schema.get("tables", {}).values():
+                    table_name_in_destination = table_config["name_in_destination"]
+                    self.fivetran_api.update_connector_table_config(
+                        connector_id,
+                        schema_name_in_destination,
+                        table_name_in_destination,
+                        table_config,
+                    )
+                    self.load_results["tables"]["updated"].add(table_name_in_destination)
 
     def _get_existent_destination(self, target_group_id):
         for dest_data in self.fivetran_api.fivetran_data.values():
             existent_dest_details = dest_data["details"]
             if existent_dest_details["group_id"] == target_group_id:
                 return dest_data
         return {}
@@ -265,36 +285,35 @@
         - create a new one if doesn't
         """
         group_name = self.fivetran_api.fivetran_groups[target_group_id]["name"]
         destination_data = {}
         # get details
         for destination_data in exported_destination.values():
             exported_dest_details = destination_data["details"]
-            exported_dest_details["run_setup_tests"] = False
             exported_dest_connectors = destination_data.get("connectors", {})
 
         # if ID in fivetran_data
         current_destination = self._get_existent_destination(target_group_id)
         if current_destination:
             # update
             self._update_fivetran_destination(exported_dest_details)
         else:
             # create
             self._create_fivetran_destination(exported_dest_details)
 
         for exported_connector in exported_dest_connectors.values():
             exported_connector_details = exported_connector["details"]
-            exported_connector_details["run_setup_tests"] = False
-            self._fill_required_config_fields(exported_connector_details, group_name)
-
             if current_destination and self._exported_connector_exists_in_destination(
                 exported_connector_details, current_destination
             ):
-                target_connector = self._update_fivetran_connector(exported_connector_details)
+                target_connector = self._update_fivetran_connector(
+                    exported_connector_details, group_name
+                )
             else:
+                self._fill_required_config_fields(exported_connector_details, group_name)
                 target_connector = self._create_fivetran_connector(exported_connector_details)
 
             exported_schemas = exported_connector.get("schemas", {})
             if exported_schemas:
                 self._update_target_connector_schema_config(target_connector, exported_schemas)
 
     def _fill_required_config_fields(self, connector_details, group_name):
```

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/load/main.py` & `dbt_coves-1.5.0/dbt_coves/tasks/load/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/setup/all.py` & `dbt_coves-1.5.0/dbt_coves/tasks/setup/all.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/setup/dbt.py` & `dbt_coves-1.5.0/dbt_coves/tasks/setup/dbt.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,16 @@
             dbt_project_yaml_path = file_exists(Path(os.getcwd()), "dbt_project.yml")
 
         if dbt_project_yaml_path.exists():
             output = run_and_capture_cwd(["dbt", "deps"], dbt_project_yaml_path.parent)
 
             if output.returncode == 0:
                 deps_status = "[green]SUCCESS :heavy_check_mark:[/green]"
+            else:
+                deps_status = "[red]FAIL :cross_mark:[/red]"
             print_row(
                 "dbt deps",
                 deps_status,
                 new_section=True,
             )
             if output.returncode > 0:
                 raise Exception("dbt deps error. Check logs.")
```

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/setup/git.py` & `dbt_coves-1.5.0/dbt_coves/tasks/setup/git.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/setup/main.py` & `dbt_coves-1.5.0/dbt_coves/tasks/setup/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from rich.console import Console
 
 from dbt_coves.tasks.base import NonDbtBaseTask
-from dbt_coves.tasks.setup.git import SetupGitTask
 
 from .all import SetupAllTask
 from .dbt import SetupDbtTask
+from .git import SetupGitTask
+from .pre_commit import SetupPrecommitTask
 from .ssh import SetupSSHTask
 
 console = Console()
 
 
+class DbtCovesSetupException(Exception):
+    pass
+
+
 class SetupTask(NonDbtBaseTask):
     """
     Task that code-gen dbt resources
     """
 
     key_column_with = 20
     value_column_with = 50
@@ -28,9 +33,10 @@
         )
         ext_subparser.set_defaults(cls=cls, which="setup")
         sub_parsers = ext_subparser.add_subparsers(title="dbt-coves setup commands", dest="task")
         SetupAllTask.register_parser(sub_parsers, base_subparser)
         SetupGitTask.register_parser(sub_parsers, base_subparser)
         SetupDbtTask.register_parser(sub_parsers, base_subparser)
         SetupSSHTask.register_parser(sub_parsers, base_subparser)
+        SetupPrecommitTask.register_parser(sub_parsers, base_subparser)
         cls.arg_parser = ext_subparser
         return ext_subparser
```

### Comparing `dbt_coves-1.4.9/dbt_coves/tasks/setup/ssh.py` & `dbt_coves-1.5.0/dbt_coves/tasks/setup/ssh.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/templates/staging_model.sql` & `dbt_coves-1.5.0/dbt_coves/templates/staging_model.sql`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/ui/traceback.py` & `dbt_coves-1.5.0/dbt_coves/ui/traceback.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/utils/flags.py` & `dbt_coves-1.5.0/dbt_coves/utils/flags.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,16 +20,22 @@
 
         Args:
             cli_parser (ArgumentParser): CLI parser.
         """
         self.cli_parser = cli_parser
         self.log_level: str = "info"
         self.config_path: Path = Path(str())
-        self.profiles_dir: Optional[Path] = None
+        self.PROFILES_DIR: Optional[Path] = None
         self.project_dir: Optional[Path] = None
+        self.threads: str = None
+        self.MACRO_DEBUGGING: bool = False
+        self.VERSION_CHECK: bool = False
+        self.TARGET_PATH: str = None
+        self.LOG_PATH: str = None
+        self.LOG_CACHE_EVENTS: bool = False
         self.verbose: bool = False
         self.generate = {
             "sources": {
                 "select_relations": [],
                 "exclude_relations": [],
                 "database": None,
                 "schemas": [],
@@ -110,35 +116,47 @@
             "git": {"no_prompt": False},
         }
         self.dbt = {"command": None, "project_dir": None, "virtualenv": None, "cleanup": False}
 
     def parse_args(self, cli_args: List[str] = list()) -> None:
         self.args = self.cli_parser.parse_args(cli_args or sys.argv[1:])
 
-        if hasattr(self.args, "profiles_dir"):
-            self.args.profiles_dir = os.path.expanduser(self.args.profiles_dir)
+        if hasattr(self.args, "PROFILES_DIR"):
+            self.args.PROFILES_DIR = os.path.expanduser(self.args.PROFILES_DIR)
 
         if getattr(self.args, "project_dir", None) is not None:
             expanded_user = os.path.expanduser(self.args.project_dir)
             self.args.project_dir = os.path.abspath(expanded_user)
         self.task = self.args.task
         self.task_cls = getattr(self.args, "cls", None)
 
         if self.task:
             if self.args:
                 if self.args.log_level:
                     self.log_level = self.args.log_level
                 if self.args.verbose:
                     self.verbose = self.args.verbose
-                if self.args.profiles_dir:
-                    self.profiles_dir = self.args.profiles_dir
+                if self.args.PROFILES_DIR:
+                    self.PROFILES_DIR = self.args.PROFILES_DIR
                 if self.args.project_dir:
                     self.project_dir = self.args.project_dir
                 if self.args.config_path:
                     self.config_path = Path(self.args.config_path).expanduser()
+                if self.args.threads:
+                    self.threads = self.args.threads
+                if self.args.MACRO_DEBUGGING:
+                    self.MACRO_DEBUGGING = self.args.MACRO_DEBUGGING
+                if self.args.VERSION_CHECK:
+                    self.VERSION_CHECK = self.args.VERSION_CHECK
+                if self.args.TARGET_PATH:
+                    self.TARGET_PATH = self.args.TARGET_PATH
+                if self.args.LOG_PATH:
+                    self.LOG_PATH = self.args.LOG_PATH
+                if self.args.LOG_CACHE_EVENTS:
+                    self.LOG_CACHE_EVENTS = self.args.LOG_CACHE_EVENTS
 
             # generate sources
             if self.args.cls.__name__ == "GenerateSourcesTask":
                 if self.args.schemas:
                     self.generate["sources"]["schemas"] = [
                         schema.strip() for schema in self.args.schemas.split(",")
                     ]
```

### Comparing `dbt_coves-1.4.9/dbt_coves/utils/jinja.py` & `dbt_coves-1.5.0/dbt_coves/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/utils/log.py` & `dbt_coves-1.5.0/dbt_coves/utils/log.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/utils/shell.py` & `dbt_coves-1.5.0/dbt_coves/utils/shell.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/dbt_coves/utils/yaml.py` & `dbt_coves-1.5.0/dbt_coves/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.4.9/pyproject.toml` & `dbt_coves-1.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt_coves"
-version = "1.4.9"
+version = "1.5.0"
 description = "CLI tool for dbt users adopting analytics engineering best practices."
 authors = ["Datacoves <hello@datacoves.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Information Technology",
@@ -32,19 +32,21 @@
 questionary = "^1.9.0"
 yamlloader = "^1.0.0"
 pyfiglet = "^0.8.post1"
 click = "^8.0.3"
 rich = ">=10.4,<14.0"
 Jinja2 = ">2.11.2"
 python-slugify = "<9.0.0"
-dbt-core = ">=1.1,<1.5"
+dbt-core = ">=1.1,<1.6"
 bumpversion = "^0.6.0"
 typing_extensions = { version = "^4.0", python = "^3.7" }
 ruamel-yaml = "^0.17.21"
 db-dtypes = "^1.0.5"
+copier = "6.0.0"
+gitpython = "^3.1.31"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 mypy = "^0.991"
 towncrier = "^22.12.0"
 pytest-mock = "^3.6.1"
@@ -58,22 +60,22 @@
 sphinxcontrib-restbuilder = "^0.3"
 types-PyYAML = "^5.4.1"
 types-python-slugify = "^8.0.0.0"
 types-requests = "^2.28.11.5"
 flake8 = "^5.0.0"
 
 [tool.poetry.group.test.dependencies]
-dbt-redshift = ">=1.1,<1.5"
-dbt-bigquery = ">=1.1,<1.5"
-dbt-snowflake = ">=1.1,<1.5"
+dbt-redshift = ">=1.1,<1.6"
+dbt-bigquery = ">=1.1,<1.6"
+dbt-snowflake = ">=1.1,<1.6"
 redshift-connector = "^2.0.910"
 pytest-dependency = "^0.5.1"
 python-dotenv = "^0.21.1"
 pandas = "^1.3.0"
-snowflake-connector-python = {extras = ["pandas"], version = "^2.7.12"}
+snowflake-connector-python = {extras = ["pandas"], version = "^3.0"}
 google-cloud-bigquery = ">2.34,<4"
 tox-poetry-installer = "^0.10.0"
 tox = "^3.23.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
@@ -115,12 +117,12 @@
 markers = ["datafiles"]
 
 [tool.black]
 line-length = 100
 target-version=['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.isort]
-known_third_party=["dbt", "dotenv", "google", "jinja2", "pretty_errors", "pydantic", "pyfiglet", "pytest", "questionary", "redshift_connector", "requests", "rich", "ruamel", "slugify", "snowflake"]
+known_third_party=["copier", "dbt", "dotenv", "git", "google", "jinja2", "pretty_errors", "pydantic", "pyfiglet", "pytest", "questionary", "redshift_connector", "requests", "rich", "ruamel", "slugify", "snowflake"]
 line_length=100
 multi_line_output=3
 include_trailing_comma=true
 profile="black"
```

### Comparing `dbt_coves-1.4.9/PKG-INFO` & `dbt_coves-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-coves
-Version: 1.4.9
+Version: 1.5.0
 Summary: CLI tool for dbt users adopting analytics engineering best practices.
 Home-page: https://datacoves.com
 License: Apache 2.0
 Keywords: data engineering,analytics engineering,dbt,ETL,data modelling
 Author: Datacoves
 Author-email: hello@datacoves.com
 Requires-Python: >=3.7.2,<3.11
@@ -22,16 +22,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Dist: Jinja2 (>2.11.2)
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: bumpversion (>=0.6.0,<0.7.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
+Requires-Dist: copier (==6.0.0)
 Requires-Dist: db-dtypes (>=1.0.5,<2.0.0)
-Requires-Dist: dbt-core (>=1.1,<1.5)
+Requires-Dist: dbt-core (>=1.1,<1.6)
+Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: luddite (>=1.0.1,<2.0.0)
 Requires-Dist: packaging (>=20.8,<22.0)
 Requires-Dist: pretty-errors (>=1.2.19,<2.0.0)
 Requires-Dist: pydantic (>=1.8,<2.0)
 Requires-Dist: pyfiglet (>=0.8.post1,<0.9)
 Requires-Dist: python-slugify (<9.0.0)
 Requires-Dist: questionary (>=1.9.0,<2.0.0)
```

