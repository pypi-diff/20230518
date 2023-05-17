# Comparing `tmp/archaea_simulation-1.0.7.tar.gz` & `tmp/archaea_simulation-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archaea_simulation-1.0.7.tar", max compression
+gzip compressed data, was "archaea_simulation-1.0.8.tar", max compression
```

## Comparing `archaea_simulation-1.0.7.tar` & `archaea_simulation-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/LICENSE
--rw-r--r--   0        0        0    11357 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/LICENSE.txt
--rw-r--r--   0        0        0      896 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/README.md
--rw-r--r--   0        0        0      333 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/__init__.py
--rw-r--r--   0        0        0     6332 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/cfd_stl_export.py
--rw-r--r--   0        0        0     6195 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/courtyard_building.py
--rw-r--r--   0        0        0     2300 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/domain.py
--rw-r--r--   0        0        0    10084 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/test_domain_init.stl
--rw-r--r--   0        0        0     1841 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/wall.py
--rw-r--r--   0        0        0       74 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/wall_type.py
--rw-r--r--   0        0        0     1624 2023-05-17 22:23:03.415880 archaea_simulation-1.0.7/archaea_simulation/simulation_objects/zone.py
--rw-r--r--   0        0        0     1871 2023-05-17 22:23:03.567881 archaea_simulation-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1715 1970-01-01 00:00:00.000000 archaea_simulation-1.0.7/setup.py
--rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 archaea_simulation-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/LICENSE
+-rw-r--r--   0        0        0    11357 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/LICENSE.txt
+-rw-r--r--   0        0        0      896 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/README.md
+-rw-r--r--   0        0        0      333 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/__init__.py
+-rw-r--r--   0        0        0     1073 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/0/U
+-rw-r--r--   0        0        0     1214 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/0/epsilon
+-rw-r--r--   0        0        0     1181 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/0/k
+-rw-r--r--   0        0        0     1058 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/0/nut
+-rw-r--r--   0        0        0     1051 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/0/p
+-rwxr-xr-x   0        0        0      252 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/Allclean
+-rwxr-xr-x   0        0        0      347 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/Allrun
+-rw-r--r--   0        0        0      757 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/constant/momentumTransport
+-rw-r--r--   0        0        0      724 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/constant/transportProperties
+-rw-r--r--   0        0        0     1359 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/system/blockMeshDict
+-rw-r--r--   0        0        0     1060 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/system/controlDict
+-rw-r--r--   0        0        0     1356 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/system/fvSchemes
+-rw-r--r--   0        0        0     1411 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/system/fvSolution
+-rw-r--r--   0        0        0      762 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/system/meshQualityDict
+-rw-r--r--   0        0        0     1852 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/system/snappyHexMeshDict
+-rw-r--r--   0        0        0     1061 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/case/system/surfaceFeaturesDict
+-rw-r--r--   0        0        0        0 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/simulation_objects/__init__.py
+-rw-r--r--   0        0        0     6836 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/simulation_objects/cfd_stl_export.py
+-rw-r--r--   0        0        0     6306 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/simulation_objects/courtyard_building.py
+-rw-r--r--   0        0        0     5875 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/simulation_objects/domain.py
+-rw-r--r--   0        0        0     1841 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/simulation_objects/wall.py
+-rw-r--r--   0        0        0       74 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/simulation_objects/wall_type.py
+-rw-r--r--   0        0        0     1624 2023-05-17 22:31:17.954642 archaea_simulation-1.0.8/archaea_simulation/simulation_objects/zone.py
+-rw-r--r--   0        0        0     1871 2023-05-17 22:31:18.110643 archaea_simulation-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 archaea_simulation-1.0.8/setup.py
+-rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 archaea_simulation-1.0.8/PKG-INFO
```

### Comparing `archaea_simulation-1.0.7/LICENSE` & `archaea_simulation-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `archaea_simulation-1.0.7/LICENSE.txt` & `archaea_simulation-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `archaea_simulation-1.0.7/README.md` & `archaea_simulation-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `archaea_simulation-1.0.7/archaea_simulation/simulation_objects/cfd_stl_export.py` & `archaea_simulation-1.0.8/archaea_simulation/simulation_objects/cfd_stl_export.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import sys
+import os
 import getopt
+from archaea.geometry.point3d import Point3d
 from archaea_simulation.simulation_objects.domain import Domain
 from archaea_simulation.simulation_objects.courtyard_building import CourtyardBuilding
-from archaea.geometry.point3d import Point3d
 
 
 def cfd_stl_export(argv):
     # Default values
+    arg_name = "test"
     arg_domain_width = 50.0
     arg_domain_depth = 100.0
     arg_domain_height = 50.0
     arg_number_of_storeys = 1
     arg_number_of_rooms = 3
     arg_courtyard_width = 10.0
     arg_room_width = 4.0
@@ -23,14 +25,15 @@
     arg_room_door_existence = 1
     arg_room_door_width = 0.8
     arg_room_door_height = 2.0
 
     arg_help = "{0}\n\n" \
                "Welcome to stl exporter program for cfd calculations! \n" \
                "Use below flags to generate stl.\n" \
+               " -n\t--name                        <name>                    default: test\n" \
                " -dw\t--domain-width               <domain_width>            default: 100.0\n" \
                " -dd\t--domain-depth               <domain_depth>            default: 50.0\n" \
                " -dh\t--domain-height              <domain_height>           default: 50.0\n" \
                " -nos\t--number-of-storeys         <number_of_storeys>        default: 1\n" \
                " -nor\t--number-of-rooms           <number_of_rooms>          default: 3\n" \
                " -cw\t--courtyard-width            <courtyard_width>         default: 10.0\n" \
                " -rw\t--room-width                 <room_width>              default: 4.0\n" \
@@ -41,16 +44,17 @@
                " -rww\t--room-window-width         <room_window_width>        default: 0.6\n" \
                " -rwh\t--room-window-height        <room_window_height>       default: 1.2\n" \
                " -rde\t--room-door-existence       <room_door_existence>      default: 1\n" \
                " -rdw\t--room-door-width           <room_door_width>          default: 0.8\n" \
                " -rdh\t--room-door-height          <room_door_height>         default: 2.0\n".format(argv[0])
 
     try:
-        opts, args = getopt.getopt(argv[1:], "hdw:dd:dh:nos:nor:cw:rw:rd:rh:rwt:rwe:rww:rwh:rde:rdw:rdh:",
+        opts, args = getopt.getopt(argv[1:], "n:hdw:dd:dh:nos:nor:cw:rw:rd:rh:rwt:rwe:rww:rwh:rde:rdw:rdh:",
                                    ["help",
+                                    "name=",
                                     "domain-width=",
                                     "domain-depth=",
                                     "domain-height=",
                                     "number-of-storeys=",
                                     "number-of-rooms=",
                                     "courtyard-width=",
                                     "room-width=",
@@ -73,19 +77,21 @@
         print("NOTE: Stl generated with default parameters because no argument provided.\n")
 
     # Find the upcoming flag and set it to it's value
     for opt, arg in opts:
         if opt in ("-h", "--help"):
             print(arg_help)  # print the help message
             sys.exit(2)
+        elif opt in ("-n", "--name"):
+            arg_name = arg
         elif opt in ("-dw", "--domain-width"):
             arg_domain_width = arg
-        elif opt in ("-dd", "--domain_depth"):
+        elif opt in ("-dd", "--domain-depth"):
             arg_domain_depth = arg
-        elif opt in ("-dh", "--domain_height"):
+        elif opt in ("-dh", "--domain-height"):
             arg_domain_height = arg
         elif opt in ("-nos", "--number-of-storeys"):
             arg_number_of_storeys = arg
         elif opt in ("-nor", "--number-of-rooms"):
             arg_number_of_rooms = arg
         elif opt in ("-cw", "--courtyard-width"):
             arg_courtyard_width = arg
@@ -124,20 +130,26 @@
         float(arg_room_window_height),
         bool(arg_room_door_existence),
         float(arg_room_door_width),
         float(arg_room_door_height)
     )
 
     domain = Domain(Point3d.origin(),
-                    arg_domain_width,       # x
-                    arg_domain_depth,       # y
-                    arg_domain_height       # z
+                    float(arg_domain_width),       # x
+                    float(arg_domain_depth),       # y
+                    float(arg_domain_height)       # z
                     )
 
     for zone in courtyard_building.zones:
         domain.add_zone(zone)
 
-    domain.export_domain_to_stl()
+    foam_run = os.getenv('FOAM_RUN')
+    # TODO: check here foam_run exist or not
+    archaea_folder = os.path.join(foam_run, 'archaea')
+    if not os.path.exists(archaea_folder):
+        os.mkdir(archaea_folder)
+
+    domain.create_case(os.path.join(archaea_folder, arg_name))
 
 
 if __name__ == "__main__":
     cfd_stl_export(sys.argv)
```

