# Comparing `tmp/quant_invest_lab-0.2.6.tar.gz` & `tmp/quant_invest_lab-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant_invest_lab-0.2.6.tar", max compression
+gzip compressed data, was "quant_invest_lab-0.2.7.tar", max compression
```

## Comparing `quant_invest_lab-0.2.6.tar` & `quant_invest_lab-0.2.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5026 2023-05-18 15:22:39.067069 quant_invest_lab-0.2.6/README.md
--rw-r--r--   0        0        0      978 2023-05-18 15:22:39.071069 quant_invest_lab-0.2.6/pyproject.toml
--rw-r--r--   0        0        0    32590 2023-05-18 15:22:39.071069 quant_invest_lab-0.2.6/quant_invest_lab/backtest.py
--rw-r--r--   0        0        0    17110 2023-05-18 15:22:39.071069 quant_invest_lab-0.2.6/quant_invest_lab/data_provider.py
--rw-r--r--   0        0        0    26301 2023-05-18 15:22:39.071069 quant_invest_lab-0.2.6/quant_invest_lab/indicators.py
--rw-r--r--   0        0        0     9477 2023-05-18 15:22:39.071069 quant_invest_lab-0.2.6/quant_invest_lab/metrics.py
--rw-r--r--   0        0        0     7659 2023-05-18 15:22:39.071069 quant_invest_lab-0.2.6/quant_invest_lab/optimization.py
--rw-r--r--   0        0        0    20461 2023-05-18 15:22:39.071069 quant_invest_lab-0.2.6/quant_invest_lab/portfolio.py
--rw-r--r--   0        0        0     3577 2023-05-18 15:22:39.071069 quant_invest_lab-0.2.6/quant_invest_lab/screener.py
--rw-r--r--   0        0        0     8477 2023-05-18 15:22:39.071069 quant_invest_lab-0.2.6/quant_invest_lab/simulation.py
--rw-r--r--   0        0        0     1107 2023-05-18 15:22:39.071069 quant_invest_lab-0.2.6/quant_invest_lab/utils.py
--rw-r--r--   0        0        0     6344 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     5020 2023-05-18 21:52:51.578303 quant_invest_lab-0.2.7/README.md
+-rw-r--r--   0        0        0     1543 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0    28604 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/backtest.py
+-rw-r--r--   0        0        0    17212 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/data_provider.py
+-rw-r--r--   0        0        0    26301 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/indicators.py
+-rw-r--r--   0        0        0    11102 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/metrics.py
+-rw-r--r--   0        0        0     7659 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/optimization.py
+-rw-r--r--   0        0        0    18363 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/portfolio.py
+-rw-r--r--   0        0        0     3577 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/screener.py
+-rw-r--r--   0        0        0     8477 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/simulation.py
+-rw-r--r--   0        0        0     3758 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/utils.py
+-rw-r--r--   0        0        0     6939 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.7/PKG-INFO
```

### Comparing `quant_invest_lab-0.2.6/README.md` & `quant_invest_lab-0.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 df_BTC = df_BTC.dropna()
 
 # Define your strategy entry and exit functions
 def buy_func(row: pd.Series, prev_row: pd.Series) -> bool:
     return True if row.EMA20 > row.EMA60 else False
 
