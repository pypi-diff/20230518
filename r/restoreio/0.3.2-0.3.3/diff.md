# Comparing `tmp/restoreio-0.3.2.tar.gz` & `tmp/restoreio-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restoreio-0.3.2.tar", last modified: Tue May 16 22:15:29 2023, max compression
+gzip compressed data, was "restoreio-0.3.3.tar", last modified: Thu May 18 04:53:46 2023, max compression
```

## Comparing `restoreio-0.3.2.tar` & `restoreio-0.3.3.tar`

### file list

```diff
@@ -1,180 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.934703 restoreio-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-16 22:15:09.000000 restoreio-0.3.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 22:15:09.000000 restoreio-0.3.2/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-16 22:15:09.000000 restoreio-0.3.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-16 22:15:09.000000 restoreio-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-16 22:15:09.000000 restoreio-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-16 22:15:29.934703 restoreio-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-16 22:15:09.000000 restoreio-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.910703 restoreio-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.910703 restoreio-0.3.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.898703 restoreio-0.3.2/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.898703 restoreio-0.3.2/docs/source/_static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.910703 restoreio-0.3.2/docs/source/_static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/assets/fonts/synconew.regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/assets/fonts/syncopate.bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/assets/fonts/syncopate.regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.914703 restoreio-0.3.2/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/css/custom-anaconda-doc.css
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/css/custom-pydata.css
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.898703 restoreio-0.3.2/docs/source/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.914703 restoreio-0.3.2/docs/source/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-anaconda.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-anaconda.png
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-anaconda.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-pypi.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-pypi.png
--rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-pypi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/docs/source/_static/images/plots/
--rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/cor_cov.png
--rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/deviation.png
--rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/ensembles.png
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/ensembles_js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/gdop_coverage.png
--rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/kl_eigenvalues.png
--rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/kl_eigenvectors.png
--rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/orig_vel_and_error.png
--rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/rbf_kernel_2d.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/docs/source/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/js/custom-pydata.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/autosummary/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/autosummary/ndarray_subclass.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/autosummary/property.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/version.html
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/cite.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/generated/restoreio.restore.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/generated/restoreio.scan.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/notebooks/quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/recursive_glob.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 22:15:09.000000 restoreio-0.3.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.902703 restoreio-0.3.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/examples/restore/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/restore/main_VaryingNumModes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7838 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/restore/plot_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/restore/plot_fixed_size_artificial_mask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/restore/plot_variable_d_artificial_masks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21770 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/restore/plot_variable_size_artificial_masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.926703 restoreio-0.3.2/examples/uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/uncertainty_quant/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/uncertainty_quant/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/uncertainty_quant/_plot_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/uncertainty_quant/plot_gdop_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/uncertainty_quant/plot_js_divergence.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 22:15:09.000000 restoreio-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-16 22:15:09.000000 restoreio-0.3.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.926703 restoreio-0.3.2/restoreio/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.926703 restoreio-0.3.2/restoreio/_file_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_file_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_file_utilities/file_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.926703 restoreio-0.3.2/restoreio/_geography/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_geography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_geography/_find_alpha_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_geography/create_mask_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_geography/detect_land_ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_geography/locate_missing_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.926703 restoreio-0.3.2/restoreio/_inpaint/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_inpaint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_inpaint/_cast_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_inpaint/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_inpaint/_plot_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_inpaint/inpaint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.930703 restoreio-0.3.2/restoreio/_input_output/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_input_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_input_output/get_datetime_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_input_output/load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_input_output/load_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_input_output/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.930703 restoreio-0.3.2/restoreio/_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_parser/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_parser/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_parser/parse_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.930703 restoreio-0.3.2/restoreio/_plots/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_plot_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_plot_quiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_plot_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_plot_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_plot_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/plot_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.930703 restoreio-0.3.2/restoreio/_plots_uq/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/_refine_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/_shifted_colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_auto_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_cor_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_ensembles_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_kl_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_rbf_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.934703 restoreio-0.3.2/restoreio/_restore/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_restore/_make_array_masked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_restore/refine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_restore/restore_generated_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_restore/restore_main_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.934703 restoreio-0.3.2/restoreio/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_scripts/examples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40432 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_scripts/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.934703 restoreio-0.3.2/restoreio/_subset/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_subset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_subset/_array_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_subset/subset_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_subset/subset_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.934703 restoreio-0.3.2/restoreio/_uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/_statistical_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/generate_image_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/get_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.926703 restoreio-0.3.2/restoreio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-16 22:15:29.938703 restoreio-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-16 22:15:09.000000 restoreio-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.934703 restoreio-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-16 22:15:09.000000 restoreio-0.3.2/tests/test_restore_local_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-16 22:15:09.000000 restoreio-0.3.2/tests/test_restore_remote_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-16 22:15:09.000000 restoreio-0.3.2/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-16 22:15:09.000000 restoreio-0.3.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-18 04:53:30.000000 restoreio-0.3.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 04:53:30.000000 restoreio-0.3.3/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-18 04:53:30.000000 restoreio-0.3.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-18 04:53:30.000000 restoreio-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-18 04:53:30.000000 restoreio-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-18 04:53:46.819939 restoreio-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-18 04:53:30.000000 restoreio-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.803938 restoreio-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.803938 restoreio-0.3.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.799938 restoreio-0.3.3/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.799938 restoreio-0.3.3/docs/source/_static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.803938 restoreio-0.3.3/docs/source/_static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/assets/fonts/synconew.regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/assets/fonts/syncopate.bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/assets/fonts/syncopate.regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.803938 restoreio-0.3.3/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/css/custom-anaconda-doc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/css/custom-pydata.css
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.799938 restoreio-0.3.3/docs/source/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.803938 restoreio-0.3.3/docs/source/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-anaconda.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-anaconda.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-anaconda.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-pypi.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-pypi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-pypi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/docs/source/_static/images/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/cor_cov.png
+-rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/deviation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/ensembles.png
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/ensembles_js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/gdop_coverage.png
+-rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/kl_eigenvalues.png
+-rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/kl_eigenvectors.png
+-rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/orig_vel_and_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/images/plots/rbf_kernel_2d.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/docs/source/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_static/js/custom-pydata.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/autosummary/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/autosummary/ndarray_subclass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/autosummary/property.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/_templates/version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/cite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/cli_restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/cli_scan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/generated/restoreio.restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/generated/restoreio.scan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/notebooks/quick_start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-18 04:53:30.000000 restoreio-0.3.3/docs/source/recursive_glob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-18 04:53:30.000000 restoreio-0.3.3/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.799938 restoreio-0.3.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/examples/restore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/restore/main_VaryingNumModes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7838 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/restore/plot_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/restore/plot_fixed_size_artificial_mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/restore/plot_variable_d_artificial_masks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21770 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/restore/plot_variable_size_artificial_masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/examples/uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/uncertainty_quant/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/uncertainty_quant/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/uncertainty_quant/_plot_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/uncertainty_quant/plot_gdop_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-05-18 04:53:30.000000 restoreio-0.3.3/examples/uncertainty_quant/plot_js_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-18 04:53:30.000000 restoreio-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-18 04:53:30.000000 restoreio-0.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.811938 restoreio-0.3.3/restoreio/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22900 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio/_file_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_file_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_file_utilities/file_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio/_geography/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_geography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_geography/_find_alpha_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_geography/create_mask_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_geography/detect_land_ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_geography/locate_missing_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio/_inpaint/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_inpaint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_inpaint/_cast_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_inpaint/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_inpaint/_plot_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_inpaint/inpaint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio/_input_output/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_input_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_input_output/get_datetime_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_input_output/load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_input_output/load_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_input_output/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio/_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_parser/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_parser/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_parser/parse_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio/_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_plot_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_plot_quiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_plot_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_plot_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/_plot_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots/plot_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/restoreio/_plots_uq/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/_refine_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/_shifted_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_auto_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_cor_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_ensembles_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_kl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/restoreio/_restore/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_restore/_make_array_masked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_restore/refine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_restore/restore_generated_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_restore/restore_main_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/restoreio/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_scripts/examples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40958 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_scripts/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/restoreio/_server_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_server_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_server_utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_server_utils/terminate_with_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/restoreio/_subset/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_subset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_subset/_array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_subset/subset_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_subset/subset_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/restoreio/_uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/_statistical_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/generate_image_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-05-18 04:53:30.000000 restoreio-0.3.3/restoreio/_uncertainty_quant/get_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.815939 restoreio-0.3.3/restoreio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 04:53:46.000000 restoreio-0.3.3/restoreio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-18 04:53:46.819939 restoreio-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-18 04:53:30.000000 restoreio-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:53:46.819939 restoreio-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-18 04:53:30.000000 restoreio-0.3.3/tests/test_restore_local_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-18 04:53:30.000000 restoreio-0.3.3/tests/test_restore_remote_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-18 04:53:30.000000 restoreio-0.3.3/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-18 04:53:30.000000 restoreio-0.3.3/tox.ini
```

### Comparing `restoreio-0.3.2/LICENSE.txt` & `restoreio-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/MANIFEST.in` & `restoreio-0.3.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/PKG-INFO` & `restoreio-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.3.2
+Version: 0.3.3
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
```

### Comparing `restoreio-0.3.2/README.rst` & `restoreio-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/Makefile` & `restoreio-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/make.bat` & `restoreio-0.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_inspect.py` & `restoreio-0.3.3/docs/source/_inspect.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/assets/fonts/synconew.regular.ttf` & `restoreio-0.3.3/docs/source/_static/assets/fonts/synconew.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/assets/fonts/syncopate.bold.ttf` & `restoreio-0.3.3/docs/source/_static/assets/fonts/syncopate.bold.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/assets/fonts/syncopate.regular.ttf` & `restoreio-0.3.3/docs/source/_static/assets/fonts/syncopate.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/css/custom-anaconda-doc.css` & `restoreio-0.3.3/docs/source/_static/css/custom-anaconda-doc.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/css/custom-pydata.css` & `restoreio-0.3.3/docs/source/_static/css/custom-pydata.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/css/custom.css` & `restoreio-0.3.3/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/icons/favicon.ico` & `restoreio-0.3.3/docs/source/_static/images/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/icons/logo-anaconda.ico` & `restoreio-0.3.3/docs/source/_static/images/icons/logo-anaconda.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/icons/logo-anaconda.png` & `restoreio-0.3.3/docs/source/_static/images/icons/logo-anaconda.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/icons/logo-anaconda.svg` & `restoreio-0.3.3/docs/source/_static/images/icons/logo-anaconda.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/icons/logo-pypi.ico` & `restoreio-0.3.3/docs/source/_static/images/icons/logo-pypi.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/icons/logo-pypi.png` & `restoreio-0.3.3/docs/source/_static/images/icons/logo-pypi.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/icons/logo-pypi.svg` & `restoreio-0.3.3/docs/source/_static/images/icons/logo-pypi.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-dark.png` & `restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-dark.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-dark.svg` & `restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-dark.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-light.png` & `restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-light.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-light.svg` & `restoreio-0.3.3/docs/source/_static/images/icons/logo-restoreio-light.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/plots/cor_cov.png` & `restoreio-0.3.3/docs/source/_static/images/plots/cor_cov.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/plots/deviation.png` & `restoreio-0.3.3/docs/source/_static/images/plots/deviation.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/plots/ensembles.png` & `restoreio-0.3.3/docs/source/_static/images/plots/ensembles.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/plots/ensembles_js_distance.png` & `restoreio-0.3.3/docs/source/_static/images/plots/ensembles_js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/plots/gdop_coverage.png` & `restoreio-0.3.3/docs/source/_static/images/plots/gdop_coverage.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/plots/js_distance.png` & `restoreio-0.3.3/docs/source/_static/images/plots/js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/plots/kl_eigenvalues.png` & `restoreio-0.3.3/docs/source/_static/images/plots/kl_eigenvalues.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/plots/kl_eigenvectors.png` & `restoreio-0.3.3/docs/source/_static/images/plots/kl_eigenvectors.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/plots/orig_vel_and_error.png` & `restoreio-0.3.3/docs/source/_static/images/plots/orig_vel_and_error.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/images/plots/rbf_kernel_2d.png` & `restoreio-0.3.3/docs/source/_static/images/plots/rbf_kernel_2d.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_static/js/custom-pydata.js` & `restoreio-0.3.3/docs/source/_static/js/custom-pydata.js`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_templates/autosummary/class.rst` & `restoreio-0.3.3/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_templates/layout.html` & `restoreio-0.3.3/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/_templates/version.html` & `restoreio-0.3.3/docs/source/_templates/version.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/cite.rst` & `restoreio-0.3.3/docs/source/cite.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/conf.py` & `restoreio-0.3.3/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,15 @@
     'numpydoc',                               # either use napoleon or numpydoc
     'sphinx_design',
     'sphinx_multitoc_numbering',
     'sphinx-prompt',
     'sphinx_copybutton',
     'nbsphinx',
    'sphinx_gallery.load_style',
+   'sphinxarg.ext',
 ]
 
 # Inner-sphinx to cross-reference imate packahe
 intersphinx_mapping = {
     'imate': ('https://ameli.github.io/imate', None),
     'detkit': ('https://ameli.github.io/detkit', None),
     'special_functions': ('https://ameli.github.io/special_functions', None),
```

