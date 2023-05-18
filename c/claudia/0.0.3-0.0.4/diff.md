# Comparing `tmp/claudia-0.0.3.tar.gz` & `tmp/claudia-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claudia-0.0.3.tar", last modified: Tue May 16 18:16:50 2023, max compression
+gzip compressed data, was "claudia-0.0.4.tar", last modified: Thu May 18 02:41:02 2023, max compression
```

## Comparing `claudia-0.0.3.tar` & `claudia-0.0.4.tar`

### file list

```diff
@@ -1,61 +1,87 @@
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.993621 claudia-0.0.3/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1073 2023-05-11 10:47:00.000000 claudia-0.0.3/LICENSE
--rw-r--r--   0 ksaxena    (502) staff       (20)     1866 2023-05-16 18:16:50.993401 claudia-0.0.3/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     3088 2023-05-15 19:36:08.000000 claudia-0.0.3/README.md
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.974413 claudia-0.0.3/claudia.egg-info/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1866 2023-05-16 18:16:50.000000 claudia-0.0.3/claudia.egg-info/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     1675 2023-05-16 18:16:50.000000 claudia-0.0.3/claudia.egg-info/SOURCES.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-05-16 18:16:50.000000 claudia-0.0.3/claudia.egg-info/dependency_links.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-16 18:16:50.000000 claudia-0.0.3/claudia.egg-info/entry_points.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       79 2023-05-16 18:16:50.000000 claudia-0.0.3/claudia.egg-info/requires.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-05-16 18:16:50.000000 claudia-0.0.3/claudia.egg-info/top_level.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-05-16 18:16:50.993682 claudia-0.0.3/setup.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)     2018 2023-05-16 17:54:04.000000 claudia-0.0.3/setup.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.968673 claudia-0.0.3/src/
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.976227 claudia-0.0.3/src/claudia/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1517 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/README.md
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     9411 2023-05-16 17:35:18.000000 claudia-0.0.3/src/claudia/claudia.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.977710 claudia-0.0.3/src/claudia/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/features/nft_burn_mint.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/features/payments.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/features/trustline.feature
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.980715 claudia-0.0.3/src/claudia/javascript/
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/cleanup
--rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/cucumber.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.981191 claudia-0.0.3/src/claudia/javascript/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1226 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/features/context.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.981634 claudia-0.0.3/src/claudia/javascript/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)     2106 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/features/lib/ObjFactory.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.984736 claudia-0.0.3/src/claudia/javascript/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    38728 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/features/steps/common.js
--rw-r--r--   0 ksaxena    (502) staff       (20)      300 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/features/steps/constants.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/features/steps/nft_mint_burn.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/features/steps/payments.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/features/steps/trustline.js
--rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/package-lock.json
--rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/package.json
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      869 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     4674 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/javascript/runTest
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.986727 claudia-0.0.3/src/claudia/python/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/behave.ini
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/cleanup
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.987641 claudia-0.0.3/src/claudia/python/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/features/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     2977 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/features/environment.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.988539 claudia-0.0.3/src/claudia/python/features/exceptions/
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/features/exceptions/InvalidInputException.py
--rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/features/exceptions/UnconfiguredEnvironmentException.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.989494 claudia-0.0.3/src/claudia/python/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)      301 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/features/lib/Helpers.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     7674 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/features/lib/ObjFactory.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-16 18:16:50.992866 claudia-0.0.3/src/claudia/python/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    24750 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/features/steps/common.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/features/steps/constants.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    66340 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/features/steps/nft_mint_burn.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    21822 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/features/steps/payments.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    54620 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/features/steps/trustline.py
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     1381 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     5634 2023-05-15 18:14:02.000000 claudia-0.0.3/src/claudia/python/runTest
--rw-r--r--   0 ksaxena    (502) staff       (20)       79 2023-05-15 19:03:09.000000 claudia-0.0.3/src/claudia/requirements.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.697970 claudia-0.0.4/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1073 2023-05-11 10:47:00.000000 claudia-0.0.4/LICENSE
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1866 2023-05-18 02:41:02.697748 claudia-0.0.4/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3088 2023-05-15 19:36:08.000000 claudia-0.0.4/README.md
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.676966 claudia-0.0.4/claudia.egg-info/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1866 2023-05-18 02:41:02.000000 claudia-0.0.4/claudia.egg-info/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2610 2023-05-18 02:41:02.000000 claudia-0.0.4/claudia.egg-info/SOURCES.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-05-18 02:41:02.000000 claudia-0.0.4/claudia.egg-info/dependency_links.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-18 02:41:02.000000 claudia-0.0.4/claudia.egg-info/entry_points.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       79 2023-05-18 02:41:02.000000 claudia-0.0.4/claudia.egg-info/requires.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-05-18 02:41:02.000000 claudia-0.0.4/claudia.egg-info/top_level.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-05-18 02:41:02.698034 claudia-0.0.4/setup.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1477 2023-05-18 02:38:59.000000 claudia-0.0.4/setup.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.670291 claudia-0.0.4/src/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.678304 claudia-0.0.4/src/claudia/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1517 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/README.md
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    10376 2023-05-16 20:58:51.000000 claudia-0.0.4/src/claudia/claudia.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.679544 claudia-0.0.4/src/claudia/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/features/nft_burn_mint.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/features/payments.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/features/trustline.feature
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.681920 claudia-0.0.4/src/claudia/javascript/
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/cleanup
+-rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/cucumber.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.682267 claudia-0.0.4/src/claudia/javascript/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1226 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/context.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.682550 claudia-0.0.4/src/claudia/javascript/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2106 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/lib/ObjFactory.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.684437 claudia-0.0.4/src/claudia/javascript/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    38728 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/steps/common.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)      300 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/steps/constants.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/steps/nft_mint_burn.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/steps/payments.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/features/steps/trustline.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/package-lock.json
+-rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/package.json
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      869 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     4674 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/javascript/runTest
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.685079 claudia-0.0.4/src/claudia/network_setup/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      251 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/Dockerfile
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.685889 claudia-0.0.4/src/claudia/network_setup/configs/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     1520 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled.cfg
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.686599 claudia-0.0.4/src/claudia/network_setup/configs/rippled_1/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2150 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_1/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_1/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.687178 claudia-0.0.4/src/claudia/network_setup/configs/rippled_2/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_2/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_2/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.687893 claudia-0.0.4/src/claudia/network_setup/configs/rippled_3/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_3/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_3/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.688610 claudia-0.0.4/src/claudia/network_setup/configs/rippled_4/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2190 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_4/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_4/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.689721 claudia-0.0.4/src/claudia/network_setup/configs/rippled_5/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2226 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_5/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/rippled_5/validators.txt
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      279 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/configs/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.691228 claudia-0.0.4/src/claudia/network_setup/lib/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     1619 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/lib/build_rippled.sh
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2161 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/lib/rippled_network.yml
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     8966 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/lib/setup_helper.sh
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     5094 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/lib/validate_network.py
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     3784 2023-05-18 02:32:34.000000 claudia-0.0.4/src/claudia/network_setup/setup.sh
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.692897 claudia-0.0.4/src/claudia/python/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/behave.ini
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/cleanup
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.693446 claudia-0.0.4/src/claudia/python/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2977 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/environment.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.694327 claudia-0.0.4/src/claudia/python/features/exceptions/
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/exceptions/InvalidInputException.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/exceptions/UnconfiguredEnvironmentException.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.695236 claudia-0.0.4/src/claudia/python/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)      301 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/lib/Helpers.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     7674 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/lib/ObjFactory.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-18 02:41:02.697333 claudia-0.0.4/src/claudia/python/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    24750 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/steps/common.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/steps/constants.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    66340 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/steps/nft_mint_burn.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    21822 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/steps/payments.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    54620 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/features/steps/trustline.py
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     1381 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     5634 2023-05-15 18:14:02.000000 claudia-0.0.4/src/claudia/python/runTest
+-rw-r--r--   0 ksaxena    (502) staff       (20)       79 2023-05-16 18:21:22.000000 claudia-0.0.4/src/claudia/requirements.txt
```

### Comparing `claudia-0.0.3/LICENSE` & `claudia-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/PKG-INFO` & `claudia-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudia
-Version: 0.0.3
+Version: 0.0.4
 Summary: Run XRPL Automated Tests
 Home-page: https://xrpl.org/
 Download-URL: https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation
 Author: Kausty Saxena
 Author-email: ksaxena@ripple.com
 Keywords: ripple xrpl python javascript
 Description-Content-Type: text/markdown
