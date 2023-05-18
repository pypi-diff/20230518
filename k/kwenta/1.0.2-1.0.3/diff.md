# Comparing `tmp/kwenta-1.0.2.tar.gz` & `tmp/kwenta-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwenta-1.0.2.tar", last modified: Mon Apr 10 21:47:10 2023, max compression
+gzip compressed data, was "kwenta-1.0.3.tar", last modified: Thu May 18 20:26:03 2023, max compression
```

## Comparing `kwenta-1.0.2.tar` & `kwenta-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:47:10.482463 kwenta-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-10 21:47:10.482463 kwenta-1.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:47:10.478462 kwenta-1.0.2/kwenta/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 21:46:37.000000 kwenta-1.0.2/kwenta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-10 21:46:37.000000 kwenta-1.0.2/kwenta/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    28866 2023-04-10 21:46:37.000000 kwenta-1.0.2/kwenta/kwenta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:47:10.478462 kwenta-1.0.2/kwenta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-10 21:47:10.000000 kwenta-1.0.2/kwenta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-10 21:47:10.000000 kwenta-1.0.2/kwenta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:47:10.000000 kwenta-1.0.2/kwenta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-10 21:47:10.000000 kwenta-1.0.2/kwenta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 21:47:10.000000 kwenta-1.0.2/kwenta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 21:47:10.482463 kwenta-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-10 21:46:37.000000 kwenta-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:26:03.035464 kwenta-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-18 20:26:03.035464 kwenta-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:26:03.031464 kwenta-1.0.3/kwenta/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 20:25:29.000000 kwenta-1.0.3/kwenta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-18 20:25:29.000000 kwenta-1.0.3/kwenta/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43018 2023-05-18 20:25:29.000000 kwenta-1.0.3/kwenta/kwenta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:26:03.035464 kwenta-1.0.3/kwenta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-18 20:26:03.000000 kwenta-1.0.3/kwenta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-18 20:26:03.000000 kwenta-1.0.3/kwenta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 20:26:03.000000 kwenta-1.0.3/kwenta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 20:26:03.000000 kwenta-1.0.3/kwenta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 20:26:03.000000 kwenta-1.0.3/kwenta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 20:26:03.000000 kwenta-1.0.3/kwenta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 20:26:03.035464 kwenta-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-18 20:25:29.000000 kwenta-1.0.3/setup.py
```

### Comparing `kwenta-1.0.2/PKG-INFO` & `kwenta-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.2/kwenta/constants.py` & `kwenta-1.0.3/kwenta/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,7 +7,12 @@
     420: 'https://api.thegraph.com/subgraphs/name/kwenta/optimism-goerli-perps'
 }
 
 DEFAULT_GQL_ENDPOINT_RATES = {
     10: 'https://api.thegraph.com/subgraphs/name/kwenta/optimism-latest-rates',
     420: 'https://api.thegraph.com/subgraphs/name/kwenta/optimism-goerli-latest-rates'
 }
+
+DEFAULT_PRICE_SERVICE_ENDPOINTS = {
+    10: 'https://xc-mainnet.pyth.network',
+    420: 'https://xc-testnet.pyth.network'
+}
```

### Comparing `kwenta-1.0.2/kwenta/kwenta.py` & `kwenta-1.0.3/kwenta/kwenta.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,55 @@
+import asyncio
 import time
 import warnings
 from web3 import Web3
 from web3.types import TxParams
+from web3.middleware import geth_poa_middleware
 from decimal import Decimal
-from .constants import DEFAULT_NETWORK_ID, DEFAULT_TRACKING_CODE, DEFAULT_SLIPPAGE, DEFAULT_GQL_ENDPOINT_PERPS, DEFAULT_GQL_ENDPOINT_RATES
+from .constants import DEFAULT_NETWORK_ID, DEFAULT_TRACKING_CODE, DEFAULT_SLIPPAGE, DEFAULT_GQL_ENDPOINT_PERPS, DEFAULT_GQL_ENDPOINT_RATES, DEFAULT_PRICE_SERVICE_ENDPOINTS
 from .contracts import abis, addresses
 from .alerts import Alerts
 from .queries import Queries
