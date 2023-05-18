# Comparing `tmp/rfcat-1.9.7.tar.gz` & `tmp/rfcat-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfcat-1.9.7.tar", last modified: Tue Dec 20 19:36:48 2022, max compression
+gzip compressed data, was "rfcat-2.0.0.tar", last modified: Thu May 18 11:05:13 2023, max compression
```

## Comparing `rfcat-1.9.7.tar` & `rfcat-2.0.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.770861 rfcat-1.9.7/
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.754861 rfcat-1.9.7/CC-Bootloader/
--rwxrwxr-x   0 atlas     (1000) atlas     (1000)     7960 2022-12-20 19:35:42.000000 rfcat-1.9.7/CC-Bootloader/rfcat_bootloader
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     1242 2020-08-28 19:27:05.000000 rfcat-1.9.7/FAQ
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      894 2020-08-28 19:27:05.000000 rfcat-1.9.7/LICENSE
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    18145 2020-08-28 19:27:05.000000 rfcat-1.9.7/LICENSE.CC-Bootloader
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      301 2020-08-28 19:27:05.000000 rfcat-1.9.7/MANIFEST.in
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    13554 2022-12-20 19:36:48.770861 rfcat-1.9.7/PKG-INFO
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      737 2020-08-28 19:27:05.000000 rfcat-1.9.7/README.immesniff
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     4493 2020-09-30 19:40:51.000000 rfcat-1.9.7/README.msfrelay
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      529 2020-08-28 19:27:05.000000 rfcat-1.9.7/README.nonroot
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    12683 2020-09-30 19:40:51.000000 rfcat-1.9.7/README.rst
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      769 2020-08-28 19:27:05.000000 rfcat-1.9.7/TODO
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.750862 rfcat-1.9.7/etc/
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.750862 rfcat-1.9.7/etc/udev/
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.754861 rfcat-1.9.7/etc/udev/rules.d/
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     1392 2020-08-28 19:27:05.000000 rfcat-1.9.7/etc/udev/rules.d/20-rfcat.rules
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.758861 rfcat-1.9.7/firmware/
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.758861 rfcat-1.9.7/firmware/CCBootloader/
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    15256 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/CCBootloader/CCBootloader-rfcat-chronosdongle.hex
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    15244 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/CCBootloader/CCBootloader-rfcat-donsdongle.hex
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    11416 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/CCBootloader/CCBootloader-rfcat-ys1.hex
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    24070 2022-08-11 17:22:23.000000 rfcat-1.9.7/firmware/Makefile
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     8191 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/appCC2531.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    48401 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/appFHSSNIC.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     7913 2020-09-30 19:40:51.000000 rfcat-1.9.7/firmware/appNIC.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     8703 2020-09-30 19:40:51.000000 rfcat-1.9.7/firmware/appNetworkTest.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    10055 2020-09-30 19:40:51.000000 rfcat-1.9.7/firmware/appSniff.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     9816 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/application.c
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.758861 rfcat-1.9.7/firmware/bins/
--rw-rw-r--   0 atlas     (1000) atlas     (1000)        0 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/bins/.placeholder
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      608 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/bootloader.c
--rwxrwxr-x   0 atlas     (1000) atlas     (1000)     1097 2022-08-11 17:22:23.000000 rfcat-1.9.7/firmware/bootloader_serial.py
--rwxrwxr-x   0 atlas     (1000) atlas     (1000)     1240 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/buildall.sh
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     4388 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/cc1111_aes.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    11097 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/cc1111_vcom.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     4054 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/cc1111_vcomdesc.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    22750 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/cc1111rf.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     1568 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/chipcon_dma.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    59284 2020-09-30 19:40:51.000000 rfcat-1.9.7/firmware/chipcon_usb.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     1049 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/chipcon_usbdebug.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     4864 2020-09-30 19:40:51.000000 rfcat-1.9.7/firmware/global.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     3667 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/immedisplay.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     4585 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/immefont.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    21492 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/immeio.c
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     3229 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/immekeys.c
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.762861 rfcat-1.9.7/firmware/include/
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     2209 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/FHSS.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      144 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/bits.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)       27 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/bootloader.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    50742 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/cc1110-ext.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     2284 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/cc1111.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      859 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/cc1111_aes.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     4222 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/cc1111_vcom.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     6122 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/cc1111rf.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)       74 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/cc1111usb.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    52288 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/cc2530-ext.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     3153 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/cc2531.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     1671 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/chipcon_dma.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    35408 2022-08-11 17:22:23.000000 rfcat-1.9.7/firmware/include/chipcon_usb.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      295 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/chipcon_usbdebug.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     6651 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/global.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     4347 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/imme5x7.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     1585 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/immedisplay.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      115 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/immefont.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      984 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/immeio.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     1302 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/immekeys.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)       67 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/immestring.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     1112 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/immeterm.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      513 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/nic.h
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      173 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/include/types.h
--rwxrwxr-x   0 atlas     (1000) atlas     (1000)      545 2022-08-11 17:22:23.000000 rfcat-1.9.7/firmware/new_serial.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)       45 2020-08-28 19:27:05.000000 rfcat-1.9.7/firmware/usbonly.c
--rwxrwxr-x   0 atlas     (1000) atlas     (1000)      632 2020-08-28 19:27:05.000000 rfcat-1.9.7/package.sh
--rwxrwxr-x   0 atlas     (1000) atlas     (1000)      175 2022-08-11 17:22:23.000000 rfcat-1.9.7/revision.sh
--rwxrwxr-x   0 atlas     (1000) atlas     (1000)     2601 2022-08-11 17:22:23.000000 rfcat-1.9.7/rfcat
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.766861 rfcat-1.9.7/rfcat.egg-info/
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    13554 2022-12-20 19:36:48.000000 rfcat-1.9.7/rfcat.egg-info/PKG-INFO
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     2200 2022-12-20 19:36:48.000000 rfcat-1.9.7/rfcat.egg-info/SOURCES.txt
--rw-rw-r--   0 atlas     (1000) atlas     (1000)        1 2022-12-20 19:36:48.000000 rfcat-1.9.7/rfcat.egg-info/dependency_links.txt
--rw-rw-r--   0 atlas     (1000) atlas     (1000)       62 2022-12-20 19:36:48.000000 rfcat-1.9.7/rfcat.egg-info/requires.txt
--rw-rw-r--   0 atlas     (1000) atlas     (1000)       12 2022-12-20 19:36:48.000000 rfcat-1.9.7/rfcat.egg-info/top_level.txt
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    13863 2020-09-01 21:48:07.000000 rfcat-1.9.7/rfcat_msfrelay
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    26765 2022-08-11 17:22:23.000000 rfcat-1.9.7/rfcat_server
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.766861 rfcat-1.9.7/rflib/
--rwxrwxr-x   0 atlas     (1000) atlas     (1000)     8229 2022-08-11 17:22:23.000000 rfcat-1.9.7/rflib/__init__.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    21357 2022-08-11 17:22:23.000000 rfcat-1.9.7/rflib/bits.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     6070 2022-08-11 17:22:23.000000 rfcat-1.9.7/rflib/cc111Xhparser.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      411 2020-08-28 19:27:05.000000 rfcat-1.9.7/rflib/ccrecvdump.py
--rwxrwxr-x   0 atlas     (1000) atlas     (1000)    20525 2022-08-11 17:22:23.000000 rfcat-1.9.7/rflib/ccspecan.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    76373 2021-01-01 15:39:22.000000 rfcat-1.9.7/rflib/chipcon_nic.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    35907 2020-12-31 15:55:39.000000 rfcat-1.9.7/rflib/chipcon_usb.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    62446 2020-09-30 19:40:51.000000 rfcat-1.9.7/rflib/chipcondefs.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    12516 2020-08-28 19:27:05.000000 rfcat-1.9.7/rflib/const.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    20908 2020-09-30 19:40:51.000000 rfcat-1.9.7/rflib/fakedongle_nic.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    42319 2022-08-11 17:22:23.000000 rfcat-1.9.7/rflib/intelhex.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     1523 2020-08-28 19:27:05.000000 rfcat-1.9.7/rflib/rflib_defs.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)       18 2022-12-20 19:36:48.000000 rfcat-1.9.7/rflib/rflib_version.py
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.770861 rfcat-1.9.7/rflib/vstruct/
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     8556 2020-12-31 15:55:39.000000 rfcat-1.9.7/rflib/vstruct/__init__.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     8029 2020-09-30 19:40:51.000000 rfcat-1.9.7/rflib/vstruct/builder.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)    10442 2020-09-30 19:40:51.000000 rfcat-1.9.7/rflib/vstruct/primitives.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)       80 2022-12-20 19:36:48.770861 rfcat-1.9.7/setup.cfg
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     2977 2022-08-11 17:29:38.000000 rfcat-1.9.7/setup.py
-drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2022-12-20 19:36:48.770861 rfcat-1.9.7/tests/
--rw-rw-r--   0 atlas     (1000) atlas     (1000)        0 2020-08-28 19:27:05.000000 rfcat-1.9.7/tests/__init__.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     8451 2020-08-28 19:27:05.000000 rfcat-1.9.7/tests/test_api.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)      473 2021-01-19 14:23:53.000000 rfcat-1.9.7/tests/test_basics.py
--rw-rw-r--   0 atlas     (1000) atlas     (1000)     4332 2022-08-11 17:22:23.000000 rfcat-1.9.7/tests/test_bits.py
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.826856 rfcat-2.0.0/
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.822856 rfcat-2.0.0/CC-Bootloader/
+-rwxrwxr-x   0 atlas     (1000) atlas     (1000)     7960 2022-12-20 19:35:42.000000 rfcat-2.0.0/CC-Bootloader/rfcat_bootloader
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     1242 2020-08-28 19:27:05.000000 rfcat-2.0.0/FAQ
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      894 2020-08-28 19:27:05.000000 rfcat-2.0.0/LICENSE
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    18145 2020-08-28 19:27:05.000000 rfcat-2.0.0/LICENSE.CC-Bootloader
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      301 2020-08-28 19:27:05.000000 rfcat-2.0.0/MANIFEST.in
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    13554 2023-05-18 11:05:13.826856 rfcat-2.0.0/PKG-INFO
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      737 2020-08-28 19:27:05.000000 rfcat-2.0.0/README.immesniff
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     4493 2020-09-30 19:40:51.000000 rfcat-2.0.0/README.msfrelay
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      529 2020-08-28 19:27:05.000000 rfcat-2.0.0/README.nonroot
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    12683 2020-09-30 19:40:51.000000 rfcat-2.0.0/README.rst
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      769 2020-08-28 19:27:05.000000 rfcat-2.0.0/TODO
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.818856 rfcat-2.0.0/etc/
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.818856 rfcat-2.0.0/etc/udev/
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.822856 rfcat-2.0.0/etc/udev/rules.d/
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     1392 2020-08-28 19:27:05.000000 rfcat-2.0.0/etc/udev/rules.d/20-rfcat.rules
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.822856 rfcat-2.0.0/firmware/
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.822856 rfcat-2.0.0/firmware/CCBootloader/
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    15256 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/CCBootloader/CCBootloader-rfcat-chronosdongle.hex
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    15244 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/CCBootloader/CCBootloader-rfcat-donsdongle.hex
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    11416 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/CCBootloader/CCBootloader-rfcat-ys1.hex
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    24070 2022-08-11 17:22:23.000000 rfcat-2.0.0/firmware/Makefile
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     8191 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/appCC2531.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    48401 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/appFHSSNIC.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     7913 2020-09-30 19:40:51.000000 rfcat-2.0.0/firmware/appNIC.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     8703 2020-09-30 19:40:51.000000 rfcat-2.0.0/firmware/appNetworkTest.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    10055 2020-09-30 19:40:51.000000 rfcat-2.0.0/firmware/appSniff.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     9816 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/application.c
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.822856 rfcat-2.0.0/firmware/bins/
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)        0 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/bins/.placeholder
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      608 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/bootloader.c
+-rwxrwxr-x   0 atlas     (1000) atlas     (1000)     1097 2022-08-11 17:22:23.000000 rfcat-2.0.0/firmware/bootloader_serial.py
+-rwxrwxr-x   0 atlas     (1000) atlas     (1000)     1240 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/buildall.sh
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     4388 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/cc1111_aes.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    11097 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/cc1111_vcom.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     4054 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/cc1111_vcomdesc.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    22750 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/cc1111rf.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     1568 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/chipcon_dma.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    59284 2020-09-30 19:40:51.000000 rfcat-2.0.0/firmware/chipcon_usb.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     1049 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/chipcon_usbdebug.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     4864 2020-09-30 19:40:51.000000 rfcat-2.0.0/firmware/global.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     3667 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/immedisplay.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     4585 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/immefont.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    21492 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/immeio.c
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     3229 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/immekeys.c
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.826856 rfcat-2.0.0/firmware/include/
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     2209 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/FHSS.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      144 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/bits.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)       27 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/bootloader.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    50742 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/cc1110-ext.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     2284 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/cc1111.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      859 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/cc1111_aes.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     4222 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/cc1111_vcom.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     6122 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/cc1111rf.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)       74 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/cc1111usb.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    52288 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/cc2530-ext.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     3153 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/cc2531.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     1671 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/chipcon_dma.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    35408 2022-08-11 17:22:23.000000 rfcat-2.0.0/firmware/include/chipcon_usb.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      295 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/chipcon_usbdebug.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     6651 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/global.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     4347 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/imme5x7.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     1585 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/immedisplay.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      115 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/immefont.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      984 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/immeio.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     1302 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/immekeys.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)       67 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/immestring.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     1112 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/immeterm.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      513 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/nic.h
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      173 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/include/types.h
+-rwxrwxr-x   0 atlas     (1000) atlas     (1000)      545 2022-08-11 17:22:23.000000 rfcat-2.0.0/firmware/new_serial.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)       45 2020-08-28 19:27:05.000000 rfcat-2.0.0/firmware/usbonly.c
+-rwxrwxr-x   0 atlas     (1000) atlas     (1000)      632 2020-08-28 19:27:05.000000 rfcat-2.0.0/package.sh
+-rwxrwxr-x   0 atlas     (1000) atlas     (1000)      175 2022-08-11 17:22:23.000000 rfcat-2.0.0/revision.sh
+-rwxrwxr-x   0 atlas     (1000) atlas     (1000)     2601 2022-08-11 17:22:23.000000 rfcat-2.0.0/rfcat
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.826856 rfcat-2.0.0/rfcat.egg-info/
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    13554 2023-05-18 11:05:13.000000 rfcat-2.0.0/rfcat.egg-info/PKG-INFO
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     2200 2023-05-18 11:05:13.000000 rfcat-2.0.0/rfcat.egg-info/SOURCES.txt
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)        1 2023-05-18 11:05:13.000000 rfcat-2.0.0/rfcat.egg-info/dependency_links.txt
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)       62 2023-05-18 11:05:13.000000 rfcat-2.0.0/rfcat.egg-info/requires.txt
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)       12 2023-05-18 11:05:13.000000 rfcat-2.0.0/rfcat.egg-info/top_level.txt
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    13863 2020-09-01 21:48:07.000000 rfcat-2.0.0/rfcat_msfrelay
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    26765 2022-08-11 17:22:23.000000 rfcat-2.0.0/rfcat_server
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.826856 rfcat-2.0.0/rflib/
+-rwxrwxr-x   0 atlas     (1000) atlas     (1000)     8474 2023-05-18 11:02:54.000000 rfcat-2.0.0/rflib/__init__.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    21357 2022-08-11 17:22:23.000000 rfcat-2.0.0/rflib/bits.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     6070 2022-08-11 17:22:23.000000 rfcat-2.0.0/rflib/cc111Xhparser.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      411 2020-08-28 19:27:05.000000 rfcat-2.0.0/rflib/ccrecvdump.py
+-rwxrwxr-x   0 atlas     (1000) atlas     (1000)    20525 2022-08-11 17:22:23.000000 rfcat-2.0.0/rflib/ccspecan.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    76373 2021-01-01 15:39:22.000000 rfcat-2.0.0/rflib/chipcon_nic.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    35907 2020-12-31 15:55:39.000000 rfcat-2.0.0/rflib/chipcon_usb.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    62446 2020-09-30 19:40:51.000000 rfcat-2.0.0/rflib/chipcondefs.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    12516 2020-08-28 19:27:05.000000 rfcat-2.0.0/rflib/const.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    20908 2020-09-30 19:40:51.000000 rfcat-2.0.0/rflib/fakedongle_nic.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    42319 2022-08-11 17:22:23.000000 rfcat-2.0.0/rflib/intelhex.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     1523 2020-08-28 19:27:05.000000 rfcat-2.0.0/rflib/rflib_defs.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)       18 2023-05-18 11:05:13.000000 rfcat-2.0.0/rflib/rflib_version.py
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.826856 rfcat-2.0.0/rflib/vstruct/
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     8556 2020-12-31 15:55:39.000000 rfcat-2.0.0/rflib/vstruct/__init__.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     8029 2020-09-30 19:40:51.000000 rfcat-2.0.0/rflib/vstruct/builder.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)    10442 2020-09-30 19:40:51.000000 rfcat-2.0.0/rflib/vstruct/primitives.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)       80 2023-05-18 11:05:13.826856 rfcat-2.0.0/setup.cfg
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     2977 2022-08-11 17:29:38.000000 rfcat-2.0.0/setup.py
+drwxrwxr-x   0 atlas     (1000) atlas     (1000)        0 2023-05-18 11:05:13.826856 rfcat-2.0.0/tests/
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)        0 2020-08-28 19:27:05.000000 rfcat-2.0.0/tests/__init__.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     8451 2020-08-28 19:27:05.000000 rfcat-2.0.0/tests/test_api.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)      473 2021-01-19 14:23:53.000000 rfcat-2.0.0/tests/test_basics.py
+-rw-rw-r--   0 atlas     (1000) atlas     (1000)     4332 2022-08-11 17:22:23.000000 rfcat-2.0.0/tests/test_bits.py
```

### Comparing `rfcat-1.9.7/CC-Bootloader/rfcat_bootloader` & `rfcat-2.0.0/CC-Bootloader/rfcat_bootloader`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/FAQ` & `rfcat-2.0.0/FAQ`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/LICENSE` & `rfcat-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/LICENSE.CC-Bootloader` & `rfcat-2.0.0/LICENSE.CC-Bootloader`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/PKG-INFO` & `rfcat-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfcat
-Version: 1.9.7
+Version: 2.0.0
 Summary: the swiss army knife of subGHz
 Home-page: https://github.com/atlas0fd00m/rfcat
 Author: atlas of d00m
 Author-email: atlas@r4780y.com
 License: UNKNOWN
 Download-URL: https://github.com/atlas0fd00m/rfcat/archive/v1.9.1.tar.gz
 Keywords: radio,subghz,cc1111,chipcon,hacking,reverse engineering
```