```

### Comparing `claudia-0.0.3/README.md` & `claudia-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/claudia.egg-info/PKG-INFO` & `claudia-0.0.4/claudia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudia
-Version: 0.0.3
+Version: 0.0.4
 Summary: Run XRPL Automated Tests
 Home-page: https://xrpl.org/
 Download-URL: https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation
 Author: Kausty Saxena
 Author-email: ksaxena@ripple.com
 Keywords: ripple xrpl python javascript
 Description-Content-Type: text/markdown
```

### Comparing `claudia-0.0.3/src/claudia/README.md` & `claudia-0.0.4/src/claudia/README.md`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/claudia.py` & `claudia-0.0.4/src/claudia/claudia.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,24 +20,63 @@
 
 @main.group()
 @click.pass_context
 def run(context):
     """This command allows you to run XRPL automated tests."""
 
 
+@main.command()
+# @click.pass_context
+@click.option('--repo', required=True, help="The path to a local rippled repo")
+def build(repo):
+    """Build rippled from source"""
+    # click.echo("Hellow12")
+    set_to_project_root_wd()
+    # click.echo("Hellow")
+    command = "sh network_setup/setup.sh --buildRippled --rippledRepo {}".format(repo)
+    subprocess.call(command, shell=True)
+
+
 @main.group()
-@click.pass_context
-def build(context):
-    """TO BE IMPLEMENTED: This command allows you to build Rippled on demand. Please choose your options wisely."""
+# @click.pass_context
+def install():
+    """Install rippled packages"""
+    click.echo("Currently not supported")
 
 
 @main.group()
-@click.pass_context
-def network(context):
-    """TO BE IMPLEMENTED: This command allows you to build a local network. Please choose your options wisely."""
+# @click.pass_context
+def network():
+    """Setup Rippled Network"""
+
+
+@network.command()
+@click.option('--repo', required=True,
+              help="path to rippled repo")
+def start(repo):
+    """Start a new rippled network"""
+    set_to_project_root_wd()
+    command = "sh ./network_setup/setup.sh --networkStart  --rippledRepo {}".format(repo)
+    subprocess.call(command, shell=True)
+
+
+@network.command()
+def stop():
+    """Stop rippled network"""
+    set_to_project_root_wd()
+    command = "sh ./network_setup/setup.sh --networkStop"
+    subprocess.call(command, shell=True)
+
+
+@network.command()
+def status():
+    """rippled network status"""
+    set_to_project_root_wd()
+    command = "sh ./network_setup/setup.sh --networkStatus"
+    subprocess.call(command, shell=True)
 
 
 @run.command()
 @click.pass_context
 @click.option('--client_type', default='websocket',
               help="The type of client to be used. Allowed values are 'websocket' and 'jsonrpc' and is defaulted to 'websocket'. More information: \n\nhttps://xrpl.org/get-started-using-http-websocket-apis.html#differences-between-json-rpc-and-websocket")
 @click.option('--network', default='local',
```