+from .pyth import Pyth
 
 warnings.filterwarnings('ignore')
 
 
 class Kwenta:
     def __init__(
             self,
             provider_rpc: str,
             wallet_address: str,
             private_key: str = None,
             network_id: int = None,
+            use_estimate_gas: bool = True,
             gql_endpoint_perps: str = None,
             gql_endpoint_rates: str = None,
+            price_service_endpoint: str = None,
             telegram_token: str = None,
             telegram_channel_name: str = None):
         # set default values
         if network_id is None:
             network_id = DEFAULT_NETWORK_ID
 
         # init account variables
         self.private_key = private_key
         self.wallet_address = wallet_address
+        self.use_estimate_gas = use_estimate_gas
+        self.provider_rpc = provider_rpc
 
         # init provider
-        w3 = Web3(Web3.HTTPProvider(provider_rpc))
-        if w3.eth.chain_id != network_id:
-            raise Exception("The RPC `chain_id` must match `network_id`")
+        if provider_rpc.startswith('https'):
+            self.provider_class = Web3.HTTPProvider
+        elif provider_rpc.startswith('wss'):
+            self.provider_class = Web3.WebsocketProvider
         else:
-            self.network_id = network_id
-            self.web3 = w3
+            raise Exception("RPC endpoint is invalid")
+
+        self.network_id = network_id
 
         # init contracts
         self.markets, self.market_contracts, self.susd_token = self._load_markets()
         self.token_list = list(self.markets.keys())
 
         # init alerts
         if telegram_token and telegram_channel_name:
@@ -50,17 +59,37 @@
         if not gql_endpoint_perps:
             gql_endpoint_perps = DEFAULT_GQL_ENDPOINT_PERPS[self.network_id]
 
         if not gql_endpoint_rates:
             gql_endpoint_rates = DEFAULT_GQL_ENDPOINT_RATES[self.network_id]
 
         self.queries = Queries(
+            self,
             gql_endpoint_perps=gql_endpoint_perps,
             gql_endpoint_rates=gql_endpoint_rates)
 
+        # init pyth
+        if not price_service_endpoint:
+            price_service_endpoint = DEFAULT_PRICE_SERVICE_ENDPOINTS[self.network_id]
+
+        self.pyth = Pyth(
+            self.network_id, price_service_endpoint=price_service_endpoint)
+
+    @property
+    def web3(self):
+        w3 = Web3(self.provider_class(self.provider_rpc))
+
+        if w3.eth.chain_id != self.network_id:
+            raise Exception("The RPC `chain_id` must match the stored `network_id`")
+        else:
+            w3.middleware_onion.inject(geth_poa_middleware, layer=0)
+            self.nonce = w3.eth.get_transaction_count(self.wallet_address)
+            return w3
+
+
     def _load_markets(self):
         """
         Initializes all market contracts
         ...
 
         Attributes
         ----------
@@ -72,15 +101,15 @@
             marketdata_contract.functions.allProxiedMarketSummaries().call())
         markets = {}
         market_contracts = {}
         for market in allmarketsdata:
             normalized_market = {
                 "market_address": market[0],
                 "asset": market[1].decode('utf-8').strip("\x00"),
-                "key": market[2].decode('utf-8').strip("\x00"),
+                "key": market[2],
                 "maxLeverage": market[3],
                 "price": market[4],
                 "marketSize": market[5],
                 "marketSkew": market[6],
                 "marketDebt": market[7],
                 "currentFundingRate": market[8],
                 "currentFundingVelocity": market[9],
@@ -105,27 +134,38 @@
             addresses['sUSD'][self.network_id]), abi=abis['sUSD'])
 
         return markets, market_contracts, susd_token
 
     def _get_tx_params(
         self, value=0, to=None
     ) -> TxParams:
-        """Get generic transaction parameters."""
+        """
+        Get the default tx params
+        ...
+
+        Attributes
+        ----------
+        value : int
+            value to send in wei
+        to : str
+            address to send to
+
+        Returns
+        -------
+        params : dict
+            transaction parameters to be completed with another function
+        """
         params: TxParams = {
             'from': self.wallet_address,
             'to': to,
             'chainId': self.network_id,
             'value': value,
-            'gas': 1500000,
-            'gasPrice': self.web3.to_wei(
-                '0.4',
-                'gwei'),
-            'nonce': self.web3.eth.get_transaction_count(self.wallet_address)
+            'gasPrice': self.web3.eth.gas_price,
+            'nonce': self.nonce
         }
-
         return params
 
     def get_market_contract(self, token_symbol: str):
         """
         Run checks and return market contract if it exists
         ...
 
