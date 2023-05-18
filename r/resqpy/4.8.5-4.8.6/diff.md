# Comparing `tmp/resqpy-4.8.5.tar.gz` & `tmp/resqpy-4.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resqpy-4.8.5.tar", max compression
+gzip compressed data, was "resqpy-4.8.6.tar", max compression
```

## Comparing `resqpy-4.8.5.tar` & `resqpy-4.8.6.tar`

### file list

```diff
@@ -1,198 +1,198 @@
--rw-r--r--   0        0        0     1059 2023-05-14 20:17:35.104948 resqpy-4.8.5/LICENSE
--rw-r--r--   0        0        0     2893 2023-05-14 20:17:35.104948 resqpy-4.8.5/README.md
--rw-r--r--   0        0        0     3227 2023-05-14 20:17:57.559186 resqpy-4.8.5/pyproject.toml
--rw-r--r--   0        0        0      555 2023-05-14 20:17:57.559186 resqpy-4.8.5/resqpy/__init__.py
--rw-r--r--   0        0        0    24782 2023-05-14 20:17:35.116949 resqpy-4.8.5/resqpy/crs.py
--rw-r--r--   0        0        0     1982 2023-05-14 20:17:35.116949 resqpy-4.8.5/resqpy/derived_model/__init__.py
--rw-r--r--   0        0        0     6410 2023-05-14 20:17:35.116949 resqpy-4.8.5/resqpy/derived_model/_add_edges_per_column_property_array.py
--rw-r--r--   0        0        0    20540 2023-05-14 20:17:35.116949 resqpy-4.8.5/resqpy/derived_model/_add_faults.py
--rw-r--r--   0        0        0     6417 2023-05-14 20:17:35.116949 resqpy-4.8.5/resqpy/derived_model/_add_one_blocked_well_property.py
--rw-r--r--   0        0        0     8657 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_add_one_grid_property_array.py
--rw-r--r--   0        0        0     2431 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_add_single_cell_grid.py
--rw-r--r--   0        0        0     5495 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_add_wells_from_ascii_file.py
--rw-r--r--   0        0        0     6037 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_add_zone_by_layer_property.py
--rw-r--r--   0        0        0    11586 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_coarsened_grid.py
--rw-r--r--   0        0        0    10201 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_common.py
--rw-r--r--   0        0        0     3730 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_copy_grid.py
--rw-r--r--   0        0        0    11731 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_drape_to_surface.py
--rw-r--r--   0        0        0    16391 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_extract_box.py
--rw-r--r--   0        0        0    22969 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_extract_box_for_well.py
--rw-r--r--   0        0        0    20325 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_fault_throw_scaling.py
--rw-r--r--   0        0        0     7157 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_gather_ensemble.py
--rw-r--r--   0        0        0    17929 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_interpolated_grid.py
--rw-r--r--   0        0        0     9876 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_local_depth_adjustment.py
--rw-r--r--   0        0        0    20513 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_refined_grid.py
--rw-r--r--   0        0        0     5166 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_tilted_grid.py
--rw-r--r--   0        0        0     4792 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_unsplit_grid.py
--rw-r--r--   0        0        0    18825 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_zonal_grid.py
--rw-r--r--   0        0        0     4358 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/derived_model/_zone_layer_ranges_from_array.py
--rw-r--r--   0        0        0      996 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/fault/__init__.py
--rw-r--r--   0        0        0    29402 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/fault/_gcs_functions.py
--rw-r--r--   0        0        0   109110 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/fault/_grid_connection_set.py
--rw-r--r--   0        0        0      692 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/grid/__init__.py
--rw-r--r--   0        0        0    20689 2023-05-14 20:17:35.120950 resqpy-4.8.5/resqpy/grid/_cell_properties.py
--rw-r--r--   0        0        0    10120 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_connection_sets.py
--rw-r--r--   0        0        0    19936 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_create_grid_xml.py
--rw-r--r--   0        0        0    32064 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_defined_geometry.py
--rw-r--r--   0        0        0    28203 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_extract_functions.py
--rw-r--r--   0        0        0    16516 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_face_functions.py
--rw-r--r--   0        0        0    12236 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_faults.py
--rw-r--r--   0        0        0   127766 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_grid.py
--rw-r--r--   0        0        0     3544 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_grid_types.py
--rw-r--r--   0        0        0      338 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_intervals_info.py
--rw-r--r--   0        0        0      604 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_moved_functions.py
--rw-r--r--   0        0        0     7243 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_pillars.py
--rw-r--r--   0        0        0     5386 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_pixel_maps.py
--rw-r--r--   0        0        0    65440 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_points_functions.py
--rw-r--r--   0        0        0    45761 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_regular_grid.py
--rw-r--r--   0        0        0    19413 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_transmissibility.py
--rw-r--r--   0        0        0     7944 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_write_hdf5_from_caches.py
--rw-r--r--   0        0        0     6147 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_write_nexus_corp.py
--rw-r--r--   0        0        0    13087 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid/_xyz.py
--rw-r--r--   0        0        0     2593 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid_surface/__init__.py
--rw-r--r--   0        0        0    35739 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid_surface/_blocked_well_populate.py
--rw-r--r--   0        0        0    64016 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid_surface/_find_faces.py
--rw-r--r--   0        0        0    26056 2023-05-14 20:17:35.124950 resqpy-4.8.5/resqpy/grid_surface/_grid_skin.py
--rw-r--r--   0        0        0    14379 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/grid_surface/_grid_surface.py
--rw-r--r--   0        0        0    22498 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/grid_surface/_trajectory_intersects.py
--rw-r--r--   0        0        0    39760 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/grid_surface/grid_surface_cuda.py
--rw-r--r--   0        0        0      539 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/lines/__init__.py
--rw-r--r--   0        0        0    11960 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/lines/_common.py
--rw-r--r--   0        0        0    41425 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/lines/_polyline.py
--rw-r--r--   0        0        0    26366 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/lines/_polyline_set.py
--rw-r--r--   0        0        0      378 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/model/__init__.py
--rw-r--r--   0        0        0    30171 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/model/_catalogue.py
--rw-r--r--   0        0        0     2840 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/model/_context.py
--rw-r--r--   0        0        0    34552 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/model/_forestry.py
--rw-r--r--   0        0        0     3371 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/model/_grids.py
--rw-r--r--   0        0        0    14238 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/model/_hdf5.py
--rw-r--r--   0        0        0   103055 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/model/_model.py
--rw-r--r--   0        0        0    23589 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/model/_xml.py
--rw-r--r--   0        0        0      909 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/multi_processing/__init__.py
--rw-r--r--   0        0        0     7301 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/multi_processing/_multiprocessing.py
--rw-r--r--   0        0        0       72 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/multi_processing/wrappers/__init__.py
--rw-r--r--   0        0        0     5952 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/multi_processing/wrappers/blocked_well_mp.py
--rw-r--r--   0        0        0    21156 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/multi_processing/wrappers/grid_surface_mp.py
--rw-r--r--   0        0        0     5793 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/multi_processing/wrappers/mesh_mp.py
--rw-r--r--   0        0        0       84 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/olio/__init__.py
--rw-r--r--   0        0        0     2147 2023-05-14 20:17:35.128951 resqpy-4.8.5/resqpy/olio/ab_toolbox.py
--rw-r--r--   0        0        0     7521 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/base.py
--rw-r--r--   0        0        0    20925 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/box_utilities.py
--rw-r--r--   0        0        0     5935 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/class_dict.py
--rw-r--r--   0        0        0     9489 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/consolidation.py
--rw-r--r--   0        0        0     5177 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/data/build.py
--rw-r--r--   0        0        0   498136 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/data/properties.json
--rw-r--r--   0        0        0    19836 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/dataframe.py
--rw-r--r--   0        0        0      307 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/exceptions.py
--rw-r--r--   0        0        0     1313 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/factors.py
--rw-r--r--   0        0        0    24541 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/fine_coarse.py
--rw-r--r--   0        0        0    27398 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/grid_functions.py
--rw-r--r--   0        0        0    20158 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/intersection.py
--rw-r--r--   0        0        0     8408 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/keyword_files.py
--rw-r--r--   0        0        0    19210 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/load_data.py
--rw-r--r--   0        0        0     6628 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/point_inclusion.py
--rw-r--r--   0        0        0     1103 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/random_seed.py
--rw-r--r--   0        0        0     5441 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/read_nexus_fault.py
--rw-r--r--   0        0        0    17083 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/relperm.py
--rw-r--r--   0        0        0    12189 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/simple_lines.py
--rw-r--r--   0        0        0      760 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/time.py
--rw-r--r--   0        0        0      822 2023-05-14 20:17:35.132951 resqpy-4.8.5/resqpy/olio/trademark.py
--rw-r--r--   0        0        0    61869 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/olio/transmission.py
--rw-r--r--   0        0        0    44768 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/olio/triangulation.py
--rw-r--r--   0        0        0     7324 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/olio/uuid.py
--rw-r--r--   0        0        0    45231 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/olio/vdb.py
--rw-r--r--   0        0        0    46253 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/olio/vector_utilities.py
--rw-r--r--   0        0        0     6185 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/olio/volume.py
--rw-r--r--   0        0        0    26220 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/olio/wellspec_keywords.py
--rw-r--r--   0        0        0     5142 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/olio/write_data.py
--rw-r--r--   0        0        0    19055 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/olio/write_hdf5.py
--rw-r--r--   0        0        0    24925 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/olio/xml_et.py
--rw-r--r--   0        0        0     1824 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/olio/xml_namespaces.py
--rw-r--r--   0        0        0     5709 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/olio/zmap_reader.py
--rw-r--r--   0        0        0     2206 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/__init__.py
--rw-r--r--   0        0        0     2937 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/_utils.py
--rw-r--r--   0        0        0     1685 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/boundary_feature.py
--rw-r--r--   0        0        0     5190 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/boundary_feature_interpretation.py
--rw-r--r--   0        0        0     6186 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/earth_model_interpretation.py
--rw-r--r--   0        0        0    12457 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/fault_interpretation.py
--rw-r--r--   0        0        0     2757 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/fluid_boundary_feature.py
--rw-r--r--   0        0        0     1702 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/frontier_feature.py
--rw-r--r--   0        0        0     4498 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/generic_interpretation.py
--rw-r--r--   0        0        0     3771 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/genetic_boundary_feature.py
--rw-r--r--   0        0        0     8605 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/geobody_boundary_interpretation.py
--rw-r--r--   0        0        0     1836 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/geobody_feature.py
--rw-r--r--   0        0        0     8052 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/geobody_interpretation.py
--rw-r--r--   0        0        0     1739 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/geologic_unit_feature.py
--rw-r--r--   0        0        0     8346 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/horizon_interpretation.py
--rw-r--r--   0        0        0     2697 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/organization_feature.py
--rw-r--r--   0        0        0     5565 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/rock_fluid_unit_feature.py
--rw-r--r--   0        0        0     1802 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/structural_organization_interpretation.py
--rw-r--r--   0        0        0     2675 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/tectonic_boundary_feature.py
--rw-r--r--   0        0        0     1843 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/wellbore_feature.py
--rw-r--r--   0        0        0     6973 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/organize/wellbore_interpretation.py
--rw-r--r--   0        0        0     2155 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/property/__init__.py
--rw-r--r--   0        0        0    16697 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/property/_collection_add_part.py
--rw-r--r--   0        0        0    13021 2023-05-14 20:17:35.136952 resqpy-4.8.5/resqpy/property/_collection_create_xml.py
--rw-r--r--   0        0        0    30121 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/property/_collection_get_attributes.py
--rw-r--r--   0        0        0     5368 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/property/_collection_support.py
--rw-r--r--   0        0        0    24426 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/property/_property.py
--rw-r--r--   0        0        0    66946 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/property/grid_property_collection.py
--rw-r--r--   0        0        0   143259 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/property/property_collection.py
--rw-r--r--   0        0        0    36127 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/property/property_common.py
--rw-r--r--   0        0        0     5557 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/property/property_kind.py
--rw-r--r--   0        0        0     7737 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/property/string_lookup.py
--rw-r--r--   0        0        0     1077 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/property/well_interval_property.py
--rw-r--r--   0        0        0     1577 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/property/well_interval_property_collection.py
--rw-r--r--   0        0        0     1205 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/property/well_log.py
--rw-r--r--   0        0        0     7633 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/property/well_log_collection.py
--rw-r--r--   0        0        0      713 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/rq_import/__init__.py
--rw-r--r--   0        0        0     4493 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/rq_import/_add_ab_properties.py
--rw-r--r--   0        0        0     6067 2023-05-14 20:17:35.140952 resqpy-4.8.5/resqpy/rq_import/_add_surfaces.py
--rw-r--r--   0        0        0    32019 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/rq_import/_grid_from_cp.py
--rw-r--r--   0        0        0    34317 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/rq_import/_import_nexus.py
--rw-r--r--   0        0        0     6306 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/rq_import/_import_vdb_all_grids.py
--rw-r--r--   0        0        0    21372 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/rq_import/_import_vdb_ensemble.py
--rw-r--r--   0        0        0     1311 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/strata/__init__.py
--rw-r--r--   0        0        0     8861 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/strata/_binary_contact_interpretation.py
--rw-r--r--   0        0        0    10381 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/strata/_geologic_unit_interpretation.py
--rw-r--r--   0        0        0     1772 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/strata/_strata_common.py
--rw-r--r--   0        0        0     6797 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/strata/_stratigraphic_column.py
--rw-r--r--   0        0        0    13322 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/strata/_stratigraphic_column_rank.py
--rw-r--r--   0        0        0     7432 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/strata/_stratigraphic_unit_feature.py
--rw-r--r--   0        0        0    10167 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/strata/_stratigraphic_unit_interpretation.py
--rw-r--r--   0        0        0      696 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/surface/__init__.py
--rw-r--r--   0        0        0     2331 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/surface/_base_surface.py
--rw-r--r--   0        0        0     3082 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/surface/_combined_surface.py
--rw-r--r--   0        0        0    42192 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/surface/_mesh.py
--rw-r--r--   0        0        0    26120 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/surface/_pointset.py
--rw-r--r--   0        0        0    56386 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/surface/_surface.py
--rw-r--r--   0        0        0    24315 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/surface/_tri_mesh.py
--rw-r--r--   0        0        0    25907 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/surface/_triangulated_patch.py
--rw-r--r--   0        0        0     1074 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/time_series/__init__.py
--rw-r--r--   0        0        0     8595 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/time_series/_any_time_series.py
--rw-r--r--   0        0        0     6617 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/time_series/_from_nexus_summary.py
--rw-r--r--   0        0        0     6366 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/time_series/_functions.py
--rw-r--r--   0        0        0     3311 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/time_series/_geologic_time_series.py
--rw-r--r--   0        0        0     2759 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/time_series/_time_duration.py
--rw-r--r--   0        0        0    10818 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/time_series/_time_series.py
--rw-r--r--   0        0        0      603 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/unstructured/__init__.py
--rw-r--r--   0        0        0    15328 2023-05-14 20:17:35.144952 resqpy-4.8.5/resqpy/unstructured/_hexa_grid.py
--rw-r--r--   0        0        0    35856 2023-05-14 20:17:35.148953 resqpy-4.8.5/resqpy/unstructured/_prism_grid.py
--rw-r--r--   0        0        0     7862 2023-05-14 20:17:35.148953 resqpy-4.8.5/resqpy/unstructured/_pyramid_grid.py
--rw-r--r--   0        0        0    10208 2023-05-14 20:17:35.148953 resqpy-4.8.5/resqpy/unstructured/_tetra_grid.py
--rw-r--r--   0        0        0    51550 2023-05-14 20:17:35.148953 resqpy-4.8.5/resqpy/unstructured/_unstructured_grid.py
--rw-r--r--   0        0        0     1135 2023-05-14 20:17:35.148953 resqpy-4.8.5/resqpy/weights_and_measures/__init__.py
--rw-r--r--   0        0        0     5434 2023-05-14 20:17:35.148953 resqpy-4.8.5/resqpy/weights_and_measures/nexus_units.py
--rw-r--r--   0        0        0    16186 2023-05-14 20:17:35.148953 resqpy-4.8.5/resqpy/weights_and_measures/weights_and_measures.py
--rw-r--r--   0        0        0      990 2023-05-14 20:17:35.148953 resqpy-4.8.5/resqpy/well/__init__.py
--rw-r--r--   0        0        0   187787 2023-05-14 20:17:35.148953 resqpy-4.8.5/resqpy/well/_blocked_well.py
--rw-r--r--   0        0        0    22138 2023-05-14 20:17:35.148953 resqpy-4.8.5/resqpy/well/_deviation_survey.py
--rw-r--r--   0        0        0     7154 2023-05-14 20:17:35.148953 resqpy-4.8.5/resqpy/well/_md_datum.py
--rw-r--r--   0        0        0    48693 2023-05-14 20:17:35.148953 resqpy-4.8.5/resqpy/well/_trajectory.py
--rw-r--r--   0        0        0    15192 2023-05-14 20:17:35.152953 resqpy-4.8.5/resqpy/well/_wellbore_frame.py
--rw-r--r--   0        0        0     8403 2023-05-14 20:17:35.152953 resqpy-4.8.5/resqpy/well/_wellbore_marker.py
--rw-r--r--   0        0        0    20933 2023-05-14 20:17:35.152953 resqpy-4.8.5/resqpy/well/_wellbore_marker_frame.py
--rw-r--r--   0        0        0    22555 2023-05-14 20:17:35.152953 resqpy-4.8.5/resqpy/well/blocked_well_frame.py
--rw-r--r--   0        0        0    24743 2023-05-14 20:17:35.152953 resqpy-4.8.5/resqpy/well/well_object_funcs.py
--rw-r--r--   0        0        0     5969 2023-05-14 20:17:35.152953 resqpy-4.8.5/resqpy/well/well_utils.py
--rw-r--r--   0        0        0     4156 1970-01-01 00:00:00.000000 resqpy-4.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-05-18 13:32:58.734024 resqpy-4.8.6/LICENSE
+-rw-r--r--   0        0        0     2893 2023-05-18 13:32:58.734024 resqpy-4.8.6/README.md
+-rw-r--r--   0        0        0     3227 2023-05-18 13:33:18.530391 resqpy-4.8.6/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-05-18 13:33:18.530391 resqpy-4.8.6/resqpy/__init__.py
+-rw-r--r--   0        0        0    24782 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/crs.py
+-rw-r--r--   0        0        0     1982 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/__init__.py
+-rw-r--r--   0        0        0     6410 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_add_edges_per_column_property_array.py
+-rw-r--r--   0        0        0    21022 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_add_faults.py
+-rw-r--r--   0        0        0     6417 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_add_one_blocked_well_property.py
+-rw-r--r--   0        0        0     8657 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_add_one_grid_property_array.py
+-rw-r--r--   0        0        0     2431 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_add_single_cell_grid.py
+-rw-r--r--   0        0        0     5495 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_add_wells_from_ascii_file.py
+-rw-r--r--   0        0        0     6037 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_add_zone_by_layer_property.py
+-rw-r--r--   0        0        0    11586 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_coarsened_grid.py
+-rw-r--r--   0        0        0    10520 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_common.py
+-rw-r--r--   0        0        0     3730 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_copy_grid.py
+-rw-r--r--   0        0        0    11731 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_drape_to_surface.py
+-rw-r--r--   0        0        0    16391 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_extract_box.py
+-rw-r--r--   0        0        0    22969 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_extract_box_for_well.py
+-rw-r--r--   0        0        0    20325 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_fault_throw_scaling.py
+-rw-r--r--   0        0        0     7157 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_gather_ensemble.py
+-rw-r--r--   0        0        0    17929 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_interpolated_grid.py
+-rw-r--r--   0        0        0     9876 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_local_depth_adjustment.py
+-rw-r--r--   0        0        0    20513 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_refined_grid.py
+-rw-r--r--   0        0        0     5166 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_tilted_grid.py
+-rw-r--r--   0        0        0     4792 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_unsplit_grid.py
+-rw-r--r--   0        0        0    18825 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_zonal_grid.py
+-rw-r--r--   0        0        0     4358 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/derived_model/_zone_layer_ranges_from_array.py
+-rw-r--r--   0        0        0      996 2023-05-18 13:32:58.750024 resqpy-4.8.6/resqpy/fault/__init__.py
+-rw-r--r--   0        0        0    29402 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/fault/_gcs_functions.py
+-rw-r--r--   0        0        0   109110 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/fault/_grid_connection_set.py
+-rw-r--r--   0        0        0      692 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/__init__.py
+-rw-r--r--   0        0        0    20689 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_cell_properties.py
+-rw-r--r--   0        0        0    10120 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_connection_sets.py
+-rw-r--r--   0        0        0    19936 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_create_grid_xml.py
+-rw-r--r--   0        0        0    32064 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_defined_geometry.py
+-rw-r--r--   0        0        0    28203 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_extract_functions.py
+-rw-r--r--   0        0        0    16516 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_face_functions.py
+-rw-r--r--   0        0        0    12236 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_faults.py
+-rw-r--r--   0        0        0   127766 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_grid.py
+-rw-r--r--   0        0        0     3544 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_grid_types.py
+-rw-r--r--   0        0        0      338 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_intervals_info.py
+-rw-r--r--   0        0        0      604 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_moved_functions.py
+-rw-r--r--   0        0        0     7243 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_pillars.py
+-rw-r--r--   0        0        0     5386 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_pixel_maps.py
+-rw-r--r--   0        0        0    65440 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_points_functions.py
+-rw-r--r--   0        0        0    45761 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_regular_grid.py
+-rw-r--r--   0        0        0    19413 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_transmissibility.py
+-rw-r--r--   0        0        0     7944 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_write_hdf5_from_caches.py
+-rw-r--r--   0        0        0     6147 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_write_nexus_corp.py
+-rw-r--r--   0        0        0    13087 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid/_xyz.py
+-rw-r--r--   0        0        0     2593 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid_surface/__init__.py
+-rw-r--r--   0        0        0    35739 2023-05-18 13:32:58.754024 resqpy-4.8.6/resqpy/grid_surface/_blocked_well_populate.py
+-rw-r--r--   0        0        0    64016 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/grid_surface/_find_faces.py
+-rw-r--r--   0        0        0    26056 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/grid_surface/_grid_skin.py
+-rw-r--r--   0        0        0    14379 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/grid_surface/_grid_surface.py
+-rw-r--r--   0        0        0    22498 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/grid_surface/_trajectory_intersects.py
+-rw-r--r--   0        0        0    39760 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/grid_surface/grid_surface_cuda.py
+-rw-r--r--   0        0        0      539 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/lines/__init__.py
+-rw-r--r--   0        0        0    11960 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/lines/_common.py
+-rw-r--r--   0        0        0    41425 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/lines/_polyline.py
+-rw-r--r--   0        0        0    26366 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/lines/_polyline_set.py
+-rw-r--r--   0        0        0      378 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/model/__init__.py
+-rw-r--r--   0        0        0    30171 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/model/_catalogue.py
+-rw-r--r--   0        0        0     2840 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/model/_context.py
+-rw-r--r--   0        0        0    34552 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/model/_forestry.py
+-rw-r--r--   0        0        0     3371 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/model/_grids.py
+-rw-r--r--   0        0        0    14238 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/model/_hdf5.py
+-rw-r--r--   0        0        0   103055 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/model/_model.py
+-rw-r--r--   0        0        0    23589 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/model/_xml.py
+-rw-r--r--   0        0        0      909 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/multi_processing/__init__.py
+-rw-r--r--   0        0        0     7301 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/multi_processing/_multiprocessing.py
+-rw-r--r--   0        0        0       72 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/multi_processing/wrappers/__init__.py
+-rw-r--r--   0        0        0     5952 2023-05-18 13:32:58.758025 resqpy-4.8.6/resqpy/multi_processing/wrappers/blocked_well_mp.py
+-rw-r--r--   0        0        0    21156 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/multi_processing/wrappers/grid_surface_mp.py
+-rw-r--r--   0        0        0     5793 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/multi_processing/wrappers/mesh_mp.py
+-rw-r--r--   0        0        0       84 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/__init__.py
+-rw-r--r--   0        0        0     2147 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/ab_toolbox.py
+-rw-r--r--   0        0        0     7521 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/base.py
+-rw-r--r--   0        0        0    20925 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/box_utilities.py
+-rw-r--r--   0        0        0     5935 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/class_dict.py
+-rw-r--r--   0        0        0     9489 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/consolidation.py
+-rw-r--r--   0        0        0     5177 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/data/build.py
+-rw-r--r--   0        0        0   498136 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/data/properties.json
+-rw-r--r--   0        0        0    19836 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/dataframe.py
+-rw-r--r--   0        0        0      307 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/exceptions.py
+-rw-r--r--   0        0        0     1313 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/factors.py
+-rw-r--r--   0        0        0    24541 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/fine_coarse.py
+-rw-r--r--   0        0        0    27669 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/grid_functions.py
+-rw-r--r--   0        0        0    20158 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/intersection.py
+-rw-r--r--   0        0        0     8408 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/keyword_files.py
+-rw-r--r--   0        0        0    19210 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/load_data.py
+-rw-r--r--   0        0        0     6628 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/point_inclusion.py
+-rw-r--r--   0        0        0     1103 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/random_seed.py
+-rw-r--r--   0        0        0     5441 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/read_nexus_fault.py
+-rw-r--r--   0        0        0    17083 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/relperm.py
+-rw-r--r--   0        0        0    12189 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/simple_lines.py
+-rw-r--r--   0        0        0      760 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/time.py
+-rw-r--r--   0        0        0      822 2023-05-18 13:32:58.762024 resqpy-4.8.6/resqpy/olio/trademark.py
+-rw-r--r--   0        0        0    61869 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/olio/transmission.py
+-rw-r--r--   0        0        0    44768 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/olio/triangulation.py
+-rw-r--r--   0        0        0     7324 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/olio/uuid.py
+-rw-r--r--   0        0        0    45231 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/olio/vdb.py
+-rw-r--r--   0        0        0    46253 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/olio/vector_utilities.py
+-rw-r--r--   0        0        0     6185 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/olio/volume.py
+-rw-r--r--   0        0        0    26220 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/olio/wellspec_keywords.py
+-rw-r--r--   0        0        0     5142 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/olio/write_data.py
+-rw-r--r--   0        0        0    19055 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/olio/write_hdf5.py
+-rw-r--r--   0        0        0    24925 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/olio/xml_et.py
+-rw-r--r--   0        0        0     1824 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/olio/xml_namespaces.py
+-rw-r--r--   0        0        0     5709 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/olio/zmap_reader.py
+-rw-r--r--   0        0        0     2206 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/__init__.py
+-rw-r--r--   0        0        0     2937 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/_utils.py
+-rw-r--r--   0        0        0     1685 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/boundary_feature.py
+-rw-r--r--   0        0        0     5190 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/boundary_feature_interpretation.py
+-rw-r--r--   0        0        0     6186 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/earth_model_interpretation.py
+-rw-r--r--   0        0        0    12457 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/fault_interpretation.py
+-rw-r--r--   0        0        0     2757 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/fluid_boundary_feature.py
+-rw-r--r--   0        0        0     1702 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/frontier_feature.py
+-rw-r--r--   0        0        0     4498 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/generic_interpretation.py
+-rw-r--r--   0        0        0     3771 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/genetic_boundary_feature.py
+-rw-r--r--   0        0        0     8605 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/geobody_boundary_interpretation.py
+-rw-r--r--   0        0        0     1836 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/geobody_feature.py
+-rw-r--r--   0        0        0     8052 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/geobody_interpretation.py
+-rw-r--r--   0        0        0     1739 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/geologic_unit_feature.py
+-rw-r--r--   0        0        0     8346 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/horizon_interpretation.py
+-rw-r--r--   0        0        0     2697 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/organization_feature.py
+-rw-r--r--   0        0        0     5565 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/rock_fluid_unit_feature.py
+-rw-r--r--   0        0        0     1802 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/structural_organization_interpretation.py
+-rw-r--r--   0        0        0     2675 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/tectonic_boundary_feature.py
+-rw-r--r--   0        0        0     1843 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/wellbore_feature.py
+-rw-r--r--   0        0        0     6973 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/organize/wellbore_interpretation.py
+-rw-r--r--   0        0        0     2155 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/property/__init__.py
+-rw-r--r--   0        0        0    16697 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/property/_collection_add_part.py
+-rw-r--r--   0        0        0    12926 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/property/_collection_create_xml.py
+-rw-r--r--   0        0        0    30090 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/property/_collection_get_attributes.py
+-rw-r--r--   0        0        0     5368 2023-05-18 13:32:58.766025 resqpy-4.8.6/resqpy/property/_collection_support.py
+-rw-r--r--   0        0        0    24426 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/property/_property.py
+-rw-r--r--   0        0        0    66946 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/property/grid_property_collection.py
+-rw-r--r--   0        0        0   143306 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/property/property_collection.py
+-rw-r--r--   0        0        0    36127 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/property/property_common.py
+-rw-r--r--   0        0        0     5557 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/property/property_kind.py
+-rw-r--r--   0        0        0     7737 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/property/string_lookup.py
+-rw-r--r--   0        0        0     1077 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/property/well_interval_property.py
+-rw-r--r--   0        0        0     1577 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/property/well_interval_property_collection.py
+-rw-r--r--   0        0        0     1205 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/property/well_log.py
+-rw-r--r--   0        0        0     7633 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/property/well_log_collection.py
+-rw-r--r--   0        0        0      713 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/rq_import/__init__.py
+-rw-r--r--   0        0        0     4493 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/rq_import/_add_ab_properties.py
+-rw-r--r--   0        0        0     6067 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/rq_import/_add_surfaces.py
+-rw-r--r--   0        0        0    32019 2023-05-18 13:32:58.770025 resqpy-4.8.6/resqpy/rq_import/_grid_from_cp.py
+-rw-r--r--   0        0        0    34317 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/rq_import/_import_nexus.py
+-rw-r--r--   0        0        0     6306 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/rq_import/_import_vdb_all_grids.py
+-rw-r--r--   0        0        0    21372 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/rq_import/_import_vdb_ensemble.py
+-rw-r--r--   0        0        0     1311 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/strata/__init__.py
+-rw-r--r--   0        0        0     8861 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/strata/_binary_contact_interpretation.py
+-rw-r--r--   0        0        0    10381 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/strata/_geologic_unit_interpretation.py
+-rw-r--r--   0        0        0     1772 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/strata/_strata_common.py
+-rw-r--r--   0        0        0     6797 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/strata/_stratigraphic_column.py
+-rw-r--r--   0        0        0    13322 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/strata/_stratigraphic_column_rank.py
+-rw-r--r--   0        0        0     7432 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/strata/_stratigraphic_unit_feature.py
+-rw-r--r--   0        0        0    10167 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/strata/_stratigraphic_unit_interpretation.py
+-rw-r--r--   0        0        0      696 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/surface/__init__.py
+-rw-r--r--   0        0        0     2331 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/surface/_base_surface.py
+-rw-r--r--   0        0        0     3082 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/surface/_combined_surface.py
+-rw-r--r--   0        0        0    42192 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/surface/_mesh.py
+-rw-r--r--   0        0        0    26120 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/surface/_pointset.py
+-rw-r--r--   0        0        0    56386 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/surface/_surface.py
+-rw-r--r--   0        0        0    24315 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/surface/_tri_mesh.py
+-rw-r--r--   0        0        0    25907 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/surface/_triangulated_patch.py
+-rw-r--r--   0        0        0     1074 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/time_series/__init__.py
+-rw-r--r--   0        0        0     8595 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/time_series/_any_time_series.py
+-rw-r--r--   0        0        0     6617 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/time_series/_from_nexus_summary.py
+-rw-r--r--   0        0        0     6366 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/time_series/_functions.py
+-rw-r--r--   0        0        0     3311 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/time_series/_geologic_time_series.py
+-rw-r--r--   0        0        0     2759 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/time_series/_time_duration.py
+-rw-r--r--   0        0        0    10818 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/time_series/_time_series.py
+-rw-r--r--   0        0        0      603 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/unstructured/__init__.py
+-rw-r--r--   0        0        0    15328 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/unstructured/_hexa_grid.py
+-rw-r--r--   0        0        0    35856 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/unstructured/_prism_grid.py
+-rw-r--r--   0        0        0     7862 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/unstructured/_pyramid_grid.py
+-rw-r--r--   0        0        0    10208 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/unstructured/_tetra_grid.py
+-rw-r--r--   0        0        0    51550 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/unstructured/_unstructured_grid.py
+-rw-r--r--   0        0        0     1135 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/weights_and_measures/__init__.py
+-rw-r--r--   0        0        0     5434 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/weights_and_measures/nexus_units.py
+-rw-r--r--   0        0        0    16186 2023-05-18 13:32:58.774025 resqpy-4.8.6/resqpy/weights_and_measures/weights_and_measures.py
+-rw-r--r--   0        0        0      990 2023-05-18 13:32:58.778025 resqpy-4.8.6/resqpy/well/__init__.py
+-rw-r--r--   0        0        0   187787 2023-05-18 13:32:58.778025 resqpy-4.8.6/resqpy/well/_blocked_well.py
+-rw-r--r--   0        0        0    22138 2023-05-18 13:32:58.778025 resqpy-4.8.6/resqpy/well/_deviation_survey.py
+-rw-r--r--   0        0        0     7154 2023-05-18 13:32:58.778025 resqpy-4.8.6/resqpy/well/_md_datum.py
+-rw-r--r--   0        0        0    48693 2023-05-18 13:32:58.778025 resqpy-4.8.6/resqpy/well/_trajectory.py
+-rw-r--r--   0        0        0    15192 2023-05-18 13:32:58.778025 resqpy-4.8.6/resqpy/well/_wellbore_frame.py
+-rw-r--r--   0        0        0     8403 2023-05-18 13:32:58.778025 resqpy-4.8.6/resqpy/well/_wellbore_marker.py
+-rw-r--r--   0        0        0    20933 2023-05-18 13:32:58.778025 resqpy-4.8.6/resqpy/well/_wellbore_marker_frame.py
+-rw-r--r--   0        0        0    22555 2023-05-18 13:32:58.778025 resqpy-4.8.6/resqpy/well/blocked_well_frame.py
+-rw-r--r--   0        0        0    24743 2023-05-18 13:32:58.778025 resqpy-4.8.6/resqpy/well/well_object_funcs.py
+-rw-r--r--   0        0        0     5969 2023-05-18 13:32:58.778025 resqpy-4.8.6/resqpy/well/well_utils.py
+-rw-r--r--   0        0        0     4156 1970-01-01 00:00:00.000000 resqpy-4.8.6/PKG-INFO
```

### Comparing `resqpy-4.8.5/LICENSE` & `resqpy-4.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/README.md` & `resqpy-4.8.6/README.md`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/pyproject.toml` & `resqpy-4.8.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires = ["poetry>=1.0.2", "poetry-dynamic-versioning"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "resqpy"
-version = "4.8.5" # Set at build time
+version = "4.8.6" # Set at build time
 description = "Python API for working with RESQML models"
 authors = ["BP"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bp/resqpy"
 documentation = "https://resqpy.readthedocs.io/en/latest/"
 keywords = ["RESQML"]
```