### Comparing `rfcat-1.9.7/README.immesniff` & `rfcat-2.0.0/README.immesniff`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/README.msfrelay` & `rfcat-2.0.0/README.msfrelay`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/README.nonroot` & `rfcat-2.0.0/README.nonroot`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/README.rst` & `rfcat-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/TODO` & `rfcat-2.0.0/TODO`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/etc/udev/rules.d/20-rfcat.rules` & `rfcat-2.0.0/etc/udev/rules.d/20-rfcat.rules`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/CCBootloader/CCBootloader-rfcat-chronosdongle.hex` & `rfcat-2.0.0/firmware/CCBootloader/CCBootloader-rfcat-chronosdongle.hex`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/CCBootloader/CCBootloader-rfcat-donsdongle.hex` & `rfcat-2.0.0/firmware/CCBootloader/CCBootloader-rfcat-donsdongle.hex`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/CCBootloader/CCBootloader-rfcat-ys1.hex` & `rfcat-2.0.0/firmware/CCBootloader/CCBootloader-rfcat-ys1.hex`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/Makefile` & `rfcat-2.0.0/firmware/Makefile`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/appCC2531.c` & `rfcat-2.0.0/firmware/appCC2531.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/appFHSSNIC.c` & `rfcat-2.0.0/firmware/appFHSSNIC.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/appNIC.c` & `rfcat-2.0.0/firmware/appNIC.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/appNetworkTest.c` & `rfcat-2.0.0/firmware/appNetworkTest.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/appSniff.c` & `rfcat-2.0.0/firmware/appSniff.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/application.c` & `rfcat-2.0.0/firmware/application.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/bootloader.c` & `rfcat-2.0.0/firmware/bootloader.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/bootloader_serial.py` & `rfcat-2.0.0/firmware/bootloader_serial.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/buildall.sh` & `rfcat-2.0.0/firmware/buildall.sh`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/cc1111_aes.c` & `rfcat-2.0.0/firmware/cc1111_aes.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/cc1111_vcom.c` & `rfcat-2.0.0/firmware/cc1111_vcom.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/cc1111_vcomdesc.c` & `rfcat-2.0.0/firmware/cc1111_vcomdesc.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/cc1111rf.c` & `rfcat-2.0.0/firmware/cc1111rf.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/chipcon_dma.c` & `rfcat-2.0.0/firmware/chipcon_dma.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/chipcon_usb.c` & `rfcat-2.0.0/firmware/chipcon_usb.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/chipcon_usbdebug.c` & `rfcat-2.0.0/firmware/chipcon_usbdebug.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/global.c` & `rfcat-2.0.0/firmware/global.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/immedisplay.c` & `rfcat-2.0.0/firmware/immedisplay.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/immefont.c` & `rfcat-2.0.0/firmware/immefont.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/immeio.c` & `rfcat-2.0.0/firmware/immeio.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/immekeys.c` & `rfcat-2.0.0/firmware/immekeys.c`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/FHSS.h` & `rfcat-2.0.0/firmware/include/FHSS.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/cc1110-ext.h` & `rfcat-2.0.0/firmware/include/cc1110-ext.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/cc1111.h` & `rfcat-2.0.0/firmware/include/cc1111.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/cc1111_aes.h` & `rfcat-2.0.0/firmware/include/cc1111_aes.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/cc1111_vcom.h` & `rfcat-2.0.0/firmware/include/cc1111_vcom.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/cc1111rf.h` & `rfcat-2.0.0/firmware/include/cc1111rf.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/cc2530-ext.h` & `rfcat-2.0.0/firmware/include/cc2530-ext.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/cc2531.h` & `rfcat-2.0.0/firmware/include/cc2531.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/chipcon_dma.h` & `rfcat-2.0.0/firmware/include/chipcon_dma.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/chipcon_usb.h` & `rfcat-2.0.0/firmware/include/chipcon_usb.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/global.h` & `rfcat-2.0.0/firmware/include/global.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/imme5x7.h` & `rfcat-2.0.0/firmware/include/imme5x7.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/immedisplay.h` & `rfcat-2.0.0/firmware/include/immedisplay.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/immeio.h` & `rfcat-2.0.0/firmware/include/immeio.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/immekeys.h` & `rfcat-2.0.0/firmware/include/immekeys.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/immeterm.h` & `rfcat-2.0.0/firmware/include/immeterm.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/include/nic.h` & `rfcat-2.0.0/firmware/include/nic.h`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/firmware/new_serial.py` & `rfcat-2.0.0/firmware/new_serial.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/package.sh` & `rfcat-2.0.0/package.sh`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rfcat` & `rfcat-2.0.0/rfcat`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rfcat.egg-info/PKG-INFO` & `rfcat-2.0.0/rfcat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfcat
-Version: 1.9.7
+Version: 2.0.0
 Summary: the swiss army knife of subGHz
 Home-page: https://github.com/atlas0fd00m/rfcat
 Author: atlas of d00m
 Author-email: atlas@r4780y.com
 License: UNKNOWN
 Download-URL: https://github.com/atlas0fd00m/rfcat/archive/v1.9.1.tar.gz
 Keywords: radio,subghz,cc1111,chipcon,hacking,reverse engineering