@@ -149,33 +189,56 @@
         tx_data : dict
             tx data to send transaction
         private_key : str
             private key of wallet sending transaction
         """
         if self.private_key is None:
             raise Exception("No private key specified.")
+
+        if "gas" not in tx_data:
+            if self.use_estimate_gas:
+                tx_data["gas"] = int(self.web3.eth.estimate_gas(tx_data) * 1.2)
+            else:
+                tx_data["gas"] = 1500000
+
         signed_txn = self.web3.eth.account.sign_transaction(
             tx_data, private_key=self.private_key)
         tx_token = self.web3.eth.send_raw_transaction(
             signed_txn.rawTransaction)
+
+        # increase nonce
+        self.nonce += 1
+
         return self.web3.to_hex(tx_token)
 
-    def check_delayed_orders(self, token_symbol: str) -> bool:
+    def check_delayed_orders(self, token_symbol: str, wallet_address: str = None) -> dict:
         """
         Check if delayed order is in queue
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
+        wallet_address : str
+            wallet address to check for delayed order
         """
+        if not wallet_address:
+            wallet_address = self.wallet_address
         market_contract = self.market_contracts[token_symbol]
-        return (market_contract.functions.delayedOrders(
-            self.wallet_address).call())[0]
+        delayed_order = market_contract.functions.delayedOrders(
+            wallet_address).call()
+
+        return {
+            'is_open': True if delayed_order[2] > 0 else False,
+            'size_delta': delayed_order[1],
+            'desired_fill_price': delayed_order[2],
+            'intention_time': int(delayed_order[7]),
+            'executable_time': int(delayed_order[7]) + 15 if int(delayed_order[7]) > 0 else 0,
+        }
 
     def get_current_asset_price(self, token_symbol: str) -> dict:
         """
         Gets current asset price for config asset.
         ...
 
         Attributes