### Comparing `claudia-0.0.3/src/claudia/features/nft_burn_mint.feature` & `claudia-0.0.4/src/claudia/features/nft_burn_mint.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/features/payments.feature` & `claudia-0.0.4/src/claudia/features/payments.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/features/trustline.feature` & `claudia-0.0.4/src/claudia/features/trustline.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/javascript/features/context.js` & `claudia-0.0.4/src/claudia/javascript/features/context.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/javascript/features/lib/ObjFactory.js` & `claudia-0.0.4/src/claudia/javascript/features/lib/ObjFactory.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/javascript/features/steps/common.js` & `claudia-0.0.4/src/claudia/javascript/features/steps/common.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/javascript/features/steps/nft_mint_burn.js` & `claudia-0.0.4/src/claudia/javascript/features/steps/nft_mint_burn.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/javascript/features/steps/payments.js` & `claudia-0.0.4/src/claudia/javascript/features/steps/payments.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/javascript/features/steps/trustline.js` & `claudia-0.0.4/src/claudia/javascript/features/steps/trustline.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/javascript/package-lock.json` & `claudia-0.0.4/src/claudia/javascript/package-lock.json`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/javascript/runSetup` & `claudia-0.0.4/src/claudia/javascript/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/javascript/runTest` & `claudia-0.0.4/src/claudia/javascript/runTest`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/python/features/environment.py` & `claudia-0.0.4/src/claudia/python/features/environment.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/python/features/lib/ObjFactory.py` & `claudia-0.0.4/src/claudia/python/features/lib/ObjFactory.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/python/features/steps/common.py` & `claudia-0.0.4/src/claudia/python/features/steps/common.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/python/features/steps/nft_mint_burn.py` & `claudia-0.0.4/src/claudia/python/features/steps/nft_mint_burn.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/python/features/steps/payments.py` & `claudia-0.0.4/src/claudia/python/features/steps/payments.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/python/features/steps/trustline.py` & `claudia-0.0.4/src/claudia/python/features/steps/trustline.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/python/runSetup` & `claudia-0.0.4/src/claudia/python/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.0.3/src/claudia/python/runTest` & `claudia-0.0.4/src/claudia/python/runTest`

 * *Files identical despite different names*