### Comparing `resqpy-4.8.5/resqpy/__init__.py` & `resqpy-4.8.6/resqpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,10 +24,10 @@
     weights_and_measures
     well
     olio
 """
 
 import logging
 
-__version__ = "4.8.5"  # Set at build time
+__version__ = "4.8.6"  # Set at build time
 log = logging.getLogger(__name__)
 log.info(f"Imported resqpy version {__version__}")
```

### Comparing `resqpy-4.8.5/resqpy/crs.py` & `resqpy-4.8.6/resqpy/crs.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/__init__.py` & `resqpy-4.8.6/resqpy/derived_model/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_add_edges_per_column_property_array.py` & `resqpy-4.8.6/resqpy/derived_model/_add_edges_per_column_property_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_add_faults.py` & `resqpy-4.8.6/resqpy/derived_model/_add_faults.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,22 +104,23 @@
         polylines = polylines.convert_to_polylines()
 
     composite_face_set_dict = {}
 
     # build pillar list dict for polylines if necessary
     if full_pillar_list_dict is None:
         full_pillar_list_dict = {}
+        log.debug('using polylines for defining faults')
         _populate_composite_face_sets_for_polylines(model, grid, polylines, lines_crs_uuid, grid.crs, lines_file_list,
                                                     full_pillar_list_dict, composite_face_set_dict)
 
     else:  # populate composite face set dictionary from full pillar list
         _populate_composite_face_sets_for_pillar_lists(source_grid, full_pillar_list_dict, composite_face_set_dict)
 
     # log.debug(f'full_pillar_list_dict:\n{full_pillar_list_dict}')
-
+    log.debug(f'number of faults to be added: {len(full_pillar_list_dict)}')
     _process_full_pillar_list_dict(grid, full_pillar_list_dict, left_right_throw_dict)
 
     collection = rqdm_c._prepare_simple_inheritance(grid, source_grid, inherit_properties, inherit_realization,
                                                     inherit_all_realizations)
     # todo: recompute depth properties (and volumes, cell lengths etc. if being strict)
 
     if new_grid_title is None or len(new_grid_title) == 0:
@@ -179,36 +180,41 @@
        delta_throw_right (float): as for delta_throw_left but applied to points to the right of the
           line
     """
 
     # this function introduces new data into the RESQML arrays representing split pillars
     # familiarity with those array representations is needed if working on this function
 
