# Comparing `tmp/hnhm-0.0.6.tar.gz` & `tmp/hnhm-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnhm-0.0.6.tar", max compression
+gzip compressed data, was "hnhm-0.0.7.tar", max compression
```

## Comparing `hnhm-0.0.6.tar` & `hnhm-0.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      707 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/__init__.py
--rw-r--r--   0        0        0     1481 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/cli.py
--rw-r--r--   0        0        0      602 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/__init__.py
--rw-r--r--   0        0        0     1084 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/attribute.py
--rw-r--r--   0        0        0      554 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/entity.py
--rw-r--r--   0        0        0       80 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/error.py
--rw-r--r--   0        0        0      311 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/group.py
--rw-r--r--   0        0        0      543 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/layout.py
--rw-r--r--   0        0        0      654 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/link.py
--rw-r--r--   0        0        0     2461 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/migrations.py
--rw-r--r--   0        0        0       80 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/priority.py
--rw-r--r--   0        0        0      517 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/sql.py
--rw-r--r--   0        0        0     2725 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/storage.py
--rw-r--r--   0        0        0     1545 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/core/tasks.py
--rw-r--r--   0        0        0      564 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/file_storage.py
--rw-r--r--   0        0        0     8343 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/flow.py
--rw-r--r--   0        0        0    10802 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/hnhm.py
--rw-r--r--   0        0        0      902 2023-04-27 17:50:39.722219 hnhm-0.0.6/hnhm/hnhm_attribute.py
--rw-r--r--   0        0        0     3865 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/hnhm_entity.py
--rw-r--r--   0        0        0     2465 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/hnhm_link.py
--rw-r--r--   0        0        0     1297 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/hnhm_registry.py
--rw-r--r--   0        0        0     6902 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/plan_printer.py
--rw-r--r--   0        0        0        0 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/__init__.py
--rw-r--r--   0        0        0    13179 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql.py
--rw-r--r--   0        0        0      459 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/__init__.py
--rw-r--r--   0        0        0      528 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/create_attribute.py
--rw-r--r--   0        0        0      549 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/create_group.py
--rw-r--r--   0        0        0      344 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/create_hub.py
--rw-r--r--   0        0        0      576 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/create_link.py
--rw-r--r--   0        0        0      228 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/create_stage.py
--rw-r--r--   0        0        0      507 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/load_hub.py
--rw-r--r--   0        0        0      983 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/load_ignore.py
--rw-r--r--   0        0        0     4563 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/load_new.py
--rw-r--r--   0        0        0     2139 2023-04-27 17:50:39.726219 hnhm-0.0.6/hnhm/postgres/sql_templates/load_update.py
--rw-r--r--   0        0        0      707 2023-04-27 17:50:39.726219 hnhm-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 hnhm-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      707 2023-05-18 14:47:59.411816 hnhm-0.0.7/hnhm/__init__.py
+-rw-r--r--   0        0        0     1481 2023-05-18 14:47:59.411816 hnhm-0.0.7/hnhm/cli.py
+-rw-r--r--   0        0        0      648 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/__init__.py
+-rw-r--r--   0        0        0     1139 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/attribute.py
+-rw-r--r--   0        0        0      627 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/entity.py
+-rw-r--r--   0        0        0       80 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/error.py
+-rw-r--r--   0        0        0      553 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/group.py
+-rw-r--r--   0        0        0      543 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/layout.py
+-rw-r--r--   0        0        0      654 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/link.py
+-rw-r--r--   0        0        0     3147 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/migrations.py
+-rw-r--r--   0        0        0       94 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/priority.py
+-rw-r--r--   0        0        0      517 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/sql.py
+-rw-r--r--   0        0        0     2776 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/storage.py
+-rw-r--r--   0        0        0     2253 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/core/tasks.py
+-rw-r--r--   0        0        0      567 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/file_storage.py
+-rw-r--r--   0        0        0     8724 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/flow.py
+-rw-r--r--   0        0        0    12112 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/hnhm.py
+-rw-r--r--   0        0        0      894 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/hnhm_attribute.py
+-rw-r--r--   0        0        0     3915 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/hnhm_entity.py
+-rw-r--r--   0        0        0     2564 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/hnhm_link.py
+-rw-r--r--   0        0        0     1297 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/hnhm_registry.py
+-rw-r--r--   0        0        0     7419 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/plan_printer.py
+-rw-r--r--   0        0        0        0 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/__init__.py
+-rw-r--r--   0        0        0    14036 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql.py
+-rw-r--r--   0        0        0      488 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/create_attribute.sql
+-rw-r--r--   0        0        0      513 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/create_group.sql
+-rw-r--r--   0        0        0      310 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/create_hub.sql
+-rw-r--r--   0        0        0      540 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/create_link.sql
+-rw-r--r--   0        0        0      192 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/create_stage.sql
+-rw-r--r--   0        0        0      474 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/load_hub.sql
+-rw-r--r--   0        0        0      946 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/load_ignore.sql
+-rw-r--r--   0        0        0     4530 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/load_new.sql
+-rw-r--r--   0        0        0     2103 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/load_update.sql
+-rw-r--r--   0        0        0      781 2023-05-18 14:47:59.415816 hnhm-0.0.7/hnhm/postgres/sql_templates/update_entity_view.sql
+-rw-r--r--   0        0        0      806 2023-05-18 14:47:59.419816 hnhm-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      511 1970-01-01 00:00:00.000000 hnhm-0.0.7/PKG-INFO
```

### Comparing `hnhm-0.0.6/hnhm/__init__.py` & `hnhm-0.0.7/hnhm/__init__.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.6/hnhm/cli.py` & `hnhm-0.0.7/hnhm/cli.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.6/hnhm/core/__init__.py` & `hnhm-0.0.7/hnhm/core/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,10 +13,12 @@
     RemoveLink,
     CreateGroup,
     RemoveGroup,
     CreateEntity,
     RemoveEntity,
     CreateAttribute,
     RemoveAttribute,
