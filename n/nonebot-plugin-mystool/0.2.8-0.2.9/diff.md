# Comparing `tmp/nonebot_plugin_mystool-0.2.8.tar.gz` & `tmp/nonebot_plugin_mystool-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mystool-0.2.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_mystool-0.2.9.tar", max compression
```

## Comparing `nonebot_plugin_mystool-0.2.8.tar` & `nonebot_plugin_mystool-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1065 2023-05-03 20:06:50.908427 nonebot_plugin_mystool-0.2.8/LICENSE
--rw-r--r--   0        0        0     3441 2023-05-03 20:06:50.908427 nonebot_plugin_mystool-0.2.8/README.md
--rw-r--r--   0        0        0     1317 2023-05-03 20:06:50.908427 nonebot_plugin_mystool-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2802 2023-05-03 20:06:50.908427 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/__init__.py
--rw-r--r--   0        0        0     2077 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/addFriend.py
--rw-r--r--   0        0        0     6938 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/address.py
--rw-r--r--   0        0        0    30682 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/bbsAPI.py
--rw-r--r--   0        0        0     7081 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/config.py
--rw-r--r--   0        0        0    15416 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/data.py
--rw-r--r--   0        0        0    22707 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/exchange.py
--rw-r--r--   0        0        0    19562 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/exchangePlan.py
--rw-r--r--   0        0        0    15573 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/gameSign.py
--rw-r--r--   0        0        0     1832 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/help.py
--rw-r--r--   0        0        0    14907 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/login.py
--rw-r--r--   0        0        0    23334 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/mybMission.py
--rw-r--r--   0        0        0    23885 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/plan.py
--rw-r--r--   0        0        0     9815 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/setting.py
--rw-r--r--   0        0        0    10836 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/utils.py
--rw-r--r--   0        0        0     4867 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2820 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/README.md
+-rw-r--r--   0        0        0     1317 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2802 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/__init__.py
+-rw-r--r--   0        0        0     2077 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/addFriend.py
+-rw-r--r--   0        0        0     6938 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/address.py
+-rw-r--r--   0        0        0    30682 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/bbsAPI.py
+-rw-r--r--   0        0        0     7081 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/config.py
+-rw-r--r--   0        0        0    15416 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/data.py
+-rw-r--r--   0        0        0    22944 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/exchange.py
+-rw-r--r--   0        0        0    20570 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/exchangePlan.py
+-rw-r--r--   0        0        0    15573 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/gameSign.py
+-rw-r--r--   0        0        0     1884 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/help.py
+-rw-r--r--   0        0        0    14907 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/login.py
+-rw-r--r--   0        0        0    23334 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/mybMission.py
+-rw-r--r--   0        0        0    24358 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/plan.py
+-rw-r--r--   0        0        0     9827 2023-05-18 07:37:15.787978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/setting.py
+-rw-r--r--   0        0        0    11531 2023-05-18 07:37:15.791978 nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/utils.py
+-rw-r--r--   0        0        0     4246 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-0.2.9/PKG-INFO
```

### Comparing `nonebot_plugin_mystool-0.2.8/LICENSE` & `nonebot_plugin_mystool-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.8/README.md` & `nonebot_plugin_mystool-0.2.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -18,199 +18,160 @@
 00000110: 5f5f 5c20 205c 205c 5f5f 5f5f 5f5c 2020  __\  \ \_____\  
 00000120: 5c20 5c5f 5f5f 5f5f 5c0a 2020 5c2f 5f2f  \ \_____\.  \/_/
 00000130: 2020 5c2f 5f2f 2020 205c 2f5f 5f5f 5f5f    \/_/   \/_____
 00000140: 2f20 2020 5c2f 5f5f 5f5f 5f2f 2020 2020  /   \/_____/    
 00000150: 205c 2f5f 2f20 2020 5c2f 5f5f 5f5f 5f2f   \/_/   \/_____/
 00000160: 2020 205c 2f5f 5f5f 5f5f 2f20 2020 5c2f     \/_____/   \/
 00000170: 5f5f 5f5f 5f2f 0a60 6060 0a0a 3c64 6976  _____/.```..<div
-00000180: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
-00000190: 7073 3a2f 2f77 7777 2e63 6f64 6566 6163  ps://www.codefac
-000001a0: 746f 722e 696f 2f72 6570 6f73 6974 6f72  tor.io/repositor
-000001b0: 792f 6769 7468 7562 2f6c 6a7a 642d 7072  y/github/ljzd-pr
-000001c0: 6f2f 6e6f 6e65 626f 742d 706c 7567 696e  o/nonebot-plugin
-000001d0: 2d6d 7973 746f 6f6c 2220 7461 7267 6574  -mystool" target
-000001e0: 3d22 5f62 6c61 6e6b 223e 0a20 2020 203c  ="_blank">.    <
-000001f0: 696d 6720 616c 743d 2243 6f64 6546 6163  img alt="CodeFac
-00000200: 746f 7222 2073 7263 3d22 6874 7470 733a  tor" src="https:
-00000210: 2f2f 7777 772e 636f 6465 6661 6374 6f72  //www.codefactor
-00000220: 2e69 6f2f 7265 706f 7369 746f 7279 2f67  .io/repository/g
-00000230: 6974 6875 622f 6c6a 7a64 2d70 726f 2f6e  ithub/ljzd-pro/n
-00000240: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
-00000250: 7374 6f6f 6c2f 6261 6467 653f 7374 796c  stool/badge?styl
-00000260: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
-00000270: 3e0a 2020 3c2f 613e 0a20 203c 6120 6872  >.  </a>.  <a hr
-00000280: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00000290: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
-000002a0: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
-000002b0: 7973 746f 6f6c 2f72 656c 6561 7365 732f  ystool/releases/
-000002c0: 6c61 7465 7374 2220 7461 7267 6574 3d22  latest" target="
-000002d0: 5f62 6c61 6e6b 223e 0a20 2020 203c 696d  _blank">.    <im
-000002e0: 6720 616c 743d 22e6 9c80 e696 b0e5 8f91  g alt=".........
-000002f0: e8a1 8ce7 8988 2220 7372 633d 2268 7474  ......" src="htt
-00000300: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000310: 2e69 6f2f 6769 7468 7562 2f76 2f72 656c  .io/github/v/rel
-00000320: 6561 7365 2f4c 6a7a 642d 5052 4f2f 6e6f  ease/Ljzd-PRO/no
-00000330: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
-00000340: 546f 6f6c 3f6c 6f67 6f3d 7079 7468 6f6e  Tool?logo=python
-00000350: 2673 7479 6c65 3d66 6f72 2d74 6865 2d62  &style=for-the-b
-00000360: 6164 6765 223e 0a20 203c 2f61 3e0a 2020  adge">.  </a>.  
-00000370: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000380: 2f67 6974 6875 622e 636f 6d2f 4c6a 7a64  /github.com/Ljzd
-00000390: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
-000003a0: 6769 6e2d 6d79 7374 6f6f 6c2f 636f 6d6d  gin-mystool/comm
-000003b0: 6974 732f 2220 7461 7267 6574 3d22 5f62  its/" target="_b
-000003c0: 6c61 6e6b 223e 0a20 2020 203c 696d 6720  lank">.    <img 
-000003d0: 616c 743d 22e6 9c80 e590 8ee6 8f90 e4ba  alt="...........
-000003e0: a422 2073 7263 3d22 6874 7470 733a 2f2f  ." src="https://
-000003f0: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
-00000400: 6974 6875 622f 6c61 7374 2d63 6f6d 6d69  ithub/last-commi
-00000410: 742f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  t/Ljzd-PRO/noneb
-00000420: 6f74 2d70 6c75 6769 6e2d 6d79 7354 6f6f  ot-plugin-mysToo
-00000430: 6c3f 7374 796c 653d 666f 722d 7468 652d  l?style=for-the-
-00000440: 6261 6467 6522 3e0a 2020 3c2f 613e 0a3c  badge">.  </a>.<
-00000450: 2f64 6976 3e0a 0a23 206d 7973 546f 6f6c  /div>..# mysTool
-00000460: 202d 20e7 b1b3 e6b8 b8e7 a4be e8be 85e5   - .............
-00000470: 8aa9 e5b7 a5e5 85b7 e68f 92e4 bbb6 0a0a  ................
-00000480: 2a2a e789 88e6 9cac 202d 2076 302e 322e  **...... - v0.2.
-00000490: 382a 2a0a 0a23 2323 20f0 9f93 a320 e69b  8**..### .... ..
-000004a0: b4e6 96b0 e586 85e5 aeb9 0a0a 2323 2323  ............####
-000004b0: 2032 3032 332e 352e 340a 2d20 e5a2 9ee5   2023.5.4.- ....
-000004c0: 8aa0 e5af b9e6 989f e7a9 b9e9 9381 e981  ................
-000004d0: 93e7 9a84 e7ad bee5 88b0 e58a 9fe8 83bd  ................
-000004e0: e79a 84e6 94af e68c 8120 2d20 5b23 3839  ......... - [#89
-000004f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000500: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
-00000510: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
-00000520: 746f 6f6c 2f70 756c 6c2f 3839 2920 6279  tool/pull/89) by
-00000530: 2040 6179 616b 6173 756b 690a 2d20 e4bf   @ayakasuki.- ..
-00000540: aee5 a48d e68f 92e4 bbb6 e591 bde4 bba4  ................
-00000550: e4bc 98e5 8588 e5ba a6e9 97ae e9a2 9820  ............... 
-00000560: 2d20 5b23 3838 5d28 6874 7470 733a 2f2f  - [#88](https://
-00000570: 6769 7468 7562 2e63 6f6d 2f4c 6a7a 642d  github.com/Ljzd-
-00000580: 5052 4f2f 6e6f 6e65 626f 742d 706c 7567  PRO/nonebot-plug
-00000590: 696e 2d6d 7973 746f 6f6c 2f70 756c 6c2f  in-mystool/pull/
-000005a0: 3838 2920 6279 2040 6179 616b 6173 756b  88) by @ayakasuk
-000005b0: 690a 2d20 e983 a8e5 8886 e696 87e6 9cac  i.- ............
-000005c0: e994 99e8 afaf e4bf aee6 ada3 202d 205b  ............ - [
-000005d0: 2339 305d 2868 7474 7073 3a2f 2f67 6974  #90](https://git
-000005e0: 6875 622e 636f 6d2f 4c6a 7a64 2d50 524f  hub.com/Ljzd-PRO
-000005f0: 2f6e 6f6e 6562 6f74 2d70 6c75 6769 6e2d  /nonebot-plugin-
-00000600: 6d79 7374 6f6f 6c2f 7075 6c6c 2f39 3029  mystool/pull/90)
-00000610: 2062 7920 4062 6c61 636b 2d7a 6572 6f33   by @black-zero3
-00000620: 3538 0a0a 2323 2323 2032 3032 332e 342e  58..#### 2023.4.
-00000630: 3238 0a2d 20e4 bfae e5a4 8de6 8f92 e4bb  28.- ...........
-00000640: b6e5 91bd e4bb a4e8 a2ab e585 b6e4 bb96  ................
-00000650: 206e 6f6e 6562 6f74 20e6 8f92 e4bb b6e6   nonebot .......
-00000660: 8d95 e88e b7e7 9a84 e997 aee9 a298 0a2d  ...............-
-00000670: 20e5 a29e e58a a0e6 94af e68c 81e6 989f   ...............
-00000680: e7a9 b9e9 9381 e981 93e7 9a84 e595 86e5  ................
-00000690: 9381 e585 91e6 8da2 0a2d 20e6 af8f e697  .........- .....
-000006a0: a5e7 adbe e588 b0e3 8081 e7b1 b3e6 b8b8  ................
-000006b0: e5b8 81e4 bbbb e58a a1e6 89a7 e8a1 8ce6  ................
-000006c0: 97b6 e997 b4e5 9ca8 e794 a8e6 88b7 e985  ................
-000006d0: 8de7 bdae e79a 84e5 9fba e7a1 80e4 b88a  ................
-000006e0: e5a2 9ee5 8aa0 e99a 8fe6 9cba e5bb b6e8  ................
-000006f0: bf9f 0a2d 20e4 bfae e5a4 8de5 a4a7 e588  ...- ...........
-00000700: abe9 878e e9a2 91e9 8193 e6af 8fe6 97a5  ................
-00000710: e4bb bbe5 8aa1 e380 81e7 adbe e588 b0e6  ................
-00000720: 89a7 e8a1 8ce5 a4b1 e8b4 a5e7 9a84 e997  ................
-00000730: aee9 a298 0a0a 2323 2323 2032 3032 332e  ......#### 2023.
-00000740: 332e 3330 0a2d 20e4 bfae e5a4 8de9 878d  3.30.- .........
-00000750: e586 99e9 858d e7bd aee6 9687 e4bb b620  ............... 
-00000760: 6070 6c75 6769 6e43 6f6e 6669 672e 6a73  `pluginConfig.js
-00000770: 6f6e 6020 e4b8 8de7 949f e695 88e7 9a84  on` ............
-00000780: e997 aee9 a298 0a2d 20e4 bfae e5a4 8de5  .......- .......
-00000790: 8d95 e8b4 a6e6 88b7 e683 85e5 86b5 e4b8  ................
-000007a0: 8be6 97a0 e6b3 95e5 a29e e588 a0e5 8591  ................
-000007b0: e68d a2e8 aea1 e588 92e7 9a84 e997 aee9  ................
-000007c0: a298 0a2d 20e4 bfae e5a4 8d20 602f e585  ...- ...... `/..
-000007d0: 91e6 8da2 6020 e591 bde4 bba4 e58f afe8  ....` ..........
-000007e0: 83bd e4b8 8ee5 85b6 e4bb 96e6 8f92 e4bb  ................
-000007f0: b6e5 91bd e4bb a4e5 86b2 e7aa 81e7 9a84  ................
-00000800: e997 aee9 a298 efbc 8ce5 908c e697 b620  ............... 
-00000810: 5bf0 9f94 97e7 94a8 e6b3 95e5 8f98 e69b  [...............
-00000820: b45d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
-00000830: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
-00000840: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
-00000850: 7374 6f6f 6c2f 7769 6b69 2f49 6e66 6f72  stool/wiki/Infor
-00000860: 6d61 7469 6f6e 2d45 7863 6861 6e67 6523  mation-Exchange#
-00000870: e5a2 9ee5 8aa0 e588 a0e9 99a4 e585 91e6  ................
-00000880: 8da2 e8ae a1e5 8892 290a 2d20 e7b2 bee7  ........).- ....
-00000890: ae80 e68e a5e6 94b6 e79a 84e5 91bd e4bb  ................
-000008a0: a40a 2d20 e69b b4e6 ada3 2060 6465 7669  ..- ...... `devi
-000008b0: 6365 5f73 6176 6560 2022 e8ae bee5 a487  ce_save` "......
-000008c0: e4bf 9de5 ad98 2220 e697 a5e5 bf97 e696  ......" ........
-000008d0: 87e6 9cac e79a 84e9 9499 e8af af0a 0a23  ...............#
-000008e0: 2320 e58a 9fe8 83bd e592 8ce7 89b9 e680  # ..............
-000008f0: a70a 0a2d 20e7 9fad e4bf a1e9 aa8c e8af  ...- ...........
-00000900: 81e7 99bb e5bd 95ef bc8c e585 8de6 8a93  ................
-00000910: e58c 85e8 8eb7 e58f 9620 436f 6f6b 6965  ......... Cookie
-00000920: 0a2d 20e8 87aa e58a a8e5 ae8c e688 90e6  .- .............
-00000930: af8f e697 a5e7 b1b3 e6b8 b8e5 b881 e4bb  ................
-00000940: bbe5 8aa1 0a2d 20e8 87aa e58a a8e8 bf9b  .....- .........
-00000950: e8a1 8ce6 b8b8 e688 8fe7 adbe e588 b00a  ................
-00000960: 2d20 e58f afe5 88b6 e5ae 9ae7 b1b3 e6b8  - ..............
-00000970: b8e5 b881 e595 86e5 9381 e585 91e6 8da2  ................
-00000980: e8ae a1e5 8892 efbc 8ce5 88b0 e782 b9e5  ................
-00000990: 8591 e68d a20a 2d20 e58f afe6 94af e68c  ......- ........
-000009a0: 81e5 a49a e4b8 aa20 5151 20e8 b4a6 e58f  ....... QQ .....
-000009b0: b7ef bc8c e6af 8fe4 b8aa 2051 5120 e8b4  .......... QQ ..
-000009c0: a6e5 8fb7 e58f afe7 bb91 e5ae 9ae5 a49a  ................
-000009d0: e4b8 aae7 b1b3 e593 88e6 b8b8 e8b4 a6e6  ................
-000009e0: 88b7 0a2d 2051 5120 e68e a8e9 8081 e689  ...- QQ ........
-000009f0: a7e8 a18c e7bb 93e6 9e9c e980 9ae7 9fa5  ................
-00000a00: 0a2d 20e5 8e9f e7a5 9ee6 a091 e884 82e3  .- .............
-00000a10: 8081 e6b4 9ee5 a4a9 e5ae 9de9 92b1 e380  ................
-00000a20: 81e8 b4a8 e987 8fe5 8f82 e58f 98e4 bbaa  ................
-00000a30: e5b7 b2e6 bba1 e697 b6e6 8ea8 e980 81e9  ................
-00000a40: 809a e79f a50a 0a23 2320 e4bd bfe7 94a8  .......## ......
-00000a50: e8af b4e6 988e 0a0a 2323 2320 f09f 9ba0  ........### ....
-00000a60: efb8 8f20 4e6f 6e65 426f 7432 20e6 9cba  ... NoneBot2 ...
-00000a70: e599 a8e4 baba e983 a8e7 bdb2 e592 8ce6  ................
-00000a80: 8f92 e4bb b6e5 ae89 e8a3 850a 0ae8 afb7  ................
-00000a90: e69f a5e7 9c8b 202d 3e20 5bf0 9f94 9749  ...... -> [....I
-00000aa0: 6e73 7461 6c6c 6174 696f 6e5d 2868 7474  nstallation](htt
-00000ab0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000ac0: 4c6a 7a64 2d50 524f 2f6e 6f6e 6562 6f74  Ljzd-PRO/nonebot
-00000ad0: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c2f  -plugin-mystool/
-00000ae0: 7769 6b69 2f49 6e73 7461 6c6c 6174 696f  wiki/Installatio
-00000af0: 6e29 0a0a 2323 2320 f09f 9396 20e6 8f92  n)..### .... ...
-00000b00: e4bb b6e5 85b7 e4bd 93e4 bdbf e794 a8e8  ................
-00000b10: afb4 e698 8e0a 0ae8 afb7 e69f a5e7 9c8b  ................
-00000b20: 202d 3e20 5bf0 9f94 9757 696b 6920 e696   -> [....Wiki ..
-00000b30: 87e6 a1a3 5d28 6874 7470 733a 2f2f 6769  ....](https://gi
-00000b40: 7468 7562 2e63 6f6d 2f4c 6a7a 642d 5052  thub.com/Ljzd-PR
-00000b50: 4f2f 6e6f 6e65 626f 742d 706c 7567 696e  O/nonebot-plugin
-00000b60: 2d6d 7973 746f 6f6c 2f77 696b 6929 0a0a  -mystool/wiki)..
-00000b70: 2323 2320 e29d 9320 e88e b7e5 8f96 e68f  ### ... ........
-00000b80: 92e4 bbb6 e5b8 aee5 8aa9 e4bf a1e6 81af  ................
-00000b90: 0a0a 2323 2323 20e6 8f92 e4bb b6e5 91bd  ..#### .........
-00000ba0: e4bb a40a 0a60 6060 0a2f e5b8 aee5 8aa9  .....```./......
-00000bb0: 0a60 6060 0a0a 3e20 e29a a0ef b88f 20e6  .```..> ...... .
-00000bc0: b3a8 e684 8f20 e6ad a4e5 a484 e6b2 a1e6  ..... ..........
-00000bd0: 9c89 e4bd bfe7 94a8 205b f09f 9497 20e6  ........ [.... .
-00000be0: 8f92 e4bb b6e5 91bd e4bb a4e5 a4b4 5d28  ..............](
-00000bf0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000c00: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
-00000c10: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
-00000c20: 6f6c 2f77 696b 692f 436f 6e66 6967 7572  ol/wiki/Configur
-00000c30: 6174 696f 6e2d 436f 6e66 6967 2363 6f6d  ation-Config#com
-00000c40: 6d61 6e64 5f73 7461 7274 290a 0a23 2320  mand_start)..## 
-00000c50: e585 b6e4 bb96 0a0a 2323 2320 5bf0 9f93  ........### [...
-00000c60: 83e6 ba90 e7a0 81e8 afb4 e698 8e5d 2868  .............](h
-00000c70: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000c80: 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  m/Ljzd-PRO/noneb
-00000c90: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
-00000ca0: 6c2f 7769 6b69 2f53 6f75 7263 652d 5374  l/wiki/Source-St
-00000cb0: 7275 6374 7572 6529 0a23 2323 20e9 8082  ructure).### ...
-00000cc0: e985 8d20 5be7 bbaa e5b1 b1e7 9c9f e5af  ... [...........
-00000cd0: bb42 6f74 5d28 6874 7470 733a 2f2f 6769  .Bot](https://gi
-00000ce0: 7468 7562 2e63 6f6d 2f48 6962 694b 6965  thub.com/HibiKie
-00000cf0: 722f 7a68 656e 7875 6e5f 626f 7429 20e7  r/zhenxun_bot) .
-00000d00: 9a84 e588 86e6 94af 0a2d 2068 7474 7073  .........- https
-00000d10: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d57  ://github.com/MW
-00000d20: 544a 432f 7a68 656e 7875 6e2d 706c 7567  TJC/zhenxun-plug
-00000d30: 696e 2d6d 7973 746f 6f6c 0a2d 2068 7474  in-mystool.- htt
-00000d40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000d50: 6179 616b 6173 756b 692f 6e6f 6e65 626f  ayakasuki/nonebo
-00000d60: 742d 706c 7567 696e 2d6d 7973 746f 6f6c  t-plugin-mystool
-00000d70: 0a                                       .
+00000180: 3e0a 2020 3c69 6d67 2061 6c74 3d22 436f  >.  <img alt="Co
+00000190: 6465 4661 6374 6f72 2220 7372 633d 2268  deFactor" src="h
+000001a0: 7474 7073 3a2f 2f77 7777 2e63 6f64 6566  ttps://www.codef
+000001b0: 6163 746f 722e 696f 2f72 6570 6f73 6974  actor.io/reposit
+000001c0: 6f72 792f 6769 7468 7562 2f6c 6a7a 642d  ory/github/ljzd-
+000001d0: 7072 6f2f 6e6f 6e65 626f 742d 706c 7567  pro/nonebot-plug
+000001e0: 696e 2d6d 7973 746f 6f6c 2f62 6164 6765  in-mystool/badge
+000001f0: 3f73 7479 6c65 3d66 6f72 2d74 6865 2d62  ?style=for-the-b
+00000200: 6164 6765 223e 0a20 203c 696d 6720 616c  adge">.  <img al
+00000210: 743d 22e6 9c80 e696 b0e5 8f91 e8a1 8ce7  t=".............
+00000220: 8988 2220 7372 633d 2268 7474 7073 3a2f  .." src="https:/
+00000230: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000240: 6769 7468 7562 2f76 2f72 656c 6561 7365  github/v/release
+00000250: 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65 626f  /Ljzd-PRO/nonebo
+00000260: 742d 706c 7567 696e 2d6d 7973 546f 6f6c  t-plugin-mysTool
+00000270: 3f6c 6f67 6f3d 7079 7468 6f6e 2673 7479  ?logo=python&sty
+00000280: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+00000290: 223e 0a20 203c 696d 6720 616c 743d 22e6  ">.  <img alt=".
+000002a0: 9c80 e590 8ee6 8f90 e4ba a422 2073 7263  ..........." src
+000002b0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000002c0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+000002d0: 6c61 7374 2d63 6f6d 6d69 742f 4c6a 7a64  last-commit/Ljzd
+000002e0: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
+000002f0: 6769 6e2d 6d79 7354 6f6f 6c3f 7374 796c  gin-mysTool?styl
+00000300: 653d 666f 722d 7468 652d 6261 6467 6522  e=for-the-badge"
+00000310: 3e0a 3c2f 6469 763e 0a0a 2320 6d79 7354  >.</div>..# mysT
+00000320: 6f6f 6c20 2d20 e7b1 b3e6 b8b8 e7a4 bee8  ool - ..........
+00000330: be85 e58a a9e5 b7a5 e585 b7e6 8f92 e4bb  ................
+00000340: b60a 0a2a 2ae7 8988 e69c ac20 2d20 7630  ...**...... - v0
+00000350: 2e32 2e39 2a2a 0a0a 2323 2320 f09f 93a3  .2.9**..### ....
+00000360: 20e6 9bb4 e696 b0e5 8685 e5ae b90a 0a23   ..............#
+00000370: 2323 2320 3230 3233 2e35 2e31 380a 2d20  ### 2023.5.18.- 
+00000380: e5a4 9ae8 bf9b e7a8 8be7 949f e688 90e5  ................
+00000390: 9586 e593 81e5 9bbe e789 87ef bc88 e5a4  ................
+000003a0: 9ae6 a0b8 efbc 89ef bc8c e58a a0e5 bfab  ................
+000003b0: e59b bee7 8987 e794 9fe6 8890 e980 9fe5  ................
+000003c0: baa6 0a2d 20e4 bfae e5a4 8de9 83a8 e588  ...- ...........
+000003d0: 86e5 9586 e593 81e5 8591 e68d a2e6 97b6  ................
+000003e0: e997 b4e9 9499 e8af afe7 9a84 e997 aee9  ................
+000003f0: a298 efbc 88e5 a682 e7b1 b3e6 b8b8 e7a4  ................
+00000400: bee5 9586 e593 81e6 999a e4ba 86e4 b880  ................
+00000410: e591 a8ef bc89 0a0a 2323 2323 2032 3032  ........#### 202
+00000420: 332e 352e 340a 2d20 e5a2 9ee5 8aa0 e5af  3.5.4.- ........
+00000430: b9e6 989f e7a9 b9e9 9381 e981 93e7 9a84  ................
+00000440: e7ad bee5 88b0 e58a 9fe8 83bd e79a 84e6  ................
+00000450: 94af e68c 8120 2d20 5b23 3839 5d28 6874  ..... - [#89](ht
+00000460: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000470: 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65 626f  /Ljzd-PRO/nonebo
+00000480: 742d 706c 7567 696e 2d6d 7973 746f 6f6c  t-plugin-mystool
+00000490: 2f70 756c 6c2f 3839 2920 6279 2040 6179  /pull/89) by @ay
+000004a0: 616b 6173 756b 690a 2d20 e4bf aee5 a48d  akasuki.- ......
+000004b0: e68f 92e4 bbb6 e591 bde4 bba4 e4bc 98e5  ................
+000004c0: 8588 e5ba a6e9 97ae e9a2 9820 2d20 5b23  ........... - [#
+000004d0: 3838 5d28 6874 7470 733a 2f2f 6769 7468  88](https://gith
+000004e0: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
+000004f0: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
+00000500: 7973 746f 6f6c 2f70 756c 6c2f 3838 2920  ystool/pull/88) 
+00000510: 6279 2040 6179 616b 6173 756b 690a 2d20  by @ayakasuki.- 
+00000520: e983 a8e5 8886 e696 87e6 9cac e994 99e8  ................
+00000530: afaf e4bf aee6 ada3 202d 205b 2339 305d  ........ - [#90]
+00000540: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000550: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
+00000560: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
+00000570: 6f6f 6c2f 7075 6c6c 2f39 3029 2062 7920  ool/pull/90) by 
+00000580: 4062 6c61 636b 2d7a 6572 6f33 3538 0a0a  @black-zero358..
+00000590: 2e2e 2e0a 0a23 2323 2320 3230 3233 2e33  .....#### 2023.3
+000005a0: 2e33 300a 2d20 e4bf aee5 a48d 2060 2fe5  .30.- ...... `/.
+000005b0: 8591 e68d a260 20e5 91bd e4bb a4e5 8faf  .....` .........
+000005c0: e883 bde4 b88e e585 b6e4 bb96 e68f 92e4  ................
+000005d0: bbb6 e591 bde4 bba4 e586 b2e7 aa81 e79a  ................
+000005e0: 84e9 97ae e9a2 98ef bc8c e590 8ce6 97b6  ................
+000005f0: 205b f09f 9497 e794 a8e6 b395 e58f 98e6   [..............
+00000600: 9bb4 5d28 6874 7470 733a 2f2f 6769 7468  ..](https://gith
+00000610: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
+00000620: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
+00000630: 7973 746f 6f6c 2f77 696b 692f 496e 666f  ystool/wiki/Info
+00000640: 726d 6174 696f 6e2d 4578 6368 616e 6765  rmation-Exchange
+00000650: 23e5 a29e e58a a0e5 88a0 e999 a4e5 8591  #...............
+00000660: e68d a2e8 aea1 e588 9229 0a2d 202e 2e2e  .........).- ...
+00000670: 0a0a 2323 20e5 8a9f e883 bde5 928c e789  ..## ...........
+00000680: b9e6 80a7 0a0a 2d20 e79f ade4 bfa1 e9aa  ......- ........
+00000690: 8ce8 af81 e799 bbe5 bd95 efbc 8ce5 858d  ................
+000006a0: e68a 93e5 8c85 e88e b7e5 8f96 2043 6f6f  ............ Coo
+000006b0: 6b69 650a 2d20 e887 aae5 8aa8 e5ae 8ce6  kie.- ..........
+000006c0: 8890 e6af 8fe6 97a5 e7b1 b3e6 b8b8 e5b8  ................
+000006d0: 81e4 bbbb e58a a10a 2d20 e887 aae5 8aa8  ........- ......
+000006e0: e8bf 9be8 a18c e6b8 b8e6 888f e7ad bee5  ................
+000006f0: 88b0 0a2d 20e5 8faf e588 b6e5 ae9a e7b1  ...- ...........
+00000700: b3e6 b8b8 e5b8 81e5 9586 e593 81e5 8591  ................
+00000710: e68d a2e8 aea1 e588 92ef bc8c e588 b0e7  ................
+00000720: 82b9 e585 91e6 8da2 0a2d 20e5 8faf e694  .........- .....
+00000730: afe6 8c81 e5a4 9ae4 b8aa 2051 5120 e8b4  .......... QQ ..
+00000740: a6e5 8fb7 efbc 8ce6 af8f e4b8 aa20 5151  ............. QQ
+00000750: 20e8 b4a6 e58f b7e5 8faf e7bb 91e5 ae9a   ...............
+00000760: e5a4 9ae4 b8aa e7b1 b3e5 9388 e6b8 b8e8  ................
+00000770: b4a6 e688 b70a 2d20 5151 20e6 8ea8 e980  ......- QQ .....
+00000780: 81e6 89a7 e8a1 8ce7 bb93 e69e 9ce9 809a  ................
+00000790: e79f a50a 2d20 e58e 9fe7 a59e e6a0 91e8  ....- ..........
+000007a0: 8482 e380 81e6 b49e e5a4 a9e5 ae9d e992  ................
+000007b0: b1e3 8081 e8b4 a8e9 878f e58f 82e5 8f98  ................
+000007c0: e4bb aae5 b7b2 e6bb a1e6 97b6 e68e a8e9  ................
+000007d0: 8081 e980 9ae7 9fa5 0a0a 2323 20e4 bdbf  ..........## ...
+000007e0: e794 a8e8 afb4 e698 8e0a 0a23 2323 20f0  ...........### .
+000007f0: 9f9b a0ef b88f 204e 6f6e 6542 6f74 3220  ...... NoneBot2 
+00000800: e69c bae5 99a8 e4ba bae9 83a8 e7bd b2e5  ................
+00000810: 928c e68f 92e4 bbb6 e5ae 89e8 a385 0a0a  ................
+00000820: e8af b7e6 9fa5 e79c 8b20 2d3e 205b f09f  ......... -> [..
+00000830: 9497 496e 7374 616c 6c61 7469 6f6e 5d28  ..Installation](
+00000840: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000850: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
+00000860: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
+00000870: 6f6c 2f77 696b 692f 496e 7374 616c 6c61  ol/wiki/Installa
+00000880: 7469 6f6e 290a 0a23 2323 20f0 9f93 9620  tion)..### .... 
+00000890: e68f 92e4 bbb6 e585 b7e4 bd93 e4bd bfe7  ................
+000008a0: 94a8 e8af b4e6 988e 0a0a e8af b7e6 9fa5  ................
+000008b0: e79c 8b20 2d3e 205b f09f 9497 5769 6b69  ... -> [....Wiki
+000008c0: 20e6 9687 e6a1 a35d 2868 7474 7073 3a2f   ......](https:/
+000008d0: 2f67 6974 6875 622e 636f 6d2f 4c6a 7a64  /github.com/Ljzd
+000008e0: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
+000008f0: 6769 6e2d 6d79 7374 6f6f 6c2f 7769 6b69  gin-mystool/wiki
+00000900: 290a 0a23 2323 20e2 9d93 20e8 8eb7 e58f  )..### ... .....
+00000910: 96e6 8f92 e4bb b6e5 b8ae e58a a9e4 bfa1  ................
+00000920: e681 af0a 0a23 2323 2320 e68f 92e4 bbb6  .....#### ......
+00000930: e591 bde4 bba4 0a0a 6060 600a 2fe5 b8ae  ........```./...
+00000940: e58a a90a 6060 600a 0a3e 20e2 9aa0 efb8  ....```..> .....
+00000950: 8f20 e6b3 a8e6 848f 20e6 ada4 e5a4 84e6  . ...... .......
+00000960: b2a1 e69c 89e4 bdbf e794 a820 5bf0 9f94  ........... [...
+00000970: 9720 e68f 92e4 bbb6 e591 bde4 bba4 e5a4  . ..............
+00000980: b45d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
+00000990: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+000009a0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+000009b0: 7374 6f6f 6c2f 7769 6b69 2f43 6f6e 6669  stool/wiki/Confi
+000009c0: 6775 7261 7469 6f6e 2d43 6f6e 6669 6723  guration-Config#
+000009d0: 636f 6d6d 616e 645f 7374 6172 7429 0a0a  command_start)..
+000009e0: 2323 20e5 85b6 e4bb 960a 0a23 2323 205b  ## ........### [
+000009f0: f09f 9383 e6ba 90e7 a081 e8af b4e6 988e  ................
+00000a00: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000a10: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
+00000a20: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
+00000a30: 746f 6f6c 2f77 696b 692f 536f 7572 6365  tool/wiki/Source
+00000a40: 2d53 7472 7563 7475 7265 290a 2323 2320  -Structure).### 
+00000a50: e980 82e9 858d 205b e7bb aae5 b1b1 e79c  ...... [........
+00000a60: 9fe5 afbb 426f 745d 2868 7474 7073 3a2f  ....Bot](https:/
+00000a70: 2f67 6974 6875 622e 636f 6d2f 4869 6269  /github.com/Hibi
+00000a80: 4b69 6572 2f7a 6865 6e78 756e 5f62 6f74  Kier/zhenxun_bot
+00000a90: 2920 e79a 84e5 8886 e694 af0a 2d20 6874  ) ..........- ht
+00000aa0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000ab0: 2f4d 5754 4a43 2f7a 6865 6e78 756e 2d70  /MWTJC/zhenxun-p
+00000ac0: 6c75 6769 6e2d 6d79 7374 6f6f 6c0a 2d20  lugin-mystool.- 
+00000ad0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000ae0: 6f6d 2f61 7961 6b61 7375 6b69 2f6e 6f6e  om/ayakasuki/non
+00000af0: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
+00000b00: 6f6f 6c0a                                ool.
```