### Comparing `restoreio-0.3.2/docs/source/custom_domain.py` & `restoreio-0.3.3/docs/source/custom_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/examples.rst` & `restoreio-0.3.3/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/index.rst` & `restoreio-0.3.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/install.rst` & `restoreio-0.3.3/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/notebooks/quick_start.ipynb` & `restoreio-0.3.3/docs/source/notebooks/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/docs/source/recursive_glob.py` & `restoreio-0.3.3/docs/source/recursive_glob.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/examples/restore/main_VaryingNumModes.py` & `restoreio-0.3.3/examples/restore/main_VaryingNumModes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/examples/restore/plot_coverage.py` & `restoreio-0.3.3/examples/restore/plot_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/examples/restore/plot_fixed_size_artificial_mask.py` & `restoreio-0.3.3/examples/restore/plot_fixed_size_artificial_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/examples/restore/plot_variable_d_artificial_masks.py` & `restoreio-0.3.3/examples/restore/plot_variable_d_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/examples/restore/plot_variable_size_artificial_masks.py` & `restoreio-0.3.3/examples/restore/plot_variable_size_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/examples/uncertainty_quant/_display_utilities.py` & `restoreio-0.3.3/examples/uncertainty_quant/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/examples/uncertainty_quant/_draw_map.py` & `restoreio-0.3.3/examples/uncertainty_quant/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/examples/uncertainty_quant/_plot_utilities.py` & `restoreio-0.3.3/examples/uncertainty_quant/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/examples/uncertainty_quant/plot_gdop_coverage.py` & `restoreio-0.3.3/examples/uncertainty_quant/plot_gdop_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/examples/uncertainty_quant/plot_js_divergence.py` & `restoreio-0.3.3/examples/uncertainty_quant/plot_js_divergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/__main__.py` & `restoreio-0.3.3/restoreio/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 
 
 # =======
 # Imports
 # =======
 
 import numpy
-import sys
 import warnings
 
 from ._parser import parse_arguments
 from ._subset import subset_domain, subset_datetime
 from ._input_output import load_dataset, load_variables, get_datetime_info, \
         write_output_file
 from ._geography import detect_land_ocean
 from ._file_utilities import get_fullpath_input_filenames_list, \
         get_fullpath_output_filenames_list, archive_multiple_files
 from ._restore import restore_main_ensemble, restore_generated_ensembles
-# from restoreio._restore import refine_grid
+from ._server_utils import globals, terminate_with_error
 
 __all__ = ['restore']
 
 
 # =================
 # process arguments
 # =================
@@ -50,37 +49,40 @@
     if detect_land == 0:
         fill_coast = False
 
     # Check Processing multiple file
     if ((min_file_index != '') and (max_file_index != '')):
 
         if ((min_file_index == '') or (max_file_index == '')):
-            raise ValueError('To process multiple files, both min and max ' +
-                             'file iterator should be specified.')
+            terminate_with_error(
+                'To process multiple files, both min and max file iterator ' +
+                'should be specified.')
 
     # A time interval and single time point cannot be both specified.
     if (min_time != '' or max_time != '') and (time != ''):
-        raise ValueError('When "time" argument is specified, the other time ' +
-                         'arguments "min_time" and "max_time" cannot be ' +
-                         'specified and vice versa.')
+        terminate_with_error(
+            'When "time" argument is specified, the other time arguments ' +
+            '"min_time" and "max_time" cannot be specified and vice versa.')
 
     # When uncertainty quantification is used, only a single time point should
     # be given, not an interval of time.
     if (uncertainty_quant is True) and (min_time != '' or max_time != ''):
-        raise ValueError('When uncertainty quantification is enabled, a time' +
-                         'interval cannot be specified, rather a single ' +
-                         'time should be specified using "time" argument.')
+        terminate_with_error(
+            'When uncertainty quantification is enabled, a time interval ' +
+            'cannot be specified, rather a single time should be specified ' +
+            'using "time" argument.')
 
     # When plotting, only a single time point can be plotted
     if (plot is True) and (((min_time != '') or (max_time != '')) or
        ((min_time == '') and (max_time == '') and (time == ''))):