@@ -188,30 +251,33 @@
         Dict with wei and USD price
         """
         market_contract = self.market_contracts[token_symbol.upper()]
         wei_price = (market_contract.functions.assetPrice().call())[0]
         usd_price = self.web3.from_wei(wei_price, 'ether')
         return {"usd": usd_price, "wei": wei_price}
 
-    def get_current_position(self, token_symbol: str) -> dict:
+    def get_current_position(self, token_symbol: str, wallet_address: str = None) -> dict:
         """
         Gets Current Position Data
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
         Returns
         ----------
         Dict: position information
         """
+        if not wallet_address:
+            wallet_address = self.wallet_address
+
         market_contract = self.get_market_contract(token_symbol)
         id, last_funding_index, margin, last_price, size = market_contract.functions.positions(
-            self.wallet_address).call()
+            wallet_address).call()
         current_asset_price = self.get_current_asset_price(token_symbol)
 
         # clean usd values
         is_short = -1 if size < 0 else 1
         size_ether = self.web3.from_wei(abs(size), 'ether') * is_short
         last_price_usd = self.web3.from_wei(last_price, 'ether')
 
@@ -246,35 +312,153 @@
         market_contract = self.get_market_contract(token_symbol)
         margin_allowed = (market_contract.functions.accessibleMargin(
             self.wallet_address).call())[0]
         margin_usd = self.web3.from_wei(margin_allowed, 'ether')
         return {"margin_remaining": margin_allowed,
                 "margin_remaining_usd": margin_usd}
 
-    def can_liquidate(self, token_symbol: str) -> dict:
+    def can_liquidate(self, token_symbol: str, wallet_address: str = None) -> dict:
         """
         Checks if Liquidation is possible for wallet
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
         Returns
         ----------
         Dict: Liquidation Data
         """
+        if not wallet_address:
+            wallet_address = self.wallet_address
         market_contract = self.get_market_contract(token_symbol)
         liquidation_check = market_contract.functions.canLiquidate(
-            self.wallet_address).call()
+            wallet_address).call()
         liquidation_price = market_contract.functions.liquidationPrice(
-            self.wallet_address).call()
+            wallet_address).call()
         return {"liq_possible": liquidation_check,
                 "liq_price": liquidation_price}
 
+    def liquidate_position(self, token_symbol: str, wallet_address: str=None,skip_check:bool=False, execute_now: bool = False) -> dict:
+        """
+        Checks if Liquidation is possible for wallet
+        ...
+
+        Attributes
+        ----------
+        token_symbol : str
+            token symbol from list of supported asset
+        wallet_address : str
+            Wallet address to liquidate
+        Returns
+        ----------
+        Dict: Liquidation of position
+        """
+        if not wallet_address:
+            wallet_address = self.wallet_address
+        market_contract = self.get_market_contract(token_symbol)
+        if skip_check:
+            data_tx = market_contract.encodeABI(
+                fn_name='liquidatePosition', args=[wallet_address])
+            tx_params = self._get_tx_params(
+                to=market_contract.address)
+            tx_params['data'] = data_tx
+            if execute_now:
+                tx_token = self.execute_transaction(tx_params)
+                print(f"Executing Liquidation for {token_symbol}")
+                print(f"TX: {tx_token}")
+                time.sleep(1)
+                return tx_token
+            else:
+                return {
+                    "token": token_symbol.upper(),
+                    "tx_data": tx_params}
+        liquidation_check = market_contract.functions.canLiquidate(
+            self.wallet_address).call()
+        # check for if liquidation is possible
+        if liquidation_check == True:
+            data_tx = market_contract.encodeABI(
+                fn_name='liquidatePosition', args=[wallet_address])
+            tx_params = self._get_tx_params(
+                to=market_contract.address)
+            tx_params['data'] = data_tx
+            if execute_now:
+                tx_token = self.execute_transaction(tx_params)
+                print(f"Executing Liquidation for {token_symbol}")
+                print(f"TX: {tx_token}")
+                time.sleep(1)
+                return tx_token
+            else:
+                return {
+                    "token": token_symbol.upper(),
+                    "tx_data": tx_params}
+        else:
+            return {
+                "token": token_symbol.upper(),
+                "tx_data": "N/A, Cannot Liquidate Position."}
+
+    def flag_position(self, token_symbol: str, wallet_address: str=None,skip_check:bool=False, execute_now: bool = False) -> dict:
+        """
+        Checks if Liquidation is possible for wallet
+        ...
+
+        Attributes
+        ----------
+        token_symbol : str
+            token symbol from list of supported asset
+        wallet_address : str
+            Wallet address to flag for liquidation
+        Returns
+        ----------
+        Dict: flag Liquidation of position
+        """
+        if not wallet_address:
+            wallet_address = self.wallet_address
+        market_contract = self.get_market_contract(token_symbol)
+        if skip_check:
+            data_tx = market_contract.encodeABI(
+                fn_name='flagPosition', args=[wallet_address])
+            tx_params = self._get_tx_params(
+                to=market_contract.address)
+            tx_params['data'] = data_tx
+            if execute_now:
+                tx_token = self.execute_transaction(tx_params)
+                print(f"Executing Flag for {token_symbol}")
+                print(f"TX: {tx_token}")
+                time.sleep(1)
+                return tx_token
+            else:
+                return {
+                    "token": token_symbol.upper(),
+                    "tx_data": tx_params}
+        liquidation_check = market_contract.functions.canLiquidate(
+            self.wallet_address).call()
+        # check for if liquidation is possible
+        if liquidation_check == True:
+            data_tx = market_contract.encodeABI(
+                fn_name='flagPosition', args=[wallet_address])
+            tx_params = self._get_tx_params(
+                to=market_contract.address)
+            tx_params['data'] = data_tx
+            if execute_now:
+                tx_token = self.execute_transaction(tx_params)
+                print(f"Executing Flag for {token_symbol}")
+                print(f"TX: {tx_token}")
+                time.sleep(1)
+                return tx_token
+            else:
+                return {
+                    "token": token_symbol.upper(),
+                    "tx_data": tx_params}
+        else:
+            return {
+                "token": token_symbol.upper(),
+                "tx_data": "N/A, Cannot Flag Position."}
+
     def get_market_skew(self, token_symbol: str) -> dict:
         """
         Gets current market long/short market skew
         ...
 
         Attributes
         ----------