-def sell_func(row: pd.Series, prev_row: pd.Series, trading_days: pd.Series) -> bool:
+def sell_func(row: pd.Series, prev_row: pd.Series, trading_days: int) -> bool:
     return True if row.EMA20 < row.EMA60 else False
 
 # Backtest your strategy
 ohlc_long_only_backtester(
     df=df_BTC,
     long_entry_function=buy_func,
     long_exit_function=sell_func,
```

#### html2text {}

```diff
@@ -29,17 +29,17 @@
 pd from quant_invest_lab.backtest import ohlc_long_only_backtester from
 quant_invest_lab.data_provider import download_crypto_historical_data symbol =
 "BTC-USDT" timeframe = "4hour" df_BTC = download_crypto_historical_data(symbol,
 timeframe) # Define your indicators df_BTC["EMA20"] = df_BTC.Close.ewm(20).mean
 () df_BTC["EMA60"] = df_BTC.Close.ewm(60).mean() df_BTC = df_BTC.dropna() #
 Define your strategy entry and exit functions def buy_func(row: pd.Series,
 prev_row: pd.Series) -> bool: return True if row.EMA20 > row.EMA60 else False
-def sell_func(row: pd.Series, prev_row: pd.Series, trading_days: pd.Series) -
-> bool: return True if row.EMA20 < row.EMA60 else False # Backtest your
-strategy ohlc_long_only_backtester( df=df_BTC, long_entry_function=buy_func,
+def sell_func(row: pd.Series, prev_row: pd.Series, trading_days: int) -> bool:
+return True if row.EMA20 < row.EMA60 else False # Backtest your strategy
+ohlc_long_only_backtester( df=df_BTC, long_entry_function=buy_func,
 long_exit_function=sell_func, timeframe=timeframe, initial_equity=1000, ) ```
 ## Optimize a portfolio (mean-variance) ```python from
 quant_invest_lab.portfolio import MonteCarloPortfolio, ConvexPortfolio,
 RiskParityPortfolio from quant_invest_lab.data_provider import
 build_multi_crypto_dataframe symbols = set( [ "BNB-USDT", "BTC-USDT", "NEAR-
 USDT", "ETH-USDT", "SOL-USDT", "EGLD-USDT", "ALGO-USDT", "FTM-USDT", "ADA-
 USDT", ] ) closes = build_multi_crypto_dataframe(symbols) returns =
```

### Comparing `quant_invest_lab-0.2.6/quant_invest_lab/backtest.py` & `quant_invest_lab-0.2.7/quant_invest_lab/backtest.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,115 +5,186 @@
 import numpy as np
 import plotly.graph_objects as go
 import plotly.figure_factory as ff
 from plotly.subplots import make_subplots
 from tqdm import tqdm
 
 from quant_invest_lab.metrics import (
+    cumulative_returns,
+    expectancy,
+    profit_factor,
     sharpe_ratio,
     calmar_ratio,
     sortino_ratio,
     max_drawdown,
     drawdown,
     kelly_criterion,
     value_at_risk,
     conditional_value_at_risk,
 )
+from quant_invest_lab.utils import timeframe_annualized
 
 
-def ohlc_long_only_backtester(
-    df: pd.DataFrame,
-    long_entry_function: Callable[[pd.Series, pd.Series], bool],
-    long_exit_function: Callable[[pd.Series, pd.Series, int], bool],
+def print_ohlc_backtest_report(
+    returns_df: pd.DataFrame,
+    trades_df: pd.DataFrame,
+    ohlcv_df: pd.DataFrame,
     timeframe: Literal[
         "1min",
         "2min",
         "5min",
         "15min",
         "30min",
         "1hour",
         "2hour",
         "4hour",
         "12hour",
         "1day",
     ],
+    initial_equity: Union[int, float] = 1000,
+) -> None:
+    good_trades = trades_df.loc[trades_df["trade_return"] > 0]
+    bad_trades = trades_df.loc[trades_df["trade_return"] < 0]
+    total_trades = len(trades_df)
+    print(f"\n{'  Strategy performances  ':-^50}")
+
+    print(
+        f'Strategy final net balance: {returns_df["Cum_Returns"].iloc[-1]*initial_equity:.2f} $, return: {(returns_df["Cum_Returns"].iloc[-1]-1)*100:.2f} %'
+    )
+    print(
+        f'Buy & Hold final net balance: {ohlcv_df["Cum_Returns"].iloc[-1]*initial_equity:.2f} $, returns: {(ohlcv_df["Cum_Returns"].iloc[-1]-1)*100:.2f} %'
+    )
+    print(f"Strategy winrate ratio: {100 * len(good_trades) / total_trades:.2f} %")
+    print(
+        f"Strategy profit factor ratio: {profit_factor(good_trades['trade_return'].mean(),bad_trades['trade_return'].mean()):.2f}"
+    )
+    print(
+        f"Strategy expectancy: {100*expectancy(len(good_trades) / total_trades,good_trades['trade_return'].mean(),bad_trades['trade_return'].mean()):.2f} %"
+    )
+
+    print(f"\n{'  Returns statistical information  ':-^50}")
+
+    print(
+        f"Expected return : {100*returns_df['Returns'].mean():.2f} %, annuzalized: {100*returns_df['Returns'].mean()*timeframe_annualized[timeframe]:.2f} %"
+    )
+    print(
+        f"Median return : {100*returns_df['Returns'].median():.2f} %, annuzalized: {100*returns_df['Returns'].median()*timeframe_annualized[timeframe]:.2f} %"
+    )
+    print(
+        f'Expected volatility: {100*returns_df["Returns"].std():.2f} %, annualized: {100*returns_df["Returns"].std()*(timeframe_annualized[timeframe]**0.5):.2f} %'
+    )
+    print(
+        f"Skewness: {skew(returns_df.Returns.values):.2f} vs {skew(ohlcv_df.Returns.values):.2f} (buy and hold), <0 = left tail, >0 = right tail -> the higher the better"
+    )
+    print(
+        f"Kurtosis: {kurtosis(returns_df.Returns.values):.2f} vs {kurtosis(ohlcv_df.Returns.values):.2f} (buy and hold)",
+        ", >3 = fat tails, <3 = thin tails -> the lower the better",
+    )
+    print(
+        f"{timeframe}-95%-VaR: {100*value_at_risk(returns_df.Returns):.2f} % vs {100*value_at_risk(ohlcv_df.Returns):.2f} % (buy and hold) -> the lower the better"
+    )
+    print(
+        f"{timeframe}-95%-CVaR: {100*conditional_value_at_risk(returns_df.Returns):.2f} % vs {100*conditional_value_at_risk(ohlcv_df.Returns):.2f} % (buy and hold) -> the lower the better"
+    )
+
+    print(f"\n{'  Strategy statistical information  ':-^50}")
+    print(
+        f"Max drawdown: {100*max_drawdown(returns_df.Returns):.2f} % vs {100*max_drawdown(ohlcv_df.Returns):.2f} % (buy and hold)"
+    )
+    print(
+        f"Kelly criterion: {100*kelly_criterion(returns_df.Returns):.2f} % vs {100*kelly_criterion(ohlcv_df.Returns):.2f} % (buy and hold)"
+    )
+    print(
+        f"Sharpe ratio (annualized): {sharpe_ratio(returns_df['Returns'], timeframe_annualized[timeframe],risk_free_rate=timeframe_annualized[timeframe]*ohlcv_df.Returns.mean()):.2f} (risk free rate = buy and hold)"
+    )
+    print(
+        f"Sortino ratio (annualized): {sortino_ratio(returns_df['Returns'], timeframe_annualized[timeframe],risk_free_rate=timeframe_annualized[timeframe]*ohlcv_df.Returns.mean()):.2f} (risk free rate = buy and hold)"
+    )
+    print(
+        f"Calmar ratio (annualized): {calmar_ratio(returns_df['Returns'], timeframe_annualized[timeframe]):.2f} (risk free rate = buy and hold)"
+    )
+
+    print(f"\n{'  Trades informations  ':-^50}")
+    print(f"Mean trade return : {100*trades_df['trade_return'].mean():.2f} %")
+    print(f"Median trade return : {100*trades_df['trade_return'].median():.2f} %")
+    print(f'Mean trade volatility: {100*trades_df["trade_return"].std():.2f} %')
+    print(
+        f"Mean trade duration: {str((trades_df['trade_duration']).mean()).split('.')[0]}"
+    )
+
+    print(f"Total trades: {total_trades}")
+
+    print(f"\n  Total good trades: {len(good_trades)}")
+    print(f"  Mean good trades return: {100*good_trades['trade_return'].mean():.2f} %")
+    print(
+        f"  Median good trades return: {100*good_trades['trade_return'].median():.2f} %"
+    )
+    print(
+        f"  Best trades return: {100*trades_df['trade_return'].max():.2f} % | Date: {trades_df.iloc[trades_df['trade_return'].idxmax()]['exit_date']} | Duration: {trades_df.iloc[trades_df['trade_return'].idxmax()]['trade_duration']}"
+    )
+    print(
+        f"  Mean good trade duration: {str((good_trades['trade_duration']).mean()).split('.')[0]}"
+    )
+    print(f"\n  Total bad trades: {len(bad_trades)}")
+    print(f"  Mean bad trades return: {100*bad_trades['trade_return'].mean():.2f} %")
+    print(
+        f"  Median bad trades return: {100*bad_trades['trade_return'].median():.2f} %"
+    )
+    print(
+        f"  Worst trades return: {100*trades_df['trade_return'].min():.2f} % | Date: {trades_df.iloc[trades_df['trade_return'].idxmin()]['exit_date']} | Duration: {trades_df.iloc[trades_df['trade_return'].idxmin()]['trade_duration']}"
+    )
+    print(
+        f"  Mean bad trade duration: {str((bad_trades['trade_duration']).mean()).split('.')[0]}"
+    )
+
+    print(f"\nExit reasons repartition: ")
+    for reason, val in zip(
+        trades_df.exit_reason.value_counts().index, trades_df.exit_reason.value_counts()
+    ):
+        print(f"- {reason}: {val}")
+
+
+def __ohlc_backtest_one_position_type(
+    ohlcv_df: pd.DataFrame,
+    entry_function: Callable[[pd.Series, pd.Series], bool],
+    exit_function: Callable[[pd.Series, pd.Series, int], bool],
+    position_type: Literal["long", "short"],
     take_profit: float = np.inf,
     stop_loss: float = np.inf,
-    initial_equity: int = 1000,
     maker_fees: Optional[float] = 0.001,
     taker_fees: Optional[float] = 0.001,
-    get_trade_df: bool = False,
-    get_returns_df: bool = False,
-    parameter_optimization: bool = False,
-    plot_result: bool = True,
-) -> Union[None, Union[float, Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]]]:
-    """Run a backtest with long only position on a OHLC dataset.
+) -> tuple[pd.DataFrame, pd.DataFrame]:
+    """Core backtesting function for OHLCV data. It iterate over the OHLCV records and run the entry and exit function when the conditions are satisfied.
+    WARNING this function shouldn't be used alone, use the long/short backtest function instead.
 
     Args:
     ----
-        df (pd.DataFrame): The dataframe containing the OHLC data.
+        ohlcv_df (pd.DataFrame): The dataframe containing the OHLC data.
 
-        long_entry_function (Callable[[pd.Series, pd.Series], bool]): The long entry function, it should take 2 arguments, the current row and the previous row and return True or False depending on your strategy.
+        entry_function (Callable[[pd.Series, pd.Series], bool]): The trade entry function, it should take 2 arguments, the current row and the previous row and return True or False depending on your strategy.
 
-        long_exit_function (Callable[[pd.Series, pd.Series, int], bool]): The long exit function, it should take 3 arguments, the current row, the previous row and the number of timeframe count since the last entry order, and return True or False depending on your strategy.
+        exit_function (Callable[[pd.Series, pd.Series, int], bool]): The long entry function, it should take 2 arguments, the current row and the previous row and return True or False depending on your strategy.
 
-        timeframe (Literal[ &quot;1min&quot;, &quot;2min&quot;, &quot;5min&quot;, &quot;15min&quot;, &quot;30min&quot;, &quot;1hour&quot;, &quot;2hour&quot;, &quot;4hour&quot;, &quot;12hour&quot;, &quot;1day&quot;, ]): The timeframe granularity of the dataframe.
+        position_type (Literal[&quot;long&quot;, &quot;short&quot;]): The position type, long or short.
 
         take_profit (float, optional): The percent of the buy price to add to create a stop order and take the profit associated. Defaults to np.inf.
 
         stop_loss (float, optional): The percent of the buy price to cut to create a stop order and stop the loss associated. Defaults to np.inf.
 
-        initial_equity (int, optional): The initial capital. Defaults to 1000.
-
         maker_fees (Optional[float], optional): The fees applied, here maker for limit orders (not yet implemented). Defaults to 0.001.
 
         taker_fees (Optional[float], optional): The fees applied, here taker for spot orders. Defaults to 0.001.
 
-        get_trade_df (bool, optional): Whether or not to return the trade dataframe (summary of trades) . Defaults to False.
-
-        get_returns_df (bool, optional): Whether or not to return the strategy returns dataframe. Defaults to False.
-
-        parameter_optimization (bool, optional): This parameter is useful when running fitting/optimization it prints nothing but the final strategy return. Defaults to False.
-
-        plot_result (bool, optional): Plot equity, price, drawdown, distribution of the strategy. Defaults to True.
-
     Returns:
     -----
-        Union[None, Union[float, Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]]]: Nothing or the strategy total return or the trade_df or the return_df or the trade_df and the return_df.
+        tuple[pd.DataFrame, pd.DataFrame]: It returns 2 dataframes, the first is the trades_df : trade summary dataframe and the second is the returns dataframe : returns_df.
     """
-    assert timeframe in [
-        "1min",
-        "2min",
-        "5min",
-        "15min",
-        "30min",
-        "1hour",
-        "2hour",
-        "4hour",
-        "12hour",
-        "1day",
-    ], "timeframe must be one of the following: 1min, 2min, 5min, 15min, 30min, 1hour, 2hour, 4hour, 12hour, 1day"
-    assert df.shape[0] > 1, "Dataframe must have at least 2 rows"
-    assert set({"Open", "High", "Low", "Close", "Returns"}).issubset(
-        df.columns
-    ), "Dataframe must have columns Open, High, Low, Close, Returns"
-    timeframe_annualized = {
-        "1min": int(365 * 24 / 1 * 60),
-        "2min": int(365 * 24 / 1 * 30),
-        "5min": int(365 * 24 / 1 * 12),
-        "15min": int(365 * 24 / 1 * 4),
-        "30min": int(365 * 24 / 1 * 2),
-        "1hour": int(365 * 24 / 1),
-        "2hour": int(365 * 24 / 2),
-        "4hour": int(365 * 24 / 4),
-        "12hour": int(365 * 24 / 12),
-        "1day": 365,
-    }
-    N = timeframe_annualized[timeframe]
-    ohlcv_df = df.copy()
+    assert position_type in ["long", "short"], "position_type must be long or short"
+
+    returns_signs = {"long": 1, "short": -1}
     previous_row = ohlcv_df.iloc[0]
     position_opened = False
     timeframe_count = 0
     current_trade: dict[str, float | datetime | int | str | pd.Timestamp] = {}
 
     trades_df = pd.DataFrame(
         columns=[
@@ -131,64 +202,96 @@
 
     for index, row in tqdm(
         ohlcv_df[1:].iterrows(),
         desc="Backtesting...",
         total=ohlcv_df.shape[0] - 1,
         leave=False,
     ):
-        if position_opened is False and long_entry_function(row, previous_row) is True:
+        if position_opened is False and entry_function(row, previous_row) is True:
             position_opened = True
             current_trade["entry_date"] = index
             current_trade["entry_price"] = row.Close
             current_trade["entry_reason"] = "Entry position triggered"
             timeframe_count = 1
             entry_price = row.Close
         elif (
-            position_opened is True
+            position_type == "long"
+            and position_opened is True
             and current_trade["entry_price"] * (1 + take_profit) <= row.High
+        ) or (
+            position_type == "short"
+            and position_opened is True
+            and current_trade["entry_price"] * (1 + stop_loss) <= row.High
         ):
             position_opened = False
             current_trade["exit_date"] = index
-            current_trade["exit_price"] = current_trade["entry_price"] * (
-                1 + take_profit
-            )
-            current_trade["exit_reason"] = "Take profit triggered"
 
-            rets = ohlcv_df.loc[
-                current_trade["entry_date"] : current_trade["exit_date"]
-            ].Returns
+            current_trade["exit_price"] = (
+                current_trade["entry_price"] * (1 + take_profit)
+                if position_type == "long"
+                else current_trade["entry_price"] * (1 + stop_loss)
+            )
+
+            current_trade["exit_reason"] = (
+                "Long take profit triggered"
+                if position_type == "long"
+                else "Short stop loss triggered"
+            )
+
+            rets = (
+                returns_signs[position_type]
+                * ohlcv_df.loc[
+                    current_trade["entry_date"] : current_trade["exit_date"]
+                ].Returns
+            )
             if isinstance(taker_fees, float) and taker_fees > 0:
                 rets.iloc[0] = rets.iloc[0] - taker_fees
                 rets.iloc[-1] = rets.iloc[-1] - taker_fees
+
             current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
 
             trades_df = pd.concat(
                 [trades_df, pd.DataFrame([current_trade])], ignore_index=True
             )
             returns_df = pd.concat(
                 [returns_df, pd.DataFrame({"Returns": rets.values}, index=rets.index)],
                 ignore_index=False,
             )
             timeframe_count = 0
 
             current_trade = {}
         elif (
-            position_opened is True
+            position_type == "long"
+            and position_opened is True
             and current_trade["entry_price"] * (1 - stop_loss) >= row.Low
+        ) or (
+            position_type == "short"
+            and position_opened is True
+            and current_trade["entry_price"] * (1 - take_profit) >= row.Low
         ):
             position_opened = False
             current_trade["exit_date"] = index
-            current_trade["exit_price"] = float(current_trade["entry_price"]) * (
-                1 - stop_loss
-            )
-            current_trade["exit_reason"] = "Stop loss triggered"
 
-            rets = ohlcv_df.loc[
-                current_trade["entry_date"] : current_trade["exit_date"]
-            ].Returns
+            current_trade["exit_price"] = (
+                current_trade["entry_price"] * (1 - stop_loss)
+                if position_type == "long"
+                else current_trade["entry_price"] * (1 - take_profit)
+            )
+            current_trade["exit_reason"] = (
+                "Long stop loss triggered"
+                if position_type == "long"
+                else "Short take profit triggered"
+            )
+
+            rets = (
+                returns_signs[position_type]
+                * ohlcv_df.loc[
+                    current_trade["entry_date"] : current_trade["exit_date"]
+                ].Returns
+            )
             if isinstance(taker_fees, float) and taker_fees > 0:
                 rets.iloc[0] = rets.iloc[0] - taker_fees
                 rets.iloc[-1] = rets.iloc[-1] - taker_fees
             current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
 
             trades_df = pd.concat(
                 [trades_df, pd.DataFrame([current_trade])], ignore_index=True
@@ -197,24 +300,27 @@
                 [returns_df, pd.DataFrame({"Returns": rets.values}, index=rets.index)],
                 ignore_index=False,
             )
             timeframe_count = 0
             current_trade = {}
         elif (
             position_opened is True
-            and long_exit_function(row, previous_row, timeframe_count) is True
+            and exit_function(row, previous_row, timeframe_count) is True
         ):
             position_opened = False
             current_trade["exit_date"] = index
             current_trade["exit_price"] = row.Close
             current_trade["exit_reason"] = "Exit position triggered"
 
-            rets = ohlcv_df.loc[
-                current_trade["entry_date"] : current_trade["exit_date"]
-            ].Returns
+            rets = (
+                returns_signs[position_type]
+                * ohlcv_df.loc[
+                    current_trade["entry_date"] : current_trade["exit_date"]
+                ].Returns
+            )
 
             if isinstance(taker_fees, float) and taker_fees > 0:
                 rets.iloc[0] = rets.iloc[0] - taker_fees
                 rets.iloc[-1] = rets.iloc[-1] - taker_fees
 
             current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
 
@@ -227,127 +333,138 @@
             )
             timeframe_count = 0
             current_trade = {}
         else:
             timeframe_count += 1
         previous_row = row
 
-    returns_df["Cum_Returns"] = (returns_df["Returns"] + 1).cumprod()
-    returns_df["Drawdown"] = drawdown(returns_df["Returns"])
-    ohlcv_df["Cum_Returns"] = (df["Returns"] + 1).cumprod()
-    ohlcv_df["Drawdown"] = drawdown(df["Returns"])
+    return trades_df, returns_df
+
+
+def ohlc_long_only_backtester(
+    df: pd.DataFrame,
+    long_entry_function: Callable[[pd.Series, pd.Series], bool],
+    long_exit_function: Callable[[pd.Series, pd.Series, int], bool],
+    timeframe: Literal[
+        "1min",
+        "2min",
+        "5min",
+        "15min",
+        "30min",
+        "1hour",
+        "2hour",
+        "4hour",
+        "12hour",
+        "1day",
+    ],
+    take_profit: float = np.inf,
+    stop_loss: float = np.inf,
+    initial_equity: int = 1000,
+    maker_fees: Optional[float] = 0.001,
+    taker_fees: Optional[float] = 0.001,
+    get_trade_df: bool = False,
+    get_returns_df: bool = False,
+    parameter_optimization: bool = False,
+    plot_result: bool = True,
+) -> Union[None, Union[float, Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]]]:
+    """Run a backtest with long only position on a OHLC dataset.
+
+    Args:
+    ----
+        df (pd.DataFrame): The dataframe containing the OHLC data.
+
+        long_entry_function (Callable[[pd.Series, pd.Series], bool]): The long entry function, it should take 2 arguments, the current row and the previous row and return True or False depending on your strategy.
+
+        long_exit_function (Callable[[pd.Series, pd.Series, int], bool]): The long exit function, it should take 3 arguments, the current row, the previous row and the number of timeframe count since the last entry order, and return True or False depending on your strategy.
+
+        timeframe (Literal[ &quot;1min&quot;, &quot;2min&quot;, &quot;5min&quot;, &quot;15min&quot;, &quot;30min&quot;, &quot;1hour&quot;, &quot;2hour&quot;, &quot;4hour&quot;, &quot;12hour&quot;, &quot;1day&quot;, ]): The timeframe granularity of the dataframe.
+
+        take_profit (float, optional): The percent of the buy price to add to create a stop order and take the profit associated. Defaults to np.inf.
+
+        stop_loss (float, optional): The percent of the buy price to cut to create a stop order and stop the loss associated. Defaults to np.inf.
+
+        initial_equity (int, optional): The initial capital. Defaults to 1000.
+
+        maker_fees (Optional[float], optional): The fees applied, here maker for limit orders (not yet implemented). Defaults to 0.001.
+
+        taker_fees (Optional[float], optional): The fees applied, here taker for spot orders. Defaults to 0.001.
+
+        get_trade_df (bool, optional): Whether or not to return the trade dataframe (summary of trades) . Defaults to False.
+
+        get_returns_df (bool, optional): Whether or not to return the strategy returns dataframe. Defaults to False.
+
+        parameter_optimization (bool, optional): This parameter is useful when running fitting/optimization it prints nothing but the final strategy return. Defaults to False.
+
+        plot_result (bool, optional): Plot equity, price, drawdown, distribution of the strategy. Defaults to True.
+
+    Returns:
+    -----
+        Union[None, Union[float, Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]]]: Nothing or the strategy total return or the trade_df or the return_df or the trade_df and the return_df.
+    """
+    assert timeframe in [
+        "1min",
+        "2min",
+        "5min",
+        "15min",
+        "30min",
+        "1hour",
+        "2hour",
+        "4hour",
+        "12hour",
+        "1day",
+    ], "timeframe must be one of the following: 1min, 2min, 5min, 15min, 30min, 1hour, 2hour, 4hour, 12hour, 1day"
+    assert df.shape[0] > 1, "Dataframe must have at least 2 rows"
+    assert set({"Open", "High", "Low", "Close", "Returns"}).issubset(
+        df.columns
+    ), "Dataframe must have columns Open, High, Low, Close, Returns"
+
+    ohlcv_df = df.copy()
+    trades_df, returns_df = __ohlc_backtest_one_position_type(
+        ohlcv_df,
+        long_entry_function,
+        long_exit_function,
+        position_type="long",
+        take_profit=take_profit,
+        stop_loss=stop_loss,
+        maker_fees=maker_fees,
+        taker_fees=taker_fees,
+    )
+
+    returns_df["Cum_Returns"] = cumulative_returns(returns_df["Returns"])
+
     if parameter_optimization is True:
         if len(trades_df) > 0:
             return returns_df["Cum_Returns"].iloc[-1]
         return 0.0
 
     assert len(trades_df) > 0, "No trades were generated"
-    trades_df["trade_duration"] = trades_df["exit_date"] - trades_df["entry_date"]
 
-    good_trades = trades_df.loc[trades_df["trade_return"] > 0]
-    bad_trades = trades_df.loc[trades_df["trade_return"] < 0]
-    total_trades = len(trades_df)
+    returns_df["Drawdown"] = drawdown(returns_df["Returns"])
+    ohlcv_df["Cum_Returns"] = cumulative_returns(df["Returns"])
+    ohlcv_df["Drawdown"] = drawdown(df["Returns"])
+    trades_df["trade_duration"] = trades_df["exit_date"] - trades_df["entry_date"]
 
     print(f"{'  Initial informations  ':-^50}")
     print(f"Period: [{str(ohlcv_df.index[0])}] -> [{str(ohlcv_df.index[-1])}]")
     print(f"Intial balance: {initial_equity:.2f} $")
     if taker_fees is not None and maker_fees is not None:
         print(
             f"Taker fees: {taker_fees*100:.2f} %, Maker fees: {maker_fees*100:.2f} %, All the metrics will be calculated considering these fees"
         )
     else:
         print("No fees considered here.")
 
-    print(f"\n{'  Strategy performances  ':-^50}")
-
-    print(
-        f'Strategy final net balance: {returns_df["Cum_Returns"].iloc[-1]*initial_equity:.2f} $, return: {(returns_df["Cum_Returns"].iloc[-1]-1)*100:.2f} %'
+    print_ohlc_backtest_report(
+        returns_df=returns_df,
+        trades_df=trades_df,
+        ohlcv_df=ohlcv_df,
+        timeframe=timeframe,
+        initial_equity=initial_equity,
     )
-    print(
-        f'Buy & Hold final net balance: {ohlcv_df["Cum_Returns"].iloc[-1]*initial_equity:.2f} $, returns: {(ohlcv_df["Cum_Returns"].iloc[-1]-1)*100:.2f} %'
-    )
-    print(f"Strategy winrate ratio: {100 * len(good_trades) / total_trades:.2f} %")
-    print(
-        f"Strategy profit factor ratio: {abs(good_trades['trade_return'].mean()/bad_trades['trade_return'].mean()):.2f}"
-    )
-
-    print(f"\n{'  Returns statistical information  ':-^50}")
 
-    print(
-        f"Expected return : {100*returns_df['Returns'].mean():.2f} %, annuzalized: {100*returns_df['Returns'].mean()*N:.2f} %"
-    )
-    print(
-        f"Median return : {100*returns_df['Returns'].median():.2f} %, annuzalized: {100*returns_df['Returns'].median()*N:.2f} %"
-    )
-    print(
-        f'Expected volatility: {100*returns_df["Returns"].std():.2f} %, annualized: {100*returns_df["Returns"].std()*(N**0.5):.2f} %'
-    )
-    print(
-        f'Skewness: {skew(returns_df["Returns"].values):.2f}, <0 = left tail, >0 = right tail -> the higher the better'
-    )
-    print(
-        f'Kurtosis: {kurtosis(returns_df["Returns"].values):.2f}',
-        ", >3 = fat tails, <3 = thin tails -> the lower the better",
-    )
-    print(f"{timeframe}-95%-VaR: {100*value_at_risk(returns_df['Returns']):.2f} %")
-    print(
-        f"{timeframe}-95%-CVaR: {100*conditional_value_at_risk(returns_df['Returns']):.2f} %"
-    )
-
-    print(f"\n{'  Strategy statistical information  ':-^50}")
-    print(f"Max drawdown: {100*max_drawdown(returns_df['Returns']):.2f} %")
-    print(f"Kelly criterion: {100*kelly_criterion(returns_df.Returns):.2f} %")
-    print(
-        f"Sharpe ratio (annualized): {sharpe_ratio(returns_df['Returns'], N,risk_free_rate=N*ohlcv_df.Returns.mean()):.2f} (risk free rate = buy and hold)"
-    )
-    print(
-        f"Sortino ratio (annualized): {sortino_ratio(returns_df['Returns'], N,risk_free_rate=N*ohlcv_df.Returns.mean()):.2f} (risk free rate = buy and hold)"
-    )
-    print(
-        f"Calmar ratio (annualized): {calmar_ratio(returns_df['Returns'], N):.2f} (risk free rate = buy and hold)"
-    )
-
-    print(f"\n{'  Trades informations  ':-^50}")
-    print(f"Mean trade return : {100*trades_df['trade_return'].mean():.2f} %")
-    print(f"Median trade return : {100*trades_df['trade_return'].median():.2f} %")
-    print(f'Mean trade volatility: {100*trades_df["trade_return"].std():.2f} %')
-    print(
-        f"Mean trade duration: {str((trades_df['trade_duration']).mean()).split('.')[0]}"
-    )
-
-    print(f"Total trades: {total_trades}")
-
-    print(f"\n  Total good trades: {len(good_trades)}")
-    print(f"  Mean good trades return: {100*good_trades['trade_return'].mean():.2f} %")
-    print(
-        f"  Median good trades return: {100*good_trades['trade_return'].median():.2f} %"
-    )
-    print(
-        f"  Best trades return: {100*trades_df['trade_return'].max():.2f} % | Date: {trades_df.iloc[trades_df['trade_return'].idxmax()]['exit_date']} | Duration: {trades_df.iloc[trades_df['trade_return'].idxmax()]['trade_duration']}"
-    )
-    print(
-        f"  Mean good trade duration: {str((good_trades['trade_duration']).mean()).split('.')[0]}"
-    )
-    print(f"\n  Total bad trades: {len(bad_trades)}")
-    print(f"  Mean bad trades return: {100*bad_trades['trade_return'].mean():.2f} %")
-    print(
-        f"  Median bad trades return: {100*bad_trades['trade_return'].median():.2f} %"
-    )
-    print(
-        f"  Worst trades return: {100*trades_df['trade_return'].min():.2f} % | Date: {trades_df.iloc[trades_df['trade_return'].idxmin()]['exit_date']} | Duration: {trades_df.iloc[trades_df['trade_return'].idxmin()]['trade_duration']}"
-    )
-    print(
-        f"  Mean bad trade duration: {str((bad_trades['trade_duration']).mean()).split('.')[0]}"
-    )
-
-    print(f"\nExit reasons repartition: ")
-    for reason, val in zip(
-        trades_df.exit_reason.value_counts().index, trades_df.exit_reason.value_counts()
-    ):
-        print(f"- {reason}: {val}")
     if plot_result is True:
         plot_from_trade_df(trades_df, ohlcv_df, returns_df)
     if get_returns_df and get_trade_df:
         return trades_df, returns_df
     if get_trade_df:
         return trades_df
     if get_returns_df:
@@ -426,260 +543,57 @@
         "12hour",
         "1day",
     ], "timeframe must be one of the following: 1min, 2min, 5min, 15min, 30min, 1hour, 2hour, 4hour, 12hour, 1day"
     assert df.shape[0] > 1, "Dataframe must have at least 2 rows"
     assert set({"Open", "High", "Low", "Close", "Returns"}).issubset(
         df.columns
     ), "Dataframe must have columns Open, High, Low, Close, Returns"
-    timeframe_annualized = {
-        "1min": int(365 * 24 / 1 * 60),
-        "2min": int(365 * 24 / 1 * 30),
-        "5min": int(365 * 24 / 1 * 12),
-        "15min": int(365 * 24 / 1 * 4),
-        "30min": int(365 * 24 / 1 * 2),
-        "1hour": int(365 * 24 / 1),
-        "2hour": int(365 * 24 / 2),
-        "4hour": int(365 * 24 / 4),
-        "12hour": int(365 * 24 / 12),
-        "1day": 365,
-    }
-    N = timeframe_annualized[timeframe]
-    ohlcv_df = df.copy()
-    previous_row = ohlcv_df.iloc[0]
-    position_opened = False
-    timeframe_count = 0
-    current_trade: dict[str, float | datetime | int | str | pd.Timestamp] = {}
 
-    trades_df = pd.DataFrame(
-        columns=[
-            "entry_date",
-            "entry_price",
-            "entry_reason",
-            "exit_date",
-            "exit_price",
-            "exit_reason",
-            "trade_return",
-        ]
+    ohlcv_df = df.copy()
+    trades_df, returns_df = __ohlc_backtest_one_position_type(
+        ohlcv_df,
+        short_entry_function,
+        short_exit_function,
+        position_type="short",
+        take_profit=take_profit,
+        stop_loss=stop_loss,
+        maker_fees=maker_fees,
+        taker_fees=taker_fees,
     )
 
-    returns_df = pd.DataFrame(columns=["Returns"])
-
-    for index, row in tqdm(
-        ohlcv_df[1:].iterrows(),
-        desc="Backtesting...",
-        total=ohlcv_df.shape[0] - 1,
-        leave=False,
-    ):
-        if position_opened is False and short_entry_function(row, previous_row) is True:
-            position_opened = True
-            current_trade["entry_date"] = index
-            current_trade["entry_price"] = row.Close
-            current_trade["entry_reason"] = "Entry position triggered"
-            timeframe_count = 1
-            entry_price = row.Close
-        elif (
-            position_opened is True
-            and current_trade["entry_price"] * (1 + stop_loss) <= row.High
-        ):
-            position_opened = False
-            current_trade["exit_date"] = index
-            current_trade["exit_price"] = current_trade["entry_price"] * (1 + stop_loss)
-            current_trade["exit_reason"] = "Stop loss triggered"
-
-            rets = -ohlcv_df.loc[
-                current_trade["entry_date"] : current_trade["exit_date"]
-            ].Returns
-            if isinstance(taker_fees, float) and taker_fees > 0:
-                rets.iloc[0] = rets.iloc[0] - taker_fees
-                rets.iloc[-1] = rets.iloc[-1] - taker_fees
-            current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
-
-            trades_df = pd.concat(
-                [trades_df, pd.DataFrame([current_trade])], ignore_index=True
-            )
-            returns_df = pd.concat(
-                [returns_df, pd.DataFrame({"Returns": rets.values}, index=rets.index)],
-                ignore_index=False,
-            )
-            timeframe_count = 0
-
-            current_trade = {}
-        elif (
-            position_opened is True
-            and current_trade["entry_price"] * (1 - take_profit) >= row.Low
-        ):
-            position_opened = False
-            current_trade["exit_date"] = index
-            current_trade["exit_price"] = float(current_trade["entry_price"]) * (
-                1 - take_profit
-            )
-            current_trade["exit_reason"] = "Take profit triggered"
-
-            rets = -ohlcv_df.loc[
-                current_trade["entry_date"] : current_trade["exit_date"]
-            ].Returns
-            if isinstance(taker_fees, float) and taker_fees > 0:
-                rets.iloc[0] = rets.iloc[0] - taker_fees
-                rets.iloc[-1] = rets.iloc[-1] - taker_fees
-            current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
-
-            trades_df = pd.concat(
-                [trades_df, pd.DataFrame([current_trade])], ignore_index=True
-            )
-            returns_df = pd.concat(
-                [returns_df, pd.DataFrame({"Returns": rets.values}, index=rets.index)],
-                ignore_index=False,
-            )
-            timeframe_count = 0
-            current_trade = {}
-        elif (
-            position_opened is True
-            and short_exit_function(row, previous_row, timeframe_count) is True
-        ):
-            position_opened = False
-            current_trade["exit_date"] = index
-            current_trade["exit_price"] = row.Close
-            current_trade["exit_reason"] = "Exit position triggered"
-
-            rets = -ohlcv_df.loc[
-                current_trade["entry_date"] : current_trade["exit_date"]
-            ].Returns
-
-            if isinstance(taker_fees, float) and taker_fees > 0:
-                rets.iloc[0] = rets.iloc[0] - taker_fees
-                rets.iloc[-1] = rets.iloc[-1] - taker_fees
+    returns_df["Cum_Returns"] = cumulative_returns(returns_df["Returns"])
 
-            current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
-
-            trades_df = pd.concat(
-                [trades_df, pd.DataFrame([current_trade])], ignore_index=True
-            )
-            returns_df = pd.concat(
-                [returns_df, pd.DataFrame({"Returns": rets.values}, index=rets.index)],
-                ignore_index=False,
-            )
-            timeframe_count = 0
-            current_trade = {}
-        else:
-            timeframe_count += 1
-        previous_row = row
-
-    returns_df["Cum_Returns"] = (returns_df["Returns"] + 1).cumprod()
-    returns_df["Drawdown"] = drawdown(returns_df["Returns"])
-    ohlcv_df["Cum_Returns"] = (df["Returns"] + 1).cumprod()
-    ohlcv_df["Drawdown"] = drawdown(df["Returns"])
     if parameter_optimization is True:
         if len(trades_df) > 0:
             return returns_df["Cum_Returns"].iloc[-1]
         return 0.0
 
     assert len(trades_df) > 0, "No trades were generated"
-    trades_df["trade_duration"] = trades_df["exit_date"] - trades_df["entry_date"]
 
-    good_trades = trades_df.loc[trades_df["trade_return"] > 0]
-    bad_trades = trades_df.loc[trades_df["trade_return"] < 0]
-    total_trades = len(trades_df)
+    returns_df["Drawdown"] = drawdown(returns_df["Returns"])
+    ohlcv_df["Cum_Returns"] = cumulative_returns(df["Returns"])
+    ohlcv_df["Drawdown"] = drawdown(df["Returns"])
+    trades_df["trade_duration"] = trades_df["exit_date"] - trades_df["entry_date"]
 
     print(f"{'  Initial informations  ':-^50}")
     print(f"Period: [{str(ohlcv_df.index[0])}] -> [{str(ohlcv_df.index[-1])}]")
     print(f"Intial balance: {initial_equity:.2f} $")
     if taker_fees is not None and maker_fees is not None:
         print(
             f"Taker fees: {taker_fees*100:.2f} %, Maker fees: {maker_fees*100:.2f} %, All the metrics will be calculated considering these fees"
         )
     else:
         print("No fees considered here.")
-
-    print(f"\n{'  Strategy performances  ':-^50}")
-
-    print(
-        f'Strategy final net balance: {returns_df["Cum_Returns"].iloc[-1]*initial_equity:.2f} $, return: {(returns_df["Cum_Returns"].iloc[-1]-1)*100:.2f} %'
-    )
-    print(
-        f'Buy & Hold final net balance: {ohlcv_df["Cum_Returns"].iloc[-1]*initial_equity:.2f} $, returns: {(ohlcv_df["Cum_Returns"].iloc[-1]-1)*100:.2f} %'
-    )
-    print(f"Strategy winrate ratio: {100 * len(good_trades) / total_trades:.2f} %")
-    print(
-        f"Strategy profit factor ratio: {abs(good_trades['trade_return'].mean()/bad_trades['trade_return'].mean()):.2f}"
-    )
-
-    print(f"\n{'  Returns statistical information  ':-^50}")
-
-    print(
-        f"Expected return : {100*returns_df['Returns'].mean():.2f} %, annuzalized: {100*returns_df['Returns'].mean()*N:.2f} %"
-    )
-    print(
-        f"Median return : {100*returns_df['Returns'].median():.2f} %, annuzalized: {100*returns_df['Returns'].median()*N:.2f} %"
-    )
-    print(
-        f'Expected volatility: {100*returns_df["Returns"].std():.2f} %, annualized: {100*returns_df["Returns"].std()*(N**0.5):.2f} %'
-    )
-    print(
-        f'Skewness: {skew(returns_df["Returns"].values):.2f}, <0 = left tail, >0 = right tail -> the higher the better'
-    )
-    print(
-        f'Kurtosis: {kurtosis(returns_df["Returns"].values):.2f}',
-        ", >3 = fat tails, <3 = thin tails -> the lower the better",
+    print_ohlc_backtest_report(
+        returns_df=returns_df,
+        trades_df=trades_df,
+        ohlcv_df=ohlcv_df,
+        timeframe=timeframe,
+        initial_equity=initial_equity,
     )
-    print(f"{timeframe}-95%-VaR: {100*value_at_risk(returns_df['Returns']):.2f} %")
-    print(
-        f"{timeframe}-95%-CVaR: {100*conditional_value_at_risk(returns_df['Returns']):.2f} %"
-    )
-
-    print(f"\n{'  Strategy statistical information  ':-^50}")
-    print(f"Max drawdown: {100*max_drawdown(returns_df['Returns']):.2f} %")
-    print(f"Kelly criterion: {100*kelly_criterion(returns_df.Returns):.2f} %")
-    print(
-        f"Sharpe ratio (annualized): {sharpe_ratio(returns_df['Returns'], N,risk_free_rate=N*ohlcv_df.Returns.mean()):.2f} (risk free rate = buy and hold)"
-    )
-    print(
-        f"Sortino ratio (annualized): {sortino_ratio(returns_df['Returns'], N,risk_free_rate=N*ohlcv_df.Returns.mean()):.2f} (risk free rate = buy and hold)"
-    )
-    print(
-        f"Calmar ratio (annualized): {calmar_ratio(returns_df['Returns'], N):.2f} (risk free rate = buy and hold)"
-    )
-
-    print(f"\n{'  Trades informations  ':-^50}")
-    print(f"Mean trade return : {100*trades_df['trade_return'].mean():.2f} %")
-    print(f"Median trade return : {100*trades_df['trade_return'].median():.2f} %")
-    print(f'Mean trade volatility: {100*trades_df["trade_return"].std():.2f} %')
-    print(
-        f"Mean trade duration: {str((trades_df['trade_duration']).mean()).split('.')[0]}"
-    )
-
-    print(f"Total trades: {total_trades}")
-
-    print(f"\n  Total good trades: {len(good_trades)}")
-    print(f"  Mean good trades return: {100*good_trades['trade_return'].mean():.2f} %")
-    print(
-        f"  Median good trades return: {100*good_trades['trade_return'].median():.2f} %"
-    )
-    print(
-        f"  Best trades return: {100*trades_df['trade_return'].max():.2f} % | Date: {trades_df.iloc[trades_df['trade_return'].idxmax()]['exit_date']} | Duration: {trades_df.iloc[trades_df['trade_return'].idxmax()]['trade_duration']}"
-    )
-    print(
-        f"  Mean good trade duration: {str((good_trades['trade_duration']).mean()).split('.')[0]}"
-    )
-    print(f"\n  Total bad trades: {len(bad_trades)}")
-    print(f"  Mean bad trades return: {100*bad_trades['trade_return'].mean():.2f} %")
-    print(
-        f"  Median bad trades return: {100*bad_trades['trade_return'].median():.2f} %"
-    )
-    print(
-        f"  Worst trades return: {100*trades_df['trade_return'].min():.2f} % | Date: {trades_df.iloc[trades_df['trade_return'].idxmin()]['exit_date']} | Duration: {trades_df.iloc[trades_df['trade_return'].idxmin()]['trade_duration']}"
-    )
-    print(
-        f"  Mean bad trade duration: {str((bad_trades['trade_duration']).mean()).split('.')[0]}"
-    )
-
-    print(f"\nExit reasons repartition: ")
-    for reason, val in zip(
-        trades_df.exit_reason.value_counts().index, trades_df.exit_reason.value_counts()
-    ):
-        print(f"- {reason}: {val}")
     if plot_result is True:
         plot_from_trade_df(trades_df, ohlcv_df, returns_df)
     if get_returns_df and get_trade_df:
         return trades_df, returns_df
     if get_trade_df:
         return trades_df
     if get_returns_df:
```

### Comparing `quant_invest_lab-0.2.6/quant_invest_lab/data_provider.py` & `quant_invest_lab-0.2.7/quant_invest_lab/data_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from datetime import datetime
+from functools import lru_cache
 from typing import Optional, Callable, Literal
 import os
 import pandas as pd
 import json
 import time
 from random import randint
 from kucoin.client import Market
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from tqdm import tqdm
 
 
+@lru_cache(maxsize=32, typed=True)
 def build_multi_crypto_dataframe(
     symbols: set,
     drop_na: bool = False,
     column_to_keep: str = "Close",
     timeframe: Literal[
         "1min",
         "2min",
@@ -63,14 +65,15 @@
                 ),
             ],
             axis=1,
         )
     return df if not drop_na else df.dropna()
 
 
+@lru_cache(maxsize=32, typed=True)
 def download_crypto_historical_data(
     symbol: str,
     timeframe: str = "1hour",
     compute_return: bool = True,
     refresh_list_of_symbol: bool = True,
 ) -> pd.DataFrame:
     """Fetch a cryptocurrency historical data from Kucoin for a given symbol and timeframe.
```

### Comparing `quant_invest_lab-0.2.6/quant_invest_lab/indicators.py` & `quant_invest_lab-0.2.7/quant_invest_lab/indicators.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.6/quant_invest_lab/metrics.py` & `quant_invest_lab-0.2.7/quant_invest_lab/metrics.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,58 @@
 import numpy as np
 import numpy.typing as npt
+from functools import lru_cache
 import pandas as pd
 import scipy.stats as stat
 from typing import Literal, Union
 
 
+@lru_cache(maxsize=20, typed=True)
+def profit_factor(
+    avg_win_return: float,
+    avg_loss_return: float,
+) -> float:
+    """The profit factor is a measure of how much profit you make per dollar that you lose. It is defined as the ratio of the total amount of money won to the total amount of money lost
+
+    Args:
+    -----
+        avg_win_return (float): The average winning trade return.
+
+        avg_loss_return (float): The average losing trade return.
+
+    Returns:
+    -----
+        float: The profit factor, it has no unit.
+    """
+    return abs(avg_win_return / avg_loss_return)
+
+
+@lru_cache(maxsize=20, typed=True)
+def expectancy(
+    winrate: float,
+    avg_win_return: float,
+    avg_loss_return: float,
+) -> float:
+    """Expectancy is a measure of the % average amount of money, (or percentage if you prefer) that you can expect to win (or lose) per trade.
+
+    Args:
+    -----
+        winrate (float): The percentage of winning trades.
+
+        avg_win_return (float): The average winning trade return.
+
+        avg_loss_return (float): The average losing trade return.
+
+    Returns:
+    -----
+        float: The expectancy.
+    """
+    return (1 + profit_factor(avg_win_return, avg_loss_return)) * winrate - 1
+
+
 def sharpe_ratio(
     returns: pd.Series,
     N: Union[int, float] = 365,
     risk_free_rate: float = 0.03,
 ) -> float:
     """The economist William F. Sharpe proposed the Sharpe ratio in 1966 as an extension of his work on the Capital Asset Pricing Model (CAPM). It is defined as the difference between the returns of the investment and the risk-free return, divided by the standard deviation of the investment.
 
@@ -78,19 +122,21 @@
 def calmar_ratio(
     returns: pd.Series,
     N: Union[int, float] = 365,
 ) -> float:
     """The final risk/reward ratio we will consider is the Calmar ratio. This is similar to the other ratios, with the key difference being that the Calmar ratio uses max drawdown in the denominator as opposed to standard deviation.
 
     Args:
+    -----
         returns (pd.Series): The strategy or portfolio not cumulative returns.
 
         N (Union[int, float], optional): The number of periods in a year. Defaults to 365.
 
     Returns:
+    -----
         float: The annualized calmar ratio.
     """
     return (returns.mean() * N) / abs(max_drawdown(returns))
 
 
 def downside_risk(returns: pd.Series) -> float:
     """Downside risk or Semi-Deviation is a method of measuring the fluctuations below the mean, unlike variance or standard deviation it only looks at the negative price fluctuations and it's used to evaluate the downside risk (The risk of loss in an investment) of an investment.
@@ -113,17 +159,31 @@
     ----
         returns (pd.Series): The strategy or portfolio not cumulative returns.
 
     Returns:
     ----
         pd.Series: The drawdown series.
     """
-    cumulative_returns = (returns + 1).cumprod()
-    running_max = cumulative_returns.cummax()
-    return (cumulative_returns - running_max) / running_max
+    cum_ret = cumulative_returns(returns)
+    running_max = cum_ret.cummax()
+    return (cum_ret - running_max) / running_max
+
+
+def cumulative_returns(returns: pd.Series) -> pd.Series:
+    """Computes the cumulative returns series of a given returns (not cumulative) time series.
+
+    Args:
+    ----
+        returns (pd.Series): The strategy or portfolio not cumulative returns.
+
+    Returns:
+    -----
+        pd.Series: The cumulative returns series.
+    """
+    return (returns + 1).cumprod()
 
 
 def max_drawdown(
     returns: pd.Series,
 ) -> float:
     """Max drawdown quantifies the steepest decline from peak to trough observed for an investment.
```

### Comparing `quant_invest_lab-0.2.6/quant_invest_lab/optimization.py` & `quant_invest_lab-0.2.7/quant_invest_lab/optimization.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.6/quant_invest_lab/portfolio.py` & `quant_invest_lab-0.2.7/quant_invest_lab/portfolio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from sklearn.decomposition import PCA
 from typing import Iterable, Literal, Optional
 import pandas as pd
 import numpy as np
 import numpy.typing as npt
 import numpy.linalg as linalg
 import matplotlib.pyplot as plt
 from tqdm import tqdm
@@ -489,64 +488,7 @@
                 p: [w]
                 for p, w in zip(
                     self._returns.columns,
                     self.__all_weights[ind, :],
                 )
             }
         )
