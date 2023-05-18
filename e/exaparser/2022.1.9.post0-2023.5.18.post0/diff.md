# Comparing `tmp/exaparser-2022.1.9.post0.tar.gz` & `tmp/exaparser-2023.5.18.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exaparser-2022.1.9.post0.tar", last modified: Sun Jan  9 00:18:57 2022, max compression
+gzip compressed data, was "exaparser-2023.5.18.post0.tar", last modified: Thu May 18 19:21:21 2023, max compression
```

## Comparing `exaparser-2022.1.9.post0.tar` & `exaparser-2023.5.18.post0.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.048404 exaparser-2022.1.9.post0/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.036404 exaparser-2022.1.9.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1542 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7292 2022-01-09 00:18:57.048404 exaparser-2022.1.9.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6831 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/config
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-01-09 00:18:56.000000 exaparser-2022.1.9.post0/exaparser/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      762 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser/data/
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/data/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser/data/handlers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/data/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/data/handlers/disk.py
--rw-r--r--   0 runner    (1001) docker     (121)     7331 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/data/handlers/exabyte.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/data/handlers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser/job/
--rw-r--r--   0 runner    (1001) docker     (121)     3310 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser/job/compute/
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/job/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/job/compute/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser/job/compute/managers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/job/compute/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/job/compute/managers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/job/compute/managers/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/templates/espresso.json
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/templates/shell.json
--rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/templates/vasp.json
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser/workflow/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/subworkflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser/workflow/units/
--rw-r--r--   0 runner    (1001) docker     (121)      861 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser/workflow/units/execution/
--rw-r--r--   0 runner    (1001) docker     (121)     3997 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/units/execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser/workflow/units/execution/modeling/
--rw-r--r--   0 runner    (1001) docker     (121)     3727 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/units/execution/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1865 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/units/execution/modeling/espresso.py
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/units/execution/modeling/vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser/workflow/units/execution/scripting/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/units/execution/scripting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/units/execution/scripting/shell.py
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/units/execution/scripting/shell_with_results.py
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/units/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/units/subworkflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/exaparser/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.040404 exaparser-2022.1.9.post0/exaparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7292 2022-01-09 00:18:56.000000 exaparser-2022.1.9.post0/exaparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5409 2022-01-09 00:18:57.000000 exaparser-2022.1.9.post0/exaparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-09 00:18:56.000000 exaparser-2022.1.9.post0/exaparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-01-09 00:18:56.000000 exaparser-2022.1.9.post0/exaparser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-01-09 00:18:56.000000 exaparser-2022.1.9.post0/exaparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-09 00:18:56.000000 exaparser-2022.1.9.post0/exaparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     1221 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-01-09 00:18:57.052404 exaparser-2022.1.9.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.044404 exaparser-2022.1.9.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.036404 exaparser-2022.1.9.post0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.044404 exaparser-2022.1.9.post0/tests/fixtures/espresso/
--rw-r--r--   0 runner    (1001) docker     (121)     4904 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/shell-job.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.044404 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/
--rwxr-xr-x   0 runner    (1001) docker     (121)      319 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/job.rms
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.036404 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.044404 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.044404 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (121)   160469 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/evc.dat
--rw-r--r--   0 runner    (1001) docker     (121)    21019 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.044404 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (121)   151125 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/evc.dat
--rw-r--r--   0 runner    (1001) docker     (121)    19851 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.044404 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (121)   151125 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/evc.dat
--rw-r--r--   0 runner    (1001) docker     (121)    19851 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.048404 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (121)   150101 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/evc.dat
--rw-r--r--   0 runner    (1001) docker     (121)    19723 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.048404 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (121)   151125 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/evc.dat
--rw-r--r--   0 runner    (1001) docker     (121)    19851 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/gkvectors.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.048404 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (121)   150101 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/evc.dat
--rw-r--r--   0 runner    (1001) docker     (121)    19723 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/gkvectors.dat
--rw-r--r--   0 runner    (1001) docker     (121)   377892 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/charge-density.dat
--rw-r--r--   0 runner    (1001) docker     (121)    16970 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/data-file.xml
--rw-r--r--   0 runner    (1001) docker     (121)   160388 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/gvectors.dat
--rw-r--r--   0 runner    (1001) docker     (121)   577736 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.048404 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/pseudo/
--rw-r--r--   0 runner    (1001) docker     (121)   577736 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/pseudo/si_pbe_gbrv_1.0.upf
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/pw-scf.in
--rw-r--r--   0 runner    (1001) docker     (121)    11496 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/stdout
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.048404 exaparser-2022.1.9.post0/tests/fixtures/vasp/
--rw-r--r--   0 runner    (1001) docker     (121)     4886 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/shell-job.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.048404 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/CHG
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/CHGCAR
--rw-r--r--   0 runner    (1001) docker     (121)      513 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/CONTCAR
--rw-r--r--   0 runner    (1001) docker     (121)    11075 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/DOSCAR
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/EIGENVAL
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/IBZKPT
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-01-09 00:18:32.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/INCAR
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/KPOINTS
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/OSZICAR
--rw-r--r--   0 runner    (1001) docker     (121)    53180 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/OUTCAR
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/PCDAT
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/POSCAR
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/POTCAR
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/WAVECAR
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/XDATCAR
--rwxr-xr-x   0 runner    (1001) docker     (121)      301 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/job.rms
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/stdout
--rw-r--r--   0 runner    (1001) docker     (121)    37663 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.048404 exaparser-2022.1.9.post0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/integration/test_job.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:57.048404 exaparser-2022.1.9.post0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-09 00:18:33.000000 exaparser-2022.1.9.post0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.928170 exaparser-2023.5.18.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.900169 exaparser-2023.5.18.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-18 19:21:21.928170 exaparser-2023.5.18.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.904169 exaparser-2023.5.18.post0/exaparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      762 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.904169 exaparser-2023.5.18.post0/exaparser/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/data/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.904169 exaparser-2023.5.18.post0/exaparser/data/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/data/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/data/handlers/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/data/handlers/exabyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/data/handlers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.904169 exaparser-2023.5.18.post0/exaparser/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/job/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/job/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/job/compute/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/job/compute/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/job/compute/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/job/compute/managers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/job/compute/managers/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.912169 exaparser-2023.5.18.post0/exaparser/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/templates/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/templates/shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/templates/vasp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/subworkflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/workflow/units/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/espresso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.908169 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/scripting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/scripting/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/execution/scripting/shell_with_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/units/subworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/exaparser/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.912169 exaparser-2023.5.18.post0/exaparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 19:21:21.000000 exaparser-2023.5.18.post0/exaparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1221 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-18 19:21:21.928170 exaparser-2023.5.18.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.916169 exaparser-2023.5.18.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.900169 exaparser-2023.5.18.post0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.916169 exaparser-2023.5.18.post0/tests/fixtures/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/shell-job.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.916169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/job.rms
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.900169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.916169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.920169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   160469 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.920169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.920169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.920169 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   150101 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.924170 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   151125 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/gkvectors.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.924170 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   150101 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/gkvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   377892 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/charge-density.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    16970 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/data-file.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   160388 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/gvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.924170 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/pseudo/
+-rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/pseudo/si_pbe_gbrv_1.0.upf
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/pw-scf.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.924170 exaparser-2023.5.18.post0/tests/fixtures/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/shell-job.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.928170 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/CHG
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/CHGCAR
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/CONTCAR
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/DOSCAR
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/EIGENVAL
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/IBZKPT
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/INCAR
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/KPOINTS
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/OSZICAR
+-rw-r--r--   0 runner    (1001) docker     (123)    53180 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/OUTCAR
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/PCDAT
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/POTCAR
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/WAVECAR
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/XDATCAR
+-rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/job.rms
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/stdout
+-rw-r--r--   0 runner    (1001) docker     (123)    37663 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.928170 exaparser-2023.5.18.post0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/integration/test_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:21:21.928170 exaparser-2023.5.18.post0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:20:39.000000 exaparser-2023.5.18.post0/tests/utils.py
```

### Comparing `exaparser-2022.1.9.post0/.github/workflows/cicd.yml` & `exaparser-2023.5.18.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/.gitignore` & `exaparser-2023.5.18.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/LICENSE` & `exaparser-2023.5.18.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/PKG-INFO` & `exaparser-2023.5.18.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: exaparser
-Version: 2022.1.9.post0
+Version: 2023.5.18.post0
 Summary: Exabyte Parser
 Home-page: https://github.com/Exabyte-io/exaparser
 Author: Exabyte Inc.
 Author-email: info@exabyte.io
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -156,9 +154,7 @@
 - Add complex workflow templates
 
 ## Links
 
 1. [Exabyte Source of Schemas and Examples (ESSE), Github Repository](https://github.com/exabyte-io/exabyte-esse)
 1. [Vienna Ab-initio Simulation Package (VASP), official website](https://cms.mpi.univie.ac.at/vasp/)
 1. [Quantum ESPRESSO, Official Website](https://www.quantum-espresso.org/)
-
-
```

### Comparing `exaparser-2022.1.9.post0/README.md` & `exaparser-2023.5.18.post0/README.md`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/config` & `exaparser-2023.5.18.post0/config`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/cli.py` & `exaparser-2023.5.18.post0/exaparser/cli.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/config.py` & `exaparser-2023.5.18.post0/exaparser/config.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/data/factory.py` & `exaparser-2023.5.18.post0/exaparser/data/factory.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/data/handlers/disk.py` & `exaparser-2023.5.18.post0/exaparser/data/handlers/disk.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/data/handlers/exabyte.py` & `exaparser-2023.5.18.post0/exaparser/data/handlers/exabyte.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/enums.py` & `exaparser-2023.5.18.post0/exaparser/enums.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/job/__init__.py` & `exaparser-2023.5.18.post0/exaparser/job/__init__.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/job/compute/__init__.py` & `exaparser-2023.5.18.post0/exaparser/job/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/templates/espresso.json` & `exaparser-2023.5.18.post0/exaparser/templates/espresso.json`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/templates/shell.json` & `exaparser-2023.5.18.post0/exaparser/templates/shell.json`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/templates/vasp.json` & `exaparser-2023.5.18.post0/exaparser/templates/vasp.json`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/utils.py` & `exaparser-2023.5.18.post0/exaparser/utils.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/workflow/subworkflow.py` & `exaparser-2023.5.18.post0/exaparser/workflow/subworkflow.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/workflow/units/__init__.py` & `exaparser-2023.5.18.post0/exaparser/workflow/units/__init__.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/workflow/units/execution/__init__.py` & `exaparser-2023.5.18.post0/exaparser/workflow/units/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/workflow/units/execution/modeling/__init__.py` & `exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/workflow/units/execution/modeling/espresso.py` & `exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/espresso.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/workflow/units/execution/modeling/vasp.py` & `exaparser-2023.5.18.post0/exaparser/workflow/units/execution/modeling/vasp.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/workflow/units/execution/scripting/shell.py` & `exaparser-2023.5.18.post0/exaparser/workflow/units/execution/scripting/shell.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/workflow/units/execution/scripting/shell_with_results.py` & `exaparser-2023.5.18.post0/exaparser/workflow/units/execution/scripting/shell_with_results.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/workflow/units/factory.py` & `exaparser-2023.5.18.post0/exaparser/workflow/units/factory.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/workflow/units/subworkflow.py` & `exaparser-2023.5.18.post0/exaparser/workflow/units/subworkflow.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser/workflow/workflow.py` & `exaparser-2023.5.18.post0/exaparser/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/exaparser.egg-info/PKG-INFO` & `exaparser-2023.5.18.post0/exaparser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: exaparser
-Version: 2022.1.9.post0
+Version: 2023.5.18.post0
 Summary: Exabyte Parser
 Home-page: https://github.com/Exabyte-io/exaparser
 Author: Exabyte Inc.
 Author-email: info@exabyte.io
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -156,9 +154,7 @@
 - Add complex workflow templates
 
 ## Links
 
 1. [Exabyte Source of Schemas and Examples (ESSE), Github Repository](https://github.com/exabyte-io/exabyte-esse)
 1. [Vienna Ab-initio Simulation Package (VASP), official website](https://cms.mpi.univie.ac.at/vasp/)
 1. [Quantum ESPRESSO, Official Website](https://www.quantum-espresso.org/)
-
-
```

### Comparing `exaparser-2022.1.9.post0/exaparser.egg-info/SOURCES.txt` & `exaparser-2023.5.18.post0/exaparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/requirements-dev.txt` & `exaparser-2023.5.18.post0/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 ase==3.17.0
 certifi==2020.11.8
 chardet==3.0.4
 click==7.1.2
-coverage==5.3
 cycler==0.10.0
 decorator==4.4.2
 esse==2021.05.06
-exabyte-api-client==2021.06.25
+exabyte-api-client==2023.5.18.post0
 exabyte-json-include==2021.05.06
-express-py==2021.05.06
+express-py==2022.1.14.post0
 Flask==1.1.2
 idna==2.7
 itsdangerous==1.1.0
-Jinja2==2.11.2
+Jinja2==2.11.3
 jsonschema==2.6.0
 kiwisolver==1.3.1
 MarkupSafe==1.1.1
 matplotlib==3.3.3
-mock==4.0.2
 monty==4.0.2
 mpmath==1.1.0
 munch==2.5.0
 networkx==2.5
 numpy==1.19.5;python_version<"3.7"
 numpy==1.20.1;python_version>="3.7"
 palettable==3.3.0
 pandas==1.1.4
-Pillow==8.0.1
+Pillow==8.3.2
 plotly==4.13.0
 pymatgen==2020.4.29
 pyparsing==2.4.7
 python-dateutil==2.8.1
 python-slugify==2.0.1
 pytz==2020.4
-PyYAML==5.3.1
-requests==2.20.1
+PyYAML==5.4
+requests==2.26.0
 retrying==1.3.3
 ruamel.yaml==0.16.12
 ruamel.yaml.clib==0.2.2
 scipy==1.5.4
 six==1.15.0
 spglib==1.16.0
 sympy==1.7
-toml==0.10.2
 tabulate==0.8.7
 Unidecode==1.1.1
-urllib3==1.24.3
+urllib3==1.26.5
 Werkzeug==1.0.1
--e .[test]
```

### Comparing `exaparser-2022.1.9.post0/run-tests.sh` & `exaparser-2023.5.18.post0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/setup.cfg` & `exaparser-2023.5.18.post0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 [options]
 package_dir = 
 	= .
 packages = find:
 python_requires = >= 3.6
 install_requires = 
-	exabyte-api-client>=2020.10.19
-	express-py>=2020.10.19
-	requests>=2.20.1
+	exabyte-api-client>=2022.1.13.post0
+	express-py>=2022.1.14.post0
+	requests>=2.26.0
 
 [options.extras_require]
 test = 
 	coverage[toml]>=5.3
 	mock>=1.3.0
 	numpy>=1.17.3
```

### Comparing `exaparser-2022.1.9.post0/tests/__init__.py` & `exaparser-2023.5.18.post0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/shell-job.json` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/shell-job.json`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/eigenval.xml` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/evc.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/gkvectors.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00001/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/eigenval.xml` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/evc.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/gkvectors.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00002/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/eigenval.xml` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/evc.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/gkvectors.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00003/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/eigenval.xml` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/evc.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/gkvectors.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00004/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/eigenval.xml` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/evc.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/gkvectors.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00005/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/eigenval.xml` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/eigenval.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/evc.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/evc.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/gkvectors.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/K00006/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/charge-density.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/charge-density.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/data-file.xml` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/data-file.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/gvectors.dat` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/gvectors.dat`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/outdir/__prefix__.save/si_pbe_gbrv_1.0.upf`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/pseudo/si_pbe_gbrv_1.0.upf` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/pseudo/si_pbe_gbrv_1.0.upf`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/pw-scf.in` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/pw-scf.in`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/espresso/test-001/stdout` & `exaparser-2023.5.18.post0/tests/fixtures/espresso/test-001/stdout`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/vasp/shell-job.json` & `exaparser-2023.5.18.post0/tests/fixtures/vasp/shell-job.json`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/CONTCAR` & `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/CONTCAR`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/DOSCAR` & `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/DOSCAR`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/EIGENVAL` & `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/EIGENVAL`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/OSZICAR` & `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/OSZICAR`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/OUTCAR` & `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/OUTCAR`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/POTCAR` & `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/POTCAR`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/stdout` & `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/stdout`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/fixtures/vasp/test-001/vasprun.xml` & `exaparser-2023.5.18.post0/tests/fixtures/vasp/test-001/vasprun.xml`

 * *Files identical despite different names*

### Comparing `exaparser-2022.1.9.post0/tests/integration/test_job.py` & `exaparser-2023.5.18.post0/tests/integration/test_job.py`

 * *Files identical despite different names*

