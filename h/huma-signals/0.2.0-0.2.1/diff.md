# Comparing `tmp/huma_signals-0.2.0.tar.gz` & `tmp/huma_signals-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huma_signals-0.2.0.tar", max compression
+gzip compressed data, was "huma_signals-0.2.1.tar", max compression
```

## Comparing `huma_signals-0.2.0.tar` & `huma_signals-0.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    34523 2023-05-06 00:10:02.616918 huma_signals-0.2.0/LICENSE
--rw-r--r--   0        0        0     2173 2023-05-06 00:10:02.617080 huma_signals-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617555 huma_signals-0.2.0/huma_signals/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.941065 huma_signals-0.2.0/huma_signals/adapters/__init__.py
--rw-r--r--   0        0        0      586 2023-05-17 01:58:33.941184 huma_signals-0.2.0/huma_signals/adapters/ethereum_wallet/README.md
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.941215 huma_signals-0.2.0/huma_signals/adapters/ethereum_wallet/__init__.py
--rw-r--r--   0        0        0     3295 2023-05-17 01:58:33.941390 huma_signals-0.2.0/huma_signals/adapters/ethereum_wallet/adapter.py
--rw-r--r--   0        0        0      186 2023-05-17 01:58:33.941462 huma_signals-0.2.0/huma_signals/adapters/ethereum_wallet/settings.py
--rw-r--r--   0        0        0      586 2023-05-17 01:58:33.941558 huma_signals-0.2.0/huma_signals/adapters/lending_pools/README.md
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.941588 huma_signals-0.2.0/huma_signals/adapters/lending_pools/__init__.py
--rw-r--r--   0        0        0    23699 2023-05-17 01:58:33.941733 huma_signals-0.2.0/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json
--rw-r--r--   0        0        0    30632 2023-05-17 01:58:33.941925 huma_signals-0.2.0/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json
--rw-r--r--   0        0        0    32155 2023-05-17 01:58:33.942012 huma_signals-0.2.0/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json
--rw-r--r--   0        0        0    30290 2023-05-17 01:58:33.942126 huma_signals-0.2.0/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json
--rw-r--r--   0        0        0     4719 2023-05-17 01:58:33.942333 huma_signals-0.2.0/huma_signals/adapters/lending_pools/adapter.py
--rw-r--r--   0        0        0     1938 2023-05-17 01:58:33.942403 huma_signals-0.2.0/huma_signals/adapters/lending_pools/registry.py
--rw-r--r--   0        0        0      158 2023-05-17 01:58:33.942479 huma_signals-0.2.0/huma_signals/adapters/lending_pools/settings.py
--rw-r--r--   0        0        0      582 2023-05-17 01:58:33.942545 huma_signals-0.2.0/huma_signals/adapters/models.py
--rw-r--r--   0        0        0      591 2023-05-17 01:58:33.942633 huma_signals-0.2.0/huma_signals/adapters/polygon_wallet/README.md
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.942663 huma_signals-0.2.0/huma_signals/adapters/polygon_wallet/__init__.py
--rw-r--r--   0        0        0     3406 2023-05-17 01:58:33.942804 huma_signals-0.2.0/huma_signals/adapters/polygon_wallet/adapter.py
--rw-r--r--   0        0        0      222 2023-05-17 01:58:33.942860 huma_signals-0.2.0/huma_signals/adapters/polygon_wallet/settings.py
--rw-r--r--   0        0        0      576 2023-05-17 01:58:33.942959 huma_signals-0.2.0/huma_signals/adapters/request_network/README.md
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.942989 huma_signals-0.2.0/huma_signals/adapters/request_network/__init__.py
--rw-r--r--   0        0        0     4372 2023-05-17 01:58:33.943071 huma_signals-0.2.0/huma_signals/adapters/request_network/models.py
--rw-r--r--   0        0        0     5889 2023-05-17 01:58:33.943221 huma_signals-0.2.0/huma_signals/adapters/request_network/request_invoice_adapter.py
--rw-r--r--   0        0        0     5202 2023-05-17 01:58:33.943386 huma_signals-0.2.0/huma_signals/adapters/request_network/request_transaction_adapter.py
--rw-r--r--   0        0        0      284 2023-05-17 01:58:33.943449 huma_signals-0.2.0/huma_signals/adapters/request_network/settings.py
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.943514 huma_signals-0.2.0/huma_signals/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.943585 huma_signals-0.2.0/huma_signals/clients/eth_client/__init__.py
--rw-r--r--   0        0        0     1427 2023-05-17 01:58:33.943803 huma_signals-0.2.0/huma_signals/clients/eth_client/eth_client.py
--rw-r--r--   0        0        0      673 2023-05-17 01:58:33.943860 huma_signals-0.2.0/huma_signals/clients/eth_client/eth_types.py
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.943913 huma_signals-0.2.0/huma_signals/clients/polygon_client/__init__.py
--rw-r--r--   0        0        0     1503 2023-05-17 01:58:33.944103 huma_signals-0.2.0/huma_signals/clients/polygon_client/polygon_client.py
--rw-r--r--   0        0        0      685 2023-05-17 01:58:33.944154 huma_signals-0.2.0/huma_signals/clients/polygon_client/polygon_types.py
--rw-r--r--   0        0        0        0 2023-05-17 01:58:33.944206 huma_signals-0.2.0/huma_signals/clients/request_client/__init__.py
--rw-r--r--   0        0        0     8129 2023-05-17 01:58:33.944358 huma_signals-0.2.0/huma_signals/clients/request_client/request_client.py
--rw-r--r--   0        0        0      900 2023-05-17 01:58:33.944420 huma_signals-0.2.0/huma_signals/clients/request_client/request_types.py
--rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617961 huma_signals-0.2.0/huma_signals/commons/__init__.py
--rw-r--r--   0        0        0      291 2023-05-17 01:58:33.944586 huma_signals-0.2.0/huma_signals/commons/chains.py
--rw-r--r--   0        0        0      330 2023-05-06 00:10:02.618090 huma_signals-0.2.0/huma_signals/commons/datetime_utils.py
--rw-r--r--   0        0        0      227 2023-05-06 00:10:02.618146 huma_signals-0.2.0/huma_signals/commons/pydantic_utils.py
--rw-r--r--   0        0        0      569 2023-05-06 00:10:02.618202 huma_signals-0.2.0/huma_signals/commons/string_utils.py
--rw-r--r--   0        0        0     1309 2023-05-06 00:10:02.618262 huma_signals-0.2.0/huma_signals/commons/tokens.py
--rw-r--r--   0        0        0     1078 2023-05-06 00:10:02.618330 huma_signals-0.2.0/huma_signals/commons/web3_utils.py
--rw-r--r--   0        0        0      499 2023-05-17 18:27:08.499593 huma_signals-0.2.0/huma_signals/dotenv/example.env
--rw-r--r--   0        0        0      946 2023-05-17 01:36:29.827407 huma_signals-0.2.0/huma_signals/exceptions.py
--rw-r--r--   0        0        0      322 2023-05-06 00:10:02.621231 huma_signals-0.2.0/huma_signals/models.py
--rw-r--r--   0        0        0        0 2023-05-10 00:22:05.269455 huma_signals-0.2.0/huma_signals/py.typed
--rw-r--r--   0        0        0     1563 2023-05-17 18:27:08.499698 huma_signals-0.2.0/huma_signals/settings.py
--rw-r--r--   0        0        0     2792 2023-05-17 22:14:47.642109 huma_signals-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3121 1970-01-01 00:00:00.000000 huma_signals-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-06 00:10:02.616918 huma_signals-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2162 2023-05-17 23:08:07.445627 huma_signals-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617555 huma_signals-0.2.1/huma_signals/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 01:58:33.941065 huma_signals-0.2.1/huma_signals/adapters/__init__.py
+-rw-r--r--   0        0        0      586 2023-05-17 01:58:33.941184 huma_signals-0.2.1/huma_signals/adapters/ethereum_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 01:58:33.941215 huma_signals-0.2.1/huma_signals/adapters/ethereum_wallet/__init__.py
+-rw-r--r--   0        0        0     3295 2023-05-17 01:58:33.941390 huma_signals-0.2.1/huma_signals/adapters/ethereum_wallet/adapter.py
+-rw-r--r--   0        0        0      186 2023-05-17 01:58:33.941462 huma_signals-0.2.1/huma_signals/adapters/ethereum_wallet/settings.py
+-rw-r--r--   0        0        0      586 2023-05-17 01:58:33.941558 huma_signals-0.2.1/huma_signals/adapters/lending_pools/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 01:58:33.941588 huma_signals-0.2.1/huma_signals/adapters/lending_pools/__init__.py
+-rw-r--r--   0        0        0    23699 2023-05-17 01:58:33.941733 huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json
+-rw-r--r--   0        0        0    30632 2023-05-17 01:58:33.941925 huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json
+-rw-r--r--   0        0        0    32155 2023-05-17 01:58:33.942012 huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json
+-rw-r--r--   0        0        0    30290 2023-05-17 01:58:33.942126 huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json
+-rw-r--r--   0        0        0     4719 2023-05-17 01:58:33.942333 huma_signals-0.2.1/huma_signals/adapters/lending_pools/adapter.py
+-rw-r--r--   0        0        0     1938 2023-05-17 01:58:33.942403 huma_signals-0.2.1/huma_signals/adapters/lending_pools/registry.py
+-rw-r--r--   0        0        0      158 2023-05-17 01:58:33.942479 huma_signals-0.2.1/huma_signals/adapters/lending_pools/settings.py
+-rw-r--r--   0        0        0      582 2023-05-17 01:58:33.942545 huma_signals-0.2.1/huma_signals/adapters/models.py
+-rw-r--r--   0        0        0      591 2023-05-17 01:58:33.942633 huma_signals-0.2.1/huma_signals/adapters/polygon_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 01:58:33.942663 huma_signals-0.2.1/huma_signals/adapters/polygon_wallet/__init__.py
+-rw-r--r--   0        0        0     3406 2023-05-17 01:58:33.942804 huma_signals-0.2.1/huma_signals/adapters/polygon_wallet/adapter.py
+-rw-r--r--   0        0        0      222 2023-05-17 01:58:33.942860 huma_signals-0.2.1/huma_signals/adapters/polygon_wallet/settings.py
+-rw-r--r--   0        0        0      576 2023-05-17 01:58:33.942959 huma_signals-0.2.1/huma_signals/adapters/request_network/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 01:58:33.942989 huma_signals-0.2.1/huma_signals/adapters/request_network/__init__.py
+-rw-r--r--   0        0        0     4372 2023-05-17 01:58:33.943071 huma_signals-0.2.1/huma_signals/adapters/request_network/models.py
+-rw-r--r--   0        0        0     5889 2023-05-17 01:58:33.943221 huma_signals-0.2.1/huma_signals/adapters/request_network/request_invoice_adapter.py
+-rw-r--r--   0        0        0     5202 2023-05-17 01:58:33.943386 huma_signals-0.2.1/huma_signals/adapters/request_network/request_transaction_adapter.py
+-rw-r--r--   0        0        0      284 2023-05-17 01:58:33.943449 huma_signals-0.2.1/huma_signals/adapters/request_network/settings.py
+-rw-r--r--   0        0        0        0 2023-05-17 01:58:33.943514 huma_signals-0.2.1/huma_signals/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-17 01:58:33.943585 huma_signals-0.2.1/huma_signals/clients/eth_client/__init__.py
+-rw-r--r--   0        0        0     1427 2023-05-17 01:58:33.943803 huma_signals-0.2.1/huma_signals/clients/eth_client/eth_client.py
+-rw-r--r--   0        0        0      673 2023-05-17 01:58:33.943860 huma_signals-0.2.1/huma_signals/clients/eth_client/eth_types.py
+-rw-r--r--   0        0        0        0 2023-05-17 01:58:33.943913 huma_signals-0.2.1/huma_signals/clients/polygon_client/__init__.py
+-rw-r--r--   0        0        0     1503 2023-05-17 01:58:33.944103 huma_signals-0.2.1/huma_signals/clients/polygon_client/polygon_client.py
+-rw-r--r--   0        0        0      685 2023-05-17 01:58:33.944154 huma_signals-0.2.1/huma_signals/clients/polygon_client/polygon_types.py
+-rw-r--r--   0        0        0        0 2023-05-17 01:58:33.944206 huma_signals-0.2.1/huma_signals/clients/request_client/__init__.py
+-rw-r--r--   0        0        0     8129 2023-05-17 01:58:33.944358 huma_signals-0.2.1/huma_signals/clients/request_client/request_client.py
+-rw-r--r--   0        0        0      900 2023-05-17 01:58:33.944420 huma_signals-0.2.1/huma_signals/clients/request_client/request_types.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:02.617961 huma_signals-0.2.1/huma_signals/commons/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-17 01:58:33.944586 huma_signals-0.2.1/huma_signals/commons/chains.py
+-rw-r--r--   0        0        0      330 2023-05-06 00:10:02.618090 huma_signals-0.2.1/huma_signals/commons/datetime_utils.py
+-rw-r--r--   0        0        0      227 2023-05-06 00:10:02.618146 huma_signals-0.2.1/huma_signals/commons/pydantic_utils.py
+-rw-r--r--   0        0        0      569 2023-05-06 00:10:02.618202 huma_signals-0.2.1/huma_signals/commons/string_utils.py
+-rw-r--r--   0        0        0     1309 2023-05-06 00:10:02.618262 huma_signals-0.2.1/huma_signals/commons/tokens.py
+-rw-r--r--   0        0        0     1078 2023-05-06 00:10:02.618330 huma_signals-0.2.1/huma_signals/commons/web3_utils.py
+-rw-r--r--   0        0        0      499 2023-05-17 22:38:39.621240 huma_signals-0.2.1/huma_signals/dotenv/example.env
+-rw-r--r--   0        0        0      946 2023-05-17 01:36:29.827407 huma_signals-0.2.1/huma_signals/exceptions.py
+-rw-r--r--   0        0        0      322 2023-05-06 00:10:02.621231 huma_signals-0.2.1/huma_signals/models.py
+-rw-r--r--   0        0        0        0 2023-05-10 00:22:05.269455 huma_signals-0.2.1/huma_signals/py.typed
+-rw-r--r--   0        0        0     1563 2023-05-17 22:38:39.621299 huma_signals-0.2.1/huma_signals/settings.py
+-rw-r--r--   0        0        0     2792 2023-05-17 23:08:07.445943 huma_signals-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 huma_signals-0.2.1/PKG-INFO
```

### Comparing `huma_signals-0.2.0/LICENSE` & `huma_signals-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/README.md` & `huma_signals-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 <p align="center">
   <a href="https://huma.finance"><img src="https://user-images.githubusercontent.com/5999398/210867640-95c8944c-fcd0-4199-9f08-b0ae6eda70c0.jpg" alt="Huma Finance" width="500px"></a>
   <h1 align="center">Decentralized Signal Portfolio</h1>
 </p>
 