### Comparing `archaea_simulation-1.0.7/archaea_simulation/simulation_objects/courtyard_building.py` & `archaea_simulation-1.0.8/archaea_simulation/simulation_objects/courtyard_building.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,17 @@
         p0 = Point3d(c.x + x_shift, c.y + y_shift, c.z)
         p1 = Point3d(c.x + x_shift, c.y + y_shift + self.room_depth, c.z)
         p2 = Point3d(c.x + x_shift - self.room_width, c.y + y_shift + self.room_depth, c.z)
         p3 = Point3d(c.x + x_shift - self.room_width, c.y + y_shift, c.z)
 
         ground_loop_1 = Loop([p0, p3, p2, p1])
         ground_face_1 = Face(ground_loop_1)
-        ground_wall = Wall(ground_loop_1, [], wall_type=WallType.INNER)
+
+        # NOTE: If we want to open ground of storey 1, we should change wall_type to wall_type=WallType.INNER
+        ground_wall = Wall(ground_loop_1, [], wall_type=WallType.OUTER)
         ceiling_wall = Wall(ground_loop_1.move(Vector3d(0, 0, self.room_height)).reverse(), [], wall_type=WallType.OUTER)
 
         window_wall = self.create_window_wall(p0, p3)
 
         door_wall = self.create_door_wall(p2, p1)
 
         side_wall_1_type = WallType.OUTER
