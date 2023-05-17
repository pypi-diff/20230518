# Comparing `tmp/archaea_simulation-1.0.6.tar.gz` & `tmp/archaea_simulation-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archaea_simulation-1.0.6.tar", max compression
+gzip compressed data, was "archaea_simulation-1.0.7.tar", max compression
```

## Comparing `archaea_simulation-1.0.6.tar` & `archaea_simulation-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-02-10 23:01:01.799018 archaea_simulation-1.0.6/LICENSE
--rw-r--r--   0        0        0    11357 2023-02-10 23:01:01.799018 archaea_simulation-1.0.6/LICENSE.txt
--rw-r--r--   0        0        0      896 2023-02-10 23:01:01.799018 archaea_simulation-1.0.6/README.md
--rw-r--r--   0        0        0      333 2023-02-10 23:01:01.799018 archaea_simulation-1.0.6/archaea_simulation/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 23:01:01.799018 archaea_simulation-1.0.6/archaea_simulation/simulation_objects/__init__.py
--rw-r--r--   0        0        0     5480 2023-02-10 23:01:01.799018 archaea_simulation-1.0.6/archaea_simulation/simulation_objects/cfd_stl_export.py
--rw-r--r--   0        0        0     1979 2023-02-10 23:01:01.799018 archaea_simulation-1.0.6/archaea_simulation/simulation_objects/domain.py
--rw-r--r--   0        0        0     1841 2023-02-10 23:01:01.799018 archaea_simulation-1.0.6/archaea_simulation/simulation_objects/wall.py
--rw-r--r--   0        0        0       74 2023-02-10 23:01:01.799018 archaea_simulation-1.0.6/archaea_simulation/simulation_objects/wall_type.py
--rw-r--r--   0        0        0     1549 2023-02-10 23:01:01.799018 archaea_simulation-1.0.6/archaea_simulation/simulation_objects/zone.py
--rw-r--r--   0        0        0     1871 2023-02-10 23:01:01.887018 archaea_simulation-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1715 1970-01-01 00:00:00.000000 archaea_simulation-1.0.6/setup.py
--rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 archaea_simulation-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/LICENSE
+-rw-r--r--   0        0        0    11357 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/LICENSE.txt
+-rw-r--r--   0        0        0      896 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/README.md
+-rw-r--r--   0        0        0      333 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/__init__.py
+-rw-r--r--   0        0        0     6332 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/cfd_stl_export.py
+-rw-r--r--   0        0        0     6195 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/courtyard_building.py
+-rw-r--r--   0        0        0     2300 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/domain.py
+-rw-r--r--   0        0        0    10084 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/test_domain_init.stl
+-rw-r--r--   0        0        0     1841 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/wall.py
+-rw-r--r--   0        0        0       74 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/wall_type.py
+-rw-r--r--   0        0        0     1624 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/zone.py
+-rw-r--r--   0        0        0     1871 2023-05-17 22:23:03.567881 archaea_simulation-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1715 1970-01-01 00:00:00.000000 archaea_simulation-1.0.7/setup.py
+-rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 archaea_simulation-1.0.7/PKG-INFO
```

### Comparing `archaea_simulation-1.0.6/LICENSE` & `archaea_simulation-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `archaea_simulation-1.0.6/LICENSE.txt` & `archaea_simulation-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archaea_simulation-1.0.6/README.md` & `archaea_simulation-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `archaea_simulation-1.0.6/archaea_simulation/simulation_objects/domain.py` & `archaea_simulation-1.0.7/archaea_simulation/simulation_objects/domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 from archaea.geometry.point3d import Point3d
 from archaea.geometry.vector3d import Vector3d
 from archaea.geometry.loop import Loop
 from archaea.geometry.face import Face
+from archaea.geometry.mesh import Mesh
 from archaea_simulation.simulation_objects.wall import Wall
 from archaea_simulation.simulation_objects.zone import Zone
 
 
 class Domain(Zone):
     center: Point3d
     ground: Face
     x: float
     y: float
     z: float
     zones: "list[Zone]"
     context: "list[Wall]"
     openings: "list[Wall]"
 