### Comparing `nonebot_plugin_mystool-0.2.8/pyproject.toml` & `nonebot_plugin_mystool-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mystool"
-version = "v0.2.8"
+version = "v0.2.9"
 description = "NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒"
 license = "MIT"
 authors = [
   "Ljzd-PRO <ljzd@office.ljzd-pro.ml>",
   "Everything0519 <598139245@qq.com>"
 ]
 readme = "README.md"
@@ -24,15 +24,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 httpx = "^0.24.0"
 nonebot_plugin_apscheduler = ">=0.2.0"
 ntplib = "^0.4.0"
 Pillow = "^9.5.0"
-requests = "^2.29.0"
+requests = "^2.30.0"
 nonebot_adapter_onebot = "^2.2.3"
 tenacity = "^8.2.2"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Ljzd-PRO/nonebot-plugin-mystool/issues"
 
 [build-system]
```

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/__init__.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 # mysTool - 米游社辅助工具插件
 
-**版本 - v0.2.8**
+**版本 - v0.2.9**
 
 ## 使用说明
 
 ### 🛠️ NoneBot2 机器人部署和插件安装
 
 请查看 -> [🔗Installation](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Installation)
 
@@ -35,15 +35,15 @@
 import pkgutil
 from pathlib import Path
 
 from nonebot.plugin import PluginMetadata
 
 from .data import create_files
 
-VERSION = "v0.2.8"
+VERSION = "v0.2.9"
 '''插件版本号'''
 
 __plugin_meta__ = PluginMetadata(
     name=f"❖米游社小助手插件❖\n版本 - {VERSION}\n",
     description="米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录\n",
     usage="""
     \n🔐 {HEAD}登录 ➢ 登录绑定米游社账户\
```

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/addFriend.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/addFriend.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/address.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/address.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/bbsAPI.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/bbsAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/config.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/data.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/exchange.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 ### 米游币兑换相关
 """
 import io
 import os
 import time
 import traceback
 import zipfile
+from multiprocessing import Lock
 from typing import List, Literal, NewType, Tuple, Union, Optional
 
 import httpx
 import tenacity
 from PIL import Image, ImageDraw, ImageFont
 
 from .bbsAPI import GameRecord, get_game_record
@@ -143,19 +144,17 @@
         return self.good_dict["price"]
 
     @property
     def time(self) -> Optional[int]:
         """
         兑换时间
         """
-        # "next_time" 为 0 表示任何时间均可兑换或兑换已结束
-        # "type" 为 1 时商品只有在指定时间开放兑换；为 0 时商品任何时间均可兑换
         if self.good_dict["type"] != 1 and self.good_dict["next_time"] == 0:
             return None
-        elif "sale_start_time" in self.good_dict:
+        elif self.good_dict["status"] == "not_in_sell" and "sale_start_time" in self.good_dict:
             return int(self.good_dict["sale_start_time"])
         else:
             return self.good_dict["next_time"]
 
     @property
     def num(self) -> Union[None, int]:
         """