@@ -390,42 +574,45 @@
                 to=market_contract.address, value=0)
             tx_params['data'] = data_tx
 
             if execute_now:
                 tx_token = self.execute_transaction(tx_params)
                 print(f"Updating Position by {token_amount}")
                 print(f"TX: {tx_token}")
-                time.sleep(1)
                 return tx_token
             else:
                 return {"token": token_symbol.upper(),
                         'token_amount': token_amount / (10**18),
                         "susd_balance": susd_balance,
                         "tx_data": tx_params}
 
     def modify_position(
             self,
             token_symbol: str,
             size_delta: float,
             slippage: float = DEFAULT_SLIPPAGE,
-            execute_now: bool = False) -> str:
+            execute_now: bool = False,
+            self_execute: bool = False) -> str:
         """
         Submits a delayed offchain order with a size of `size_delta`
         ...
 
         Attributes
         ----------
         size_delta : float
             Position amount *in human readable* as trade asset i.e. 12 SOL == 12*(10**18). Exact position in a direction, with negative values representing short orders.
         token_symbol : str
             token symbol from list of supported asset
         wallet_address : str
             wallet_address of wallet to check
         slippage : float
             slippage percentage
+        self_execute : bool
+            If True, wait until the order is executable and execute it
+
         Returns
         ----------
         str: token transfer Tx id
         """
         is_short = -1 if size_delta < 0 else 1
         market_contract = self.get_market_contract(token_symbol)
         size_delta = self.web3.to_wei(abs(size_delta), 'ether') * is_short
@@ -444,37 +631,42 @@
         tx_params = self._get_tx_params(to=market_contract.address, value=0)
         tx_params['data'] = data_tx
 
         print(f"Updating Position by {size_delta}")
         if execute_now:
             tx_token = self.execute_transaction(tx_params)
             print(f"TX: {tx_token}")
-            time.sleep(1)
+
+            if self_execute:
+                self._wait_and_execute(tx_token, token_symbol)
             return tx_token
         else:
             return {
                 "token": token_symbol.upper(),
                 'current_position': current_position['size'],
                 "tx_data": tx_params}
 
     def close_position(
             self,
             token_symbol: str,
             slippage: float = DEFAULT_SLIPPAGE,
-            execute_now: bool = False) -> str:
+            execute_now: bool = False,
+            self_execute: bool = False) -> str:
         """
         Fully closes account position
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
         slippage : float
             slippage percentage
+        self_execute : bool
+            If True, wait until the order is executable and execute it
 
         Returns
         ----------
         str: token transfer Tx id
         """
         market_contract = self.get_market_contract(token_symbol)
         current_position = self.get_current_position(token_symbol)
@@ -496,30 +688,33 @@
         tx_params = self._get_tx_params(to=market_contract.address, value=0)
         tx_params['data'] = data_tx
 
         if execute_now:
             tx_token = self.execute_transaction(tx_params)
             print(f"Closing Position by {-current_position['size']}")
             print(f"TX: {tx_token}")
-            time.sleep(1)
+            if self_execute:
+                self._wait_and_execute(tx_token, token_symbol)
+
             return tx_token
         else:
             return {
                 "token": token_symbol.upper(),
                 'current_position': current_position['size'],
                 "tx_data": tx_params}
 
     def open_position(
             self,
             token_symbol: str,
             short: bool = False,
             size_delta: float = None,
             slippage: float = DEFAULT_SLIPPAGE,
             leverage_multiplier: float = None,
-            execute_now: bool = False) -> str:
+            execute_now: bool = False,
+            self_execute: bool = False) -> str:
         """
         Open account position in a direction
         ...
 
         Attributes
         ----------
         token_symbol : str
@@ -528,26 +723,28 @@
             set to True when creating a short. (Implemented to double check side)
         size_delta : int, optional
             position amount in human readable format as trade asset i.e. 12 SOL. Exact position in a direction (Sign this It WILL MATTER).
         leverage_multiplier :
             Multiplier of Leverage to use when creating order. Based on available margin in account.
         slippage : float
             slippage percentage
+        self_execute : bool
+            If True, wait until the order is executable and execute it
 
         *Use either size_delta or leverage_multiplier.
 
         Returns
         ----------
         str: token transfer Tx id
         """
         if (size_delta is None) and (leverage_multiplier is None):