```

### Comparing `rfcat-1.9.7/rfcat.egg-info/SOURCES.txt` & `rfcat-2.0.0/rfcat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rfcat_msfrelay` & `rfcat-2.0.0/rfcat_msfrelay`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rfcat_server` & `rfcat-2.0.0/rfcat_server`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/__init__.py` & `rfcat-2.0.0/rflib/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,17 +216,21 @@
     lcls = locals()
     interact(lcls, gbls)
 
 def interact(lcls, gbls):
     shellexception = None
 
     try:
-        from IPython.terminal.interactiveshell import TerminalInteractiveShell
-        ipsh = TerminalInteractiveShell()
-        ipsh.user_global_ns.update(gbls)
+        import IPython
+        if IPython.core.getipython.get_ipython() is None:
+            ipsh = IPython.terminal.embed.InteractiveShellEmbed.instance()
+        else:
+            ipsh = IPython.terminal.embed.InteractiveShellEmbed()
+       
+        ipsh.user_global_ns.update(gbls)    
         ipsh.user_global_ns.update(lcls)
         ipsh.autocall = 2       # don't require parenthesis around *everything*.  be smart!
         ipsh.mainloop()
     except ImportError as e:
         shellexception = e
 
     if shellexception:
@@ -236,16 +240,19 @@
             ipsh.mainloop()
 
         except ImportError as e:
             shellexception = e
 
     if shellexception:
         try:
-            from IPython.frontend.terminal.interactiveshell import TerminalInteractiveShell
-            ipsh = TerminalInteractiveShell()
+            import IPython
+            if IPython.core.getipython.get_ipython() is None:
+                ipsh = IPython.terminal.embed.InteractiveShellEmbed.instance()
+            else:
+                ipsh = IPython.terminal.embed.InteractiveShellEmbed()
             ipsh.user_global_ns.update(gbls)
             ipsh.user_global_ns.update(lcls)
             ipsh.autocall = 2       # don't require parenthesis around *everything*.  be smart!
 
             ipsh.mainloop()
         except ImportError as e:
             shellexception = e
```

### Comparing `rfcat-1.9.7/rflib/bits.py` & `rfcat-2.0.0/rflib/bits.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/cc111Xhparser.py` & `rfcat-2.0.0/rflib/cc111Xhparser.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/ccspecan.py` & `rfcat-2.0.0/rflib/ccspecan.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/chipcon_nic.py` & `rfcat-2.0.0/rflib/chipcon_nic.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/chipcon_usb.py` & `rfcat-2.0.0/rflib/chipcon_usb.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/chipcondefs.py` & `rfcat-2.0.0/rflib/chipcondefs.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/const.py` & `rfcat-2.0.0/rflib/const.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/fakedongle_nic.py` & `rfcat-2.0.0/rflib/fakedongle_nic.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/intelhex.py` & `rfcat-2.0.0/rflib/intelhex.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/rflib_defs.py` & `rfcat-2.0.0/rflib/rflib_defs.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/vstruct/__init__.py` & `rfcat-2.0.0/rflib/vstruct/__init__.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/vstruct/builder.py` & `rfcat-2.0.0/rflib/vstruct/builder.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/rflib/vstruct/primitives.py` & `rfcat-2.0.0/rflib/vstruct/primitives.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/setup.py` & `rfcat-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/tests/test_api.py` & `rfcat-2.0.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `rfcat-1.9.7/tests/test_bits.py` & `rfcat-2.0.0/tests/test_bits.py`

 * *Files identical despite different names*