@@ -216,15 +215,16 @@
         logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
         logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
     except Exception:
         logger.error(f"{conf.LOG_HEAD}米游币商品兑换 - 获取商品详细信息: 网络请求失败")
         logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
 
 
-async def get_good_list(game: Literal["bh3", "ys", "bh2", "wd", "bbs", "xq"], retry: bool = True) -> Optional[List[Good]]:
+async def get_good_list(game: Literal["bh3", "ys", "bh2", "wd", "bbs", "xq"], retry: bool = True) -> Optional[
+    List[Good]]:
     """
     获取商品信息列表，若获取失败则返回`None`
 
     :param game: 游戏简称
     :param retry: 是否允许重试
     :return: 商品信息列表
     """
@@ -283,15 +283,17 @@
     return result
 
 
 class Exchange:
     """
     米游币商品兑换相关(需两步初始化对象，先`__init__`，后异步`async_init`)\n
     示例:
-    >>> exchange = await Exchange(account, good_id, game_uid).async_init()
+    ```python
+    exchange = await Exchange(account, good_id, game_uid).async_init()
+    ```
 
     - `result`属性为 `-1`: 用户登录失效，放弃兑换
     - `result`属性为 `-2`: 商品为游戏内物品，由于未配置stoken，放弃兑换
     - `result`属性为 `-3`: 商品为游戏内物品，由于stoken为\"v2\"类型，且未配置mid，放弃兑换
     - `result`属性为 `-4`: 暂不支持商品所属的游戏，放弃兑换
     - `result`属性为 `-5`: 获取商品的信息时，网络请求失败或服务器没有正确返回，放弃兑换
     - `result`属性为 `-6`: 获取用户游戏账户数据失败，放弃兑换
@@ -448,22 +450,29 @@
             except Exception:
                 logger.error(
                     f"{conf.LOG_HEAD}米游币商品兑换 - 执行兑换: 用户 {self.account.phone} 商品 {self.goodID} 请求失败")
                 logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
                 return -3
 
 
-async def game_list_to_image(good_list: List[Good], retry: bool = True):
+async def game_list_to_image(good_list: List[Good], lock: Lock = None, retry: bool = True):
     """
     将商品信息列表转换为图片数据，若返回`None`说明生成失败
 
     :param good_list: 商品列表数据
