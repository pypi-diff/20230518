# Comparing `tmp/pygama-1.3.1.tar.gz` & `tmp/pygama-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygama-1.3.1.tar", last modified: Tue May 16 14:10:23 2023, max compression
+gzip compressed data, was "pygama-1.3.2.tar", last modified: Thu May 18 09:53:32 2023, max compression
```

## Comparing `pygama-1.3.1.tar` & `pygama-1.3.2.tar`

### file list

```diff
@@ -1,255 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 14:10:15.000000 pygama-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-16 14:10:23.377868 pygama-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-16 14:10:15.000000 pygama-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-16 14:10:15.000000 pygama-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-16 14:10:23.377868 pygama-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 14:10:15.000000 pygama-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.349867 pygama-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.353868 pygama-1.3.1/src/pygama/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12151 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.357868 pygama-1.3.1/src/pygama/dsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    71519 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processing_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/dsp/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/bl_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/dplms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/dwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/fftw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/gaussian_filter1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/linear_slope_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/log_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/min_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/moving_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/multi_a_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/multi_t_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/param_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/peak_snr_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/pole_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/presum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/pulse_injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/soft_pileup_corr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/time_over_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/time_point_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/trap_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/wiener_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/processors/windower.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/dsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/evt/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/evt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/evt/build_tcm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/evt/tcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/flow/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60726 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/flow/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    27420 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/flow/file_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/flow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/hit/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/hit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/hit/build_hit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/lgdo/
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/arrayofequalsizedarrays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/lgdo/compression/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/compression/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/compression/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/compression/radware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/compression/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/compression/varlen.py
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/lgdo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/lgdo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68140 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/lh5_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/lgdo/waveform_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.361868 pygama-1.3.1/src/pygama/math/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/math/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/math/peak_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/math/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/math/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.365867 pygama-1.3.1/src/pygama/pargen/
--rw-r--r--   0 runner    (1001) docker     (123)    46542 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/AoE_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/data_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/dsp_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    33112 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/ecal_th.py
--rw-r--r--   0 runner    (1001) docker     (123)    52594 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/energy_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)    72502 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/energy_optimisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/extract_tau.py
--rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/pargen/mse_psd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.365867 pygama-1.3.1/src/pygama/raw/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.365867 pygama-1.3.1/src/pygama/raw/buffer_processor/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/buffer_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/buffer_processor/buffer_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/buffer_processor/lh5_buffer_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/build_raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.365867 pygama-1.3.1/src/pygama/raw/compass/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/compass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/compass/compass_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/compass/compass_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/compass/compass_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/compass/compass_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/data_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/data_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.365867 pygama-1.3.1/src/pygama/raw/fc/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/fc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/fc/fc_config_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/fc/fc_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/fc/fc_status_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/fc/fc_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/src/pygama/raw/orca/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_digitizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    33100 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_flashcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_run_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/orca/orca_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/raw/raw_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/src/pygama/vis/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/vis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/src/pygama/vis/mpl/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/vis/mpl/clint.mpl
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/vis/mpl/root.mpl
--rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-05-16 14:10:15.000000 pygama-1.3.1/src/pygama/vis/waveform_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.357868 pygama-1.3.1/src/pygama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 14:10:23.000000 pygama-1.3.1/src/pygama.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/dsp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/dsp/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/configs/icpc-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/configs/numpy-parsing.json
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/configs/sipm-dplms-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/configs/sipm-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/dsp/processors/
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/processors/dplms_noise_mat.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/processors/test_dplms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/processors/test_dwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/processors/test_fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/processors/test_get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/processors/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/test_build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/test_list_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/test_numpy_constants_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/test_processing_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/dsp/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/flow/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/configs/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/configs/data-loader-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/configs/filedb-config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.369868 pygama-1.3.1/tests/flow/configs/nested/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/configs/nested/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/configs/nested/data-loader-config-nested.json
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/test_filedb.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/flow/test_flow_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/functional/test_l200_dataproc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/functional/test_teststand_dataproc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/hit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/hit/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/hit/configs/basic-hit-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/hit/configs/spms-hit-a-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/hit/configs/spms-hit-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/hit/configs/spms-hit-multi-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/hit/test_build_hit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/integration/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/lgdo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/lgdo/compression/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/lgdo/compression/sigcompress/
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/sigcompress/special-wf-clipped.dat
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)    47033 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/test_radware_sigcompress.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/test_str2wfcodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/compression/test_uleb128_zigzag_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_arrayofequalsizedarrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_lgdo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_lh5_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_lh5_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_table_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/lgdo/test_waveform_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/math/test_fwhm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/pargen/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/pargen/test_ecal.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/pargen/test_energy_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.373868 pygama-1.3.1/tests/raw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/raw/buffer_processor/
--rw-r--r--   0 runner    (1001) docker     (123)    56908 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor_configs/raw_out_spec_no_proc.json
--rw-r--r--   0 runner    (1001) docker     (123)    42875 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/buffer_processor/test_lh5_buffer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/raw/compass/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/compass/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/compass/test_compass_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/compass/test_compass_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/compass/test_compass_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/raw/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/configs/fc-out-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/configs/orca-out-spec-cli.json
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/configs/orca-out-spec.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/raw/fc/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/fc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/fc/test_fc_config_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/fc/test_fc_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/fc/test_fc_status_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/fc/test_fc_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/raw/orca/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/orca/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/orca/test_or_run_decoder_for_run.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/orca/test_orca_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/test_build_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/test_daq_to_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/raw/test_raw_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/vis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:10:23.377868 pygama-1.3.1/tests/vis/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/vis/configs/hpge-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-16 14:10:15.000000 pygama-1.3.1/tests/vis/test_waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.025236 pygama-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 09:53:24.000000 pygama-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-18 09:53:32.025236 pygama-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-18 09:53:24.000000 pygama-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-18 09:53:24.000000 pygama-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-18 09:53:32.025236 pygama-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-18 09:53:24.000000 pygama-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.001236 pygama-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.005236 pygama-1.3.2/src/pygama/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 09:53:31.000000 pygama-1.3.2/src/pygama/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12151 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.005236 pygama-1.3.2/src/pygama/dsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72552 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processing_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.009236 pygama-1.3.2/src/pygama/dsp/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/bl_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/dplms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/dwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/fftw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/gaussian_filter1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/linear_slope_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/log_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/moving_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/multi_a_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/multi_t_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/param_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/peak_snr_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/pole_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/presum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/pulse_injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/soft_pileup_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/time_over_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/time_point_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/trap_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/wiener_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/processors/windower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/dsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.009236 pygama-1.3.2/src/pygama/evt/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/evt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/evt/build_tcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/evt/tcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.009236 pygama-1.3.2/src/pygama/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62151 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/flow/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27420 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/flow/file_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/flow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.009236 pygama-1.3.2/src/pygama/hit/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/hit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/hit/build_hit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.013236 pygama-1.3.2/src/pygama/lgdo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/arrayofequalsizedarrays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.013236 pygama-1.3.2/src/pygama/lgdo/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/compression/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/compression/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/compression/radware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/compression/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/compression/varlen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/lgdo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/lgdo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68426 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/lgdo/waveform_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.013236 pygama-1.3.2/src/pygama/math/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/math/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/math/peak_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/math/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/math/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.013236 pygama-1.3.2/src/pygama/pargen/
+-rw-r--r--   0 runner    (1001) docker     (123)    46542 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/pargen/AoE_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/pargen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/pargen/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/pargen/data_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/pargen/dsp_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33112 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/pargen/ecal_th.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52594 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/pargen/energy_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72502 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/pargen/energy_optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/pargen/extract_tau.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/pargen/mse_psd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.013236 pygama-1.3.2/src/pygama/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.013236 pygama-1.3.2/src/pygama/raw/buffer_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/buffer_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/buffer_processor/buffer_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/buffer_processor/lh5_buffer_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/build_raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.017236 pygama-1.3.2/src/pygama/raw/compass/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/compass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/compass/compass_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/compass/compass_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/compass/compass_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/compass/compass_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/data_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/data_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.017236 pygama-1.3.2/src/pygama/raw/fc/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/fc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/fc/fc_config_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/fc/fc_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/fc/fc_status_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/fc/fc_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.017236 pygama-1.3.2/src/pygama/raw/orca/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/orca/orca_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/orca/orca_digitizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33100 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/orca/orca_flashcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/orca/orca_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/orca/orca_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/orca/orca_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/orca/orca_run_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/orca/orca_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/raw/raw_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.017236 pygama-1.3.2/src/pygama/vis/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/vis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.017236 pygama-1.3.2/src/pygama/vis/mpl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/vis/mpl/clint.mpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/vis/mpl/root.mpl
+-rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-05-18 09:53:24.000000 pygama-1.3.2/src/pygama/vis/waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.005236 pygama-1.3.2/src/pygama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-18 09:53:31.000000 pygama-1.3.2/src/pygama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-18 09:53:31.000000 pygama-1.3.2/src/pygama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:53:31.000000 pygama-1.3.2/src/pygama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 09:53:31.000000 pygama-1.3.2/src/pygama.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:53:31.000000 pygama-1.3.2/src/pygama.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-18 09:53:31.000000 pygama-1.3.2/src/pygama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 09:53:31.000000 pygama-1.3.2/src/pygama.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.017236 pygama-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.017236 pygama-1.3.2/tests/dsp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.017236 pygama-1.3.2/tests/dsp/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/configs/icpc-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/configs/numpy-parsing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/configs/sipm-dplms-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/configs/sipm-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.017236 pygama-1.3.2/tests/dsp/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/processors/dplms_noise_mat.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/processors/test_dplms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/processors/test_dwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/processors/test_fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/processors/test_get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/processors/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/test_build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/test_list_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/test_numpy_constants_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/test_processing_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/dsp/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.021236 pygama-1.3.2/tests/flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.021236 pygama-1.3.2/tests/flow/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/flow/configs/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/flow/configs/data-loader-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/flow/configs/filedb-config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.021236 pygama-1.3.2/tests/flow/configs/nested/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/flow/configs/nested/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/flow/configs/nested/data-loader-config-nested.json
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/flow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/flow/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/flow/test_filedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/flow/test_flow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.021236 pygama-1.3.2/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/functional/test_l200_dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/functional/test_teststand_dataproc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.021236 pygama-1.3.2/tests/hit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.021236 pygama-1.3.2/tests/hit/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/hit/configs/basic-hit-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/hit/configs/spms-hit-a-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/hit/configs/spms-hit-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/hit/configs/spms-hit-multi-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/hit/test_build_hit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.021236 pygama-1.3.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/integration/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.021236 pygama-1.3.2/tests/lgdo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.021236 pygama-1.3.2/tests/lgdo/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/compression/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.021236 pygama-1.3.2/tests/lgdo/compression/sigcompress/
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/compression/sigcompress/special-wf-clipped.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/compression/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47033 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/compression/test_radware_sigcompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/compression/test_str2wfcodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/compression/test_uleb128_zigzag_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_arrayofequalsizedarrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_lgdo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_lh5_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_table_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/lgdo/test_waveform_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.021236 pygama-1.3.2/tests/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/math/test_fwhm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.021236 pygama-1.3.2/tests/pargen/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/pargen/test_ecal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/pargen/test_energy_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.025236 pygama-1.3.2/tests/raw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.025236 pygama-1.3.2/tests/raw/buffer_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)    56908 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/buffer_processor/test_buffer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.025236 pygama-1.3.2/tests/raw/buffer_processor/test_buffer_processor_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/buffer_processor/test_buffer_processor_configs/raw_out_spec_no_proc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42875 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/buffer_processor/test_lh5_buffer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.025236 pygama-1.3.2/tests/raw/compass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/compass/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/compass/test_compass_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/compass/test_compass_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/compass/test_compass_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.025236 pygama-1.3.2/tests/raw/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/configs/fc-out-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/configs/orca-out-spec-cli.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/configs/orca-out-spec.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.025236 pygama-1.3.2/tests/raw/fc/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/fc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/fc/test_fc_config_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/fc/test_fc_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/fc/test_fc_status_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/fc/test_fc_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.025236 pygama-1.3.2/tests/raw/orca/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/orca/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/orca/test_or_run_decoder_for_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/orca/test_orca_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/test_build_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/test_daq_to_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/raw/test_raw_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.025236 pygama-1.3.2/tests/vis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:53:32.025236 pygama-1.3.2/tests/vis/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/vis/configs/hpge-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-18 09:53:24.000000 pygama-1.3.2/tests/vis/test_waveform_browser.py
```

### Comparing `pygama-1.3.1/LICENSE` & `pygama-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/PKG-INFO` & `pygama-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygama
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python package for decoding and processing digitizer data
 Home-page: https://github.com/legend-exp/pygama
 Author: The LEGEND collaboration
 Maintainer: The LEGEND collaboration
 License: GPL-3.0
 Project-URL: Documentation, https://pygama.readthedocs.io
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pygama-1.3.1/README.md` & `pygama-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/setup.cfg` & `pygama-1.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 	parse
 	pint
 	pyfcutils
 	pyfftw
 	scikit-learn
 	scipy>=1.0.1
 	tables