-    if full_pillar_list is None or len(full_pillar_list) < 3:
+    if full_pillar_list is None or len(full_pillar_list) < 2:
         return
     assert grid.z_units() == grid.xy_units(),  \
         'crs used by grid has differing xy and z units – mix not supported when adding faults'
     grid.cache_all_geometry_arrays()
     assert hasattr(grid, 'points_cached')
     # make grid into a faulted grid if hitherto unfaulted
     if not grid.has_split_coordinate_lines:
+        log.debug('converting grid to split pillar representation')
         grid.points_cached = grid.points_cached.reshape((grid.nk_plus_k_gaps + 1, (grid.nj + 1) * (grid.ni + 1), 3))
         grid.split_pillar_indices_cached = np.array([], dtype = int)
         grid.cols_for_split_pillars = np.array([], dtype = int)
         grid.cols_for_split_pillars_cl = np.array([], dtype = int)
         grid.has_split_coordinate_lines = True
     assert grid.points_cached.ndim == 3
     if len(grid.cols_for_split_pillars_cl) == 0:
         cl = 0
     else:
         cl = grid.cols_for_split_pillars_cl[-1]
     original_p = np.zeros((grid.nk_plus_k_gaps + 1, 3), dtype = float)
     n_primaries = (grid.nj + 1) * (grid.ni + 1)
