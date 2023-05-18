# Comparing `tmp/br2-0.0.2.tar.gz` & `tmp/br2-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/br2-0.0.2.tar", last modified: Thu Mar 17 21:44:41 2022, max compression
+gzip compressed data, was "br2-0.1.0.tar", max compression
```

## Comparing `br2-0.0.2.tar` & `br2-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,13 @@
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-03-17 21:44:41.289403 br2-0.0.2/
--rw-r--r--   0 skim0119   (501) staff       (20)     5204 2022-03-17 21:44:41.288991 br2-0.0.2/PKG-INFO
--rw-r--r--   0 skim0119   (501) staff       (20)     3574 2022-03-17 04:44:56.000000 br2-0.0.2/README.md
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-03-17 21:44:41.286515 br2-0.0.2/br2/
--rw-r--r--   0 skim0119   (501) staff       (20)        0 2022-03-17 01:02:58.000000 br2-0.0.2/br2/__init__.py
--rw-r--r--   0 skim0119   (501) staff       (20)     2624 2022-03-16 19:34:38.000000 br2-0.0.2/br2/custom_activation.py
--rw-r--r--   0 skim0119   (501) staff       (20)     3161 2022-03-16 19:09:30.000000 br2-0.0.2/br2/custom_constraint.py
--rw-r--r--   0 skim0119   (501) staff       (20)    14913 2022-03-17 09:02:25.000000 br2-0.0.2/br2/environment.py
--rw-r--r--   0 skim0119   (501) staff       (20)     8224 2022-03-17 08:47:00.000000 br2-0.0.2/br2/free_custom_systems.py
--rw-r--r--   0 skim0119   (501) staff       (20)    16410 2022-03-17 02:35:58.000000 br2-0.0.2/br2/free_simulator.py
--rw-r--r--   0 skim0119   (501) staff       (20)    18622 2021-11-08 18:01:24.000000 br2-0.0.2/br2/post_processing.py
--rw-r--r--   0 skim0119   (501) staff       (20)    17333 2022-03-17 01:08:15.000000 br2-0.0.2/br2/surface_connection_parallel_rod_numba.py
--rw-r--r--   0 skim0119   (501) staff       (20)       18 2022-03-17 21:44:34.000000 br2-0.0.2/br2/version.py
-drwxr-xr-x   0 skim0119   (501) staff       (20)        0 2022-03-17 21:44:41.288416 br2-0.0.2/br2.egg-info/
--rw-r--r--   0 skim0119   (501) staff       (20)     5204 2022-03-17 21:44:40.000000 br2-0.0.2/br2.egg-info/PKG-INFO
--rw-r--r--   0 skim0119   (501) staff       (20)      369 2022-03-17 21:44:40.000000 br2-0.0.2/br2.egg-info/SOURCES.txt
--rw-r--r--   0 skim0119   (501) staff       (20)        1 2022-03-17 21:44:40.000000 br2-0.0.2/br2.egg-info/dependency_links.txt
--rw-r--r--   0 skim0119   (501) staff       (20)       53 2022-03-17 21:44:40.000000 br2-0.0.2/br2.egg-info/requires.txt
--rw-r--r--   0 skim0119   (501) staff       (20)        4 2022-03-17 21:44:40.000000 br2-0.0.2/br2.egg-info/top_level.txt
--rw-r--r--   0 skim0119   (501) staff       (20)       38 2022-03-17 21:44:41.289514 br2-0.0.2/setup.cfg
--rw-r--r--   0 skim0119   (501) staff       (20)     3653 2022-03-17 04:16:31.000000 br2-0.0.2/setup.py
+-rw-r--r--   0        0        0     1058 2023-05-17 20:59:58.460813 br2-0.1.0/LICENSE
+-rw-r--r--   0        0        0      931 2022-03-18 22:53:27.879616 br2-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2022-03-17 01:02:58.517375 br2-0.1.0/br2/__init__.py
+-rw-r--r--   0        0        0     2624 2022-03-16 19:34:38.406421 br2-0.1.0/br2/custom_activation.py
+-rw-r--r--   0        0        0     3161 2022-03-16 19:09:30.151571 br2-0.1.0/br2/custom_constraint.py
+-rw-r--r--   0        0        0    15137 2023-05-18 14:17:20.055468 br2-0.1.0/br2/environment.py
+-rw-r--r--   0        0        0     7989 2023-05-18 15:13:26.835489 br2-0.1.0/br2/free_custom_systems.py
+-rw-r--r--   0        0        0    16545 2023-05-18 15:19:35.275102 br2-0.1.0/br2/free_simulator.py
+-rw-r--r--   0        0        0    18570 2023-05-18 14:07:47.745249 br2-0.1.0/br2/post_processing.py
+-rw-r--r--   0        0        0    17501 2023-05-18 02:06:18.266193 br2-0.1.0/br2/surface_connection_parallel_rod_numba.py
+-rw-r--r--   0        0        0       18 2022-03-17 21:44:34.971236 br2-0.1.0/br2/version.py
+-rw-r--r--   0        0        0      748 2023-05-18 14:20:36.808881 br2-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 br2-0.1.0/PKG-INFO
```

### Comparing `br2-0.0.2/br2/custom_activation.py` & `br2-0.1.0/br2/custom_activation.py`

 * *Files identical despite different names*

### Comparing `br2-0.0.2/br2/custom_constraint.py` & `br2-0.1.0/br2/custom_constraint.py`

 * *Files identical despite different names*

### Comparing `br2-0.0.2/br2/environment.py` & `br2-0.1.0/br2/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Optional, Union
 
 import os
 import copy
 import time