-	tqdm
+	tqdm>=4.27
 	xmltodict
 python_requires = >=3.9
 include_package_data = True
 package_dir = 
 	= src
 zip_safe = False
```

### Comparing `pygama-1.3.1/src/pygama/cli.py` & `pygama-1.3.2/src/pygama/cli.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/__init__.py` & `pygama-1.3.2/src/pygama/dsp/__init__.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/build_dsp.py` & `pygama-1.3.2/src/pygama/dsp/build_dsp.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 import os
 import sys
 import time
 
 import h5py
 import numpy as np
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 import pygama
 import pygama.lgdo as lgdo
 import pygama.lgdo.lh5_store as lh5
 from pygama.dsp.errors import DSPFatal
 from pygama.dsp.processing_chain import build_processing_chain
 from pygama.lgdo.lgdo_utils import expand_path
```

### Comparing `pygama-1.3.1/src/pygama/dsp/errors.py` & `pygama-1.3.2/src/pygama/dsp/errors.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processing_chain.py` & `pygama-1.3.2/src/pygama/dsp/processing_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -942,16 +942,46 @@
         if not isinstance(var, ProcChainVar):
             return round(float(var))
         else:
             raise ProcessingChainError(
                 "round() is not implemented for variables, only constants."
             )
 
+    # type cast variable
+    def _astype(var: ProcChainVar, dtype: str) -> ProcChainVar:  # noqa: N805
+        dtype = np.dtype(dtype)
+        if var is None:
+            return None
+        if not isinstance(var, ProcChainVar):
+            raise ProcessingChainError(f"cannot call astype() on {var}")
+        else:
+            name = f"{var.name}.astype(`{dtype.char}`)"
+            out = ProcChainVar(
+                var.proc_chain,
+                name,
+                var.shape,
+                dtype,
+                var.grid,
+                var.unit,
+                var.is_coord,
+            )
+            var.proc_chain._proc_managers.append(
+                ProcessorManager(
+                    var.proc_chain,
+                    np.copyto,
+                    [out, var],
+                    kw_params={"casting": "'unsafe'"},
+                    signature="(),(),()",
+                    types=f"{dtype.char}{var.dtype.char}",
+                )
+            )
+            return out
+
     # dict of functions that can be parsed by get_variable