+    RemoveEntityView,
     AddGroupAttribute,
+    RecreateEntityView,
     RemoveGroupAttribute,
 )
```

### Comparing `hnhm-0.0.6/hnhm/core/attribute.py` & `hnhm-0.0.7/hnhm/core/attribute.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,21 +30,25 @@
         return self.name
 
 
 class Attribute(pydantic.BaseModel):
     """Attribute core representation."""
 
     name: str
+    entity_name: str
     comment: str
     type: Type
     change_type: ChangeType
     group: str | None = None
-    owner: str | None = None
+
+    @property
+    def table(self):
+        return f"attr__{self.entity_name}__{self.name}"
 
     def __str__(self):
         return f"<{self.type} '{self.name}' change_type='{self.change_type}'>"
 
     def __hash__(self):
-        return hash(f"{self.owner}.{self.name}.{self.type}")
+        return hash(self.table)
 
     def __eq__(self, other):
         return hash(self) == hash(other)
```

### Comparing `hnhm-0.0.6/hnhm/core/layout.py` & `hnhm-0.0.7/hnhm/core/layout.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.6/hnhm/core/link.py` & `hnhm-0.0.7/hnhm/core/link.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.6/hnhm/core/migrations.py` & `hnhm-0.0.7/hnhm/core/migrations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+"""
+Create Entity order:
+    1. Create Entity
+    2. Create Attribute, Group
+    3. Recreate Entity's view
+
+Update Entity order:
+    1. Remove Entity's view
+    2. Create Entity
+    3. Create Attribute, Group
+    4. Recreate Entity's view
+
+Remove Entity order:
+    1. Remove Entity's view
+    2. Remove Attribute, Group
+    3. Remove Entity
+"""
 import pydantic
 
 from .link import Link
 from .group import Group
 from .entity import Entity
 from .priority import Priority
 from .attribute import Attribute
@@ -16,32 +33,48 @@
     entity: Entity
 
     def __str__(self):
         return f"<CreateEntity '{self.entity.name}'>"
 
 
 class RemoveEntity(Migration):
-    priority = Priority.SECOND
+    priority = Priority.THIRD
     entity: Entity
 
     def __str__(self):
         return f"<RemoveEntity '{self.entity.name}'>"
 
 
+class RecreateEntityView(Migration):
+    priority = Priority.THIRD
+    entity: Entity
+
+    def __str__(self):
+        return f"<RecreateEntityView '{self.entity.name}'>"
+
+
+class RemoveEntityView(Migration):
+    priority = Priority.FIRST
+    entity: Entity
+
+    def __str__(self):
+        return f"<RemoveEntityView '{self.entity.name}'>"
+
+
 class CreateAttribute(Migration):
     priority = Priority.SECOND
     entity: Entity
     attribute: Attribute
 
     def __str__(self):
         return f"<CreateAttribute '{self.attribute.name}' entity='{self.entity.name}'>"
 
 
 class RemoveAttribute(Migration):
-    priority = Priority.FIRST
+    priority = Priority.SECOND
     entity: Entity
     attribute: Attribute
 
     def __str__(self):
         return f"<RemoveAttribute '{self.attribute.name}' entity='{self.entity.name}'>"
 
 
@@ -51,15 +84,15 @@
     group: Group
 
     def __str__(self):
         return f"<CreateGroup '{self.group.name}' entity='{self.entity.name}'>"
 
 
 class RemoveGroup(Migration):
-    priority = Priority.FIRST
+    priority = Priority.SECOND
     entity: Entity
     group: Group
 
     def __str__(self):
         return f"<RemoveGroup '{self.group.name}' entity='{self.entity.name}'>"
```

### Comparing `hnhm-0.0.6/hnhm/core/sql.py` & `hnhm-0.0.7/hnhm/core/sql.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.6/hnhm/core/storage.py` & `hnhm-0.0.7/hnhm/core/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .error import HnhmError
 
 
 class HnhmStorageData(pydantic.BaseModel):
     """State data for hnhm."""
 
     entities: dict[str, Entity]
+    entities_views: set[str]
     links: dict[str, Link]
 
     def check_entity_exists(self, entity: str):
         if entity not in self.entities:
             raise HnhmError(f"Entity '{entity}' doesn't exist.")
 
     def check_entity_not_exists(self, entity: str):
@@ -68,11 +69,11 @@
     @abc.abstractmethod
     def save(self, data: HnhmStorageData):
         raise NotImplementedError
 
 
 class InMemStorage(Storage):
     def load(self) -> HnhmStorageData:
-        return HnhmStorageData(entities={}, links={})
+        return HnhmStorageData(entities={}, entities_views=set(), links={})
 
     def save(self, data: HnhmStorageData):
         pass