-        raise ValueError('When plotting is enabled, a time interval with ' +
-                         '"min_time" or "max_time" arguments should not be ' +
-                         'given. Rather, only a single time point can be ' +
-                         'plotted that is specified with "time" argument.')
+        terminate_with_error(
+            'When plotting is enabled, a time interval with "min_time" or ' +
+            '"max_time" arguments should not be given. Rather, only a ' +
+            'single time point can be plotted that is specified with ' +
+            '"time" argument.')
 
     return fill_coast
 
 
 # =======
 # Restore
 # =======
@@ -295,19 +297,25 @@
 
     terminate ; bool, default=False
         If `True`, the program exists with code 1. This is useful when this
         package is executed on a server to pass exit signals to a Node
         application. On the downside, this option causes an interactive python
         environment to both terminate the script and the python environment
         itself. To avoid this, set this option to `False`. In this case, upon
-        an error, the ``ValueError` is raised, which cases the script to
+        an error, the ``ValueError`` is raised, which cases the script to
         terminate, however, an interactive python environment will not be
         exited.
     """
 
+    # Define global variable for terminate with error
+    if terminate:
+        globals.terminate = True
+    else:
+        globals.terminate = False
+
     # Check arguments
     fill_coast = process_arguments(
             detect_land, min_file_index, max_file_index, fill_coast,
             time, min_time, max_time, uncertainty_quant, plot)
 
     # Get list of all separate input files to process
     fullpath_input_filenames_list, input_base_filenames_list = \
@@ -339,23 +347,22 @@
         warnings.filterwarnings('ignore')
 
         # Get datetime info from datetime netcdf object
         datetime_info = get_datetime_info(datetime_obj)
 
         # Subset time
         min_datetime_index, max_datetime_index = subset_datetime(
-            datetime_info, min_time, max_time, time, terminate)
+            datetime_info, min_time, max_time, time)
 
         datetime_info['array'] = \
             datetime_info['array'][min_datetime_index:max_datetime_index+1]
 
         # Subset domain
         min_lon_index, max_lon_index, min_lat_index, max_lat_index = \
-            subset_domain(lon_obj, lat_obj, min_lon, max_lon, min_lat, max_lat,
-                          terminate)
+            subset_domain(lon_obj, lat_obj, min_lon, max_lon, min_lat, max_lat)
         lon = lon_obj[min_lon_index:max_lon_index+1]
         lat = lat_obj[min_lat_index:max_lat_index+1]
 
         # if the velocity arrays have depth dimension, use only the first index
         depth_index = 0
         vel_array_dim = len(east_vel_obj.shape)
 
@@ -383,16 +390,16 @@
             V_all_times = north_vel_obj[
                     min_datetime_index:max_datetime_index+1,
                     depth_index,
                     min_lat_index:max_lat_index+1,
                     min_lon_index:max_lon_index+1]
 
         else:
-            raise ValueError('Velocity arrays should have three or four' +
-                             'dimensions.')
+            terminate_with_error('Velocity arrays should have three or four' +
+                                 'dimensions.')
 
         # Velocity error
         if east_vel_error_obj is None:
             # When None, no uncertainty quantification should be used.
             U_error_all_times = None
             V_error_all_times = None
 
@@ -427,16 +434,17 @@
                 V_error_all_times = north_vel_obj[
                         min_datetime_index:max_datetime_index+1,
                         depth_index,
                         min_lat_index:max_lat_index+1,
                         min_lon_index:max_lon_index+1]
 
             else:
-                raise ValueError('Velocity error or DGOP arrays should have ' +
-                                 'three or four dimensions.')
+                terminate_with_error(
+                    'Velocity error or DGOP arrays should have three or ' +
+                    'four dimensions.')
 
         # Refinement
         # Do not use this, because (1) lon and lat for original and refined
         # grids will be different, hence the plot functions should be aware of
         # these two grids, and (2) inpainted results on refined grid is poor.
         # if refine_grid != 1:
         #     lon, lat, U_all_times, V_all_times = refine_grid(
@@ -531,15 +539,15 @@
 
     # Converting all warnings to error
     # warnings.simplefilter('error', UserWarning)
     warnings.filterwarnings("ignore", category=numpy.VisibleDeprecationWarning)
     warnings.filterwarnings("ignore", category=DeprecationWarning)
 
     # Parse arguments
-    arguments = parse_arguments(sys.argv)
+    arguments = parse_arguments()
 
     # Main function
     restore(**arguments)
 
 
 # ===========
 # Script main
```

### Comparing `restoreio-0.3.2/restoreio/_file_utilities/__init__.py` & `restoreio-0.3.3/restoreio/_file_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_file_utilities/file_utilities.py` & `restoreio-0.3.3/restoreio/_file_utilities/file_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_geography/__init__.py` & `restoreio-0.3.3/restoreio/_geography/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_geography/_find_alpha_shapes.py` & `restoreio-0.3.3/restoreio/_geography/_find_alpha_shapes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_geography/create_mask_info.py` & `restoreio-0.3.3/restoreio/_geography/create_mask_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_geography/detect_land_ocean.py` & `restoreio-0.3.3/restoreio/_geography/detect_land_ocean.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_geography/locate_missing_data.py` & `restoreio-0.3.3/restoreio/_geography/locate_missing_data.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_inpaint/_cast_types.py` & `restoreio-0.3.3/restoreio/_inpaint/_cast_types.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_inpaint/_image.py` & `restoreio-0.3.3/restoreio/_inpaint/_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_inpaint/_plot_image.py` & `restoreio-0.3.3/restoreio/_inpaint/_plot_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_inpaint/inpaint.py` & `restoreio-0.3.3/restoreio/_inpaint/inpaint.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_input_output/__init__.py` & `restoreio-0.3.3/restoreio/_input_output/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_input_output/get_datetime_info.py` & `restoreio-0.3.3/restoreio/_input_output/get_datetime_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_input_output/load_dataset.py` & `restoreio-0.3.3/restoreio/_input_output/load_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Imports
 # =======
 
 import sys
 import netCDF4
 import pyncml
 import os.path
+from .._server_utils import terminate_with_error
 
 try:
     # Python 3
     from urllib.parse import urlparse
 except ImportError:
     # python 2
     from urlparse import urlparse
@@ -75,51 +76,54 @@
         except BaseException as error:
             print('ERROR: Can not read local netcdf file: ' + filename)
             raise error
 
         return nc
 
     else:
-        raise ValueError("File format %s is not recognized." % file_extension)
+        terminate_with_error(
+            "File format %s is not recognized." % file_extension)
 
 
 # ===================
 # Load Remote Dataset
 # ===================
 
 def load_remote_dataset(url):
     """
     url can be point to a *.nc or *.ncml file.
     """
 
     # Check URL is opendap
     if (url.startswith('http://') is False) and \
        (url.startswith('https://') is False):
-        raise ValueError('Input data URL does not seem to be a URL. ' +
-                         'A URL should start with "http://" or "https://".')
+        terminate_with_error(
+            'Input data URL does not seem to be a URL. A URL should start ' +
+            'with "http://" or "https://".')
 
     elif ("/thredds/dodsC/" not in url) and ("opendap" not in url):
-        raise ValueError('Input data URL is not an OpenDap URL or is not ' +
-                         'hosted on a THREDDs server. Check if your data ' +
-                         'URL contains "/thredds/dodsC/" or "/opendap/".')
+        terminate_with_error(
+            'Input data URL is not an OpenDap URL or is not hosted on a ' +
+            'THREDDs server. Check if your data URL contains ' +
+            '"/thredds/dodsC/" or "/opendap/".')
 
     # Check file extension
     file_extension = os.path.splitext(url)[1]
 
     # Case of zipped files (get the correct file extension before the '.gz')
     if file_extension == ".gz":
         file_extension = os.path.splitext(url[:-3])[1]
 
     # Note that some opendap urls do not even have a file extension
     if file_extension != "":
 
         # If a file extension exists, check if it is a standard netcdf file
         if file_extension not in \
                 ['.nc', '.ncd', '.nc.gz', '.ncml', '.ncml.gz']:
-            raise ValueError(
+            terminate_with_error(
                 'The input data URL is not an netcdf file. The URL should ' +
                 'end with ".nc", ".ncd", ".nc.gz", ".ncml", ".ncml.gz", or ' +
                 'without file extension.')
 
     try:
 
         # nc = open_url(url)
@@ -141,16 +145,17 @@
 
     1. load_local_dataset: For files where the input_filename is a path on the
        local machine.
     2. load_remote_dataset: For files remotely where input_filename is a url.
     """
 
     if input_filename == '':
-        raise ValueError('Input data is empty. You should provide a local' +
-                         'filename or an OpenDap URL or remote data.')
+        terminate_with_error(
+            'Input data is empty. You should provide a local filename or an ' +
+            'OpenDap URL or remote data.')
 
     # Check if the input_filename has a "host" name
     if bool(urlparse(input_filename).netloc):
         # input_filename is a url
         return load_remote_dataset(input_filename)
     else:
         # input_filename is a path
```

### Comparing `restoreio-0.3.2/restoreio/_input_output/load_variables.py` & `restoreio-0.3.3/restoreio/_input_output/load_variables.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_input_output/writer.py` & `restoreio-0.3.3/restoreio/_input_output/writer.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_parser/examples.py` & `restoreio-0.3.3/restoreio/_parser/examples.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_parser/formatter.py` & `restoreio-0.3.3/restoreio/_parser/formatter.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_parser/parse_arguments.py` & `restoreio-0.3.3/restoreio/_parser/parse_arguments.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,21 +15,24 @@
 from .formatter import WrappedNewlineFormatter
 from .examples import examples
 from ..__version__ import __version__
 
 __all__ = ['parse_arguments']
 
 
-# ==========
-# Parse Args
-# ==========
+# =============
+# Create Parser
+# ============
 
-def parse_arguments(argv):
+def create_parser():
     """
-    Parse the user's command line arguments.
+    Creates parser object.
+
+    The parser object can be used in both parsing arguments and to generate
+    Sphinx documentation for the command line interface (CLI).
     """
 
     # Instantiate the parser
     description = 'Restore incomplete oceanographic dataset. ' + \
         '"restore" is provided by "restoreio" python package.'
     epilog = examples
     # formatter_class = argparse.RawTextHelpFormatter
@@ -49,61 +52,63 @@
     # Add back help
     optional.add_argument('-h', '--help', action='help',
                           default=argparse.SUPPRESS,
                           help='show this help message and exit')
 
     # Input filename
     help_input = """
-    Input filename. This can be either the path to a local file or the url to
-    a remote dataset. The file extension should be *.nc or *.ncml only.
+    Input filename. This can be either the path to a local file or the URL to
+    a remote dataset. The file or URL may or may not have a file extension.
+    However, if the file does have an extension, the file extension should be
+    either ``.nc``, ``.ncd``, ``.nc.gz``, ``.ncml``, or ``*.ncml.gz`` only.
     """
     required.add_argument('-i', type=str, help=help_input, metavar='INPUT',
                           required=True)
 
     # Output filename
     help_output = """
-    Output filename. This can be either the path to a local file or the url to
-    a remote dataset. The file extension should be *.nc or *.ncml only. If
-    no output file is provided, the output filename is constructed by adding
-    the word '_restored' at the end of the input filename.
+    Output filename. This can be either the path to a local file or the URL to
+    a remote dataset. The file extension should be ``.nc`` or ``.ncml`` only.
+    If no output file is provided, the output filename is constructed by adding
+    the word ``_restored`` at the end of the input filename.
     """
     required.add_argument('-o', type=str, default='', metavar='OUTPUT',
                           help=help_output, required=True)
 
     # Min Longitude
     help_min_lon = """
     Minimum longitude in the unit of degrees to subset the processing domain.
-    If not provided or set to `nan`, the minimum longitude of the input data
+    If not provided or set to ``nan``, the minimum longitude of the input data
     is considered.
     """
     optional.add_argument('--min-lon', type=float, default=float('nan'),
                           metavar='MIN_LON', help=help_min_lon)
 
     # Mix Longitude
     help_max_lon = """
     Maximum longitude in the unit of degrees to subset the processing domain.
-    If not provided or set to `nan`, the maximum longitude of the input data
+    If not provided or set to ``nan``, the maximum longitude of the input data
     is considered.
     """
     optional.add_argument('--max-lon', type=float, default=float('nan'),
                           metavar='MAX_LON', help=help_max_lon)
 
     # Min Latitude
     help_min_lat = """
     Minimum latitude in the unit of degrees to subset the processing domain.
-    If not provided or set to `nan`, the minimum latitude of the input data
+    If not provided or set to ``nan``, the minimum latitude of the input data
     is considered.
     """
     optional.add_argument('--min-lat', type=float, default=float('nan'),
                           metavar='MIN_LAT', help=help_min_lat)
 
     # Mix Latitude
     help_max_lat = """
     Maximum latitude in the unit of degrees to subset the processing domain.
-    If not provided or set to `nan`, the maximum latitude of the input data
+    If not provided or set to ``nan``, the maximum latitude of the input data
     is considered.
     """
     optional.add_argument('--max-lat', type=float, default=float('nan'),
                           metavar='MAX_LAT', help=help_max_lat)
 
     # Min time
     help_min_time = """
@@ -120,40 +125,40 @@
     """
     optional.add_argument('--min-time', type=str, default='',
                           metavar="MIN_TIME", help=help_min_time)
 
     # Max time
     help_max_time = """
     The end of the time interval within the dataset times to be processed. The
-    time should be provided as a string with the format yyyy-mm-ddTHH:MM:SS
-    where yyyy is year, mm is month, dd is day, HH is hour from 00 to 23, MM is
-    minutes and SS is seconds. If the given time does not exactly match any
-    time in the dataset, the closest data time is used. If this argument is not
-    given, the latest available time in the dataset is used. Note that
-    specifying a time interval cannot be used together with uncertainty
-    quantification (using option '-u'). For this case, use '--time' argument
-    instead which specifies a single time point.
+    time should be provided as a string with the format ``yyyy-mm-ddTHH:MM:SS``
+    where ``yyyy`` is year, ``mm`` is month, ``dd`` is day, ``HH`` is hour from
+    `00` to `23`, ``MM`` is minutes and ``SS`` is seconds. If the given time
+    does not exactly match any time in the dataset, the closest data time is
+    used. If this argument is not given, the latest available time in the
+    dataset is used. Note that specifying a time interval cannot be used
+    together with uncertainty quantification (using option ``-u``). For this
+    case, use ``--time`` argument instead which specifies a single time point.
     (default: %(default)s)
     """
     optional.add_argument('--max-time', type=str, default='',
                           metavar="MAX_TIME", help=help_max_time)
 
     # time
     help_time = """
     Specify a single time point to process. The time should be provided as a
-    string with the format yyyy-mm-ddTHH:MM:SS where yyyy is year, mm is month,
-    dd is day, HH is hour from 00 to 23, MM is minutes and SS is seconds. If
-    the given time does not exactly match any time in the dataset, the closest
-    data time is used. If this option is not given, the latest available time
-    in the dataset is used. This option sets both '--min-time' and '--max-time'
-    to this given time value. The argument is useful when performing
-    uncertainty quantification (using argument '-u') or plotting (using
-    argument '-p') as these require a single time, rather than a time interval.
-    In contrary, to specify a time interval, use '--min-time' and '--max-time'
-    arguments.
+    string with the format ``yyyy-mm-ddTHH:MM:SS`` where ``yyyy`` is year,
+    ``mm`` is month, ``dd`` is day, ``HH`` is hour from `00` to `23`, ``MM`` is
+    minutes and ``SS`` is seconds. If the given time does not exactly match any
+    time in the dataset, the closest data time is used. If this option is not
+    given, the latest available time in the dataset is used. This option sets
+    both ``--min-time`` and ``--max-time`` to this given time value. The
+    argument is useful when performing uncertainty quantification (using
+    argument ``-u``) or plotting (using argument ``-p``) as these require a
+    single time, rather than a time interval. In contrary, to specify a time
+    interval, use ``--min-time`` and ``--max-time`` arguments.
     (default: %(default)s)
     """
     optional.add_argument('-t', '--time', type=str, default='',
                           metavar="TIME", help=help_time)
 
     # diffusivity
     help_diffusivity = """
@@ -170,47 +175,48 @@
     solution independent of direction.
     """
     optional.add_argument('-s', action='store_true', help=help_sweep)
 
     # Plot
     help_plot = """
     Plots the results. In this case, instead of iterating through all time
-    frames, only one time frame (given with option -t) is restored and plotted.
-    If in addition, the uncertainty quantification is enabled (with option -u),
-    the statistical analysis for the given time frame is also plotted.
+    frames, only one time frame (given with option ``--time``) is restored and
+    plotted. If in addition, the uncertainty quantification is enabled (with
+    option ``-u``), the statistical analysis for the given time frame is also
+    plotted.
     """
     optional.add_argument('-p', action='store_true', help=help_plot)
 
     # Save
     help_save = """
     If `True`, the plots are not displayed, rather are saved in the current
     directory as ``.pdf`` and ``.svg`` format. This option is useful when
     executing this script in an environment without display (such as remote
     cluster). If `False`, the generated plots will be displayed.
     """
-    optional.add_argument('-s', action='store_true', help=help_save)
+    optional.add_argument('-S', action='store_true', help=help_save)
 
     # Detect land
     help_detect_land = """
     Detect land and exclude it from ocean's missing data points. This option
     should be an boolean or an integer with the following values
     (default: %(default)s):
 
-    - False: Same as 0. See below.
+    - ``False``: Same as ``0``. See below.
 
-    - True: Same as 2. See below.
+    - ``True``: Same as ``2``. See below.
 
-    - 0: Does not detect land from ocean. All land points are assumed to be a
-         part of ocean's missing points.
+    - ``0``: Does not detect land from ocean. All land points are assumed to be
+        a part of ocean's missing points.
 
-    - 1: Detect land. Most accurate, slowest.
+    - ``1``: Detect land. Most accurate, slowest.
 
-    - 2: Detect land. Less accurate, fastest (preferred method).
+    - ``2``: Detect land. Less accurate, fastest (preferred method).
 
-    - 3: Detect land. Currently this option is not fully implemented.
+    - ``3``: Detect land. Currently this option is not fully implemented.
     """
     optional.add_argument('-L', choices=[0, 1, 2, 3, False, True],
                           default=True, type=int, metavar='DETECT_LAND',
                           help=help_detect_land)
 
     # Include near shore
     help_fill_coast = """
@@ -226,80 +232,81 @@
     """
     optional.add_argument('-c', action="store_true", help=help_convex_hull)
 
     # Alpha
     help_alpha = """
     The alpha number for alpha shape. If not specified or a negative number,
     this value is computed automatically. This option is only relevant to
-    concave shapes. This option is ignored if convex shape is used with '-c'
+    concave shapes. This option is ignored if convex shape is used with ``-c``
     option.
     """
     optional.add_argument('-a', default=-1, type=float, metavar="ALPHA",
                           help=help_alpha)
 
     # Refine
     help_refine_grid = """
     Refines the grid by increasing the number of points on each axis by a
     multiple of a given integer. If this option is set to 1, no refinement is
     performed. If set to integer n, the number of grid points is refined by
-    n^2 times (that is n times on each axis).
+    `n^2` times (that is `n` times on each axis).
     (default: %(default)s)
     """
     optional.add_argument('-r', type=int, default=1, metavar="REFINE",
                           help=help_refine_grid)
 
     # Uncertainty quantification
     help_uncertainty_quant = """
-    Enables uncertainty quantification for the time frame given in option -t.
-    This either produces results in output file as given in option -o, or plots
-    the results if the option -p is specified.
+    Enables uncertainty quantification for the time frame given in option
+    ``--time``. This either produces results in output file as given in option
+    ``-o``, or plots the results if the option ``-p`` is specified.
     """
     optional.add_argument('-u', action="store_true",
                           help=help_uncertainty_quant)
 
     # Number of ensembles
     help_num_ensembles = """
     Number of ensembles used for uncertainty quantification. This option is
-    only relevant to uncertainty quantification (when -u is used).
+    only relevant to uncertainty quantification (when ``-u`` is used).
     (default: %(default)s)
     """
     optional.add_argument('-e', type=int, default=1000, metavar="NUM_ENSEMBLE",
                           help=help_num_ensembles)
 
     # Number of modes
     help_ratio_num_modes = """
     Ratio of the number of KL eigen-modes to be used in the truncation of the
     KL expansion. The ratio is defined by the number of modes to be used over
-    the total number of modes. The ratio is a number between 0 and 1. For
-    instance, if set to 1, all modes are used, hence the KL expansion is not
-    truncated. If set to 0.5, half of the number of modes are used. This option
-    is only relevant to uncertainty quantification (when -u is used).
+    the total number of modes. The ratio is a number between `0` and `1`. For
+    instance, if set to `1`, all modes are used, hence the KL expansion is not
+    truncated. If set to `0.5`, half of the number of modes are used. This
+    option is only relevant to uncertainty quantification (when ``-u`` is
+    used).
     """
     optional.add_argument('-m', type=float, default=1.0, metavar="NUM_MODES",
                           help=help_ratio_num_modes)
 
     # Kernel window
     help_kernel_width = """
     Window of the kernel to estimate covariance of data. The window width
     should be given by the integer number of pixels (data points). The non-zero
     extent of the kernel a square area with twice the window length in both
     longitude and latitude directions. This option is only relevant to
-    uncertainty quantification (when -u is used).
+    uncertainty quantification (when ``-u`` is used).
     (default: %(default)s)
     """
     optional.add_argument('-w', default=5, type=int, metavar="WINDOW",
                           help=help_kernel_width)
 
     # Scale error
     help_scale_error = """
     Scale velocity error of the input data by a factor. Often, the input
     velocity error is the dimensionless GDOP which needs to be scaled by the
     standard deviation of the velocity error to represent the actual velocity
     error. This value scales the error. This option is only relevant to
-    uncertainty quantification (when -u is used).
+    uncertainty quantification (when ``-u`` is used).
     (default: %(default)s)
     """
     optional.add_argument('-E', default=0.08, type=float,
                           metavar="SCALE_ERROR", help=help_scale_error)
 
     # Start file index
     help_min_file_index = """
@@ -329,28 +336,43 @@
 
     # Terminate
     help_terminate = """
     If `True`, the program exists with code 1. This is useful when this
     package is executed on a server to pass exit signals to a Node application.
     On the downside, this option causes an interactive python environment to
     both terminate the script and the python environment itself. To avoid this,
-    set this option to `False`. In this case, upon an error, the ``ValueError`
+    set this option to `False`. In this case, upon an error, the ``ValueError``
     is raised, which cases the script to terminate, however, an interactive
     python environment will not be exited.
     """
     optional.add_argument('-T', action='store_true', help=help_terminate)
 
     # Version
     help_version = """
     Prints version.
     """
     version = '%(prog)s {version}'.format(version=__version__)
     parser.add_argument('-V', '--version', action='version', version=version,
                         help=help_version)
 
+    return parser
+
+
+# ===============
+# Parse Arguments
+# ===============
+
+def parse_arguments():
+    """
+    Parse the user's command line arguments.
+    """
+
+    # Create parser object
+    parser = create_parser()
+
     # Parse arguments. Here args is a namespace
     args = parser.parse_args()
 
     # Convert namespace to dictionary
     # args = vars(args)
 
     # Output dictionary
```

### Comparing `restoreio-0.3.2/restoreio/_plots/_display_utilities.py` & `restoreio-0.3.3/restoreio/_plots/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots/_draw_map.py` & `restoreio-0.3.3/restoreio/_plots/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots/_plot_grid.py` & `restoreio-0.3.3/restoreio/_plots/_plot_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots/_plot_quiver.py` & `restoreio-0.3.3/restoreio/_plots/_plot_quiver.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots/_plot_streamlines.py` & `restoreio-0.3.3/restoreio/_plots/_plot_streamlines.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots/_plot_utilities.py` & `restoreio-0.3.3/restoreio/_plots/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots/_plot_velocities.py` & `restoreio-0.3.3/restoreio/_plots/_plot_velocities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots/plot_results.py` & `restoreio-0.3.3/restoreio/_plots/plot_results.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots_uq/__init__.py` & `restoreio-0.3.3/restoreio/_plots_uq/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots_uq/_refine_mask.py` & `restoreio-0.3.3/restoreio/_plots_uq/_refine_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots_uq/_shifted_colormap.py` & `restoreio-0.3.3/restoreio/_plots_uq/_shifted_colormap.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots_uq/plot_auto_correlation.py` & `restoreio-0.3.3/restoreio/_plots_uq/plot_auto_correlation.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots_uq/plot_convergence.py` & `restoreio-0.3.3/restoreio/_plots_uq/plot_convergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots_uq/plot_cor_cov.py` & `restoreio-0.3.3/restoreio/_plots_uq/plot_cor_cov.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots_uq/plot_ensembles_stat.py` & `restoreio-0.3.3/restoreio/_plots_uq/plot_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots_uq/plot_kl_transform.py` & `restoreio-0.3.3/restoreio/_plots_uq/plot_kl_transform.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots_uq/plot_rbf_kernel.py` & `restoreio-0.3.3/restoreio/_plots_uq/plot_rbf_kernel.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py` & `restoreio-0.3.3/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_restore/__init__.py` & `restoreio-0.3.3/restoreio/_restore/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_restore/_make_array_masked.py` & `restoreio-0.3.3/restoreio/_restore/_make_array_masked.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_restore/refine_grid.py` & `restoreio-0.3.3/restoreio/_restore/refine_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_restore/restore_generated_ensembles.py` & `restoreio-0.3.3/restoreio/_restore/restore_generated_ensembles.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from .._inpaint import inpaint_missing_points_inside_domain
 from .._geography import locate_missing_data, create_mask_info
 from .._uncertainty_quant import generate_image_ensembles, \
         get_ensembles_stat
 from .._plots_uq import plot_ensembles_stat, plot_convergence
 from ._make_array_masked import make_array_masked
+from .._server_utils import terminate_with_error
 
 __all__ = ['restore_generated_ensembles']
 
 
 # ============================
 # Restore Ensemble Per Process
 # ============================
@@ -137,21 +138,22 @@
 
     # Get one time frame of velocities
     U_one_time = make_array_masked(U_all_times[time_index, :, :])
     V_one_time = make_array_masked(V_all_times[time_index, :, :])
 
     # Check if data has errors of velocities variable
     if (U_error_all_times is None):
-        raise ValueError('Input netCDF data does not have East ' +
-                         'Velocity error, which is needed for ' +
-                         'uncertainty quantification.')
+        terminate_with_error('Input netCDF data does not have East ' +
+                             'Velocity error, which is needed for ' +
+                             'uncertainty quantification.')
+
     if (V_error_all_times is None):
-        raise ValueError('Input netCDF data does not have North ' +
-                         'Velocity error, which is needed for ' +
-                         'uncertainty quantification.')
+        terminate_with_error('Input netCDF data does not have North ' +
+                             'Velocity error, which is needed for ' +
+                             'uncertainty quantification.')
 
     # Make sure arrays are masked arrays
     U_error_one_time = make_array_masked(U_error_all_times[time_index, :, :])
     V_error_one_time = make_array_masked(V_error_all_times[time_index, :, :])
 
     # scale Errors
     scale = scale_error  # in m/s unit
```

### Comparing `restoreio-0.3.2/restoreio/_restore/restore_main_ensemble.py` & `restoreio-0.3.3/restoreio/_restore/restore_main_ensemble.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_scripts/examples.py` & `restoreio-0.3.3/restoreio/_scripts/examples.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_scripts/scan.py` & `restoreio-0.3.3/restoreio/_scripts/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,21 +66,24 @@
         sys.stdout.flush()
         sys.exit(1)
 
     else:
         raise ValueError(message)
 
 
-# ===============
-# Parse Arguments
-# ===============
+# =============
+# Create Parser
+# ============
 
-def _parse_arguments(argv):
+def create_parser():
     """
-    Parses the argument of the executable and obtains the filename.
+    Creates parser object.
+
+    The parser object can be used in both parsing arguments and to generate
+    Sphinx documentation for the command line interface (CLI).
     """
 
     # Instantiate the parser
     description = 'Restore incomplete oceanographic dataset. ' + \
         '"restore" is provided by "restoreio" python package.'
     epilog = examples
     # formatter_class = argparse.RawTextHelpFormatter
@@ -100,57 +103,74 @@
     # Add back help
     optional.add_argument('-h', '--help', action='help',
                           default=argparse.SUPPRESS,
                           help='show this help message and exit')
 
     # Input filename
     help_input = """
-    Input filename. This can be either the path to a local file or the url to
-    a remote dataset. The file extension should be *.nc or *.ncml only.
+    Input filename. This can be either the path to a local file or the URL to
+    a remote dataset. The file or URL may or may not have a file extension.
+    However, if the file does have an extension, the file extension should be
+    either ``.nc``, ``.ncd``, ``.nc.gz``, ``.ncml``, or ``*.ncml.gz`` only.
     """
     required.add_argument('-i', type=str, help=help_input, metavar='INPUT',
                           required=True)
 
-    # Scan velocities
-    help_scan_velocities = """
+    # Scan velocity
+    help_scan_velocity = """
     Scans the velocity arrays of the file. This is useful to find the min and
     max range of the velocity data to adjust the color bar for plotting.
     """
-    optional.add_argument('-V', action='store_true', help=help_scan_velocities)
+    optional.add_argument('-V', action='store_true', help=help_scan_velocity)
 
     # Terminate
     help_terminate = """
-    If `True`, the program exists with code 1. This is useful when this
+    If `True`, the program exists with code `1`. This is useful when this
     package is executed on a server to pass exit signals to a Node application.
     On the downside, this option causes an interactive python environment to
     both terminate the script and the python environment itself. To avoid this,
-    set this option to `False`. In this case, upon an error, the ``ValueError`
+    set this option to `False`. In this case, upon an error, the ``ValueError``
     is raised, which cases the script to terminate, however, an interactive
     python environment will not be exited.
     """
     optional.add_argument('-T', action='store_true', help=help_terminate)
 
     # Version
     help_version = """
     Prints version.
     """
     version = '%(prog)s {version}'.format(version=__version__)
-    parser.add_argument('-V', '--version', action='version', version=version,
+    parser.add_argument('-v', '--version', action='version', version=version,
                         help=help_version)
 
+    return parser
+
+
+# ===============
+# Parse Arguments
+# ===============
+
+def _parse_arguments():
+    """
+    Parses the argument of the executable and obtains the filename.
+    """
+
+    # Create parser object
+    parser = create_parser()
+
     # Parse arguments. Here args is a namespace
     args = parser.parse_args()
 
     # Convert namespace to dictionary
     # args = vars(args)
 
     # Output dictionary
     arguments = {
         'input': args.i,
-        'scan_velocities': args.V,
+        'scan_velocity': args.V,
         'terminate': args.T,
     }
 
     return arguments
 
 
 # ==================
@@ -986,15 +1006,15 @@
 
     input : str
         The input netcdf file URL (if remote file) or file name (if local
         data). The URL should either have no extension, if it does have an
         extension, the file extension should be either of ``.nc``, ``.nc.gz``,
         ``.ncd``, ``.ncml``, or ``.ncml.gz``.
 
-    scan_velocities : bool, default=False
+    scan_velocity : bool, default=False
         Scans the velocity arrays of the file. This is useful to find the min
         and max range of the velocity data to adjust the color bar for
         plotting.
 
     terminate : bool, default=False
         If `True`, the program exists with code 1. This is useful when this
         package is executed on a server to pass exit signals to a Node
@@ -1004,31 +1024,32 @@
         an error, the ``ValueError` is raised, which cases the script to
         terminate, however, an interactive python environment will not be
         exited.
 
     Notes
     -----
 
-    * If the option -V is used to scan min and max of velocities, we do not
-      find the min and max of velocity for all time frames. This is because if
-      the nc file is large, it takes a long time. Also we do not load the whole
-      velocities like U[:] or V[:] because it the data is large, the netCDF4
-      package raises an error.
+    * If the ``scan_velocity`` option (or ``-V`` in command line) is used to
+      scan min and max of velocities, we do not find the min and max of
+      velocity for all time frames. This is because if the `nc` file is large,
+      it takes a long time. Also we do not load the whole velocities like
+      ``U[:]`` or ``V[:]`` because it the data is large, the netCDF4 package
+      raises an error.
 
     Examples
     --------
 
     .. code-block:: python
 
         >>> from restoreio import scan
         >>> input = 'http://transport.me.berkeley.edu/thredds/dodsC/root/' + \
         ...         'WHOI-HFR/WHOI_HFR_2014_original.nc'
 
         >>> # Run script
-        >>> scan(input, scan_velocities=True, terminate=False)
+        >>> scan(input, scan_velocity=True, terminate=False)
         {
             "Scan": {
                 "ScanStatus": true,
                 "Message": ""
             },
             "TimeInfo": {
                 "InitialTime": {
@@ -1160,15 +1181,15 @@
 
     # Converting all warnings to error
     # warnings.simplefilter('error', UserWarning)
     warnings.filterwarnings("ignore", category=numpy.VisibleDeprecationWarning)
     warnings.filterwarnings("ignore", category=DeprecationWarning)
 
     # Parse arguments
-    arguments = _parse_arguments(sys.argv)
+    arguments = _parse_arguments()
 
     # Main function
     scan(**arguments)
 
 
 # ===========
 # Script Main
```

### Comparing `restoreio-0.3.2/restoreio/_subset/subset_datetime.py` & `restoreio-0.3.3/restoreio/_subset/subset_datetime.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,62 +7,58 @@
 # of this source tree.
 
 
 # =======
 # Imports
 # =======
 
-from ._array_utilities import check_monotonicity, find_closest_index, \
-        terminate_with_error
+from ._array_utilities import check_monotonicity, find_closest_index
+from .._server_utils import terminate_with_error
 from datetime import datetime
 import netCDF4
 
 __all__ = ['subset_datetime']
 
 
 # ==================
 # Get Datetime Index
 # ==================
 
 def _get_datetime_index(
         datetime_string,
         datetime_name,
-        datetime_info,
-        terminate):
+        datetime_info):
     """
     Returns time index compared to an array of datetimes.
     """
 
     # datetime string format
     datetime_format = '%Y-%m-%dT%H:%M:%S'
 
     # Time object
     try:
         time_obj = datetime.strptime(datetime_string, datetime_format)
     except ValueError as err:
         print(err)
         terminate_with_error(
-            '%s is not in %s format.' % (datetime_string, datetime_format),
-            terminate)
+            '%s is not in %s format.' % (datetime_string, datetime_format))
 
     # Convert object to number since an epoch given by the unit of the dataset
     # for example in the unit of days since 1970-01-01 00:00:00
     time_value = netCDF4.date2num(time_obj, units=datetime_info['unit'],
                                   calendar=datetime_info['calendar'])
 
     # Check consistency of time value
     if time_value < datetime_info['array'][0]:
         terminate_with_error(
-            'The given time %s is earlier than the dataset time.' % time_value,
-            terminate)
+            'The given time %s is earlier than the dataset time.' % time_value)
 
     elif time_value > datetime_info['array'][-1]:
         terminate_with_error(
-            'The given time %s is after than the dataset time.' % time_value,
-            terminate)
+            'The given time %s is after than the dataset time.' % time_value)
 
     # Find index of time
     datetime_index = find_closest_index(datetime_info['array'],
                                         float(time_value))
 
     return datetime_index
 
