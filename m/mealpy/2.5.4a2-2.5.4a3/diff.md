# Comparing `tmp/mealpy-2.5.4a2.tar.gz` & `tmp/mealpy-2.5.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mealpy-2.5.4a2.tar", last modified: Mon May  8 09:26:07 2023, max compression
+gzip compressed data, was "mealpy-2.5.4a3.tar", last modified: Thu May 18 04:30:05 2023, max compression
```

## Comparing `mealpy-2.5.4a2.tar` & `mealpy-2.5.4a3.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.389421 mealpy-2.5.4a2/
--rw-r--r--   0 runner    (1001) docker     (123)    58037 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    90608 2023-05-08 09:26:07.389421 mealpy-2.5.4a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    88069 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.369420 mealpy-2.5.4a2/mealpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.369420 mealpy-2.5.4a2/mealpy/bio_based/
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/BBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/BBOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/BMO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/EOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/IWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/SBO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/SMA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/SOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/SOS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/TPO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/TSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/VCS.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/WHO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.373420 mealpy-2.5.4a2/mealpy/evolutionary_based/
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/CRO.py
--rw-r--r--   0 runner    (1001) docker     (123)    40520 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/DE.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/EP.py
--rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/ES.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/FPA.py
--rw-r--r--   0 runner    (1001) docker     (123)    38686 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/GA.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/MA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.373420 mealpy-2.5.4a2/mealpy/human_based/
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/BRO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/BSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/CA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/CHIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/FBIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/GSKA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/HBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/HCO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/ICA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/LCO.py
--rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/QSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/SARO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/SPBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/SSDO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/TLO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/TOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/WarSO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.377420 mealpy-2.5.4a2/mealpy/math_based/
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/AOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/CEM.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/CGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/CircleSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/GBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/HC.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/INFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/PSS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/RUN.py
--rw-r--r--   0 runner    (1001) docker     (123)    13376 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/SCA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/SHIO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/multitask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.377420 mealpy-2.5.4a2/mealpy/music_based/
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/music_based/HS.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/music_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33893 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.377420 mealpy-2.5.4a2/mealpy/physics_based/
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/ASO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/ArchOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/CDO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/EFO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/EO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/EVO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/FLA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/HGSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/MVO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/NRO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/RIME.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/SA.py
--rw-r--r--   0 runner    (1001) docker     (123)    20823 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/TWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/WDO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.385421 mealpy-2.5.4a2/mealpy/swarm_based/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ABC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ACOR.py
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/AGTO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ALO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/AO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ARO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/AVOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/BA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/BES.py
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/BFO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/BSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    17152 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/BeesA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/COA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/CSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/CSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/CoatiOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/DMOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/DO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/EHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ESOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/FA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/FFA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/FFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/FOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/FOX.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/GJO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/GOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/GTO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/GWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/HBA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/HGS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/HHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/JA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/MFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/MGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/MPA.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/MRFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/MSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/NGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/NMRA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/OOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/PFA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/POA.py
--rw-r--r--   0 runner    (1001) docker     (123)    27073 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/PSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SCSO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SHO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SLO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SRSR.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SSpiderA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SSpiderO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/STO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SeaHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ServalOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/TDO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/TSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/WOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/WaOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ZOA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.385421 mealpy-2.5.4a2/mealpy/system_based/
--rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/system_based/AEO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/system_based/GCO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/system_based/WCA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/system_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.389421 mealpy-2.5.4a2/mealpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/termination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.389421 mealpy-2.5.4a2/mealpy/utils/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/visualize/linechart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.369420 mealpy-2.5.4a2/mealpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    90608 2023-05-08 09:26:07.000000 mealpy-2.5.4a2/mealpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-08 09:26:07.000000 mealpy-2.5.4a2/mealpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:26:07.000000 mealpy-2.5.4a2/mealpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 09:26:07.000000 mealpy-2.5.4a2/mealpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 09:26:07.000000 mealpy-2.5.4a2/mealpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:26:07.389421 mealpy-2.5.4a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.389421 mealpy-2.5.4a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/tests/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/tests/test_tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.017120 mealpy-2.5.4a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    58092 2023-05-18 04:28:16.000000 mealpy-2.5.4a3/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 04:28:16.000000 mealpy-2.5.4a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-18 04:28:16.000000 mealpy-2.5.4a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    90608 2023-05-18 04:30:05.017120 mealpy-2.5.4a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    88069 2023-05-18 04:28:16.000000 mealpy-2.5.4a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:04.981119 mealpy-2.5.4a3/mealpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:04.989120 mealpy-2.5.4a3/mealpy/bio_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/BBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/BBOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/BMO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/EOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/IWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/SBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/SMA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/SOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/SOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/TPO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/TSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/VCS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/WHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/bio_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:04.993120 mealpy-2.5.4a3/mealpy/evolutionary_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/CRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40520 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/DE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/EP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/ES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/FPA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38895 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/GA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/MA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/evolutionary_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:04.997120 mealpy-2.5.4a3/mealpy/human_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/BRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/BSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/CA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/CHIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/FBIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/GSKA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/HBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/HCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/ICA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/LCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/QSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/SARO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/SPBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/SSDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/TLO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/TOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/WarSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/human_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.005120 mealpy-2.5.4a3/mealpy/math_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/AOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/CEM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/CGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/CircleSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/GBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/HC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/PSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/RUN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/SCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/SHIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/math_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/multitask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.005120 mealpy-2.5.4a3/mealpy/music_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/music_based/HS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/music_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33913 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.005120 mealpy-2.5.4a3/mealpy/physics_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/ASO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/ArchOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/CDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/EFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/EO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/EVO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/FLA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/HGSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/MVO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/NRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/RIME.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/SA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20830 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/TWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/WDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/physics_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.013120 mealpy-2.5.4a3/mealpy/swarm_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ABC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ACOR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/AGTO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ALO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/AO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ARO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/AVOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/BA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/BES.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/BFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/BSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/BeesA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/COA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/CSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/CSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/CoatiOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/DMOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/DO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/EHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ESOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/FA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/FFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/FFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/FOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/FOX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/GJO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/GOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18697 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/GTO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/GWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/HBA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/HGS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/HHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/JA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/MFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/MGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/MPA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/MRFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/MSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/NGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/NMRA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/OOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/PFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/POA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26955 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/PSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SCSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12436 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SLO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SRSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SSpiderA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SSpiderO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/STO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/SeaHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ServalOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/TDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/TSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/WOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/WaOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/ZOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/swarm_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.013120 mealpy-2.5.4a3/mealpy/system_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/system_based/AEO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/system_based/GCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/system_based/WCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/system_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.017120 mealpy-2.5.4a3/mealpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/termination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.017120 mealpy-2.5.4a3/mealpy/utils/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/mealpy/utils/visualize/linechart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:04.985120 mealpy-2.5.4a3/mealpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    90608 2023-05-18 04:30:04.000000 mealpy-2.5.4a3/mealpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-18 04:30:04.000000 mealpy-2.5.4a3/mealpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 04:30:04.000000 mealpy-2.5.4a3/mealpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 04:30:04.000000 mealpy-2.5.4a3/mealpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 04:30:04.000000 mealpy-2.5.4a3/mealpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 04:30:05.017120 mealpy-2.5.4a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 04:30:05.017120 mealpy-2.5.4a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/tests/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-18 04:28:17.000000 mealpy-2.5.4a3/tests/test_tuner.py
```

### Comparing `mealpy-2.5.4a2/ChangeLog.md` & `mealpy-2.5.4a3/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   * 2.4.0 <= mealpy <= 2.4.2 (From this version, algorithms can solve discrete problem)
   * mealpy >= 2.5.1 (Define model 1 time, solve multiple problems)
 
 
 # Version 2.5.4
 
 ### Update
++ Remove deepcopy() to improve the computational speed
 + Update the parameter's order in Tuner class  
 + Update the saving's bug when using Termination in Multitask
 + Remove ILA optimizer 
 + Rename "amend_position()" definition in some algorithms to "bounded_position()".
 + Add a "amend_position()" function in Optimizer class. This function will call two functions.
   + bounded_position() from optimizer. This means for optimizer level (get in valid range of position)
   + amend_position() from problem. This means for problem level (transform to the correct solution)
```

### Comparing `mealpy-2.5.4a2/LICENSE` & `mealpy-2.5.4a3/LICENSE`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/PKG-INFO` & `mealpy-2.5.4a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mealpy
-Version: 2.5.4a2
+Version: 2.5.4a3
 Summary: MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python
 Home-page: https://github.com/thieu1995/mealpy
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mealpy.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mealpy
```

### Comparing `mealpy-2.5.4a2/README.md` & `mealpy-2.5.4a3/README.md`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/__init__.py` & `mealpy-2.5.4a3/mealpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # >>>
 # >>> ## Run the algorithm
 # >>> model = PSO.C_PSO(epoch=5, pop_size=50, name="C-PSO")
 # >>> best_position, best_fitness = model.solve(problem)
 # >>> print(f"Best solution: {best_position}, Best fitness: {best_fitness}")
 
 