```

### Comparing `hnhm-0.0.6/hnhm/core/tasks.py` & `hnhm-0.0.7/hnhm/core/tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from abc import abstractmethod
+
 import pydantic
 
 from .link import Link
 from .group import Group
 from .entity import Entity
 from .priority import Priority
 from .attribute import Attribute
@@ -10,30 +12,48 @@
 class Task(pydantic.BaseModel):
     """Flow task."""
 
     priority: Priority
     source: Entity
     business_time_field: Attribute
     keys_mapping: dict[Attribute, Attribute]
+    depends_on: list[str] = []
+
+    @property
+    @abstractmethod
+    def id(self):
+        raise NotImplementedError
 
 
 class LoadHub(Task):
     priority = Priority.FIRST
     target: Entity
 
+    @property
+    def id(self):
+        return f"load_hub__{self.source.name}__{self.target.name}"
+
     def __str__(self):
         return f"<LoadHub source='{self.source.name}' target='{self.target.name}'>"
 
 
 class LoadAttribute(Task):
     priority = Priority.SECOND
     target: Entity
     source_attribute: Attribute
     target_attribute: Attribute
 
+    @property
+    def id(self):
+        return (
+            "load_attribute"
+            f"__{self.source.name}_{self.source_attribute.name}"
+            f"__{self.target.name}_{self.target_attribute.name}"
+        )
+
     def __str__(self):
         return (
             "<LoadAttribute"
             f" source='{self.source.name}'"
             f" target='{self.target.name}'"
             f" source_attribute='{self.source_attribute.name}'"
             f" target_attribute='{self.target_attribute.name}'>"
@@ -42,23 +62,34 @@
 
 class LoadGroup(Task):
     priority = Priority.SECOND
     target: Entity
     group: Group
     attributes_mapping: dict[Attribute, Attribute]
 
+    @property
+    def id(self):
+        return (
+            f"load_group"
+            f"__{self.source.name}"
+            f"__{self.target.name}_{self.group.name}"
+        )
+
     def __str__(self):
         return (
-            "<LoadGroup"
+            f"<LoadGroup '{self.group.name}'"
             f" source='{self.source.name}'"
-            f" target='{self.target.name}'"
-            f" group_name='{self.group.name}'>"
+            f" target='{self.target.name}'>"
         )
 
 
 class LoadLink(Task):
     priority = Priority.SECOND
     link: Link
     keys_mapping: dict[str, dict[Attribute, Attribute]]
 
+    @property
+    def id(self):
+        return f"load_link__{self.source.name}__{self.link.name}"
+
     def __str__(self):
-        return f"<LoadLink source='{self.source.name}' link_name='{self.link.name}'>"
+        return f"<LoadLink '{self.link.name}' source='{self.source.name}'>"
```

### Comparing `hnhm-0.0.6/hnhm/flow.py` & `hnhm-0.0.7/hnhm/flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         if source.layout.type != LayoutType.STAGE:
             raise HnhmError(
                 f"Flow doesn't support loading from entities with layout type '{source.layout.type}'."
                 " Please, use Flow to load data only from STAGE entities."
             )
 
         self.source = source
-        self.business_time_field = business_time_field.to_core()
+        self.business_time_field = business_time_field.to_core(source.name)
 
         # {entity_name -> {attribute_target -> attribute_source}}
         self._entities_keys_mappings: dict[str, dict[Attribute, Attribute]] = {}
 
         # {entity_name -> target}
         self._hubs: dict[str, Entity] = {}
 
@@ -39,72 +39,78 @@
         self._groups: dict[str, dict[str, dict[Attribute, Attribute]]] = {}
 
         # {link_name -> {entity_name -> {attribute_target -> attribute_source}}}
         self._links = {}
 
     @property
     def tasks(self) -> list[Task]:
-        tasks: list[Task] = []
+        tasks = []
+        hub_tasks = {}
         for target_name, target in self._hubs.items():
             keys_mapping = self._entities_keys_mappings[target_name]
-            tasks.append(
-                LoadHub(
-                    source=self.source,
-                    target=target,
-                    keys_mapping=keys_mapping,
-                    business_time_field=self.business_time_field,
-                )
+            hub_tasks[target_name] = LoadHub(
+                source=self.source,
+                target=target,
+                keys_mapping=keys_mapping,
+                business_time_field=self.business_time_field,
             )
 
         for target_name, attributes_mapping in self._attributes.items():
             target = self._hubs[target_name]
+            depends_on = [hub_tasks[target_name].id]
             keys_mapping = self._entities_keys_mappings[target_name]
+
             for target_attribute, source_attribute in attributes_mapping.items():
                 tasks.append(
                     LoadAttribute(
                         source=self.source,
                         target=target,
                         keys_mapping=keys_mapping,
                         source_attribute=source_attribute,
                         target_attribute=target_attribute,
                         business_time_field=self.business_time_field,
+                        depends_on=depends_on,
                     )
                 )
 
         for target_name, groups_mapping in self._groups.items():
             target = self._hubs[target_name]
+            depends_on = [hub_tasks[target_name].id]
             keys_mapping = self._entities_keys_mappings[target_name]
             for group_name, attributes_mapping in groups_mapping.items():
                 group = target.groups[group_name]
                 tasks.append(
                     LoadGroup(
                         source=self.source,
                         target=target,
                         group=group,
                         keys_mapping=keys_mapping,
                         attributes_mapping=attributes_mapping,
                         business_time_field=self.business_time_field,
+                        depends_on=depends_on,
                     )
                 )
 
         for link_name, link in self._links.items():
             keys_mapping = {}
+            depends_on = []
             for link_element in link.elements:
-                keys_mapping[link_element.entity.name] = self._entities_keys_mappings[
-                    link_element.entity.name
-                ]
+                entity_name = link_element.entity.name
+                depends_on.append(hub_tasks[entity_name].id)
+                keys_mapping[entity_name] = self._entities_keys_mappings[entity_name]
             tasks.append(
                 LoadLink(
                     source=self.source,
                     link=link,
                     keys_mapping=keys_mapping,
                     business_time_field=self.business_time_field,
+                    depends_on=depends_on,
                 )
             )
-
+        tasks.extend(hub_tasks.values())
         tasks = sorted(tasks, key=lambda t: t.priority)
         return tasks
 
     def load(
         self,
         target: HnhmEntity | HnhmLink,
         mapping: dict[HnhmAttribute, HnhmAttribute] | None = None,
@@ -125,16 +131,16 @@
                         f" Your target entity='{target_entity.name}' has LayoutType='{target_entity.layout.type}'."
                     )
 
                 keys_mapping = {}
                 groups_mapping = {}
                 attributes_mapping = {}
                 for attribute_target, attribute_source in mapping.items():
-                    attribute_target = attribute_target.to_core()
-                    attribute_source = attribute_source.to_core()
+                    attribute_target = attribute_target.to_core(target_entity.name)
+                    attribute_source = attribute_source.to_core(self.source.name)
                     if attribute_target in target_entity.keys:
                         keys_mapping[attribute_target] = attribute_source
                     elif attribute_target.group:
                         group_name = attribute_target.group
                         if group_name not in groups_mapping:
                             groups_mapping[group_name] = {}
                         groups_mapping[group_name][attribute_target] = attribute_source
```

### Comparing `hnhm-0.0.6/hnhm/hnhm.py` & `hnhm-0.0.7/hnhm/hnhm.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,17 @@
     RemoveLink,
     CreateGroup,
     RemoveGroup,
     CreateEntity,
     RemoveEntity,
     CreateAttribute,
     RemoveAttribute,
+    RemoveEntityView,
     AddGroupAttribute,
+    RecreateEntityView,
     RemoveGroupAttribute,
 )
 
 from .hnhm_link import HnhmLink
 from .hnhm_entity import HnhmEntity
 
 
@@ -82,32 +84,42 @@
             link_core = link.to_core()
             core_links[link_core.name] = link_core
 
         plan = Plan(entities_migrations={}, links_migrations={})
 
         # Entity: create if not exists
         for entity in core_entities.values():
-            if entity.name in self.data.entities:
-                continue
+            migrations = []
+
+            # Entity's View: create/update if not exists
+            if (
+                entity.name not in self.data.entities_views
+                and entity.layout.type == LayoutType.HNHM
+            ):
+                migrations.append(RecreateEntityView(entity=entity))
 
             # Create Entity
-            migrations = [CreateEntity(entity=entity)]
+            if entity.name not in self.data.entities:
+                migrations.append(CreateEntity(entity=entity))
 
-            if entity.layout.type == LayoutType.HNHM:
-                # Create Attribute
-                for attribute in entity.attributes.values():
-                    migrations.append(CreateAttribute(entity=entity, attribute=attribute))
-                # Create Group
-                for group in entity.groups.values():
-                    migrations.append(CreateGroup(entity=entity, group=group))
+                if entity.layout.type == LayoutType.HNHM:
+                    # Create Attribute
+                    for attribute in entity.attributes.values():
+                        migrations.append(
+                            CreateAttribute(entity=entity, attribute=attribute)
+                        )
+                    # Create Group
+                    for group in entity.groups.values():
+                        migrations.append(CreateGroup(entity=entity, group=group))
 
-            plan.entities_migrations[entity.name] = PlanCollection(
-                type=PlanType.CREATE,
-                migrations=migrations,
-            )
+            if migrations:
+                plan.entities_migrations[entity.name] = PlanCollection(
+                    type=PlanType.CREATE,
+                    migrations=migrations,
+                )
 
         # Entity: create/remove/update Attribute/Group
         for entity in core_entities.values():
             if entity.name not in self.data.entities:
                 continue
 
             attributes_state = self.data.entities[entity.name].attributes
@@ -151,14 +163,21 @@
 
             # Remove Group
             for group_name, group in groups_state.items():
                 if group_name not in entity.groups:
                     migrations.append(RemoveGroup(entity=entity, group=group))
 
             if migrations:
+                if entity.layout.type == LayoutType.HNHM:
+                    migrations.extend(
+                        [
+                            RemoveEntityView(entity=entity),
+                            RecreateEntityView(entity=entity),
+                        ]
+                    )
                 plan.entities_migrations[entity.name] = PlanCollection(
                     type=PlanType.UPDATE,
                     migrations=migrations,
                 )
 
         # Link: remove
         for link_name, link in self.data.links.items():
@@ -170,14 +189,16 @@
 
         # Entity: remove
         for entity_name, entity in self.data.entities.items():
             if entity_name not in core_entities:
                 migrations = []
 
                 if entity.layout.type == LayoutType.HNHM:
+                    migrations.append(RemoveEntityView(entity=entity))
+
                     attributes_state = self.data.entities[entity_name].attributes
                     groups_state = self.data.entities[entity_name].groups
                     # Remove Attribute
                     for _, attribute_state in attributes_state.items():
                         migrations.append(
                             RemoveAttribute(entity=entity, attribute=attribute_state)
                         )
@@ -225,14 +246,24 @@
                     )
 
                 case RemoveEntity(entity=entity):
                     self.data.check_entity_exists(entity.name)
                     self.sql.execute(sql)
                     del self.data.entities[entity.name]
 