@@ -71,16 +67,15 @@
 # Subset Time
 # ===========
 
 def subset_datetime(
         datetime_info,
         min_time,
         max_time,
-        time,
-        terminate):
+        time):
     """
     Find min and max indices to subset the processing time interval.
     """
 
     datetime_array = datetime_info['array']
 
     # Check longitude and latitude arrays are monotonic
@@ -96,42 +91,41 @@
 
         # This is when a single time is specified (such as in uncertainty
         # quantification or plotting where only time time point is used).
 
         # When single time point is specified, a time interval should not also
         # be specified.
         if (min_time != '') or (max_time != ''):
-            raise ValueError(
+            terminate_with_error(
                 'When "time" argument is specified, the other time ' +
                 'arguments "min_time" and "max_time" cannot be specified ' +
                 'and vice versa.')
 
         # Get time index of the given time string
-        time_index = _get_datetime_index(time, 'time point', datetime_info,
-                                         terminate)
+        time_index = _get_datetime_index(time, 'time point', datetime_info)
 
         # Make interval of length zero with the same time for the start and end
         min_datetime_index = time_index
         max_datetime_index = time_index
 
     else:
 
         # Process min time
         if min_time == '':
             min_datetime_index = 0
         else:
             min_datetime_index = _get_datetime_index(min_time, 'initial time',
-                                                     datetime_info, terminate)
+                                                     datetime_info)
 
         # Process max time
         if max_time == '':
             max_datetime_index = datetime_array.size - 1
         else:
             max_datetime_index = _get_datetime_index(max_time, 'final time',
-                                                     datetime_info, terminate)
+                                                     datetime_info)
 
         # Check consistency
         if min_datetime_index > max_datetime_index:
             terminate_with_error(
-                'Initial time should be earlier than final time.', terminate)
+                'Initial time should be earlier than final time.')
 
     return min_datetime_index, max_datetime_index
