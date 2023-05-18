# Comparing `tmp/ephysiopy-1.9.17.tar.gz` & `tmp/ephysiopy-1.9.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysiopy-1.9.17.tar", last modified: Tue May  2 12:34:41 2023, max compression
+gzip compressed data, was "ephysiopy-1.9.18.tar", last modified: Thu May 18 17:37:36 2023, max compression
```

## Comparing `ephysiopy-1.9.17.tar` & `ephysiopy-1.9.18.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:41.612868 ephysiopy-1.9.17/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-02 12:34:41.612868 ephysiopy-1.9.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:41.608868 ephysiopy-1.9.17/ephysiopy/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:41.608868 ephysiopy-1.9.17/ephysiopy/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/axona/axonaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/axona/file_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/axona/tetrode_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/axona/tintcolours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:41.612868 ephysiopy-1.9.17/ephysiopy/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34025 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/common/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/common/ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/common/fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/common/gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/common/mle_von_mises_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/common/phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/common/rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/common/spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/common/statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:41.612868 ephysiopy-1.9.17/ephysiopy/format_converters/
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/format_converters/OE_Axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/format_converters/OE_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/format_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:41.612868 ephysiopy-1.9.17/ephysiopy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23946 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/io/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:41.612868 ephysiopy-1.9.17/ephysiopy/openephys2py/
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/openephys2py/KiloSort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/openephys2py/OESettings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/openephys2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:41.612868 ephysiopy-1.9.17/ephysiopy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_axona_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_axona_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_dacq2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:41.612868 ephysiopy-1.9.17/ephysiopy/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32396 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/ephysiopy/visualise/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:34:41.608868 ephysiopy-1.9.17/ephysiopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-02 12:34:41.000000 ephysiopy-1.9.17/ephysiopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-02 12:34:41.000000 ephysiopy-1.9.17/ephysiopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:34:41.000000 ephysiopy-1.9.17/ephysiopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 12:34:41.000000 ephysiopy-1.9.17/ephysiopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 12:34:41.000000 ephysiopy-1.9.17/ephysiopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 12:34:41.612868 ephysiopy-1.9.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-02 12:34:35.000000 ephysiopy-1.9.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:36.010528 ephysiopy-1.9.18/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-18 17:37:36.010528 ephysiopy-1.9.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:36.002528 ephysiopy-1.9.18/ephysiopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:36.002528 ephysiopy-1.9.18/ephysiopy/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/axona/axonaIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/axona/file_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/axona/tetrode_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/axona/tintcolours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:36.006528 ephysiopy-1.9.18/ephysiopy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/common/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/common/ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/common/fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/common/gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/common/mle_von_mises_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/common/phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/common/rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/common/spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/common/statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:36.006528 ephysiopy-1.9.18/ephysiopy/format_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/format_converters/OE_Axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/format_converters/OE_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/format_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:36.006528 ephysiopy-1.9.18/ephysiopy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23946 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/io/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:36.006528 ephysiopy-1.9.18/ephysiopy/openephys2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/openephys2py/KiloSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/openephys2py/OESettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/openephys2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:36.006528 ephysiopy-1.9.18/ephysiopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_axona_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_axona_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_dacq2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:36.010528 ephysiopy-1.9.18/ephysiopy/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32324 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/ephysiopy/visualise/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:37:36.002528 ephysiopy-1.9.18/ephysiopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-18 17:37:35.000000 ephysiopy-1.9.18/ephysiopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-18 17:37:35.000000 ephysiopy-1.9.18/ephysiopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:37:35.000000 ephysiopy-1.9.18/ephysiopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-18 17:37:35.000000 ephysiopy-1.9.18/ephysiopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 17:37:35.000000 ephysiopy-1.9.18/ephysiopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-18 17:37:36.010528 ephysiopy-1.9.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-18 17:37:29.000000 ephysiopy-1.9.18/setup.py
```

### Comparing `ephysiopy-1.9.17/LICENSE` & `ephysiopy-1.9.18/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/PKG-INFO` & `ephysiopy-1.9.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.17
+Version: 1.9.18
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.17/README.md` & `ephysiopy-1.9.18/README.md`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/axona/axonaIO.py` & `ephysiopy-1.9.18/ephysiopy/axona/axonaIO.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/axona/file_headers.py` & `ephysiopy-1.9.18/ephysiopy/axona/file_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/axona/tetrode_dict.py` & `ephysiopy-1.9.18/ephysiopy/axona/tetrode_dict.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/axona/tintcolours.py` & `ephysiopy-1.9.18/ephysiopy/axona/tintcolours.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/common/binning.py` & `ephysiopy-1.9.18/ephysiopy/common/binning.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,14 @@
     @property
     def var2Bin(self):
         return self._var2Bin
 
     @var2Bin.setter
     def var2Bin(self, value):
         self._var2Bin = value
-        # self._calcBinEdges()
 
     @property
     def mapType(self):
         return self._mapType
 
     @mapType.setter
     def mapType(self, value):
@@ -152,32 +151,49 @@
     def nBins(self, value):
         '''
         Sets the number of bins
         '''
         if self.var2Bin == VariableToBin.XY:
             x_lims, y_lims = self._getXYLimits()
             if len(value) == 1:
-                _x = np.linspace(x_lims[0], x_lims[1], int(value[0]))
-                _y = np.linspace(y_lims[0], y_lims[1], int(value[0]))
+                _x, bs_x = np.linspace(x_lims[0],
+                                       x_lims[1],
+                                       int(value[0]),
+                                       retstep=True)
+                _y, bs_y = np.linspace(y_lims[0],
+                                       y_lims[1],
+                                       int(value[0]),
+                                       retstep=True)
             elif len(value) == 2:
-                _x = np.linspace(x_lims[0], x_lims[1], int(value[0]))
-                _y = np.linspace(y_lims[0], y_lims[1], int(value[1]))
+                _x, bs_x = np.linspace(x_lims[0],
+                                       x_lims[1],
+                                       int(value[0]),
+                                       retstep=True)
+                _y, bs_y = np.linspace(y_lims[0],
+                                       y_lims[1],
+                                       int(value[1]),
+                                       retstep=True)
             self._binedges = _y, _x
+            self.binsize = np.mean([bs_x, bs_y])
         elif self.var2Bin == VariableToBin.DIR:
-            self._binedges = [np.linspace(0, 360 + self.binsize, value[0])]
+            self._binedges, binsize = np.linspace(0,
+                                                  360 + self.binsize,
+                                                  value[0],
+                                                  retstep=True)
+            self.binsize = binsize
         elif self.var2Bin == VariableToBin.SPEED:
             maxspeed = np.max(self.speed)
-            self._binedges = [np.linspace(0, maxspeed, value[0])]
-        self._calcBinDims()
+            self._binedges, binsize = np.linspace(0,
+                                                  maxspeed,
+                                                  value[0],
+                                                  retstep=True)
+            self.binsize = binsize
 
     @property
     def binedges(self):
-        # Returns binedges calculated in _calcBinEdges and based on cmsPerBin
-        # if self._binedges is None:
-        #     self._binedges = self._calcBinEdges(self.binsize)
         return self._binedges
 
     @binedges.setter
     def binedges(self, value):
         self._binedges = value
 
     @property
@@ -281,18 +297,16 @@
             self.binedges = np.arange(0, 360 + binsize, binsize)
         elif self.var2Bin == VariableToBin.SPEED:
             maxspeed = np.max(self.speed)
             # assume min speed = 0
             self.binedges = np.arange(0, maxspeed, binsize)
         else:  # self.var2Bin == VariableToBin.XY:
             x_lims, y_lims = self._getXYLimits()
-            n_x = np.ceil((x_lims[1] - x_lims[0]) / binsize)
-            n_y = np.ceil((y_lims[1] - y_lims[0]) / binsize)
-            _x = np.linspace(x_lims[0], x_lims[1], int(n_x))
-            _y = np.linspace(y_lims[0], y_lims[1], int(n_y))
+            _x = np.arange(x_lims[0], x_lims[1], binsize)
+            _y = np.arange(y_lims[0], y_lims[1], binsize)
             self.binedges = _y, _x
         self._calcBinDims()
         return self.binedges
 
     def getMap(self, spkWeights,
                varType=VariableToBin.XY,
                mapType=MapType.RATE,
```