+                case RecreateEntityView(entity=entity):
+                    self.sql.execute(sql)
+                    self.data.entities_views.add(entity.name)
+
+                case RemoveEntityView(entity=entity):
+                    if entity.name not in self.data.entities_views:
+                        raise HnhmError(f"Entity's View '{entity.name}' doesn't exist.")
+                    self.sql.execute(sql)
+                    self.data.entities_views.remove(entity.name)
+
                 case CreateAttribute(entity=entity, attribute=attribute):
                     self.data.check_attribute_not_exists(entity.name, attribute.name)
                     self.sql.execute(sql)
                     self.data.entities[entity.name].attributes[attribute.name] = attribute
 
                 case RemoveAttribute(entity=entity, attribute=attribute):
                     self.data.check_attribute_exists(entity.name, attribute.name)
```

### Comparing `hnhm-0.0.6/hnhm/hnhm_attribute.py` & `hnhm-0.0.7/hnhm/hnhm_attribute.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,29 +12,27 @@
         comment: str,
         change_type: ChangeType,
         group: str | None = None,
     ):
         self.comment = comment
         self.change_type = change_type
         self.group = group
-
-        self.owner = None
         self.name = None
 
-    def to_core(self) -> Attribute:
+    def to_core(self, entity_name: str) -> Attribute:
         return Attribute(
             name=self.name,
+            entity_name=entity_name,
             comment=self.comment,
             type=self.type,
             change_type=self.change_type,
             group=self.group,
         )
 