-    def __init__(self, center: Point3d, x: float, y: float, z: float, zones=None, context=None):
+    def __init__(self,
+                 center: Point3d,
+                 x: float,
+                 y: float,
+                 z: float,
+                 zones=None,
+                 context=None):
         if context is None:
             context = []
         if zones is None:
             zones = []
         self.center = center
         self.x = x
         self.y = y
@@ -53,7 +60,13 @@
         faces += self.walls
 
         for zone in self.zones:
             faces += zone.create_solid_faces()
 
         return faces
 
+    def export_domain_to_stl(self):
+        mesh = Mesh()
+        walls = self.create_solid_faces()
+        mesh.add_from_faces(walls)
+        mesh.to_stl("", "test_domain_init")
+
```

### Comparing `archaea_simulation-1.0.6/archaea_simulation/simulation_objects/wall.py` & `archaea_simulation-1.0.7/archaea_simulation/simulation_objects/wall.py`

 * *Files identical despite different names*

### Comparing `archaea_simulation-1.0.6/archaea_simulation/simulation_objects/zone.py` & `archaea_simulation-1.0.7/archaea_simulation/simulation_objects/zone.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,17 +31,19 @@
         walls = []
         for line in wall_lines:
             border: Face = line.extrude(move_vector)
             wall = Wall(border.outer_loop, border.inner_loops)
             walls.append(wall)
         self.walls = walls
 
-    def create_solid_faces(self):
-        all_walls = self.walls
-        all_walls.append(self.floor.reverse())
-        all_walls.append(self.ceiling.reverse())
+    def all_surfaces(self):
+        all_surfaces = self.walls
+        all_surfaces.append(self.floor.reverse())
+        all_surfaces.append(self.ceiling.reverse())
+        return all_surfaces
 
+    def create_solid_faces(self):
         faces = []
-        for wall in all_walls:
+        for wall in self.all_surfaces():
             faces += wall.create_solid_faces()
 
         return faces
```

### Comparing `archaea_simulation-1.0.6/pyproject.toml` & `archaea_simulation-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archaea-simulation"
-version = "1.0.6"
+version = "1.0.7"
 description = "Wrapper definitions for simulation tools."
 readme = "README.md"
 authors = ["Oğuzhan Koral <oguzhankoral@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/archaeans/archaea-simulation"
 keywords = ["geometry", "simulation"]
 classifiers = [
```

### Comparing `archaea_simulation-1.0.6/setup.py` & `archaea_simulation-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['archaea>=1.1.13,<2.0.0']
 
 setup_kwargs = {
     'name': 'archaea-simulation',
-    'version': '1.0.6',
+    'version': '1.0.7',
     'description': 'Wrapper definitions for simulation tools.',
     'long_description': "# Archaea Simulation\n\nWrapper definitions for simulation tools.\n\nMotivation of creating this library is started with master thesis, departments of Computational\nScience and Engineering and Architecture at Istanbul Technical University. \nAim of thesis is to create scenarios for different environmental\nsolvers like EnergyPlus and OpenFOAM to run them parallely on Linux environment.\nPreparation of these scenario files done by geometric [Archaea](https://github.com/archaeans/archaea) library.\n\n\n## Focused Simulation Tools\n\n- OpenFOAM: OpenFOAM requires stl geometries to run it's solvers\nbehind the scenes. (Pre-Alpha)\n- EnergyPlus: EnergyPlus requires idf schema to run simulations. (MVP)\n- UWG: Urban weather generator is a solver to calculate effects on urban microclimate.\nIt creates new .epw file for EnergyPlus simulations.\n\nMain idea behind this work is to be experimental and didactic. ",
     'author': 'Oğuzhan Koral',
     'author_email': 'oguzhankoral@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/archaeans/archaea-simulation',
```

### Comparing `archaea_simulation-1.0.6/PKG-INFO` & `archaea_simulation-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archaea-simulation
-Version: 1.0.6
+Version: 1.0.7
 Summary: Wrapper definitions for simulation tools.
 Home-page: https://github.com/archaeans/archaea-simulation
 License: Apache-2.0
 Keywords: geometry,simulation
 Author: Oğuzhan Koral
 Author-email: oguzhankoral@gmail.com
 Requires-Python: >=3.8,<4.0
```