### Comparing `ephysiopy-1.9.17/ephysiopy/common/ephys_generic.py` & `ephysiopy-1.9.18/ephysiopy/common/ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/common/fieldcalcs.py` & `ephysiopy-1.9.18/ephysiopy/common/fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/common/gridcell.py` & `ephysiopy-1.9.18/ephysiopy/common/gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/common/mle_von_mises_vals.py` & `ephysiopy-1.9.18/ephysiopy/common/mle_von_mises_vals.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/common/phasecoding.py` & `ephysiopy-1.9.18/ephysiopy/common/phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/common/rhythmicity.py` & `ephysiopy-1.9.18/ephysiopy/common/rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/common/spikecalcs.py` & `ephysiopy-1.9.18/ephysiopy/common/spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/common/statscalcs.py` & `ephysiopy-1.9.18/ephysiopy/common/statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/common/utils.py` & `ephysiopy-1.9.18/ephysiopy/common/utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/format_converters/OE_Axona.py` & `ephysiopy-1.9.18/ephysiopy/format_converters/OE_Axona.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/format_converters/OE_numpy.py` & `ephysiopy-1.9.18/ephysiopy/format_converters/OE_numpy.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/io/recording.py` & `ephysiopy-1.9.18/ephysiopy/io/recording.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/openephys2py/KiloSort.py` & `ephysiopy-1.9.18/ephysiopy/openephys2py/KiloSort.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/openephys2py/OESettings.py` & `ephysiopy-1.9.18/ephysiopy/openephys2py/OESettings.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/conftest.py` & `ephysiopy-1.9.18/ephysiopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/test_axona_headers.py` & `ephysiopy-1.9.18/ephysiopy/tests/test_axona_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/test_axona_io.py` & `ephysiopy-1.9.18/ephysiopy/tests/test_axona_io.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/test_binning.py` & `ephysiopy-1.9.18/ephysiopy/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/test_dacq2py.py` & `ephysiopy-1.9.18/ephysiopy/tests/test_dacq2py.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/test_ephys_generic.py` & `ephysiopy-1.9.18/ephysiopy/tests/test_ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/test_fieldcalcs.py` & `ephysiopy-1.9.18/ephysiopy/tests/test_fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/test_gridcell.py` & `ephysiopy-1.9.18/ephysiopy/tests/test_gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/test_phasecoding.py` & `ephysiopy-1.9.18/ephysiopy/tests/test_phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/test_rhythmicity.py` & `ephysiopy-1.9.18/ephysiopy/tests/test_rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/test_spikecalcs.py` & `ephysiopy-1.9.18/ephysiopy/tests/test_spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/test_statscalcs.py` & `ephysiopy-1.9.18/ephysiopy/tests/test_statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/tests/test_utils.py` & `ephysiopy-1.9.18/ephysiopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/ephysiopy/visualise/plotting.py` & `ephysiopy-1.9.18/ephysiopy/visualise/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,25 +45,24 @@
         self.PosCalcs = None
 
     def initialise(self):
         xy = getattr(self.PosCalcs, "xy")
         hdir = getattr(self.PosCalcs, "dir")
         speed = getattr(self.PosCalcs, "speed")
         ppm = getattr(self.PosCalcs, "ppm")