-    def __set_name__(self, owner, name):
-        self.owner = str(owner)
+    def __set_name__(self, _, name):
         self.name = name
 
 
 class String(HnhmAttribute):
     type = Type.STRING
```

### Comparing `hnhm-0.0.6/hnhm/hnhm_entity.py` & `hnhm-0.0.7/hnhm/hnhm_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,37 +49,38 @@
                 for key in keys_hnhm:
                     if key.change_type != ChangeType.IGNORE:
                         raise HnhmError(
                             f"Change type='{key.change_type}' is not supported for Key attributes."
                             f" Use 'ChangeType.IGNORE' for the key attributes in the '{layout.type}.{name}' entity."
                         )
 
-                keys = [key.to_core() for key in keys_hnhm]
+                keys = [key.to_core(name) for key in keys_hnhm]
                 if len(keys) != len(set(keys)):
                     raise HnhmError(
                         f"Found duplicated keys for entity: '{layout.type}.{name}'."
                     )
 
             case _:
                 raise HnhmError(f"Unknown LayoutType='{layout.type}'")
 
         groups = {}
         attributes = {}
         for class_attribute in inspected.values():
             if not isinstance(class_attribute, HnhmAttribute):
                 continue
 
-            attribute = class_attribute.to_core()
+            attribute = class_attribute.to_core(name)
             attribute_name = attribute.name
 
             if attribute.group:
                 group_name = attribute.group
                 if group_name not in groups:
                     groups[group_name] = Group(
                         name=group_name,
+                        entity_name=name,
                         attributes={attribute_name: attribute},
                         change_type=attribute.change_type,
                     )
 
                 if groups[group_name].change_type != attribute.change_type:
                     raise HnhmError(
                         f"Found conflicting ChangeType for the entity='{layout.type}.{name}' group='{group_name}'."
```

### Comparing `hnhm-0.0.6/hnhm/hnhm_link.py` & `hnhm-0.0.7/hnhm/hnhm_link.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,24 +52,30 @@
         doc: str = inspected["__doc__"]
 
         if not inspected.get("__keys__"):
             raise HnhmError(
                 f"At least one Key is required for link='{name}'."
                 " Please, specify link's keys via the '__keys__' attribute."
             )
-        keys = inspected["__keys__"]
-        keys = [key.to_core() for key in keys]
+        keys_hnhm: list[HnhmEntity] = inspected["__keys__"]
+        keys = [key.to_core() for key in keys_hnhm]
 
         elements = []
         for class_attribute in inspected.values():
             if not isinstance(class_attribute, HnhmLinkElement):
                 continue
             link_element = class_attribute.to_core()
             elements.append(link_element)
 
         if len(elements) < 2:
             raise HnhmError(
                 f"At least two LinkElements are required for link='{name}'."
                 " Please, specify more than one elements."
             )
 
-        return Link(name=name, layout=layout, doc=doc, elements=elements, keys=keys)
+        return Link(
+            name=name,
+            layout=layout,
+            doc=doc,
+            elements=elements,
+            keys=keys,
+        )
```

### Comparing `hnhm-0.0.6/hnhm/hnhm_registry.py` & `hnhm-0.0.7/hnhm/hnhm_registry.py`

 * *Files identical despite different names*

### Comparing `hnhm-0.0.6/hnhm/plan_printer.py` & `hnhm-0.0.7/hnhm/plan_printer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     RemoveLink,
     CreateGroup,
     RemoveGroup,
     CreateEntity,
     RemoveEntity,
     CreateAttribute,
     RemoveAttribute,
+    RemoveEntityView,
     AddGroupAttribute,
+    RecreateEntityView,
     RemoveGroupAttribute,
 )
 
 
 class Color(str, Enum):
     green = "green"
     red = "red"