-__version__ = "2.5.4-alpha.2"
+__version__ = "2.5.4-alpha.3"
 
 from .bio_based import (BBO, BBOA, BMO, EOA, IWO, SBO, SMA, SOA, SOS, TPO, TSA, VCS, WHO)
 from .evolutionary_based import (CRO, DE, EP, ES, FPA, GA, MA)
 from .human_based import (BRO, BSO, CA, CHIO, FBIO, GSKA, HBO, HCO, ICA, LCO, QSA, SARO, SPBO, SSDO, TLO, TOA, WarSO)
 from .math_based import (AOA, CEM, CGO, CircleSA, GBO, HC, INFO, PSS, RUN, SCA, SHIO)
 from .physics_based import (ArchOA, ASO, CDO, EFO, EO, EVO, FLA, HGSO, MVO, NRO, RIME, SA, TWO, WDO)
 from .swarm_based import (ABC, ACOR, AGTO, ALO, AO, ARO, AVOA, BA, BeesA, BES, BFO, BSA, COA, CoatiOA, CSA, CSO,
```

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/BBO.py` & `mealpy-2.5.4a3/mealpy/bio_based/BBO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 12:24, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalBBO(Optimizer):
     """
     The original version of: Biogeography-Based Optimization (BBO)
 
@@ -75,27 +74,26 @@
         Args:
             epoch (int): The current iteration
         """
         _, pop_elites, _ = self.get_special_solutions(self.pop, best=self.elites)
         pop = []
         for idx in range(0, self.pop_size):
             # Probabilistic migration to the i-th position
-            pos_new = deepcopy(self.pop[idx][self.ID_POS])
+            pos_new = self.pop[idx][self.ID_POS].copy()
             for j in range(self.problem.n_dims):
                 if np.random.uniform() < self.mr[idx]:  # Should we immigrate?
                     # Pick a position from which to emigrate (roulette wheel selection)
                     random_number = np.random.uniform() * np.sum(self.mu)
                     select = self.mu[0]
                     select_index = 0
                     while (random_number > select) and (select_index < self.pop_size - 1):
                         select_index += 1
                         select += self.mu[select_index]
                     # this is the migration step
                     pos_new[j] = self.pop[select_index][self.ID_POS][j]
-
             noise = np.random.uniform(self.problem.lb, self.problem.ub)
             condition = np.random.random(self.problem.n_dims) < self.p_m
             pos_new = np.where(condition, noise, pos_new)
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
```

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/BBOA.py` & `mealpy-2.5.4a3/mealpy/bio_based/BBOA.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         pop_new = []
         for idx in range(0, self.pop_size):
             kk = np.random.choice(list(set(range(0, self.pop_size)) - {idx}))
             if self.compare_agent(self.pop[idx], self.pop[kk]):
                 pos_new = self.pop[idx][self.ID_POS] + np.random.rand() * (self.pop[idx][self.ID_POS] - self.pop[kk][self.ID_POS])
             else:
                 pos_new = self.pop[idx][self.ID_POS] + np.random.rand() * (self.pop[kk][self.ID_POS] - self.pop[idx][self.ID_POS])
+            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
                 self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop = self.greedy_selection_population(self.pop, pop_new)
```

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/BMO.py` & `mealpy-2.5.4a3/mealpy/bio_based/BMO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/EOA.py` & `mealpy-2.5.4a3/mealpy/bio_based/EOA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 14:52, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalEOA(Optimizer):
     """
     The developed version: Earthworm Optimisation Algorithm (EOA)
 
@@ -127,15 +126,15 @@
             self.pop = self.greedy_selection_population(self.pop, pop)
         self.dyn_beta = self.gamma * self.beta
         self.pop = self.get_sorted_strim_population(self.pop, self.pop_size)
 
         pos_list = np.array([item[self.ID_POS] for item in self.pop])
         x_mean = np.mean(pos_list, axis=0)
         ## Cauchy mutation (CM)
-        cauchy_w = deepcopy(self.g_best[self.ID_POS])
+        cauchy_w = self.g_best[self.ID_POS].copy()
         pop_new = []
         for idx in range(self.n_best, self.pop_size):  # Don't allow the elites to be mutated
             condition = np.random.random(self.problem.n_dims) < self.p_m
             cauchy_w = np.where(condition, x_mean, cauchy_w)
             x_t1 = (cauchy_w + self.g_best[self.ID_POS]) / 2
             pos_new = self.amend_position(x_t1, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
@@ -145,15 +144,15 @@
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop[self.n_best:] = self.greedy_selection_population(pop_new, self.pop[self.n_best:])
 
         ## Elitism Strategy: Replace the worst with the previous generation's elites.
         self.pop, local_best = self.get_global_best_solution(self.pop)
         for i in range(0, self.n_best):
-            self.pop[self.pop_size - i - 1] = deepcopy(pop_elites[i])
+            self.pop[self.pop_size - i - 1] = pop_elites[i].copy()
 
         ## Make sure the population does not have duplicates.
         new_set = set()
         for idx, agent in enumerate(self.pop):
             if tuple(agent[self.ID_POS].tolist()) in new_set:
                 self.pop[idx] = self.create_solution(self.problem.lb, self.problem.ub)
             else:
```

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/IWO.py` & `mealpy-2.5.4a3/mealpy/bio_based/IWO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/SBO.py` & `mealpy-2.5.4a3/mealpy/bio_based/SBO.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 12:48, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseSBO(Optimizer):
     """
     The developed version: Satin Bowerbird Optimizer (SBO)
 
@@ -179,35 +178,35 @@
             epoch (int): The current iteration
         """
         # (percent of the difference between the upper and lower limit (Eq. 7))
         self.sigma = self.psw * (self.problem.ub - self.problem.lb)
 
         ## Calculate the probability of bowers using Eqs. (1) and (2)
         fx_list = np.array([agent[self.ID_TAR][self.ID_FIT] for agent in self.pop])
-        fit_list = deepcopy(fx_list)
-        for i in range(0, self.pop_size):
-            if fx_list[i] < 0:
-                fit_list[i] = 1.0 + np.abs(fx_list[i])
+        fit_list = fx_list.copy()
+        for idx in range(0, self.pop_size):
+            if fx_list[idx] < 0:
+                fit_list[idx] = 1.0 + np.abs(fx_list[idx])
             else:
-                fit_list[i] = 1.0 / (1.0 + np.abs(fx_list[i]))
+                fit_list[idx] = 1.0 / (1.0 + np.abs(fx_list[idx]))
         fit_sum = np.sum(fit_list)
         ## Calculating the probability of each bower
         prob_list = fit_list / fit_sum
         pop_new = []
-        for i in range(0, self.pop_size):
-            pos_new = deepcopy(self.pop[i][self.ID_POS])
+        for idx in range(0, self.pop_size):
+            pos_new = self.pop[idx][self.ID_POS].copy()
             for j in range(0, self.problem.n_dims):
                 ### Select a bower using roulette wheel
-                idx = self.roulette_wheel_selection__(prob_list)
+                rdx = self.roulette_wheel_selection__(prob_list)
                 ### Calculating Step Size
-                lamda = self.alpha / (1 + prob_list[idx])
-                pos_new[j] = self.pop[i][self.ID_POS][j] + lamda * \
-                             ((self.pop[idx][self.ID_POS][j] + self.g_best[self.ID_POS][j]) / 2 - self.pop[i][self.ID_POS][j])
+                lamda = self.alpha / (1 + prob_list[rdx])
+                pos_new[j] = self.pop[idx][self.ID_POS][j] + lamda * \
+                             ((self.pop[rdx][self.ID_POS][j] + self.g_best[self.ID_POS][j]) / 2 - self.pop[idx][self.ID_POS][j])
                 ### Mutation
                 if np.random.uniform() < self.p_m:
-                    pos_new[j] = self.pop[i][self.ID_POS][j] + np.random.normal(0, 1) * self.sigma[j]
+                    pos_new[j] = self.pop[idx][self.ID_POS][j] + np.random.normal(0, 1) * self.sigma[j]
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
-                self.pop[i] = [pos_new, self.get_target_wrapper(pos_new)]
+                self.pop[idx] = [pos_new, self.get_target_wrapper(pos_new)]
         if self.mode in self.AVAILABLE_MODES:
             self.pop = self.update_target_wrapper_population(pop_new)
```

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/SMA.py` & `mealpy-2.5.4a3/mealpy/bio_based/SMA.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 20:22, 12/06/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseSMA(Optimizer):
     """
     The developed version: Slime Mould Algorithm (SMA)
 
@@ -198,28 +197,27 @@
 
         a = np.arctanh(-((epoch + 1) / (self.epoch+1)) + 1)  # Eq.(2.4)
         b = 1 - (epoch + 1) / (self.epoch+1)
 
         pop_new = []
         for idx in range(0, self.pop_size):
             # Update the Position of search agent
-            current_agent = deepcopy(self.pop[idx])
+            pos, fit, weight = self.pop[idx][self.ID_POS].copy(), self.pop[idx][self.ID_TAR][self.ID_FIT], self.pop[idx][self.ID_WEI].copy()
             if np.random.uniform() < self.p_t:  # Eq.(2.7)
-                current_agent[self.ID_POS] = np.random.uniform(self.problem.lb, self.problem.ub)
+                pos = np.random.uniform(self.problem.lb, self.problem.ub)
             else:
-                p = np.tanh(np.abs(current_agent[self.ID_TAR][self.ID_FIT] - self.g_best[self.ID_TAR][self.ID_FIT]))  # Eq.(2.2)
+                p = np.tanh(np.abs(fit - self.g_best[self.ID_TAR][self.ID_FIT]))  # Eq.(2.2)
                 vb = np.random.uniform(-a, a, self.problem.n_dims)  # Eq.(2.3)
                 vc = np.random.uniform(-b, b, self.problem.n_dims)
                 for j in range(0, self.problem.n_dims):
                     # two positions randomly selected from population
                     id_a, id_b = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 2, replace=False)
                     if np.random.uniform() < p:  # Eq.(2.1)
-                        current_agent[self.ID_POS][j] = self.g_best[self.ID_POS][j] + \
-                            vb[j] * (current_agent[self.ID_WEI][j] * self.pop[id_a][self.ID_POS][j] - self.pop[id_b][self.ID_POS][j])
+                        pos[j] = self.g_best[self.ID_POS][j] + vb[j] * (weight[j] * self.pop[id_a][self.ID_POS][j] - self.pop[id_b][self.ID_POS][j])
                     else:
-                        current_agent[self.ID_POS][j] = vc[j] * current_agent[self.ID_POS][j]
-            pos_new = self.amend_position(current_agent[self.ID_POS], self.problem.lb, self.problem.ub)
+                        pos[j] = vc[j] * pos[j]
+            pos_new = self.amend_position(pos, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None, np.zeros(self.problem.n_dims)])
             if self.mode not in self.AVAILABLE_MODES:
                 self.pop[idx] = [pos_new, self.get_target_wrapper(pos_new), np.zeros(self.problem.n_dims)]
         if self.mode in self.AVAILABLE_MODES:
             self.pop = self.update_target_wrapper_population(pop_new)
```

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/SOA.py` & `mealpy-2.5.4a3/mealpy/bio_based/SOA.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,20 +70,20 @@
             C = A * self.pop[idx][self.ID_POS]                                  # Eq. 5
             D = np.abs(C + M)                                                   # Eq. 9
             k = np.random.uniform(0, 2*np.pi)
             r = uu * np.exp(k*vv)
             xx = r * np.cos(k)
             yy = r * np.sin(k)
             zz = r * k
-            x_new = xx * yy * zz * D + np.random.normal(0, 1) * self.g_best[self.ID_POS]                 # Eq. 14
-            x_new = self.amend_position(x_new, self.problem.lb, self.problem.ub)
-            pop_new.append([x_new, None])
+            pos_new = xx * yy * zz * D + np.random.normal(0, 1) * self.g_best[self.ID_POS]                 # Eq. 14
+            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+            pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
-                target = self.get_target_wrapper(x_new)
-                self.pop[idx] = self.get_better_solution([x_new, target], self.pop[idx])
+                target = self.get_target_wrapper(pos_new)
+                self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop = self.greedy_selection_population(self.pop, pop_new)
 
 
 class OriginalSOA(Optimizer):
     """
@@ -146,13 +146,13 @@
             C = A * self.pop[idx][self.ID_POS]                                  # Eq. 5
             D = np.abs(C + M)                                                   # Eq. 9
             k = np.random.uniform(0, 2*np.pi)
             r = uu * np.exp(k*vv)
             xx = r * np.cos(k)
             yy = r * np.sin(k)
             zz = r * k
-            x_new = xx * yy * zz * D + self.g_best[self.ID_POS]                 # Eq. 14
-            x_new = self.amend_position(x_new, self.problem.lb, self.problem.ub)
-            pop_new.append([x_new, None])
+            pos_new = xx * yy * zz * D + self.g_best[self.ID_POS]                 # Eq. 14
+            pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+            pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
-                pop_new[-1][self.ID_TAR] = self.get_target_wrapper(x_new)
+                pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         self.pop = self.update_target_wrapper_population(pop_new)
```

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/SOS.py` & `mealpy-2.5.4a3/mealpy/bio_based/SOS.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,10 +82,11 @@
                 self.pop[idx] = [xi_new, xi_tar]
 
             ## Parasitism phase
             jdx = np.random.choice(list(set(range(0, self.pop_size)) - {idx}))
             temp_idx = np.random.randint(0, self.problem.n_dims)
             xi_new = self.pop[jdx][self.ID_POS].copy()
             xi_new[temp_idx] = self.generate_position(self.problem.lb, self.problem.ub)[temp_idx]
+            xi_new = self.amend_position(xi_new, self.problem.lb, self.problem.ub)
             xi_tar = self.get_target_wrapper(xi_new)
             if self.compare_agent([xi_new, xi_tar], self.pop[idx]):
                 self.pop[idx] = [xi_new, xi_tar]
```

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/TPO.py` & `mealpy-2.5.4a3/mealpy/bio_based/TPO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/TSA.py` & `mealpy-2.5.4a3/mealpy/bio_based/TSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/VCS.py` & `mealpy-2.5.4a3/mealpy/bio_based/VCS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/bio_based/WHO.py` & `mealpy-2.5.4a3/mealpy/bio_based/WHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/evolutionary_based/CRO.py` & `mealpy-2.5.4a3/mealpy/evolutionary_based/CRO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/evolutionary_based/DE.py` & `mealpy-2.5.4a3/mealpy/evolutionary_based/DE.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/evolutionary_based/EP.py` & `mealpy-2.5.4a3/mealpy/evolutionary_based/EP.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 19:27, 10/04/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalEP(Optimizer):
     """
     The original version of: Evolutionary Programming (EP)
 
@@ -194,16 +193,16 @@
                 if self.compare_agent(pop[i], pop[rand_idx]):
                     pop[i][self.ID_WIN] += 1
                 else:
                     pop[rand_idx][self.ID_WIN] += 1
 
         ## Keep the top population, but 50% of left population will make a comeback an take the good position
         pop = sorted(pop, key=lambda agent: agent[self.ID_WIN], reverse=True)
-        pop_new = deepcopy(pop[:self.pop_size])
-        pop_left = deepcopy(pop[self.pop_size:])
+        pop_new = pop[:self.pop_size]
+        pop_left = pop[self.pop_size:]
 
         ## Choice random 50% of population left
         pop_comeback = []
         idx_list = np.random.choice(range(0, len(pop_left)), int(0.5 * len(pop_left)), replace=False)
         for idx in idx_list:
             pos_new = pop_left[idx][self.ID_POS] + self.get_levy_flight_step(multiplier=0.01, size=self.problem.n_dims, case=-1)
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
```

### Comparing `mealpy-2.5.4a2/mealpy/evolutionary_based/ES.py` & `mealpy-2.5.4a3/mealpy/evolutionary_based/ES.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/evolutionary_based/FPA.py` & `mealpy-2.5.4a3/mealpy/evolutionary_based/FPA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/evolutionary_based/GA.py` & `mealpy-2.5.4a3/mealpy/evolutionary_based/GA.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Created by "Thieu" at 09:33, 16/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
 from mealpy.optimizer import Optimizer
-import copy as cp
 
 
 class BaseGA(Optimizer):
     """
     The original version of: Genetic Algorithm (GA)
 
     Links:
@@ -122,14 +121,16 @@
 
         Returns:
             list: The position of dad and mom
         """
         if self.selection == "roulette":
             id_c1 = self.get_index_roulette_wheel_selection(list_fitness)
             id_c2 = self.get_index_roulette_wheel_selection(list_fitness)
+            while id_c2 == id_c1:
+                id_c2 = self.get_index_roulette_wheel_selection(list_fitness)
         elif self.selection == "random":
             id_c1, id_c2 = np.random.choice(range(self.pop_size), 2, replace=False)
         else:   ## tournament
             id_c1, id_c2 = self.get_index_kway_tournament_selection(self.pop, k_way=self.k_way, output=2)
         return self.pop[id_c1][self.ID_POS], self.pop[id_c2][self.ID_POS]
 
     def selection_process_00__(self, pop_selected):
@@ -146,14 +147,16 @@
         Returns:
             list: The position of dad and mom
         """
         if self.selection == "roulette":
             list_fitness = np.array([agent[self.ID_TAR][self.ID_FIT] for agent in pop_selected])
             id_c1 = self.get_index_roulette_wheel_selection(list_fitness)
             id_c2 = self.get_index_roulette_wheel_selection(list_fitness)
+            while id_c2 == id_c1:
+                id_c2 = self.get_index_roulette_wheel_selection(list_fitness)
         elif self.selection == "random":
             id_c1, id_c2 = np.random.choice(range(len(pop_selected)), 2, replace=False)
         else:   ## tournament
             id_c1, id_c2 = self.get_index_kway_tournament_selection(pop_selected, k_way=self.k_way, output=2)
         return pop_selected[id_c1][self.ID_POS], pop_selected[id_c2][self.ID_POS]
 
     def selection_process_01__(self, pop_dad, pop_mom):
@@ -301,22 +304,26 @@
             if np.random.uniform() < self.pc:
                 child1, child2 = self.crossover_process__(child1, child2)
 
             ### Mutation
             child1 = self.mutation_process__(child1)
             child2 = self.mutation_process__(child2)
 
-            pop_new.append([self.amend_position(child1, self.problem.lb, self.problem.ub), None])
-            pop_new.append([self.amend_position(child2, self.problem.lb, self.problem.ub), None])
+            child1 = self.amend_position(child1, self.problem.lb, self.problem.ub)
+            child2 = self.amend_position(child2, self.problem.lb, self.problem.ub)
+
+            pop_new.append([child1, None])
+            pop_new.append([child2, None])
 
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-2][self.ID_TAR] = self.get_target_wrapper(child1)
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(child2)
+        if self.mode in self.AVAILABLE_MODES:
+            pop_new = self.update_target_wrapper_population(pop_new)
         ### Survivor Selection
-        pop_new = self.update_target_wrapper_population(pop_new)
         self.pop = self.survivor_process__(self.pop, pop_new)
 
 
 class SingleGA(BaseGA):
     """
     The developed single-point mutation of: Genetic Algorithm (GA)
 
@@ -522,18 +529,18 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        pop_new = cp.deepcopy(self.pop[:self.n_elite_best])
+        pop_new = self.pop[:self.n_elite_best]
 
         if self.strategy == 0:
-            pop_old = cp.deepcopy(self.pop[self.n_elite_best:])
+            pop_old = self.pop[self.n_elite_best:]
             for idx in range(self.n_elite_best, self.pop_size):
                 ### Selection
                 child1, child2 = self.selection_process_00__(pop_old)
                 ### Crossover
                 if np.random.uniform() < self.pc:
                     child1, child2 = self.crossover_process__(child1, child2)
                 child = child1 if np.random.random() <= 0.5 else child2
@@ -542,16 +549,16 @@
                 ### Survivor Selection
                 pos_new = self.amend_position(child, self.problem.lb, self.problem.ub)
                 pop_new.append([pos_new, None])
                 if self.mode not in self.AVAILABLE_MODES:
                     pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
             self.pop = self.update_target_wrapper_population(pop_new)
         else:
-            pop_dad = cp.deepcopy(self.pop[self.n_elite_best:self.n_elite_best+self.n_elite_worst])
-            pop_mom = cp.deepcopy(self.pop[self.n_elite_best+self.n_elite_worst:])
+            pop_dad = self.pop[self.n_elite_best:self.n_elite_best+self.n_elite_worst]
+            pop_mom = self.pop[self.n_elite_best+self.n_elite_worst:]
             for idx in range(self.n_elite_best, self.pop_size):
                 ### Selection
                 child1, child2 = self.selection_process_01__(pop_dad, pop_mom)
                 ### Crossover
                 if np.random.uniform() < self.pc:
                     child1, child2 = self.crossover_process__(child1, child2)
                 child = child1 if np.random.random() <= 0.5 else child2
@@ -744,18 +751,18 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        pop_new = cp.deepcopy(self.pop[:self.n_elite_best])
+        pop_new = self.pop[:self.n_elite_best]
 
         if self.strategy == 0:
-            pop_old = cp.deepcopy(self.pop[self.n_elite_best:])
+            pop_old = self.pop[self.n_elite_best:]
             for idx in range(self.n_elite_best, self.pop_size):
                 ### Selection
                 child1, child2 = self.selection_process_00__(pop_old)
                 ### Crossover
                 if np.random.uniform() < self.pc:
                     child1, child2 = self.crossover_process__(child1, child2)
                 child = child1 if np.random.random() <= 0.5 else child2
@@ -764,16 +771,16 @@
                 ### Survivor Selection
                 pos_new = self.amend_position(child, self.problem.lb, self.problem.ub)
                 pop_new.append([pos_new, None])
                 if self.mode not in self.AVAILABLE_MODES:
                     pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
             self.pop = self.update_target_wrapper_population(pop_new)
         else:
-            pop_dad = cp.deepcopy(self.pop[self.n_elite_best:self.n_elite_best+self.n_elite_worst])
-            pop_mom = cp.deepcopy(self.pop[self.n_elite_best+self.n_elite_worst:])
+            pop_dad = self.pop[self.n_elite_best:self.n_elite_best+self.n_elite_worst]
+            pop_mom = self.pop[self.n_elite_best+self.n_elite_worst:]
             for idx in range(self.n_elite_best, self.pop_size):
                 ### Selection
                 child1, child2 = self.selection_process_01__(pop_dad, pop_mom)
                 ### Crossover
                 if np.random.uniform() < self.pc:
                     child1, child2 = self.crossover_process__(child1, child2)
                 child = child1 if np.random.random() <= 0.5 else child2
```

### Comparing `mealpy-2.5.4a2/mealpy/evolutionary_based/MA.py` & `mealpy-2.5.4a3/mealpy/evolutionary_based/MA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 14:22, 11/04/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalMA(Optimizer):
     """
     The original version of: Memetic Algorithm (MA)
 
@@ -112,16 +111,15 @@
         for idx in range(0, self.problem.n_dims):
             param = bitstring[idx * self.bits_per_param: (idx + 1) * self.bits_per_param]  # Select 16 bit every time
             vector[idx] = self.problem.lb[idx] + ((self.problem.ub[idx] - self.problem.lb[idx]) / ((2.0 ** self.bits_per_param) - 1)) * int(param, 2)
         return vector
 
     def crossover__(self, dad=None, mom=None):
         if np.random.uniform() >= self.pc:
-            temp = deepcopy([dad])
-            return temp[0]
+            return dad
         else:
             child = ""
             for idx in range(0, self.bits_total):
                 if np.random.uniform() < 0.5:
                     child += dad[idx]
                 else:
                     child += mom[idx]
@@ -133,18 +131,18 @@
             if np.random.uniform() < self.pc:
                 child += "0" if bit == "1" else "1"
             else:
                 child += bit
         return child
 
     def bits_climber__(self, child=None):
-        current = deepcopy(child)
+        current = child
         list_local = []
         for idx in range(0, self.max_local_gens):
-            child = deepcopy(current)
+            child = current
             bitstring_new = self.point_mutation__(child[self.ID_BIT])
             pos_new = self.decode_(bitstring_new)
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             list_local.append([pos_new, None, bitstring_new])
             if self.mode not in self.AVAILABLE_MODES:
                 list_local[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         list_local = self.update_target_wrapper_population(list_local)
@@ -170,15 +168,15 @@
         Args:
             epoch (int): The current iteration
         """
         ## Binary tournament
         children = []
         for idx in range(0, self.pop_size):
             idx_offspring = self.get_index_kway_tournament_selection(self.pop, k_way=2, output=1)[0]
-            children.append(deepcopy(self.pop[idx_offspring]))
+            children.append(self.pop[idx_offspring].copy())
         pop = []
         for idx in range(0, self.pop_size):
             ancient = children[idx + 1] if idx % 2 == 0 else children[idx - 1]
             if idx == self.pop_size - 1:
                 ancient = children[0]
             bitstring_new = self.crossover__(children[idx][self.ID_BIT], ancient[self.ID_BIT])
             bitstring_new = self.point_mutation__(bitstring_new)
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/BRO.py` & `mealpy-2.5.4a3/mealpy/human_based/BRO.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Created by "Thieu" at 09:17, 09/11/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
 from scipy.spatial.distance import cdist
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseBRO(Optimizer):
     """
     The developed version: Battle Royale Optimization (BRO)
 
@@ -60,16 +59,16 @@
         self.set_parameters(["epoch", "pop_size", "threshold"])
         self.support_parallel_modes = False
         self.sort_flag = False
 
     def initialize_variables(self):
         shrink = np.ceil(np.log10(self.epoch))
         self.dyn_delta = np.round(self.epoch / shrink)
-        self.problem.lb_updated = deepcopy(self.problem.lb)
-        self.problem.ub_updated = deepcopy(self.problem.ub)
+        self.problem.lb_updated = self.problem.lb.copy()
+        self.problem.ub_updated = self.problem.ub.copy()
 
     def create_solution(self, lb=None, ub=None, pos=None):
         """
         Overriding method in Optimizer class
 
         Returns:
             list: wrapper of solution with format [position, target, damage]
@@ -100,48 +99,48 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        for i in range(self.pop_size):
+        for idx in range(self.pop_size):
             # Compare ith soldier with nearest one (jth)
-            j = self.find_idx_min_distance__(self.pop[i][self.ID_POS], self.pop)
-            if self.compare_agent(self.pop[i], self.pop[j]):
+            jdx = self.find_idx_min_distance__(self.pop[idx][self.ID_POS], self.pop)
+            if self.compare_agent(self.pop[idx], self.pop[jdx]):
                 ## Update Winner based on global best solution
-                pos_new = self.pop[i][self.ID_POS] + np.random.normal(0, 1) * \
-                          np.mean(np.array([self.pop[i][self.ID_POS], self.g_best[self.ID_POS]]), axis=0)
+                pos_new = self.pop[idx][self.ID_POS] + np.random.normal(0, 1) * \
+                          np.mean(np.array([self.pop[idx][self.ID_POS], self.g_best[self.ID_POS]]), axis=0)
                 pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
                 target = self.get_target_wrapper(pos_new)
-                dam_new = self.pop[i][self.ID_DAM] - 1  ## Substract damaged hurt -1 to go next battle
-                self.pop[i] = [pos_new, target, dam_new]
+                dam_new = self.pop[idx][self.ID_DAM] - 1  ## Substract damaged hurt -1 to go next battle
+                self.pop[idx] = [pos_new, target, dam_new]
                 ## Update Loser
-                if self.pop[j][self.ID_DAM] < self.threshold:  ## If loser not dead yet, move it based on general
-                    pos_new = np.random.uniform() * (np.maximum(self.pop[j][self.ID_POS], self.g_best[self.ID_POS]) -
-                                                     np.minimum(self.pop[j][self.ID_POS], self.g_best[self.ID_POS])) + \
-                              np.maximum(self.pop[j][self.ID_POS], self.g_best[self.ID_POS])
-                    dam_new = self.pop[j][self.ID_DAM] + 1
+                if self.pop[jdx][self.ID_DAM] < self.threshold:  ## If loser not dead yet, move it based on general
+                    pos_new = np.random.uniform() * (np.maximum(self.pop[jdx][self.ID_POS], self.g_best[self.ID_POS]) -
+                                                     np.minimum(self.pop[jdx][self.ID_POS], self.g_best[self.ID_POS])) + \
+                              np.maximum(self.pop[jdx][self.ID_POS], self.g_best[self.ID_POS])
+                    dam_new = self.pop[jdx][self.ID_DAM] + 1
 
-                    self.pop[j][self.ID_TAR] = self.get_target_wrapper(self.pop[j][self.ID_POS])
+                    self.pop[jdx][self.ID_TAR] = self.get_target_wrapper(self.pop[jdx][self.ID_POS])
                 else:  ## Loser dead and respawn again
                     pos_new = self.generate_position(self.problem.lb_updated, self.problem.ub_updated)
                     dam_new = 0
                 pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
                 target = self.get_target_wrapper(pos_new)
-                self.pop[j] = [pos_new, target, dam_new]
+                self.pop[jdx] = [pos_new, target, dam_new]
             else:
                 ## Update Loser by following position of Winner
-                self.pop[i] = deepcopy(self.pop[j])
+                self.pop[idx] = self.pop[jdx].copy()
                 ## Update Winner by following position of General to protect the King and General
-                pos_new = self.pop[j][self.ID_POS] + np.random.uniform() * (self.g_best[self.ID_POS] - self.pop[j][self.ID_POS])
+                pos_new = self.pop[jdx][self.ID_POS] + np.random.uniform() * (self.g_best[self.ID_POS] - self.pop[jdx][self.ID_POS])
                 pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
                 target = self.get_target_wrapper(pos_new)
                 dam_new = 0
-                self.pop[j] = [pos_new, target, dam_new]
+                self.pop[jdx] = [pos_new, target, dam_new]
         if epoch >= self.dyn_delta:  # max_epoch = 1000 -> delta = 300, 450, >500,....
             pos_list = np.array([self.pop[idx][self.ID_POS] for idx in range(0, self.pop_size)])
             pos_std = np.std(pos_list, axis=0)
             lb = self.g_best[self.ID_POS] - pos_std
             ub = self.g_best[self.ID_POS] + pos_std
             self.problem.lb_updated = np.clip(lb, self.problem.lb_updated, self.problem.ub_updated)
             self.problem.ub_updated = np.clip(ub, self.problem.lb_updated, self.problem.ub_updated)
@@ -199,20 +198,20 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        for i in range(self.pop_size):
+        for idx in range(self.pop_size):
             # Compare ith soldier with nearest one (jth)
-            j = self.find_idx_min_distance__(self.pop[i][self.ID_POS], self.pop)
-            dam, vic = i, j  ## This error in the algorithm's flow in the paper, But in the matlab code, he changed.
-            if self.compare_agent(self.pop[i], self.pop[j]):
-                dam, vic = j, i  ## The mistake also here in the paper.
+            jdx = self.find_idx_min_distance__(self.pop[idx][self.ID_POS], self.pop)
+            dam, vic = idx, jdx  ## This error in the algorithm's flow in the paper, But in the matlab code, he changed.
+            if self.compare_agent(self.pop[idx], self.pop[jdx]):
+                dam, vic = jdx, idx  ## The mistake also here in the paper.
             if self.pop[dam][self.ID_DAM] < self.threshold:
                 pos_new = np.random.uniform(0, 1, self.problem.n_dims) * \
                           (np.maximum(self.pop[dam][self.ID_POS], self.g_best[self.ID_POS]) -
                            np.minimum(self.pop[dam][self.ID_POS], self.g_best[self.ID_POS])) + \
                           np.maximum(self.pop[dam][self.ID_POS], self.g_best[self.ID_POS])
                 self.pop[dam][self.ID_POS] = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
                 self.pop[dam][self.ID_TAR] = self.get_target_wrapper(self.pop[dam][self.ID_POS])
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/BSO.py` & `mealpy-2.5.4a3/mealpy/human_based/BSO.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         self.m_solution = int(self.pop_size / self.m_clusters)
         self.pop_group, self.centers = None, None
 
     def find_cluster__(self, pop_group):
         centers = []
         for i in range(0, self.m_clusters):
             _, local_best = self.get_global_best_solution(pop_group[i])
-            centers.append(deepcopy(local_best))
+            centers.append(local_best)
         return centers
 
     def initialization(self):
         if self.pop is None:
             self.pop = self.create_population(self.pop_size)
         self.pop_group = self.create_pop_group(self.pop, self.m_clusters, self.m_solution)
         self.centers = self.find_cluster__(self.pop_group)
@@ -93,42 +93,42 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        epxilon = 1 - 1 * (epoch + 1) / self.epoch  # 1. Changed here, no need: k
+        epsilon = 1 - 1 * (epoch + 1) / self.epoch  # 1. Changed here, no need: k
 
         if np.random.uniform() < self.p1:  # p_5a
             idx = np.random.randint(0, self.m_clusters)
             solution_new = self.create_solution(self.problem.lb, self.problem.ub)
             self.centers[idx] = solution_new
 
         pop_group = deepcopy(self.pop_group)
         for i in range(0, self.pop_size):  # Generate new individuals
             cluster_id = int(i / self.m_solution)
             location_id = int(i % self.m_solution)
 
             if np.random.uniform() < self.p2:  # p_6b
                 if np.random.uniform() < self.p3:
-                    pos_new = self.centers[cluster_id][self.ID_POS] + epxilon * np.random.normal(0, 1, self.problem.n_dims)
+                    pos_new = self.centers[cluster_id][self.ID_POS] + epsilon * np.random.normal(0, 1, self.problem.n_dims)
                 else:  # 2. Using levy flight here
                     levy_step = self.get_levy_flight_step(beta=1.0, multiplier=0.001, size=self.problem.n_dims, case=-1)
                     pos_new = self.pop_group[cluster_id][location_id][self.ID_POS] + levy_step
             else:
                 id1, id2 = np.random.choice(range(0, self.m_clusters), 2, replace=False)
                 if np.random.uniform() < self.p4:
                     pos_new = 0.5 * (self.centers[id1][self.ID_POS] + self.centers[id2][self.ID_POS]) + \
-                              epxilon * np.random.normal(0, 1, self.problem.n_dims)
+                              epsilon * np.random.normal(0, 1, self.problem.n_dims)
                 else:
                     rand_id1 = np.random.randint(0, self.m_solution)
                     rand_id2 = np.random.randint(0, self.m_solution)
                     pos_new = 0.5 * (self.pop_group[id1][rand_id1][self.ID_POS] + self.pop_group[id2][rand_id2][self.ID_POS]) + \
-                              epxilon * np.random.normal(0, 1, self.problem.n_dims)
+                              epsilon * np.random.normal(0, 1, self.problem.n_dims)
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_group[cluster_id][location_id] = [pos_new, None]
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
                 pop_group[cluster_id][location_id] = self.get_better_solution([pos_new, target], self.pop_group[cluster_id][location_id])
         if self.mode in self.AVAILABLE_MODES:
             for idx in range(0, self.m_clusters):
@@ -215,15 +215,15 @@
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         x = (0.5 * self.epoch - (epoch + 1)) / self.slope
-        epxilon = np.random.uniform() * (1 / (1 + np.exp(-x)))
+        epsilon = np.random.uniform() * (1 / (1 + np.exp(-x)))
 
         if np.random.rand() < self.p1:  # p_5a
             idx = np.random.randint(0, self.m_clusters)
             solution_new = self.create_solution(self.problem.lb, self.problem.ub)
             self.centers[idx] = solution_new
 
         pop_group = deepcopy(self.pop_group)
@@ -231,28 +231,28 @@
             cluster_id = int(i / self.m_solution)
             location_id = int(i % self.m_solution)
 
             if np.random.uniform() < self.p2:  # p_6b
                 if np.random.uniform() < self.p3:  # p_6i
                     cluster_id = np.random.randint(0, self.m_clusters)
                 if np.random.uniform() < self.p3:
-                    pos_new = self.centers[cluster_id][self.ID_POS] + epxilon * np.random.normal(0, 1, self.problem.n_dims)
+                    pos_new = self.centers[cluster_id][self.ID_POS] + epsilon * np.random.normal(0, 1, self.problem.n_dims)
                 else:
                     rand_idx = np.random.randint(0, self.m_solution)
                     pos_new = self.pop_group[cluster_id][rand_idx][self.ID_POS] + np.random.normal(0, 1, self.problem.n_dims)
             else:
                 id1, id2 = np.random.choice(range(0, self.m_clusters), 2, replace=False)
                 if np.random.uniform() < self.p4:
                     pos_new = 0.5 * (self.centers[id1][self.ID_POS] + self.centers[id2][self.ID_POS]) + \
-                              epxilon * np.random.normal(0, 1, self.problem.n_dims)
+                              epsilon * np.random.normal(0, 1, self.problem.n_dims)
                 else:
                     rand_id1 = np.random.randint(0, self.m_solution)
                     rand_id2 = np.random.randint(0, self.m_solution)
                     pos_new = 0.5 * (self.pop_group[id1][rand_id1][self.ID_POS] + self.pop_group[id2][rand_id2][self.ID_POS]) + \
-                              epxilon * np.random.normal(0, 1, self.problem.n_dims)
+                              epsilon * np.random.normal(0, 1, self.problem.n_dims)
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_group[cluster_id][location_id] = [pos_new, None]
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
                 pop_group[cluster_id][location_id] = self.get_better_solution([pos_new, target], self.pop_group[cluster_id][location_id])
         if self.mode in self.AVAILABLE_MODES:
             for idx in range(0, self.m_clusters):
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/CA.py` & `mealpy-2.5.4a3/mealpy/human_based/CA.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,16 @@
 
         # select next generation
         pop_new = []
         pop_full = self.pop + pop_child
         size_new = len(pop_full)
         for _ in range(0, self.pop_size):
             id1, id2 = np.random.choice(list(range(0, size_new)), 2, replace=False)
-            pop_new.append(self.get_better_solution(pop_full[id1], pop_full[id2]))
+            agent = self.get_better_solution(pop_full[id1], pop_full[id2])
+            pop_new.append(agent)
         self.pop = self.get_sorted_strim_population(pop_new)
 
         # Get accepted faithful
         accepted = self.pop[:self.dyn_accepted_num]
 
         # Update belief_space
         self.dyn_belief_space = self.update_belief_space__(self.dyn_belief_space, accepted)
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/CHIO.py` & `mealpy-2.5.4a3/mealpy/human_based/CHIO.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 19:24, 09/05/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalCHIO(Optimizer):
     """
     The original version of: Coronavirus Herd Immunity Optimization (CHIO)
 
@@ -75,15 +74,15 @@
 
         Args:
             epoch (int): The current iteration
         """
         pop_new = []
         is_corona_list = [False, ] * self.pop_size
         for i in range(0, self.pop_size):
-            pos_new = deepcopy(self.pop[i][self.ID_POS])
+            pos_new = self.pop[i][self.ID_POS].copy()
             for j in range(0, self.problem.n_dims):
                 rand = np.random.uniform()
                 if rand < (1.0 / 3) * self.brr:
                     idx_candidates = np.where(self.immunity_type_list == 1)  # Infected list
                     if idx_candidates[0].size == 0:
                         self.finished = True
                         # print("Epoch: {}, i: {}, immunity_list: {}".format(epoch, i, self.immunity_type_list))
@@ -113,15 +112,15 @@
         if len(pop_new) != self.pop_size:
             pop_child = self.create_population(self.pop_size - len(pop_new))
             pop_new = pop_new + pop_child
 
         for idx in range(0, self.pop_size):
             # Step 4: Update herd immunity population
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
             else:
                 self.age_list[idx] += 1
 
             ## Calculate immunity mean of population
             fit_list = np.array([item[self.ID_TAR][self.ID_FIT] for item in self.pop])
             delta_fx = np.mean(fit_list)
             if (self.compare_agent(pop_new[idx], [None, [delta_fx, None]])) and (self.immunity_type_list[idx] == 0) and is_corona_list[idx]:
@@ -185,15 +184,15 @@
 
         Args:
             epoch (int): The current iteration
         """
         pop_new = []
         is_corona_list = [False, ] * self.pop_size
         for i in range(0, self.pop_size):
-            pos_new = deepcopy(self.pop[i][self.ID_POS])
+            pos_new = self.pop[i][self.ID_POS].copy()
             for j in range(0, self.problem.n_dims):
                 rand = np.random.uniform()
                 if rand < (1.0 / 3) * self.brr:
                     idx_candidates = np.where(self.immunity_type_list == 1)  # Infected list
                     if idx_candidates[0].size == 0:
                         rand_choice = np.random.choice(range(0, self.pop_size), int(0.33 * self.pop_size), replace=False)
                         self.immunity_type_list[rand_choice] = 1
@@ -224,15 +223,15 @@
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_new = self.update_target_wrapper_population(pop_new)
 
         for idx in range(0, self.pop_size):
             # Step 4: Update herd immunity population
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
             else:
                 self.age_list[idx] += 1
 
             ## Calculate immunity mean of population
             fit_list = np.array([item[self.ID_TAR][self.ID_FIT] for item in self.pop])
             delta_fx = np.mean(fit_list)
             if (self.compare_agent(pop_new[idx], [None, [delta_fx, None]])) and (self.immunity_type_list[idx] == 0) and is_corona_list[idx]:
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/FBIO.py` & `mealpy-2.5.4a3/mealpy/human_based/FBIO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 08:57, 14/06/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseFBIO(Optimizer):
     """
     The developed : Forensic-Based Investigation Optimization (FBIO)
 
@@ -66,15 +65,15 @@
         # Investigation team - team A
         # Step A1
         pop_new = []
         for idx in range(0, self.pop_size):
             n_change = np.random.randint(0, self.problem.n_dims)
             nb1, nb2 = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 2, replace=False)
             # Eq.(2) in FBI Inspired Meta - Optimization
-            pos_a = deepcopy(self.pop[idx][self.ID_POS])
+            pos_a = self.pop[idx][self.ID_POS].copy()
             pos_a[n_change] = self.pop[idx][self.ID_POS][n_change] + np.random.normal() * \
                 (self.pop[idx][self.ID_POS][n_change] - (self.pop[nb1][self.ID_POS][n_change] + self.pop[nb2][self.ID_POS][n_change]) / 2)
             pos_a = self.amend_position(pos_a, self.problem.lb, self.problem.ub)
             pop_new.append([pos_a, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_a)
                 self.pop[idx] = self.get_better_solution([pos_a, target], self.pop[idx])
@@ -200,15 +199,15 @@
         # Investigation team - team A
         # Step A1
         pop_new = []
         for idx in range(0, self.pop_size):
             n_change = np.random.randint(0, self.problem.n_dims)
             nb1, nb2 = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 2, replace=False)
             # Eq.(2) in FBI Inspired Meta - Optimization