-            print("Enter EITHER a position amount or a leverage multiplier!")
+            print("Enter EITHER a size_delta or a leverage_multiplier!")
             return None
         elif (size_delta is not None) and (leverage_multiplier is not None):
-            print("Enter EITHER a position amount or a leverage multiplier!")
+            print("Enter EITHER a size_delta or a leverage_multiplier!")
             return None
 
         market_contract = self.get_market_contract(token_symbol)
         current_position = self.get_current_position(token_symbol)
         current_price = self.get_current_asset_price(token_symbol)
 
         # starting at zero otherwise use Update position
@@ -588,24 +785,236 @@
                 to=market_contract.address, value=0)
             tx_params['data'] = data_tx
 
             if execute_now:
                 tx_token = self.execute_transaction(tx_params)
                 print(f"Updating Position by {size_delta}")
                 print(f"TX: {tx_token}")
-                time.sleep(1)
+                if self_execute:
+                    self._wait_and_execute(tx_token, token_symbol)
                 return tx_token
             else:
                 return {"token": token_symbol.upper(),
                         'position_size': size_delta / (10**18),
                         'current_position': current_position['size'],
                         "max_leverage": max_leverage / (10**18),
                         "leveraged_percent": (size_delta / max_leverage) * 100,
                         "tx_data": tx_params}