@@ -68,14 +70,19 @@
                             lines.append(
                                 PlanLine(
                                     text=f"    |attribute '{attribute.name}'",
                                     color=Color.green,
                                 )
                             )
 
+                case RecreateEntityView(entity=entity):
+                    lines.append(
+                        PlanLine(text=f"  {symbol} view '{entity.name}'", color=color)
+                    )
+
                 case CreateAttribute(entity=_, attribute=attribute):
                     lines.append(
                         PlanLine(
                             text=f"  + attribute '{attribute.name}'", color=Color.green
                         )
                     )
 
@@ -114,14 +121,20 @@
                             lines.append(
                                 PlanLine(
                                     text=f"    |attribute '{attribute.name}'",
                                     color=Color.red,
                                 )
                             )
 
+                case RemoveEntityView(entity=entity):
+                    if plan_collection.type == PlanType.REMOVE:
+                        lines.append(
+                            PlanLine(text=f"  - view '{entity.name}'", color=Color.red)
+                        )
+
                 case RemoveAttribute(entity=_, attribute=attribute):
                     lines.append(
                         PlanLine(
                             text=f"  - attribute '{attribute.name}'", color=Color.red
                         )
                     )
```

### Comparing `hnhm-0.0.6/hnhm/postgres/sql.py` & `hnhm-0.0.7/hnhm/postgres/sql.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from textwrap import dedent
 
 import jinja2
-from sqlalchemy import URL, Engine, text, create_engine
+from sqlalchemy import create_engine
+from sqlalchemy.engine import URL, Engine
 
 from hnhm.core import (
     Sql,
     Task,
     Type,
     LoadHub,
     LoadLink,
@@ -19,51 +20,41 @@
     CreateGroup,
     RemoveGroup,
     CreateEntity,
     RemoveEntity,
     LoadAttribute,
     CreateAttribute,
     RemoveAttribute,
+    RemoveEntityView,
     AddGroupAttribute,
+    RecreateEntityView,
     RemoveGroupAttribute,
 )
 
-from .sql_templates import (
-    SQL_TEMPLATE__LOAD_HUB,
-    SQL_TEMPLATE__LOAD_NEW,
-    SQL_TEMPLATE__CREATE_HUB,
-    SQL_TEMPLATE__CREATE_LINK,
-    SQL_TEMPLATE__LOAD_IGNORE,
-    SQL_TEMPLATE__LOAD_UPDATE,
-    SQL_TEMPLATE__CREATE_GROUP,
-    SQL_TEMPLATE__CREATE_STAGE,
-    SQL_TEMPLATE__CREATE_ATTRIBUTE,
-)
-
 PG_TYPES = {
     Type.STRING: "TEXT",
     Type.INTEGER: "INTEGER",
     Type.TIMESTAMP: "TIMESTAMPTZ",
 }
 
 
 def generate_sql(migration_or_task: Migration | Task, jinja: jinja2.Environment) -> str:
     match migration_or_task:
         case CreateEntity(entity=entity):
             if entity.layout.type == LayoutType.HNHM:
-                template = jinja.from_string(SQL_TEMPLATE__CREATE_HUB)
+                template = jinja.get_template("create_hub.sql")
                 columns = []
                 columns_types = []
                 for key in entity.keys:
                     columns.append(key.name)
                     column_type = PG_TYPES[key.type]
                     columns_types.append(f"{column_type} NOT NULL")
 
             elif entity.layout.type == LayoutType.STAGE:
-                template = jinja.from_string(SQL_TEMPLATE__CREATE_STAGE)
+                template = jinja.get_template("create_stage.sql")
                 columns = []
                 columns_types = []
                 for attribute in entity.attributes.values():
                     columns.append(attribute.name)
                     columns_types.append(PG_TYPES[attribute.type])
 
             else:
@@ -71,25 +62,51 @@
 
             return template.render(
                 name=entity.name,
                 columns=columns,
                 columns_types=columns_types,
             )
 
+        case RecreateEntityView(entity=entity):
+            template = jinja.get_template("update_entity_view.sql")
+
+            view_name = f"entity__{entity.name}"
+            sk = entity.sk
+            hub = f"hub__{entity.name}"
+
+            selects = []
+            for attribute in entity.attributes.values():
+                selects.append((attribute.table, attribute.name, attribute.name))
+
+            for group in entity.groups.values():
+                for attribute in group.attributes.values():
+                    selects.append(
+                        (group.table, attribute.name, f"{group.name}__{attribute.name}")
+                    )
+
+            return template.render(
+                view_name=view_name,
+                sk=sk,
+                hub=hub,
+                selects=selects,
+                attributes=entity.attributes.values(),
+                groups=entity.groups.values(),
+            )
+
         case CreateAttribute(entity=entity, attribute=attribute):
             attribute_type = PG_TYPES[attribute.type]
 
             if entity.layout.type == LayoutType.STAGE:
                 return f"ALTER TABLE stg__{entity.name} ADD COLUMN {attribute.name} {attribute_type}"
 
             time_columns = ["valid_from TIMESTAMPTZ NOT NULL"]
             if attribute.change_type == ChangeType.NEW:
                 time_columns.append("valid_to TIMESTAMPTZ")
 