-    for p_index in range(1, len(full_pillar_list) - 1):
+    for p_index in range(len(full_pillar_list)):
         primary_ji0 = full_pillar_list[p_index]
+        # if end pillar is internal to model, do not split
+        if p_index == 0 or p_index == len(full_pillar_list) - 1:
+            if not (primary_ji0[0] in (0, grid.nj) or primary_ji0[1] in (0, grid.ni)):
+                continue
         primary = primary_ji0[0] * (grid.ni + 1) + primary_ji0[1]
         p_vector = np.array(_pillar_vector(grid, primary), dtype = float)
         if p_vector is None:
             continue
         throw_left_vector = np.expand_dims(delta_throw_left * p_vector, axis = 0)
         throw_right_vector = np.expand_dims(delta_throw_right * p_vector, axis = 0)
         # log.debug(f'T: p ji0: {primary_ji0}; p vec: {p_vector}; left v: {throw_left_vector}; right v: {throw_right_vector}')
@@ -340,14 +346,15 @@
                     cl += 1
                     grid.cols_for_split_pillars_cl[-1] = cl
     return cl
 
 
 def _process_full_pillar_list_dict(grid, full_pillar_list_dict, left_right_throw_dict):
     for fault_key in full_pillar_list_dict:
+        log.debug(f'processing fault: {fault_key}')
         full_pillar_list = full_pillar_list_dict[fault_key]
         left_right_throw = None
         if left_right_throw_dict is not None:
             left_right_throw = left_right_throw_dict.get(fault_key)
         if left_right_throw is None:
             left_right_throw = (+0.5, -0.5)
         log.debug(
```

### Comparing `resqpy-4.8.5/resqpy/derived_model/_add_one_blocked_well_property.py` & `resqpy-4.8.6/resqpy/derived_model/_add_one_blocked_well_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_add_one_grid_property_array.py` & `resqpy-4.8.6/resqpy/derived_model/_add_one_grid_property_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_add_single_cell_grid.py` & `resqpy-4.8.6/resqpy/derived_model/_add_single_cell_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_add_wells_from_ascii_file.py` & `resqpy-4.8.6/resqpy/derived_model/_add_wells_from_ascii_file.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_add_zone_by_layer_property.py` & `resqpy-4.8.6/resqpy/derived_model/_add_zone_by_layer_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_coarsened_grid.py` & `resqpy-4.8.6/resqpy/derived_model/_coarsened_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_common.py` & `resqpy-4.8.6/resqpy/derived_model/_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,19 @@
         source_collection = source_grid.extract_property_collection()
         if source_collection is not None:
             #  do not inherit the inactive property array by this mechanism
             collection = rqp.GridPropertyCollection()
             collection.set_grid(grid)
             collection.extend_imported_list_copying_properties_from_other_grid_collection(
                 source_collection, realization = inherit_realization, copy_all_realizations = inherit_all_realizations)
+        if source_grid.model is not grid.model:
+            uuids = source_collection.time_series_uuid_list(sort_list = False)
+            uuids += source_collection.string_lookup_uuid_list(sort_list = False)
+            for uuid in uuids:
+                grid.model.copy_uuid_from_other_model(source_grid.model, uuid)
     return collection
 
 
 def _write_grid(epc_file,
                 grid,
                 ext_uuid = None,
                 property_collection = None,
```

### Comparing `resqpy-4.8.5/resqpy/derived_model/_copy_grid.py` & `resqpy-4.8.6/resqpy/derived_model/_copy_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_drape_to_surface.py` & `resqpy-4.8.6/resqpy/derived_model/_drape_to_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_extract_box.py` & `resqpy-4.8.6/resqpy/derived_model/_extract_box.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_extract_box_for_well.py` & `resqpy-4.8.6/resqpy/derived_model/_extract_box_for_well.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_fault_throw_scaling.py` & `resqpy-4.8.6/resqpy/derived_model/_fault_throw_scaling.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_gather_ensemble.py` & `resqpy-4.8.6/resqpy/derived_model/_gather_ensemble.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_interpolated_grid.py` & `resqpy-4.8.6/resqpy/derived_model/_interpolated_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_local_depth_adjustment.py` & `resqpy-4.8.6/resqpy/derived_model/_local_depth_adjustment.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_refined_grid.py` & `resqpy-4.8.6/resqpy/derived_model/_refined_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_tilted_grid.py` & `resqpy-4.8.6/resqpy/derived_model/_tilted_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_unsplit_grid.py` & `resqpy-4.8.6/resqpy/derived_model/_unsplit_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_zonal_grid.py` & `resqpy-4.8.6/resqpy/derived_model/_zonal_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/derived_model/_zone_layer_ranges_from_array.py` & `resqpy-4.8.6/resqpy/derived_model/_zone_layer_ranges_from_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/fault/__init__.py` & `resqpy-4.8.6/resqpy/fault/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/fault/_gcs_functions.py` & `resqpy-4.8.6/resqpy/fault/_gcs_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/fault/_grid_connection_set.py` & `resqpy-4.8.6/resqpy/fault/_grid_connection_set.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/__init__.py` & `resqpy-4.8.6/resqpy/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_cell_properties.py` & `resqpy-4.8.6/resqpy/grid/_cell_properties.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_connection_sets.py` & `resqpy-4.8.6/resqpy/grid/_connection_sets.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_create_grid_xml.py` & `resqpy-4.8.6/resqpy/grid/_create_grid_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_defined_geometry.py` & `resqpy-4.8.6/resqpy/grid/_defined_geometry.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_extract_functions.py` & `resqpy-4.8.6/resqpy/grid/_extract_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_face_functions.py` & `resqpy-4.8.6/resqpy/grid/_face_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_faults.py` & `resqpy-4.8.6/resqpy/grid/_faults.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_grid.py` & `resqpy-4.8.6/resqpy/grid/_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_grid_types.py` & `resqpy-4.8.6/resqpy/grid/_grid_types.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_moved_functions.py` & `resqpy-4.8.6/resqpy/grid/_moved_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_pillars.py` & `resqpy-4.8.6/resqpy/grid/_pillars.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_pixel_maps.py` & `resqpy-4.8.6/resqpy/grid/_pixel_maps.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_points_functions.py` & `resqpy-4.8.6/resqpy/grid/_points_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_regular_grid.py` & `resqpy-4.8.6/resqpy/grid/_regular_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_transmissibility.py` & `resqpy-4.8.6/resqpy/grid/_transmissibility.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_write_hdf5_from_caches.py` & `resqpy-4.8.6/resqpy/grid/_write_hdf5_from_caches.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_write_nexus_corp.py` & `resqpy-4.8.6/resqpy/grid/_write_nexus_corp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid/_xyz.py` & `resqpy-4.8.6/resqpy/grid/_xyz.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid_surface/__init__.py` & `resqpy-4.8.6/resqpy/grid_surface/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid_surface/_blocked_well_populate.py` & `resqpy-4.8.6/resqpy/grid_surface/_blocked_well_populate.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid_surface/_find_faces.py` & `resqpy-4.8.6/resqpy/grid_surface/_find_faces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid_surface/_grid_skin.py` & `resqpy-4.8.6/resqpy/grid_surface/_grid_skin.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid_surface/_grid_surface.py` & `resqpy-4.8.6/resqpy/grid_surface/_grid_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid_surface/_trajectory_intersects.py` & `resqpy-4.8.6/resqpy/grid_surface/_trajectory_intersects.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/grid_surface/grid_surface_cuda.py` & `resqpy-4.8.6/resqpy/grid_surface/grid_surface_cuda.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/lines/__init__.py` & `resqpy-4.8.6/resqpy/lines/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/lines/_common.py` & `resqpy-4.8.6/resqpy/lines/_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/lines/_polyline.py` & `resqpy-4.8.6/resqpy/lines/_polyline.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/lines/_polyline_set.py` & `resqpy-4.8.6/resqpy/lines/_polyline_set.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/model/_catalogue.py` & `resqpy-4.8.6/resqpy/model/_catalogue.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/model/_context.py` & `resqpy-4.8.6/resqpy/model/_context.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/model/_forestry.py` & `resqpy-4.8.6/resqpy/model/_forestry.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/model/_grids.py` & `resqpy-4.8.6/resqpy/model/_grids.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/model/_hdf5.py` & `resqpy-4.8.6/resqpy/model/_hdf5.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/model/_model.py` & `resqpy-4.8.6/resqpy/model/_model.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/model/_xml.py` & `resqpy-4.8.6/resqpy/model/_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/multi_processing/__init__.py` & `resqpy-4.8.6/resqpy/multi_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/multi_processing/_multiprocessing.py` & `resqpy-4.8.6/resqpy/multi_processing/_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/multi_processing/wrappers/blocked_well_mp.py` & `resqpy-4.8.6/resqpy/multi_processing/wrappers/blocked_well_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/multi_processing/wrappers/grid_surface_mp.py` & `resqpy-4.8.6/resqpy/multi_processing/wrappers/grid_surface_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/multi_processing/wrappers/mesh_mp.py` & `resqpy-4.8.6/resqpy/multi_processing/wrappers/mesh_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/ab_toolbox.py` & `resqpy-4.8.6/resqpy/olio/ab_toolbox.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/base.py` & `resqpy-4.8.6/resqpy/olio/base.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/box_utilities.py` & `resqpy-4.8.6/resqpy/olio/box_utilities.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/class_dict.py` & `resqpy-4.8.6/resqpy/olio/class_dict.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/consolidation.py` & `resqpy-4.8.6/resqpy/olio/consolidation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/data/build.py` & `resqpy-4.8.6/resqpy/olio/data/build.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/data/properties.json` & `resqpy-4.8.6/resqpy/olio/data/properties.json`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/dataframe.py` & `resqpy-4.8.6/resqpy/olio/dataframe.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/factors.py` & `resqpy-4.8.6/resqpy/olio/factors.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/fine_coarse.py` & `resqpy-4.8.6/resqpy/olio/fine_coarse.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/grid_functions.py` & `resqpy-4.8.6/resqpy/olio/grid_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -549,20 +549,25 @@
 
     return framed[1:-1, 1:-1]
 
 
 def left_right_foursome(full_pillar_list, p_index):
     """Returns (2, 2) bool numpy array indicating which columns around a primary pillar are to the right of a line."""
 
-    assert 0 < p_index < len(full_pillar_list) - 1
+    assert 0 <= p_index <= len(full_pillar_list) - 1
     here = np.array(full_pillar_list[p_index], dtype = int)
-    previous = np.array(full_pillar_list[p_index - 1], dtype = int)
-    next = np.array(full_pillar_list[p_index + 1], dtype = int)
-    entry = tuple(here - previous)
-    exit = tuple(next - here)
+    previous = np.array(full_pillar_list[p_index - 1], dtype = int) if p_index > 0 else None
+    next = np.array(full_pillar_list[p_index + 1], dtype = int) if p_index < len(full_pillar_list) - 1 else None
+    assert previous is not None or next is not None
+    entry = None if previous is None else tuple(here - previous)
+    exit = None if next is None else tuple(next - here)
+    if entry is None:
+        entry = exit
+    elif exit is None:
+        exit = entry
     # yapf: disable
     entry_tuples_list = [(0, 1), (0, -1), (1, 0), (-1, 0)]
     exit_tuples_list = [[(-1, 0), (0, 1),  (1, 0)],
                         [(-1, 0), (0, -1), (1, 0)],
                         [(0, -1), (1, 0),  (0, 1)],
                         [(0, -1), (-1, 0), (0, 1)]]
     result_arrays_list = [[np.array([[False, True],  [True,  True]],  dtype = bool),
```

### Comparing `resqpy-4.8.5/resqpy/olio/intersection.py` & `resqpy-4.8.6/resqpy/olio/intersection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/keyword_files.py` & `resqpy-4.8.6/resqpy/olio/keyword_files.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/load_data.py` & `resqpy-4.8.6/resqpy/olio/load_data.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/point_inclusion.py` & `resqpy-4.8.6/resqpy/olio/point_inclusion.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/random_seed.py` & `resqpy-4.8.6/resqpy/olio/random_seed.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/read_nexus_fault.py` & `resqpy-4.8.6/resqpy/olio/read_nexus_fault.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/relperm.py` & `resqpy-4.8.6/resqpy/olio/relperm.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/simple_lines.py` & `resqpy-4.8.6/resqpy/olio/simple_lines.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/time.py` & `resqpy-4.8.6/resqpy/olio/time.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/trademark.py` & `resqpy-4.8.6/resqpy/olio/trademark.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/transmission.py` & `resqpy-4.8.6/resqpy/olio/transmission.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/triangulation.py` & `resqpy-4.8.6/resqpy/olio/triangulation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/uuid.py` & `resqpy-4.8.6/resqpy/olio/uuid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/vdb.py` & `resqpy-4.8.6/resqpy/olio/vdb.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/vector_utilities.py` & `resqpy-4.8.6/resqpy/olio/vector_utilities.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/volume.py` & `resqpy-4.8.6/resqpy/olio/volume.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/wellspec_keywords.py` & `resqpy-4.8.6/resqpy/olio/wellspec_keywords.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/write_data.py` & `resqpy-4.8.6/resqpy/olio/write_data.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/write_hdf5.py` & `resqpy-4.8.6/resqpy/olio/write_hdf5.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/xml_et.py` & `resqpy-4.8.6/resqpy/olio/xml_et.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/xml_namespaces.py` & `resqpy-4.8.6/resqpy/olio/xml_namespaces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/olio/zmap_reader.py` & `resqpy-4.8.6/resqpy/olio/zmap_reader.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/__init__.py` & `resqpy-4.8.6/resqpy/organize/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/_utils.py` & `resqpy-4.8.6/resqpy/organize/_utils.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/boundary_feature.py` & `resqpy-4.8.6/resqpy/organize/boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/boundary_feature_interpretation.py` & `resqpy-4.8.6/resqpy/organize/boundary_feature_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/earth_model_interpretation.py` & `resqpy-4.8.6/resqpy/organize/earth_model_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/fault_interpretation.py` & `resqpy-4.8.6/resqpy/organize/fault_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/fluid_boundary_feature.py` & `resqpy-4.8.6/resqpy/organize/fluid_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/frontier_feature.py` & `resqpy-4.8.6/resqpy/organize/frontier_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/generic_interpretation.py` & `resqpy-4.8.6/resqpy/organize/generic_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/genetic_boundary_feature.py` & `resqpy-4.8.6/resqpy/organize/genetic_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/geobody_boundary_interpretation.py` & `resqpy-4.8.6/resqpy/organize/geobody_boundary_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/geobody_feature.py` & `resqpy-4.8.6/resqpy/organize/geobody_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/geobody_interpretation.py` & `resqpy-4.8.6/resqpy/organize/geobody_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/geologic_unit_feature.py` & `resqpy-4.8.6/resqpy/organize/geologic_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/horizon_interpretation.py` & `resqpy-4.8.6/resqpy/organize/horizon_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/organization_feature.py` & `resqpy-4.8.6/resqpy/organize/organization_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/rock_fluid_unit_feature.py` & `resqpy-4.8.6/resqpy/organize/rock_fluid_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/structural_organization_interpretation.py` & `resqpy-4.8.6/resqpy/organize/structural_organization_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/tectonic_boundary_feature.py` & `resqpy-4.8.6/resqpy/organize/tectonic_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/wellbore_feature.py` & `resqpy-4.8.6/resqpy/organize/wellbore_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/organize/wellbore_interpretation.py` & `resqpy-4.8.6/resqpy/organize/wellbore_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/property/__init__.py` & `resqpy-4.8.6/resqpy/property/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/property/_collection_add_part.py` & `resqpy-4.8.6/resqpy/property/_collection_add_part.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/property/_collection_create_xml.py` & `resqpy-4.8.6/resqpy/property/_collection_create_xml.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import resqpy.property._collection_get_attributes as pcga
 import resqpy.property.property_common as rqp_c
 from resqpy.olio.xml_namespaces import curly_namespace as ns
 
 
 def _create_xml_add_as_part(collection, add_as_part, p_uuid, p_node, add_relationships, support_root,
                             property_kind_uuid, related_time_series_node, sl_root, discrete, string_lookup_uuid,
-                            const_value, ext_uuid):
+                            const_value, ext_uuid, d_or_c_text):
     if add_as_part:
-        collection.model.add_part('obj_' + collection.d_or_c_text + 'Property', p_uuid, p_node)
+        collection.model.add_part('obj_' + d_or_c_text + 'Property', p_uuid, p_node)
         if add_relationships:
             _create_xml_add_relationships(collection, p_node, support_root, property_kind_uuid,
                                           related_time_series_node, sl_root, discrete, string_lookup_uuid, const_value,
                                           ext_uuid)
 
 
 def _create_property_set_xml_add_as_part(collection, ps_node, ps_uuid, add_relationships, parent_set_ref_node,
@@ -38,23 +38,20 @@
         if collection.parent_set_root is not None:
             collection.model.create_reciprocal_relationship(ps_node, 'destinationObject', parent_set_ref_node,
                                                             'sourceObject')
         for prop_node in prop_node_list:
             collection.model.create_reciprocal_relationship(ps_node, 'destinationObject', prop_node, 'sourceObject')
 
 
-def _create_xml_get_basics(collection, discrete, points, const_value, facet_type, null_value, support_uuid, ext_uuid):
+def _create_xml_get_basics(collection, discrete, points, const_value, facet_type, support_uuid, ext_uuid):
     assert not discrete or not points
     assert not points or const_value is None
     assert not points or facet_type is None
     assert collection.model is not None
 
-    if null_value is not None:
-        collection.null_value = null_value
-
     if support_uuid is None:
         support_uuid = collection.support_uuid
     assert support_uuid is not None
     support_root = collection.model.root_for_uuid(support_uuid)
     # assert support_root is not None
 
     if ext_uuid is None:
@@ -84,50 +81,50 @@
                                          property_kind_uuid,
                                          content_type = 'obj_PropertyKind',
                                          root = p_kind_node)
     return property_kind_uuid
 
 
 def _create_xml_patch_node(collection, p_node, points, const_value, indexable_element, direction, p_uuid, ext_uuid,
-                           expand_const_arrays):
+                           expand_const_arrays, hdf5_type, xsd_type, null_value):
     # create patch node
     const_count = None
     if const_value is not None and not expand_const_arrays:
         s_shape = collection.supporting_shape(indexable_element = indexable_element, direction = direction)
         assert s_shape is not None
         const_count = np.product(np.array(s_shape, dtype = int))
     else:
         const_value = None
     _ = collection.model.create_patch(p_uuid,
                                       ext_uuid,
                                       root = p_node,
-                                      hdf5_type = collection.hdf5_type,
-                                      xsd_type = collection.xsd_type,
-                                      null_value = collection.null_value,
+                                      hdf5_type = hdf5_type,
+                                      xsd_type = xsd_type,
+                                      null_value = null_value,
                                       const_value = const_value,
                                       const_count = const_count,
                                       points = points)
 
 
 def _create_xml_property_min_max(collection, property_array, const_value, discrete, add_min_max, p_node, min_value,
-                                 max_value, categorical, null_value, points):
+                                 max_value, categorical, null_value, points, xsd_type):
     if add_min_max and not categorical and not points:
         # todo: use active cell mask on numpy min and max operations; exclude null values on discrete min max
         min_value, max_value = pcga._get_property_array_min_max_value(collection, property_array, const_value, discrete,
                                                                       min_value, max_value, categorical, null_value)
         if min_value is not None:
             min_node = rqet.SubElement(p_node, ns['resqml2'] + 'MinimumValue')