+    :param lock: 进程同步锁，防止多进程同时在下载字体
     :param retry: 是否允许重试
     """
+    # TODO: 暂时会阻塞，目前还找不到更好的解决方案
+    #   回调函数是否适用于 NoneBot Matcher 暂不清楚，
+    #   若适用则可以传入回调函数而不阻塞主进程
     try:
+        if lock is not None:
+            lock.acquire()
+
         font_path = conf.goodListImage.FONT_PATH
         if font_path is None or not os.path.isfile(font_path):
             if os.path.isfile(FONT_SAVE_PATH):
                 font_path = FONT_SAVE_PATH
             else:
                 logger.warning(
                     f"{conf.LOG_HEAD}商品列表图片生成 - 缺少字体，正在从 https://github.com/adobe-fonts/source-han-sans/tree/release "
@@ -490,15 +499,16 @@
                     os.remove(TEMP_FONT_PATH)
                 except Exception:
                     logger.warning(
                         f"{conf.LOG_HEAD}商品列表图片生成 - 无法清理下载的字体压缩包临时文件")
                     logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
                 font_path = FONT_SAVE_PATH
 
-        logger.info(f"{conf.LOG_HEAD}商品列表图片生成 - 正在生成图片...")
+        if lock is not None:
+            lock.release()
 
         font = ImageFont.truetype(
             str(font_path), conf.goodListImage.FONT_SIZE, encoding=conf.ENCODING)
 
         size_y = 0
         '''起始粘贴位置 高'''
         position: List[tuple] = []
```

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/exchangePlan.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/exchangePlan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """
 ### 米游社商品兑换前端以及计划任务相关
 """
 import asyncio
 import io
 import os
+import threading
 import time
 from copy import deepcopy
 from datetime import datetime
-from typing import List, Set, Union
+from multiprocessing import Manager
+from multiprocessing.pool import Pool
+from multiprocessing.synchronize import Lock
+from typing import List, Set, Union, Callable, Any
 
 from nonebot import get_bot, on_command
 from nonebot.adapters.onebot.v11 import (MessageEvent, MessageSegment,
                                          PrivateMessageEvent, GroupMessageEvent)
 from nonebot.adapters.onebot.v11.message import Message
 from nonebot.matcher import Matcher
 from nonebot.params import ArgStr, ArgPlainText, T_State, CommandArg, Command
@@ -54,15 +58,16 @@
 
         bot = get_bot()
 
         success_tasks: List[asyncio.Task] = list(filter(lambda task: isinstance(
             task.result(), tuple) and task.result()[0], self.tasks))
         if success_tasks:
             await bot.send_private_msg(
-                user_id=self.qq, message=f"🎉用户 📱{self.account.phone}\n🛒商品 {self.plans[0].goodID} 兑换成功，可前往米游社查看")
+                user_id=self.qq,
+                message=f"🎉用户 📱{self.account.phone}\n🛒商品 {self.plans[0].goodID} 兑换成功，可前往米游社查看")
         else:
             msg = f"⚠️用户 📱{self.account.phone}\n🛒商品 {self.plans[0].goodID} 兑换失败\n返回结果：\n"
             num = 0
             for task in self.tasks:
                 num += 1
                 msg += f"{num}: "
                 if isinstance(task.result(), tuple):
@@ -75,15 +80,16 @@
             if plan == (self.plans[0].goodID, self.plans[0].gameUID):
                 self.account.exchange.remove(plan)
         UserData.set_account(self.account, self.qq,
                              self.account.phone)
 
 
 myb_exchange_plan = on_command(f"{conf.COMMAND_START}兑换",
-                               aliases={(f"{conf.COMMAND_START}兑换", "+"), (f"{conf.COMMAND_START}兑换", "-")}, priority=5, block=True)
+                               aliases={(f"{conf.COMMAND_START}兑换", "+"), (f"{conf.COMMAND_START}兑换", "-")},
+                               priority=5, block=True)
 myb_exchange_plan.name = "兑换"
 myb_exchange_plan.usage = f"跟随指引，配置米游币商品自动兑换计划。添加计划之前，请先前往米游社设置好收货地址，并使用『{COMMAND_BEGIN}地址』选择你要使用的地址。所需的商品ID可通过命令『{COMMAND_BEGIN}商品』获取。注意，不限兑换时间的商品将不会在此处显示。 "
 myb_exchange_plan.extra_usage = """\
 具体用法：
 {HEAD}兑换{SEP}+ <商品ID> ➢ 新增兑换计划
 {HEAD}兑换{SEP}- <商品ID> ➢ 删除兑换计划
 {HEAD}商品 ➢ 查看米游社商品
@@ -102,19 +108,21 @@
     """
     if command_arg and len(command) == 1:
         # 如果没有二级命令，但是有参数，则说明用户没有意向使用本功能。
         # 例如：/兑换码获取，识别到的参数为"码获取"，而用户可能有意使用其他插件。
         await matcher.finish()
     elif len(command) > 1 and command[1] in ["+", "-"]:
         if not command_arg:
-            await matcher.reject('⚠️您的输入有误，缺少商品ID，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN,
-                                                                                          SEP=get_last_command_sep()))
+            await matcher.reject(
+                '⚠️您的输入有误，缺少商品ID，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN,
+                                                                                        SEP=get_last_command_sep()))
         elif not str(command_arg).isdigit():
             await matcher.reject(
-                '⚠️商品ID必须为数字，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep()))
+                '⚠️商品ID必须为数字，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN,
+                                                                                 SEP=get_last_command_sep()))
 
     if isinstance(event, GroupMessageEvent):
         await matcher.finish("⚠️为了保护您的隐私，请添加机器人好友后私聊进行操作")
     qq_account = int(event.user_id)
     user_account = UserData.read_account_all(qq_account)
     if not user_account:
         await matcher.finish(f"⚠️你尚未绑定米游社账户，请先使用『{COMMAND_BEGIN}{conf.COMMAND_START}登录』进行登录")
@@ -219,15 +227,16 @@
                             msg += f'\n🎮 {record.region_name} - {record.nickname} - UID {record.uid}'
                         uids.append(record.uid)
                     if uids:
                         await matcher.send("您兑换的是虚拟物品，请发送想要接收奖励的游戏账号UID：\n🚪发送“退出”即可退出")
                         await asyncio.sleep(0.5)
                         await matcher.send(msg)
                     else:
-                        await matcher.finish(f"您还没有绑定『{game_name}』账号哦，暂时不能进行兑换，请先前往米游社绑定后重试")
+                        await matcher.finish(
+                            f"您还没有绑定『{game_name}』账号哦，暂时不能进行兑换，请先前往米游社绑定后重试")
             else:
                 if not account.address:
                     await matcher.finish('⚠️您还没有配置地址哦，请先配置地址')
             state['uids'] = uids
             matcher.set_arg('uid', Message())
         else:
             await matcher.finish(f'⚠️该商品暂时不可以兑换，请重新设置')
@@ -243,15 +252,16 @@
                     await matcher.finish('兑换计划删除成功')
             await matcher.finish(f"您没有设置商品ID为 {good_id} 的兑换哦~")
         else:
             await matcher.finish("您还没有配置兑换计划哦~")
 
     else:
         await matcher.reject(
-            '⚠️您的输入有误，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN, SEP=get_last_command_sep()))
+            '⚠️您的输入有误，请重新输入\n\n' + matcher.extra_usage.format(HEAD=COMMAND_BEGIN,
+                                                                         SEP=get_last_command_sep()))
 
 
 @myb_exchange_plan.got('uid')
 async def _(event: PrivateMessageEvent, matcher: Matcher, state: T_State, uid=ArgPlainText('uid')):
     """
     初始化商品兑换任务，如果传入UID为None则为实物商品，仍可继续
     """
@@ -313,15 +323,15 @@
         \n- 原神\
         \n- 崩坏2\
         \n- 崩坏：星穹铁道\
         \n- 未定事件簿\
         \n- 米游社\
         \n若是商品图片与米游社商品不符或报错 请发送“更新”哦~\
         \n—— 🚪发送“退出”以结束""".strip())
-async def _(event: MessageEvent, matcher: Matcher, arg=ArgPlainText("content")):
+async def _(_: MessageEvent, matcher: Matcher, arg=ArgPlainText("content")):
     """
     根据传入的商品类别，发送对应的商品列表图片
     """
     if arg == '退出':
         await matcher.finish('🚪已成功退出')
     elif arg in ['原神', 'ys']:
         arg = ('ys', '原神')
@@ -332,33 +342,29 @@
     elif arg in ['崩坏：星穹铁道', '星铁', '星穹铁道', '铁道', '轨子', '星穹', 'xq']:
         arg = ('xq', '崩坏：星穹铁道')
     elif arg in ['未定', '未定事件簿', 'wd']:
         arg = ('wd', '未定事件簿')
     elif arg in ['大别野', '米游社']:
         arg = ('bbs', '米游社')
     elif arg == '更新':
-        await get_good_image.send('⏳正在生成商品信息图片...')
-        await generate_image(is_auto=False)
-        await get_good_image.finish('商品信息图片刷新成功')
+        threading.Thread(generate_image(is_auto=False)).start()
+        await get_good_image.finish('✔后台已生成商品信息图片')
     else:
         await get_good_image.reject('⚠️您的输入有误，请重新输入')
     good_list = await get_good_list(arg[0])
     if good_list:
         img_path = time.strftime(
             f'{conf.goodListImage.SAVE_PATH}/%m-%d-{arg[0]}.jpg', time.localtime())
         if os.path.exists(img_path):
             with open(img_path, 'rb') as f:
                 image_bytes = io.BytesIO(f.read())
             await get_good_image.finish(MessageSegment.image(image_bytes))
         else:
-            await get_good_image.send('⏳请稍等，商品图片正在生成哦~')
-            await generate_image(is_auto=False)
-            img_path = time.strftime(
-                f'{conf.goodListImage.SAVE_PATH}/%m-%d-{arg[0]}.jpg', time.localtime())
-            await get_good_image.finish(MessageSegment.image('file:///' + img_path))
+            threading.Thread(generate_image(is_auto=False)).start()
+            await get_good_image.finish('⏳后台正在生成商品信息图片，请稍后查询')
     else:
         await get_good_image.finish(f"{arg[1]} 部分目前没有可兑换商品哦~")
 
 
 @driver.on_startup
 async def _():
     """
@@ -390,36 +396,59 @@
                     exchange_plan = await Exchange(account, exchange_good[0], exchange_good[1]).async_init()
                     scheduler.add_job(id=str(account.phone) + '_' + exchange_good[0], replace_existing=True,
                                       trigger='date', func=ExchangeStart(
                             account, qq, exchange_plan, conf.EXCHANGE_THREAD).start,
                                       next_run_time=datetime.fromtimestamp(good_detail.time))
 
 
-@driver.on_startup
-async def generate_image(is_auto=True):
+def image_process(game: str, lock: Lock):
+    """
+    生成并保存图片的进程函数
+
+    :param game: 游戏名
+    :param lock: 进程锁
+    :return: 生成成功或无商品返回True，否则返回False
     """
-    生成米游币商品信息图片。
+    loop = asyncio.new_event_loop()
+    good_list = loop.run_until_complete(get_good_list(game))
+    if good_list:
+        logger.info(f"{conf.LOG_HEAD}正在生成 {game} 分区的商品列表图片")
+        image_bytes = loop.run_until_complete(game_list_to_image(good_list, lock))
+        if not image_bytes:
+            return False
+        date = time.strftime('%m-%d', time.localtime())
+        path = conf.goodListImage.SAVE_PATH / f"{date}-{game}.jpg"
+        with open(path, 'wb') as f:
+            f.write(image_bytes)
+        logger.info(f"{conf.LOG_HEAD}已完成 {game} 分区的商品列表图片生成")
+    else:
+        logger.info(f"{conf.LOG_HEAD}{game}分区暂时没有商品，跳过生成商品列表图片")
+    return True
+
+
+def generate_image(is_auto=True, callback: Callable[[bool], Any] = None):
+    """
+    生成米游币商品信息图片。该函数会阻塞当前线程
 
     :param is_auto: True为每日自动生成，False为用户手动更新