-            template = jinja.from_string(SQL_TEMPLATE__CREATE_ATTRIBUTE)
+            template = jinja.get_template("create_attribute.sql")
             return template.render(
                 entity_name=entity.name,
                 attribute_name=attribute.name,
                 attribute_type=attribute_type,
                 time_columns=time_columns,
             )
 
@@ -99,15 +116,15 @@
                 column_type = PG_TYPES[attribute.type]
                 columns.append(f"{attribute.name} {column_type}")
 
             time_columns = ["valid_from TIMESTAMPTZ NOT NULL"]
             if group.change_type == ChangeType.NEW:
                 time_columns.append("valid_to TIMESTAMPTZ")
 
-            template = jinja.from_string(SQL_TEMPLATE__CREATE_GROUP)
+            template = jinja.get_template("create_group.sql")
             return template.render(
                 entity_name=entity.name,
                 group_name=group.name,
                 columns=columns,
                 time_columns=time_columns,
             )
 
@@ -120,15 +137,15 @@
             for link_element in link.elements:
                 entities.append(link_element.entity.name)
 
             primary_keys = ["valid_from"]
             for key in link.keys:
                 primary_keys.append(f"{key.entity.name}_sk")
 
-            template = jinja.from_string(SQL_TEMPLATE__CREATE_LINK)
+            template = jinja.get_template("create_link.sql")
             return template.render(
                 name=link.name,
                 entities=entities,
                 primary_keys=primary_keys,
             )
 
         case RemoveEntity(entity=entity):
@@ -149,28 +166,32 @@
 
         case RemoveGroupAttribute(entity=entity, group=group, attribute=attribute):
             return f"ALTER TABLE group__{entity.name}__{group.name} DROP COLUMN {attribute.name}"
 
         case RemoveLink(link=link):
             return f"DROP TABLE link__{link.name}"
 
+        case RemoveEntityView(entity=entity):
+            view_name = f"entity__{entity.name}"
+            return f"DROP VIEW {view_name}"
+
         case LoadHub(
             source=source,
             target=target,
             business_time_field=business_time_field,
             keys_mapping=keys_mapping,
         ):
             source_keys = [key_source.name for key_source in keys_mapping.values()]
             source_sk_components = (f"{key}::TEXT" for key in source_keys)
             source_sk_components = "|| '-' ||".join(source_sk_components)
             source_sk = f"MD5({source_sk_components})"
 
             target_keys = [key.name for key in target.keys]
 