-            min_node.set(ns['xsi'] + 'type', ns['xsd'] + collection.xsd_type)
+            min_node.set(ns['xsi'] + 'type', ns['xsd'] + xsd_type)
             if discrete:
                 min_node.text = str(maths.floor(min_value))
             else:
                 min_node.text = str(min_value)
         if max_value is not None:
             max_node = rqet.SubElement(p_node, ns['resqml2'] + 'MaximumValue')
-            max_node.set(ns['xsi'] + 'type', ns['xsd'] + collection.xsd_type)
+            max_node.set(ns['xsi'] + 'type', ns['xsd'] + xsd_type)
             if discrete:
                 max_node.text = str(maths.ceil(max_value))
             else:
                 max_node.text = str(max_value)
 
 
 def _create_xml_lookup_node(collection, p_node, string_lookup_uuid):
@@ -223,16 +220,16 @@
     collection.model.create_supporting_representation(support_uuid = support_uuid,
                                                       root = p_node,
                                                       title = support_title,
                                                       content_type = support_type)
     return related_time_series_node
 
 
-def _create_xml_get_p_node(collection, p_uuid):
-    p_node = collection.model.new_obj_node(collection.d_or_c_text + 'Property')
+def _create_xml_get_p_node(collection, p_uuid, d_or_c_text):
+    p_node = collection.model.new_obj_node(d_or_c_text + 'Property')
     if p_uuid is None:
         p_uuid = bu.uuid_from_string(p_node.attrib['uuid'])
     else:
         p_node.attrib['uuid'] = str(p_uuid)
     return p_node, p_uuid