-
-
-def reduce_dimentionality(
-    full_dataframe: pd.DataFrame,
-    mode: Literal["pca", "tsne"] = "pca",
-    target_explained_variance: float = 0.95,
-    result_as_df: bool = True,
-) -> npt.NDArray[np.float64] | pd.DataFrame:
-    """Reduce the dimension of a dataset given a target explained variance.
-
-    Args:
-    -----
-        full_dataframe (pd.DataFrame): The dataframe to reduce the dimension.
-
-        mode (Literal[&quot;pca&quot;, &quot;tsne&quot;], optional): The dimensionality reduction algorithm. Defaults to "pca".
-
-        target_explained_variance (float, optional): The minimum threshold for explained variance. Defaults to 0.95.
-
-        result_as_df (bool, optional): Whether or not return the result as a dataframe or as a numpy array. Defaults to True.
-
-    Returns:
-    -------
-        npt.NDArray[np.float64] | pd.DataFrame: The reduced dataset.
-    """
-    assert (
-        isinstance(full_dataframe, pd.DataFrame)
-        and full_dataframe.shape[0] != 0
-        and full_dataframe.shape[1] > 1
-    ), "full_dataframe must be a pandas DataFrame containing at least 2 columns and 1 row"
-    assert (
-        target_explained_variance > 0 and target_explained_variance < 1
-    ), "target_explained_variance must be a float between 0 and 1"
-    X = full_dataframe.to_numpy()
-    match mode:
-        case "pca":
-            calibration_pca = PCA()
-            calibration_pca.fit(X)
-
-            d = (
-                np.argmax(
-                    np.cumsum(calibration_pca.explained_variance_ratio_)
-                    >= target_explained_variance
-                )
-                + 1
-            )
-            pca = PCA(n_components=d)
-            pca.fit(X)
-
-            if result_as_df:
-                return pd.DataFrame(
-                    pca.transform(X), columns=[f"PC_{i}" for i in range(1, d + 1)]
-                )
-            return pca.transform(X)
-        case "tsne":
-            raise NotImplementedError("TSNE is not implemented yet")
-        case _:
-            raise ValueError("mode must be either pca or tsne")
```

### Comparing `quant_invest_lab-0.2.6/quant_invest_lab/screener.py` & `quant_invest_lab-0.2.7/quant_invest_lab/screener.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.6/quant_invest_lab/simulation.py` & `quant_invest_lab-0.2.7/quant_invest_lab/simulation.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.6/PKG-INFO` & `quant_invest_lab-0.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 Metadata-Version: 2.1
 Name: quant-invest-lab