```

### Comparing `archaea_simulation-1.0.7/archaea_simulation/simulation_objects/wall.py` & `archaea_simulation-1.0.8/archaea_simulation/simulation_objects/wall.py`

 * *Files identical despite different names*

### Comparing `archaea_simulation-1.0.7/archaea_simulation/simulation_objects/zone.py` & `archaea_simulation-1.0.8/archaea_simulation/simulation_objects/zone.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     height: float
     volume: float
     wall_default_thickness: float
     openings: "list[Face]"
 
     def __init__(self, floor: Face, height, walls=None, wall_default_thickness=0.1):
         self.floor = Wall(floor.outer_loop, floor.inner_loops)
-        self.floor.update_wall_type(WallType.INNER)
+        self.floor.update_wall_type(WallType.OUTER)
         self.height = height
         self.wall_default_thickness = wall_default_thickness
         self.volume = self.floor.area * height
         move_vector = Vector3d(0, 0, self.height)
         self.ceiling = self.floor.move(move_vector).reverse()
         if walls is None:
             self.create_walls(move_vector)
```

### Comparing `archaea_simulation-1.0.7/pyproject.toml` & `archaea_simulation-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archaea-simulation"
-version = "1.0.7"
+version = "1.0.8"
 description = "Wrapper definitions for simulation tools."
 readme = "README.md"
 authors = ["Oğuzhan Koral <oguzhankoral@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/archaeans/archaea-simulation"
 keywords = ["geometry", "simulation"]
 classifiers = [
```

### Comparing `archaea_simulation-1.0.7/setup.py` & `archaea_simulation-1.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 package_dir = \
 {'': '.'}
 
 packages = \
 ['archaea_simulation', 'archaea_simulation.simulation_objects']
 
 package_data = \
-{'': ['*']}
+{'': ['*'],
+ 'archaea_simulation': ['case/*',
+                        'case/0/*',
+                        'case/constant/*',
+                        'case/system/*']}
 
 install_requires = \
 ['archaea>=1.1.13,<2.0.0']
 
 setup_kwargs = {
     'name': 'archaea-simulation',
-    'version': '1.0.7',
+    'version': '1.0.8',
     'description': 'Wrapper definitions for simulation tools.',
     'long_description': "# Archaea Simulation\n\nWrapper definitions for simulation tools.\n\nMotivation of creating this library is started with master thesis, departments of Computational\nScience and Engineering and Architecture at Istanbul Technical University. \nAim of thesis is to create scenarios for different environmental\nsolvers like EnergyPlus and OpenFOAM to run them parallely on Linux environment.\nPreparation of these scenario files done by geometric [Archaea](https://github.com/archaeans/archaea) library.\n\n\n## Focused Simulation Tools\n\n- OpenFOAM: OpenFOAM requires stl geometries to run it's solvers\nbehind the scenes. (Pre-Alpha)\n- EnergyPlus: EnergyPlus requires idf schema to run simulations. (MVP)\n- UWG: Urban weather generator is a solver to calculate effects on urban microclimate.\nIt creates new .epw file for EnergyPlus simulations.\n\nMain idea behind this work is to be experimental and didactic. ",
     'author': 'Oğuzhan Koral',
     'author_email': 'oguzhankoral@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/archaeans/archaea-simulation',
```

### Comparing `archaea_simulation-1.0.7/PKG-INFO` & `archaea_simulation-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archaea-simulation
-Version: 1.0.7
+Version: 1.0.8
 Summary: Wrapper definitions for simulation tools.
 Home-page: https://github.com/archaeans/archaea-simulation
 License: Apache-2.0
 Keywords: geometry,simulation
 Author: Oğuzhan Koral
 Author-email: oguzhankoral@gmail.com
 Requires-Python: >=3.8,<4.0
```

