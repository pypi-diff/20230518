# Comparing `tmp/multicloud_diagrams-0.2.5.tar.gz` & `tmp/multicloud_diagrams-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicloud_diagrams-0.2.5.tar", max compression
+gzip compressed data, was "multicloud_diagrams-0.3.0.tar", max compression
```

## Comparing `multicloud_diagrams-0.2.5.tar` & `multicloud_diagrams-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.2.5/LICENSE
--rw-r--r--   0        0        0     2423 2023-05-16 16:49:37.678198 multicloud_diagrams-0.2.5/README.md
--rw-r--r--   0        0        0    17035 2023-05-14 17:33:30.479330 multicloud_diagrams-0.2.5/multicloud_diagrams/__init__.py
--rw-r--r--   0        0        0      509 2023-05-16 16:49:37.688685 multicloud_diagrams-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2941 1970-01-01 00:00:00.000000 multicloud_diagrams-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-14 15:36:37.276228 multicloud_diagrams-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6733 2023-05-17 16:53:05.643771 multicloud_diagrams-0.3.0/README.md
+-rw-r--r--   0        0        0    18312 2023-05-17 15:40:04.072572 multicloud_diagrams-0.3.0/multicloud_diagrams/__init__.py
+-rw-r--r--   0        0        0      525 2023-05-17 16:55:53.000990 multicloud_diagrams-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7251 1970-01-01 00:00:00.000000 multicloud_diagrams-0.3.0/PKG-INFO
```

### Comparing `multicloud_diagrams-0.2.5/LICENSE` & `multicloud_diagrams-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multicloud_diagrams-0.2.5/multicloud_diagrams/__init__.py` & `multicloud_diagrams-0.3.0/multicloud_diagrams/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import xml.etree.ElementTree as et
 import logging
 import os.path
 
+import yaml
+
 
 class MultiCloudDiagrams:
     def __init__(self):
         self.mxfile = et.Element('mxfile', host="multicloud-diagrams",
                                  agent="PIP package multicloud-diagrams. Generate resources in draw.io compatible format for Cloud infrastructure. Copyrights @ Roman Tsypuk 2023. MIT license.",
                                  type="MultiCloud")
         self.diagram = et.SubElement(self.mxfile, 'diagram', id="diagram_1", name="AWS components")
@@ -293,14 +295,43 @@
         self.add_connection(src_node_id, dst_node_id, "classic", "none")
 
     def add_link_list(self, links):
         for link in links:
             self.add_link(src_node_id=link['sourceNodeID'], dst_node_id=link['destinationNodeID'])
         return
 
+    def augment_from_yaml(self, yaml_name: str):
+        with open(yaml_name, 'r') as file:
+            data = yaml.safe_load(file)
+            for vertex in data['vertices']:
+                self.add_vertex(
+                    id=vertex['arn'],
+                    node_name=vertex['name'],
+                    arn=vertex['arn'],
+                    node_type=vertex['type'],
+                    # optional attributes
+                    metadata={},
+                    # icon
+                )
+            for edge in data['edges']:
+                self.add_link(
+                    src_node_id=self._build_vertex_id(data['vertices'], edge, 'src'),
+                    dst_node_id=self._build_vertex_id(data['vertices'], edge, 'dst'),
+                    action=[edge['label']]
+                )
+
+    def _build_vertex_id(self, vertex_details, edge, src_dst_marker: str):
+        resource = {}
+        if f'{src_dst_marker}_arn' in edge:
+            resource["type"] = edge[f"{src_dst_marker}_type"]
+            resource["arn"] = edge[f'{src_dst_marker}_arn']
+        elif src_dst_marker in edge:
+            resource = [vertex for vertex in vertex_details if vertex['name'] == edge[src_dst_marker]][0]
+        return f'{resource["type"]}:{resource["arn"]}'
+
     def read_coords_from_file(self, file_name: str):
         if os.path.isfile(file_name):
             tree = et.parse(file_name)
             root = tree.getroot()
 
             for neighbor in root.iter('mxCell'):
                 if neighbor.get('id').startswith("vertex:"):
```