-
-
 <p align="center">
   <a href="https://github.com/00labs/huma-signals/actions" target="_blank">
-    <img alt="Action Status" src="https://github.com/00labs/huma-signals/actions/workflows/ci.yaml/badge.svg">
+    <img alt="Action Status" src="https://github.com/00labs/huma-signals/actions/workflows/ci-main.yml/badge.svg">
   </a>
-  <img alt="Version" src="https://img.shields.io/badge/version-0.1.0-blue.svg?cacheSeconds=2592000" />
+  <img alt="Version" src="https://img.shields.io/badge/version-0.2.1-blue.svg?cacheSeconds=2592000" />
   <a href="https://docs.huma.finance/" target="_blank">
     <img alt="Documentation" src="https://img.shields.io/badge/documentation-yes-brightgreen.svg" />
   </a>
   <a href="https://discord.gg/7e2fdMSCZr">
     <img alt="" src="https://badgen.net/badge/Join/HUMAnity%20Discord/cyan?icon=discor">
   </a>
   <a href="https://www.gnu.org/licenses/agpl-3.0.en.html" target="_blank">
     <img alt="License: AGPLv3" src="https://img.shields.io/badge/License-AGPLv3-yellow.svg" />
   </a>
   <a href="https://twitter.com/humafinance" target="_blank">
     <img alt="Twitter: humafinance" src="https://img.shields.io/twitter/follow/humafinance.svg?style=social" />
   </a>
 