-Version: 0.2.6
+Version: 0.2.7
 Summary: Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project.
+Home-page: https://github.com/BaptisteZloch/Quant-Invest-Lab
+License: MIT
+Keywords: trading,backtest,investments,portfolio,quantitative
 Author: BaptisteZloch
 Author-email: bzloch@hotmail.fr
+Maintainer: BaptisteZloch
+Maintainer-email: bzloch@hotmail.fr
 Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Office/Business :: Financial :: Investment
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: fitter (>=1.5.2,<2.0.0)
 Requires-Dist: kucoin-python (>=1.0.11,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: nbformat (>=5.8.0,<6.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: ta (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Project-URL: Bug Tracker, https://github.com/BaptisteZloch/Quant-Invest-Lab/issues
+Project-URL: Repository, https://github.com/BaptisteZloch/Quant-Invest-Lab
 Description-Content-Type: text/markdown
 
 # Quant Invest Lab
 <p align="left">
 <a href="https://pypi.org/project/quant-invest-lab/"><img alt="PyPI" src="https://img.shields.io/pypi/v/quant-invest-lab"></a>
 <a><img alt="commit update" src="https://img.shields.io/github/last-commit/BaptisteZloch/Quant-Invest-Lab"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
@@ -77,15 +88,15 @@
 
 df_BTC = df_BTC.dropna()
 
 # Define your strategy entry and exit functions
 def buy_func(row: pd.Series, prev_row: pd.Series) -> bool:
     return True if row.EMA20 > row.EMA60 else False
 
-def sell_func(row: pd.Series, prev_row: pd.Series, trading_days: pd.Series) -> bool:
+def sell_func(row: pd.Series, prev_row: pd.Series, trading_days: int) -> bool:
     return True if row.EMA20 < row.EMA60 else False
 
 # Backtest your strategy
 ohlc_long_only_backtester(
     df=df_BTC,
     long_entry_function=buy_func,
     long_exit_function=sell_func,
```

#### html2text {}

```diff
@@ -1,24 +1,32 @@
-Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.6 Summary: Quant
+Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.7 Summary: Quant
 Invest Lab is a python package to help you to do some quantitative experiments,
 while trying to learn or build quantitative investment solutions. This project
 was initially my own set of functionnalities but I decided to build a package
-for that and sharing it as open source project. Author: BaptisteZloch Author-
-email: bzloch@hotmail.fr Requires-Python: >=3.8,<3.12 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: fitter
+for that and sharing it as open source project. Home-page: https://github.com/
+BaptisteZloch/Quant-Invest-Lab License: MIT Keywords:
+trading,backtest,investments,portfolio,quantitative Author: BaptisteZloch
+Author-email: bzloch@hotmail.fr Maintainer: BaptisteZloch Maintainer-email:
+bzloch@hotmail.fr Requires-Python: >=3.8,<3.12 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic :: Office/
+Business :: Financial :: Investment Classifier: Topic :: Software Development
+:: Build Tools Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: fitter
 (>=1.5.2,<2.0.0) Requires-Dist: kucoin-python (>=1.0.11,<2.0.0) Requires-Dist:
 matplotlib (>=3.7.1,<4.0.0) Requires-Dist: nbformat (>=5.8.0,<6.0.0) Requires-
 Dist: numpy (>=1.23.5,<2.0.0) Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-
 Dist: plotly (>=5.14.1,<6.0.0) Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0) Requires-Dist: seaborn
 (>=0.12.2,<0.13.0) Requires-Dist: statsmodels (>=0.14.0,<0.15.0) Requires-Dist:
-ta (>=0.10.2,<0.11.0) Requires-Dist: tqdm (>=4.64.1,<5.0.0) Description-
+ta (>=0.10.2,<0.11.0) Requires-Dist: tqdm (>=4.64.1,<5.0.0) Project-URL: Bug
+Tracker, https://github.com/BaptisteZloch/Quant-Invest-Lab/issues Project-URL:
+Repository, https://github.com/BaptisteZloch/Quant-Invest-Lab Description-
 Content-Type: text/markdown # Quant Invest Lab
 [PyPI] [commit update] [Code_style:_black] [Code_Climate] [GitHub_Actions_CI]
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-
 brightgreen.svg?style=flat-square)](https://github.com/BaptisteZloch/Quant-
 Invest-Lab/issues) **Quant Invest Lab** is a project aimed to provide a set of
 basic tools for quantitative experiments. By quantitative experiment I mean
 trying to build you own set of investments solution. The project is still in
@@ -46,17 +54,17 @@
 pd from quant_invest_lab.backtest import ohlc_long_only_backtester from
 quant_invest_lab.data_provider import download_crypto_historical_data symbol =
 "BTC-USDT" timeframe = "4hour" df_BTC = download_crypto_historical_data(symbol,
 timeframe) # Define your indicators df_BTC["EMA20"] = df_BTC.Close.ewm(20).mean
 () df_BTC["EMA60"] = df_BTC.Close.ewm(60).mean() df_BTC = df_BTC.dropna() #
 Define your strategy entry and exit functions def buy_func(row: pd.Series,
 prev_row: pd.Series) -> bool: return True if row.EMA20 > row.EMA60 else False
-def sell_func(row: pd.Series, prev_row: pd.Series, trading_days: pd.Series) -
-> bool: return True if row.EMA20 < row.EMA60 else False # Backtest your
-strategy ohlc_long_only_backtester( df=df_BTC, long_entry_function=buy_func,
+def sell_func(row: pd.Series, prev_row: pd.Series, trading_days: int) -> bool:
+return True if row.EMA20 < row.EMA60 else False # Backtest your strategy
+ohlc_long_only_backtester( df=df_BTC, long_entry_function=buy_func,
 long_exit_function=sell_func, timeframe=timeframe, initial_equity=1000, ) ```
 ## Optimize a portfolio (mean-variance) ```python from
 quant_invest_lab.portfolio import MonteCarloPortfolio, ConvexPortfolio,
 RiskParityPortfolio from quant_invest_lab.data_provider import
 build_multi_crypto_dataframe symbols = set( [ "BNB-USDT", "BTC-USDT", "NEAR-
 USDT", "ETH-USDT", "SOL-USDT", "EGLD-USDT", "ALGO-USDT", "FTM-USDT", "ADA-
 USDT", ] ) closes = build_multi_crypto_dataframe(symbols) returns =
```