```

### Comparing `restoreio-0.3.2/restoreio/_subset/subset_domain.py` & `restoreio-0.3.3/restoreio/_subset/subset_domain.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,32 +9,31 @@
 
 # =======
 # Imports
 # =======
 
 import numpy
 import math
-from ._array_utilities import check_monotonicity, find_closest_index, \
-    terminate_with_error
+from ._array_utilities import check_monotonicity, find_closest_index
+from .._server_utils import terminate_with_error
 
 __all__ = ['subset_domain']
 
 
 # =============
 # Subset Domain
 # =============
 
 def subset_domain(
         lon,
         lat,
         min_lon,
         max_lon,
         min_lat,
-        max_lat,
-        terminate):
+        max_lat):
     """
     Find min and max indices to subset the processing domain.
     """
 
     # Check longitude and latitude arrays are monotonic
     check_monotonicity(lon[:], 'Longitudes')
     check_monotonicity(lat[:], 'Latitudes')
@@ -47,99 +46,99 @@
 
     # Check consistency of the bounds
     if (not math.isnan(min_lon)) and (not math.isnan(max_lon)):
         if min_lon >= max_lon:
             terminate_with_error(
                 'The given min longitude (%0.4f) ' % min_lon +
                 'should be smaller than the given max longitude ' +
-                '(%0.4f).' % max_lon, terminate)
+                '(%0.4f).' % max_lon)
 
     if (not math.isnan(min_lat)) and (not math.isnan(max_lat)):
         if min_lat >= max_lat:
             terminate_with_error(
                 'The given min latitude (%0.4f) ' % min_lat +
                 'should be smaller than the given max latitude ' +
-                '(%0.4f).' % max_lat, terminate)
+                '(%0.4f).' % max_lat)
 
     # min lon
     if math.isnan(min_lon):
         min_lon_index = 0
     else:
         # Check bound
         if min_lon < dataset_min_lon:
             terminate_with_error(
                 'The given min longitude %0.4f ' % min_lon + 'is smaller ' +
                 'then the min longitude of the data, which is %f.'
-                % dataset_min_lon, terminate)
+                % dataset_min_lon)
 
         if min_lon > dataset_max_lon:
             terminate_with_error(
                 'The given min longitude %0.4f ' % min_lon + 'is larger ' +
                 'then the max longitude of the data, which is %f.'
-                % dataset_max_lon, terminate)
+                % dataset_max_lon)
 
         # Find min lon index
         min_lon_index = find_closest_index(lon[:], min_lon)
 
     # max lon
     if math.isnan(max_lon):
         max_lon_index = lon.size-1
     else:
         # Check bound
         if max_lon > dataset_max_lon:
             terminate_with_error(
                 'The given max longitude %0.4f ' % max_lon + 'is greater ' +
                 'than the max longitude of the data, which is %f.'
-                % dataset_max_lon, terminate)
+                % dataset_max_lon)
 
         if max_lon < dataset_min_lon:
             terminate_with_error(
                 'The given max longitude %0.4f ' % max_lon + 'is smaller ' +
                 'than the min longitude of the data, which is %f.'
-                % dataset_min_lon, terminate)
+                % dataset_min_lon)
 
         # Find max lon index
         max_lon_index = find_closest_index(lon[:], max_lon)
 
     # min lat
     if math.isnan(min_lat):
         min_lat_index = 0
     else:
         # Check bound
         if min_lat < dataset_min_lat:
             terminate_with_error(
                 'The given min latitude %0.4f ' % min_lat + 'is smaller ' +
                 'than the min latitude of the data, which is %f.'
-                % dataset_min_lat, terminate)
+                % dataset_min_lat)
 
         if min_lat > dataset_max_lat:
             terminate_with_error(
                 'The given min latitude %0.4f ' % min_lat + 'is larger ' +
                 'than the max latitude of the data, which is %f.'
-                % dataset_max_lat, terminate)
+                % dataset_max_lat)
 
         # Find min lat index
         min_lat_index = find_closest_index(lat[:], min_lat)
 
     # max lat
     if math.isnan(max_lat):
         max_lat_index = lat.size-1
     else:
         # Check bound
         if max_lat > dataset_max_lat:
             terminate_with_error(
                 'The given max latitude %0.4f ' % max_lat + 'is greater ' +
                 'than the max latitude of the data, which is %f.'
-                % dataset_max_lat, terminate)
+                % dataset_max_lat)
 
         if max_lat < dataset_min_lat:
             terminate_with_error(
                 'The given max latitude %0.4f ' % max_lat + 'is smaller ' +
                 'than the min latitude of the data, which is %f.'
-                % dataset_min_lat, terminate)
+                % dataset_min_lat)
 
         # Find max lat index
         max_lat_index = find_closest_index(lat[:], max_lat)
 
     # In some dataset, the direction of lon or lat arrays are reversed, meaning
     # they are decreasing monotonic. In such a case, the min or max indices
     # should be swapped.