-        binsize = getattr(self.PosCalcs, "binsize", 3)
         setattr(self, "npos", xy.shape[1])
         pos_weights = None
         if hdir is not None:
             if np.ma.is_masked(hdir):
                 pos_weights = np.array(~hdir.mask).astype(int)
             else:
                 pos_weights = np.ones_like(hdir)
         self.RateMap = RateMap(
             xy=xy, hdir=hdir, speed=speed, pos_weights=pos_weights, ppm=ppm,
-            xyInCms=True, binsize=binsize)
+            xyInCms=True)
         self.RateMap.x_lims = getattr(self, 'x_lims', None)  # 2-tuple
         self.RateMap.y_lims = getattr(self, 'y_lims', None)
 
     def getSpikePosIndices(self, spk_times: np.ndarray):
         pos_times = getattr(self.PosCalcs, 'xyTS')
         idx = np.searchsorted(pos_times, spk_times)
         idx[idx == len(pos_times)] = idx[idx == len(pos_times)] - 1
```

### Comparing `ephysiopy-1.9.17/ephysiopy.egg-info/PKG-INFO` & `ephysiopy-1.9.18/ephysiopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.17
+Version: 1.9.18
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.17/ephysiopy.egg-info/SOURCES.txt` & `ephysiopy-1.9.18/ephysiopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.17/setup.py` & `ephysiopy-1.9.18/setup.py`

 * *Files identical despite different names*