+import logging
 
 from dataclasses import dataclass
 
 from tqdm import tqdm
 
 import numpy as np
 
@@ -194,15 +195,15 @@
         """
 
         assert os.path.exists(rod_database_path), "Rod database path does not exists."
         assert os.path.exists(
             assembly_config_path
         ), "Assembly configuration does not exists."
 
-        self.assy = FreeAssembly(**kwargs)
+        self.assy = FreeAssembly(self, **kwargs)
 
         """rod name -> [seg,rod]"""
         self.shearable_rods = self.assy.build(rod_database_path, assembly_config_path)
         self.simulator = self.assy.simulator
 
         # Collect data using callback function for postprocessing
         # set the diagnostics for rod and collect data
@@ -262,22 +263,23 @@
             # fmt: on
 
         # Simulation
         time = self.time
         if not duration:
             duration = self.time_step
         with tqdm(
-            total=duration, mininterval=0.5, disable=disable_progress_bar
+            total=self.time + duration, mininterval=0.5, disable=disable_progress_bar,
+            bar_format = "{desc}: {percentage:.3f}%|{bar}| {n:.5f}/{total_fmt} [{elapsed}<{remaining}"
         ) as pbar:
             while time < self.time + duration:
                 time = self.do_step(
                     self.StatefulStepper,
                     self.stages_and_updates,
                     self.simulator,
-                    self.time,
+                    time,
                     self.time_step,
                 )
                 pbar.update(self.time_step)
         self.time = time
 
         # Check steady state
         if check_steady_state == 1:
@@ -390,26 +392,29 @@
     ) -> None:
         """
         Make video 3D rod movement in time.
         """
 
         filename_video = "br2_simulation"
         save_folder = self.paths.renderings
+        if not os.path.exists(save_folder):
+            os.makedirs(save_folder)
+        else:
+            logging.warning("The folder already exists. The data will be overwritten.")
 
         plot_video_with_surface(
             self.data_rods,
             video_name=filename_video,
             fps=self.rendering_fps,
             step=1,
             save_folder=save_folder,
             **kwargs,
         )
 
-        position_data_path = os.path.join(save_folder, f"br2_data_{data_tag}.npz")
-        self.save_data(position_data_path)
+        self.save_data("position")
 
     def save_data(self, tag:Optional[str]=None) -> None:
         """save_data.
 
         Parameters
         ----------
         tag : Optional[str]
```

### Comparing `br2-0.0.2/br2/free_custom_systems.py` & `br2-0.1.0/br2/free_custom_systems.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,43 +13,43 @@
 import numba
 from numba import njit
 
 # Defining Variable Bending
 class FreeBendActuation(NoForces):
     # TODO
 