```

### Comparing `resqpy-4.8.5/resqpy/property/_collection_get_attributes.py` & `resqpy-4.8.6/resqpy/property/_collection_get_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,33 +54,34 @@
                                     example_uom = uom,
                                     parent_property_kind = 'discrete' if discrete else 'continuous')
             lpk.create_xml()
             property_kind_uuid = lpk.uuid
     return property_kind_uuid
 
 
-def _get_property_type_details(collection, discrete, string_lookup_uuid, points):
+def _get_property_type_details(discrete, string_lookup_uuid, points, null_value):
+    d_or_c_text = xsd_type = hdf5_type = None
     if discrete:
         if string_lookup_uuid is None:
-            collection.d_or_c_text = 'Discrete'
-
+            d_or_c_text = 'Discrete'
         else:
-            collection.d_or_c_text = 'Categorical'
-        collection.xsd_type = 'integer'
-        collection.hdf5_type = 'IntegerHdf5Array'
+            d_or_c_text = 'Categorical'
+        xsd_type = 'integer'
+        hdf5_type = 'IntegerHdf5Array'
     elif points:
-        collection.d_or_c_text = 'Points'
-        collection.xsd_type = 'double'
-        collection.hdf5_type = 'Point3dHdf5Array'
-        collection.null_value = None
+        d_or_c_text = 'Points'
+        xsd_type = 'double'
+        hdf5_type = 'Point3dHdf5Array'
+        null_value = None
     else:
-        collection.d_or_c_text = 'Continuous'
-        collection.xsd_type = 'double'
-        collection.hdf5_type = 'DoubleHdf5Array'
-        collection.null_value = None
+        d_or_c_text = 'Continuous'
+        xsd_type = 'double'
+        hdf5_type = 'DoubleHdf5Array'
+        null_value = None
+    return d_or_c_text, xsd_type, hdf5_type, null_value
 
 
 def _get_property_array_min_max_value(collection, property_array, const_value, discrete, min_value, max_value,
                                       categorical, null_value):
     if const_value is not None:
         return _get_property_array_min_max_const(const_value, collection.null_value, min_value, max_value, discrete)
     elif property_array is not None:
```

### Comparing `resqpy-4.8.5/resqpy/property/_collection_support.py` & `resqpy-4.8.6/resqpy/property/_collection_support.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/property/_property.py` & `resqpy-4.8.6/resqpy/property/_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/property/grid_property_collection.py` & `resqpy-4.8.6/resqpy/property/grid_property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/property/property_collection.py` & `resqpy-4.8.6/resqpy/property/property_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -2545,16 +2545,15 @@
 
         assert title, 'missing title when creating xml for property'
 
         #      log.debug('creating property node for ' + title)
         # currently assumes discrete properties to be 32 bit integers and continuous to be 64 bit reals
         # also assumes property_kind is one of the standard resqml property kinds; todo: allow local p kind node as optional arg
         support_root, support_uuid, ext_uuid = pcxml._create_xml_get_basics(self, discrete, points, const_value,
-                                                                            facet_type, null_value, support_uuid,
-                                                                            ext_uuid)
+                                                                            facet_type, support_uuid, ext_uuid)
 
         support_type = self.model.type_of_part(self.model.part_for_uuid(support_uuid))
         indexable_element = pcga._get_indexable_element(indexable_element, support_type)
         direction = None if facet_type is None or facet_type != 'direction' else facet
 
         if self.support is not None:
             pcxml._check_shape_list(self, indexable_element, direction, property_array, points, count)