-            template = jinja.from_string(SQL_TEMPLATE__LOAD_HUB)
+            template = jinja.get_template("load_hub.sql")
             return template.render(
                 source_name=source.name,
                 source_sk=source_sk,
                 source_keys=source_keys,
                 target_name=target.name,
                 target_keys=target_keys,
                 business_time_field=business_time_field.name,
@@ -196,19 +217,19 @@
             target_table = f"attr__{target.name}__{target_attribute.name}"
             target_sk = f"{target.name}_sk"
             target_sks = [f"{target.name}_sk"]
 
             target_attributes = [target_attribute.name]
 
             if target_attribute.change_type == ChangeType.IGNORE:
-                template = jinja.from_string(SQL_TEMPLATE__LOAD_IGNORE)
+                template = jinja.get_template("load_ignore.sql")
             elif target_attribute.change_type == ChangeType.UPDATE:
-                template = jinja.from_string(SQL_TEMPLATE__LOAD_UPDATE)
+                template = jinja.get_template("load_update.sql")
             elif target_attribute.change_type == ChangeType.NEW:
-                template = jinja.from_string(SQL_TEMPLATE__LOAD_NEW)
+                template = jinja.get_template("load_new.sql")
             else:
                 raise HnhmError(f"Unknown change type: '{target_attribute.change_type}'.")
 
             return template.render(
                 source_table=source_table,
                 source_sk=source_sk,
                 source_sks=[source_sk],
@@ -245,19 +266,19 @@
             target_sks = [target_sk]
 
             target_attributes = [
                 target_attribute.name for target_attribute in attributes_mapping
             ]
 
             if group.change_type == ChangeType.IGNORE:
-                template = jinja.from_string(SQL_TEMPLATE__LOAD_IGNORE)
+                template = jinja.get_template("load_ignore.sql")
             elif group.change_type == ChangeType.UPDATE:
-                template = jinja.from_string(SQL_TEMPLATE__LOAD_UPDATE)
+                template = jinja.get_template("load_update.sql")
             elif group.change_type == ChangeType.NEW:
-                template = jinja.from_string(SQL_TEMPLATE__LOAD_NEW)
+                template = jinja.get_template("load_new.sql")
             else:
                 raise HnhmError(f"Unknown change type: '{group.change_type}'.")
 
             return template.render(
                 source_table=source_table,
                 source_sk=source_sk,
                 source_sks=[source_sk],
@@ -289,15 +310,15 @@
                 source_sk = f"MD5({source_sk_components})"
 
                 target_sks.append(f"{entity_name}_sk")
                 source_sks.append(source_sk)
 
             target_table = f"link__{link.name}"
 
-            template = jinja.from_string(SQL_TEMPLATE__LOAD_NEW)
+            template = jinja.get_template("load_new.sql")
             return template.render(
                 source_table=source_table,
                 source_sks=source_sks,
                 source_attributes=[],
                 target_table=target_table,
                 target_sks=target_sks,
                 target_attributes=[],
@@ -332,15 +353,17 @@
                 password=password,
                 host=host,
                 database=database,
                 port=port,
             )
             self.engine = create_engine(connection_url)
 
-        self.jinja = jinja2.Environment()
+        self.jinja = jinja2.Environment(
+            loader=jinja2.PackageLoader("hnhm.postgres", "sql_templates")
+        )
         self.jinja.globals.update(zip=zip)
 
     @classmethod
     def with_engine(cls, engine: Engine):
         if engine.url.drivername != "postgresql+psycopg2":
             raise HnhmError(
                 f"Wrong driver name '{engine.url.drivername}'. Required: 'postgresql+psycopg2'."
@@ -353,15 +376,15 @@
     def execute(self, sql: str, debug: bool = False):
         if debug:
             print(dedent(sql).strip())
 
         conn = None
         try:
             conn = self.engine.connect()
-            conn.execute(text(sql))
-            conn.commit()
+            conn = conn.execution_options(isolation_level="AUTOCOMMIT")
+            conn.execute(sql)
         except Exception as e:
             raise e
         finally:
             if conn:
                 conn.close()
             self.engine.dispose()
```

### Comparing `hnhm-0.0.6/hnhm/postgres/sql_templates/create_group.py` & `hnhm-0.0.7/hnhm/postgres/sql_templates/create_group.sql`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-SQL_TEMPLATE__CREATE_GROUP = """
 CREATE TABLE group__{{ entity_name }}__{{ group_name }}(
     {{ entity_name }}_sk VARCHAR(32) NOT NULL,
     {% for column in columns -%}
         {{ column }},
     {% endfor -%}
     {% for time_column in time_columns -%}
         {{ time_column }},
     {% endfor -%}
     _source VARCHAR(512) NOT NULL,
     _loaded_at TIMESTAMPTZ NOT NULL,
     CONSTRAINT fk_{{ entity_name }}_sk
         FOREIGN KEY({{ entity_name }}_sk) 
         REFERENCES hub__{{ entity_name }}({{ entity_name }}_sk)
         ON DELETE NO ACTION
-)"""
+)
```

### Comparing `hnhm-0.0.6/hnhm/postgres/sql_templates/create_link.py` & `hnhm-0.0.7/hnhm/postgres/sql_templates/create_link.sql`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-SQL_TEMPLATE__CREATE_LINK = """
 CREATE TABLE link__{{ name }}(
     {% for entity in entities -%}
         {{ entity }}_sk VARCHAR(32) NOT NULL,
     {% endfor -%}
     valid_from TIMESTAMPTZ NOT NULL,
     valid_to TIMESTAMPTZ,
     _source VARCHAR(512) NOT NULL,
@@ -13,8 +12,7 @@
             FOREIGN KEY({{ entity }}_sk) 
             REFERENCES hub__{{ entity }}({{ entity }}_sk)
             ON DELETE NO ACTION,
     {% endfor -%}
 
     PRIMARY KEY({{ primary_keys | join(', ') }})
 )
-"""
```

### Comparing `hnhm-0.0.6/hnhm/postgres/sql_templates/load_ignore.py` & `hnhm-0.0.7/hnhm/postgres/sql_templates/load_ignore.sql`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-SQL_TEMPLATE__LOAD_IGNORE = """
 WITH data AS (
     SELECT
         {{ source_sk }} AS sk,
         {{ business_time_field }} AS valid_from,
 
         {% for source_attribute in source_attributes -%}
             {{ source_attribute }},
@@ -35,9 +34,8 @@
 FROM
     data d
 LEFT OUTER JOIN
     {{ target_table }} t
     ON d.sk = t.{{ target_sk }}
 WHERE
     t.{{ target_sk }} IS NULL
-    AND d.row_number = 1;
-"""
+    AND d.row_number = 1
```

### Comparing `hnhm-0.0.6/hnhm/postgres/sql_templates/load_new.py` & `hnhm-0.0.7/hnhm/postgres/sql_templates/load_new.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-SQL_TEMPLATE__LOAD_NEW = """
 BEGIN;
 
 CREATE TABLE _tmp__{{ target_table }}__load__new
 AS
 WITH data_all AS (
     SELECT
         {% for source_sk, target_sk in zip(source_sks, target_sks) -%}
@@ -169,8 +168,7 @@
             {% if not loop.last %} || '-' || {% endif %}
         {% endfor -%}
     );
 
 DROP TABLE _tmp__{{ target_table }}__load__new;
 
 COMMIT;
-"""
```

### Comparing `hnhm-0.0.6/hnhm/postgres/sql_templates/load_update.py` & `hnhm-0.0.7/hnhm/postgres/sql_templates/load_update.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-SQL_TEMPLATE__LOAD_UPDATE = """
 BEGIN;
 
 CREATE TABLE tmp__{{ target_table }}__load__update
 AS
 SELECT
     {{ source_sk }} AS sk,
     {{ business_time_field }} AS valid_from,
@@ -86,8 +85,7 @@
     updates u
 WHERE
     {{ target_sk }} = u.sk;
 
 DROP TABLE tmp__{{ target_table }}__load__update;
 
 COMMIT;
-"""
```