-        return 'some'
+
+    def cancel_order(
+            self,
+            token_symbol: str,
+            account: str = None,
+            execute_now: bool = False) -> str:
+        """
+        Cancels an open order
+        ...
+
+        Attributes
+        ----------
+        account : str
+            address of the account to cancel. (defaults to connected wallet)
+        token_symbol : str
+            token symbol from list of supported asset
+
+        Returns
+        ----------
+        str: transaction hash for closing the order
+        """
+        market_contract = self.get_market_contract(token_symbol)
+        delayed_order = self.check_delayed_orders(token_symbol)
+
+        if account is None:
+            account = self.wallet_address
+
+        if not delayed_order['is_open']:
+            print("No open order")
+            return None
+
+        data_tx = market_contract.encodeABI(
+            fn_name='cancelOffchainDelayedOrder', args=[self.wallet_address])
+
+        tx_params = self._get_tx_params(to=market_contract.address, value=0)
+        tx_params['data'] = data_tx
+
+        if execute_now:
+            tx_token = self.execute_transaction(tx_params)
+            print(f"Cancelling order for {token_symbol}")
+            print(f"TX: {tx_token}")
+            return tx_token
+        else:
+            return {
+                "token": token_symbol.upper(),
+                "tx_data": tx_params}
+
+    def execute_order(
+            self,
+            token_symbol: str,
+            account: str = None,
+            execute_now: bool = False,
+            estimate_gas: bool = False) -> str:
+        """
+        Executes an open order
+        ...
+
+        Attributes
+        ----------
+        account : str
+            address of the account to execute. (defaults to connected wallet)
+        token_symbol : str
+            token symbol from list of supported asset
+
+        Returns
+        ----------
+        str: transaction hash for executing the order
+        """
+        if not account:
+            account = self.wallet_address
+
+        market_contract = self.get_market_contract(token_symbol)
+        delayed_order = self.check_delayed_orders(token_symbol, account)
+
+        if not delayed_order['is_open']:
+            print("No open order")
+            return None
+
+        # get price update data
+        price_update_data = self.pyth.price_update_data(token_symbol)
+
+        if not price_update_data:
+            raise Exception(
+                "Failed to get price update data from price service")
+
+        data_tx = market_contract.encodeABI(
+            fn_name='executeOffchainDelayedOrder', args=[account, [price_update_data]])
+
+        tx_params = self._get_tx_params(to=market_contract.address, value=1)
+        tx_params['data'] = data_tx
+
+        if execute_now:
+            tx_token = self.execute_transaction(tx_params)
+            print(f"Executing order for {token_symbol}")
+            print(f"TX: {tx_token}")
+            return tx_token
+        elif estimate_gas:
+            try:
+                gas_estimate = self.web3.eth.estimate_gas(tx_params)
+                return gas_estimate
+            except Exception as e:
+                print(f'Error estimating gas: {e}')
+                return None
+        else:
+            return {
+                "token": token_symbol.upper(),
+                "tx_data": tx_params}
+
+    async def _wait_and_execute(self, tx, token_symbol, retries=3, retry_interval=1):
+        """
+        Wait for a transaction receipt and execute the order when executable
+        ...
+
+        Attributes
+        ----------
+        tx: str
+            Transaction hash for the order that was submitted
+        token_symbol : str
+            token symbol from list of supported asset
+
+        Returns
+        ----------
+        str: token transfer Tx id
+        """
+        # wait for receipt
+        self.web3.eth.wait_for_transaction_receipt(tx)
+
+        # get delayed order
+        delayed_order = self.check_delayed_orders(token_symbol)
+
+        # wait until executable
+        print('Waiting until order is executable')
+        time.sleep(delayed_order['executable_time'] - time.time())
+
+        # set up the estimate
+        gas_estimate = None
+        attempt = 0
+
+        # Retry gas estimation multiple times
+        while attempt < retries:
+            gas_estimate = self.execute_order(token_symbol, estimate_gas=True)
+
+            if gas_estimate is not None:
+                break
+
+            print(
+                f'Gas estimation failed, retrying in {retry_interval} seconds...')
+            time.sleep(retry_interval)
+            attempt += 1
+
+        # If gas estimation is successful, execute the order
+        if gas_estimate:
+            print(f'Gas estimate for executing order: {gas_estimate}')
+            tx_execute = self.execute_order(token_symbol, execute_now=True)
+            print(f'Executing tx: {tx_execute}')
+        else:
+            print(
+                'Gas estimation failed after multiple retries, not executing the order.')
+
+    async def execute_for_address(self, token_symbol, wallet_address, retries=5, retry_interval=1):
+        """
+        Check an addresses delayed orders and execute the order when executable
+        ...
+
+        Attributes
+        ----------
+        token_symbol : str
+            token symbol from list of supported asset
+        wallet_address: str
+            Transaction hash for the order that was submitted
+        """
+        if not wallet_address:
+            wallet_address = self.wallet_address
+
+        # check delayed orders
+        delayed_order = self.check_delayed_orders(token_symbol, wallet_address)
+
+        # if no order, exit
+        if not delayed_order['is_open']:
+            print("No delayed order open")
+            return
+
+        # wait until executable
+        print('Waiting until order is executable')
+        await asyncio.sleep(delayed_order['executable_time'] - time.time())
+
+        # set up the estimate
+        gas_estimate = None
+        attempt = 0
+
+        # Retry gas estimation multiple times
+        while attempt < retries:
+            gas_estimate = self.execute_order(
+                token_symbol, account=wallet_address, estimate_gas=True)
+
+            if gas_estimate is not None:
+                break
+
+            print(
+                f'Gas estimation failed, retrying in {retry_interval} seconds...')
+            await asyncio.sleep(retry_interval)
+            attempt += 1
+
+        # If gas estimation is successful, execute the order
+        if gas_estimate:
+            print(f'Gas estimate for executing order: {gas_estimate}')
+            tx_execute = self.execute_order(
+                token_symbol, account=wallet_address, execute_now=True)
+            print(f'Executing tx: {tx_execute}')
+        else:
+            print(
+                'Gas estimation failed after multiple retries, not executing the order.')
 
     def open_limit(
             self,
             token_symbol: str,
             limit_price: float,
             size_delta: float = None,
             leverage_multiplier: float = None,
```

### Comparing `kwenta-1.0.2/kwenta.egg-info/PKG-INFO` & `kwenta-1.0.3/kwenta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.2/setup.py` & `kwenta-1.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from setuptools import setup, find_packages
 setup(
     name='kwenta',
-    version='1.0.2',
+    version='1.0.3',
     description='Python SDK for Kwenta',
     long_description='Python SDK for Kwenta',
     author='Kwenta DAO',
     packages=['kwenta'],
     install_requires=[
         "numpy",
         "pandas",
         "requests",
         "web3>=6.0.0",
+        "gql"
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     python_requires=">=3.8",
     package_data={"kwenta": ["json/*"]},
     include_package_data=True,
+    entry_points={
+        'console_scripts': [
+            'kwenta = kwenta.cli.kwenta_cli:kwenta_cli',
+        ],
+    },
 )
```