@@ -2563,41 +2562,42 @@
         #    numpy data type matches discrete flag (and assumptions about precision)
         #    uom are valid units for property_kind
         assert property_kind, 'missing property kind when creating xml for property'
 
         if find_local_property_kinds and property_kind in ['continuous', 'discrete', 'categorical']:
             property_kind = title
 
-        pcga._get_property_type_details(self, discrete, string_lookup_uuid, points)
-        p_node, p_uuid = pcxml._create_xml_get_p_node(self, p_uuid)
+        d_or_c_text, xsd_type, hdf5_type, null_value = pcga._get_property_type_details(
+            discrete, string_lookup_uuid, points, null_value)
+        p_node, p_uuid = pcxml._create_xml_get_p_node(self, p_uuid, d_or_c_text)
 
         pcxml._create_xml_add_basics_to_p_node(self, p_node, title, originator, extra_metadata, source, count,
                                                indexable_element)
 
         pcxml._create_xml_realization_node(realization, p_node)
         related_time_series_node = pcxml._create_xml_time_series_node(self, time_series_uuid, time_index, p_node,
                                                                       support_uuid, support_type, support_root)
         property_kind_uuid = pcxml._create_xml_property_kind(self, p_node, find_local_property_kinds, property_kind,
                                                              uom, discrete, property_kind_uuid)
         pcxml._create_xml_patch_node(self, p_node, points, const_value, indexable_element, direction, p_uuid, ext_uuid,
-                                     expand_const_arrays)
+                                     expand_const_arrays, hdf5_type, xsd_type, null_value)
         pcxml._create_xml_facet_node(facet_type, facet, p_node)
 
         pcxml._create_xml_property_min_max(self, property_array, const_value, discrete, add_min_max, p_node, min_value,
-                                           max_value, string_lookup_uuid is not None, null_value, points)
+                                           max_value, string_lookup_uuid is not None, null_value, points, xsd_type)
 
         if discrete:
             sl_root = pcxml._create_xml_lookup_node(self, p_node, string_lookup_uuid)
         else:  # continuous
             pcxml._create_xml_uom_node(self, p_node, uom, property_kind, min_value, max_value, facet_type, facet, title,
                                        points)
             sl_root = None
         pcxml._create_xml_add_as_part(self, add_as_part, p_uuid, p_node, add_relationships, support_root,
                                       property_kind_uuid, related_time_series_node, sl_root, discrete,
-                                      string_lookup_uuid, const_value, ext_uuid)
+                                      string_lookup_uuid, const_value, ext_uuid, d_or_c_text)
 
         return p_node
 
     def create_property_set_xml(self,
                                 title,
                                 ps_uuid = None,
                                 originator = None,
```

### Comparing `resqpy-4.8.5/resqpy/property/property_common.py` & `resqpy-4.8.6/resqpy/property/property_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/property/property_kind.py` & `resqpy-4.8.6/resqpy/property/property_kind.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/property/string_lookup.py` & `resqpy-4.8.6/resqpy/property/string_lookup.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/property/well_interval_property.py` & `resqpy-4.8.6/resqpy/property/well_interval_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/property/well_interval_property_collection.py` & `resqpy-4.8.6/resqpy/property/well_interval_property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/property/well_log.py` & `resqpy-4.8.6/resqpy/property/well_log.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/property/well_log_collection.py` & `resqpy-4.8.6/resqpy/property/well_log_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/rq_import/__init__.py` & `resqpy-4.8.6/resqpy/rq_import/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/rq_import/_add_ab_properties.py` & `resqpy-4.8.6/resqpy/rq_import/_add_ab_properties.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/rq_import/_add_surfaces.py` & `resqpy-4.8.6/resqpy/rq_import/_add_surfaces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/rq_import/_grid_from_cp.py` & `resqpy-4.8.6/resqpy/rq_import/_grid_from_cp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/rq_import/_import_nexus.py` & `resqpy-4.8.6/resqpy/rq_import/_import_nexus.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/rq_import/_import_vdb_all_grids.py` & `resqpy-4.8.6/resqpy/rq_import/_import_vdb_all_grids.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/rq_import/_import_vdb_ensemble.py` & `resqpy-4.8.6/resqpy/rq_import/_import_vdb_ensemble.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/strata/__init__.py` & `resqpy-4.8.6/resqpy/strata/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/strata/_binary_contact_interpretation.py` & `resqpy-4.8.6/resqpy/strata/_binary_contact_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/strata/_geologic_unit_interpretation.py` & `resqpy-4.8.6/resqpy/strata/_geologic_unit_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/strata/_strata_common.py` & `resqpy-4.8.6/resqpy/strata/_strata_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/strata/_stratigraphic_column.py` & `resqpy-4.8.6/resqpy/strata/_stratigraphic_column.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/strata/_stratigraphic_column_rank.py` & `resqpy-4.8.6/resqpy/strata/_stratigraphic_column_rank.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/strata/_stratigraphic_unit_feature.py` & `resqpy-4.8.6/resqpy/strata/_stratigraphic_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/strata/_stratigraphic_unit_interpretation.py` & `resqpy-4.8.6/resqpy/strata/_stratigraphic_unit_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/surface/__init__.py` & `resqpy-4.8.6/resqpy/surface/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/surface/_base_surface.py` & `resqpy-4.8.6/resqpy/surface/_base_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/surface/_combined_surface.py` & `resqpy-4.8.6/resqpy/surface/_combined_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/surface/_mesh.py` & `resqpy-4.8.6/resqpy/surface/_mesh.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/surface/_pointset.py` & `resqpy-4.8.6/resqpy/surface/_pointset.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/surface/_surface.py` & `resqpy-4.8.6/resqpy/surface/_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/surface/_tri_mesh.py` & `resqpy-4.8.6/resqpy/surface/_tri_mesh.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/surface/_triangulated_patch.py` & `resqpy-4.8.6/resqpy/surface/_triangulated_patch.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/time_series/__init__.py` & `resqpy-4.8.6/resqpy/time_series/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/time_series/_any_time_series.py` & `resqpy-4.8.6/resqpy/time_series/_any_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/time_series/_from_nexus_summary.py` & `resqpy-4.8.6/resqpy/time_series/_from_nexus_summary.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/time_series/_functions.py` & `resqpy-4.8.6/resqpy/time_series/_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/time_series/_geologic_time_series.py` & `resqpy-4.8.6/resqpy/time_series/_geologic_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/time_series/_time_duration.py` & `resqpy-4.8.6/resqpy/time_series/_time_duration.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/time_series/_time_series.py` & `resqpy-4.8.6/resqpy/time_series/_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/unstructured/__init__.py` & `resqpy-4.8.6/resqpy/unstructured/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/unstructured/_hexa_grid.py` & `resqpy-4.8.6/resqpy/unstructured/_hexa_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/unstructured/_prism_grid.py` & `resqpy-4.8.6/resqpy/unstructured/_prism_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/unstructured/_pyramid_grid.py` & `resqpy-4.8.6/resqpy/unstructured/_pyramid_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/unstructured/_tetra_grid.py` & `resqpy-4.8.6/resqpy/unstructured/_tetra_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/unstructured/_unstructured_grid.py` & `resqpy-4.8.6/resqpy/unstructured/_unstructured_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/weights_and_measures/__init__.py` & `resqpy-4.8.6/resqpy/weights_and_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/weights_and_measures/nexus_units.py` & `resqpy-4.8.6/resqpy/weights_and_measures/nexus_units.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/weights_and_measures/weights_and_measures.py` & `resqpy-4.8.6/resqpy/weights_and_measures/weights_and_measures.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/well/__init__.py` & `resqpy-4.8.6/resqpy/well/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/well/_blocked_well.py` & `resqpy-4.8.6/resqpy/well/_blocked_well.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/well/_deviation_survey.py` & `resqpy-4.8.6/resqpy/well/_deviation_survey.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/well/_md_datum.py` & `resqpy-4.8.6/resqpy/well/_md_datum.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/well/_trajectory.py` & `resqpy-4.8.6/resqpy/well/_trajectory.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/well/_wellbore_frame.py` & `resqpy-4.8.6/resqpy/well/_wellbore_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/well/_wellbore_marker.py` & `resqpy-4.8.6/resqpy/well/_wellbore_marker.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/well/_wellbore_marker_frame.py` & `resqpy-4.8.6/resqpy/well/_wellbore_marker_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/well/blocked_well_frame.py` & `resqpy-4.8.6/resqpy/well/blocked_well_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/well/well_object_funcs.py` & `resqpy-4.8.6/resqpy/well/well_object_funcs.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/resqpy/well/well_utils.py` & `resqpy-4.8.6/resqpy/well/well_utils.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.5/PKG-INFO` & `resqpy-4.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resqpy
-Version: 4.8.5
+Version: 4.8.6
 Summary: Python API for working with RESQML models
 Home-page: https://github.com/bp/resqpy
 License: MIT
 Keywords: RESQML
 Author: BP
 Requires-Python: >=3.8.1,<3.11
 Classifier: Development Status :: 5 - Production/Stable
```