-    def __init__(self, actuation_ref, z_angle, scale, ramp_up_time=1.0):
+    def __init__(self, actuation_ref, z_angle, scale, ramp_up_time=0.2):
         super(FreeBendActuation, self).__init__()
         self.actuation_ref = actuation_ref
         self.z_angle = z_angle
         self.magnitude_scale = scale # TODO
         '''
         Currently we are using scale to externally compute the moment scale.
         We are assuming the radius is not changing as it deform.
         If we want to incorporate the change in radius, we cannot use default
         CR radius, since the basic CR is implemented assuming solid cylinder
         '''
         self.ramp_up_time = ramp_up_time
 
     ''' (deprecated)
-    def apply_forces(self, system, time: np.float = 0.0):
+    def apply_forces(self, system, time: float = 0.0):
         factor = min(1.0, time / self.ramp_up_time)
         force_on_one_element = self.actuation_ref[0] * factor
         tangents = system.tangents[...]
         system.external_forces[..., 0] -= factor * 0.5 * force_on_one_element * tangents[..., 0]
         system.external_forces[..., -1] += factor * 0.5 * force_on_one_element * tangents[..., -1]
         system.external_forces[..., 1:-1] += (
             factor * 0.5 * force_on_one_element
             * (tangents[..., :-1] - tangents[..., 1:])
         )
     '''
 
-    def apply_torques(self, system, time: np.float = 0.0):
-        factor = min(1.0, time / self.ramp_up_time) # Not sure
-        torque_mag = self.actuation_ref[0] * self.magnitude_scale # * factor
+    def apply_torques(self, system, time: float = 0.0):
+        factor = min(1.0, time / self.ramp_up_time)
+        torque_mag = self.actuation_ref[0] * self.magnitude_scale * factor
         local_unit_vector = np.array([np.cos(self.z_angle),
                                       np.sin(self.z_angle),
                                       0.0
                                       ])
         torque = torque_mag * local_unit_vector
         system.external_torques[...,-1] += torque
         #system.external_torques[...,-1] += system.director_collection[...,-1] @ torque
@@ -64,54 +64,49 @@
         )
 
 
 # Defining Variable Torque
 class FreeTwistActuation(NoForces):
     # TODO
 
-    def __init__(self, actuation_ref, scale, ramp_up_time=1.0):
+    def __init__(self, actuation_ref, scale, ramp_up_time=0.2):
         """
 
         Parameters
         ----------
         actuation_ref: list
         scale: float
         """
         super(FreeTwistActuation, self).__init__()
         self.actuation_ref = actuation_ref
         self.direction = np.array([0.0, 0.0, 1.0]) # Rod always in tangent
         self.scale = scale
         self.ramp_up_time = ramp_up_time
 
     '''
-    def apply_forces(self, system, time: np.float = 0.0):
+    def apply_forces(self, system, time: float = 0.0):
         factor = min(1.0, time / self.ramp_up_time)
         force_on_one_element = self.torque[0] / 3.14742e-2 * factor # TODO: double check the ratio
         tangents = system.tangents[...]
         system.external_forces[..., 0] -= factor * 0.5 * force_on_one_element * tangents[..., 0]
         system.external_forces[..., -1] += factor * 0.5 * force_on_one_element * tangents[..., -1]
         system.external_forces[..., 1:-1] += (
             factor * 0.5 * force_on_one_element
             * (tangents[..., :-1] - tangents[..., 1:])
         )
     '''
 
-    def apply_torques(self, system, time: np.float = 0.0):
-        #factor = min(1.0, time / self.ramp_up_time)
-        torque = self.actuation_ref[0] * self.scale * self.direction #* factor
+    def apply_torques(self, system, time: float = 0.0):
+        factor = min(1.0, time / self.ramp_up_time)
+        torque = self.actuation_ref[0] * self.scale * self.direction * factor
         n_elems = system.n_elems
         torques = (
             _batch_product_i_k_to_ik(torque, np.ones((n_elems))) / n_elems
         )
         system.external_torques += torques