-            pos_a = deepcopy(self.pop[idx][self.ID_POS])
+            pos_a = self.pop[idx][self.ID_POS].copy()
             pos_a[n_change] = self.pop[idx][self.ID_POS][n_change] + (np.random.uniform() - 0.5) * 2 * \
                 (self.pop[idx][self.ID_POS][n_change] - (self.pop[nb1][self.ID_POS][n_change] + self.pop[nb2][self.ID_POS][n_change]) / 2)
             ## Not good move here, change only 1 variable but check bound of all variable in solution
             pos_a = self.amend_position(pos_a, self.problem.lb, self.problem.ub)
             pop_new.append([pos_a, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_a)
@@ -220,15 +219,15 @@
         # Step A2
         list_fitness = np.array([item[self.ID_TAR][self.ID_FIT] for item in self.pop])
         prob = self.probability__(list_fitness)
         pop_child = []
         for idx in range(0, self.pop_size):
             if np.random.uniform() > prob[idx]:
                 r1, r2, r3 = np.random.choice(list(set(range(0, self.pop_size)) - {idx}), 3, replace=False)
-                pos_a = deepcopy(self.pop[idx][self.ID_POS])
+                pos_a = self.pop[idx][self.ID_POS].copy()
                 Rnd = np.floor(np.random.uniform() * self.problem.n_dims) + 1
 
                 for j in range(0, self.problem.n_dims):
                     if (np.random.uniform() < np.random.uniform() or Rnd == j):
                         pos_a[j] = self.g_best[self.ID_POS][j] + self.pop[r1][self.ID_POS][j] + \
                                    np.random.uniform() * (self.pop[r2][self.ID_POS][j] - self.pop[r3][self.ID_POS][j])
                     ## In the original matlab code they do the else condition here, not good again because no need else here
@@ -245,15 +244,15 @@
             pop_child = self.update_target_wrapper_population(pop_child)
             self.pop = self.greedy_selection_population(pop_child, self.pop)
 
         ## Persuing team - team B
         ## Step B1
         pop_new = []
         for idx in range(0, self.pop_size):
-            pos_b = deepcopy(self.pop[idx][self.ID_POS])
+            pos_b = self.pop[idx][self.ID_POS].copy()
             for j in range(0, self.problem.n_dims):
                 ### Eq.(6) in FBI Inspired Meta-Optimization
                 pos_b[j] = np.random.uniform() * self.pop[idx][self.ID_POS][j] + \
                            np.random.uniform() * (self.g_best[self.ID_POS][j] - self.pop[idx][self.ID_POS][j])
             pos_b = self.amend_position(pos_b, self.problem.lb, self.problem.ub)
             pop_new.append([pos_b, None])
             if self.mode not in self.AVAILABLE_MODES:
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/GSKA.py` & `mealpy-2.5.4a3/mealpy/human_based/GSKA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 16:58, 08/04/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseGSKA(Optimizer):
     """
     The developed version: Gaining Sharing Knowledge-based Algorithm (GSKA)
 
@@ -206,15 +205,15 @@
                 previ, nexti = idx - 2, idx - 1
             # Other case it chooses i-1, i+1
             else:
                 previ, nexti = idx - 1, idx + 1
 
             # The random individual is for all dimension values
             rand_idx = np.random.choice(list(set(range(0, self.pop_size)) - {previ, idx, nexti}))
-            pos_new = deepcopy(self.pop[idx][self.ID_POS])
+            pos_new = self.pop[idx][self.ID_POS].copy()
 
             for j in range(0, self.problem.n_dims):
                 if j < D:  # junior gaining and sharing
                     if np.random.uniform() <= self.kr:
                         if self.compare_agent(self.pop[rand_idx], self.pop[idx]):
                             pos_new[j] = self.pop[idx][self.ID_POS][j] + self.kf * \
                                          (self.pop[previ][self.ID_POS][j] - self.pop[nexti][self.ID_POS][j] +
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/HBO.py` & `mealpy-2.5.4a3/mealpy/human_based/HBO.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 00:47, 16/10/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalHBO(Optimizer):
     """
     The original version of: Heap-based optimizer (HBO)
 
@@ -111,15 +110,15 @@
         p2 = p1 + (1 - p1) / 2
         for c in range(self.pop_size-1, 0, -1):
 
             if c == 0: # Dealing with root
                 continue
             else:
                 parent_id = int(np.floor((c+1)/self.degree) - 1)
-                cur_agent = deepcopy(self.pop[self.heap[c][1]])         #Sol to be updated
+                cur_agent = self.pop[self.heap[c][1]].copy()         #Sol to be updated
                 par_agent = self.pop[self.heap[parent_id][1]]           #Sol to be updated with reference to
 
                 # Sol to be updated with reference to
                 if self.friend_limits[c, 0] < self.friend_limits[c, 1]+1:
                     friend_idx = self.friend_limits[c, 0]
                 else:
                     friend_idx = np.random.choice(list(set(range(self.friend_limits[c, 0], self.friend_limits[c, 1])) - {c}))
@@ -142,15 +141,15 @@
                         else:
                             cur_agent[self.ID_POS][jdx] += rn[jdx] * gama * np.abs(fri_agent[self.ID_POS][jdx] - cur_agent[self.ID_POS][jdx])
                 cur_agent[self.ID_POS] = self.amend_position(cur_agent[self.ID_POS], self.problem.lb, self.problem.ub)
                 cur_agent[self.ID_TAR] = self.get_target_wrapper(cur_agent[self.ID_POS])
 
                 if self.compare_agent(cur_agent, [None, self.heap[c][0]]):
                     self.pop[self.heap[c][1]] = cur_agent
-                    self.heap[c][0] = deepcopy(cur_agent[self.ID_TAR])
+                    self.heap[c][0] = cur_agent[self.ID_TAR].copy()
 
             # Heapifying
             t = c
             while t > 1:
                 parent_id = int((t + 1) / self.degree)
                 if self.compare_agent([None, self.heap[parent_id][0]], [None, self.heap[t][0]]):
                     break
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/HCO.py` & `mealpy-2.5.4a3/mealpy/human_based/HCO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 08:57, 12/03/2023 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalHCO(Optimizer):
     """
     The original version of: Human Conception Optimizer (HCO)
 
@@ -92,15 +91,15 @@
             if self.compare_agent([None, [pfit, None]], self.pop[idx]):
                 while True:
                     sol = self.create_solution(self.problem.lb, self.problem.ub)
                     if self.compare_agent(sol, [None, [pfit, None]]):
                         self.pop[idx] = sol
                         break
         self.vec = np.random.rand(self.pop_size, self.problem.n_dims)
-        self.pop_p = deepcopy(self.pop)
+        self.pop_p = self.pop.copy()
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
@@ -127,8 +126,8 @@
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
 
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], self.pop[idx]):
                 self.pop[idx] = pop_new[idx]
                 if self.compare_agent(pop_new[idx], self.pop_p[idx]):
-                    self.pop_p[idx] = deepcopy(pop_new[idx])
+                    self.pop_p[idx] = pop_new[idx].copy()
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/ICA.py` & `mealpy-2.5.4a3/mealpy/human_based/ICA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/human_based/LCO.py` & `mealpy-2.5.4a3/mealpy/human_based/LCO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/human_based/QSA.py` & `mealpy-2.5.4a3/mealpy/human_based/QSA.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 10:21, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseQSA(Optimizer):
     """
     The developed version: Queuing Search Algorithm (QSA)
 
@@ -75,23 +74,23 @@
         t1, t2, t3 = pop[0][self.ID_TAR][self.ID_FIT], pop[1][self.ID_TAR][self.ID_FIT], pop[2][self.ID_TAR][self.ID_FIT]
         q1, q2, q3 = self.calculate_queue_length__(t1, t2, t3)
         case = None
         for i in range(self.pop_size):
             if i < q1:
                 if i == 0:
                     case = 1
-                A = deepcopy(A1)
+                A = A1.copy()
             elif q1 <= i < q1 + q2:
                 if i == q1:
                     case = 1
-                A = deepcopy(A2)
+                A = A2.copy()
             else:
                 if i == q1 + q2:
                     case = 1
-                A = deepcopy(A3)
+                A = A3.copy()
             beta = np.power(current_epoch, np.power(current_epoch / self.epoch, 0.5))
             alpha = np.random.uniform(-1, 1)
             E = np.random.exponential(0.5, self.problem.n_dims)
             F1 = beta * alpha * (E * np.abs(A - pop[i][self.ID_POS])) + np.random.exponential(0.5) * (A - pop[i][self.ID_POS])
             F2 = beta * alpha * (E * np.abs(A - pop[i][self.ID_POS]))
             if case == 1:
                 pos_new = A + F1
@@ -120,19 +119,19 @@
         if t1 > 1.0e-005:
             cv = t1 / (t2 + t3)
         else:
             cv = 1.0 / 2
         pop_new = []
         for i in range(self.pop_size):
             if i < q1:
-                A = deepcopy(A1)
+                A = A1.copy()
             elif q1 <= i < q1 + q2:
-                A = deepcopy(A2)
+                A = A2.copy()
             else:
-                A = deepcopy(A3)
+                A = A3.copy()
             if np.random.random() < pr[i]:
                 i1, i2 = np.random.choice(self.pop_size, 2, replace=False)
                 if np.random.random() < cv:
                     X_new = pop[i][self.ID_POS] + np.random.exponential(0.5) * (pop[i1][self.ID_POS] - pop[i2][self.ID_POS])
                 else:
                     X_new = pop[i][self.ID_POS] + np.random.exponential(0.5) * (A - pop[i1][self.ID_POS])
             else:
@@ -147,15 +146,15 @@
             pop_new = self.greedy_selection_population(pop, pop_new)
         return self.get_sorted_strim_population(pop_new, self.pop_size)
 
     def update_business_3__(self, pop, g_best):
         pr = np.array([i / self.pop_size for i in range(1, self.pop_size + 1)])
         pop_new = []
         for i in range(self.pop_size):
-            X_new = deepcopy(pop[i][self.ID_POS])
+            X_new = pop[i][self.ID_POS].copy()
             id1 = np.random.choice(self.pop_size)
             temp = g_best[self.ID_POS] + np.random.exponential(0.5, self.problem.n_dims) * (pop[id1][self.ID_POS] - pop[i][self.ID_POS])
             X_new = np.where(np.random.random(self.problem.n_dims) > pr[i], temp, X_new)
             pos_new = self.amend_position(X_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
@@ -283,19 +282,19 @@
         if t1 > 1.0e-6:
             cv = t1 / (t2 + t3)
         else:
             cv = 1 / 2
         pop_new = []
         for i in range(self.pop_size):
             if i < q1:
-                A = deepcopy(A1)
+                A = A1.copy()
             elif q1 <= i < q1 + q2:
-                A = deepcopy(A2)
+                A = A2.copy()
             else:
-                A = deepcopy(A3)
+                A = A3.copy()
             if np.random.random() < pr[i]:
                 id1 = np.random.choice(self.pop_size)
                 if np.random.random() < cv:
                     levy_step = self.get_levy_flight_step(beta=1.0, multiplier=0.001, case=-1)
                     X_new = pop[i][self.ID_POS] + np.random.normal(0, 1, self.problem.n_dims) * levy_step
                 else:
                     X_new = pop[i][self.ID_POS] + np.random.exponential(0.5) * (A - pop[id1][self.ID_POS])
@@ -423,15 +422,15 @@
         super().__init__(epoch, pop_size, **kwargs)
         self.sort_flag = True
 
     def update_business_3__(self, pop, g_best):
         pr = [i / self.pop_size for i in range(1, self.pop_size + 1)]
         pop_new = []
         for i in range(self.pop_size):
-            pos_new = deepcopy(pop[i][self.ID_POS])
+            pos_new = pop[i][self.ID_POS].copy()
             for j in range(self.problem.n_dims):
                 if np.random.random() > pr[i]:
                     i1, i2 = np.random.choice(self.pop_size, 2, replace=False)
                     e = np.random.exponential(0.5)
                     X1 = pop[i1][self.ID_POS]
                     X2 = pop[i2][self.ID_POS]
                     pos_new[j] = X1[j] + e * (X2[j] - pop[i][self.ID_POS][j])
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/SARO.py` & `mealpy-2.5.4a3/mealpy/human_based/SARO.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 11:16, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseSARO(Optimizer):
     """
     The developed version: Search And Rescue Optimization (SARO)
 
@@ -74,16 +73,16 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        pop_x = deepcopy(self.pop[:self.pop_size])
-        pop_m = deepcopy(self.pop[self.pop_size:])
+        pop_x = self.pop[:self.pop_size].copy()
+        pop_m = self.pop[self.pop_size:].copy()
 
         pop_new = []
         for idx in range(self.pop_size):
             ## Social Phase
             k = np.random.choice(list(set(range(0, 2 * self.pop_size)) - {idx}))
             sd = pop_x[idx][self.ID_POS] - self.pop[k][self.ID_POS]
 
@@ -95,36 +94,36 @@
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_new = self.update_target_wrapper_population(pop_new)
         for idx in range(self.pop_size):
             if self.compare_agent(pop_new[idx], pop_x[idx]):
-                pop_m[np.random.randint(0, self.pop_size)] = deepcopy(pop_x[idx])
-                pop_x[idx] = deepcopy(pop_new[idx])
+                pop_m[np.random.randint(0, self.pop_size)] = pop_x[idx].copy()
+                pop_x[idx] = pop_new[idx].copy()
                 self.dyn_USN[idx] = 0
             else:
                 self.dyn_USN[idx] += 1
 
-        pop = deepcopy(pop_x) + deepcopy(pop_m)
+        pop = pop_x.copy() + pop_m.copy()
         pop_new = []
         for idx in range(self.pop_size):
             ## Individual phase
             k1, k2 = np.random.choice(list(set(range(0, 2 * self.pop_size)) - {idx}), 2, replace=False)
             #### Remove third loop here, and flight back strategy now be a random
             pos_new = self.g_best[self.ID_POS] + np.random.uniform() * (pop[k1][self.ID_POS] - pop[k2][self.ID_POS])
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_new = self.update_target_wrapper_population(pop_new)
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], pop_x[idx]):
-                pop_m[np.random.randint(0, self.pop_size)] = deepcopy(pop_x[idx])
-                pop_x[idx] = deepcopy(pop_new[idx])
+                pop_m[np.random.randint(0, self.pop_size)] = pop_x[idx].copy()
+                pop_x[idx] = pop_new[idx].copy()
                 self.dyn_USN[idx] = 0
             else:
                 self.dyn_USN[idx] += 1
 
             if self.dyn_USN[idx] > self.mu:
                 pop_x[idx] = self.create_solution(self.problem.lb, self.problem.ub)
                 self.dyn_USN[idx] = 0
@@ -184,26 +183,26 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        pop_x = deepcopy(self.pop[:self.pop_size])
-        pop_m = deepcopy(self.pop[self.pop_size:])
+        pop_x = self.pop[:self.pop_size].copy()
+        pop_m = self.pop[self.pop_size:].copy()
 
         pop_new = []
         for idx in range(self.pop_size):
             ## Social Phase
             k = np.random.choice(list(set(range(0, 2 * self.pop_size)) - {idx}))
             sd = pop_x[idx][self.ID_POS] - self.pop[k][self.ID_POS]
             j_rand = np.random.randint(0, self.problem.n_dims)
             r1 = np.random.uniform(-1, 1)
 
-            pos_new = deepcopy(pop_x[idx][self.ID_POS])
+            pos_new = pop_x[idx][self.ID_POS].copy()
             for j in range(0, self.problem.n_dims):
                 if np.random.uniform() < self.se or j == j_rand:
                     if self.compare_agent(self.pop[k], pop_x[idx]):
                         pos_new[j] = self.pop[k][self.ID_POS][j] + r1 * sd[j]
                     else:
                         pos_new[j] = pop_x[idx][self.ID_POS][j] + r1 * sd[j]
                 if pos_new[j] < self.problem.lb[j]:
@@ -213,22 +212,22 @@
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_new = self.update_target_wrapper_population(pop_new)
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], pop_x[idx]):
-                pop_m[np.random.randint(0, self.pop_size)] = deepcopy(pop_x[idx])
-                pop_x[idx] = deepcopy(pop_new[idx])
+                pop_m[np.random.randint(0, self.pop_size)] = pop_x[idx].copy()
+                pop_x[idx] = pop_new[idx].copy()
                 self.dyn_USN[idx] = 0
             else:
                 self.dyn_USN[idx] += 1
 
         ## Individual phase
-        pop = deepcopy(pop_x) + deepcopy(pop_m)
+        pop = pop_x.copy() + pop_m.copy()
         pop_new = []
         for idx in range(0, self.pop_size):
             k, m = np.random.choice(list(set(range(0, 2 * self.pop_size)) - {idx}), 2, replace=False)
             pos_new = pop_x[idx][self.ID_POS] + np.random.uniform() * (pop[k][self.ID_POS] - pop[m][self.ID_POS])
             for j in range(0, self.problem.n_dims):
                 if pos_new[j] < self.problem.lb[j]:
                     pos_new[j] = (pop_x[idx][self.ID_POS][j] + self.problem.lb[j]) / 2
@@ -238,15 +237,15 @@
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_new = self.update_target_wrapper_population(pop_new)
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], pop_x[idx]):
                 pop_m[np.random.randint(0, self.pop_size)] = pop_x[idx]
-                pop_x[idx] = deepcopy(pop_new[idx])
+                pop_x[idx] = pop_new[idx].copy()
                 self.dyn_USN[idx] = 0
             else:
                 self.dyn_USN[idx] += 1
 
             if self.dyn_USN[idx] > self.mu:
                 pop_x[idx] = self.create_solution(self.problem.lb, self.problem.ub)
                 self.dyn_USN[idx] = 0
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/SPBO.py` & `mealpy-2.5.4a3/mealpy/human_based/SPBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/human_based/SSDO.py` & `mealpy-2.5.4a3/mealpy/human_based/SSDO.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 11:17, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalSSDO(Optimizer):
     """
     The original version of: Social Ski-Driver Optimization (SSDO)
 
@@ -67,15 +66,15 @@
             list: wrapper of solution with format [position, target, velocity, best_local_position]
         """
         if pos is None:
             pos = self.generate_position(lb, ub)
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         velocity = np.random.uniform(lb, ub)
-        pos_local = deepcopy(position)
+        pos_local = position.copy()
         return [position, target, velocity, pos_local]
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
@@ -83,15 +82,15 @@
         """
         c = 2 - epoch * (2.0 / self.epoch)  # a decreases linearly from 2 to 0
 
         ## Calculate the mean of the best three solutions in each dimension. Eq 9
         _, pop_best3, _ = self.get_special_solutions(self.pop, best=3)
         pos_mean = np.mean(np.array([item[self.ID_POS] for item in pop_best3]))
 
-        pop_new = deepcopy(self.pop)
+        pop_new = self.pop.copy()
         # Updating velocity vectors
         r1 = np.random.uniform()  # r1, r2 is a random number in [0,1]
         r2 = np.random.uniform()
         for i in range(0, self.pop_size):
             if r2 <= 0.5:  ## Use Sine function to move
                 vel_new = c * np.sin(r1) * (self.pop[i][self.ID_LOC] - self.pop[i][self.ID_POS]) + (2-c)*np.sin(r1) * (pos_mean - self.pop[i][self.ID_POS])
             else:  ## Use Cosine function to move
@@ -101,13 +100,13 @@
         ## Reproduction
         for idx in range(0, self.pop_size):
             pos_new = np.random.normal(0, 1, self.problem.n_dims) * pop_new[idx][self.ID_POS] + np.random.rand() * pop_new[idx][self.ID_VEL]
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new[idx][self.ID_LOC] = self.pop[idx][self.ID_POS]
             pop_new[idx][self.ID_POS] = pos_new
             if self.mode not in self.AVAILABLE_MODES:
-                old = deepcopy(pop_new[idx])
+                old = pop_new[idx].copy()
                 old[self.ID_TAR] = self.get_target_wrapper(pos_new)
                 self.pop[idx] = self.get_better_solution(pop_new[idx], old)
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop = self.greedy_selection_population(self.pop, pop_new)
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/TLO.py` & `mealpy-2.5.4a3/mealpy/human_based/TLO.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Created by "Thieu" at 10:14, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
 from functools import reduce
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseTLO(Optimizer):
     """
     The developed version: Teaching Learning-based Optimization (TLO)
 
@@ -83,15 +82,15 @@
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop = self.greedy_selection_population(self.pop, pop_new)
 
         pop_child = []
         for idx in range(0, self.pop_size):
             ## Learning Phrase
-            temp = deepcopy(self.pop[idx][self.ID_POS]).astype(float)
+            temp = self.pop[idx][self.ID_POS].copy().astype(float)
             id_partner = np.random.choice(np.setxor1d(np.array(range(self.pop_size)), np.array([idx])))
             if self.compare_agent(self.pop[idx], self.pop[id_partner]):
                 temp += np.random.rand(self.problem.n_dims) * (self.pop[idx][self.ID_POS] - self.pop[id_partner][self.ID_POS])
             else:
                 temp += np.random.rand(self.problem.n_dims) * (self.pop[id_partner][self.ID_POS] - self.pop[idx][self.ID_POS])
             pos_new = self.amend_position(temp, self.problem.lb, self.problem.ub)
             pop_child.append([pos_new, None])
@@ -239,15 +238,15 @@
         self.n_students_in_team = int(self.n_students / self.n_teachers)
         self.sort_flag = False
 
     def initialization(self):
         if self.pop is None:
             self.pop = self.create_population(self.pop_size)
         sorted_pop, self.g_best = self.get_global_best_solution(self.pop)
-        self.teachers = deepcopy(sorted_pop[:self.n_teachers])
+        self.teachers = sorted_pop[:self.n_teachers].copy()
         sorted_pop = sorted_pop[self.n_teachers:]
         idx_list = np.random.permutation(range(0, self.n_students))
         self.teams = []
         for id_teacher in range(0, self.n_teachers):
             group = []
             for idx in range(0, self.n_students_in_team):
                 start_index = id_teacher * self.n_students_in_team + idx
@@ -311,9 +310,8 @@
             self.teams[id_teach] = pop_new
 
         for id_teach, teacher in enumerate(self.teachers):
             team = self.teams[id_teach] + [teacher]
             team, local_best = self.get_global_best_solution(team)
             self.teachers[id_teach] = local_best
             self.teams[id_teach] = team[1:]
-
         self.pop = self.teachers + reduce(lambda x, y: x + y, self.teams)
```

### Comparing `mealpy-2.5.4a2/mealpy/human_based/TOA.py` & `mealpy-2.5.4a3/mealpy/human_based/TOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/human_based/WarSO.py` & `mealpy-2.5.4a3/mealpy/human_based/WarSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/math_based/AOA.py` & `mealpy-2.5.4a3/mealpy/math_based/AOA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 09:56, 07/07/2021 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalAOA(Optimizer):
     """
     The original version of: Arithmetic Optimization Algorithm (AOA)
 
@@ -81,15 +80,15 @@
             epoch (int): The current iteration
         """
         moa = self.moa_min + (epoch+1) * ((self.moa_max - self.moa_min) / self.epoch)  # Eq. 2
         mop = 1 - ((epoch+1) ** (1.0 / self.alpha)) / (self.epoch ** (1.0 / self.alpha))  # Eq. 4
 
         pop_new = []
         for idx in range(0, self.pop_size):
-            pos_new = deepcopy(self.pop[idx][self.ID_POS])
+            pos_new = self.pop[idx][self.ID_POS].copy()
             for j in range(0, self.problem.n_dims):
                 r1, r2, r3 = np.random.rand(3)
                 if r1 > moa:  # Exploration phase
                     if r2 < 0.5:
                         pos_new[j] = self.g_best[self.ID_POS][j] / (mop + self.EPSILON) * \
                                      ((self.problem.ub[j] - self.problem.lb[j]) * self.miu + self.problem.lb[j])
                     else:
```

### Comparing `mealpy-2.5.4a2/mealpy/math_based/CEM.py` & `mealpy-2.5.4a3/mealpy/math_based/CEM.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/math_based/CGO.py` & `mealpy-2.5.4a3/mealpy/math_based/CGO.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 22:24, 02/03/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalCGO(Optimizer):
     """
     The original version of: Chaos Game Optimization (CGO)
 
@@ -87,15 +86,15 @@
             ## In the text said, multiple variables, but the defination of k is 1 variable. So confused
             k = np.random.randint(0, self.problem.n_dims)
             k_idx = np.random.choice(range(0, self.problem.n_dims), k, replace=False)
 
             seed1 = self.pop[idx][self.ID_POS] + alpha1 * (beta[0] * self.g_best[self.ID_POS] - gama[0] * MG)  # Eq. 3
             seed2 = self.g_best[self.ID_POS] + alpha2 * (beta[1] * self.pop[idx][self.ID_POS] - gama[1] * MG)  # Eq. 4
             seed3 = MG + alpha3 * (beta[2] * self.pop[idx][self.ID_POS] - gama[2] * self.g_best[self.ID_POS])  # Eq. 5
-            seed4 = deepcopy(self.pop[idx][self.ID_POS]).astype(float)
+            seed4 = self.pop[idx][self.ID_POS].copy().astype(float)
             seed4[k_idx] += np.random.uniform(0, 1, k)
 
             # Check if solutions go outside the search space and bring them back
             seed1 = self.amend_position(seed1, self.problem.lb, self.problem.ub)
             seed2 = self.amend_position(seed2, self.problem.lb, self.problem.ub)
             seed3 = self.amend_position(seed3, self.problem.lb, self.problem.ub)
             seed4 = self.amend_position(seed4, self.problem.lb, self.problem.ub)
```

### Comparing `mealpy-2.5.4a2/mealpy/math_based/CircleSA.py` & `mealpy-2.5.4a3/mealpy/math_based/CircleSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/math_based/GBO.py` & `mealpy-2.5.4a3/mealpy/math_based/GBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/math_based/HC.py` & `mealpy-2.5.4a3/mealpy/math_based/HC.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/math_based/INFO.py` & `mealpy-2.5.4a3/mealpy/math_based/INFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/math_based/PSS.py` & `mealpy-2.5.4a3/mealpy/math_based/PSS.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Created by "Thieu" at 19:38, 10/03/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from scipy.stats import qmc
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalPSS(Optimizer):
     """
     The original version of: Pareto-like Sequential Sampling (PSS)
 
@@ -98,15 +97,15 @@
 
         Args:
             epoch (int): The current iteration
         """
         pop_new = []
         pop_rand = self.create_population(self.pop_size)
         for idx in range(0, self.pop_size):
-            pos_new = deepcopy(self.pop[idx][self.ID_POS]).astype(float)
+            pos_new = self.pop[idx][self.ID_POS].copy().astype(float)
             for k in range(self.problem.n_dims):
                 # Update the ranges
                 deviation = np.random.uniform(0, self.g_best[self.ID_POS][k])
                 if self.new_solution:
                     # The deviation is positive dynamic real number
                     deviation = abs(0.5 * (1. - self.acceptance_rate) * (self.problem.ub[k] - self.problem.lb[k])) * (1 - ((epoch+1) / self.epoch))
```

### Comparing `mealpy-2.5.4a2/mealpy/math_based/RUN.py` & `mealpy-2.5.4a3/mealpy/math_based/RUN.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/math_based/SCA.py` & `mealpy-2.5.4a3/mealpy/math_based/SCA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 17:44, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseSCA(Optimizer):
     """
     The developed version: Sine Cosine Algorithm (SCA)
 
@@ -136,15 +135,15 @@
             epoch (int): The current iteration
         """
         pop_new = []
         for idx in range(0, self.pop_size):
             # Eq 3.4, r1 decreases linearly from a to 0
             a = 2.0
             r1 = a - (epoch + 1) * (a / self.epoch)
-            pos_new = deepcopy(self.pop[idx][self.ID_POS])
+            pos_new = self.pop[idx][self.ID_POS].copy()
             for j in range(self.problem.n_dims):  # j-th dimension
                 # Update r2, r3, and r4 for Eq. (3.3)
                 r2 = 2 * np.pi * np.random.uniform()
                 r3 = 2 * np.random.uniform()
                 r4 = np.random.uniform()
                 # Eq. 3.3, 3.1 and 3.2
                 if r4 < 0.5:
@@ -288,15 +287,15 @@
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         for idx in range(0, self.pop_size):
-            agent = deepcopy(self.pop[idx])
+            agent = self.pop[idx].copy()
             ## Step 3: State computation
             den = self.density__(self.pop)
             dis = self.distance__(self.g_best, self.pop, self.problem.lb, self.problem.ub)
             ## Step 4: Action execution
             state = self.pop[idx][self.ID_QTB].get_state(density=den, distance=dis)
             action = self.pop[idx][self.ID_QTB].get_action(state=state)
             r1_bound, r3_bound = self.pop[idx][self.ID_QTB].get_action_params(action)
```

### Comparing `mealpy-2.5.4a2/mealpy/math_based/SHIO.py` & `mealpy-2.5.4a3/mealpy/math_based/SHIO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/multitask.py` & `mealpy-2.5.4a3/mealpy/multitask.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/music_based/HS.py` & `mealpy-2.5.4a3/mealpy/music_based/HS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/optimizer.py` & `mealpy-2.5.4a3/mealpy/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -622,15 +622,15 @@
             case (int): Should be one of these value [0, 1, -1].
 
                 * 0: return multiplier * s * np.random.uniform()
                 * 1: return multiplier * s * np.random.normal(0, 1)
                 * -1: return multiplier * s
 
         Returns:
-            int: The step size of Levy-flight trajectory
+            float, list, np.ndarray: The step size of Levy-flight trajectory
         """
         # u and v are two random variables which follow np.random.normal distribution
         # sigma_u : standard deviation of u
         sigma_u = np.power(gamma(1 + beta) * np.sin(np.pi * beta / 2) / (gamma((1 + beta) / 2) * beta * np.power(2, (beta - 1) / 2)), 1 / beta)
         # sigma_v : standard deviation of v
         sigma_v = 1
         size = 1 if size is None else size
```

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/ASO.py` & `mealpy-2.5.4a3/mealpy/physics_based/ASO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 07:03, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalASO(Optimizer):
     """
     The original version of: Atom Search Optimization (ASO)
 
@@ -113,21 +112,20 @@
                 rs = radius / average_dist
         potential = c * (12 * (-rs) ** (-13) - 6 * (-rs) ** (-7))
         return potential
 
     def acceleration__(self, population, g_best, iteration):
         eps = 2 ** (-52)
         pop = self.update_mass__(population)
-
         G = np.exp(-20.0 * (iteration + 1) / self.epoch)
         k_best = int(self.pop_size - (self.pop_size - 2) * ((iteration + 1) / self.epoch) ** 0.5) + 1
         if self.problem.minmax == "min":
-            k_best_pop = deepcopy(sorted(pop, key=lambda agent: agent[self.ID_MAS], reverse=True)[:k_best])
+            k_best_pop = sorted(pop, key=lambda agent: agent[self.ID_MAS], reverse=True)[:k_best].copy()
         else:
-            k_best_pop = deepcopy(sorted(pop, key=lambda agent: agent[self.ID_MAS])[:k_best])
+            k_best_pop = sorted(pop, key=lambda agent: agent[self.ID_MAS])[:k_best].copy()
         mk_average = np.mean([item[self.ID_POS] for item in k_best_pop])
 
         acc_list = np.zeros((self.pop_size, self.problem.n_dims))
         for i in range(0, self.pop_size):
             dist_average = np.linalg.norm(pop[i][self.ID_POS] - mk_average)
             temp = np.zeros((self.problem.n_dims))
 
@@ -151,15 +149,15 @@
         """
         # Calculate acceleration.
         atom_acc_list = self.acceleration__(self.pop, self.g_best, iteration=epoch)
 
         # Update velocity based on random dimensions and position of global best
         pop_new = []
         for idx in range(0, self.pop_size):
-            agent = deepcopy(self.pop[idx])
+            agent = self.pop[idx].copy()
             velocity = np.random.random(self.problem.n_dims) * self.pop[idx][self.ID_VEL] + atom_acc_list[idx]
             # print(velocity)
             pos_new = self.pop[idx][self.ID_POS] + velocity
             # Relocate atom out of range
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             # print(pos_new)
             agent[self.ID_POS] = pos_new
@@ -169,8 +167,8 @@
                 agent[self.ID_TAR] = target
                 self.pop[idx] = self.get_better_solution(agent, self.pop[idx])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop = self.greedy_selection_population(self.pop, pop_new)
         _, current_best = self.get_global_best_solution(pop_new)
         if self.compare_agent(self.g_best, current_best):
-            self.pop[np.random.randint(0, self.pop_size)] = deepcopy(self.g_best)
+            self.pop[np.random.randint(0, self.pop_size)] = self.g_best.copy()
```

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/ArchOA.py` & `mealpy-2.5.4a3/mealpy/physics_based/ArchOA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 16:10, 08/07/2021 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalArchOA(Optimizer):
     """
     The original version of: Archimedes Optimization Algorithm (ArchOA)
 
@@ -135,15 +134,15 @@
         max_acc = np.max(list_acc)
         ## Normalize acceleration using Eq. 12
         for i in range(0, self.pop_size):
             self.pop[i][self.ID_ACC] = self.acc_max * (list_acc[i] - min_acc) / (max_acc - min_acc) + self.acc_min
 
         pop_new = []
         for idx in range(0, self.pop_size):
-            solution = deepcopy(self.pop[idx])
+            solution = self.pop[idx].copy()
             if tf <= 0.5:  # update position using Eq. 13
                 id_rand = np.random.choice(list(set(range(0, self.pop_size)) - {idx}))
                 pos_new = self.pop[idx][self.ID_POS] + self.c1 * np.random.uniform() * \
                           self.pop[idx][self.ID_ACC] * ddf * (self.pop[id_rand][self.ID_POS] - self.pop[idx][self.ID_POS])
             else:
                 p = 2 * np.random.rand() - self.c4
                 f = 1 if p <= 0.5 else -1
```

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/CDO.py` & `mealpy-2.5.4a3/mealpy/physics_based/CDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/EFO.py` & `mealpy-2.5.4a3/mealpy/physics_based/EFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/EO.py` & `mealpy-2.5.4a3/mealpy/physics_based/EO.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 07:03, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalEO(Optimizer):
     """
     The original version of: Equilibrium Optimizer (EO)
 
@@ -182,15 +181,15 @@
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop = self.greedy_selection_population(self.pop, pop_new)
 
         ## Sort the updated population based on fitness
         _, pop_s1, _ = self.get_special_solutions(self.pop, best=self.pop_len)
 
         ## Mutation scheme
-        pop_s2 = deepcopy(pop_s1)
+        pop_s2 = pop_s1.copy()
         pop_s2_new = []
         for i in range(0, self.pop_len):
             pos_new = pop_s2[i][self.ID_POS] * (1 + np.random.normal(0, 1, self.problem.n_dims))  # Eq. 12
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_s2_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
@@ -207,15 +206,14 @@
             pos_new = (c_pool[0][self.ID_POS] - pos_s1_mean) - np.random.random() * \
                       (self.problem.lb + np.random.random() * (self.problem.ub - self.problem.lb))
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_s3.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 pop_s3[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_s3 = self.update_target_wrapper_population(pop_s3)
-
         ## Construct a new population
         self.pop = pop_s1 + pop_s2 + pop_s3
         n_left = self.pop_size - len(self.pop)
         idx_selected = np.random.choice(range(0, len(c_pool)), n_left, replace=False)
         for i in range(0, n_left):
             self.pop.append(c_pool[idx_selected[i]])
 
@@ -271,34 +269,29 @@
 
         Args:
             epoch (int): The current iteration
         """
         # ---------------- Memory saving-------------------  make equilibrium pool
         _, c_eq_list, _ = self.get_special_solutions(self.pop, best=4)
         c_pool = self.make_equilibrium_pool__(c_eq_list)
-
         # Eq. 9
         t = (1 - epoch / self.epoch) ** (self.a2 * epoch / self.epoch)
-
         ## Memory saving, Eq 20, 21
         t = (1 - epoch / self.epoch) ** (self.a2 * epoch / self.epoch)
-
         pop_new = []
         for idx in range(0, self.pop_size):
             lamda = np.random.uniform(0, 1, self.problem.n_dims)
             r = np.random.uniform(0, 1, self.problem.n_dims)
             c_eq = c_pool[np.random.randint(0, len(c_pool))][self.ID_POS]  # random selection 1 of candidate from the pool
             f = self.a1 * np.sign(r - 0.5) * (np.exp(-lamda * t) - 1.0)  # Eq. 14
-
             r1 = np.random.uniform()
             r2 = np.random.uniform()
             gcp = 0.5 * r1 * np.ones(self.problem.n_dims) * (r2 >= self.GP)
             g0 = gcp * (c_eq - lamda * self.pop[idx][self.ID_POS])
             g = g0 * f
-
             fit_average = np.mean([item[self.ID_TAR][self.ID_FIT] for item in self.pop])  # Eq. 19
             pos_new = c_eq + (self.pop[idx][self.ID_POS] - c_eq) * f + (g * self.V / lamda) * (1.0 - f)  # Eq. 9
             if self.pop[idx][self.ID_TAR][self.ID_FIT] >= fit_average:
                 pos_new = np.multiply(pos_new, (0.5 + np.random.uniform(0, 1, self.problem.n_dims)))
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
```

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/EVO.py` & `mealpy-2.5.4a3/mealpy/physics_based/EVO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/FLA.py` & `mealpy-2.5.4a3/mealpy/physics_based/FLA.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 21:00, 14/03/2023 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalFLA(Optimizer):
     """
     The original version of: Fick's Law Algorithm (FLA)
 
@@ -84,16 +83,16 @@
         self.set_parameters(["epoch", "pop_size", "C1", "C2", "C3", "C4", "C5", "DD"])
         self.sort_flag = False
 
     def before_main_loop(self):
         self.xss, self.g_best = self.get_global_best_solution(self.pop)
         self.n1 = int(np.round(self.pop_size/2))
         self.n2 = self.pop_size - self.n1
-        self.pop1 = deepcopy(self.pop[:self.n1])
-        self.pop2 = deepcopy(self.pop[self.n1:])
+        self.pop1 = self.pop[:self.n1].copy()
+        self.pop2 = self.pop[self.n1:].copy()
         _, self.best1 = self.get_global_best_solution(self.pop1)
         _, self.best2 = self.get_global_best_solution(self.pop2)
         if self.compare_agent(self.best1, self.best2):
             self.fsss = self.best1[self.ID_TAR][self.ID_FIT]
         else:
             self.fsss = self.best2[self.ID_TAR][self.ID_FIT]
 
@@ -118,100 +117,110 @@
             if tdo < np.random.rand():
                 m1n, m2n = self.C3*self.n1, self.C4*self.n1
                 nt12 = int(np.round((m2n - m1n)*np.random.rand() + m1n))
                 for idx in range(0, nt12):
                     dfg = np.random.randint(1, 3)
                     jj = -self.DD * (xm2 - xm1) / np.linalg.norm(self.best2[self.ID_POS] - self.pop1[idx][self.ID_POS] + self.EPSILON)
                     pos_new = self.best2[self.ID_POS] + dfg*dof*np.random.rand(self.problem.n_dims)*(jj*self.best2[self.ID_POS] - self.pop1[idx][self.ID_POS])
-                    pop_new.append([self.amend_position(pos_new, self.problem.lb, self.problem.ub), None])
+                    pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                    pop_new.append([pos_new, None])
                 for idx in range(nt12, self.n1):
                     tt = self.pop1[idx][self.ID_POS] + dof * (np.random.rand(self.problem.n_dims) * (self.problem.ub - self.problem.lb) + self.problem.lb)
                     pp = np.random.rand(self.problem.n_dims)
                     pos_new = np.where(pp < 0.8, self.best1[self.ID_POS], np.where(pp >=0.9, self.pop1[idx][self.ID_POS], tt))
-                    pop_new.append([self.amend_position(pos_new, self.problem.lb, self.problem.ub), None])
+                    pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                    pop_new.append([pos_new, None])
                 for idx in range(0, self.n2):
                     pos_new = self.best2[self.ID_POS] + dof * (np.random.rand(self.problem.n_dims) * (self.problem.ub - self.problem.lb) + self.problem.lb)
-                    pop_new.append([self.amend_position(pos_new, self.problem.lb, self.problem.ub), None])
+                    pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                    pop_new.append([pos_new, None])
             else:
                 m1n, m2n = 0.1 * self.n2, 0.2 * self.n2
                 nt12 = int(np.round((m2n - m1n) * np.random.rand() + m1n))
                 for idx in range(0, nt12):
                     dfg = np.random.randint(1, 3)
                     jj = -self.DD*(xm1-xm2) / np.linalg.norm(self.best1[self.ID_POS] - self.pop2[idx][self.ID_POS] + self.EPSILON)
                     pos_new = self.best1[self.ID_POS] + dfg * dof * np.random.rand(self.problem.n_dims) * (jj * self.best1[self.ID_POS] - self.pop2[idx][self.ID_POS])
-                    pop_new.append([self.amend_position(pos_new, self.problem.lb, self.problem.ub), None])
+                    pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                    pop_new.append([pos_new, None])
                 for idx in range(nt12, self.n2):
                     tt = self.pop2[idx][self.ID_POS] + dof * (np.random.rand(self.problem.n_dims) * (self.problem.ub - self.problem.lb) + self.problem.lb)
                     pp = np.random.rand(self.problem.n_dims)
                     pos_new = np.where(pp < 0.8, self.best2[self.ID_POS], np.where(pp >= 0.9, self.pop2[idx][self.ID_POS], tt))
-                    pop_new.append([self.amend_position(pos_new, self.problem.lb, self.problem.ub), None])
+                    pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                    pop_new.append([pos_new, None])
                 for idx in range(0, self.n1):
                     pos_new = self.best1[self.ID_POS] + dof * (np.random.rand(self.problem.n_dims) * (self.problem.ub - self.problem.lb) + self.problem.lb)
-                    pop_new.append([self.amend_position(pos_new, self.problem.lb, self.problem.ub), None])
+                    pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                    pop_new.append([pos_new, None])
         else:       # Equilibrium operator (EO)
             if tf <= 1:
                 for idx in range(0, self.n1):
                     dfg = np.random.randint(1, 3)
                     tttt = np.linalg.norm(self.best1[self.ID_POS] - self.pop1[idx][self.ID_POS])
                     if tttt == 0:
                         jj = 0
                     else:
                         jj = -self.DD*(self.best1[self.ID_POS] - xm1) / tttt
                     drf = np.exp(-jj / tf)
                     ms = np.exp(-self.best1[self.ID_TAR][self.ID_FIT] / self.pop1[idx][self.ID_TAR][self.ID_FIT] + self.EPSILON)
                     qeo = dfg * drf * np.random.rand(self.problem.n_dims)
                     pos_new = self.best1[self.ID_POS] + qeo*self.pop1[idx][self.ID_POS] + qeo *(ms * self.best1[self.ID_POS] - self.pop1[idx][self.ID_POS])
-                    pop_new.append([self.amend_position(pos_new, self.problem.lb, self.problem.ub), None])
+                    pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                    pop_new.append([pos_new, None])
                 for idx in range(0, self.n2):
                     dfg = np.random.randint(1, 3)
                     tttt = np.linalg.norm(self.best2[self.ID_POS] - self.pop2[idx][self.ID_POS])
                     if tttt == 0:
                         jj = 0
                     else:
                         jj = -self.DD * (self.best2[self.ID_POS] - xm2) / tttt
                     drf = np.exp(-jj / tf)
                     ms = np.exp(-self.best2[self.ID_TAR][self.ID_FIT] / self.pop2[idx][self.ID_TAR][self.ID_FIT] + self.EPSILON)
                     qeo = dfg * drf * np.random.rand(self.problem.n_dims)
                     pos_new = self.best2[self.ID_POS] + qeo * self.pop2[idx][self.ID_POS] + qeo * (ms * self.best2[self.ID_POS] - self.pop2[idx][self.ID_POS])
-                    pop_new.append([self.amend_position(pos_new, self.problem.lb, self.problem.ub), None])
+                    pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                    pop_new.append([pos_new, None])
             else:   # Steady state operator (SSO)
                 for idx in range(0, self.n1):
                     dfg = np.random.randint(1, 3)
                     tttt = np.linalg.norm(self.g_best[self.ID_POS] - self.pop1[idx][self.ID_POS])
                     if tttt == 0:
                         jj = 0
                     else:
                         jj = -self.DD * (xm - xm1) / tttt
                     drf = np.exp(-jj / tf)
                     ms = np.exp(-self.fsss / self.pop1[idx][self.ID_TAR][self.ID_FIT] + self.EPSILON)
                     qg = dfg * drf * np.random.rand(self.problem.n_dims)
                     pos_new = self.g_best[self.ID_POS] + qg * self.pop1[idx][self.ID_POS] + qg * (ms * self.best1[self.ID_POS] - self.pop1[idx][self.ID_POS])
-                    pop_new.append([self.amend_position(pos_new, self.problem.lb, self.problem.ub), None])
+                    pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                    pop_new.append([pos_new, None])
                 for idx in range(0, self.n2):
                     dfg = np.random.randint(1, 3)
                     tttt = np.linalg.norm(self.g_best[self.ID_POS] - self.pop2[idx][self.ID_POS])
                     if tttt == 0:
                         jj = 0
                     else:
                         jj = -self.DD * (xm - xm2) / tttt
                     drf = np.exp(-jj / tf)
                     ms = np.exp(-self.fsss / self.pop2[idx][self.ID_TAR][self.ID_FIT] + self.EPSILON)
                     qg = dfg * drf * np.random.rand(self.problem.n_dims)
                     pos_new = self.g_best[self.ID_POS] + qg * self.pop2[idx][self.ID_POS] + qg * (ms * self.g_best[self.ID_POS] - self.pop2[idx][self.ID_POS])
-                    pop_new.append([self.amend_position(pos_new, self.problem.lb, self.problem.ub), None])
+                    pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
+                    pop_new.append([pos_new, None])
 
         if self.mode not in self.AVAILABLE_MODES:
             for idx in range(0, self.pop_size):
                 pop_new[idx][self.ID_TAR] = self.get_target_wrapper(pop_new[idx][self.ID_POS])
         else:
             pop_new = self.update_target_wrapper_population(pop_new)
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], self.pop[idx]):
                 self.pop[idx] = pop_new[idx]
-        self.pop1 = deepcopy(self.pop[:self.n1])
-        self.pop2 = deepcopy(self.pop[self.n1:])
+        self.pop1 = self.pop[:self.n1].copy()
+        self.pop2 = self.pop[self.n1:].copy()
         _, self.best1 = self.get_global_best_solution(self.pop1)
         _, self.best2 = self.get_global_best_solution(self.pop2)
         if self.compare_agent(self.best1, self.best2):
             self.fsss = self.best1[self.ID_TAR][self.ID_FIT]
         else:
             self.fsss = self.best2[self.ID_TAR][self.ID_FIT]
```

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/HGSO.py` & `mealpy-2.5.4a3/mealpy/physics_based/HGSO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 07:03, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalHGSO(Optimizer):
     """
     The original version of: Henry Gas Solubility Optimization (HGSO)
 
@@ -61,15 +60,15 @@
         self.set_parameters(["epoch", "pop_size", "n_clusters"])
         self.n_elements = int(self.pop_size / self.n_clusters)
         self.sort_flag = False
         self.T0 = 298.15
         self.K = 1.0
         self.beta = 1.0
         self.alpha = 1
-        self.epxilon = 0.05
+        self.epsilon = 0.05
         self.l1 = 5E-2
         self.l2 = 100.0
         self.l3 = 1E-2
 
     def initialize_variables(self):
         self.H_j = self.l1 * np.random.uniform()
         self.P_ij = self.l2 * np.random.uniform()
@@ -108,16 +107,16 @@
             pop_new = []
             for j in range(self.n_elements):
                 F = -1.0 if np.random.uniform() < 0.5 else 1.0
 
                 ##### Based on Eq. 8, 9, 10
                 self.H_j = self.H_j * np.exp(-self.C_j * (1.0 / np.exp(-epoch / self.epoch) - 1.0 / self.T0))
                 S_ij = self.K * self.H_j * self.P_ij
-                gama = self.beta * np.exp(- ((self.p_best[i][self.ID_TAR][self.ID_FIT] + self.epxilon) /
-                                             (self.pop_group[i][j][self.ID_TAR][self.ID_FIT] + self.epxilon)))
+                gama = self.beta * np.exp(- ((self.p_best[i][self.ID_TAR][self.ID_FIT] + self.epsilon) /
+                                             (self.pop_group[i][j][self.ID_TAR][self.ID_FIT] + self.epsilon)))
                 X_ij = self.pop_group[i][j][self.ID_POS] + F * np.random.uniform() * gama * \
                        (self.p_best[i][self.ID_POS] - self.pop_group[i][j][self.ID_POS]) + \
                        F * np.random.uniform() * self.alpha * (S_ij * self.g_best[self.ID_POS] - self.pop_group[i][j][self.ID_POS])
                 pos_new = self.amend_position(X_ij, self.problem.lb, self.problem.ub)
                 pop_new.append([pos_new, None])
                 if self.mode not in self.AVAILABLE_MODES:
                     pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
@@ -142,10 +141,10 @@
             pos_new = self.amend_position(X_new, self.problem.lb, self.problem.ub)
             pop_idx.append(id)
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_new = self.update_target_wrapper_population(pop_new)
         for idx, id_selected in enumerate(pop_idx):
-            self.pop[id_selected] = deepcopy(pop_new[idx])
+            self.pop[id_selected] = pop_new[idx].copy()
         self.pop_group = self.create_pop_group(self.pop, self.n_clusters, self.n_elements)
         self.p_best = self.get_best_solution_in_team__(self.pop_group)
```

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/MVO.py` & `mealpy-2.5.4a3/mealpy/physics_based/MVO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 21:19, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseMVO(Optimizer):
     """
     The developed version: Multi-Verse Optimizer (MVO)
 
@@ -191,15 +190,15 @@
             list_fitness_normalized = np.random.uniform(0, 0.1, self.pop_size)
         else:
             ### Normalize inflation rates (NI in Eq. (3.1) in the paper)
             list_fitness_normalized = np.reshape(self.normalize__(np.array([list_fitness_raw])), self.pop_size)  # Matrix
 
         pop_new = []
         for idx in range(0, self.pop_size):
-            black_hole_pos = deepcopy(self.pop[idx][self.ID_POS])
+            black_hole_pos = self.pop[idx][self.ID_POS].copy()
             for j in range(0, self.problem.n_dims):
                 r1 = np.random.uniform()
                 if r1 < list_fitness_normalized[idx]:
                     white_hole_id = self.roulette_wheel_selection__((-1 * list_fitness_raw))
                     if white_hole_id == None or white_hole_id == -1:
                         white_hole_id = 0
                     # Eq. (3.1) in the paper
```

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/NRO.py` & `mealpy-2.5.4a3/mealpy/physics_based/NRO.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Created by "Thieu" at 07:02, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
 import math
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalNRO(Optimizer):
     """
     The original version of: Nuclear Reaction Optimization (NRO)
 
@@ -114,21 +113,20 @@
                 target = self.get_target_wrapper(pos_new)
                 self.pop[i] = self.get_better_solution([pos_new, target], self.pop[i])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop = self.greedy_selection_population(self.pop, pop_new)
 
         # NFu phase
-
         ## Ionization stage
         ## Calculate the Pa through Eq. (10)
         pop_child = []
         ranked_pop = np.argsort([self.pop[i][self.ID_TAR][self.ID_FIT] for i in range(self.pop_size)])
         for i in range(self.pop_size):
-            X_ion = deepcopy(self.pop[i][self.ID_POS])
+            X_ion = self.pop[i][self.ID_POS].copy()
             if (ranked_pop[i] * 1.0 / self.pop_size) < np.random.random():
                 i1, i2 = np.random.choice(list(set(range(0, self.pop_size)) - {i}), 2, replace=False)
                 for j in range(self.problem.n_dims):
                     #### Levy flight strategy is described as Eq. 18
                     if self.pop[i2][self.ID_POS][j] == self.pop[i][self.ID_POS][j]:
                         X_ion[j] = self.pop[i][self.ID_POS][j] + alpha * levy_b * (self.pop[i][self.ID_POS][j] - self.g_best[self.ID_POS][j])
                     #### If not, based on Eq. 11, 12
@@ -145,27 +143,25 @@
                     ##### Based on Eq. 21
                     if X_worst[self.ID_POS][j] == self.g_best[self.ID_POS][j]:
                         X_ion[j] = self.pop[i][self.ID_POS][j] + alpha * levy_b * (self.problem.ub[j] - self.problem.lb[j])
                     ##### Based on Eq. 13
                     else:
                         X_ion[j] = self.pop[i][self.ID_POS][j] + round(np.random.uniform()) * np.random.uniform() * \
                                    (X_worst[self.ID_POS][j] - self.g_best[self.ID_POS][j])
-
             ## Check the boundary and evaluate the fitness function for X_ion
             pos_new = self.amend_position(X_ion, self.problem.lb, self.problem.ub)
             pop_child.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
                 self.pop[i] = self.get_better_solution([pos_new, target], self.pop[i])
         if self.mode in self.AVAILABLE_MODES:
             pop_child = self.update_target_wrapper_population(pop_child)
             self.pop = self.greedy_selection_population(pop_child, self.pop)
 
         ## Fusion Stage
-
         ### all ions obtained from ionization are ranked based on (14) - Calculate the Pc through Eq. (14)
         pop_new = []
         ranked_pop = np.argsort([self.pop[i][self.ID_TAR][self.ID_FIT] for i in range(self.pop_size)])
         for i in range(self.pop_size):
             i1, i2 = np.random.choice(list(set(range(0, self.pop_size)) - {i}), 2, replace=False)
 
             #### Generate fusion nucleus
```

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/RIME.py` & `mealpy-2.5.4a3/mealpy/physics_based/RIME.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/SA.py` & `mealpy-2.5.4a3/mealpy/physics_based/SA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 22:08, 01/03/2021 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalSA(Optimizer):
     """
     The original version of: Simulated Annealing (SA)
 
@@ -126,17 +125,17 @@
             # Columnize and Sort Newly Created Population
             pop_new = self.get_sorted_strim_population(pop_new, self.pop_size)
 
             # Randomized Selection
             for idx in range(0, self.pop_size):
                 # Check if new solution is better than current
                 if self.compare_agent(pop_new[idx], self.pop[idx]):
-                    self.pop[idx] = deepcopy(pop_new[idx])
+                    self.pop[idx] = pop_new[idx].copy()
                 else:
                     # Compute difference according to problem type
                     delta = np.abs(pop_new[idx][self.ID_TAR][self.ID_FIT] - self.pop[idx][self.ID_TAR][self.ID_FIT])
                     p = np.exp(-delta / self.dyn_t)  # Compute Acceptance Probability
                     if np.random.uniform() <= p:  # Accept / Reject
-                        self.pop[idx] = deepcopy(pop_new[idx])
+                        self.pop[idx] = pop_new[idx].copy()
         # Update Temperature
         self.dyn_t = self.t_damp * self.dyn_t
         self.dyn_sigma = self.mutation_step_size_damp * self.dyn_sigma
```

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/TWO.py` & `mealpy-2.5.4a3/mealpy/physics_based/TWO.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 21:18, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalTWO(Optimizer):
     """
     The original version of: Tug of War Optimization (TWO)
 
@@ -97,29 +96,29 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        pop_new = deepcopy(self.pop)
+        pop_new = self.pop.copy()
         for idx in range(self.pop_size):
-            pos_new = pop_new[idx][self.ID_POS].astype(float)
+            pos_new = pop_new[idx][self.ID_POS].copy().astype(float)
             for j in range(self.pop_size):
                 if self.pop[idx][self.ID_WEIGHT] < self.pop[j][self.ID_WEIGHT]:
                     force = max(self.pop[idx][self.ID_WEIGHT] * self.muy_s, self.pop[j][self.ID_WEIGHT] * self.muy_s)
                     resultant_force = force - self.pop[idx][self.ID_WEIGHT] * self.muy_k
                     g = self.pop[j][self.ID_POS] - self.pop[idx][self.ID_POS]
                     acceleration = resultant_force * g / (self.pop[idx][self.ID_WEIGHT] * self.muy_k)
                     delta_x = 0.5 * acceleration + np.power(self.alpha, epoch + 1) * self.beta * \
                               (self.problem.ub - self.problem.lb) * np.random.normal(0, 1, self.problem.n_dims)
                     pos_new += delta_x
             pop_new[idx][self.ID_POS] = pos_new
         for idx in range(self.pop_size):
-            pos_new = pop_new[idx][self.ID_POS].astype(float)
+            pos_new = pop_new[idx][self.ID_POS].copy().astype(float)
             for j in range(self.problem.n_dims):
                 if pos_new[j] < self.problem.lb[j] or pos_new[j] > self.problem.ub[j]:
                     if np.random.random() <= 0.5:
                         pos_new[j] = self.g_best[self.ID_POS][j] + np.random.randn() / (epoch + 1) * \
                                                      (self.g_best[self.ID_POS][j] - pos_new[j])
                         if pos_new[j] < self.problem.lb[j] or pos_new[j] > self.problem.ub[j]:
                             pos_new[j] = self.pop[idx][self.ID_POS][j]
@@ -193,29 +192,28 @@
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         ## Apply force of others solution on each individual solution
-        pop_new = deepcopy(self.pop)
+        pop_new = self.pop.copy()
         for idx in range(self.pop_size):
-            pos_new = pop_new[idx][self.ID_POS].astype(float)
+            pos_new = pop_new[idx][self.ID_POS].copy().astype(float)
             for j in range(self.pop_size):
                 if self.pop[idx][self.ID_WEIGHT] < self.pop[j][self.ID_WEIGHT]:
                     force = max(self.pop[idx][self.ID_WEIGHT] * self.muy_s, self.pop[j][self.ID_WEIGHT] * self.muy_s)
                     resultant_force = force - self.pop[idx][self.ID_WEIGHT] * self.muy_k
                     g = self.pop[j][self.ID_POS] - self.pop[idx][self.ID_POS]
                     temp = (self.pop[idx][self.ID_WEIGHT] * self.muy_k)
                     acceleration = resultant_force * g / temp
                     delta_x = 1 / 2 * acceleration + np.power(self.alpha, epoch + 1) * self.beta * \
                               (self.problem.ub - self.problem.lb) * np.random.normal(0, 1, self.problem.n_dims)
                     pos_new += delta_x
             self.pop[idx][self.ID_POS] = pos_new
-
         ## Amend solution and update fitness value
         for idx in range(self.pop_size):
             pos_new = self.g_best[self.ID_POS] + np.random.normal(0, 1, self.problem.n_dims) / (epoch + 1) * \
                       (self.g_best[self.ID_POS] - pop_new[idx][self.ID_POS])
             conditions = np.logical_or(pop_new[idx][self.ID_POS] < self.problem.lb, pop_new[idx][self.ID_POS] > self.problem.ub)
             conditions = np.logical_and(conditions, np.random.random(self.problem.n_dims) < 0.5)
             pos_new = np.where(conditions, pos_new, self.pop[idx][self.ID_POS])
@@ -280,29 +278,29 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        pop_new = deepcopy(self.pop)
+        pop_new = self.pop.copy()
         for i in range(self.pop_size):
-            pos_new = self.pop[i][self.ID_POS].astype(float)
+            pos_new = self.pop[i][self.ID_POS].copy().astype(float)
             for k in range(self.pop_size):
                 if self.pop[i][self.ID_WEIGHT] < self.pop[k][self.ID_WEIGHT]:
                     force = max(self.pop[i][self.ID_WEIGHT] * self.muy_s, self.pop[k][self.ID_WEIGHT] * self.muy_s)
                     resultant_force = force - self.pop[i][self.ID_WEIGHT] * self.muy_k
                     g = self.pop[k][self.ID_POS] - self.pop[i][self.ID_POS]
                     acceleration = resultant_force * g / (self.pop[i][self.ID_WEIGHT] * self.muy_k)
                     delta_x = 1 / 2 * acceleration + np.power(self.alpha, epoch + 1) * self.beta * \
                               (self.problem.ub - self.problem.lb) * np.random.normal(0, 1, self.problem.n_dims)
                     pos_new +=delta_x
             pop_new[i][self.ID_POS] = pos_new
         for i in range(self.pop_size):
-            pos_new = self.pop[i][self.ID_POS].astype(float)
+            pos_new = self.pop[i][self.ID_POS].copy().astype(float)
             for j in range(self.problem.n_dims):
                 if pos_new[j] < self.problem.lb[j] or pos_new[j] > self.problem.ub[j]:
                     if np.random.random() <= 0.5:
                         pos_new[j] = self.g_best[self.ID_POS][j] + np.random.randn() / (epoch + 1) * \
                                                      (self.g_best[self.ID_POS][j] - pos_new[j])
                         if pos_new[j] < self.problem.lb[j] or pos_new[j] > self.problem.ub[j]:
                             pos_new[j] = self.pop[i][self.ID_POS][j]
@@ -374,15 +372,15 @@
             pop_size (int): number of population size, default = 100
         """
         super().__init__(epoch, pop_size, **kwargs)
 
     def initialization(self):
         if self.pop is None:
             self.pop = self.create_population(self.pop_size)
-        pop_oppo = deepcopy(self.pop)
+        pop_oppo = self.pop.copy()
         for i in range(self.pop_size):
             pos_opposite = self.problem.ub + self.problem.lb - self.pop[i][self.ID_POS]
             pos_new = self.amend_position(pos_opposite, self.problem.lb, self.problem.ub)
             pop_oppo[i][self.ID_POS] = pos_new
             if self.mode not in self.AVAILABLE_MODES:
                 pop_oppo[i][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_oppo = self.update_target_wrapper_population(pop_oppo)
@@ -392,29 +390,29 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        pop_new = deepcopy(self.pop)
+        pop_new = self.pop.copy()
         for i in range(self.pop_size):
-            pos_new = self.pop[i][self.ID_POS].astype(float)
+            pos_new = self.pop[i][self.ID_POS].copy().astype(float)
             for k in range(self.pop_size):
                 if self.pop[i][self.ID_WEIGHT] < self.pop[k][self.ID_WEIGHT]:
                     force = max(self.pop[i][self.ID_WEIGHT] * self.muy_s, self.pop[k][self.ID_WEIGHT] * self.muy_s)
                     resultant_force = force - self.pop[i][self.ID_WEIGHT] * self.muy_k
                     g = self.pop[k][self.ID_POS] - self.pop[i][self.ID_POS]
                     acceleration = resultant_force * g / (self.pop[i][self.ID_WEIGHT] * self.muy_k)
                     delta_x = 1 / 2 * acceleration + np.power(self.alpha, epoch + 1) * self.beta * \
                               (self.problem.ub - self.problem.lb) * np.random.normal(0, 1, self.problem.n_dims)
                     pos_new += delta_x
             pop_new[i][self.ID_POS] = pos_new
         for i in range(self.pop_size):
-            pos_new = self.pop[i][self.ID_POS].astype(float)
+            pos_new = self.pop[i][self.ID_POS].copy().astype(float)
             for j in range(self.problem.n_dims):
                 if pos_new[j] < self.problem.lb[j] or pos_new[j] > self.problem.ub[j]:
                     if np.random.random() <= 0.5:
                         pos_new[j] = self.g_best[self.ID_POS][j] + np.random.randn() / (epoch + 1) * \
                                                      (self.g_best[self.ID_POS][j] - pos_new[j])
                         if pos_new[j] < self.problem.lb[j] or pos_new[j] > self.problem.ub[j]:
                             pos_new[j] = self.pop[i][self.ID_POS][j]
```

### Comparing `mealpy-2.5.4a2/mealpy/physics_based/WDO.py` & `mealpy-2.5.4a3/mealpy/physics_based/WDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/ABC.py` & `mealpy-2.5.4a3/mealpy/swarm_based/ABC.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/ACOR.py` & `mealpy-2.5.4a3/mealpy/swarm_based/ACOR.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/AGTO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/AGTO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/ALO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/ALO.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 12:01, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalALO(Optimizer):
     """
     The original version of: Ant Lion Optimizer (ALO)
 
@@ -125,15 +124,15 @@
         pop_new = self.update_target_wrapper_population(pop_new)
 
         # Update antlion positions and fitnesses based on the ants (if an ant becomes fitter than an antlion
         # we assume it was caught by the antlion and the antlion update goes to its position to build the trap)
         self.pop = self.get_sorted_strim_population(self.pop + pop_new, self.pop_size)
 
         # Keep the elite in the population
-        self.pop[-1] = deepcopy(self.g_best)
+        self.pop[-1] = self.g_best.copy()
 
 
 class BaseALO(OriginalALO):
     """
     The developed version: Ant Lion Optimizer (ALO)
 
     Notes
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/AO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/AO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/ARO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/ARO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/AVOA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/AVOA.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,21 +68,14 @@
         self.p2 = self.validator.check_float("p2", p2, (0, 1))
         self.p3 = self.validator.check_float("p3", p3, (0, 1))
         self.alpha = self.validator.check_float("alpha", alpha, (0, 1))
         self.gama = self.validator.check_float("gama", gama, (0, 5.0))
         self.set_parameters(["epoch", "pop_size", "p1", "p2", "p3", "alpha", "gama"])
         self.sort_flag = False
 
-    def get_levy_flight__(self, beta=1.0, size=None):
-        sigma = np.random.gamma(1 + beta) * np.sin(np.pi * beta/2) / (np.random.gamma((1+beta)/2) * beta * 2**((beta-1)/2)) ** (1 / beta)
-        u = np.random.normal(0, 1, size) * sigma
-        v = np.random.normal(0, 1, size)
-        step = u / np.abs(v)**(1 / beta)
-        return step
-
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
@@ -105,15 +98,16 @@
                     best_x1 = best_list[0][self.ID_POS]
                     best_x2 = best_list[1][self.ID_POS]
                     if np.random.rand() < self.p2:
                         A = best_x1 - ((best_x1 * self.pop[idx][self.ID_POS]) / (best_x1 - self.pop[idx][self.ID_POS]**2))*F
                         B = best_x2-((best_x2 * self.pop[idx][self.ID_POS]) / (best_x2 - self.pop[idx][self.ID_POS]**2))*F
                         pos_new = (A + B) / 2
                     else:
-                        pos_new = rand_pos - np.abs(rand_pos - self.pop[idx][self.ID_POS]) * F * self.get_levy_flight__(beta=1.5, size=self.problem.n_dims)
+                        pos_new = rand_pos - np.abs(rand_pos - self.pop[idx][self.ID_POS]) * F * \
+                                  self.get_levy_flight_step(beta=1.5, multiplier=1., size=self.problem.n_dims, case=-1)
                 else:       # Phase 2
                     if np.random.rand() < self.p3:
                         pos_new = (np.abs((2 * np.random.rand()) * rand_pos - self.pop[idx][self.ID_POS])) * (F + np.random.rand()) - \
                                   (rand_pos - self.pop[idx][self.ID_POS])
                     else:
                         s1 = rand_pos * (np.random.rand() * self.pop[idx][self.ID_POS] / (2 * np.pi)) * np.cos(self.pop[idx][self.ID_POS])
                         s2 = rand_pos * (np.random.rand() * self.pop[idx][self.ID_POS] / (2 * np.pi)) * np.sin(self.pop[idx][self.ID_POS])
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/BA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/BA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 12:00, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalBA(Optimizer):
     """
     The original version of: Bat-inspired Algorithm (BA)
 
@@ -97,15 +96,15 @@
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         pop_new = []
         for idx in range(0, self.pop_size):
-            agent = deepcopy(self.pop[idx])
+            agent = self.pop[idx].copy()
             agent[self.ID_VEC] = agent[self.ID_VEC] + self.pop[idx][self.ID_PFRE] * (self.pop[idx][self.ID_POS] - self.g_best[self.ID_POS])
             x = self.pop[idx][self.ID_POS] + agent[self.ID_VEC]
             ## Local Search around g_best position
             if np.random.uniform() > self.pulse_rate:
                 x = self.g_best[self.ID_POS] + 0.0001 * np.random.normal(self.problem.n_dims)  # gauss
             pos_new = self.amend_position(x, self.problem.lb, self.problem.ub)
             agent[self.ID_POS] = pos_new
@@ -113,15 +112,15 @@
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_new = self.update_target_wrapper_population(pop_new)
         for idx in range(self.pop_size):
             ## Replace the old position by the new one when its has better fitness.
             ##  and then update loudness and emission rate
             if self.compare_agent(pop_new[idx], self.pop[idx]) and np.random.rand() < self.loudness:
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
 
 
 class AdaptiveBA(Optimizer):
     """
     The original version of: Adaptive Bat-inspired Algorithm (BA)
 
     Notes
@@ -222,15 +221,15 @@
 
         Args:
             epoch (int): The current iteration
         """
         mean_a = np.mean([agent[self.ID_LOUD] for agent in self.pop])
         pop_new = []
         for idx in range(0, self.pop_size):
-            agent = deepcopy(self.pop[idx])
+            agent = self.pop[idx].copy()
             agent[self.ID_VEC] = agent[self.ID_VEC] + self.pop[idx][self.ID_PFRE] * (self.pop[idx][self.ID_POS] - self.g_best[self.ID_POS])
             x = self.pop[idx][self.ID_POS] + agent[self.ID_VEC]
             ## Local Search around g_best position
             if np.random.uniform() > agent[self.ID_PRAT]:
                 # print(f"{epoch}, {mean_a}, {self.dyn_r}")
                 x = self.g_best[self.ID_POS] + mean_a * np.random.normal(-1, 1)
             pos_new = self.amend_position(x, self.problem.lb, self.problem.ub)
@@ -241,15 +240,15 @@
         pop_new = self.update_target_wrapper_population(pop_new)
         for idx in range(0, self.pop_size):
             ## Replace the old position by the new one when its has better fitness.
             ##  and then update loudness and emission rate
             if self.compare_agent(pop_new[idx], self.pop[idx]) and np.random.rand() < pop_new[idx][self.ID_LOUD]:
                 pop_new[idx][self.ID_LOUD] = self.alpha * pop_new[idx][self.ID_LOUD]
                 pop_new[idx][self.ID_PRAT] = pop_new[idx][self.ID_PRAT] * (1 - np.exp(-self.gamma * (epoch + 1)))
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
 
 
 class ModifiedBA(Optimizer):
     """
     The original version of: Modified Bat-inspired Algorithm (MBA)
 
     Notes
@@ -321,21 +320,21 @@
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_new = self.update_target_wrapper_population(pop_new)
         pop_child_idx = []
         pop_child = []
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
             else:
                 if np.random.random() > self.pulse_rate:
                     x = self.g_best[self.ID_POS] + 0.01 * np.random.uniform(self.problem.lb, self.problem.ub)
                     pos_new = self.amend_position(x, self.problem.lb, self.problem.ub)
                     pop_child_idx.append(idx)
                     pop_child.append([pos_new, None])
                     if self.mode not in self.AVAILABLE_MODES:
                         pop_child[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_child = self.update_target_wrapper_population(pop_child)
         for idx, idx_selected in enumerate(pop_child_idx):
             if self.compare_agent(pop_child[idx], pop_new[idx_selected]):
-                pop_new[idx_selected] = deepcopy(pop_child[idx])
+                pop_new[idx_selected] = pop_child[idx].copy()
         self.pop = pop_new
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/BES.py` & `mealpy-2.5.4a3/mealpy/swarm_based/BES.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/BFO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/BFO.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 10:21, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalBFO(Optimizer):
     """
     The original version of: Bacterial Foraging Optimization (BFO)
 
@@ -170,16 +169,15 @@
                         self.pop[idx][self.ID_POS] = pos_new
                         self.pop[idx][self.ID_TAR] = target
                         break
                     sum_nutrients += self.pop[idx][self.ID_COST]
                 self.pop[idx][self.ID_SUM_NUTRIENTS] = sum_nutrients
 
             cells = sorted(self.pop, key=lambda cell: cell[self.ID_SUM_NUTRIENTS])
-            self.pop = deepcopy(cells[0:self.half_pop_size]) + deepcopy(cells[0:self.half_pop_size])
-
+            self.pop = cells[0:self.half_pop_size].copy() + cells[0:self.half_pop_size].copy()
             for idc in range(self.pop_size):
                 if np.random.rand() < self.p_eliminate:
                     self.pop[idc] = self.create_solution(self.problem.lb, self.problem.ub)
 
 
 class ABFO(Optimizer):
     """
@@ -269,16 +267,16 @@
             list: wrapper of solution with format [position, target, nutrient, local_pos_best, local_fit_best]
         """
         if pos is None:
             pos = self.generate_position(lb, ub)
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         nutrient = 0  # total nutrient gained by the bacterium in its whole searching process.(int number)
-        local_pos_best = deepcopy(position)
-        local_fit_best = deepcopy(target)
+        local_pos_best = position.copy()
+        local_fit_best = target.copy()
         return [position, target, nutrient, local_pos_best, local_fit_best]
 
     def update_step_size__(self, pop=None, idx=None):
         total_fitness = np.sum([temp[self.ID_TAR][self.ID_FIT] for temp in pop])
         step_size = self.C_s - (self.C_s - self.C_e) * pop[idx][self.ID_TAR][self.ID_FIT] / total_fitness
         step_size = step_size / self.pop[idx][self.ID_NUT] if self.pop[idx][self.ID_NUT] > 0 else step_size
         return step_size
@@ -302,25 +300,25 @@
                 target = self.get_target_wrapper(pos_new)
                 if self.compare_agent([pos_new, target], self.pop[i]):
                     self.pop[i][self.ID_POS] = pos_new
                     self.pop[i][self.ID_TAR] = target
                     self.pop[i][self.ID_NUT] += 1
                     # Update personal best
                     if self.compare_agent([pos_new, target], [None, self.pop[i][self.ID_LOC_FIT]]):
-                        self.pop[i][self.ID_LOC_POS] = deepcopy(pos_new)
-                        self.pop[i][self.ID_LOC_FIT] = deepcopy(target)
+                        self.pop[i][self.ID_LOC_POS] = pos_new.copy()
+                        self.pop[i][self.ID_LOC_FIT] = target
                 else:
                     self.pop[i][self.ID_NUT] -= 1
 
             if self.pop[i][self.ID_NUT] > max(self.N_split, self.N_split + (len(self.pop) - self.pop_size) / self.N_adapt):
                 pos_new = self.pop[i][self.ID_POS] + np.random.normal(self.problem.lb, self.problem.ub) * \
                           (self.g_best[self.ID_POS] - self.pop[i][self.ID_POS])
                 pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
                 target = self.get_target_wrapper(pos_new)
-                self.pop.append([pos_new, target, 0, deepcopy(pos_new), deepcopy(target)])
+                self.pop.append([pos_new, target, 0, pos_new.copy(), target.copy()])
 
             nut_min = min(self.N_adapt, self.N_adapt + (len(self.pop) - self.pop_size) / self.N_adapt)
             if self.pop[i][self.ID_NUT] < nut_min or np.random.rand() < self.p_eliminate:
                 self.pop[i] = self.create_solution(self.problem.lb, self.problem.ub)
 
         ## Make sure the population does not have duplicates.
         new_set = set()
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/BSA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/BSA.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 11:59, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalBSA(Optimizer):
     """
     The original version of: Bird Swarm Algorithm (BSA)
 
@@ -97,16 +96,16 @@
         Returns:
             list: a solution with format [position, target, local_position, local_fitness]
         """
         if pos is None:
             pos = self.generate_position(lb, ub)
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
-        local_position = deepcopy(position)
-        local_fitness = deepcopy(target)
+        local_position = position.copy()
+        local_fitness = target.copy()
         return [position, target, local_position, local_fitness]
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
@@ -116,15 +115,15 @@
         fit_list = np.array([item[self.ID_LBF][self.ID_FIT] for item in self.pop])
         pos_mean = np.mean(pos_list, axis=0)
         fit_sum = np.sum(fit_list)
 
         if epoch % self.ff != 0:
             pop_new = []
             for i in range(0, self.pop_size):
-                agent = deepcopy(self.pop[i])
+                agent = self.pop[i].copy()
                 prob = np.random.uniform() * 0.2 + self.pff  # The probability of foraging for food
                 if np.random.uniform() < prob:  # Birds forage for food. Eq. 1
                     x_new = self.pop[i][self.ID_POS] + self.c1 * \
                             np.random.uniform() * (self.pop[i][self.ID_LBP] - self.pop[i][self.ID_POS]) + \
                             self.c2 * np.random.uniform() * (self.g_best[self.ID_POS] - self.pop[i][self.ID_POS])
                 else:  # Birds keep vigilance. Eq. 2
                     A1 = self.a1 * np.exp(-self.pop_size * self.pop[i][self.ID_LBF][self.ID_FIT] / (self.EPSILON + fit_sum))
@@ -139,15 +138,15 @@
                 if self.mode not in self.AVAILABLE_MODES:
                     agent[self.ID_TAR] = self.get_target_wrapper(pos_new)
                     self.pop[i] = self.get_better_solution(agent, self.pop[i])
             if self.mode in self.AVAILABLE_MODES:
                 pop_new = self.update_target_wrapper_population(pop_new)
                 self.pop = self.greedy_selection_population(self.pop, pop_new)
         else:
-            pop_new = deepcopy(self.pop)
+            pop_new = self.pop.copy()
             # Divide the bird swarm into two parts: producers and scroungers.
             min_idx = np.argmin(fit_list)
             max_idx = np.argmax(fit_list)
             choose = 0
             if min_idx < 0.5 * self.pop_size and max_idx < 0.5 * self.pop_size:
                 choose = 1
             if min_idx > 0.5 * self.pop_size and max_idx < 0.5 * self.pop_size:
@@ -155,44 +154,44 @@
             if min_idx < 0.5 * self.pop_size and max_idx > 0.5 * self.pop_size:
                 choose = 3
             if min_idx > 0.5 * self.pop_size and max_idx > 0.5 * self.pop_size:
                 choose = 4
 
             if choose < 3:  # Producing (Equation 5)
                 for i in range(int(self.pop_size / 2 + 1), self.pop_size):
-                    agent = deepcopy(self.pop[i])
+                    agent = self.pop[i].copy()
                     x_new = self.pop[i][self.ID_POS] + np.random.uniform(self.problem.lb, self.problem.ub) * self.pop[i][self.ID_POS]
                     agent[self.ID_POS] = self.amend_position(x_new, self.problem.lb, self.problem.ub)
                     pop_new[i] = agent
                 if choose == 1:
                     x_new = self.pop[min_idx][self.ID_POS] + np.random.uniform(self.problem.lb, self.problem.ub) * self.pop[min_idx][self.ID_POS]
-                    agent = deepcopy(self.pop[min_idx])
+                    agent = self.pop[min_idx].copy()
                     agent[self.ID_POS] = self.amend_position(x_new, self.problem.lb, self.problem.ub)
                     pop_new[min_idx] = agent
                 for i in range(0, int(self.pop_size / 2)):
                     if choose == 2 or min_idx != i:
-                        agent = deepcopy(self.pop[i])
+                        agent = self.pop[i].copy()
                         FL = np.random.uniform() * 0.4 + self.fl
                         idx = np.random.randint(0.5 * self.pop_size + 1, self.pop_size)
                         x_new = self.pop[i][self.ID_POS] + (self.pop[idx][self.ID_POS] - self.pop[i][self.ID_POS]) * FL
                         agent[self.ID_POS] = self.amend_position(x_new, self.problem.lb, self.problem.ub)
                         pop_new[i] = agent
             else:  # Scrounging (Equation 6)
                 for i in range(0, int(0.5 * self.pop_size)):
-                    agent = deepcopy(self.pop[i])
+                    agent = self.pop[i].copy()
                     x_new = self.pop[i][self.ID_POS] + np.random.uniform(self.problem.lb, self.problem.ub) * self.pop[i][self.ID_POS]
                     agent[self.ID_POS] = self.amend_position(x_new, self.problem.lb, self.problem.ub)
                     pop_new[i] = agent
                 if choose == 4:
-                    agent = deepcopy(self.pop[min_idx])
+                    agent = self.pop[min_idx].copy()
                     x_new = self.pop[min_idx][self.ID_POS] + np.random.uniform(self.problem.lb, self.problem.ub) * self.pop[min_idx][self.ID_POS]
                     agent[self.ID_POS] = self.amend_position(x_new, self.problem.lb, self.problem.ub)
                 for i in range(int(self.pop_size / 2 + 1), self.pop_size):
                     if choose == 3 or min_idx != i:
-                        agent = deepcopy(self.pop[i])
+                        agent = self.pop[i].copy()
                         FL = np.random.uniform() * 0.4 + self.fl
                         idx = np.random.randint(0, 0.5 * self.pop_size)
                         x_new = self.pop[i][self.ID_POS] + (self.pop[idx][self.ID_POS] - self.pop[i][self.ID_POS]) * FL
                         agent[self.ID_POS] = self.amend_position(x_new, self.problem.lb, self.problem.ub)
                         pop_new[i] = agent
             if self.mode in self.AVAILABLE_MODES:
                 pop_new = self.update_target_wrapper_population(pop_new)
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/BeesA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/BeesA.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Created by "Thieu" at 15:34, 01/03/2021 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
 from mealpy.optimizer import Optimizer
-from copy import deepcopy
 
 
 class CleverBookBeesA(Optimizer):
     """
     The original version of: Bees Algorithm
 
     Notes
@@ -85,15 +84,15 @@
     def search_neighborhood__(self, parent=None, neigh_size=None):
         """
         Search 1 best position in neigh_size position
         """
         pop_neigh = []
         for idx in range(0, neigh_size):
             t1 = np.random.randint(0, len(parent[self.ID_POS]) - 1)
-            new_bee = deepcopy(parent[self.ID_POS])
+            new_bee = parent[self.ID_POS].copy()
             new_bee[t1] = (parent[self.ID_POS][t1] + np.random.uniform() * self.patch_size) if np.random.uniform() < 0.5 \
                 else (parent[self.ID_POS][t1] - np.random.uniform() * self.patch_size)
             pos_new = self.amend_position(new_bee, self.problem.lb, self.problem.ub)
             pop_neigh.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 pop_neigh[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_neigh = self.update_target_wrapper_population(pop_neigh)
@@ -215,15 +214,15 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        pop_new = deepcopy(self.pop)
+        pop_new = self.pop.copy()
         for idx in range(0, self.pop_size):
             # Elite Sites
             if idx < self.n_elite_bees:
                 pop_child = []
                 for j in range(0, self.n_elite_bees_local):
                     pos_new = self.perform_dance__(self.pop[idx][self.ID_POS], self.dyn_radius)
                     pop_child.append([pos_new, None])
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/COA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/COA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 13:59, 24/06/2021 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalCOA(Optimizer):
     """
     The original version of: Coyote Optimization Algorithm (COA)
 
@@ -140,15 +139,15 @@
             if self.compare_agent([pos_new, target], packs[-1]):
                 if self.problem.minmax == "min":
                     packs = sorted(packs, key=lambda agent: agent[self.ID_AGE])
                 else:
                     packs = sorted(packs, key=lambda agent: agent[self.ID_AGE], reverse=True)
                 # Replace worst element by new child, New born child with age = 0
                 packs[-1] = [pos_new, target, 0]
-                self.pop_group[p] = deepcopy(packs)
+                self.pop_group[p] = packs.copy()
 
         # A coyote can leave a pack and enter in another pack (Eq. 4)
         if self.n_packs > 1:
             if np.random.rand() < self.p_leave:
                 id_pack1, id_pack2 = np.random.choice(list(range(0, self.n_packs)), 2, replace=False)
                 id1, id2 = np.random.choice(list(range(0, self.n_coyotes)), 2, replace=False)
                 self.pop_group[id_pack1][id1], self.pop_group[id_pack2][id2] = self.pop_group[id_pack2][id2], self.pop_group[id_pack1][id1]
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/CSA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/CSA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 18:37, 28/05/2021 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalCSA(Optimizer):
     """
     The original version of: Cuckoo Search Algorithm (CSA)
 
@@ -65,15 +64,15 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        pop_new = deepcopy(self.pop)
+        pop_new = self.pop.copy()
         for i in range(0, self.pop_size):
             ## Generate levy-flight solution
             levy_step = self.get_levy_flight_step(multiplier=0.001, case=-1)
             pos_new = self.pop[i][self.ID_POS] + 1.0 / np.sqrt(epoch + 1) * np.sign(np.random.random() - 0.5) * \
                       levy_step * (self.pop[i][self.ID_POS] - self.g_best[self.ID_POS])
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             target = self.get_target_wrapper(pos_new)
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/CSO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/CSO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 10:09, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalCSO(Optimizer):
     """
     The original version of: Cat Swarm Optimization (CSO)
 
@@ -118,16 +117,16 @@
         flag = True if np.random.uniform() < self.mixture_ratio else False
         return [position, target, velocity, flag]
 
     def seeking_mode__(self, cat):
         candidate_cats = []
         clone_cats = self.create_population(self.smp)
         if self.spc:
-            candidate_cats.append(deepcopy(cat))
-            clone_cats = [deepcopy(cat) for _ in range(self.smp - 1)]
+            candidate_cats.append(cat.copy())
+            clone_cats = [cat.copy() for _ in range(self.smp - 1)]
 
         for clone in clone_cats:
             idx = np.random.choice(range(0, self.problem.n_dims), int(self.cdc * self.problem.n_dims), replace=False)
             pos_new1 = clone[self.ID_POS] * (1 + self.srd)
             pos_new2 = clone[self.ID_POS] * (1 - self.srd)
 
             pos_new = np.where(np.random.random(self.problem.n_dims) < 0.5, pos_new1, pos_new2)
@@ -160,15 +159,15 @@
 
         Args:
             epoch (int): The current iteration
         """
         w = (self.epoch - epoch) / self.epoch * (self.w_max - self.w_min) + self.w_min
         pop_new = []
         for idx in range(0, self.pop_size):
-            agent = deepcopy(self.pop[idx])
+            agent = self.pop[idx].copy()
             # tracing mode
             if self.pop[idx][self.ID_FLAG]:
                 pos_new = self.pop[idx][self.ID_POS] + w * self.pop[idx][self.ID_VEL] + \
                           np.random.uniform() * self.c1 * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
                 pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             else:
                 pos_new = self.seeking_mode__(self.pop[idx])
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/CoatiOA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/CoatiOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/DMOA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/DMOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/DO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/DO.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 04:43, 02/03/2021 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalDO(Optimizer):
     """
     The original version of: Dragonfly Optimization (DO)
 
@@ -104,16 +103,16 @@
             # Separation: Eq 3.1, Alignment: Eq 3.2, Cohesion: Eq 3.3
             if neighbours_num > 1:
                 S = np.sum(pos_neighbours, axis=0) - neighbours_num * self.pop[i][self.ID_POS]
                 A = np.sum(pos_neighbours_delta, axis=0) / neighbours_num
                 C_temp = np.sum(pos_neighbours, axis=0) / neighbours_num
             else:
                 S = np.zeros(self.problem.n_dims)
-                A = deepcopy(self.pop_delta[i][self.ID_POS])
-                C_temp = deepcopy(self.pop[i][self.ID_POS])
+                A = self.pop_delta[i][self.ID_POS].copy()
+                C_temp = self.pop[i][self.ID_POS].copy()
             C = C_temp - self.pop[i][self.ID_POS]
 
             # Attraction to food: Eq 3.4
             dist_to_food = np.abs(self.pop[i][self.ID_POS] - self.g_best[self.ID_POS])
             if np.all(dist_to_food <= r):
                 F = self.g_best[self.ID_POS] - self.pop[i][self.ID_POS]
             else:
@@ -122,22 +121,22 @@
             # Distraction from enemy: Eq 3.5
             dist_to_enemy = np.abs(self.pop[i][self.ID_POS] - self.g_worst[self.ID_POS])
             if np.all(dist_to_enemy <= r):
                 enemy = self.g_worst[self.ID_POS] + self.pop[i][self.ID_POS]
             else:
                 enemy = np.zeros(self.problem.n_dims)
 
-            pos_new = deepcopy(self.pop[i][self.ID_POS]).astype(float)
-            pos_delta_new = deepcopy(self.pop_delta[i][self.ID_POS]).astype(float)
+            pos_new = self.pop[i][self.ID_POS].copy().astype(float)
+            pos_delta_new = self.pop_delta[i][self.ID_POS].copy().astype(float)
             if np.any(dist_to_food > r):
                 if neighbours_num > 1:
                     temp = w * self.pop_delta[i][self.ID_POS] + np.random.uniform(0, 1, self.problem.n_dims) * A + \
                            np.random.uniform(0, 1, self.problem.n_dims) * C + np.random.uniform(0, 1, self.problem.n_dims) * S
                     temp = np.clip(temp, -1 * self.delta_max, self.delta_max)
-                    pos_delta_new = deepcopy(temp)
+                    pos_delta_new = temp.copy()
                     pos_new += temp
                 else:  # Eq. 3.8
                     pos_new += self.get_levy_flight_step(beta=1.5, multiplier=0.01, case=-1) * self.pop[i][self.ID_POS]
                     pos_delta_new = np.zeros(self.problem.n_dims)
             else:
                 # Eq. 3.6
                 temp = (a * A + c * C + s * S + f * F + e * enemy) + w * self.pop_delta[i][self.ID_POS]
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/EHO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/EHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/ESOA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/ESOA.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Created by "Thieu" at 17:48, 21/05/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from mealpy.optimizer import Optimizer
-from copy import deepcopy
 
 
 class OriginalESOA(Optimizer):
     """
     The original version of: Egret Swarm Optimization Algorithm (ESOA)
 
     Links:
@@ -64,15 +63,15 @@
             pos = self.generate_position(lb, ub)
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         weights = np.random.uniform(-1, 1, len(lb))
         g = (np.sum(weights * position) - target[self.ID_FIT]) * position
         m = np.zeros(self.problem.n_dims)
         v = np.zeros(self.problem.n_dims)
-        return [position, target, weights, position.copy(), deepcopy(target), g, m, v]
+        return [position, target, weights, position.copy(), target.copy(), g, m, v]
 
     def initialize_variables(self):
         self.beta1 = 0.9
         self.beta2 = 0.99
 
     def evolve(self, epoch):
         """
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/FA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/FA.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 22:07, 07/04/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalFA(Optimizer):
     """
     The original version of: Fireworks Algorithm (FA)
 
@@ -99,29 +98,29 @@
                 si_ = int(round(self.p_b * self.max_sparks) + 1)
             else:
                 si_ = int(round(si) + 1)
 
             ## Algorithm 1
             pop_new = []
             for j in range(0, si_):
-                pos_new = deepcopy(self.pop[idx][self.ID_POS])
+                pos_new = self.pop[idx][self.ID_POS].copy()
                 list_idx = np.random.choice(range(0, self.problem.n_dims), round(np.random.uniform() * self.problem.n_dims), replace=False)
                 displacement = Ai * np.random.uniform(-1, 1)
                 pos_new[list_idx] = pos_new[list_idx] + displacement
                 pos_new = np.where(np.logical_or(pos_new < self.problem.lb, pos_new > self.problem.ub),
                                    self.problem.lb + np.abs(pos_new) % (self.problem.ub - self.problem.lb), pos_new)
                 pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
                 pop_new.append([pos_new, None])
                 if self.mode not in self.AVAILABLE_MODES:
                     pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
             pop_new = self.update_target_wrapper_population(pop_new)
 
         for _ in range(0, self.m_sparks):
             idx = np.random.randint(0, self.pop_size)
-            pos_new = deepcopy(self.pop[idx][self.ID_POS])
+            pos_new = self.pop[idx][self.ID_POS].copy()
             list_idx = np.random.choice(range(0, self.problem.n_dims), round(np.random.uniform() * self.problem.n_dims), replace=False)
             pos_new[list_idx] = pos_new[list_idx] + np.random.normal(0, 1, len(list_idx))  # Gaussian
             condition = np.logical_or(pos_new < self.problem.lb, pos_new > self.problem.ub)
             pos_true = self.problem.lb + np.abs(pos_new) % (self.problem.ub - self.problem.lb)
             pos_new = np.where(condition, pos_true, pos_new)
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/FFA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/FFA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 17:13, 01/03/2021 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalFFA(Optimizer):
     """
     The original version of: Firefly Algorithm (FFA)
 
@@ -90,15 +89,15 @@
 
         Args:
             epoch (int): The current iteration
         """
         # Maximum Distance
         dmax = np.sqrt(self.problem.n_dims)
         for idx in range(0, self.pop_size):
-            agent = deepcopy(self.pop[idx])
+            agent = self.pop[idx].copy()
             pop_child = []
             for j in range(idx + 1, self.pop_size):
                 # Move Towards Better Solutions
                 if self.compare_agent(self.pop[j], agent):
                     # Calculate Radius and Attraction Level
                     rij = np.linalg.norm(agent[self.ID_POS] - self.pop[j][self.ID_POS]) / dmax
                     beta = self.beta_base * np.exp(-self.gamma * rij ** self.exponent)
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/FFO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/FFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/FOA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/FOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/FOX.py` & `mealpy-2.5.4a3/mealpy/swarm_based/FOX.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/GJO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/GJO.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Created by "Thieu" at 00:08, 27/10/2022 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from mealpy.optimizer import Optimizer
-from math import gamma
 
 
 class OriginalGJO(Optimizer):
     """
     The original version of: Golden jackal optimization (GJO)
 
     Links:
@@ -51,31 +50,23 @@
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
         self.set_parameters(["epoch", "pop_size"])
         self.sort_flag = False
 
-    def levy__(self, beta=1.0, size=None):
-        num = gamma(1 + beta) * np.sin(np.pi * beta/2)
-        den = gamma((1+beta)/2) * beta * 2**((beta-1)/2)
-        sigma_u = (num/den)**(1.0/beta)
-        u = np.random.normal(0, sigma_u, size=size)
-        v = np.random.normal(0, 1, size=size)
-        return u/(np.abs(v)**(1.0/beta))
-
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         E1 = 1.5*(1-((1+epoch)/self.epoch))
-        RL = 0.05*self.levy__(beta=1.5, size=(self.pop_size, self.problem.n_dims))
+        RL = self.get_levy_flight_step(beta=1.5, multiplier=0.05, size=(self.pop_size, self.problem.n_dims), case=-1)
         _, (male, female), _ = self.get_special_solutions(self.pop, best=2, worst=1)
         pop_new = []
         for idx in range(0, self.pop_size):
             male_pos = male[self.ID_POS].copy()
             female_pos = female[self.ID_POS].copy()
 
             for jdx in range(0, self.problem.n_dims):
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/GOA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/GOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/GTO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/GTO.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 21:58, 16/03/2023 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
-from math import gamma
 import numpy as np
 from mealpy.optimizer import Optimizer
 
 
 class OriginalGTO(Optimizer):
     """
     The original version of: Giant Trevally Optimizer (GTO)
@@ -62,35 +61,27 @@
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
         self.A = self.validator.check_float("A", A, [-10., 10.])
         self.H = self.validator.check_float("H", H, [1., 10.])
         self.set_parameters(["epoch", "pop_size", "A", "H"])
         self.sort_flag = True
 
-    def levy__(self, beta=1.0, size=None, step=0.01):
-        num = gamma(1 + beta) * np.sin(np.pi * beta/2)
-        den = gamma((1+beta)/2) * beta * 2**((beta-1)/2)
-        sigma_u = (num/den)**(1.0/beta)
-        u = np.random.normal(0, sigma_u, size=size)
-        v = np.random.normal(0, 1, size=size)
-        return u/(np.abs(v)**(1.0/beta)) * step
-
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         # Step 1: Extensive Search
         pop_new = []
         for idx in range(0, self.pop_size):
             # Eq.(4)
             pos_new = self.g_best[self.ID_POS] * np.random.rand() + ((self.problem.ub - self.problem.lb) * np.random.rand() + self.problem.lb) * \
-                      self.levy__(beta=1.5, size=self.problem.n_dims)
+                      self.get_levy_flight_step(beta=1.5, multiplier=0.01, size=self.problem.n_dims, case=-1)
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
                 self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
@@ -183,35 +174,27 @@
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
         self.set_parameters(["epoch", "pop_size"])
         self.sort_flag = True
 
-    def levy__(self, beta=1.0, size=None, step=0.01):
-        num = gamma(1 + beta) * np.sin(np.pi * beta/2)
-        den = gamma((1+beta)/2) * beta * 2**((beta-1)/2)
-        sigma_u = (num/den)**(1.0/beta)
-        u = np.random.normal(0, sigma_u, size=size)
-        v = np.random.normal(0, 1, size=size)
-        return u/(np.abs(v)**(1.0/beta)) * step
-
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         # Step 1: Extensive Search
         pop_new = []
         for idx in range(0, self.pop_size):
             # foraging movement patterns of giant trevallies are simulated using Eq.(4)
             pos_new = self.g_best[self.ID_POS] * np.random.rand() + ((self.problem.ub - self.problem.lb) * np.random.rand() + self.problem.lb) * \
-                      self.levy__(beta=1.5, size=self.problem.n_dims)
+                    self.get_levy_flight_step(beta=1.5, multiplier=0.01, size=self.problem.n_dims, case=-1)
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
                 self.pop[idx] = self.get_better_solution([pos_new, target], self.pop[idx])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
@@ -308,22 +291,14 @@
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
         self.set_parameters(["epoch", "pop_size"])
         self.sort_flag = True
 
-    def levy__(self, beta=1.0, size=None, step=0.01):
-        num = gamma(1 + beta) * np.sin(np.pi * beta/2)
-        den = gamma((1+beta)/2) * beta * 2**((beta-1)/2)
-        sigma_u = (num/den)**(1.0/beta)
-        u = np.random.normal(0, sigma_u, size=size)
-        v = np.random.normal(0, 1, size=size)
-        return u/(np.abs(v)**(1.0/beta)) * step
-
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
@@ -331,15 +306,15 @@
         for idx in range(0, self.pop_size):
             pop_new = []
             for jdx in range(0, self.pop_size):
                 if idx == jdx:
                     continue
                 # foraging movement patterns of giant trevallies are simulated using Eq.(4)
                 pos_new = self.g_best[self.ID_POS] * np.random.rand() + ((self.problem.ub - self.problem.lb) * np.random.rand() + self.problem.lb) * \
-                          self.levy__(beta=1.5, size=self.problem.n_dims)
+                          self.get_levy_flight_step(beta=1.5, multiplier=0.01, size=self.problem.n_dims, case=-1)
                 pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
                 pop_new.append([pos_new, None])
                 if self.mode not in self.AVAILABLE_MODES:
                     pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
             pop_new = self.update_target_wrapper_population(pop_new)
             _, self.pop[idx] = self.get_global_best_solution(pop_new + [self.pop[idx]])
         _, self.g_best = self.update_global_best_solution(self.pop, save=False)
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/GWO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/GWO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/HBA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/HBA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/HGS.py` & `mealpy-2.5.4a3/mealpy/swarm_based/HGS.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 15:37, 19/03/2021 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalHGS(Optimizer):
     """
     The original version of: Hunger Games Search (HGS)
 
@@ -118,15 +117,15 @@
 
         ## Eq. (2.4)
         shrink = 2 * (1 - (epoch + 1) / self.epoch)
         total_hunger = np.sum([pop[idx][self.ID_HUN] for idx in range(0, self.pop_size)])
 
         pop_new = []
         for idx in range(0, self.pop_size):
-            agent = deepcopy(self.pop[idx])
+            agent = self.pop[idx].copy()
             #### Variation control
             E = self.sech__(self.pop[idx][self.ID_TAR][self.ID_FIT] - g_best[self.ID_TAR][self.ID_FIT])
 
             # R is a ranging controller added to limit the range of activity, in which the range of R is gradually reduced to 0
             R = 2 * shrink * np.random.rand() - shrink  # Eq. (2.3)
 
             ## Calculate the hungry weight of each position
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/HHO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/HHO.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 14:51, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from math import gamma
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalHHO(Optimizer):
     """
     The original version of: Harris Hawks Optimization (HHO)
 
@@ -71,17 +69,16 @@
             E = 2 * E0 * (1 - (epoch + 1) * 1.0 / self.epoch)
             J = 2 * (1 - np.random.uniform())
 
             # -------- Exploration phase Eq. (1) in paper -------------------
             if np.abs(E) >= 1:
                 # Harris' hawks perch randomly based on 2 strategy:
                 if np.random.rand() >= 0.5:  # perch based on other family members
-                    X_rand = deepcopy(self.pop[np.random.randint(0, self.pop_size)][self.ID_POS])
+                    X_rand = self.pop[np.random.randint(0, self.pop_size)][self.ID_POS].copy()
                     pos_new = X_rand - np.random.uniform() * np.abs(X_rand - 2 * np.random.uniform() * self.pop[idx][self.ID_POS])
-
                 else:  # perch on a random tall tree (random site inside group's home range)
                     X_m = np.mean([x[self.ID_POS] for x in self.pop])
                     pos_new = (self.g_best[self.ID_POS] - X_m) - np.random.uniform() * \
                               (self.problem.lb + np.random.uniform() * (self.problem.ub - self.problem.lb))
                 pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
                 pop_new.append([pos_new, None])
             # -------- Exploitation phase -------------------
@@ -94,17 +91,15 @@
                     if np.abs(E) >= 0.5:  # Hard besiege Eq. (6) in paper
                         pos_new = delta_X - E * np.abs(J * self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
                     else:  # Soft besiege Eq. (4) in paper
                         pos_new = self.g_best[self.ID_POS] - E * np.abs(delta_X)
                     pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
                     pop_new.append([pos_new, None])
                 else:
-                    xichma = np.power((gamma(1 + 1.5) * np.sin(np.pi * 1.5 / 2.0)) /
-                                      (gamma((1 + 1.5) * 1.5 * np.power(2, (1.5 - 1) / 2)) / 2.0), 1.0 / 1.5)
-                    LF_D = 0.01 * np.random.uniform() * xichma / np.power(np.abs(np.random.uniform()), 1.0 / 1.5)
+                    LF_D = self.get_levy_flight_step(beta=1.5, multiplier=0.01, case=-1)
                     if np.abs(E) >= 0.5:  # Soft besiege Eq. (10) in paper
                         Y = self.g_best[self.ID_POS] - E * np.abs(J * self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
                     else:  # Hard besiege Eq. (11) in paper
                         X_m = np.mean([x[self.ID_POS] for x in self.pop])
                         Y = self.g_best[self.ID_POS] - E * np.abs(J * self.g_best[self.ID_POS] - X_m)
                     pos_Y = self.amend_position(Y, self.problem.lb, self.problem.ub)
                     target_Y = self.get_target_wrapper(pos_Y)
@@ -113,14 +108,14 @@
                     target_Z = self.get_target_wrapper(pos_Z)
                     if self.compare_agent([pos_Y, target_Y], self.pop[idx]):
                         pop_new.append([pos_Y, target_Y])
                         continue
                     if self.compare_agent([pos_Z, target_Z], self.pop[idx]):
                         pop_new.append([pos_Z, target_Z])
                         continue
-                    pop_new.append(deepcopy(self.pop[idx]))
+                    pop_new.append(self.pop[idx].copy())
         if self.mode not in self.AVAILABLE_MODES:
             for idx, agent in enumerate(pop_new):
                 pop_new[idx][self.ID_TAR] = self.get_target_wrapper(agent[self.ID_POS])
         else:
             pop_new = self.update_target_wrapper_population(pop_new)
         self.pop = self.greedy_selection_population(self.pop, pop_new)
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/JA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/JA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/MFO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/MFO.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 11:59, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseMFO(Optimizer):
     """
     The developed version: Moth-Flame Optimization (MFO)
 
@@ -62,37 +61,30 @@
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         # Number of flames Eq.(3.14) in the paper (linearly decreased)
         num_flame = round(self.pop_size - (epoch + 1) * ((self.pop_size - 1) / self.epoch))
-
         # a linearly decreases from -1 to -2 to calculate t in Eq. (3.12)
         a = -1 + (epoch + 1) * ((-1) / self.epoch)
-
         pop_flames, g_best = self.get_global_best_solution(self.pop)
-
         pop_new = []
         for idx in range(0, self.pop_size):
             #   D in Eq.(3.13)
             distance_to_flame = np.abs(pop_flames[idx][self.ID_POS] - self.pop[idx][self.ID_POS])
             t = (a - 1) * np.random.uniform(0, 1, self.problem.n_dims) + 1
             b = 1
-
             # Update the position of the moth with respect to its corresponding flame, Eq.(3.12).
             temp_1 = distance_to_flame * np.exp(b * t) * np.cos(t * 2 * np.pi) + pop_flames[idx][self.ID_POS]
-
             # Update the position of the moth with respect to one flame Eq.(3.12).
             ## Here is a changed, I used the best position of flames not the position num_flame th (as original code)
             temp_2 = distance_to_flame * np.exp(b * t) * np.cos(t * 2 * np.pi) + g_best[self.ID_POS]
-
             list_idx = idx * np.ones(self.problem.n_dims)
             pos_new = np.where(list_idx < num_flame, temp_1, temp_2)
-
             ## This is the way I make this algorithm working. I tried to run matlab code with large dimension and it doesn't convergence.
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
                 self.pop[idx] = self.get_better_solution(self.pop[idx], [pos_new, target])
         if self.mode in self.AVAILABLE_MODES:
@@ -147,23 +139,20 @@
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         # Number of flames Eq.(3.14) in the paper (linearly decreased)
         num_flame = round(self.pop_size - (epoch + 1) * ((self.pop_size - 1) / self.epoch))
-
         # a linearly decreases from -1 to -2 to calculate t in Eq. (3.12)
         a = -1 + (epoch + 1) * ((-1) / self.epoch)
-
         pop_flames, g_best = self.get_global_best_solution(self.pop)
-
         pop_new = []
         for idx in range(0, self.pop_size):
-            pos_new = deepcopy(self.pop[idx][self.ID_POS])
+            pos_new = self.pop[idx][self.ID_POS].copy()
             for j in range(self.problem.n_dims):
                 #   D in Eq.(3.13)
                 distance_to_flame = np.abs(pop_flames[idx][self.ID_POS][j] - self.pop[idx][self.ID_POS][j])
                 t = (a - 1) * np.random.uniform() + 1
                 b = 1
                 if idx <= num_flame:  # Update the position of the moth with respect to its corresponding flame
                     # Eq.(3.12)
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/MGO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/MGO.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 
             # Update the location
             x2 = self.g_best[self.ID_POS] - np.abs((np.random.randint(1, 3)*M - np.random.randint(1, 3)*self.pop[idx][self.ID_POS]) * A) * cofi[np.random.randint(0, 4), :]
             x3 = M + cofi[np.random.randint(0, 4), :] + (np.random.randint(1, 3)*self.g_best[self.ID_POS] - np.random.randint(1, 3)*self.pop[np.random.randint(self.pop_size)][self.ID_POS])*cofi[np.random.randint(0, 4), :]
             x4 = self.pop[idx][self.ID_POS] - D + (np.random.randint(1, 3)*self.g_best[self.ID_POS] - np.random.randint(1, 3)*M) * cofi[np.random.randint(0, 4), :]
 
             x1 = self.generate_position(self.problem.lb, self.problem.ub)
+            x1 = self.amend_position(x1, self.problem.lb, self.problem.ub)
             x2 = self.amend_position(x2, self.problem.lb, self.problem.ub)
             x3 = self.amend_position(x3, self.problem.lb, self.problem.ub)
             x4 = self.amend_position(x4, self.problem.lb, self.problem.ub)
 
             pop_new += [[x1, None], [x2, None], [x3, None], [x4, None]]
             if self.mode not in self.AVAILABLE_MODES:
                 for jdx in range(-4, 0):
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/MPA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/MPA.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,32 +61,24 @@
         self.set_parameters(["epoch", "pop_size"])
         self.sort_flag = False
 
     def initialize_variables(self):
         self.FADS = 0.2
         self.P = 0.5
 
-    def levy_step(self, beta, size=None):
-        num = np.random.gamma(1 + beta) * np.sin(np.pi * beta /2)
-        den = np.random.gamma((1+beta)/2) * beta * 2**((beta-1)/2)
-        sigma_u = (num/den) ** (1 / beta)
-        u = np.random.normal(0, sigma_u, size)
-        v = np.random.normal(0, 1, size)
-        return u / np.abs(v)**(1/beta)
-
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         CF = (1 - (epoch+1)/self.epoch)**(2 * (epoch+1)/self.epoch)
         # RL = self.get_levy_flight_step(beta=1.5, multiplier=0.05, size=(self.pop_size, self.problem.n_dims), case=-1)
-        RL = 0.05 * self.levy_step(1.5, (self.pop_size, self.problem.n_dims))
+        RL = self.get_levy_flight_step(beta=1.5, multiplier=0.05, size=(self.pop_size, self.problem.n_dims), case=-1)
         RB = np.random.randn(self.pop_size, self.problem.n_dims)
         per1 = np.random.permutation(self.pop_size)
         per2 = np.random.permutation(self.pop_size)
         pop_new = []
         for idx in range(0, self.pop_size):
             R = np.random.rand(self.problem.n_dims)
             t = self.epoch + 1
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/MRFO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/MRFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/MSA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/MSA.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Created by "Thieu" at 14:52, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
 from math import gamma
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalMSA(Optimizer):
     """
     The original version: Moth Search Algorithm (MSA)
 
@@ -94,16 +93,15 @@
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
-        pop_best = deepcopy(self.pop[:self.n_best])
-
+        pop_best = self.pop[:self.n_best].copy()
         pop_new = []
         for idx in range(0, self.pop_size):
             # Migration operator
             if idx < self.n_moth1:
                 # scale = self.max_step_size / (epoch+1)       # Smaller step for local walk
                 pos_new = self.pop[idx][self.ID_POS] + np.random.normal() * self._levy_walk(epoch)
             else:
@@ -120,8 +118,8 @@
                 self.pop[idx] = self.get_better_solution(self.pop[idx], [pos_new, target])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop = self.greedy_selection_population(self.pop, pop_new)
         self.pop, _ = self.get_global_best_solution(self.pop)
         # Replace the worst with the previous generation's elites.
         for i in range(0, self.n_best):
-            self.pop[-1 - i] = deepcopy(pop_best[i])
+            self.pop[-1 - i] = pop_best[i].copy()
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/NGO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/NGO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/NMRA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/NMRA.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 14:52, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalNMRA(Optimizer):
     """
     The original version of: Naked Mole-Rat Algorithm (NMRA)
 
@@ -67,15 +66,15 @@
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         pop_new = []
         for idx in range(0, self.pop_size):
-            pos_new = deepcopy(self.pop[idx][self.ID_POS])
+            pos_new = self.pop[idx][self.ID_POS].copy()
             if idx < self.size_b:  # breeding operators
                 if np.random.uniform() < self.pb:
                     alpha = np.random.uniform()
                     pos_new = (1 - alpha) * self.pop[idx][self.ID_POS] + alpha * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
             else:  # working operators
                 t1, t2 = np.random.choice(range(self.size_b, self.pop_size), 2, replace=False)
                 pos_new = self.pop[idx][self.ID_POS] + np.random.uniform() * (self.pop[t1][self.ID_POS] - self.pop[t2][self.ID_POS])
@@ -151,15 +150,15 @@
     def crossover_random__(self, pop, g_best):
         start_point = np.random.randint(0, self.problem.n_dims / 2)
         id1 = start_point
         id2 = int(start_point + self.problem.n_dims / 3)
         id3 = int(self.problem.n_dims)
 
         partner = pop[np.random.randint(0, self.pop_size)][self.ID_POS]
-        new_temp = deepcopy(g_best[self.ID_POS])
+        new_temp = g_best[self.ID_POS].copy()
         new_temp[0:id1] = g_best[self.ID_POS][0:id1]
         new_temp[id1:id2] = partner[id1:id2]
         new_temp[id2:id3] = g_best[self.ID_POS][id2:id3]
         return new_temp
 
     def evolve(self, epoch):
         """
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/OOA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/OOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/PFA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/PFA.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 14:51, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalPFA(Optimizer):
     """
     The original version of: Pathfinder Algorithm (PFA)
 
@@ -71,16 +70,16 @@
         pos_new = self.pop[0][self.ID_POS] + 2 * np.random.uniform() * (self.g_best[self.ID_POS] - self.pop[0][self.ID_POS]) + A
         pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
         target = self.get_target_wrapper(pos_new)
         pop_new = [[pos_new, target], ]
 
         ## Update positions of members, check the bound and calculate new fitness
         for idx in range(1, self.pop_size):
-            agent = deepcopy(self.pop[idx])
-            pos_new = deepcopy(self.pop[idx][self.ID_POS]).astype(float)
+            agent = self.pop[idx].copy()
+            pos_new = self.pop[idx][self.ID_POS].copy().astype(float)
             for k in range(1, self.pop_size):
                 dist = np.sqrt(np.sum((self.pop[k][self.ID_POS] - self.pop[idx][self.ID_POS]) ** 2)) / self.problem.n_dims
                 t2 = alpha * np.random.uniform() * (self.pop[k][self.ID_POS] - self.pop[idx][self.ID_POS])
                 ## First stabilize the distance
                 t3 = np.random.uniform() * t * (dist / space)
                 pos_new += t2 + t3
             ## Second stabilize the population size
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/POA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/POA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/PSO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/PSO.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 09:49, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalPSO(Optimizer):
     """
     The original version of: Particle Swarm Optimization (PSO)
 
@@ -87,16 +86,16 @@
             list: wrapper of solution with format [position, target, velocity, local_pos, local_fit]
         """
         if pos is None:
             pos = self.generate_position(lb, ub)
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         velocity = np.random.uniform(self.v_min, self.v_max)
-        local_pos = deepcopy(position)
-        local_fit = deepcopy(target)
+        local_pos = position.copy()
+        local_fit = target.copy()
         return [position, target, velocity, local_pos, local_fit]
 
     def bounded_position(self, position=None, lb=None, ub=None):
         condition = np.logical_and(lb <= position, position <= ub)
         pos_rand = np.random.uniform(lb, ub)
         return np.where(condition, position, pos_rand)
 
@@ -107,15 +106,15 @@
         Args:
             epoch (int): The current iteration
         """
         # Update weight after each move count  (weight down)
         w = (self.epoch - epoch) / self.epoch * (self.w_max - self.w_min) + self.w_min
         pop_new = []
         for idx in range(0, self.pop_size):
-            agent = deepcopy(self.pop[idx])
+            agent = self.pop[idx].copy()
             v_new = w * self.pop[idx][self.ID_VEC] + self.c1 * np.random.rand() * (self.pop[idx][self.ID_LOP] - self.pop[idx][self.ID_POS]) + \
                     self.c2 * np.random.rand() * (self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
             x_new = self.pop[idx][self.ID_POS] + v_new  # Xi(new) = Xi(old) + Vi(new) * deltaT (deltaT = 1)
             pos_new = self.amend_position(x_new, self.problem.lb, self.problem.ub)
             agent[self.ID_POS] = pos_new
             agent[self.ID_VEC] = v_new
             pop_new.append(agent)
@@ -123,18 +122,18 @@
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
 
         # Update current position, current velocity and compare with past position, past fitness (local best)
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
                 if self.compare_agent(pop_new[idx], [None, self.pop[idx][self.ID_LOF]]):
-                    self.pop[idx][self.ID_LOP] = deepcopy(pop_new[idx][self.ID_POS])
-                    self.pop[idx][self.ID_LOF] = deepcopy(pop_new[idx][self.ID_TAR])
+                    self.pop[idx][self.ID_LOP] = pop_new[idx][self.ID_POS].copy()
+                    self.pop[idx][self.ID_LOF] = pop_new[idx][self.ID_TAR].copy()
 
 
 class PPSO(Optimizer):
     """
     The original version of: Phasor Particle Swarm Optimization (P-PSO)
 
     Examples
@@ -193,36 +192,36 @@
             list: wrapper of solution with format [position, target, velocity, local_pos, local_fit]
         """
         if pos is None:
             pos = self.generate_position(lb, ub)
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         velocity = np.random.uniform(self.v_min, self.v_max)
-        local_pos = deepcopy(position)
-        local_fit = deepcopy(target)
+        local_pos = position.copy()
+        local_fit = target.copy()
         return [position, target, velocity, local_pos, local_fit]
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         pop_new = []
         for i in range(0, self.pop_size):
-            agent = deepcopy(self.pop[i])
+            agent = self.pop[i].copy()
             aa = 2 * (np.sin(self.dyn_delta_list[i]))
             bb = 2 * (np.cos(self.dyn_delta_list[i]))
             ee = np.abs(np.cos(self.dyn_delta_list[i])) ** aa
             tt = np.abs(np.sin(self.dyn_delta_list[i])) ** bb
 
             v_new = ee * (self.pop[i][self.ID_LOP] - self.pop[i][self.ID_POS]) + tt * (self.g_best[self.ID_POS] - self.pop[i][self.ID_POS])
             v_new = np.minimum(np.maximum(v_new, -self.v_max), self.v_max)
-            agent[self.ID_VEC] = deepcopy(v_new)
+            agent[self.ID_VEC] = v_new.copy()
 
             pos_new = self.pop[i][self.ID_POS] + v_new
             agent[self.ID_POS] = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
 
             self.dyn_delta_list[i] += np.abs(aa + bb) * (2 * np.pi)
             self.v_max = (np.abs(np.cos(self.dyn_delta_list[i])) ** 2) * (self.problem.ub - self.problem.lb)
             pop_new.append(agent)
@@ -230,18 +229,18 @@
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(agent[self.ID_POS])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
 
         # Update current position, current velocity and compare with past position, past fitness (local best)
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
                 if self.compare_agent(pop_new[idx], [None, self.pop[idx][self.ID_LOF]]):
-                    self.pop[idx][self.ID_LOP] = deepcopy(pop_new[idx][self.ID_POS])
-                    self.pop[idx][self.ID_LOF] = deepcopy(pop_new[idx][self.ID_TAR])
+                    self.pop[idx][self.ID_LOP] = pop_new[idx][self.ID_POS].copy()
+                    self.pop[idx][self.ID_LOF] = pop_new[idx][self.ID_TAR].copy()
 
 
 class HPSO_TVAC(PPSO):
     """
     The original version of: Hierarchical PSO Time-Varying Acceleration (HPSO-TVAC)
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
@@ -299,15 +298,15 @@
 
         Args:
             epoch (int): The current iteration
         """
         c_it = ((self.cf - self.ci) * ((epoch + 1) / self.epoch)) + self.ci
         pop_new = []
         for i in range(0, self.pop_size):
-            agent = deepcopy(self.pop[i])
+            agent = self.pop[i].copy()
             idx_k = np.random.randint(0, self.pop_size)
             w = np.random.normal()
             while np.abs(w - 1.0) < 0.01:
                 w = np.random.normal()
             c1_it = np.abs(w) ** (c_it * w)
             c2_it = np.abs(1 - w) ** (c_it / (1 - w))
 
@@ -331,18 +330,18 @@
         # Update fitness for all solutions
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
 
         # Update current position, current velocity and compare with past position, past fitness (local best)
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
                 if self.compare_agent(pop_new[idx], [None, self.pop[idx][self.ID_LOF]]):
-                    self.pop[idx][self.ID_LOP] = deepcopy(pop_new[idx][self.ID_POS])
-                    self.pop[idx][self.ID_LOF] = deepcopy(pop_new[idx][self.ID_TAR])
+                    self.pop[idx][self.ID_LOP] = pop_new[idx][self.ID_POS].copy()
+                    self.pop[idx][self.ID_LOF] = pop_new[idx][self.ID_TAR].copy()
 
 
 class C_PSO(OriginalPSO):
     """
     The original version of: Chaos Particle Swarm Optimization (C-PSO)
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
@@ -402,16 +401,16 @@
         self.set_parameters(["epoch", "pop_size", "c1", "c2", "w_min", "w_max"])
         self.sort_flag = False
     
     def initialize_variables(self):
         self.v_max = 0.5 * (self.problem.ub - self.problem.lb)
         self.v_min = -self.v_max
         self.N_CLS = int(self.pop_size / 5)  # Number of chaotic local searches
-        self.dyn_lb = deepcopy(self.problem.lb)
-        self.dyn_ub = deepcopy(self.problem.ub)
+        self.dyn_lb = self.problem.lb.copy()
+        self.dyn_ub = self.problem.ub.copy()
 
     def get_weights__(self, fit, fit_avg, fit_min):
         temp1 = self.w_min + (self.w_max - self.w_min) * (fit - fit_min) / (fit_avg - fit_min)
         if self.problem.minmax == "min":
             output = temp1 if fit <= fit_avg else self.w_max
         else:
             output = self.w_max if fit <= fit_avg else temp1
@@ -425,15 +424,15 @@
             epoch (int): The current iteration
         """
         list_fits = [item[self.ID_TAR][self.ID_FIT] for item in self.pop]
         fit_avg = np.mean(list_fits)
         fit_min = np.min(list_fits)
         pop_new = []
         for i in range(self.pop_size):
-            agent = deepcopy(self.pop[i])
+            agent = self.pop[i].copy()
             w = self.get_weights__(self.pop[i][self.ID_TAR][self.ID_FIT], fit_avg, fit_min)
             v_new = w * self.pop[i][self.ID_VEC] + self.c1 * np.random.rand() * (self.pop[i][self.ID_LOP] - self.pop[i][self.ID_POS]) + \
                     self.c2 * np.random.rand() * (self.g_best[self.ID_POS] - self.pop[i][self.ID_POS])
             v_new = np.clip(v_new, self.v_min, self.v_max)
             x_new = self.pop[i][self.ID_POS].astype(float) + v_new
             agent[self.ID_VEC] = v_new
             pos_new = self.amend_position(x_new, self.dyn_lb, self.dyn_ub)
@@ -443,18 +442,18 @@
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
 
         # Update current position, current velocity and compare with past position, past fitness (local best)
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
                 if self.compare_agent(pop_new[idx], [None, self.pop[idx][self.ID_LOF]]):
-                    self.pop[idx][self.ID_LOP] = deepcopy(pop_new[idx][self.ID_POS])
-                    self.pop[idx][self.ID_LOF] = deepcopy(pop_new[idx][self.ID_TAR])
+                    self.pop[idx][self.ID_LOP] = pop_new[idx][self.ID_POS].copy()
+                    self.pop[idx][self.ID_LOF] = pop_new[idx][self.ID_TAR].copy()
 
         ## Implement chaostic local search for the best solution
         g_best = self.g_best
         cx_best_0 = (self.g_best[self.ID_POS] - self.problem.lb) / (self.problem.ub - self.problem.lb)  # Eq. 7
         cx_best_1 = 4 * cx_best_0 * (1 - cx_best_0)  # Eq. 6
         x_best = self.problem.lb + cx_best_1 * (self.problem.ub - self.problem.lb)  # Eq. 8
         x_best = self.amend_position(x_best, self.problem.lb, self.problem.ub)
@@ -550,36 +549,34 @@
             list: wrapper of solution with format [position, target, velocity, local_pos, local_fit]
         """
         if pos is None:
             pos = self.generate_position(lb, ub)
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         velocity = np.random.uniform(self.v_min, self.v_max)
-        local_pos = deepcopy(position)
-        local_fit = deepcopy(target)
+        local_pos = position.copy()
+        local_fit = target.copy()
         return [position, target, velocity, local_pos, local_fit]
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         wk = self.w_max * (epoch / self.epoch) * (self.w_max - self.w_min)
         pop_new = []
         for i in range(0, self.pop_size):
-            agent = deepcopy(self.pop[i])
+            agent = self.pop[i].copy()
             if self.flags[i] >= self.max_flag:
                 self.flags[i] = 0
                 agent = self.create_solution(self.problem.lb, self.problem.ub)
-
             pci = 0.05 + 0.45 * (np.exp(10 * (i + 1) / self.pop_size) - 1) / (np.exp(10) - 1)
-
-            vec_new = deepcopy(self.pop[i][self.ID_VEC])
+            vec_new = self.pop[i][self.ID_VEC].copy()
             for j in range(0, self.problem.n_dims):
                 if np.random.rand() > pci:
                     vj = wk * self.pop[i][self.ID_VEC][j] + self.c_local * np.random.rand() * \
                          (self.pop[i][self.ID_LOP][j] - self.pop[i][self.ID_POS][j])
                 else:
                     id1, id2 = np.random.choice(list(set(range(0, self.pop_size)) - {i}), 2, replace=False)
                     if self.compare_agent(self.pop[id1], self.pop[id2]):
@@ -599,14 +596,14 @@
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
 
         # Update current position, current velocity and compare with past position, past fitness (local best)
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
                 if self.compare_agent(pop_new[idx], [None, self.pop[idx][self.ID_LOF]]):
-                    self.pop[idx][self.ID_LOP] = deepcopy(pop_new[idx][self.ID_POS])
-                    self.pop[idx][self.ID_LOF] = deepcopy(pop_new[idx][self.ID_TAR])
+                    self.pop[idx][self.ID_LOP] = pop_new[idx][self.ID_POS].copy()
+                    self.pop[idx][self.ID_LOF] = pop_new[idx][self.ID_TAR].copy()
                     self.flags[idx] = 0
                 else:
                     self.flags[idx] += 1
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/SCSO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/SCSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/SFO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/SFO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 14:51, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalSFO(Optimizer):
     """
     The original version of: SailFish Optimizer (SFO)
 
@@ -96,47 +95,45 @@
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
                 self.pop[idx] = self.get_better_solution(self.pop[idx], [pos_new, target])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop = self.greedy_selection_population(self.pop, pop_new)
-
         ## Calculate AttackPower using Eq.(10)
         AP = self.AP * (1 - 2 * (epoch + 1) * self.epsilon)
         if AP < 0.5:
             alpha = int(self.s_size * np.abs(AP))
             beta = int(self.problem.n_dims * np.abs(AP))
             ### Random np.random.choice number of sardines which will be updated their position
             list1 = np.random.choice(range(0, self.s_size), alpha)
             for i in range(0, self.s_size):
                 if i in list1:
                     #### Random np.random.choice number of dimensions in sardines updated, remove third loop by numpy vector computation
-                    pos_new = deepcopy(self.s_pop[i][self.ID_POS])
+                    pos_new = self.s_pop[i][self.ID_POS].copy()
                     list2 = np.random.choice(range(0, self.problem.n_dims), beta, replace=False)
                     pos_new[list2] = (np.random.uniform(0, 1, self.problem.n_dims) *
                                       (self.pop[self.ID_POS] - self.s_pop[i][self.ID_POS] + AP))[list2]
                     pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
                     self.s_pop[i] = [pos_new, None]
         else:
             ### Update the position of all sardine using Eq.(9)
             for i in range(0, self.s_size):
                 pos_new = np.random.uniform() * (self.g_best[self.ID_POS] - self.s_pop[i][self.ID_POS] + AP)
                 self.s_pop[i][self.ID_POS] = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
         ## Recalculate the fitness of all sardine
         self.s_pop = self.update_target_wrapper_population(self.s_pop)
-
         ## Sort the population of sailfish and sardine (for reducing computational cost)
         self.pop, g_best = self.get_global_best_solution(self.pop)
         self.s_pop, s_gbest = self.get_global_best_solution(self.s_pop)
         for i in range(0, self.pop_size):
             for j in range(0, self.s_size):
                 ### If there is a better position in sardine population.
                 if self.compare_agent(self.s_pop[j], self.pop[i]):
-                    self.pop[i] = deepcopy(self.s_pop[j])
+                    self.pop[i] = self.s_pop[j].copy()
                     del self.s_pop[j]
                 break  #### This simple keyword helped reducing ton of comparing operation.
                 #### Especially when sardine pop size >> sailfish pop size
         temp = self.s_size - len(self.s_pop)
         if temp == 1:
             self.s_pop = self.s_pop + [self.create_solution(self.problem.lb, self.problem.ub)]
         else:
@@ -225,15 +222,14 @@
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 target = self.get_target_wrapper(pos_new)
                 self.pop[idx] = self.get_better_solution(self.pop[idx], [pos_new, target])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop = self.greedy_selection_population(self.pop, pop_new)
-
         ## ## Calculate AttackPower using my Eq.thieu
         #### This is our proposed, simple but effective, no need A and epsilon parameters
         AP = 1 - epoch * 1.0 / self.epoch
         if AP < 0.5:
             for i in range(0, len(self.s_pop)):
                 temp = (self.g_best[self.ID_POS] + AP) / 2
                 pos_new = self.problem.lb + self.problem.ub - temp + np.random.uniform() * (temp - self.s_pop[i][self.ID_POS])
@@ -241,22 +237,20 @@
         else:
             ### Update the position of all sardine using Eq.(9)
             for i in range(0, len(self.s_pop)):
                 pos_new = np.random.uniform() * (self.g_best[self.ID_POS] - self.s_pop[i][self.ID_POS] + AP)
                 self.s_pop[i][self.ID_POS] = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
         ## Recalculate the fitness of all sardine
         self.s_pop = self.update_target_wrapper_population(self.s_pop)
-
         ## Sort the population of sailfish and sardine (for reducing computational cost)
         self.pop = self.get_sorted_strim_population(self.pop, self.pop_size)
         self.s_pop = self.get_sorted_strim_population(self.s_pop, len(self.s_pop))
         for i in range(0, self.pop_size):
             for j in range(0, len(self.s_pop)):
                 ### If there is a better position in sardine population.
                 if self.compare_agent(self.s_pop[j], self.pop[i]):
-                    self.pop[i] = deepcopy(self.s_pop[j])
+                    self.pop[i] = self.s_pop[j].copy()
                     del self.s_pop[j]
                 break  #### This simple keyword helped reducing ton of comparing operation.
                 #### Especially when sardine pop size >> sailfish pop size
-
         self.s_pop = self.s_pop + self.create_population(self.s_size - len(self.s_pop))
         _, self.s_gbest = self.get_global_best_solution(self.s_pop)
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/SHO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/SHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/SLO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/SLO.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Created by "Thieu" at 15:05, 03/06/2021 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
 from math import gamma
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalSLO(Optimizer):
     """
     The original version of: Sea Lion Optimization Algorithm (SLO)
 
@@ -193,15 +192,15 @@
             pa = 0.3  # At the beginning of the process, the probability for shrinking encircling is small
         else:
             pa = 0.7  # But at the end of the process, it become larger. Because sea lion are shrinking encircling prey
         SP_leader = np.random.uniform(0, 1)
 
         pop_new = []
         for idx in range(0, self.pop_size):
-            agent = deepcopy(self.pop[idx])
+            agent = self.pop[idx].copy()
             if SP_leader >= 0.6:
                 pos_new = np.cos(2 * np.pi * np.random.normal(0, 1)) * \
                           np.abs(self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS]) + self.g_best[self.ID_POS]
             else:
                 if np.random.uniform() < pa:
                     dist1 = np.random.uniform() * np.abs(2 * self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
                     pos_new = self.shrink_encircling_levy__(self.pop[idx][self.ID_POS], epoch, dist1, c)
@@ -213,18 +212,18 @@
             pop_new.append(agent)
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(agent[self.ID_POS])
         pop_new = self.update_target_wrapper_population(pop_new)
 
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
                 if self.compare_agent(pop_new[idx], [None, self.pop[idx][self.ID_LOC_FIT]]):
-                    self.pop[idx][self.ID_LOC_POS] = deepcopy(pop_new[idx][self.ID_POS])
-                    self.pop[idx][self.ID_LOC_FIT] = deepcopy(pop_new[idx][self.ID_TAR])
+                    self.pop[idx][self.ID_LOC_POS] = pop_new[idx][self.ID_POS].copy()
+                    self.pop[idx][self.ID_LOC_FIT] = pop_new[idx][self.ID_TAR].copy()
 
 
 class ImprovedSLO(ModifiedSLO):
     """
     The original version: Improved Sea Lion Optimization (ImprovedSLO)
 
     Hyper-parameters should fine-tune in approximate range to get faster convergence toward the global optimum:
@@ -282,15 +281,15 @@
         t0 = np.random.rand()
         v1 = np.sin(2 * np.pi * t0)
         v2 = np.sin(2 * np.pi * (1 - t0))
         SP_leader = np.abs(v1 * (1 + v2) / v2)
 
         pop_new = []
         for idx in range(0, self.pop_size):
-            agent = deepcopy(self.pop[idx])
+            agent = self.pop[idx].copy()
             if SP_leader < 0.5:
                 if c < 1:  # Exploitation improved by historical movement + global best affect
                     # pos_new = g_best[self.ID_POS] - c * np.abs(2 * rand() * g_best[self.ID_POS] - pop[i][self.ID_POS])
                     dif1 = np.abs(2 * np.random.rand() * self.g_best[self.ID_POS] - self.pop[idx][self.ID_POS])
                     dif2 = np.abs(2 * np.random.rand() * self.pop[idx][self.ID_LOC_POS] - self.pop[idx][self.ID_POS])
                     pos_new = self.c1 * np.random.rand() * (self.pop[idx][self.ID_POS] - dif1) + \
                               self.c2 * np.random.rand() * (self.pop[idx][self.ID_POS] - dif2)
@@ -314,11 +313,11 @@
             pop_new.append(agent)
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(agent[self.ID_POS])
         pop_new = self.update_target_wrapper_population(pop_new)
 
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
                 if self.compare_agent(pop_new[idx], [None, self.pop[idx][self.ID_LOC_FIT]]):
-                    self.pop[idx][self.ID_LOC_POS] = deepcopy(pop_new[idx][self.ID_POS])
-                    self.pop[idx][self.ID_LOC_FIT] = deepcopy(pop_new[idx][self.ID_TAR])
+                    self.pop[idx][self.ID_LOC_POS] = pop_new[idx][self.ID_POS].copy()
+                    self.pop[idx][self.ID_LOC_FIT] = pop_new[idx][self.ID_TAR].copy()
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/SRSR.py` & `mealpy-2.5.4a3/mealpy/swarm_based/SRSR.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 14:51, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalSRSR(Optimizer):
     """
     The original version of: Swarm Robotics Search And Rescue (SRSR)
 
@@ -72,16 +71,16 @@
         """
         if pos is None:
             pos = self.generate_position(lb, ub)
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         mu = 0
         sigma = 0
-        x_new = deepcopy(position)
-        target_new = deepcopy(target)
+        x_new = position.copy()
+        target_new = target.copy()
         target_move = 0
         return [position, target, mu, sigma, x_new, target_new, target_move]
 
     def initialize_variables(self):
         # Control Parameters Of Algorithm
         # ==============================================================================================
         #  [c1] movement_factor : Determines Movement Pace Of Robots During Exploration Policy
@@ -110,44 +109,43 @@
         if epoch % 2 == 1:
             self.pop[0][self.ID_MU] = (1 - self.pop[0][self.ID_SIGMA]) * self.pop[0][self.ID_POS]
         else:
             self.pop[0][self.ID_MU] = (1 + (1 - self.mu_factor) * self.pop[0][self.ID_SIGMA]) * self.pop[0][self.ID_POS]
 
         pop_new = []
         for i in range(0, self.pop_size):
-            agent = deepcopy(self.pop[i])
+            agent = self.pop[i].copy()
             # ---------- CALCULATING MU AND SIGMA FOR SLAVE ROBOTS ---------
             self.pop[i][self.ID_MU] = self.mu_factor * self.pop[0][self.ID_POS] + (1 - self.mu_factor) * self.pop[i][self.ID_POS]
             if epoch == 0:
                 self.SIF = 6
             self.sigma_temp[i] = self.SIF * np.random.uniform()
             self.pop[i][self.ID_SIGMA] = self.sigma_temp[i] * np.abs(self.pop[0][self.ID_POS] - self.pop[i][self.ID_POS]) + \
                                          np.random.uniform() ** 2 * ((self.pop[0][self.ID_POS] - self.pop[i][self.ID_POS]) < 0.05)
-
             # ----- Generating New Positions Using New Obtained Mu And Sigma Values --------------
             pos_new = np.random.normal(self.pop[i][self.ID_MU], self.pop[i][self.ID_SIGMA], self.problem.n_dims)
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             agent[self.ID_POS] = pos_new
             pop_new.append(agent)
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_new = self.update_target_wrapper_population(pop_new)
 
         for idx in range(0, self.pop_size):
             # --------- Calculate Degree Of Cost Movement Of Robots During Movement --------------
             self.pop[idx][self.ID_FIT_MOVE] = self.pop[idx][self.ID_TAR][self.ID_FIT] - self.pop[idx][self.ID_FIT_NEW][self.ID_FIT]
 
-            self.pop[idx][self.ID_POS_NEW] = deepcopy(pop_new[idx][self.ID_POS])
-            self.pop[idx][self.ID_FIT_NEW] = deepcopy(pop_new[idx][self.ID_TAR])
+            self.pop[idx][self.ID_POS_NEW] = pop_new[idx][self.ID_POS].copy()
+            self.pop[idx][self.ID_FIT_NEW] = pop_new[idx][self.ID_TAR].copy()
 
             # ---------- Progress Assessment: Replacing More Quality Solutions With Previous Ones ------
             # Replace Solution If It Reached To A More Quality Position
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx][self.ID_POS] = deepcopy(pop_new[idx][self.ID_POS])
-                self.pop[idx][self.ID_TAR] = deepcopy(pop_new[idx][self.ID_TAR])
+                self.pop[idx][self.ID_POS] = pop_new[idx][self.ID_POS].copy()
+                self.pop[idx][self.ID_TAR] = pop_new[idx][self.ID_TAR].copy()
 
         # --------- Determining Sigma Improvement Factor (Sif) Based On Vvss Movement -------------------
         ## Get best improved fitness
         fit_id = np.argmax([item[self.ID_FIT_MOVE] for item in self.pop])
         sigma_factor = 1 + np.random.uniform() * np.max(self.problem.ub - self.problem.lb)
         self.SIF = sigma_factor * self.sigma_temp[fit_id]
         # Controlling Parameter Of Algorithm
@@ -155,15 +153,15 @@
             self.SIF = np.max(self.problem.ub) * np.random.uniform()
 
         # ========================================================================================= %%
         #            Phase 2 (Exploration): Moving Slave Robots Toward Master Robot                   %
         # ===========================================================================================%%
         pop_new = []
         for i in range(0, self.pop_size):
-            agent = deepcopy(self.pop[i])
+            agent = self.pop[i].copy()
             gb = np.random.uniform(-1, 1, self.problem.n_dims)
             gb[gb >= 0] = 1
             gb[gb < 0] = -1
             pos_new = self.pop[i][self.ID_POS] * np.random.uniform() + gb * (self.pop[0][self.ID_POS] - self.pop[i][self.ID_POS]) + \
                    self.movement_factor * np.random.uniform(self.problem.lb, self.problem.ub)
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             agent[self.ID_POS] = pos_new
@@ -172,35 +170,35 @@
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_new = self.update_target_wrapper_population(pop_new)
 
         for idx in range(0, self.pop_size):
             # --------- Calculate Degree Of Cost Movement Of Robots During Movement --------------
             self.pop[idx][self.ID_FIT_MOVE] = self.pop[idx][self.ID_TAR][self.ID_FIT] - self.pop[idx][self.ID_FIT_NEW][self.ID_FIT]
 
-            self.pop[idx][self.ID_POS_NEW] = deepcopy(pop_new[idx][self.ID_POS])
-            self.pop[idx][self.ID_FIT_NEW] = deepcopy(pop_new[idx][self.ID_TAR])
+            self.pop[idx][self.ID_POS_NEW] = pop_new[idx][self.ID_POS].copy()
+            self.pop[idx][self.ID_FIT_NEW] = pop_new[idx][self.ID_TAR].copy()
 
             # ---------- Progress Assessment: Replacing More Quality Solutions With Previous Ones ------
             # Replace Solution If It Reached To A More Quality Position
             if self.compare_agent(pop_new[idx], self.pop[idx]):
-                self.pop[idx][self.ID_POS] = deepcopy(pop_new[idx][self.ID_POS])
-                self.pop[idx][self.ID_TAR] = deepcopy(pop_new[idx][self.ID_TAR])
+                self.pop[idx][self.ID_POS] = pop_new[idx][self.ID_POS].copy()
+                self.pop[idx][self.ID_TAR] = pop_new[idx][self.ID_TAR].copy()
 
         # ========================================================================================= %%
         #        PHASE 3 (LOCAL SEARCH): CREATING SOME WORKER ROBOTS ASSIGNED TO SEARCH               %
         #                      LOCATIONS AROUND POSITION OF MASTER ROBOT                              %
         # ===========================================================================================%%
 
         if epoch > 0:
             # --- EXTRACTING "INTEGER PART" AND "FRACTIONAL PART"  OF THE ELEMENTS OF MASTER RPBOT POSITION------
-            master_robot = {"original": deepcopy(np.reshape(self.pop[0][self.ID_POS], (self.problem.n_dims, 1))),
-                            "sign": deepcopy(np.reshape(np.sign(self.pop[0][self.ID_POS]), (self.problem.n_dims, 1))),
-                            "abs": deepcopy(np.reshape(abs(self.pop[0][self.ID_POS]), (self.problem.n_dims, 1))),
-                            "int": deepcopy(np.reshape(np.floor(abs(self.pop[0][self.ID_POS])), (self.problem.n_dims, 1))),  # INTEGER PART
-                            "frac": deepcopy(np.reshape(abs(self.pop[0][self.ID_POS]) - np.floor(abs(self.pop[0][self.ID_POS])), (self.problem.n_dims, 1)))
+            master_robot = {"original": np.reshape(self.pop[0][self.ID_POS], (self.problem.n_dims, 1)),
+                            "sign": np.reshape(np.sign(self.pop[0][self.ID_POS]), (self.problem.n_dims, 1)),
+                            "abs": np.reshape(abs(self.pop[0][self.ID_POS]), (self.problem.n_dims, 1)),
+                            "int": np.reshape(np.floor(abs(self.pop[0][self.ID_POS])), (self.problem.n_dims, 1)),  # INTEGER PART
+                            "frac": np.reshape(abs(self.pop[0][self.ID_POS]) - np.floor(abs(self.pop[0][self.ID_POS])), (self.problem.n_dims, 1))
                             }  # FRACTIONAL PART
 
             # ------- Applying Nth-root And Nth-exponent Operators To Create Position Of New Worker Robots -------
             worker_robot1 = (master_robot["int"] + np.power(master_robot["frac"], 1 / (1 + np.random.randint(1, 4)))) * master_robot["sign"]
             id_changed1 = np.argwhere(np.round(np.random.uniform(self.problem.lb, self.problem.ub)))
             id_changed1 = np.reshape(id_changed1, (len(id_changed1)))
             worker_robot1 = np.reshape(worker_robot1, (self.problem.n_dims, 1))
@@ -244,9 +242,9 @@
                 pop_workers.append([pos_new, None])
                 if self.mode not in self.AVAILABLE_MODES:
                     pop_workers[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
             pop_workers = self.update_target_wrapper_population(pop_workers)
 
             for i in range(0, 5):
                 if self.compare_agent(pop_workers[i], self.pop[1]):
-                    self.pop[-(i + 1)][self.ID_POS] = deepcopy(pop_workers[i][self.ID_POS])
-                    self.pop[-(i + 1)][self.ID_TAR] = deepcopy(pop_workers[i][self.ID_TAR])
+                    self.pop[-(i + 1)][self.ID_POS] = pop_workers[i][self.ID_POS].copy()
+                    self.pop[-(i + 1)][self.ID_TAR] = pop_workers[i][self.ID_TAR].copy()
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/SSA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/SSA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 17:22, 29/05/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseSSA(Optimizer):
     """
     The developed version: Sparrow Search Algorithm (SSA)
 
@@ -110,15 +109,15 @@
                 target = self.get_target_wrapper(pos_new)
                 self.pop[idx] = self.get_better_solution(self.pop[idx], [pos_new, target])
         if self.mode in self.AVAILABLE_MODES:
             pop_new = self.update_target_wrapper_population(pop_new)
             self.pop = self.greedy_selection_population(self.pop, pop_new)
         self.pop, best, worst = self.get_special_solutions(self.pop, best=1, worst=1)
         g_best, g_worst = best[0], worst[0]
-        pop2 = deepcopy(self.pop[self.n2:])
+        pop2 = self.pop[self.n2:]
         child = []
         for idx in range(0, len(pop2)):
             #  Using equation (5) update the sparrow’s location;
             if self.compare_agent(self.pop[idx], g_best):
                 x_new = pop2[idx][self.ID_POS] + np.random.uniform(-1, 1) * (np.abs(pop2[idx][self.ID_POS] - g_worst[self.ID_POS]) /
                         (pop2[idx][self.ID_TAR][self.ID_FIT] - g_worst[self.ID_TAR][self.ID_FIT] + self.EPSILON))
             else:
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/SSO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/SSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/SSpiderA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/SSpiderA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 11:59, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from scipy.spatial.distance import cdist
 from mealpy.optimizer import Optimizer
 
 
 class OriginalSSpiderA(Optimizer):
     """
     The developed version of: Social Spider Algorithm (OriginalSSpiderA)
@@ -98,38 +97,36 @@
             list: wrapper of solution with format [position, target, intensity, target_position, previous_movement_vector, dimension_mask]
         """
         if pos is None:
             pos = self.generate_position(lb, ub)
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         intensity = np.log(1. / (abs(target[self.ID_FIT]) + self.EPSILON) + 1)
-        target_position = deepcopy(position)
+        target_position = position.copy()
         previous_movement_vector = np.zeros(self.problem.n_dims)
         dimension_mask = np.zeros(self.problem.n_dims)
         return [position, target, intensity, target_position, previous_movement_vector, dimension_mask]
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         all_pos = np.array([it[self.ID_POS] for it in self.pop])  ## Matrix (pop_size, problem_size)
         base_distance = np.mean(np.std(all_pos, axis=0))  ## Number
         dist = cdist(all_pos, all_pos, 'euclidean')
-
         intensity_source = np.array([it[self.ID_INT] for it in self.pop])
         intensity_attenuation = np.exp(-dist / (base_distance * self.r_a))  ## vector (pop_size)
         intensity_receive = np.dot(np.reshape(intensity_source, (1, self.pop_size)), intensity_attenuation)  ## vector (1, pop_size)
         id_best_intennsity = np.argmax(intensity_receive)
-
         pop_new = []
         for idx in range(0, self.pop_size):
-            agent = deepcopy(self.pop[idx])
+            agent = self.pop[idx].copy()
             if self.pop[id_best_intennsity][self.ID_INT] > self.pop[idx][self.ID_INT]:
                 agent[self.ID_TARGET_POS] = self.pop[id_best_intennsity][self.ID_TARGET_POS]
             if np.random.uniform() > self.p_c:  ## changing mask
                 agent[self.ID_MASK] = np.where(np.random.uniform(0, 1, self.problem.n_dims) < self.p_m, 0, 1)
             pos_new = np.where(self.pop[idx][self.ID_MASK] == 0, self.pop[idx][self.ID_TARGET_POS],
                                self.pop[np.random.randint(0, self.pop_size)][self.ID_POS])
             ## Perform random walk
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/SSpiderO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/SSpiderO.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 12:00, 17/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalSSpiderO(Optimizer):
     """
     The original version of: Social Spider Optimization (SSpiderO)
 
@@ -246,15 +245,15 @@
         return list_child
 
     def survive__(self, pop=None, pop_child=None):
         n_child = len(pop)
         pop_child = self.get_sorted_strim_population(pop_child, n_child)
         for i in range(0, n_child):
             if self.compare_agent(pop_child[i], pop[i]):
-                pop[i] = deepcopy(pop_child[i])
+                pop[i] = pop_child[i].copy()
         return pop
 
     def recalculate_weights__(self, pop=None):
         fit_total, fit_best, fit_worst = self.get_special_fitness(pop)
         for i in range(len(pop)):
             if fit_best == fit_worst:
                 pop[i][self.ID_WEI] = np.random.uniform(0.2, 0.8)
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/STO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/STO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/SeaHO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/SeaHO.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Created by "Thieu" at 13:42, 06/03/2023 ----------%                                                                               
 #       Email: nguyenthieu2102@gmail.com            %                                                    
 #       Github: https://github.com/thieu1995        %                         
 # --------------------------------------------------%
 
 import numpy as np
 from mealpy.optimizer import Optimizer
-from math import gamma
 
 
 class OriginalSeaHO(Optimizer):
     """
     The original version of: Sea-Horse Optimization (SeaHO)
 
     Links:
@@ -57,32 +56,23 @@
         self.sort_flag = False
 
     def initialize_variables(self):
         self.uu = 0.05
         self.vv = 0.05
         self.ll = 0.05
 
-    def levy__(self, omega, size):
-        num = gamma(1 + omega) * np.sin(np.pi * omega/2)
-        den = gamma((1 + omega)/2) * omega* 2**((omega - 1) / 2)
-        sigma_u = (num / den) ** (1 / omega)
-        uu = np.random.normal(0, sigma_u, size)
-        vv = np.random.normal(0, 1, size)
-        zz = uu / (np.abs(vv) ** (1 / omega))
-        return zz
-
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
             epoch (int): The current iteration
         """
         # The motor behavior of sea horses
-        step_length = self.levy__(1.5, (self.pop_size, self.problem.n_dims))
+        step_length = self.get_levy_flight_step(beta=1.5, multiplier=0.01, size=(self.pop_size, self.problem.n_dims), case=-1)
         pop_new = []
         for idx in range(0, self.pop_size):
             beta = np.random.normal(0, 1, self.problem.n_dims)
             theta = 2 * np.pi * np.random.rand(self.problem.n_dims)
             row = self.uu * np.exp(theta * self.vv)
             xx, yy, zz = row * np.cos(theta), row * np.sin(theta), row * theta
             if np.random.normal(0, 1) > 0:      # Eq. 4
```

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/ServalOA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/ServalOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/TDO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/TDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/TSO.py` & `mealpy-2.5.4a3/mealpy/swarm_based/TSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/WOA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/WOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/WaOA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/WaOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/swarm_based/ZOA.py` & `mealpy-2.5.4a3/mealpy/swarm_based/ZOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/system_based/AEO.py` & `mealpy-2.5.4a3/mealpy/system_based/AEO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/system_based/GCO.py` & `mealpy-2.5.4a3/mealpy/system_based/GCO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 16:44, 18/03/2020 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class BaseGCO(Optimizer):
     """
     The developed version: Germinal Center Optimization (GCO)
 
@@ -89,15 +88,15 @@
             pop_new.append([pos_new, None])
             if self.mode not in self.AVAILABLE_MODES:
                 pop_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
         pop_new = self.update_target_wrapper_population(pop_new)
         for idx in range(0, self.pop_size):
             if self.compare_agent(pop_new[idx], self.pop[idx]):
                 self.dyn_list_cell_counter[idx] += 10
-                self.pop[idx] = deepcopy(pop_new[idx])
+                self.pop[idx] = pop_new[idx].copy()
 
         ## Light-zone process   (no needs parallelization)
         for i in range(0, self.pop_size):
             self.dyn_list_cell_counter[i] = 10
             fit_list = np.array([item[self.ID_TAR][self.ID_FIT] for item in self.pop])
             fit_max = max(fit_list)
             fit_min = min(fit_list)
```

### Comparing `mealpy-2.5.4a2/mealpy/system_based/WCA.py` & `mealpy-2.5.4a3/mealpy/system_based/WCA.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python
 # Created by "Thieu" at 09:55, 02/03/2021 ----------%
 #       Email: nguyenthieu2102@gmail.com            %
 #       Github: https://github.com/thieu1995        %
 # --------------------------------------------------%
 
 import numpy as np
-from copy import deepcopy
 from mealpy.optimizer import Optimizer
 
 
 class OriginalWCA(Optimizer):
     """
     The original version of: Water Cycle Algorithm (WCA)
 
@@ -78,17 +77,17 @@
 
     def initialization(self):
         if self.pop is None:
             self.pop = self.create_population(self.pop_size)
         self.pop, self.g_best = self.get_global_best_solution(self.pop)
         self.ecc = self.dmax  # Evaporation condition constant - variable
         n_stream = self.pop_size - self.nsr
-        g_best = deepcopy(self.pop[0])  # Global best solution (sea)
-        self.pop_best = deepcopy(self.pop[:self.nsr])  # Including sea and river (1st solution is sea)
-        self.pop_stream = deepcopy(self.pop[self.nsr:])  # Forming Stream
+        g_best = self.pop[0].copy()  # Global best solution (sea)
+        self.pop_best = self.pop[:self.nsr]  # Including sea and river (1st solution is sea)
+        self.pop_stream = self.pop[self.nsr:] # Forming Stream
 
         # Designate streams to rivers and sea
         cost_river_list = np.array([solution[self.ID_TAR][self.ID_FIT] for solution in self.pop_best])
         num_child_in_river_list = np.round(np.abs(cost_river_list / np.sum(cost_river_list)) * n_stream).astype(int)
         if np.sum(num_child_in_river_list) < n_stream:
             num_child_in_river_list[-1] += n_stream - np.sum(num_child_in_river_list)
         streams = {}
@@ -122,15 +121,15 @@
                 stream_new.append([pos_new, None])
                 if self.mode not in self.AVAILABLE_MODES:
                     stream_new[-1][self.ID_TAR] = self.get_target_wrapper(pos_new)
             stream_new = self.update_target_wrapper_population(stream_new)
             stream_new, stream_best = self.get_global_best_solution(stream_new)
             self.streams[idx] = stream_new
             if self.compare_agent(stream_best, self.pop_best[idx]):
-                self.pop_best[idx] = deepcopy(stream_best)
+                self.pop_best[idx] = stream_best.copy()
 
             # Update river
             pos_new = self.pop_best[idx][self.ID_POS] + np.random.uniform() * self.wc * (self.g_best[self.ID_POS] - self.pop_best[idx][self.ID_POS])
             pos_new = self.amend_position(pos_new, self.problem.lb, self.problem.ub)
             target = self.get_target_wrapper(pos_new)
             if self.compare_agent([pos_new, target], self.pop_best[idx]):
                 self.pop_best[idx] = [pos_new, target]
@@ -139,12 +138,12 @@
         for i in range(1, self.nsr):
             distance = np.sqrt(np.sum((self.g_best[self.ID_POS] - self.pop_best[i][self.ID_POS]) ** 2))
             if distance < self.ecc or np.random.rand() < 0.1:
                 child = self.create_solution(self.problem.lb, self.problem.ub)
                 pop_current_best, _ = self.get_global_best_solution(self.streams[i] + [child])
                 self.pop_best[i] = pop_current_best.pop(0)
                 self.streams[i] = pop_current_best
-        self.pop = deepcopy(self.pop_best)
+        self.pop = self.pop_best.copy()
         for idx, stream_list in self.streams.items():
             self.pop += stream_list
         # Reduce the ecc
         self.ecc = self.ecc - self.ecc / self.epoch
```

### Comparing `mealpy-2.5.4a2/mealpy/tuner.py` & `mealpy-2.5.4a3/mealpy/tuner.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/utils/history.py` & `mealpy-2.5.4a3/mealpy/utils/history.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/utils/io.py` & `mealpy-2.5.4a3/mealpy/utils/io.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/utils/logger.py` & `mealpy-2.5.4a3/mealpy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/utils/problem.py` & `mealpy-2.5.4a3/mealpy/utils/problem.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/utils/termination.py` & `mealpy-2.5.4a3/mealpy/utils/termination.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/utils/validator.py` & `mealpy-2.5.4a3/mealpy/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy/utils/visualize/linechart.py` & `mealpy-2.5.4a3/mealpy/utils/visualize/linechart.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/mealpy.egg-info/PKG-INFO` & `mealpy-2.5.4a3/mealpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mealpy
-Version: 2.5.4a2
+Version: 2.5.4a3
 Summary: MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python
 Home-page: https://github.com/thieu1995/mealpy
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mealpy.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mealpy
```

### Comparing `mealpy-2.5.4a2/mealpy.egg-info/SOURCES.txt` & `mealpy-2.5.4a3/mealpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/setup.py` & `mealpy-2.5.4a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mealpy",
-    version="2.5.4-alpha.2",
+    version="2.5.4-alpha.3",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["optimization", "metaheuristics", "MHA", "mathematical optimization", "nature-inspired algorithms",
               "evolutionary computation", "soft computing", "population-based algorithms",
```

### Comparing `mealpy-2.5.4a2/tests/test_optimizer.py` & `mealpy-2.5.4a3/tests/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a2/tests/test_tuner.py` & `mealpy-2.5.4a3/tests/test_tuner.py`

 * *Files identical despite different names*