```

### Comparing `restoreio-0.3.2/restoreio/_uncertainty_quant/_compute_correlation_matrix.py` & `restoreio-0.3.3/restoreio/_uncertainty_quant/_compute_correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py` & `restoreio-0.3.3/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # ======
 
 import numpy
 import scipy.stats
 import pyDOE
 from ._compute_correlation_matrix import compute_correlation_matrix
 from .._plots_uq import plot_cor_cov, plot_valid_vector_ensembles_stat
+from .._server_utils import terminate_with_error
 
 __all__ = ['generate_valid_vector_ensembles']
 
 
 # =========================
 # generate Samples On Plane
 # =========================
@@ -140,17 +141,17 @@
 
     """
 
     # Make sure the number of ensembles is more than variables
     # if num_ensembles < num_modes:
     #     print('Number of variables: %d'%num_modes)
     #     print('Number of Ensembles: %d'%num_ensembles)
-    #     raise ValueError('In Latin Hypercube sampling, it is better to ' +
-    #                      'have more number of ensembles than number of ' +
-    #                      'variables.')
+    #     terminate_with_error(
+    #         'In Latin Hypercube sampling, it is better to have more ' +
+    #         'number of ensembles than number of variables.')
 
     # Mean (center) Latin Hypercube. lhs_uniform is of the
     # size (num_ensembles, num_modes)
     lhs_uniform = pyDOE.lhs(num_modes, samples=num_ensembles,
                             criterion='center')
 
     # Convert uniform distribution to normal distribution
@@ -370,16 +371,17 @@
                       eigenvalues[negative_indices[0][i]])
                 raise RuntimeError('Encountered negative eigenvalue in ' +
                                    'computing KL transform of positive ' +
                                    'definite covariance matrix.')
 
     # Number of modes for KL expansion
     if ratio_num_modes > 1.0 or ratio_num_modes <= 0.0:
-        raise ValueError('The ratio of the number of modes should be larger' +
-                         'than 0 and smaller or equal to 1.')
+        terminate_with_error(
+            'The ratio of the number of modes should be larger than 0 and ' +
+            'smaller or equal to 1.')
 
     # Convert ratio of num modes to num modes
     if ratio_num_modes == 1.0:
         num_modes = valid_vector.size
     else:
         num_modes = int(ratio_num_modes * valid_vector.size)
```

### Comparing `restoreio-0.3.2/restoreio/_uncertainty_quant/_image_utils.py` & `restoreio-0.3.3/restoreio/_uncertainty_quant/_image_utils.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_uncertainty_quant/_statistical_distances.py` & `restoreio-0.3.3/restoreio/_uncertainty_quant/_statistical_distances.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_uncertainty_quant/generate_image_ensembles.py` & `restoreio-0.3.3/restoreio/_uncertainty_quant/generate_image_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio/_uncertainty_quant/get_ensembles_stat.py` & `restoreio-0.3.3/restoreio/_uncertainty_quant/get_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/restoreio.egg-info/PKG-INFO` & `restoreio-0.3.3/restoreio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.3.2
+Version: 0.3.3
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
```

### Comparing `restoreio-0.3.2/restoreio.egg-info/SOURCES.txt` & `restoreio-0.3.3/restoreio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 docs/Makefile
 docs/make.bat
 docs/notes.rst
 docs/requirements.txt
 docs/source/_inspect.py
 docs/source/api.rst
 docs/source/cite.rst
+docs/source/cli_restore.rst
+docs/source/cli_scan.rst
 docs/source/conf.py
 docs/source/contents.rst
 docs/source/custom_domain.py
 docs/source/examples.rst
 docs/source/index.rst
 docs/source/install.rst
 docs/source/recursive_glob.py
@@ -127,14 +129,17 @@
 restoreio/_restore/_make_array_masked.py
 restoreio/_restore/refine_grid.py
 restoreio/_restore/restore_generated_ensembles.py
 restoreio/_restore/restore_main_ensemble.py
 restoreio/_scripts/__init__.py
 restoreio/_scripts/examples.py
 restoreio/_scripts/scan.py
+restoreio/_server_utils/__init__.py
+restoreio/_server_utils/globals.py
+restoreio/_server_utils/terminate_with_error.py
 restoreio/_subset/__init__.py
 restoreio/_subset/_array_utilities.py
 restoreio/_subset/subset_datetime.py
 restoreio/_subset/subset_domain.py
 restoreio/_uncertainty_quant/__init__.py
 restoreio/_uncertainty_quant/_compute_correlation_matrix.py
 restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
```

### Comparing `restoreio-0.3.2/setup.py` & `restoreio-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.2/tests/test_restore_local_data.py` & `restoreio-0.3.3/tests/test_restore_local_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,18 +47,18 @@
     """
     Test for `restore` function.
     """
 
     # Data
     input = 'Monterey_Small_2km_Hourly_2017_01.nc'
     output = 'output_local_data.nc'
-    min_lon = None
-    max_lon = None
-    min_lat = None
-    max_lat = None
+    min_lon = float('nan')
+    max_lon = float('nan')
+    min_lat = float('nan')
+    max_lat = float('nan')
     time = '2017-01-25T03:00:00'
 
     # Absolute path
     dir = os.path.dirname(os.path.realpath(__file__))
     input = os.path.join(dir, input)
     output = os.path.join(dir, output)
 
@@ -67,23 +67,23 @@
         raise RuntimeError('File: %s does not exists.' % input)
 
     # Restore main file
     restore(input, min_file_index='', max_file_index='', output=output,
             min_lon=min_lon, max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
             time=time, sweep=False, detect_land=True, fill_coast=False,
             convex_hull=False, alpha=20, refine_grid=1,
-            uncertainty_quant=False, plot=True, verbose=True)
+            uncertainty_quant=False, plot=True, verbose=True, terminate=False)
 
     # Uncertainty quantification
     restore(input, min_file_index='', max_file_index='', output=output,
             min_lon=min_lon, max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
             time=time, sweep=False, detect_land=True, fill_coast=False,
             convex_hull=False, alpha=20, refine_grid=1, uncertainty_quant=True,
             num_ensembles=200, ratio_num_modes=1, kernel_width=5,
-            scale_error=0.08, plot=True, verbose=True)
+            scale_error=0.08, plot=True, verbose=True, terminate=False)
 
     # Remove outputs
     remove_file('*.svg')
     remove_file('*.pdf')
     remove_file(output)
```

### Comparing `restoreio-0.3.2/tests/test_restore_remote_data.py` & `restoreio-0.3.3/tests/test_restore_remote_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,42 +59,43 @@
     # min_lat = 36.507
     # max_lat = 36.9925
     # time = '2017-01-25T03:00:00'
 
     # Martha's Vineyard
     input = 'http://transport.me.berkeley.edu/thredds/dodsC/root/' + \
             'WHOI-HFR/WHOI_HFR_2014_original.nc'
-    min_lon = None
-    max_lon = None
-    min_lat = None
-    max_lat = None
-    time = '2017-08-17T20:00:00'
+    min_lon = -70.7
+    max_lon = -70.5
+    min_lat = 41.2
+    max_lat = 41.3
+    min_time = '2014-07-01T20:00:00'
+    max_time = '2014-07-03T20:00:00'
 
     # Output
     output = 'output_remote_data.nc'
 
     # Absolute path
     dir = os.path.dirname(os.path.realpath(__file__))
     output = os.path.join(dir, output)
 
     # Restore main file
     restore(input, min_file_index='', max_file_index='', output=output,
             min_lon=min_lon, max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
-            time=time, sweep=False, detect_land=True, fill_coast=False,
-            convex_hull=False, alpha=20, refine_grid=1,
-            uncertainty_quant=False, plot=True, verbose=True)
+            min_time=min_time, max_time=max_time, sweep=False,
+            detect_land=True, fill_coast=False, convex_hull=False, alpha=20,
+            refine_grid=1, uncertainty_quant=False, plot=False, verbose=True)
 
     # These lines are commented since WHOI-HFR data don't have error variables.
     # Uncertainty quantification
-    restore(input, min_file_index='', max_file_index='', output=output,
-            min_lon=min_lon, max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
-            time=time, sweep=False, detect_land=True, fill_coast=False,
-            convex_hull=False, alpha=20, refine_grid=1, uncertainty_quant=True,
-            num_ensembles=200, ratio_num_modes=1, kernel_width=5,
-            scale_error=0.08, plot=True, verbose=True)
+    # restore(input, min_file_index='', max_file_index='', output=output,
+    #         min_lon=min_lon, max_lon=max_lon, min_lat=min_lat,
+    #         max_lat=max_lat, time=time, sweep=False, detect_land=True,
+    #         fill_coast=False, convex_hull=False, alpha=20, refine_grid=1,
+    #         uncertainty_quant=True, num_ensembles=200, ratio_num_modes=1,
+    #         kernel_width=5, scale_error=0.08, plot=True, verbose=True)
 
     # Remove outputs
     remove_file('*.svg')
     remove_file('*.pdf')
     remove_file(output)
```

### Comparing `restoreio-0.3.2/tests/test_scan.py` & `restoreio-0.3.3/tests/test_scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """
 
     # Martha's Vineyard
     input = 'http://transport.me.berkeley.edu/thredds/dodsC/root/' + \
             'WHOI-HFR/WHOI_HFR_2014_original.nc'
 
     # Run script
-    scan(input, scan_velocities=True, terminate=False)
+    scan(input, scan_velocity=True, terminate=False)
 
 
 # ===========
 # Script main
 # ===========
 
 if __name__ == "__main__":
```

### Comparing `restoreio-0.3.2/tox.ini` & `restoreio-0.3.3/tox.ini`

 * *Files identical despite different names*