-The Decentralized Signal Portfolio (DSP) is an open platform that enables access to high-quality signals about a borrower's income, assets, and liabilities. These signals are collected through Signal Adapters hosted on the DSP, which gather data from a variety of on-chain and off-chain sources. Any developer can contribute to the platform by adding a new Signal Adapter for a specific data source.
-
+The Decentralized Signal Portfolio (DSP) is an open source package that enables access to high-quality signals about a borrower's income, assets, and liabilities. These signals are collected through Signal Adapters, which gather data from a variety of on-chain and off-chain sources. Any developer can contribute to the platform by adding a new Signal Adapter for a specific data source.
 </p>
 
 ## Overview
 
 📜 [Huma Whitepaper](https://docs.huma.finance/)
 
 🏠 [Homepage](https://huma.finance)
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
                                 [Huma_Finance]
                  ****** Decentralized Signal Portfolio ******
     [Action_Status] [Version] [Documentation]  [License:_AGPLv3] [Twitter:
-humafinance] The Decentralized Signal Portfolio (DSP) is an open platform that
- enables access to high-quality signals about a borrower's income, assets, and
-liabilities. These signals are collected through Signal Adapters hosted on the
- DSP, which gather data from a variety of on-chain and off-chain sources. Any
- developer can contribute to the platform by adding a new Signal Adapter for a
-                             specific data source.
+humafinance] The Decentralized Signal Portfolio (DSP) is an open source package
+that enables access to high-quality signals about a borrower's income, assets,
+  and liabilities. These signals are collected through Signal Adapters, which
+gather data from a variety of on-chain and off-chain sources. Any developer can
+ contribute to the platform by adding a new Signal Adapter for a specific data
+                                    source.
 ## Overview ð [Huma Whitepaper](https://docs.huma.finance/) ð  [Homepage]
 (https://huma.finance) ## Documentation For additional guides, examples, and
 APIs, see the [documentation](./docs/). ## Want to help? Give a â­ï¸ if this
 project helped you! Want to file a bug, contribute some code, or improve the
 documentation? Excellent! Read up on our guidelines for [contributing]
 (.docs/../docs/contributing.md). ## ð License This project is [AGPL v3]
 (https://www.gnu.org/licenses/agpl-3.0.en.html) licensed.
```

### Comparing `huma_signals-0.2.0/huma_signals/adapters/ethereum_wallet/README.md` & `huma_signals-0.2.1/huma_signals/adapters/ethereum_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/ethereum_wallet/adapter.py` & `huma_signals-0.2.1/huma_signals/adapters/ethereum_wallet/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/lending_pools/README.md` & `huma_signals-0.2.1/huma_signals/adapters/lending_pools/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json` & `huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json` & `huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json` & `huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json` & `huma_signals-0.2.1/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/lending_pools/adapter.py` & `huma_signals-0.2.1/huma_signals/adapters/lending_pools/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/lending_pools/registry.py` & `huma_signals-0.2.1/huma_signals/adapters/lending_pools/registry.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/models.py` & `huma_signals-0.2.1/huma_signals/adapters/models.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/polygon_wallet/README.md` & `huma_signals-0.2.1/huma_signals/adapters/polygon_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/polygon_wallet/adapter.py` & `huma_signals-0.2.1/huma_signals/adapters/polygon_wallet/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/request_network/README.md` & `huma_signals-0.2.1/huma_signals/adapters/request_network/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/request_network/models.py` & `huma_signals-0.2.1/huma_signals/adapters/request_network/models.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/request_network/request_invoice_adapter.py` & `huma_signals-0.2.1/huma_signals/adapters/request_network/request_invoice_adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/adapters/request_network/request_transaction_adapter.py` & `huma_signals-0.2.1/huma_signals/adapters/request_network/request_transaction_adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/clients/eth_client/eth_client.py` & `huma_signals-0.2.1/huma_signals/clients/eth_client/eth_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/clients/eth_client/eth_types.py` & `huma_signals-0.2.1/huma_signals/clients/eth_client/eth_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/clients/polygon_client/polygon_client.py` & `huma_signals-0.2.1/huma_signals/clients/polygon_client/polygon_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/clients/polygon_client/polygon_types.py` & `huma_signals-0.2.1/huma_signals/clients/polygon_client/polygon_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/clients/request_client/request_client.py` & `huma_signals-0.2.1/huma_signals/clients/request_client/request_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/clients/request_client/request_types.py` & `huma_signals-0.2.1/huma_signals/clients/request_client/request_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/commons/string_utils.py` & `huma_signals-0.2.1/huma_signals/commons/string_utils.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/commons/tokens.py` & `huma_signals-0.2.1/huma_signals/commons/tokens.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/commons/web3_utils.py` & `huma_signals-0.2.1/huma_signals/commons/web3_utils.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/exceptions.py` & `huma_signals-0.2.1/huma_signals/exceptions.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/huma_signals/settings.py` & `huma_signals-0.2.1/huma_signals/settings.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.2.0/pyproject.toml` & `huma_signals-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huma-signals"
-version = "0.2.0"
+version = "0.2.1"
 description = "Enables access to high-quality signals about a borrower's income, assets, and liabilities."
 authors = ["Jiatu Liu <jiatu@huma.finance>", "Ji Peng <ji@huma.finance>"]
 license = "AGPL v3"
 readme = "README.md"
 packages = [{include = "huma_signals"}]
 homepage = "https://github.com/00labs/huma-signals/"
 documentation = "https://docs.huma.finance/developer-guidelines/decentralized_signal_portfolio"
```

### Comparing `huma_signals-0.2.0/PKG-INFO` & `huma_signals-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huma-signals
-Version: 0.2.0
+Version: 0.2.1
 Summary: Enables access to high-quality signals about a borrower's income, assets, and liabilities.
 Home-page: https://github.com/00labs/huma-signals/
 License: AGPL v3
 Author: Jiatu Liu
 Author-email: jiatu@huma.finance
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
@@ -22,36 +22,33 @@
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://huma.finance"><img src="https://user-images.githubusercontent.com/5999398/210867640-95c8944c-fcd0-4199-9f08-b0ae6eda70c0.jpg" alt="Huma Finance" width="500px"></a>
   <h1 align="center">Decentralized Signal Portfolio</h1>
 </p>
 
-
-
 <p align="center">
   <a href="https://github.com/00labs/huma-signals/actions" target="_blank">
-    <img alt="Action Status" src="https://github.com/00labs/huma-signals/actions/workflows/ci.yaml/badge.svg">
+    <img alt="Action Status" src="https://github.com/00labs/huma-signals/actions/workflows/ci-main.yml/badge.svg">
   </a>
-  <img alt="Version" src="https://img.shields.io/badge/version-0.1.0-blue.svg?cacheSeconds=2592000" />
+  <img alt="Version" src="https://img.shields.io/badge/version-0.2.1-blue.svg?cacheSeconds=2592000" />
   <a href="https://docs.huma.finance/" target="_blank">
     <img alt="Documentation" src="https://img.shields.io/badge/documentation-yes-brightgreen.svg" />
   </a>
   <a href="https://discord.gg/7e2fdMSCZr">
     <img alt="" src="https://badgen.net/badge/Join/HUMAnity%20Discord/cyan?icon=discor">
   </a>
   <a href="https://www.gnu.org/licenses/agpl-3.0.en.html" target="_blank">
     <img alt="License: AGPLv3" src="https://img.shields.io/badge/License-AGPLv3-yellow.svg" />
   </a>
   <a href="https://twitter.com/humafinance" target="_blank">
     <img alt="Twitter: humafinance" src="https://img.shields.io/twitter/follow/humafinance.svg?style=social" />
   </a>
 
-The Decentralized Signal Portfolio (DSP) is an open platform that enables access to high-quality signals about a borrower's income, assets, and liabilities. These signals are collected through Signal Adapters hosted on the DSP, which gather data from a variety of on-chain and off-chain sources. Any developer can contribute to the platform by adding a new Signal Adapter for a specific data source.
-
+The Decentralized Signal Portfolio (DSP) is an open source package that enables access to high-quality signals about a borrower's income, assets, and liabilities. These signals are collected through Signal Adapters, which gather data from a variety of on-chain and off-chain sources. Any developer can contribute to the platform by adding a new Signal Adapter for a specific data source.
 </p>
 
 ## Overview
 
 📜 [Huma Whitepaper](https://docs.huma.finance/)
 
 🏠 [Homepage](https://huma.finance)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: huma-signals Version: 0.2.0 Summary: Enables access
+Metadata-Version: 2.1 Name: huma-signals Version: 0.2.1 Summary: Enables access
 to high-quality signals about a borrower's income, assets, and liabilities.
 Home-page: https://github.com/00labs/huma-signals/ License: AGPL v3 Author:
 Jiatu Liu Author-email: jiatu@huma.finance Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: aiofiles (>=22.1.0,<23.0.0) Requires-Dist: httpx
 (>=0.24.0,<0.25.0) Requires-Dist: orjson (>=3.8.5,<4.0.0) Requires-Dist: pandas
@@ -10,20 +10,20 @@
 urllib3 (>=1.26,<2.0) Requires-Dist: web3 (>=6.1.0,<7.0.0) Project-URL:
 Documentation, https://docs.huma.finance/developer-guidelines/
 decentralized_signal_portfolio Project-URL: Repository, https://github.com/
 00labs/huma-signals.git Description-Content-Type: text/markdown
                                 [Huma_Finance]
                  ****** Decentralized Signal Portfolio ******
     [Action_Status] [Version] [Documentation]  [License:_AGPLv3] [Twitter:
-humafinance] The Decentralized Signal Portfolio (DSP) is an open platform that
- enables access to high-quality signals about a borrower's income, assets, and
-liabilities. These signals are collected through Signal Adapters hosted on the
- DSP, which gather data from a variety of on-chain and off-chain sources. Any
- developer can contribute to the platform by adding a new Signal Adapter for a
-                             specific data source.
+humafinance] The Decentralized Signal Portfolio (DSP) is an open source package
+that enables access to high-quality signals about a borrower's income, assets,
+  and liabilities. These signals are collected through Signal Adapters, which
+gather data from a variety of on-chain and off-chain sources. Any developer can
+ contribute to the platform by adding a new Signal Adapter for a specific data
+                                    source.
 ## Overview ð [Huma Whitepaper](https://docs.huma.finance/) ð  [Homepage]
 (https://huma.finance) ## Documentation For additional guides, examples, and
 APIs, see the [documentation](./docs/). ## Want to help? Give a â­ï¸ if this
 project helped you! Want to file a bug, contribute some code, or improve the
 documentation? Excellent! Read up on our guidelines for [contributing]
 (.docs/../docs/contributing.md). ## ð License This project is [AGPL v3]
 (https://www.gnu.org/licenses/agpl-3.0.en.html) licensed.
```

