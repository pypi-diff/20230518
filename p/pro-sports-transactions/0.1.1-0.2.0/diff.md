# Comparing `tmp/pro_sports_transactions-0.1.1.tar.gz` & `tmp/pro_sports_transactions-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pro_sports_transactions-0.1.1.tar", max compression
+gzip compressed data, was "pro_sports_transactions-0.2.0.tar", max compression
```

## Comparing `pro_sports_transactions-0.1.1.tar` & `pro_sports_transactions-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-05-14 17:50:23.756712 pro_sports_transactions-0.1.1/LICENSE
--rw-r--r--   0        0        0     5067 2023-05-14 18:01:22.107791 pro_sports_transactions-0.1.1/README.md
--rw-r--r--   0        0        0     1372 2023-05-14 18:03:14.633992 pro_sports_transactions-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      105 2023-05-14 17:50:23.884787 pro_sports_transactions-0.1.1/src/pro_sports_transactions/__init__.py
--rw-r--r--   0        0        0     5149 2023-05-14 17:57:59.206254 pro_sports_transactions-0.1.1/src/pro_sports_transactions/search.py
--rw-r--r--   0        0        0     6449 1970-01-01 00:00:00.000000 pro_sports_transactions-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-14 17:50:23.756712 pro_sports_transactions-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5066 2023-05-18 21:02:37.352728 pro_sports_transactions-0.2.0/README.md
+-rw-r--r--   0        0        0     1396 2023-05-18 21:04:24.747503 pro_sports_transactions-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-05-18 21:02:37.390633 pro_sports_transactions-0.2.0/src/pro_sports_transactions/__init__.py
+-rw-r--r--   0        0        0     5399 2023-05-18 21:02:37.417001 pro_sports_transactions-0.2.0/src/pro_sports_transactions/search.py
+-rw-r--r--   0        0        0     6448 1970-01-01 00:00:00.000000 pro_sports_transactions-0.2.0/PKG-INFO
```

### Comparing `pro_sports_transactions-0.1.1/LICENSE` & `pro_sports_transactions-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pro_sports_transactions-0.1.1/README.md` & `pro_sports_transactions-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # League (MLB, MLS, NBA, NFL, and NHL)
 league = pst.League.NBA
 
 # Disciplinary Actions, Injured List, Injuries,
 # Legal Incidents, Minor League To/For, Personal Reasons,
 # and General (e.g., Trades, Acquisitions, Waivers, Draft Picks, etc.)
-transaction_types = tuple([t for t in pst.TransactionTypes])
+transaction_types = tuple([t for t in pst.TransactionType])
 
 # From the start of the 2022-23 NBA Regular Season
 start_date = date.fromisoformat("2022-10-18")
 
 # From the end of the 2022-23 NBA Regular Season
 end_date = date.fromisoformat("2023-04-09")
```

### Comparing `pro_sports_transactions-0.1.1/pyproject.toml` & `pro_sports_transactions-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pro_sports_transactions"
-version = "0.1.1"
+version = "0.2.0"
 description = "A Python Library for Consuming Transactions from Pro Sports Transactions (https://www.prosportstransactions.com)"
 license = "MIT"
 authors = ["Randy Forbes <randy.forbes@gmail.com>"]
 readme = "README.md"
 maintainers = ["Randy Forbes <randy.forbes@gmail.com>"]
 repository = "https://github.com/rsforbes/pro_sports_transactions"
 documentation = "https://github.com/rsforbes/pro_sports_transactions/blob/main/README.md"
@@ -27,14 +27,15 @@
 bs4 = "^0.0.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
+pytest-mock = "^3.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = [
```

### Comparing `pro_sports_transactions-0.1.1/src/pro_sports_transactions/search.py` & `pro_sports_transactions-0.2.0/src/pro_sports_transactions/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import date
 from enum import Enum, StrEnum
-from pandas import read_html
+from pandas import DataFrame, read_html
 from typing import Dict
 from urllib import parse
 import aiohttp
 import json
 import pandas as pd
 
 
@@ -12,36 +12,36 @@
     MLB = "baseball"
     NBA = "basketball"
     NFL = "football"
     NHL = "hockey"
     MLS = "soccer"
 
 
-class TransactionTypes(Enum):
-    DisciplinaryActions = {"default": "DisciplinaryChkBx"}
+class TransactionType(Enum):
+    Disciplinary = {"default": "DisciplinaryChkBx"}
     InjuredList = {"default": "ILChkBx", "MLB": "DLChkBx"}
-    Injuries = {"default": "InjuriesChkBx"}
-    LegalIncidents = {"default": "LegalChkBx"}
+    Injury = {"default": "InjuriesChkBx"}
+    LegalIncident = {"default": "LegalChkBx"}
     MinorLeagueToFrom = {"default": "NBADLChkBx", "MLB": "MinorsChkBx"}
     General = {"default": "PlayerMovementChkBx"}