+    :param callback: 回调函数，参数为生成成功与否
+    >>> generate_image(is_auto=False)
     """
     for root, _, files in os.walk(conf.goodListImage.SAVE_PATH, topdown=False):
         for name in files:
             date = time.strftime('%m-%d', time.localtime())
             # 若图片开头为当日日期，则退出函数不执行
             if name.startswith(date):
                 if is_auto:
                     return
-            # 删除旧图片，以方便生成当日图片
+            # 删除旧图片
             if name.endswith('.jpg'):
                 os.remove(os.path.join(root, name))
-    for game in "bh3", "ys", "bh2", "xq", "wd", "bbs":
-        good_list = await get_good_list(game)
-        if good_list:
-            img_path = time.strftime(
-                f'{conf.goodListImage.SAVE_PATH}/%m-%d-{game}.jpg', time.localtime())
-            image_bytes = await game_list_to_image(good_list)
-            if not image_bytes:
-                return
-            with open(img_path, 'wb') as f:
-                f.write(image_bytes)
-        else:
-            logger.info(f"{conf.LOG_HEAD}{game}分区暂时没有商品，跳过生成...")
+
+    lock: Lock = Manager().Lock()
+    with Pool() as pool:
+        for game in "bh3", "ys", "bh2", "xq", "wd", "bbs":
+            pool.apply_async(image_process,
+                             args=(game, lock),
+                             callback=callback)
+        pool.close()
+        pool.join()
```

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/gameSign.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/gameSign.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/help.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/help.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 from nonebot.adapters.onebot.v11.message import Message
 from nonebot.matcher import Matcher
 from nonebot.params import Arg, CommandArg
 
 from .config import config as conf
 from .utils import PLUGIN, COMMAND_BEGIN
 
-helper = on_command(conf.COMMAND_START + "help", priority=1,
-                    aliases={conf.COMMAND_START + "帮助"})
+helper = on_command(conf.COMMAND_START + "help",
+                    priority=1,
+                    aliases={conf.COMMAND_START + "帮助"},
+                    block=True)
 
 helper.name = '帮助'
 helper.usage = '''\
     🍺欢迎使用米游社小助手帮助系统！\
     \n{HEAD}帮助 ➢ 查看米游社小助手使用说明\
     \n{HEAD}帮助 <功能名> ➢ 查看目标功能详细说明\
 '''.strip()
```

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/login.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/login.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/mybMission.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/mybMission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/plan.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,31 +92,34 @@
     for account in accounts:
         gamesign = GameSign(account)
         record_list: List[GameRecord] = await get_game_record(account)
         if isinstance(record_list, int):
             if record_list == -1:
                 failed_accounts.append(account)
                 if group_event:
-                    await bot.send(event=group_event, at_sender=True, message=f"⚠️账户 {blur(account.phone)} 登录失效，请重新登录")
+                    await bot.send(event=group_event, at_sender=True,
+                                   message=f"⚠️账户 {blur(account.phone)} 登录失效，请重新登录")
                 else:
                     await bot.send_private_msg(user_id=qq, message=f"⚠️账户 {account.phone} 登录失效，请重新登录")
                 continue
             else:
                 if group_event:
                     await bot.send(event=group_event, at_sender=True,
                                    message=f"⚠️账户 {blur(account.phone)} 获取游戏账号信息失败，请重新尝试")
                 else:
-                    await bot.send_private_msg(user_id=qq, message=f"⚠️账户 {account.phone} 获取游戏账号信息失败，请重新尝试")
+                    await bot.send_private_msg(user_id=qq,
+                                               message=f"⚠️账户 {account.phone} 获取游戏账号信息失败，请重新尝试")
                 continue
         if not record_list and not is_auto:
             if group_event:
                 await bot.send(event=group_event, at_sender=True,
                                message=f"⚠️账户 {blur(account.phone)} 没有绑定任何游戏账号，跳过游戏签到")
             else:
-                await bot.send_private_msg(user_id=qq, message=f"⚠️账户 {account.phone} 没有绑定任何游戏账号，跳过游戏签到")
+                await bot.send_private_msg(user_id=qq,
+                                           message=f"⚠️账户 {account.phone} 没有绑定任何游戏账号，跳过游戏签到")
             continue
         for record in record_list:
             if GameInfo.ABBR_TO_ID[record.game_id][0] not in GameSign.SUPPORTED_GAMES:
                 logger.info(f"{conf.LOG_HEAD}执行游戏签到 - {GameInfo.ABBR_TO_ID[record.game_id][1]} 暂不支持")
                 continue
             else:
                 sign_game = GameInfo.ABBR_TO_ID[record.game_id][0]
@@ -222,34 +225,38 @@
     failed_accounts = []
     for account in accounts:
         missions_state = await get_missions_state(account)
         mybmission = await Action(account).async_init()
         if isinstance(missions_state, int):
             if mybmission == -1:
                 if group_event:
-                    await bot.send(event=group_event, at_sender=True, message=f'⚠️账户 {blur(account.phone)} 登录失效，请重新登录')
+                    await bot.send(event=group_event, at_sender=True,
+                                   message=f'⚠️账户 {blur(account.phone)} 登录失效，请重新登录')
                 else:
                     await bot.send_private_msg(user_id=qq, message=f'⚠️账户 {account.phone} 登录失效，请重新登录')
                 continue
             if group_event:
                 await bot.send(event=group_event, at_sender=True,
                                message=f'⚠️账户 {blur(account.phone)} 获取任务完成情况请求失败，你可以手动前往App查看')
             else:
-                await bot.send_private_msg(user_id=qq, message=f'⚠️账户 {account.phone} 获取任务完成情况请求失败，你可以手动前往App查看')
+                await bot.send_private_msg(user_id=qq,
+                                           message=f'⚠️账户 {account.phone} 获取任务完成情况请求失败，你可以手动前往App查看')
             continue
         if isinstance(mybmission, int):
             if mybmission == -1:
                 failed_accounts.append(account)
                 if group_event:
-                    await bot.send(event=group_event, at_sender=True, message=f'⚠️账户 {blur(account.phone)} 登录失效，请重新登录')
+                    await bot.send(event=group_event, at_sender=True,
+                                   message=f'⚠️账户 {blur(account.phone)} 登录失效，请重新登录')
                 else:
                     await bot.send_private_msg(user_id=qq, message=f'⚠️账户 {account.phone} 登录失效，请重新登录')
                 continue
             if group_event:
-                await bot.send(event=group_event, at_sender=True, message=f'⚠️账户 {blur(account.phone)} 请求失败，请重新尝试')
+                await bot.send(event=group_event, at_sender=True,
+                               message=f'⚠️账户 {blur(account.phone)} 请求失败，请重新尝试')
             else:
                 await bot.send_private_msg(user_id=qq, message=f'⚠️账户 {account.phone} 请求失败，请重新尝试')
             continue
         # 自动执行米游币任务时，要求用户打开了任务功能；手动执行时都可以调用执行。
         if (account.mybMission and is_auto) or not is_auto:
             if not is_auto:
                 if not group_event:
@@ -267,15 +274,16 @@
                 missions_state = await get_missions_state(account)
                 if isinstance(missions_state, int):
                     if mybmission == -1:
                         if group_event:
                             await bot.send(event=group_event, at_sender=True,
                                            message=f'⚠️账户 {blur(account.phone)} 登录失效，请重新登录')
                         else:
-                            await bot.send_private_msg(user_id=qq, message=f'⚠️账户 {account.phone} 登录失效，请重新登录')
+                            await bot.send_private_msg(user_id=qq,
+                                                       message=f'⚠️账户 {account.phone} 登录失效，请重新登录')
                         continue
                     if group_event:
                         await bot.send(event=group_event, at_sender=True,
                                        message=f'⚠️账户 {blur(account.phone)} 获取任务完成情况请求失败，你可以手动前往App查看')
                     else:
                         await bot.send_private_msg(user_id=qq,
                                                    message=f'⚠️账户 {account.phone} 获取任务完成情况请求失败，你可以手动前往App查看')
@@ -333,31 +341,34 @@
             if isinstance(genshinstatus, int):
                 if genshinstatus == -1:
                     if not is_auto:
                         if group_event:
                             await bot.send(event=group_event, at_sender=True,
                                            message=f'⚠️账户 {blur(account.phone)} 登录失效，请重新登录')
                         else:
-                            await bot.send_private_msg(user_id=qq, message=f'⚠️账户 {account.phone} 登录失效，请重新登录')
+                            await bot.send_private_msg(user_id=qq,
+                                                       message=f'⚠️账户 {account.phone} 登录失效，请重新登录')
                 if genshinstatus == -4:
                     if not is_auto:
                         if group_event:
                             await bot.send(event=group_event, at_sender=True,
                                            message=f'⚠️账户 {blur(account.phone)} 没有绑定任何原神账户，请绑定后再重试')
                         else:
-                            await bot.send_private_msg(user_id=qq, message=f'⚠️账户 {account.phone} 没有绑定任何原神账户，请绑定后再重试')
+                            await bot.send_private_msg(user_id=qq,
+                                                       message=f'⚠️账户 {account.phone} 没有绑定任何原神账户，请绑定后再重试')
                         account.checkResin = False
                         UserData.set_account(account, qq, account.phone)
                         continue
                 if not is_auto:
                     if group_event:
                         await bot.send(event=group_event, at_sender=True,
                                        message=f'⚠️账户 {blur(account.phone)} 获取实时便笺请求失败，你可以手动前往App查看')
                     else:
-                        await bot.send_private_msg(user_id=qq, message=f'⚠️账户 {account.phone} 获取实时便笺请求失败，你可以手动前往App查看')
+                        await bot.send_private_msg(user_id=qq,
+                                                   message=f'⚠️账户 {account.phone} 获取实时便笺请求失败，你可以手动前往App查看')
                 continue
             msg = ''
             # 手动查询体力时，无需判断是否溢出
             if not is_auto:
                 pass
             else:
                 # 体力溢出提醒
@@ -403,20 +414,20 @@
             if group_event:
                 await bot.send(event=group_event, at_sender=True, message=msg)
             else:
                 await bot.send_private_msg(user_id=qq, message=msg)
 
 
 @scheduler.scheduled_job("cron", hour='0', minute='0', id="daily_goodImg_update")
-async def daily_update():
+def daily_update():
     """
     每日图片生成函数
     """
     logger.info(f"{conf.LOG_HEAD}开始生成每日商品图片")
-    await generate_image()
+    generate_image()
 
 
 @scheduler.scheduled_job("cron",
                          hour=conf.SIGN_TIME.split(':')[0],
                          minute=conf.SIGN_TIME.split(':')[1],
                          id="daily_schedule")
 async def daily_schedule():
```

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/setting.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .bbsAPI import GameInfo
 from .config import config as conf
 from .data import UserAccount, UserData
 from .mybMission import GAME_ID
 from .utils import COMMAND_BEGIN
 
-setting = on_command(conf.COMMAND_START + '设置', priority=4)
+setting = on_command(conf.COMMAND_START + '设置', priority=4, block=True)
 setting.name = "设置"
 setting.usage = f'如需配置是否开启每日任务、设备平台、频道任务等相关选项，请使用『{COMMAND_BEGIN}账号设置』命令。\n如需设置米游币任务和游戏签到后是否进行QQ通知，请使用『{COMMAND_BEGIN}通知设置』命令。'
 
 
 @setting.handle()
 async def _(event: MessageEvent):
     msg = f'如需配置是否开启每日任务、设备平台、频道任务等相关选项，请使用『{COMMAND_BEGIN}账号设置』命令\n如需设置米游币任务和游戏签到后是否进行QQ通知，请使用『{COMMAND_BEGIN}通知设置』命令'
```

### Comparing `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/utils.py` & `nonebot_plugin_mystool-0.2.9/src/nonebot_plugin_mystool/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import httpx
 import nonebot
 import nonebot.log
 import nonebot.plugin
 import ntplib
 import tenacity
+from nonebot.internal.matcher import Matcher
 from nonebot.log import logger
 
 from .config import config as conf
 
 if TYPE_CHECKING:
     from loguru import Logger
 
@@ -337,7 +338,23 @@
             self.index = 0
         if not success:
             return False
         else:
             conf.parse_obj(Subscribe.conf_list[self.index]["config"])
             self.index += 1
             return True
+
+# TODO: 一个用于构建on_command事件相应器的函数，
+#  将使用偏好设置里的priority优先级和block设置，
+#  可能可以作为装饰器使用
+#   （需要先等用户数据改用Pydantic作为数据模型）
+def command_matcher(command: str, priority: int = None, block: bool = None) -> Matcher:
+    """
+    用于构建on_command事件相应器的函数，
+    将使用偏好设置里的priority优先级和block设置
+
+    :param command: 指令名
+    :param priority: 优先级，为 None 则读取偏好设置
+    :param block: 是否阻塞，为 None 则读取偏好设置
+    :return: 事件响应器
+    """
+    ...
```

### Comparing `nonebot_plugin_mystool-0.2.8/PKG-INFO` & `nonebot_plugin_mystool-0.2.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e6f 6e65  : 2.1.Name: none
 00000020: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
 00000030: 6f6c 0a56 6572 7369 6f6e 3a20 302e 322e  ol.Version: 0.2.
-00000040: 380a 5375 6d6d 6172 793a 204e 6f6e 6542  8.Summary: NoneB
+00000040: 390a 5375 6d6d 6172 793a 204e 6f6e 6542  9.Summary: NoneB
 00000050: 6f74 32e6 8f92 e4bb b67c e7b1 b3e6 b8b8  ot2......|......
 00000060: e7a4 bee5 b7a5 e585 b72d e6af 8fe6 97a5  .........-......
 00000070: e7b1 b3e6 b8b8 e5b8 81e4 bbbb e58a a1e3  ................
 00000080: 8081 e6b8 b8e6 888f e7ad bee5 88b0 e380  ................
 00000090: 81e5 9586 e593 81e5 8591 e68d a2e3 8081  ................
 000000a0: e585 8de6 8a93 e58c 85e7 99bb e5bd 95e3  ................
 000000b0: 8081 e58e 9fe7 a59e e6a0 91e8 8482 e68f  ................
@@ -61,15 +61,15 @@
 000003c0: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
 000003d0: 6973 743a 206e 6f6e 6562 6f74 5f70 6c75  ist: nonebot_plu
 000003e0: 6769 6e5f 6170 7363 6865 6475 6c65 7220  gin_apscheduler 
 000003f0: 283e 3d30 2e32 2e30 290a 5265 7175 6972  (>=0.2.0).Requir
 00000400: 6573 2d44 6973 743a 206e 7470 6c69 6220  es-Dist: ntplib 
 00000410: 283e 3d30 2e34 2e30 2c3c 302e 352e 3029  (>=0.4.0,<0.5.0)
 00000420: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000430: 7265 7175 6573 7473 2028 3e3d 322e 3239  requests (>=2.29
+00000430: 7265 7175 6573 7473 2028 3e3d 322e 3330  requests (>=2.30
 00000440: 2e30 2c3c 332e 302e 3029 0a52 6571 7569  .0,<3.0.0).Requi
 00000450: 7265 732d 4469 7374 3a20 7465 6e61 6369  res-Dist: tenaci
 00000460: 7479 2028 3e3d 382e 322e 322c 3c39 2e30  ty (>=8.2.2,<9.0
 00000470: 2e30 290a 5072 6f6a 6563 742d 5552 4c3a  .0).Project-URL:
 00000480: 2042 7567 2054 7261 636b 6572 2c20 6874   Bug Tracker, ht
 00000490: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000004a0: 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65 626f  /Ljzd-PRO/nonebo
@@ -107,199 +107,160 @@
 000006a0: 5f5f 5f5c 2020 5c20 5c5f 5f5f 5f5f 5c20  ___\  \ \_____\ 
 000006b0: 205c 205c 5f5f 5f5f 5f5c 0a20 205c 2f5f   \ \_____\.  \/_
 000006c0: 2f20 205c 2f5f 2f20 2020 5c2f 5f5f 5f5f  /  \/_/   \/____
 000006d0: 5f2f 2020 205c 2f5f 5f5f 5f5f 2f20 2020  _/   \/_____/   
 000006e0: 2020 5c2f 5f2f 2020 205c 2f5f 5f5f 5f5f    \/_/   \/_____
 000006f0: 2f20 2020 5c2f 5f5f 5f5f 5f2f 2020 205c  /   \/_____/   \
 00000700: 2f5f 5f5f 5f5f 2f0a 6060 600a 0a3c 6469  /_____/.```..<di
-00000710: 763e 0a20 203c 6120 6872 6566 3d22 6874  v>.  <a href="ht
-00000720: 7470 733a 2f2f 7777 772e 636f 6465 6661  tps://www.codefa
-00000730: 6374 6f72 2e69 6f2f 7265 706f 7369 746f  ctor.io/reposito
-00000740: 7279 2f67 6974 6875 622f 6c6a 7a64 2d70  ry/github/ljzd-p
-00000750: 726f 2f6e 6f6e 6562 6f74 2d70 6c75 6769  ro/nonebot-plugi
-00000760: 6e2d 6d79 7374 6f6f 6c22 2074 6172 6765  n-mystool" targe
-00000770: 743d 225f 626c 616e 6b22 3e0a 2020 2020  t="_blank">.    
-00000780: 3c69 6d67 2061 6c74 3d22 436f 6465 4661  <img alt="CodeFa
-00000790: 6374 6f72 2220 7372 633d 2268 7474 7073  ctor" src="https
-000007a0: 3a2f 2f77 7777 2e63 6f64 6566 6163 746f  ://www.codefacto
-000007b0: 722e 696f 2f72 6570 6f73 6974 6f72 792f  r.io/repository/
-000007c0: 6769 7468 7562 2f6c 6a7a 642d 7072 6f2f  github/ljzd-pro/
-000007d0: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
-000007e0: 7973 746f 6f6c 2f62 6164 6765 3f73 7479  ystool/badge?sty
-000007f0: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
-00000800: 223e 0a20 203c 2f61 3e0a 2020 3c61 2068  ">.  </a>.  <a h
-00000810: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000820: 6875 622e 636f 6d2f 4c6a 7a64 2d50 524f  hub.com/Ljzd-PRO
-00000830: 2f6e 6f6e 6562 6f74 2d70 6c75 6769 6e2d  /nonebot-plugin-
-00000840: 6d79 7374 6f6f 6c2f 7265 6c65 6173 6573  mystool/releases
-00000850: 2f6c 6174 6573 7422 2074 6172 6765 743d  /latest" target=
-00000860: 225f 626c 616e 6b22 3e0a 2020 2020 3c69  "_blank">.    <i
-00000870: 6d67 2061 6c74 3d22 e69c 80e6 96b0 e58f  mg alt="........
-00000880: 91e8 a18c e789 8822 2073 7263 3d22 6874  ......." src="ht
-00000890: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000008a0: 732e 696f 2f67 6974 6875 622f 762f 7265  s.io/github/v/re
-000008b0: 6c65 6173 652f 4c6a 7a64 2d50 524f 2f6e  lease/Ljzd-PRO/n
-000008c0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
-000008d0: 7354 6f6f 6c3f 6c6f 676f 3d70 7974 686f  sTool?logo=pytho
-000008e0: 6e26 7374 796c 653d 666f 722d 7468 652d  n&style=for-the-
-000008f0: 6261 6467 6522 3e0a 2020 3c2f 613e 0a20  badge">.  </a>. 
-00000900: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000910: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 6a7a  //github.com/Ljz
-00000920: 642d 5052 4f2f 6e6f 6e65 626f 742d 706c  d-PRO/nonebot-pl
-00000930: 7567 696e 2d6d 7973 746f 6f6c 2f63 6f6d  ugin-mystool/com
-00000940: 6d69 7473 2f22 2074 6172 6765 743d 225f  mits/" target="_
-00000950: 626c 616e 6b22 3e0a 2020 2020 3c69 6d67  blank">.    <img
-00000960: 2061 6c74 3d22 e69c 80e5 908e e68f 90e4   alt="..........
-00000970: baa4 2220 7372 633d 2268 7474 7073 3a2f  .." src="https:/
-00000980: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000990: 6769 7468 7562 2f6c 6173 742d 636f 6d6d  github/last-comm
-000009a0: 6974 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  it/Ljzd-PRO/none
-000009b0: 626f 742d 706c 7567 696e 2d6d 7973 546f  bot-plugin-mysTo
-000009c0: 6f6c 3f73 7479 6c65 3d66 6f72 2d74 6865  ol?style=for-the
-000009d0: 2d62 6164 6765 223e 0a20 203c 2f61 3e0a  -badge">.  </a>.
-000009e0: 3c2f 6469 763e 0a0a 2320 6d79 7354 6f6f  </div>..# mysToo
-000009f0: 6c20 2d20 e7b1 b3e6 b8b8 e7a4 bee8 be85  l - ............
-00000a00: e58a a9e5 b7a5 e585 b7e6 8f92 e4bb b60a  ................
-00000a10: 0a2a 2ae7 8988 e69c ac20 2d20 7630 2e32  .**...... - v0.2
-00000a20: 2e38 2a2a 0a0a 2323 2320 f09f 93a3 20e6  .8**..### .... .
-00000a30: 9bb4 e696 b0e5 8685 e5ae b90a 0a23 2323  .............###
-00000a40: 2320 3230 3233 2e35 2e34 0a2d 20e5 a29e  # 2023.5.4.- ...
-00000a50: e58a a0e5 afb9 e698 9fe7 a9b9 e993 81e9  ................
-00000a60: 8193 e79a 84e7 adbe e588 b0e5 8a9f e883  ................
-00000a70: bde7 9a84 e694 afe6 8c81 202d 205b 2338  .......... - [#8
-00000a80: 395d 2868 7474 7073 3a2f 2f67 6974 6875  9](https://githu
-00000a90: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
-00000aa0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
-00000ab0: 7374 6f6f 6c2f 7075 6c6c 2f38 3929 2062  stool/pull/89) b
-00000ac0: 7920 4061 7961 6b61 7375 6b69 0a2d 20e4  y @ayakasuki.- .
-00000ad0: bfae e5a4 8de6 8f92 e4bb b6e5 91bd e4bb  ................
-00000ae0: a4e4 bc98 e585 88e5 baa6 e997 aee9 a298  ................
-00000af0: 202d 205b 2338 385d 2868 7474 7073 3a2f   - [#88](https:/
-00000b00: 2f67 6974 6875 622e 636f 6d2f 4c6a 7a64  /github.com/Ljzd
-00000b10: 2d50 524f 2f6e 6f6e 6562 6f74 2d70 6c75  -PRO/nonebot-plu
-00000b20: 6769 6e2d 6d79 7374 6f6f 6c2f 7075 6c6c  gin-mystool/pull
-00000b30: 2f38 3829 2062 7920 4061 7961 6b61 7375  /88) by @ayakasu
-00000b40: 6b69 0a2d 20e9 83a8 e588 86e6 9687 e69c  ki.- ...........
-00000b50: ace9 9499 e8af afe4 bfae e6ad a320 2d20  ............. - 
-00000b60: 5b23 3930 5d28 6874 7470 733a 2f2f 6769  [#90](https://gi
-00000b70: 7468 7562 2e63 6f6d 2f4c 6a7a 642d 5052  thub.com/Ljzd-PR
-00000b80: 4f2f 6e6f 6e65 626f 742d 706c 7567 696e  O/nonebot-plugin
-00000b90: 2d6d 7973 746f 6f6c 2f70 756c 6c2f 3930  -mystool/pull/90
-00000ba0: 2920 6279 2040 626c 6163 6b2d 7a65 726f  ) by @black-zero
-00000bb0: 3335 380a 0a23 2323 2320 3230 3233 2e34  358..#### 2023.4
-00000bc0: 2e32 380a 2d20 e4bf aee5 a48d e68f 92e4  .28.- ..........
-00000bd0: bbb6 e591 bde4 bba4 e8a2 abe5 85b6 e4bb  ................
-00000be0: 9620 6e6f 6e65 626f 7420 e68f 92e4 bbb6  . nonebot ......
-00000bf0: e68d 95e8 8eb7 e79a 84e9 97ae e9a2 980a  ................
-00000c00: 2d20 e5a2 9ee5 8aa0 e694 afe6 8c81 e698  - ..............
-00000c10: 9fe7 a9b9 e993 81e9 8193 e79a 84e5 9586  ................
-00000c20: e593 81e5 8591 e68d a20a 2d20 e6af 8fe6  ..........- ....
-00000c30: 97a5 e7ad bee5 88b0 e380 81e7 b1b3 e6b8  ................
-00000c40: b8e5 b881 e4bb bbe5 8aa1 e689 a7e8 a18c  ................
-00000c50: e697 b6e9 97b4 e59c a8e7 94a8 e688 b7e9  ................
-00000c60: 858d e7bd aee7 9a84 e59f bae7 a180 e4b8  ................
-00000c70: 8ae5 a29e e58a a0e9 9a8f e69c bae5 bbb6  ................
-00000c80: e8bf 9f0a 2d20 e4bf aee5 a48d e5a4 a7e5  ....- ..........
-00000c90: 88ab e987 8ee9 a291 e981 93e6 af8f e697  ................
-00000ca0: a5e4 bbbb e58a a1e3 8081 e7ad bee5 88b0  ................
-00000cb0: e689 a7e8 a18c e5a4 b1e8 b4a5 e79a 84e9  ................
-00000cc0: 97ae e9a2 980a 0a23 2323 2320 3230 3233  .......#### 2023
-00000cd0: 2e33 2e33 300a 2d20 e4bf aee5 a48d e987  .3.30.- ........
-00000ce0: 8de5 8699 e985 8de7 bdae e696 87e4 bbb6  ................
-00000cf0: 2060 706c 7567 696e 436f 6e66 6967 2e6a   `pluginConfig.j
-00000d00: 736f 6e60 20e4 b88d e794 9fe6 9588 e79a  son` ...........
-00000d10: 84e9 97ae e9a2 980a 2d20 e4bf aee5 a48d  ........- ......
-00000d20: e58d 95e8 b4a6 e688 b7e6 8385 e586 b5e4  ................
-00000d30: b88b e697 a0e6 b395 e5a2 9ee5 88a0 e585  ................
-00000d40: 91e6 8da2 e8ae a1e5 8892 e79a 84e9 97ae  ................
-00000d50: e9a2 980a 2d20 e4bf aee5 a48d 2060 2fe5  ....- ...... `/.
-00000d60: 8591 e68d a260 20e5 91bd e4bb a4e5 8faf  .....` .........
-00000d70: e883 bde4 b88e e585 b6e4 bb96 e68f 92e4  ................
-00000d80: bbb6 e591 bde4 bba4 e586 b2e7 aa81 e79a  ................
-00000d90: 84e9 97ae e9a2 98ef bc8c e590 8ce6 97b6  ................
-00000da0: 205b f09f 9497 e794 a8e6 b395 e58f 98e6   [..............
-00000db0: 9bb4 5d28 6874 7470 733a 2f2f 6769 7468  ..](https://gith
-00000dc0: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
-00000dd0: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
-00000de0: 7973 746f 6f6c 2f77 696b 692f 496e 666f  ystool/wiki/Info
-00000df0: 726d 6174 696f 6e2d 4578 6368 616e 6765  rmation-Exchange
-00000e00: 23e5 a29e e58a a0e5 88a0 e999 a4e5 8591  #...............
-00000e10: e68d a2e8 aea1 e588 9229 0a2d 20e7 b2be  .........).- ...
-00000e20: e7ae 80e6 8ea5 e694 b6e7 9a84 e591 bde4  ................
-00000e30: bba4 0a2d 20e6 9bb4 e6ad a320 6064 6576  ...- ...... `dev
-00000e40: 6963 655f 7361 7665 6020 22e8 aebe e5a4  ice_save` ".....
-00000e50: 87e4 bf9d e5ad 9822 20e6 97a5 e5bf 97e6  ......." .......
-00000e60: 9687 e69c ace7 9a84 e994 99e8 afaf 0a0a  ................
-00000e70: 2323 20e5 8a9f e883 bde5 928c e789 b9e6  ## .............
-00000e80: 80a7 0a0a 2d20 e79f ade4 bfa1 e9aa 8ce8  ....- ..........
-00000e90: af81 e799 bbe5 bd95 efbc 8ce5 858d e68a  ................
-00000ea0: 93e5 8c85 e88e b7e5 8f96 2043 6f6f 6b69  .......... Cooki
-00000eb0: 650a 2d20 e887 aae5 8aa8 e5ae 8ce6 8890  e.- ............
-00000ec0: e6af 8fe6 97a5 e7b1 b3e6 b8b8 e5b8 81e4  ................
-00000ed0: bbbb e58a a10a 2d20 e887 aae5 8aa8 e8bf  ......- ........
-00000ee0: 9be8 a18c e6b8 b8e6 888f e7ad bee5 88b0  ................
-00000ef0: 0a2d 20e5 8faf e588 b6e5 ae9a e7b1 b3e6  .- .............
-00000f00: b8b8 e5b8 81e5 9586 e593 81e5 8591 e68d  ................
-00000f10: a2e8 aea1 e588 92ef bc8c e588 b0e7 82b9  ................
-00000f20: e585 91e6 8da2 0a2d 20e5 8faf e694 afe6  .......- .......
-00000f30: 8c81 e5a4 9ae4 b8aa 2051 5120 e8b4 a6e5  ........ QQ ....
-00000f40: 8fb7 efbc 8ce6 af8f e4b8 aa20 5151 20e8  ........... QQ .
-00000f50: b4a6 e58f b7e5 8faf e7bb 91e5 ae9a e5a4  ................
-00000f60: 9ae4 b8aa e7b1 b3e5 9388 e6b8 b8e8 b4a6  ................
-00000f70: e688 b70a 2d20 5151 20e6 8ea8 e980 81e6  ....- QQ .......
-00000f80: 89a7 e8a1 8ce7 bb93 e69e 9ce9 809a e79f  ................
-00000f90: a50a 2d20 e58e 9fe7 a59e e6a0 91e8 8482  ..- ............
-00000fa0: e380 81e6 b49e e5a4 a9e5 ae9d e992 b1e3  ................
-00000fb0: 8081 e8b4 a8e9 878f e58f 82e5 8f98 e4bb  ................
-00000fc0: aae5 b7b2 e6bb a1e6 97b6 e68e a8e9 8081  ................
-00000fd0: e980 9ae7 9fa5 0a0a 2323 20e4 bdbf e794  ........## .....
-00000fe0: a8e8 afb4 e698 8e0a 0a23 2323 20f0 9f9b  .........### ...
-00000ff0: a0ef b88f 204e 6f6e 6542 6f74 3220 e69c  .... NoneBot2 ..
-00001000: bae5 99a8 e4ba bae9 83a8 e7bd b2e5 928c  ................
-00001010: e68f 92e4 bbb6 e5ae 89e8 a385 0a0a e8af  ................
-00001020: b7e6 9fa5 e79c 8b20 2d3e 205b f09f 9497  ....... -> [....
-00001030: 496e 7374 616c 6c61 7469 6f6e 5d28 6874  Installation](ht
-00001040: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001050: 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65 626f  /Ljzd-PRO/nonebo
-00001060: 742d 706c 7567 696e 2d6d 7973 746f 6f6c  t-plugin-mystool
-00001070: 2f77 696b 692f 496e 7374 616c 6c61 7469  /wiki/Installati
-00001080: 6f6e 290a 0a23 2323 20f0 9f93 9620 e68f  on)..### .... ..
-00001090: 92e4 bbb6 e585 b7e4 bd93 e4bd bfe7 94a8  ................
-000010a0: e8af b4e6 988e 0a0a e8af b7e6 9fa5 e79c  ................
-000010b0: 8b20 2d3e 205b f09f 9497 5769 6b69 20e6  . -> [....Wiki .
-000010c0: 9687 e6a1 a35d 2868 7474 7073 3a2f 2f67  .....](https://g
-000010d0: 6974 6875 622e 636f 6d2f 4c6a 7a64 2d50  ithub.com/Ljzd-P
-000010e0: 524f 2f6e 6f6e 6562 6f74 2d70 6c75 6769  RO/nonebot-plugi
-000010f0: 6e2d 6d79 7374 6f6f 6c2f 7769 6b69 290a  n-mystool/wiki).
-00001100: 0a23 2323 20e2 9d93 20e8 8eb7 e58f 96e6  .### ... .......
-00001110: 8f92 e4bb b6e5 b8ae e58a a9e4 bfa1 e681  ................
-00001120: af0a 0a23 2323 2320 e68f 92e4 bbb6 e591  ...#### ........
-00001130: bde4 bba4 0a0a 6060 600a 2fe5 b8ae e58a  ......```./.....
-00001140: a90a 6060 600a 0a3e 20e2 9aa0 efb8 8f20  ..```..> ...... 
-00001150: e6b3 a8e6 848f 20e6 ada4 e5a4 84e6 b2a1  ...... .........
-00001160: e69c 89e4 bdbf e794 a820 5bf0 9f94 9720  ......... [.... 
-00001170: e68f 92e4 bbb6 e591 bde4 bba4 e5a4 b45d  ...............]
-00001180: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001190: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
-000011a0: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
-000011b0: 6f6f 6c2f 7769 6b69 2f43 6f6e 6669 6775  ool/wiki/Configu
-000011c0: 7261 7469 6f6e 2d43 6f6e 6669 6723 636f  ration-Config#co
-000011d0: 6d6d 616e 645f 7374 6172 7429 0a0a 2323  mmand_start)..##
-000011e0: 20e5 85b6 e4bb 960a 0a23 2323 205b f09f   ........### [..
-000011f0: 9383 e6ba 90e7 a081 e8af b4e6 988e 5d28  ..............](
-00001200: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001210: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
-00001220: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
-00001230: 6f6c 2f77 696b 692f 536f 7572 6365 2d53  ol/wiki/Source-S
-00001240: 7472 7563 7475 7265 290a 2323 2320 e980  tructure).### ..
-00001250: 82e9 858d 205b e7bb aae5 b1b1 e79c 9fe5  .... [..........
-00001260: afbb 426f 745d 2868 7474 7073 3a2f 2f67  ..Bot](https://g
-00001270: 6974 6875 622e 636f 6d2f 4869 6269 4b69  ithub.com/HibiKi
-00001280: 6572 2f7a 6865 6e78 756e 5f62 6f74 2920  er/zhenxun_bot) 
-00001290: e79a 84e5 8886 e694 af0a 2d20 6874 7470  ..........- http
-000012a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
-000012b0: 5754 4a43 2f7a 6865 6e78 756e 2d70 6c75  WTJC/zhenxun-plu
-000012c0: 6769 6e2d 6d79 7374 6f6f 6c0a 2d20 6874  gin-mystool.- ht
-000012d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000012e0: 2f61 7961 6b61 7375 6b69 2f6e 6f6e 6562  /ayakasuki/noneb
-000012f0: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
-00001300: 6c0a 0a                                  l..
+00000710: 763e 0a20 203c 696d 6720 616c 743d 2243  v>.  <img alt="C
+00000720: 6f64 6546 6163 746f 7222 2073 7263 3d22  odeFactor" src="
+00000730: 6874 7470 733a 2f2f 7777 772e 636f 6465  https://www.code
+00000740: 6661 6374 6f72 2e69 6f2f 7265 706f 7369  factor.io/reposi
+00000750: 746f 7279 2f67 6974 6875 622f 6c6a 7a64  tory/github/ljzd
+00000760: 2d70 726f 2f6e 6f6e 6562 6f74 2d70 6c75  -pro/nonebot-plu
+00000770: 6769 6e2d 6d79 7374 6f6f 6c2f 6261 6467  gin-mystool/badg
+00000780: 653f 7374 796c 653d 666f 722d 7468 652d  e?style=for-the-
+00000790: 6261 6467 6522 3e0a 2020 3c69 6d67 2061  badge">.  <img a
+000007a0: 6c74 3d22 e69c 80e6 96b0 e58f 91e8 a18c  lt="............
+000007b0: e789 8822 2073 7263 3d22 6874 7470 733a  ..." src="https:
+000007c0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000007d0: 2f67 6974 6875 622f 762f 7265 6c65 6173  /github/v/releas
+000007e0: 652f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  e/Ljzd-PRO/noneb
+000007f0: 6f74 2d70 6c75 6769 6e2d 6d79 7354 6f6f  ot-plugin-mysToo
+00000800: 6c3f 6c6f 676f 3d70 7974 686f 6e26 7374  l?logo=python&st
+00000810: 796c 653d 666f 722d 7468 652d 6261 6467  yle=for-the-badg
+00000820: 6522 3e0a 2020 3c69 6d67 2061 6c74 3d22  e">.  <img alt="
+00000830: e69c 80e5 908e e68f 90e4 baa4 2220 7372  ............" sr
+00000840: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000850: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00000860: 2f6c 6173 742d 636f 6d6d 6974 2f4c 6a7a  /last-commit/Ljz
+00000870: 642d 5052 4f2f 6e6f 6e65 626f 742d 706c  d-PRO/nonebot-pl
+00000880: 7567 696e 2d6d 7973 546f 6f6c 3f73 7479  ugin-mysTool?sty
+00000890: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+000008a0: 223e 0a3c 2f64 6976 3e0a 0a23 206d 7973  ">.</div>..# mys
+000008b0: 546f 6f6c 202d 20e7 b1b3 e6b8 b8e7 a4be  Tool - .........
+000008c0: e8be 85e5 8aa9 e5b7 a5e5 85b7 e68f 92e4  ................
+000008d0: bbb6 0a0a 2a2a e789 88e6 9cac 202d 2076  ....**...... - v
+000008e0: 302e 322e 392a 2a0a 0a23 2323 20f0 9f93  0.2.9**..### ...
+000008f0: a320 e69b b4e6 96b0 e586 85e5 aeb9 0a0a  . ..............
+00000900: 2323 2323 2032 3032 332e 352e 3138 0a2d  #### 2023.5.18.-
+00000910: 20e5 a49a e8bf 9be7 a88b e794 9fe6 8890   ...............
+00000920: e595 86e5 9381 e59b bee7 8987 efbc 88e5  ................
+00000930: a49a e6a0 b8ef bc89 efbc 8ce5 8aa0 e5bf  ................
+00000940: abe5 9bbe e789 87e7 949f e688 90e9 809f  ................
+00000950: e5ba a60a 2d20 e4bf aee5 a48d e983 a8e5  ....- ..........
+00000960: 8886 e595 86e5 9381 e585 91e6 8da2 e697  ................
+00000970: b6e9 97b4 e994 99e8 afaf e79a 84e9 97ae  ................
+00000980: e9a2 98ef bc88 e5a6 82e7 b1b3 e6b8 b8e7  ................
+00000990: a4be e595 86e5 9381 e699 9ae4 ba86 e4b8  ................
+000009a0: 80e5 91a8 efbc 890a 0a23 2323 2320 3230  .........#### 20
+000009b0: 3233 2e35 2e34 0a2d 20e5 a29e e58a a0e5  23.5.4.- .......
+000009c0: afb9 e698 9fe7 a9b9 e993 81e9 8193 e79a  ................
+000009d0: 84e7 adbe e588 b0e5 8a9f e883 bde7 9a84  ................
+000009e0: e694 afe6 8c81 202d 205b 2338 395d 2868  ...... - [#89](h
+000009f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000a00: 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  m/Ljzd-PRO/noneb
+00000a10: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
+00000a20: 6c2f 7075 6c6c 2f38 3929 2062 7920 4061  l/pull/89) by @a
+00000a30: 7961 6b61 7375 6b69 0a2d 20e4 bfae e5a4  yakasuki.- .....
+00000a40: 8de6 8f92 e4bb b6e5 91bd e4bb a4e4 bc98  ................
+00000a50: e585 88e5 baa6 e997 aee9 a298 202d 205b  ............ - [
+00000a60: 2338 385d 2868 7474 7073 3a2f 2f67 6974  #88](https://git
+00000a70: 6875 622e 636f 6d2f 4c6a 7a64 2d50 524f  hub.com/Ljzd-PRO
+00000a80: 2f6e 6f6e 6562 6f74 2d70 6c75 6769 6e2d  /nonebot-plugin-
+00000a90: 6d79 7374 6f6f 6c2f 7075 6c6c 2f38 3829  mystool/pull/88)
+00000aa0: 2062 7920 4061 7961 6b61 7375 6b69 0a2d   by @ayakasuki.-
+00000ab0: 20e9 83a8 e588 86e6 9687 e69c ace9 9499   ...............
+00000ac0: e8af afe4 bfae e6ad a320 2d20 5b23 3930  ......... - [#90
+00000ad0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000ae0: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
+00000af0: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
+00000b00: 746f 6f6c 2f70 756c 6c2f 3930 2920 6279  tool/pull/90) by
+00000b10: 2040 626c 6163 6b2d 7a65 726f 3335 380a   @black-zero358.
+00000b20: 0a2e 2e2e 0a0a 2323 2323 2032 3032 332e  ......#### 2023.
+00000b30: 332e 3330 0a2d 20e4 bfae e5a4 8d20 602f  3.30.- ...... `/
+00000b40: e585 91e6 8da2 6020 e591 bde4 bba4 e58f  ......` ........
+00000b50: afe8 83bd e4b8 8ee5 85b6 e4bb 96e6 8f92  ................
+00000b60: e4bb b6e5 91bd e4bb a4e5 86b2 e7aa 81e7  ................
+00000b70: 9a84 e997 aee9 a298 efbc 8ce5 908c e697  ................
+00000b80: b620 5bf0 9f94 97e7 94a8 e6b3 95e5 8f98  . [.............
+00000b90: e69b b45d 2868 7474 7073 3a2f 2f67 6974  ...](https://git
+00000ba0: 6875 622e 636f 6d2f 4c6a 7a64 2d50 524f  hub.com/Ljzd-PRO
+00000bb0: 2f6e 6f6e 6562 6f74 2d70 6c75 6769 6e2d  /nonebot-plugin-
+00000bc0: 6d79 7374 6f6f 6c2f 7769 6b69 2f49 6e66  mystool/wiki/Inf
+00000bd0: 6f72 6d61 7469 6f6e 2d45 7863 6861 6e67  ormation-Exchang
+00000be0: 6523 e5a2 9ee5 8aa0 e588 a0e9 99a4 e585  e#..............
+00000bf0: 91e6 8da2 e8ae a1e5 8892 290a 2d20 2e2e  ..........).- ..
+00000c00: 2e0a 0a23 2320 e58a 9fe8 83bd e592 8ce7  ...## ..........
+00000c10: 89b9 e680 a70a 0a2d 20e7 9fad e4bf a1e9  .......- .......
+00000c20: aa8c e8af 81e7 99bb e5bd 95ef bc8c e585  ................
+00000c30: 8de6 8a93 e58c 85e8 8eb7 e58f 9620 436f  ............. Co
+00000c40: 6f6b 6965 0a2d 20e8 87aa e58a a8e5 ae8c  okie.- .........
+00000c50: e688 90e6 af8f e697 a5e7 b1b3 e6b8 b8e5  ................
+00000c60: b881 e4bb bbe5 8aa1 0a2d 20e8 87aa e58a  .........- .....
+00000c70: a8e8 bf9b e8a1 8ce6 b8b8 e688 8fe7 adbe  ................
+00000c80: e588 b00a 2d20 e58f afe5 88b6 e5ae 9ae7  ....- ..........
+00000c90: b1b3 e6b8 b8e5 b881 e595 86e5 9381 e585  ................
+00000ca0: 91e6 8da2 e8ae a1e5 8892 efbc 8ce5 88b0  ................
+00000cb0: e782 b9e5 8591 e68d a20a 2d20 e58f afe6  ..........- ....
+00000cc0: 94af e68c 81e5 a49a e4b8 aa20 5151 20e8  ........... QQ .
+00000cd0: b4a6 e58f b7ef bc8c e6af 8fe4 b8aa 2051  .............. Q
+00000ce0: 5120 e8b4 a6e5 8fb7 e58f afe7 bb91 e5ae  Q ..............
+00000cf0: 9ae5 a49a e4b8 aae7 b1b3 e593 88e6 b8b8  ................
+00000d00: e8b4 a6e6 88b7 0a2d 2051 5120 e68e a8e9  .......- QQ ....
+00000d10: 8081 e689 a7e8 a18c e7bb 93e6 9e9c e980  ................
+00000d20: 9ae7 9fa5 0a2d 20e5 8e9f e7a5 9ee6 a091  .....- .........
+00000d30: e884 82e3 8081 e6b4 9ee5 a4a9 e5ae 9de9  ................
+00000d40: 92b1 e380 81e8 b4a8 e987 8fe5 8f82 e58f  ................
+00000d50: 98e4 bbaa e5b7 b2e6 bba1 e697 b6e6 8ea8  ................
+00000d60: e980 81e9 809a e79f a50a 0a23 2320 e4bd  ...........## ..
+00000d70: bfe7 94a8 e8af b4e6 988e 0a0a 2323 2320  ............### 
+00000d80: f09f 9ba0 efb8 8f20 4e6f 6e65 426f 7432  ....... NoneBot2
+00000d90: 20e6 9cba e599 a8e4 baba e983 a8e7 bdb2   ...............
+00000da0: e592 8ce6 8f92 e4bb b6e5 ae89 e8a3 850a  ................
+00000db0: 0ae8 afb7 e69f a5e7 9c8b 202d 3e20 5bf0  .......... -> [.
+00000dc0: 9f94 9749 6e73 7461 6c6c 6174 696f 6e5d  ...Installation]
+00000dd0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000de0: 636f 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e  com/Ljzd-PRO/non
+00000df0: 6562 6f74 2d70 6c75 6769 6e2d 6d79 7374  ebot-plugin-myst
+00000e00: 6f6f 6c2f 7769 6b69 2f49 6e73 7461 6c6c  ool/wiki/Install
+00000e10: 6174 696f 6e29 0a0a 2323 2320 f09f 9396  ation)..### ....
+00000e20: 20e6 8f92 e4bb b6e5 85b7 e4bd 93e4 bdbf   ...............
+00000e30: e794 a8e8 afb4 e698 8e0a 0ae8 afb7 e69f  ................
+00000e40: a5e7 9c8b 202d 3e20 5bf0 9f94 9757 696b  .... -> [....Wik
+00000e50: 6920 e696 87e6 a1a3 5d28 6874 7470 733a  i ......](https:
+00000e60: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 6a7a  //github.com/Ljz
+00000e70: 642d 5052 4f2f 6e6f 6e65 626f 742d 706c  d-PRO/nonebot-pl
+00000e80: 7567 696e 2d6d 7973 746f 6f6c 2f77 696b  ugin-mystool/wik
+00000e90: 6929 0a0a 2323 2320 e29d 9320 e88e b7e5  i)..### ... ....
+00000ea0: 8f96 e68f 92e4 bbb6 e5b8 aee5 8aa9 e4bf  ................
+00000eb0: a1e6 81af 0a0a 2323 2323 20e6 8f92 e4bb  ......#### .....
+00000ec0: b6e5 91bd e4bb a40a 0a60 6060 0a2f e5b8  .........```./..
+00000ed0: aee5 8aa9 0a60 6060 0a0a 3e20 e29a a0ef  .....```..> ....
+00000ee0: b88f 20e6 b3a8 e684 8f20 e6ad a4e5 a484  .. ...... ......
+00000ef0: e6b2 a1e6 9c89 e4bd bfe7 94a8 205b f09f  ............ [..
+00000f00: 9497 20e6 8f92 e4bb b6e5 91bd e4bb a4e5  .. .............
+00000f10: a4b4 5d28 6874 7470 733a 2f2f 6769 7468  ..](https://gith
+00000f20: 7562 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f  ub.com/Ljzd-PRO/
+00000f30: 6e6f 6e65 626f 742d 706c 7567 696e 2d6d  nonebot-plugin-m
+00000f40: 7973 746f 6f6c 2f77 696b 692f 436f 6e66  ystool/wiki/Conf
+00000f50: 6967 7572 6174 696f 6e2d 436f 6e66 6967  iguration-Config
+00000f60: 2363 6f6d 6d61 6e64 5f73 7461 7274 290a  #command_start).
+00000f70: 0a23 2320 e585 b6e4 bb96 0a0a 2323 2320  .## ........### 
+00000f80: 5bf0 9f93 83e6 ba90 e7a0 81e8 afb4 e698  [...............
+00000f90: 8e5d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
+00000fa0: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+00000fb0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+00000fc0: 7374 6f6f 6c2f 7769 6b69 2f53 6f75 7263  stool/wiki/Sourc
+00000fd0: 652d 5374 7275 6374 7572 6529 0a23 2323  e-Structure).###
+00000fe0: 20e9 8082 e985 8d20 5be7 bbaa e5b1 b1e7   ...... [.......
+00000ff0: 9c9f e5af bb42 6f74 5d28 6874 7470 733a  .....Bot](https:
+00001000: 2f2f 6769 7468 7562 2e63 6f6d 2f48 6962  //github.com/Hib
+00001010: 694b 6965 722f 7a68 656e 7875 6e5f 626f  iKier/zhenxun_bo
+00001020: 7429 20e7 9a84 e588 86e6 94af 0a2d 2068  t) ..........- h
+00001030: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001040: 6d2f 4d57 544a 432f 7a68 656e 7875 6e2d  m/MWTJC/zhenxun-
+00001050: 706c 7567 696e 2d6d 7973 746f 6f6c 0a2d  plugin-mystool.-
+00001060: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00001070: 636f 6d2f 6179 616b 6173 756b 692f 6e6f  com/ayakasuki/no
+00001080: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
+00001090: 746f 6f6c 0a0a                           tool..
```