-        '''
-        system.external_torques += _batch_matvec(
-            system.director_collection, torque_on_one_element
-        )
-        '''
 
 class FreeBaseEndSoftFixed(ConstraintBase):
 
     def __init__(self, fixed_position, fixed_directors, k, nu, kt, **kwargs):
         """
         Parameters
         ----------
@@ -128,15 +123,14 @@
         self.kt = kt
 
         # Accumulated rotation
         self.rev = 0
 
     def constrain_values(self, rod, time):
         super().constrain_values(rod, time)
-        #rod.position_collection[...,0] = self.fixed_position
         self.restrict_position(
             rod.position_collection[...,0],
             self.fixed_position,
             rod.velocity_collection[...,0],
             rod.external_forces,
             self.k,
             self.nu,
```

### Comparing `br2-0.0.2/br2/free_simulator.py` & `br2-0.1.0/br2/free_simulator.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     FreeTwistActuation,
     FreeBaseEndSoftFixed
 )
 
 
 
 # Set base elastica simulator class
-class BR2Simulator(BaseSystemCollection, Constraints, Connections, Forcing, CallBacks):
+class BR2Simulator(BaseSystemCollection, Constraints, Connections, Forcing, Damping, CallBacks):
     pass
 
 
 class FreeCallback(CallBackBaseClass):
     def __init__(self, step_skip: int, callback_params: dict, time_interval=None):
         CallBackBaseClass.__init__(self)
         self.every = step_skip
@@ -59,29 +59,33 @@
         self.callback_params["external_forces"].append( system.external_forces.copy() )
         self.callback_params["external_torques"].append( system.external_torques.copy() )
         self.callback_params["internal_forces"].append( system.internal_forces.copy() )
         self.callback_params["internal_torques"].append( system.internal_torques.copy() )
         self.callback_params["lengths"].append(system.lengths.copy())
         self.callback_params["dilatation"].append(system.dilatation.copy())
         self.callback_params["radius"].append(system.radius.copy())
+        self.callback_params["com"].append(system.compute_position_center_of_mass())
+        #self.callback_params["vcom"].append(system.compute_velocity_center_of_mass())
 
 
 class FreeAssembly:
-    def __init__(self, gravity=False, **kwargs):
+    def __init__(self, env, gravity=False, **kwargs):
+        self.env = env
+
         self.simulator = BR2Simulator()
         self.actuation = defaultdict(list)
         self.free = {}  # Key: <segment name>_<order>_<rod name>
 
         # Parameter
         self.toggle_gravity = gravity
 
         ## Debut
-        self.k_multiplier = kwargs.get('t_multiplier', 1) * 1.0e-2
+        self.k_multiplier = kwargs.get('t_multiplier', 1) #* 1.0e-2
         self.nu_multiplier = kwargs.get('nu_multiplier', 1) * 1.0e-3
-        self.kt_multiplier = kwargs.get('kt_multiplier', 1) * 0.0 #1e0
+        self.kt_multiplier = kwargs.get('kt_multiplier', 1) #* 0.0 #1e0
 
     def save_state(self, **kwargs):
         # kwargs: directory, time, verbose
         save_state(self.simulator, **kwargs)
 
     def load_state(self, **kwargs):
         # kwargs: directory, verbose
@@ -163,22 +167,21 @@
                 seg_rods.append(rod_name)
             assert seg_lengths.count(seg_lengths[0]) == len(seg_lengths), "rods' lengths should all be the same within a segment"
             assert seg_n_elements.count(seg_n_elements[0]) == len(seg_n_elements), "rods' number of elements should all be the same within a segment"
             start_y_position += seg_lengths[0]
 
             '''Parallel Connection'''
             print("connecting in parallel...")
-            # TODO: I do not know what these terms are for, conceivably for the coupling of the arms
             outer_radius = rod_spec['outer_radius']
             base_length = rod_spec['base_length']
             E = rod_spec['youngs_modulus']
             n_elem = rod_spec['n_elements']
-            k_connection = np.pi * outer_radius * E / n_elem * self.k_multiplier  # 50  # 1e5
+            k_connection = np.pi * outer_radius * E / n_elem * self.k_multiplier
             nu_connection = base_length / n_elem * self.nu_multiplier
-            kt_connection = outer_radius / 2 * self.kt_multiplier  # 1e-3
+            kt_connection = outer_radius / 2 * self.kt_multiplier
             #print(f'  {k_connection=} {nu_connection=} {kt_connection=}')
             for rod_i in range(len(seg_rods)):
                 first_rod_name = seg_rods[rod_i-1]
                 second_rod_name = seg_rods[rod_i]
                 print(f"    connecting seg {seg_idx}: {first_rod_name} || {second_rod_name}")
                 self.add_parallel_connection(first_rod_name,
                                              second_rod_name,
@@ -248,14 +251,23 @@
         rod.outer_radius = rod_spec['outer_radius']
         rod.inner_radius = rod_spec['inner_radius']
         self.free[name] = rod
 
         # Append rod to simulator
         self.simulator.append(rod)
 
+        # add damping
+        if "damping_constant" in rod_spec:
+            damping_constant = rod_spec["damping_constant"]
+            self.simulator.dampen(rod).using(
+                AnalyticalLinearDamper,
+                damping_constant=damping_constant,
+                time_step=self.env.time_step,
+            )
+
         # Constrain one end of the rod (TODO : Modify for serial connection)
         if is_first_segment:
             self.simulator.constrain(rod).using(
                 FreeBaseEndSoftFixed, constrained_position_idx=(0,), constrained_director_idx=(0,),
                 k=1e9, nu=0, kt=0.0
             )
 
@@ -264,32 +276,24 @@
             self.simulator.add_forcing_to(rod).using(
                 GravityForces,
                 acc_gravity=np.array([0., 9.80665, 0.])  # Reverse direction
             )
 
         return rod
 
-    def add_alpha_fibers(self, rod, actuation_ref, fiber_angles:list):
+    def add_angled_fibers(self, rod, actuation_ref, fiber_angles:list):
         for alpha in fiber_angles:
             angle = alpha * np.pi / 180
             scale = np.pi * (rod.inner_radius**3) * ((np.sin(angle)**2) + 2*(np.cos(angle)**2)) / (np.sin(2*angle))
             self.simulator.add_forcing_to(rod).using(
                 FreeTwistActuation,
                 actuation_ref,
                 scale=scale
             )
 
-    def add_beta_fibers(self, rod, actuation_ref, fiber_angles: list):
-        for beta in fiber_angles:
-            self.simulator.add_forcing_to(rod).using(
-                FreeTwistActuation,
-                actuation_ref,
-                scale=beta * np.pi / 180
-            )
-
     def add_straight_fibers(self, rod, actuation_ref, fiber_angles: list):
         scale = np.pi * rod.radius[-1] * (rod.inner_radius**2)
         for gamma in fiber_angles:
             self.simulator.add_forcing_to(rod).using(
                 FreeBendActuation,
                 actuation_ref,
                 z_angle=gamma * np.pi / 180.0,
@@ -299,16 +303,16 @@
     def add_free(self, name, actuation_name, alpha=[], beta=[], gamma=[], **rod_spec):
         # Create rod
         rod = self.create_rod(name, **rod_spec)
         actuation_ref = self.get_actuation_reference(actuation_name)
 
         # Add fiber
         if actuation_ref is not None:
-            self.add_alpha_fibers(rod, actuation_ref, alpha)
-            self.add_beta_fibers(rod, actuation_ref, beta)
+            self.add_angled_fibers(rod, actuation_ref, alpha)
+            self.add_angled_fibers(rod, actuation_ref, beta)
             self.add_straight_fibers(rod, actuation_ref, gamma)
 
         return rod
 
     def add_parallel_connection(self, name1, name2, **param):
         rod1 = self.free[name1]
         rod2 = self.free[name2]
```

### Comparing `br2-0.0.2/br2/post_processing.py` & `br2-0.1.0/br2/post_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib.colors import to_rgb
+import matplotlib.animation as animation
 from mpl_toolkits.mplot3d import proj3d, Axes3D
 #from tqdm import tqdm
 
 from typing import Dict, Sequence
 
+#plt.rcParams.update({"font.size": 22})
+
 def tqdm(obj): # tqdm suppressor
     return obj
 
 def plot_video_2d(
     plot_params1: dict, plot_params2: dict, video_name="video.mp4", margin=0.2, fps=40
 ):  # (time step, x/y/z, node)
     import matplotlib.animation as manimation
@@ -62,31 +65,27 @@
     video_name="video",
     fps=60,
     step=1,
     save_folder="",
     vis2D=True,
     **kwargs,
 ):
-    #plt.rcParams.update({"font.size": 22})
-
-    # 2d case <always 2d case for now>
-    import matplotlib.animation as animation
 
     # simulation time
     sim_time = np.array(rods_history[0]["time"])
 
     # Rod
     n_visualized_rods = len(rods_history)  # should be one for now
     # Rod info
-    rod_history_unpacker = lambda rod_idx, t_idx: (
-        rods_history[rod_idx]["position"][t_idx],
-        rods_history[rod_idx]["radius"][t_idx],
-    )
+    def rod_history_unpacker(rod_idx, t_idx):
+        return rods_history[rod_idx]["position"][t_idx], rods_history[rod_idx]["radius"][t_idx]
+
     # Rod center of mass
-    com_history_unpacker = lambda rod_idx, t_idx: rods_history[rod_idx]["com"][time_idx]
+    def com_history_unpacker(rod_idx, t_idx):
+        return rods_history[rod_idx]["com"][t_idx]
 
     # video pre-processing
     #print("plot scene visualization video")
     FFMpegWriter = animation.writers["ffmpeg"]
     metadata = dict(title="Movie Test", artist="Matplotlib", comment="Movie support!")
     writer = FFMpegWriter(fps=fps, metadata=metadata)
     dpi = kwargs.get("dpi", 100)
```

### Comparing `br2-0.0.2/br2/surface_connection_parallel_rod_numba.py` & `br2-0.1.0/br2/surface_connection_parallel_rod_numba.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from elastica.joint import FreeJoint
 from elastica.utils import Tolerance
 
 # Join the two rods
 from elastica._linalg import _batch_norm, _batch_cross, _batch_matvec, _batch_dot, _batch_matmul, _batch_matrix_transpose
 from elastica.interaction import (
     elements_to_nodes_inplace,
-    node_to_element_pos_or_vel,
+    node_to_element_position,
+    node_to_element_velocity,
 )
 
 from elastica._rotations import _inv_skew_symmetrize
 
 @njit(cache=True)
 def _single_get_rotation_matrix(theta:float, unit_axis):
     rot_mat = np.empty((3, 3))
@@ -131,14 +132,16 @@
     # Apply force is same as free joint
     def apply_forces(self, rod_one, index_one, rod_two, index_two):
         # TODO: documentation
 
         self.rod_one_rd2, self.rod_two_rd2, self.spring_force = self._apply_forces(
             self.k,
             self.nu,
+            rod_one.mass,
+            rod_two.mass,
             self.rd1_local,
             self.rd2_local,
             rod_one.position_collection,
             rod_two.position_collection,
             rod_one.radius[None,:],
             rod_two.radius[None,:],
             rod_one.velocity_collection,
@@ -152,14 +155,16 @@
         )
 
     @staticmethod
     @njit(cache=True)
     def _apply_forces(
         k,
         nu,
+        rod_one_mass,
+        rod_two_mass,
 		rod_one_rd2_local,
 		rod_two_rd2_local,
         rod_one_position_collection,
         rod_two_position_collection,
         rod_one_radius,
         rod_two_radius,
         rod_one_velocity_collection,
@@ -168,18 +173,18 @@
         rod_two_director_collection,
         rod_one_tangents,
         rod_two_tangents,
         rod_one_external_forces,
         rod_two_external_forces,
     ):
         # Compute element positions
-        rod_one_element_position = node_to_element_pos_or_vel(
+        rod_one_element_position = node_to_element_position(
             rod_one_position_collection
         )
-        rod_two_element_position = node_to_element_pos_or_vel(
+        rod_two_element_position = node_to_element_position(
             rod_two_position_collection
         )
 
         # Compute vector r*d2 (radius * normal vector) for each rod and element
         rod_one_rd2 = _batch_matvec(
 				_batch_matrix_transpose(rod_one_director_collection),
                 rod_one_rd2_local * rod_one_radius
@@ -193,18 +198,20 @@
 
         # Compute spring force between two rods using Fc=k*epsilon
         distance_vector = rod_two_surface_position - rod_one_surface_position
         distance = _batch_norm(distance_vector)
         spring_force = k * (distance_vector)
 
         # Damping force
-        rod_one_element_velocity = node_to_element_pos_or_vel(
+        rod_one_element_velocity = node_to_element_velocity(
+            rod_one_mass,
             rod_one_velocity_collection
         )
-        rod_two_element_velocity = node_to_element_pos_or_vel(
+        rod_two_element_velocity = node_to_element_velocity(
+            rod_two_mass,
             rod_two_velocity_collection
         )
 
         relative_velocity = rod_two_element_velocity - rod_one_element_velocity
 
         normalized_distance_vector = np.zeros((relative_velocity.shape))
```