-    PersonalReasons = {"default": "PersonalChkBx"}
+    PersonalReason = {"default": "PersonalChkBx"}
 
     def __getitem__(cls, value):
         if type(value) == League:
             name = value.name
             return cls.value[name] if name in cls.value else cls.value["default"]
         else:
             return cls.value
 
 
 class Search:
     def __init__(
         self,
         league: League = League.NBA,
-        transaction_types: TransactionTypes = (),
+        transaction_types: TransactionType = (),
         start_date: date = date.today(),
         end_date: date = date.today(),
         player: str = None,
         team: str = None,
         starting_row: int = 0,
     ):
         self._url = UrlBuilder.build(
@@ -50,31 +50,40 @@
             start_date=start_date,
             end_date=end_date,
             player=player,
             team=team,
             starting_row=starting_row,
         )
 
-    async def _search(self) -> list:
+    async def _get_dataframe(self) -> DataFrame:
+        # Generic DataFrame to hold results
         response = await Http.get(self._url)
-        return read_html(response, header=0, keep_default_na=False)
 
-    async def get_dataframe(self):
-        data = await self._search()
-        df = pd.DataFrame(data[0], columns=["Date", "Team", "Acquired", "Relinquished", "Notes"])
-        df.attrs["pages"] = data[1].columns[2].split(" ")[-1]
+        df = None
+        try:
+            df_list = read_html(response, header=0, keep_default_na=False)
+            df = pd.DataFrame(
+                df_list[0], columns=["Date", "Team", "Acquired", "Relinquished", "Notes"]
+            )
+            df.attrs["pages"] = int(df_list[1].columns[2].split(" ")[-1])
+        except Exception as e:
+            df = pd.DataFrame(columns=["Date", "Team", "Acquired", "Relinquished", "Notes"])
+            df.attrs["pages"] = 0
+            df.attrs["errors"] = (repr(e),)
+
         return df
 
     async def get_dict(self):
-        results = await self._search()
+        df = await self._get_dataframe()
 
         data = {}
-        data["transactions"] = results[0].to_dict(orient="records")
-        data["pages"] = int(results[1].columns[2].split(" ")[-1])
-
+        data["transactions"] = df.to_dict(orient="records")
+        data["pages"] = df.attrs["pages"]
+        if "errors" in df.attrs:
+            data["errors"] = df.attrs["errors"]
         return data
 
     async def get_json(self):
         return json.dumps(await self.get_dict())
 
     async def get_url(self):
         return self._url
@@ -97,20 +106,15 @@
     ),
 }
 
 
 class Parameter:
     @staticmethod
     def date_param(key: str, value: date) -> Dict:
-        iso8601 = ""
-
-        if value is not None and type(value) == date:
-            iso8601 = value.strftime("%Y-%m-%d")
-
-        return {key: iso8601}
+        return {key: value.strftime("%Y-%m-%d") if type(value) == date else ""}
 
     @staticmethod
     def transaction_type(param_name) -> Dict:
         return {param_name: "yes"}
 
     @staticmethod
     def start_date(start_date: date) -> Dict:
@@ -154,15 +158,15 @@
         params |= Parameter.player(player)
         params |= Parameter.team(team)
         params |= Parameter.starting_row(starting_row)
         params |= Parameter.submit()
 
         # Add all Transaction Type parameter values
         for transaction_type in transaction_types:
-            params |= Parameter.transaction_type(TransactionTypes[transaction_type.name][league])
+            params |= Parameter.transaction_type(TransactionType[transaction_type.name][league])
 
         return f"{netloc}/{league.value}/{path}?{parse.urlencode(params)}"
 
 
 class Http:
     @staticmethod
     async def get(url):
```

### Comparing `pro_sports_transactions-0.1.1/PKG-INFO` & `pro_sports_transactions-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pro-sports-transactions
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python Library for Consuming Transactions from Pro Sports Transactions (https://www.prosportstransactions.com)
 Home-page: https://github.com/rsforbes/pro_sports_transactions
 License: MIT
 Keywords: api,data science,basketball,prosports,prosportstransactions,pro sports,pro sports transactions,trades,draft,transactions,injuries,fines,data,nba,mlb,mls,nfl,nhl,sports,stats
 Author: Randy Forbes
 Author-email: randy.forbes@gmail.com
 Maintainer: Randy Forbes
@@ -50,15 +50,15 @@
 
 # League (MLB, MLS, NBA, NFL, and NHL)
 league = pst.League.NBA
 
 # Disciplinary Actions, Injured List, Injuries,
 # Legal Incidents, Minor League To/For, Personal Reasons,
 # and General (e.g., Trades, Acquisitions, Waivers, Draft Picks, etc.)
-transaction_types = tuple([t for t in pst.TransactionTypes])
+transaction_types = tuple([t for t in pst.TransactionType])
 
 # From the start of the 2022-23 NBA Regular Season
 start_date = date.fromisoformat("2022-10-18")
 
 # From the end of the 2022-23 NBA Regular Season
 end_date = date.fromisoformat("2023-04-09")
```