-    func_list = {"len": _length, "round": _round}
+    func_list = {"len": _length, "round": _round, "astype": _astype}
     module_list = {"np": np, "numpy": np}
 
 
 class ProcessorManager:
     """The class that calls processors and makes sure variables are compatible."""
 
     @dataclass
@@ -1014,15 +1044,15 @@
         # of the correct dimensions and unit system
         dims_list = re.findall(r"\((.*?)\)", self.signature)
 
         if not len(dims_list) == len(params) + len(kw_params):
             raise ProcessingChainError(
                 f"expected {len(dims_list)} arguments from signature "
                 f"{self.signature}; found "
-                f"{len(params)}: ({', '.join([str(par) for par in params])})"
+                f"{len(params)+len(kw_params)}: ({', '.join([str(par) for par in params])})"
             )
 
         dims_dict = {}  # map from dim name -> DimInfo
         outerdims = []  # list of DimInfo
         grid = None  # period/offset to use for unit and coordinate conversions
 
         for ipar, (dims, param) in enumerate(
```

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/__init__.py` & `pygama-1.3.2/src/pygama/dsp/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/bl_subtract.py` & `pygama-1.3.2/src/pygama/dsp/processors/bl_subtract.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/convolutions.py` & `pygama-1.3.2/src/pygama/dsp/processors/convolutions.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/dplms.py` & `pygama-1.3.2/src/pygama/dsp/processors/dplms.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/dwt.py` & `pygama-1.3.2/src/pygama/dsp/processors/dwt.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/fftw.py` & `pygama-1.3.2/src/pygama/dsp/processors/fftw.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/fixed_time_pickoff.py` & `pygama-1.3.2/src/pygama/dsp/processors/fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/gaussian_filter1d.py` & `pygama-1.3.2/src/pygama/dsp/processors/gaussian_filter1d.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/get_multi_local_extrema.py` & `pygama-1.3.2/src/pygama/dsp/processors/get_multi_local_extrema.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/histogram.py` & `pygama-1.3.2/src/pygama/dsp/processors/histogram.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/linear_slope_fit.py` & `pygama-1.3.2/src/pygama/dsp/processors/linear_slope_fit.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/log_check.py` & `pygama-1.3.2/src/pygama/dsp/processors/log_check.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/min_max.py` & `pygama-1.3.2/src/pygama/dsp/processors/min_max.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/moving_windows.py` & `pygama-1.3.2/src/pygama/dsp/processors/moving_windows.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/multi_a_filter.py` & `pygama-1.3.2/src/pygama/dsp/processors/multi_a_filter.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/multi_t_filter.py` & `pygama-1.3.2/src/pygama/dsp/processors/multi_t_filter.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/optimize.py` & `pygama-1.3.2/src/pygama/dsp/processors/optimize.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/param_lookup.py` & `pygama-1.3.2/src/pygama/dsp/processors/param_lookup.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/peak_snr_threshold.py` & `pygama-1.3.2/src/pygama/dsp/processors/peak_snr_threshold.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/pole_zero.py` & `pygama-1.3.2/src/pygama/dsp/processors/pole_zero.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/presum.py` & `pygama-1.3.2/src/pygama/dsp/processors/presum.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/pulse_injector.py` & `pygama-1.3.2/src/pygama/dsp/processors/pulse_injector.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/saturation.py` & `pygama-1.3.2/src/pygama/dsp/processors/saturation.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/soft_pileup_corr.py` & `pygama-1.3.2/src/pygama/dsp/processors/soft_pileup_corr.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/time_over_threshold.py` & `pygama-1.3.2/src/pygama/dsp/processors/time_over_threshold.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/time_point_thresh.py` & `pygama-1.3.2/src/pygama/dsp/processors/time_point_thresh.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/trap_filters.py` & `pygama-1.3.2/src/pygama/dsp/processors/trap_filters.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/upsampler.py` & `pygama-1.3.2/src/pygama/dsp/processors/upsampler.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/wiener_filter.py` & `pygama-1.3.2/src/pygama/dsp/processors/wiener_filter.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/processors/windower.py` & `pygama-1.3.2/src/pygama/dsp/processors/windower.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/dsp/utils.py` & `pygama-1.3.2/src/pygama/dsp/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/evt/build_tcm.py` & `pygama-1.3.2/src/pygama/evt/build_tcm.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/evt/tcm.py` & `pygama-1.3.2/src/pygama/evt/tcm.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/flow/data_loader.py` & `pygama-1.3.2/src/pygama/flow/data_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import string
 from itertools import product
 from keyword import iskeyword
 from typing import Iterator
 
 import numpy as np
 import pandas as pd
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from pygama.lgdo import Array, LH5Iterator, LH5Store, Struct, Table, lgdo_utils
 from pygama.lgdo.vectorofvectors import build_cl, explode_arrays, explode_cl
 from pygama.vis import WaveformBrowser
 
 from . import utils
 from .file_db import FileDB
@@ -227,27 +227,30 @@
                 if "tcm_cols" not in config["levels"][level].keys():
                     log.warning(
                         f"TCM levels, e.g. {level}, need to specify the TCM lookup columns"
                     )
             else:
                 self.cut_priority[level] = 0
 
-    def set_files(self, query: str | list[str]) -> None:
+    def set_files(self, query: str | list[str], append: bool = False) -> None:
         """Apply a file selection.
 
         Sets `self.file_list`, which is a list of indices corresponding to the
         rows in the file database.
 
         Parameters
         ----------
         query
             if single string, defines an operation on the file database columns
             supported by :meth:`pandas.DataFrame.query`. In addition, the
             ``all`` keyword is supported to select all files in the database.
             If list of strings, will be interpreted as key (cycle timestamp) list.
+        append
+            if ``True``, appends files to the existing `self.file_list`
+            instead of overwriting.
 
         Note
         ----
         Call this function before any other operation. A second call to
         :meth:`set_files` does not replace the current file list, which gets
         instead integrated with the new list. Use :meth:`reset` to reset the
         file query.
@@ -269,46 +272,52 @@
                 )
         else:
             raise ValueError("bad query format")
 
         if not inds:
             log.warning("no files matching selection found")
 
-        if self.file_list is None:
-            self.file_list = inds
-        else:
+        if append and self.file_list is not None:
             self.file_list += inds
+            self.file_list = sorted(list(set(self.file_list)))
+        else:
+            self.file_list = inds
 
     def get_file_list(self) -> pd.DataFrame:
         """
         Returns a copy of the file database with its dataframe pared down to
         the current file list.
         """
         return self.filedb.df.iloc[self.file_list]
 
-    def set_datastreams(self, ds: list | tuple | np.ndarray, word: str) -> None:
+    def set_datastreams(
+        self, ds: list | tuple | np.ndarray, word: str, append: bool = False
+    ) -> None:
         """Apply selection on data streams (or channels).
 
         Sets `self.table_list`.
 
         Parameters
         ----------
         ds
             identifies the detectors of interest. Can be a list of detector
             names, serial numbers, or channels or a list of subsystems of
             interest e.g.  ``ged``.
         word
             the type of identifier used in ds. Should be a key in the given
             channel map or a word defined in the configuration file.
+        append
+            if ``True``, appends datastreams to the existing `self.table_list`
+            instead of overwriting.
 
         Example
         -------
         >>> dl.set_datastreams(np.arange(40, 45), "ch")
         """
-        if self.table_list is None:
+        if self.table_list is None or not append:
             self.table_list = {}
 
         ds = list(ds)
 
         found = False
         for level in self.levels:
             tier = self.tiers[level][0]
@@ -320,47 +329,50 @@
             if len(names) > 0:
                 keyword = names[0]
 
             if word == keyword:
                 found = True
                 if level in self.table_list.keys():
                     self.table_list[level] += ds
+                    self.table_list[level] = sorted(list(set(self.table_list[level])))
                 else:
                     self.table_list[level] = ds
 
         if not found:
             # look for word in channel map
             raise NotImplementedError
 
-    def set_cuts(self, cuts: dict | list) -> None:
+    def set_cuts(self, cuts: dict | list, append: bool = False) -> None:
         """Apply a selection on columns in the data tables.
 
         Parameters
         ----------
         cut
             the cuts on the columns of the data table, e.g. ``trapEftp_cal >
             1000``.  If passing a dictionary, the dictionary should be
             structured as ``dict[tier] = cut_expr``. If passing a list, each
             item in the array should be able to be applied on one level of
             tables. The cuts at different levels will be joined with an AND.
+        append
+            if True, appends cuts to the existing cuts instead of overwriting
 
         Example
         -------
         >>> dl.set_cuts({"raw": "daqenergy > 1000", "hit": "AoE > 3"})
         """
-        if self.cuts is None:
+        if self.cuts is None or not append:
             self.cuts = {}
         if isinstance(cuts, dict):
             # verify the correct structure
             for key, value in cuts.items():
                 if not (key in self.levels and isinstance(value, str)):
                     raise ValueError(
                         r"cuts dictionary must be in the format \{ level: string \}"
                     )
-                if key in self.cuts.keys():
+                if key in self.cuts.keys() and append:
                     self.cuts[key] += " and " + value
                 else:
                     self.cuts[key] = value
         elif isinstance(cuts, list):
             raise NotImplementedError
             self.cuts = {}
             # TODO Parse strings to match column names so you don't have to specify which level it is
@@ -417,15 +429,14 @@
         self.cuts = None
         self.merge_files = True
         self.output_format = "lgdo.Table"
         self.output_columns = None
         self.aoesa_to_vov = False
         self.data = None
 
-    # TODO: mode
     def build_entry_list(
         self,
         tcm_level: str = None,
         tcm_table: int | str = None,
         mode: str = "only",
         save_output_columns: bool = False,
         in_memory: bool = True,
@@ -519,16 +530,30 @@
                             for_output.append(term)
 
         if save_output_columns:
             entry_cols += for_output
 
         sto = LH5Store()
 
+        if log.getEffectiveLevel() >= logging.INFO:
+            progress_bar = tqdm(
+                desc="Building entry list",
+                total=len(self.file_list),
+                delay=2,
+                unit="keys",
+            )
+
         # Make the entry list for each file
         for file in self.file_list:
+            if log.getEffectiveLevel() >= logging.INFO:
+                progress_bar.update()
+                progress_bar.set_postfix(
+                    key=self.filedb.df.iloc[file][self.filedb.sortby]
+                )
+
             # Get the TCM specified
             # Assumes that each TCM level only has one tier
             tcm_tier = self.tiers[tcm_level][0]
             tcm_tables = self.filedb.df.loc[file, f"{tcm_tier}_tables"]
             if len(tcm_tables) > 1 and tcm_table is None:
                 raise ValueError(
                     f"There are {len(tcm_tables)} TCM tables, need to specify which to use"
@@ -673,14 +698,17 @@
                 if self.merge_files:
                     sto.write_object(f_struct, "entries", output_file, wo_mode="a")
                 else:
                     sto.write_object(
                         f_struct, f"entries/{file}", output_file, wo_mode="a"
                     )
 
+        if log.getEffectiveLevel() >= logging.INFO:
+            progress_bar.close()
+
         if in_memory:
             if self.merge_files:
                 entries = pd.concat(entries.values(), ignore_index=True)
             return entries
 
     def build_hit_entries(
         self,
@@ -745,15 +773,15 @@
         sto = LH5Store()
 
         if log.getEffectiveLevel() >= logging.INFO:
             progress_bar = tqdm(
                 desc="Building entry list",
                 total=len(self.file_list),
                 delay=2,
-                unit=" keys",
+                unit="keys",
             )
 
         # now we loop over the files in our list
         for file in self.file_list:
             if log.getEffectiveLevel() >= logging.INFO:
                 progress_bar.update()
                 progress_bar.set_postfix(
@@ -834,14 +862,15 @@
                             if tb_table is None:
                                 tb_table = tier_tb
                             else:
                                 tb_table.join(tier_tb)
 
                     if tb_table is None:
                         continue
+
                     # convert to DataFrame and apply cuts
                     tb_df = tb_table.get_dataframe()
                     tb_df.query(cut, inplace=True)
                     tb_df[f"{low_level}_table"] = tb
                     tb_df[f"{low_level}_idx"] = tb_df.index
 
                 # final DataFrame
@@ -857,15 +886,14 @@
                 f_struct = Struct(f_dict)
                 if self.merge_files:
                     sto.write_object(f_struct, "entries", output_file, wo_mode="a")
                 else:
                     sto.write_object(
                         f_struct, f"entries/{file}", output_file, wo_mode="a"
                     )
-            # end file loop
 
         if log.getEffectiveLevel() >= logging.INFO:
             progress_bar.close()
 
         if in_memory:
             if self.merge_files:
                 entries = pd.concat(entries.values(), ignore_index=True)
@@ -1032,23 +1060,40 @@
             col_tiers = self.get_tiers_for_col(field_mask)
             col_dict = entry_list.to_dict("list")
             attr_dict = {}
             for key in col_dict:
                 attr_dict[key] = None
             table_length = len(entry_list)
 
+            tot_iter = 0
+            for _, level in product(tables, load_levels):
+                for _ in self.tiers[level]:
+                    tot_iter += 1
+
+            if log.getEffectiveLevel() >= logging.INFO:
+                progress_bar = tqdm(
+                    desc="Loading data",
+                    total=tot_iter,
+                    delay=2,
+                )
+
             for tb, level in product(tables, load_levels):
                 gb = entry_list.query(f"{parent}_table == {tb}").groupby("file")
                 files = list(gb.groups.keys())
                 el_idx = list(gb.groups.values())
                 idx_mask = [list(entry_list.loc[i, f"{level}_idx"]) for i in el_idx]
 
                 for tier in self.tiers[level]:
+                    if log.getEffectiveLevel() >= logging.INFO:
+                        progress_bar.update()
+                        progress_bar.set_postfix(table=tb, tier=tier)
+
                     if tb not in col_tiers[tier]:
                         continue
+
                     tb_name = self.filedb.get_table_name(tier, tb)
                     tier_paths = [
                         os.path.join(
                             self.data_dir,
                             self.filedb.tier_dirs[tier].lstrip("/"),
                             self.filedb.df.iloc[file][f"{tier}_file"].lstrip("/"),
                         )
@@ -1070,14 +1115,17 @@
                         col_dict,
                         attr_dict,
                         [idx for idx_list in el_idx for idx in idx_list],
                         table_length,
                         self.aoesa_to_vov,
                     )
 
+            if log.getEffectiveLevel() >= logging.INFO:
+                progress_bar.close()
+
             # Convert col_dict to lgdo.Table
             f_table = utils.dict_to_table(col_dict=col_dict, attr_dict=attr_dict)
 
             if output_file:
                 sto.write_object(f_table, "merged_data", output_file, wo_mode="o")
             if in_memory:
                 if self.output_format == "lgdo.Table":
@@ -1086,22 +1134,22 @@
                     return f_table.get_dataframe()
                 else:
                     raise ValueError(
                         f"'{self.output_format}' output format not supported"
                     )
         else:  # not merge_files
             if in_memory:
-                load_out = {}
+                load_out = Struct(attrs={"int_keys": True})
 
             if log.getEffectiveLevel() >= logging.INFO:
                 progress_bar = tqdm(
                     desc="Loading data",
                     total=len(entry_list),
                     delay=2,
-                    unit=" keys",
+                    unit="keys",
                 )
 
             # now loop over the output of build_entry_list()
             for file, f_entries in entry_list.items():
                 if log.getEffectiveLevel() >= logging.INFO:
                     progress_bar.update()
                     progress_bar.set_postfix(
@@ -1175,21 +1223,23 @@
                         )
                         # end tb loop
 
                 # Convert col_dict to lgdo.Table
                 f_table = utils.dict_to_table(col_dict, attr_dict)
 
                 if in_memory:
-                    load_out[file] = f_table
+                    load_out.add_field(name=file, obj=f_table)
                 if output_file:
                     sto.write_object(f_table, f"{file}", output_file, wo_mode="o")
                 # end file loop
 
             if log.getEffectiveLevel() >= logging.INFO:
                 progress_bar.close()
+            if load_out:
+                load_out.update_datatype()
 
             if in_memory:
                 if self.output_format == "lgdo.Table":
                     return load_out
                 elif self.output_format == "pd.DataFrame":
                     for file in load_out.keys():
                         load_out[file] = load_out[file].get_dataframe()
@@ -1215,15 +1265,15 @@
 
         sto = LH5Store()
 
         if self.merge_files:  # Try to load all information at once
             raise NotImplementedError
         else:  # Not merge_files
             if in_memory:
-                load_out = {}
+                load_out = Struct(attrs={"int_keys": True})
             for file, f_entries in entry_list.items():
                 field_mask = []
                 f_table = None
                 # Pre-allocate memory for output columns
                 for col in self.output_columns:
                     if col not in f_entries.columns:
                         f_entries[col] = None
@@ -1351,23 +1401,24 @@
                         tb_names += [self.filedb.get_table_name(tier, tb)] * len(gb)
                         idx_list += [
                             list(entry_list.loc[i, f"{level}_idx"])
                             for i in gb.groups.values()
                         ]
 
                     # Create iterator for this tier and friend to other tiers
-                    lh5_it = LH5Iterator(
-                        lh5_files=lh5_files,
-                        groups=tb_names,
-                        base_path=self.data_dir,
-                        entry_list=idx_list,
-                        field_mask=field_mask,
-                        buffer_len=buffer_len,
-                        friend=lh5_it,
-                    )
+                    if len(lh5_files) > 0:
+                        lh5_it = LH5Iterator(
+                            lh5_files=lh5_files,
+                            groups=tb_names,
+                            base_path=self.data_dir,
+                            entry_list=idx_list,
+                            field_mask=field_mask,
+                            buffer_len=buffer_len,
+                            friend=lh5_it,
+                        )
 
             return lh5_it
         else:  # not merge_files
             raise NotImplementedError
 
     def load_detector(self, det_id):
         """
@@ -1402,34 +1453,31 @@
         handle this one separately because waveforms can easily fill up memory.
         """
         raise NotImplementedError
 
     # TODO: automatically get the dsp_config/par_database used for
     #   processing when these are set to None
     def browse(
-        self,
-        entry_list: pd.DataFrame = None,
-        dsp_config=None,
-        par_database: str | dict = None,
-        aux_values: pd.DataFrame = None,
-        lines: str | list[str] = "waveform",
-        styles: dict[str, list] | str = None,
-        legend: str | list[str] = None,
-        legend_opts: dict = None,
-        n_drawn: int = 1,
-        x_unit: pint.Unit | str = None,  # noqa: F821
-        x_lim: tuple[float | str | pint.Quantity] = None,  # noqa: F821
-        y_lim: tuple[float | str | pint.Quantity] = None,  # noqa: F821
-        norm: str = None,
-        align: str = None,
-        buffer_len: int = 128,
-        block_width: int = 8,
-    ):
-        """
-        Interface between :class:DataLoader and :class:WaveformBrowser.
+        self, entry_list: pd.DataFrame = None, buffer_len: int = 128, **kwargs
+    ) -> WaveformBrowser:
+        """Return a :class:`.WaveformBrowser` object for waveform inspection.
+
+        Parameters
+        ----------
+        entry_list
+            the output of :meth:`.build_entry_list`. If ``None``, builds it
+            according to the current configuration.
+        buffer_len
+            number of waveforms to keep in memory at a time.
+        **kwargs
+            keyword arguments forwarded to :class:`.WaveformBrowser`.
+
+        See Also
+        --------
+        .WaveformBrowser
         """
         if entry_list is None:
             entry_list = self.build_entry_list()
 
         parent = self.levels[0]
         tables = entry_list[f"{parent}_table"].unique()
 
@@ -1460,32 +1508,15 @@
                 base_path=self.data_dir,
                 entry_list=idx_list,
                 buffer_len=buffer_len,
                 field_mask={"tracelist": False},
                 friend=lh5_it,
             )
 
-        return WaveformBrowser(
-            lh5_it,
-            dsp_config=dsp_config,
-            database=par_database,
-            aux_values=aux_values,
-            lines=lines,
-            styles=styles,
-            legend=legend,
-            legend_opts=legend_opts,
-            n_drawn=n_drawn,
-            x_unit=x_unit,
-            x_lim=x_lim,
-            y_lim=y_lim,
-            norm=norm,
-            align=align,
-            buffer_len=buffer_len,
-            block_width=block_width,
-        )
+        return WaveformBrowser(lh5_it, buffer_len=buffer_len, **kwargs)
 
     def get_tiers_for_col(
         self, columns: list | np.ndarray, merge_files: bool = None
     ) -> dict:
         """For each column given, get the tiers and tables in that tier where
         that column can be found.
```

### Comparing `pygama-1.3.1/src/pygama/flow/file_db.py` & `pygama-1.3.2/src/pygama/flow/file_db.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/flow/utils.py` & `pygama-1.3.2/src/pygama/flow/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/hit/build_hit.py` & `pygama-1.3.2/src/pygama/hit/build_hit.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/__init__.py` & `pygama-1.3.2/src/pygama/lgdo/__init__.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/array.py` & `pygama-1.3.2/src/pygama/lgdo/array.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/arrayofequalsizedarrays.py` & `pygama-1.3.2/src/pygama/lgdo/arrayofequalsizedarrays.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/compression/__init__.py` & `pygama-1.3.2/src/pygama/lgdo/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/compression/base.py` & `pygama-1.3.2/src/pygama/lgdo/compression/base.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/compression/generic.py` & `pygama-1.3.2/src/pygama/lgdo/compression/generic.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/compression/radware.py` & `pygama-1.3.2/src/pygama/lgdo/compression/radware.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/compression/utils.py` & `pygama-1.3.2/src/pygama/lgdo/compression/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/compression/varlen.py` & `pygama-1.3.2/src/pygama/lgdo/compression/varlen.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/encoded.py` & `pygama-1.3.2/src/pygama/lgdo/encoded.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/fixedsizearray.py` & `pygama-1.3.2/src/pygama/lgdo/fixedsizearray.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/lgdo.py` & `pygama-1.3.2/src/pygama/lgdo/lgdo.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/lgdo_utils.py` & `pygama-1.3.2/src/pygama/lgdo/lgdo_utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/lh5_store.py` & `pygama-1.3.2/src/pygama/lgdo/lh5_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,20 @@
             for field in elements:
                 if not field_mask[field]:
                     continue
                 # TODO: it's strange to pass start_row, n_rows, idx to struct
                 # fields. If they all had shared indexing, they should be in a
                 # table... Maybe should emit a warning? Or allow them to be
                 # dicts keyed by field name?
-                obj_dict[field], _ = self.read_object(
+                if "int_keys" in h5f[name].attrs:
+                    if dict(h5f[name].attrs)["int_keys"]:
+                        f = int(field)
+                else:
+                    f = str(field)
+                obj_dict[f], _ = self.read_object(
                     name + "/" + field,
                     h5f,
                     start_row=start_row,
                     n_rows=n_rows,
                     idx=idx,
                     decompress=decompress,
                 )
@@ -925,17 +930,19 @@
                     and isinstance(obj.values.attrs["compression"], WaveformCodec)
                 ):
                     codec = obj.values.attrs["compression"]
                     obj_fld = compress.encode(obj.values, codec=codec)
                 else:
                     obj_fld = obj[field]
 
+                # Convert keys to string for dataset names
+                f = str(field)
                 self.write_object(
                     obj_fld,
-                    field,
+                    f,
                     lh5_file,
                     group=group,
                     start_row=start_row,
                     n_rows=n_rows,
                     wo_mode=wo_mode,
                     write_start=write_start,
                     hdf5_compression=hdf5_compression,
```

### Comparing `pygama-1.3.1/src/pygama/lgdo/scalar.py` & `pygama-1.3.2/src/pygama/lgdo/scalar.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/struct.py` & `pygama-1.3.2/src/pygama/lgdo/struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,25 +40,27 @@
 
         super().__init__(attrs)
 
     def datatype_name(self) -> str:
         return "struct"
 
     def form_datatype(self) -> str:
-        return self.datatype_name() + "{" + ",".join(self.keys()) + "}"
+        return (
+            self.datatype_name() + "{" + ",".join([str(k) for k in self.keys()]) + "}"
+        )
 
     def update_datatype(self) -> None:
         self.attrs["datatype"] = self.form_datatype()
 
-    def add_field(self, name: str, obj: LGDO) -> None:
+    def add_field(self, name: str | int, obj: LGDO) -> None:
         """Add a field to the table."""
         self[name] = obj
         self.update_datatype()
 
-    def remove_field(self, name: str, delete: bool = False) -> None:
+    def remove_field(self, name: str | int, delete: bool = False) -> None:
         """Remove a field from the table.
 
         Parameters
         ----------
         name
             name of the field to be removed
         delete
```

### Comparing `pygama-1.3.1/src/pygama/lgdo/table.py` & `pygama-1.3.2/src/pygama/lgdo/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
                     column = self[col].to_aoesa()
                 else:
                     column = self[col]
 
                 if not hasattr(column, "nda"):
                     raise ValueError(f"column {col} does not have an nda")
                 else:
-                    df[prefix + col] = column.nda.tolist()
+                    df[prefix + str(col)] = column.nda.tolist()
 
         return df
 
     def eval(self, expr_config: dict) -> Table:
         """Apply column operations to the table and return a new table holding
         the resulting columns.
```

### Comparing `pygama-1.3.1/src/pygama/lgdo/vectorofvectors.py` & `pygama-1.3.2/src/pygama/lgdo/vectorofvectors.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/lgdo/waveform_table.py` & `pygama-1.3.2/src/pygama/lgdo/waveform_table.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/logging.py` & `pygama-1.3.2/src/pygama/logging.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/math/histogram.py` & `pygama-1.3.2/src/pygama/math/histogram.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/math/peak_fitting.py` & `pygama-1.3.2/src/pygama/math/peak_fitting.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/math/utils.py` & `pygama-1.3.2/src/pygama/math/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/pargen/AoE_cal.py` & `pygama-1.3.2/src/pygama/pargen/AoE_cal.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/pargen/cuts.py` & `pygama-1.3.2/src/pygama/pargen/cuts.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/pargen/data_cleaning.py` & `pygama-1.3.2/src/pygama/pargen/data_cleaning.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/pargen/dsp_optimize.py` & `pygama-1.3.2/src/pygama/pargen/dsp_optimize.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/pargen/ecal_th.py` & `pygama-1.3.2/src/pygama/pargen/ecal_th.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/pargen/energy_cal.py` & `pygama-1.3.2/src/pygama/pargen/energy_cal.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/pargen/energy_optimisation.py` & `pygama-1.3.2/src/pygama/pargen/energy_optimisation.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/pargen/extract_tau.py` & `pygama-1.3.2/src/pygama/pargen/extract_tau.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/pargen/mse_psd.py` & `pygama-1.3.2/src/pygama/pargen/mse_psd.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/__init__.py` & `pygama-1.3.2/src/pygama/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/buffer_processor/buffer_processor.py` & `pygama-1.3.2/src/pygama/raw/buffer_processor/buffer_processor.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/buffer_processor/lh5_buffer_processor.py` & `pygama-1.3.2/src/pygama/raw/buffer_processor/lh5_buffer_processor.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/build_raw.py` & `pygama-1.3.2/src/pygama/raw/build_raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import logging
 import os
 import time
 
 import hdf5plugin
 import numpy as np
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from pygama import lgdo
 from pygama.lgdo.lh5_store import DEFAULT_HDF5_COMPRESSION
 from pygama.math.utils import sizeof_fmt
 
 from .compass.compass_streamer import CompassStreamer
 from .fc.fc_streamer import FCStreamer
```

### Comparing `pygama-1.3.1/src/pygama/raw/compass/compass_config_parser.py` & `pygama-1.3.2/src/pygama/raw/compass/compass_config_parser.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/compass/compass_event_decoder.py` & `pygama-1.3.2/src/pygama/raw/compass/compass_event_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/compass/compass_header_decoder.py` & `pygama-1.3.2/src/pygama/raw/compass/compass_header_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/compass/compass_streamer.py` & `pygama-1.3.2/src/pygama/raw/compass/compass_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/data_decoder.py` & `pygama-1.3.2/src/pygama/raw/data_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/data_streamer.py` & `pygama-1.3.2/src/pygama/raw/data_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/fc/fc_config_decoder.py` & `pygama-1.3.2/src/pygama/raw/fc/fc_config_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/fc/fc_event_decoder.py` & `pygama-1.3.2/src/pygama/raw/fc/fc_event_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/fc/fc_status_decoder.py` & `pygama-1.3.2/src/pygama/raw/fc/fc_status_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/fc/fc_streamer.py` & `pygama-1.3.2/src/pygama/raw/fc/fc_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/orca/orca_base.py` & `pygama-1.3.2/src/pygama/raw/orca/orca_base.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/orca/orca_digitizers.py` & `pygama-1.3.2/src/pygama/raw/orca/orca_digitizers.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/orca/orca_flashcam.py` & `pygama-1.3.2/src/pygama/raw/orca/orca_flashcam.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/orca/orca_header.py` & `pygama-1.3.2/src/pygama/raw/orca/orca_header.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/orca/orca_header_decoder.py` & `pygama-1.3.2/src/pygama/raw/orca/orca_header_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/orca/orca_packet.py` & `pygama-1.3.2/src/pygama/raw/orca/orca_packet.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/orca/orca_run_decoder.py` & `pygama-1.3.2/src/pygama/raw/orca/orca_run_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/orca/orca_streamer.py` & `pygama-1.3.2/src/pygama/raw/orca/orca_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/raw/raw_buffer.py` & `pygama-1.3.2/src/pygama/raw/raw_buffer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/vis/mpl/clint.mpl` & `pygama-1.3.2/src/pygama/vis/mpl/clint.mpl`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/vis/mpl/root.mpl` & `pygama-1.3.2/src/pygama/vis/mpl/root.mpl`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/src/pygama/vis/waveform_browser.py` & `pygama-1.3.2/src/pygama/vis/waveform_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     def __init__(
         self,
         files_in: str | list[str] | lgdo.LH5Iterator,  # noqa: F821
         lh5_group: str | list[str] = "",
         base_path: str = "",
         entry_list: list[int] | list[list[int]] = None,
         entry_mask: list[int] | list[list[int]] = None,
-        dsp_config: str = None,
+        dsp_config: dict | str = None,
         database: str | dict = None,
         aux_values: pandas.DataFrame = None,
         lines: str | list[str] = "waveform",
         styles: dict[str, list] | str = None,
         legend: str | list[str] = None,
         legend_opts: dict = None,
         n_drawn: int = 1,
```

### Comparing `pygama-1.3.1/src/pygama.egg-info/PKG-INFO` & `pygama-1.3.2/src/pygama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygama
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python package for decoding and processing digitizer data
 Home-page: https://github.com/legend-exp/pygama
 Author: The LEGEND collaboration
 Maintainer: The LEGEND collaboration
 License: GPL-3.0
 Project-URL: Documentation, https://pygama.readthedocs.io
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pygama-1.3.1/src/pygama.egg-info/SOURCES.txt` & `pygama-1.3.2/src/pygama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/conftest.py` & `pygama-1.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/configs/icpc-dsp-config.json` & `pygama-1.3.2/tests/dsp/configs/icpc-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/configs/numpy-parsing.json` & `pygama-1.3.2/tests/dsp/configs/numpy-parsing.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/configs/sipm-dplms-config.json` & `pygama-1.3.2/tests/dsp/configs/sipm-dplms-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/configs/sipm-dsp-config.json` & `pygama-1.3.2/tests/dsp/configs/sipm-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/conftest.py` & `pygama-1.3.2/tests/dsp/conftest.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/processors/dplms_noise_mat.dat` & `pygama-1.3.2/tests/dsp/processors/dplms_noise_mat.dat`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/processors/test_dplms.py` & `pygama-1.3.2/tests/dsp/processors/test_dplms.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/processors/test_dwt.py` & `pygama-1.3.2/tests/dsp/processors/test_dwt.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/processors/test_fixed_time_pickoff.py` & `pygama-1.3.2/tests/dsp/processors/test_fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/processors/test_get_multi_local_extrema.py` & `pygama-1.3.2/tests/dsp/processors/test_get_multi_local_extrema.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/processors/test_histogram.py` & `pygama-1.3.2/tests/dsp/processors/test_histogram.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/test_build_dsp.py` & `pygama-1.3.2/tests/dsp/test_build_dsp.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/test_list_parsing.py` & `pygama-1.3.2/tests/dsp/test_list_parsing.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/test_numpy_constants_parsing.py` & `pygama-1.3.2/tests/dsp/test_numpy_constants_parsing.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/dsp/test_processing_chain.py` & `pygama-1.3.2/tests/dsp/test_processing_chain.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/flow/configs/filedb-config.json` & `pygama-1.3.2/tests/flow/configs/filedb-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/flow/conftest.py` & `pygama-1.3.2/tests/flow/conftest.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/flow/test_data_loader.py` & `pygama-1.3.2/tests/flow/test_data_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 
 def test_no_merge(test_dl):
     test_dl.set_files("all")
     test_dl.set_output(columns=["timestamp"], merge_files=False)
     data = test_dl.load()
 
-    assert isinstance(data, dict)
+    assert isinstance(data, lgdo.Struct)
     assert isinstance(data[0], lgdo.Table)
     assert len(data) == 4  # 4 files
     assert list(data[0].keys()) == ["hit_table", "hit_idx", "timestamp"]
 
 
 def test_outputs(test_dl):
     test_dl.set_files("type == 'phy'")
@@ -143,14 +143,35 @@
     test_dl.set_datastreams([1084803], "ch")
     test_dl.set_output(columns=["is_valid_cal"], fmt="pd.DataFrame")
     data = test_dl.load()
 
     assert (data.is_valid_cal == False).all()  # noqa: E712
 
 
+def test_setter_overwrite(test_dl):
+    test_dl.set_files("all")
+    test_dl.set_datastreams([1084803, 1084804, 1121600], "ch")
+    test_dl.set_cuts({"hit": "trapEmax > 5000"})
+    test_dl.set_output(columns=["trapEmax"])
+
+    data = test_dl.load().get_dataframe()
+
+    test_dl.set_files("timestamp == '20230318T012144Z'")
+    test_dl.set_datastreams([1084803, 1121600], "ch")
+    test_dl.set_cuts({"hit": "trapEmax > 0"})
+
+    data2 = test_dl.load().get_dataframe()
+
+    assert 1084804 not in data2["hit_table"]
+    assert len(pd.unique(data2["file"])) == 1
+    assert len(data2.query("hit_table == 1084803")) > len(
+        data.query("hit_table == 1084803")
+    )
+
+
 def test_browse(test_dl):
     test_dl.set_files("type == 'phy'")
     test_dl.set_datastreams([1057600, 1059201], "ch")
     test_dl.set_output(
         fmt="pd.DataFrame", columns=["timestamp", "channel", "energies", "energy_in_pe"]
     )
     wb = test_dl.browse()
```

### Comparing `pygama-1.3.1/tests/flow/test_filedb.py` & `pygama-1.3.2/tests/flow/test_filedb.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/hit/configs/spms-hit-a-config.json` & `pygama-1.3.2/tests/hit/configs/spms-hit-a-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/hit/test_build_hit.py` & `pygama-1.3.2/tests/hit/test_build_hit.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat` & `pygama-1.3.2/tests/lgdo/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/compression/sigcompress/special-wf-clipped.dat` & `pygama-1.3.2/tests/lgdo/compression/sigcompress/special-wf-clipped.dat`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/compression/test_compression.py` & `pygama-1.3.2/tests/lgdo/compression/test_compression.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/compression/test_radware_sigcompress.py` & `pygama-1.3.2/tests/lgdo/compression/test_radware_sigcompress.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/compression/test_str2wfcodec.py` & `pygama-1.3.2/tests/lgdo/compression/test_str2wfcodec.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/compression/test_uleb128_zigzag_diff.py` & `pygama-1.3.2/tests/lgdo/compression/test_uleb128_zigzag_diff.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_array.py` & `pygama-1.3.2/tests/lgdo/test_array.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_arrayofequalsizedarrays.py` & `pygama-1.3.2/tests/lgdo/test_arrayofequalsizedarrays.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_encoded.py` & `pygama-1.3.2/tests/lgdo/test_encoded.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_fixedsizearray.py` & `pygama-1.3.2/tests/lgdo/test_fixedsizearray.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_lgdo_utils.py` & `pygama-1.3.2/tests/lgdo/test_lgdo_utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_lh5_iterator.py` & `pygama-1.3.2/tests/lgdo/test_lh5_iterator.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_lh5_store.py` & `pygama-1.3.2/tests/lgdo/test_lh5_store.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_representations.py` & `pygama-1.3.2/tests/lgdo/test_representations.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_scalar.py` & `pygama-1.3.2/tests/lgdo/test_scalar.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_struct.py` & `pygama-1.3.2/tests/lgdo/test_struct.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_table.py` & `pygama-1.3.2/tests/lgdo/test_table.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_table_eval.py` & `pygama-1.3.2/tests/lgdo/test_table_eval.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_vectorofvectors.py` & `pygama-1.3.2/tests/lgdo/test_vectorofvectors.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/lgdo/test_waveform_table.py` & `pygama-1.3.2/tests/lgdo/test_waveform_table.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/math/test_fwhm.py` & `pygama-1.3.2/tests/math/test_fwhm.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor.py` & `pygama-1.3.2/tests/raw/buffer_processor/test_buffer_processor.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json` & `pygama-1.3.2/tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json` & `pygama-1.3.2/tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/buffer_processor/test_lh5_buffer_processor.py` & `pygama-1.3.2/tests/raw/buffer_processor/test_lh5_buffer_processor.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/compass/conftest.py` & `pygama-1.3.2/tests/raw/compass/conftest.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/compass/test_compass_event_decoder.py` & `pygama-1.3.2/tests/raw/compass/test_compass_event_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/compass/test_compass_header_decoder.py` & `pygama-1.3.2/tests/raw/compass/test_compass_header_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/compass/test_compass_streamer.py` & `pygama-1.3.2/tests/raw/compass/test_compass_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/fc/test_fc_config_decoder.py` & `pygama-1.3.2/tests/raw/fc/test_fc_config_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/fc/test_fc_event_decoder.py` & `pygama-1.3.2/tests/raw/fc/test_fc_event_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/fc/test_fc_status_decoder.py` & `pygama-1.3.2/tests/raw/fc/test_fc_status_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/fc/test_fc_streamer.py` & `pygama-1.3.2/tests/raw/fc/test_fc_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/orca/test_or_run_decoder_for_run.py` & `pygama-1.3.2/tests/raw/orca/test_or_run_decoder_for_run.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/test_build_raw.py` & `pygama-1.3.2/tests/raw/test_build_raw.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/test_cli.py` & `pygama-1.3.2/tests/raw/test_cli.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/test_daq_to_raw.py` & `pygama-1.3.2/tests/raw/test_daq_to_raw.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/raw/test_raw_buffer.py` & `pygama-1.3.2/tests/raw/test_raw_buffer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/vis/configs/hpge-dsp-config.json` & `pygama-1.3.2/tests/vis/configs/hpge-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.3.1/tests/vis/test_waveform_browser.py` & `pygama-1.3.2/tests/vis/test_waveform_browser.py`

 * *Files identical despite different names*

