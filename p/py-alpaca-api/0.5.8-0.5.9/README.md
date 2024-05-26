# Comparing `tmp/py_alpaca_api-0.5.8.tar.gz` & `tmp/py_alpaca_api-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.5.8.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.5.9.tar", max compression
```

## Comparing `py_alpaca_api-0.5.8.tar` & `py_alpaca_api-0.5.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2024-05-24 01:31:49.350968 py_alpaca_api-0.5.8/LICENSE
--rw-r--r--   0        0        0    16791 2024-05-24 01:31:49.350968 py_alpaca_api-0.5.8/README.md
--rw-r--r--   0        0        0        0 2024-05-24 01:31:49.354302 py_alpaca_api-0.5.8/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0     2193 2024-05-25 16:14:06.398947 py_alpaca_api-0.5.8/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0        0 2024-05-24 01:31:49.354302 py_alpaca_api-0.5.8/py_alpaca_api/src/__init__.py
--rw-r--r--   0        0        0     6216 2024-05-25 16:14:06.398947 py_alpaca_api-0.5.8/py_alpaca_api/src/account.py
--rw-r--r--   0        0        0     3324 2024-05-25 16:14:06.398947 py_alpaca_api-0.5.8/py_alpaca_api/src/asset.py
--rw-r--r--   0        0        0    22112 2024-05-24 02:26:00.502180 py_alpaca_api-0.5.8/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     8465 2024-05-24 02:26:07.905556 py_alpaca_api-0.5.8/py_alpaca_api/src/history.py
--rw-r--r--   0        0        0     2985 2024-05-25 16:14:06.398947 py_alpaca_api-0.5.8/py_alpaca_api/src/market.py
--rw-r--r--   0        0        0    13542 2024-05-24 02:26:23.698984 py_alpaca_api-0.5.8/py_alpaca_api/src/order.py
--rw-r--r--   0        0        0    13633 2024-05-25 16:14:06.398947 py_alpaca_api-0.5.8/py_alpaca_api/src/position.py
--rw-r--r--   0        0        0     9202 2024-05-24 02:26:38.579074 py_alpaca_api-0.5.8/py_alpaca_api/src/screener.py
--rw-r--r--   0        0        0    15411 2024-05-24 02:24:59.025171 py_alpaca_api-0.5.8/py_alpaca_api/src/watchlist.py
--rw-r--r--   0        0        0     1344 2024-05-25 16:14:06.398947 py_alpaca_api-0.5.8/pyproject.toml
--rw-r--r--   0        0        0    17593 1970-01-01 00:00:00.000000 py_alpaca_api-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-25 20:54:28.642031 py_alpaca_api-0.5.9/LICENSE
+-rw-r--r--   0        0        0    16791 2024-05-25 20:54:28.642031 py_alpaca_api-0.5.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-25 20:54:28.648697 py_alpaca_api-0.5.9/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2193 2024-05-26 00:47:40.736842 py_alpaca_api-0.5.9/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-25 20:54:28.648697 py_alpaca_api-0.5.9/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     6791 2024-05-26 00:47:40.736842 py_alpaca_api-0.5.9/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     3324 2024-05-25 20:54:28.648697 py_alpaca_api-0.5.9/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    15970 2024-05-26 15:45:30.270707 py_alpaca_api-0.5.9/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     8341 2024-05-26 00:47:40.736842 py_alpaca_api-0.5.9/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     2985 2024-05-25 20:54:28.648697 py_alpaca_api-0.5.9/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    17430 2024-05-26 15:45:30.270707 py_alpaca_api-0.5.9/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0     9323 2024-05-26 15:45:30.270707 py_alpaca_api-0.5.9/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0     8824 2024-05-26 00:47:40.736842 py_alpaca_api-0.5.9/py_alpaca_api/src/screener.py
+-rw-r--r--   0        0        0    14951 2024-05-26 13:07:04.489420 py_alpaca_api-0.5.9/py_alpaca_api/src/watchlist.py
+-rw-r--r--   0        0        0     1344 2024-05-26 15:45:30.270707 py_alpaca_api-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0    17593 1970-01-01 00:00:00.000000 py_alpaca_api-0.5.9/PKG-INFO
```

### Comparing `py_alpaca_api-0.5.8/LICENSE` & `py_alpaca_api-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.8/README.md` & `py_alpaca_api-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.8/py_alpaca_api/alpaca.py` & `py_alpaca_api-0.5.9/py_alpaca_api/alpaca.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.8/py_alpaca_api/src/account.py` & `py_alpaca_api-0.5.9/py_alpaca_api/src/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         Args:
             trade_url: The URL for the trade.
             headers: The headers for the trade request.
         """
         self.trade_url = trade_url
         self.headers = headers
 
-    def account_activities(self, activity_type: str, date: str = None, until_date: str = None) -> pd.DataFrame:
+    def activity(self, activity_type: str, date: str = None, until_date: str = None) -> pd.DataFrame:
         """
         Retrieves account activities for a specific activity type.
 
         Args:
             activity_type (str): The type of activity to retrieve.
             date (str, optional): The starting date for the activities. Defaults to None.
             until_date (str, optional): The ending date for the activities. Defaults to None.
@@ -51,17 +51,40 @@
         request = requests.get(url=url, headers=self.headers, params=params)
 
         if request.status_code != 200:
             raise Exception(f"Failed to get account activities. Response: {request.text}")
 
         response = json.loads(request.text)
 
+        activity_df = pd.DataFrame()
+        activity_df = activity_df.assign(
+            symbol="NAN",
+            activity_type="NAN",
+            id="NAN",
+            cum_qty="NAN",
+            leaves_qty="NAN",
+            price="NAN",
+            qty="NAN",
+            side="NAN",
+            transaction_time="NAN",
+            order_id="NAN",
+            type="NAN",
+            order_status="NAN",
+        )
+
         activity_df = pd.DataFrame(response).reset_index(drop=True)
 
-        activity_df["transaction_time"] = [pendulum.parse(x, tz="America/New_York").to_datetime_string() for x in activity_df["transaction_time"]]
+        if activity_df.empty:
+            return activity_df
+
+        activity_df["transaction_time"] = (
+            [pendulum.parse(x, tz="America/New_York").to_datetime_string() for x in activity_df["transaction_time"]]
+            if "transaction_time" in activity_df.columns
+            else None
+        )
 
         activity_df = activity_df.astype(
             {
                 "symbol": "str",
                 "activity_type": "str",
                 "id": "str",
                 "cum_qty": "float",
```

### Comparing `py_alpaca_api-0.5.8/py_alpaca_api/src/asset.py` & `py_alpaca_api-0.5.9/py_alpaca_api/src/asset.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.8/py_alpaca_api/src/history.py` & `py_alpaca_api-0.5.9/py_alpaca_api/src/history.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 import requests
 
 from .asset import Asset
 from .data_classes import AssetClass
 
 
 class History:
-    def __init__(
-        self, data_url: str, headers: Dict[str, str], asset: Asset
-    ) -> None:
+    def __init__(self, data_url: str, headers: Dict[str, str], asset: Asset) -> None:
         """
         Args:
             data_url: A string representing the URL of the data.
             headers: A dictionary containing the headers to be included in the request.
             asset: An instance of the Asset class representing the asset.
 
         """
@@ -74,23 +72,19 @@
             "4h": "4Hour",
             "1d": "1Day",
             "1w": "1Week",
             "1M": "1Month",
         }
 
         if timeframe not in timeframe_mapping:
-            raise ValueError(
-                'Invalid timeframe. Must be "1m", "5m", "15m", "30m", "1h", "4h", "1d", "1w", or "1M"'
-            )
+            raise ValueError('Invalid timeframe. Must be "1m", "5m", "15m", "30m", "1h", "4h", "1d", "1w", or "1M"')
 
         # Parameters for historical stock data request
         params = {
-            "timeframe": timeframe_mapping[
-                timeframe
-            ],  # Timeframe for historical data, default: 1d
+            "timeframe": timeframe_mapping[timeframe],  # Timeframe for historical data, default: 1d
             "start": start,  # Start date for historical data
             "end": end,  # End date for historical data
             "currency": currency,  # Currency for historical data, default: USD
             "limit": limit,  # Limit number of data points, default: 1000
             "adjustment": adjustment,  # Adjustment for historical data, default: raw
             "feed": feed,  # Data feed source, default: iex
             "sort": sort,  # Sort order, default: asc
@@ -126,17 +120,15 @@
                 raise ValueError(f"{symbol} is not a stock.")
         return asset
 
     ###########################################
     # /////////// PreProcess Data \\\\\\\\\\\ #
     ###########################################
     @staticmethod
-    def preprocess_data(
-        symbol_data: list[defaultdict], symbol: str
-    ) -> pd.DataFrame:
+    def preprocess_data(symbol_data: list[defaultdict], symbol: str) -> pd.DataFrame:
         """Prepross data
         Preprocesses the given symbol data by converting it to a pandas DataFrame and performing various
         data transformations.
 
         Args:
             symbol_data: A list of defaultdict objects representing the JSON response data.
             symbol: A string representing the symbol or ticker for the stock data.
@@ -147,17 +139,15 @@
         """
         # Convert JSON response to dictionary
         bar_data_df = pd.DataFrame(symbol_data)
 
         # Add symbol column to DataFrame
         bar_data_df.insert(0, "symbol", symbol)
         # Reformat date column
-        bar_data_df["t"] = pd.to_datetime(
-            bar_data_df["t"].replace("[A-Za-z]", " ", regex=True)
-        )
+        bar_data_df["t"] = pd.to_datetime(bar_data_df["t"].replace("[A-Za-z]", " ", regex=True))
         # Rename columns for consistency
         bar_data_df.rename(
             columns={
                 "t": "date",
                 "o": "open",
                 "h": "high",
                 "l": "low",
@@ -184,17 +174,15 @@
         )
         # Return historical stock data as a DataFrame
         return bar_data_df
 
     ###########################################
     # ///////// Get Historical Data \\\\\\\\\ #
     ###########################################
-    def get_historical_data(
-        self, symbol: str, url: str, params: dict
-    ) -> list[defaultdict]:
+    def get_historical_data(self, symbol: str, url: str, params: dict) -> list[defaultdict]:
         """Get historical stock data
         Args:
             symbol (str): The symbol of the stock or asset for which historical data is being fetched.
             url (str): The URL of the API endpoint from where the historical data is being fetched.
             params (dict): Additional parameters to be passed along with the API request.
 
         Returns:
```

### Comparing `py_alpaca_api-0.5.8/py_alpaca_api/src/market.py` & `py_alpaca_api-0.5.9/py_alpaca_api/src/market.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.8/py_alpaca_api/src/order.py` & `py_alpaca_api-0.5.9/py_alpaca_api/src/order.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,85 +4,44 @@
 import requests
 
 from .data_classes import OrderClass, order_class_from_dict
 
 
 class Order:
     def __init__(self, trade_url: str, headers: Dict[str, str]) -> None:
-        """Initialize Order class
+        """
+        Initializes a new instance of the Order class.
 
-        Parameters:
-        ___________
-        trade_url: str
-                Alpaca Trade API URL required
-
-        headers: object
-                API request headers required
-
-        Raises:
-        _______
-        ValueError: If trade URL is not provided
-
-        ValueError: If headers are not provided
-        """  # noqa
+        Args:
+            trade_url (str): The URL for trading.
+            headers (Dict[str, str]): The headers for the API request.
 
+        Returns:
+            None
+        """
         self.trade_url = trade_url
         self.headers = headers
 
     #########################################################
     # \\\\\\\\\/////////  Get Order BY id \\\\\\\///////////#
     #########################################################
     def get_by_id(self, order_id: str, nested: bool = False) -> OrderClass:
-        """Get order information by order ID
-
-        Parameters:
-        -----------
-        order_id:   Order ID to get information
-                    A valid order ID string required
+        """
+        Retrieves order information by its ID.
 
-        nested:     Include nested objects (default: False)
-                    Include nested objects (optional) bool
+        Args:
+            order_id (str): The ID of the order to retrieve.
+            nested (bool, optional): Whether to include nested objects in the response. Defaults to False.
 
         Returns:
-        --------
-        OrderClass: Order information as an OrderClass object
+            OrderClass: An object representing the order information.
 
         Raises:
-        -------
-        ValueError: If failed to get order information
-
-        Example:
-        --------
-        >>> from py_alpaca_api.alpaca import PyAlpacaApi
-            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
-            order = api.order.get_by_id(order_id="ORDER_ID")
-            print(order)
-
-        OrderClass(
-            id="ORDER_ID",
-            client_order_id="CLIENT_ORDER_ID",
-            created_at="2021-10-01T00:00:00Z",
-            submitted_at="2021-10-01 00:00:00",
-            asset_id="ASSET_ID",
-            symbol="AAPL",
-            asset_class="us_equity",
-            notional=1000.0,
-            qty=10.0,
-            filled_qty=10.0,
-            filled_avg_price=100.0,
-            order_class="simple",
-            order_type="market",
-            limit_price=None,
-            stop_price=None,
-            status="new",
-            side="buy",
-            time_in_force="day",
-            extended_hours=False
-        )
-        """  # noqa
+            ValueError: If the request to retrieve order information fails.
+        """
 
         # Parameters for the request
         params = {"nested": nested}
         # Alpaca API URL for order information
         url = f"{self.trade_url}/orders/{order_id}"
         # Get request to Alpaca API for order information
         response = requests.get(url, headers=self.headers, params=params)
@@ -91,122 +50,112 @@
             # Convert JSON response to dictionary
             res = json.loads(response.text)
             # Return order information as an OrderClass object
             return order_class_from_dict(res)
         # If response is not successful, raise an exception
         else:
             res = json.loads(response.text)
-            raise ValueError(
-                f'Failed to get order information. Response: {res["message"]}'
-            )
+            raise ValueError(f'Failed to get order information. Response: {res["message"]}')
 
     ########################################################
     # \\\\\\\\\\\\\\\\\ Cancel Order By ID /////////////////#
     ########################################################
     def cancel_by_id(self, order_id: str) -> str:
-        """Cancel order by order ID
+        """
+        Cancel an order by its ID.
 
-        Parameters:
-        -----------
-        order_id:   Order ID to cancel
-                    A valid order ID string required
+        Args:
+            order_id (str): The ID of the order to be cancelled.
 
         Returns:
-        --------
-        str:        Order cancellation confirmation message
+            str: A message indicating the status of the cancellation.
 
         Raises:
-        -------
-        Exception:  If failed to cancel order
-
-        Example:
-        --------
-        >>> from py_alpaca_api.alpaca import PyAlpacaApi
-            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
-            order = api.order.cancel_by_id(order_id="ORDER_ID")
-            print(order)
-
-        Order ORDER_ID has been cancelled
-        """  # noqa
+            Exception: If the cancellation request fails, an exception is raised with the error message.
+        """
 
         # Alpaca API URL for canceling an order
         url = f"{self.trade_url}/orders/{order_id}"
         # Delete request to Alpaca API for canceling an order
         response = requests.delete(url, headers=self.headers)
         # Check if response is successful
         if response.status_code == 204:
             # Convert JSON response to dictionary
             return f"Order {order_id} has been cancelled"
         # If response is not successful, raise an exception
         else:
             res = json.loads(response.text)
-            raise Exception(
-                f'Failed to cancel order {order_id}, Response: {res["message"]}'
-            )
+            raise Exception(f'Failed to cancel order {order_id}, Response: {res["message"]}')
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Cancel All Orders //////////////////#
     ########################################################
     def cancel_all(self) -> str:
-        """Cancel all orders
+        """
+        Cancels all open orders.
 
         Returns:
-        --------
-        str:        Order cancellation confirmation message
+            str: A message indicating the number of orders that have been cancelled.
 
         Raises:
-        -------
-        Exception:  If failed to cancel all orders
-
-        Example:
-        --------
-        >>> from py_alpaca_api.alpaca import PyAlpacaApi
-            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
-            order = api.order.cancel_all()
-            print(order)
-
-        10 orders have been cancelled
-        """  # noqa
-
+            Exception: If the request to cancel orders is not successful, an exception is raised with the error message.
+        """
         # Alpaca API URL for canceling all orders
         url = f"{self.trade_url}/orders"
         # Delete request to Alpaca API for canceling all orders
         response = requests.delete(url, headers=self.headers)
         # Check if response is successful
         if response.status_code == 207:
             # Convert JSON response to dictionary
             res = json.loads(response.text)
             return f"{len(res)} orders have been cancelled"
         # If response is not successful, raise an exception
         else:
             res = json.loads(response.text)
-            raise Exception(
-                f'Failed to cancel orders. Response: {res["message"]}'
-            )
+            raise Exception(f'Failed to cancel orders. Response: {res["message"]}')
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Submit Market Order ////////////////#
     ########################################################
     def market(
         self,
         symbol: str,
         qty: float = None,
         notional: float = None,
         side: str = "buy",
         time_in_force: str = "day",
         extended_hours: bool = False,
     ) -> OrderClass:
+        """
+        Submits a market order for the specified symbol.
+
+        Args:
+            symbol (str): The symbol to trade.
+            qty (float, optional): The quantity to trade. Either `qty` or `notional` must be provided, not both.
+            Defaults to None.
+            notional (float, optional): The notional value of the trade. Either `qty` or `notional` must be provided, not both.
+            Defaults to None.
+            side (str, optional): The side of the trade. Defaults to "buy".
+            time_in_force (str, optional): The time in force for the order. Defaults to "day".
+            extended_hours (bool, optional): Whether to allow trading during extended hours. Defaults to False.
+
+        Returns:
+            OrderClass: The submitted market order.
+
+        Raises:
+            ValueError: If `symbol` is not provided.
+            ValueError: If both `qty` and `notional` are not provided, or if both are provided.
+        """
 
         if not symbol:
             raise ValueError("Must provide symbol for trading.")
 
         if not (qty or notional) or (qty and notional):
             raise ValueError("Qty or Notional are required, not both.")
 
-        # Return market order using submit order method
         return self.__submit_order(
             symbol=symbol,
             side=side,
             qty=qty,
             notional=notional,
             entry_type="market",
             time_in_force=time_in_force,
@@ -222,24 +171,45 @@
         limit_price: float,
         qty: float = None,
         notional: float = None,
         side: str = "buy",
         time_in_force: str = "day",
         extended_hours: bool = False,
     ) -> OrderClass:
+        """
+        Submits a limit order for trading.
+
+        Args:
+            symbol (str): The symbol of the security to trade.
+            limit_price (float): The limit price for the order.
+            qty (float, optional): The quantity of shares to trade. Either `qty` or `notional` must be provided, not both.
+            Defaults to None.
+            notional (float, optional): The notional value of the trade. Either `qty` or `notional` must be provided, not both.
+            Defaults to None.
+            side (str, optional): The side of the order, either 'buy' or 'sell'. Defaults to 'buy'.
+            time_in_force (str, optional): The time in force for the order. Defaults to 'day'.
+            extended_hours (bool, optional): Whether to allow trading during extended hours. Defaults to False.
+
+        Returns:
+            OrderClass: The submitted limit order.
+
+        Raises:
+            ValueError: If `symbol` or `limit_price` is not provided, or if both `qty` and `notional` are provided or not provided.
+
+        """
 
         if not symbol:
             raise ValueError("Must provide symbol for trading.")
 
         if not limit_price:
             raise ValueError("Must provide limit price for trading.")
 
         if not (qty or notional) or (qty and notional):
             raise ValueError("Qty or Notional are required, not both.")
-        # Return limit order
+
         return self.__submit_order(
             symbol=symbol,
             side=side,
             limit_price=limit_price,
             qty=qty,
             notional=notional,
             entry_type="limit",
@@ -255,24 +225,41 @@
         symbol: str,
         stop_price: float,
         qty: float,
         side: str = "buy",
         time_in_force: str = "day",
         extended_hours: bool = False,
     ) -> OrderClass:
+        """
+        Submits a stop order for trading.
+
+        Args:
+            symbol (str): The symbol of the security to trade.
+            stop_price (float): The stop price for the order.
+            qty (float): The quantity of shares to trade.
+            side (str, optional): The side of the order. Defaults to "buy".
+            time_in_force (str, optional): The time in force for the order. Defaults to "day".
+            extended_hours (bool, optional): Whether to allow trading during extended hours. Defaults to False.
+
+        Returns:
+            OrderClass: The submitted stop order.
+
+        Raises:
+            ValueError: If symbol, stop_price, or qty is not provided.
+        """
 
         if not symbol:
             raise ValueError("Must provide symbol for trading.")
 
         if not stop_price:
             raise ValueError("Must provide stop price for trading.")
 
         if not qty:
             raise ValueError("Qty is required.")
-        # Return stop order
+
         return self.__submit_order(
             symbol=symbol,
             side=side,
             stop_price=stop_price,
             qty=qty,
             entry_type="stop",
             time_in_force=time_in_force,
@@ -288,24 +275,44 @@
         stop_price: float,
         limit_price: float,
         qty: float,
         side: str = "buy",
         time_in_force: str = "day",
         extended_hours: bool = False,
     ) -> OrderClass:
+        """
+        Submits a stop-limit order for trading.
+
+        Args:
+            symbol (str): The symbol of the security to trade.
+            stop_price (float): The stop price for the order.
+            limit_price (float): The limit price for the order.
+            qty (float): The quantity of shares to trade.
+            side (str, optional): The side of the order, either 'buy' or 'sell'. Defaults to 'buy'.
+            time_in_force (str, optional): The time in force for the order. Defaults to 'day'.
+            extended_hours (bool, optional): Whether to allow trading during extended hours. Defaults to False.
+
+        Returns:
+            OrderClass: The submitted stop-limit order.
+
+        Raises:
+            ValueError: If symbol is not provided.
+            ValueError: If neither limit_price nor stop_price is provided.
+            ValueError: If qty is not provided.
+        """
 
         if not symbol:
             raise ValueError("Must provide symbol for trading.")
 
         if not (limit_price or stop_price):
             raise ValueError("Must provide limit and stop price for trading.")
 
         if not qty:
             raise ValueError("Qty is required.")
-        # Return stop_limit order
+
         return self.__submit_order(
             symbol=symbol,
             side=side,
             stop_price=stop_price,
             limit_price=limit_price,
             qty=qty,
             entry_type="stop_limit",
@@ -322,36 +329,51 @@
         qty: float,
         trail_percent: float = None,
         trail_price: float = None,
         side: str = "buy",
         time_in_force: str = "day",
         extended_hours: bool = False,
     ) -> OrderClass:
+        """
+        Submits a trailing stop order for the specified symbol.
+
+        Args:
+            symbol (str): The symbol of the security to trade.
+            qty (float): The quantity of shares to trade.
+            trail_percent (float, optional): The trailing stop percentage. Either `trail_percent` or `trail_price`
+            must be provided, not both. Defaults to None.
+            trail_price (float, optional): The trailing stop price. Either `trail_percent` or `trail_price`
+            must be provided, not both. Defaults to None.
+            side (str, optional): The side of the order, either 'buy' or 'sell'. Defaults to 'buy'.
+            time_in_force (str, optional): The time in force for the order. Defaults to 'day'.
+            extended_hours (bool, optional): Whether to allow trading during extended hours. Defaults to False.
+
+        Returns:
+            OrderClass: The submitted trailing stop order.
+
+        Raises:
+            ValueError: If `symbol` is not provided.
+            ValueError: If `qty` is not provided.
+            ValueError: If both `trail_percent` and `trail_price` are provided, or if neither is provided.
+            ValueError: If `trail_percent` is less than 0.
+        """
 
         if not symbol:
             raise ValueError("Must provide symbol for trading.")
 
         if not qty:
             raise ValueError("Qty is required.")
 
-        if (
-            trail_percent is None
-            and trail_price is None
-            or trail_percent
-            and trail_price
-        ):
-            raise ValueError(
-                "Either trail_percent or trail_price must be provided, not both."
-            )
+        if trail_percent is None and trail_price is None or trail_percent and trail_price:
+            raise ValueError("Either trail_percent or trail_price must be provided, not both.")
 
         if trail_percent:
             if trail_percent < 0:
                 raise ValueError("Trail percent must be greater than 0.")
 
-        # Return trailing_stop
         return self.__submit_order(
             symbol=symbol,
             side=side,
             trail_price=trail_price,
             trail_percent=trail_percent,
             qty=qty,
             entry_type="trailing_stop",
@@ -372,14 +394,36 @@
         limit_price: float = None,
         trail_percent: float = None,
         trail_price: float = None,
         side: str = "buy",
         time_in_force: str = "day",
         extended_hours: bool = False,
     ) -> OrderClass:
+        """
+        Submits an order to the Alpaca API.
+
+        Args:
+            symbol (str): The symbol of the security to trade.
+            entry_type (str): The type of order to submit (e.g., 'market', 'limit', 'stop').
+            qty (float, optional): The quantity of shares to trade. Defaults to None.
+            notional (float, optional): The desired notional value of the trade. Defaults to None.
+            stop_price (float, optional): The stop price for a stop order. Defaults to None.
+            limit_price (float, optional): The limit price for a limit order. Defaults to None.
+            trail_percent (float, optional): The trailing stop percentage for a trailing stop order. Defaults to None.
+            trail_price (float, optional): The trailing stop price for a trailing stop order. Defaults to None.
+            side (str, optional): The side of the trade ('buy' or 'sell'). Defaults to 'buy'.
+            time_in_force (str, optional): The time in force for the order ('day', 'gtc', 'opg', 'ioc', 'fok'). Defaults to 'day'.
+            extended_hours (bool, optional): Whether to allow trading during extended hours. Defaults to False.
+
+        Returns:
+            OrderClass: An object representing the submitted order.
+
+        Raises:
+            Exception: If the order submission fails, an exception is raised with the error message.
+        """
 
         payload = {
             "symbol": symbol,
             "qty": qty if qty else None,
             "notional": round(notional, 2) if notional else None,
             "stop_price": stop_price if stop_price else None,
             "limit_price": limit_price if limit_price else None,
@@ -387,23 +431,17 @@
             "trail_price": trail_price if trail_price else None,
             "side": side if side == "buy" else "sell",
             "type": entry_type,
             "time_in_force": time_in_force,
             "extended_hours": extended_hours,
         }
 
-        # Alpaca API URL for submitting an order
         url = f"{self.trade_url}/orders"
-        # Post request to Alpaca API for submitting an order
+
         response = requests.post(url, headers=self.headers, json=payload)
-        # Check if response is successful
+
         if response.status_code == 200:
-            # Convert JSON response to dictionary
             res = json.loads(response.text)
-            # Return order information as an OrderClass object
             return order_class_from_dict(res)
-        # If response is not successful, raise an exception
         else:
             res = json.loads(response.text)
-            raise Exception(
-                f'Failed to submit order. Code: {response.status_code}, Response: {res["message"]}'
-            )
+            raise Exception(f'Failed to submit order. Code: {response.status_code}, Response: {res["message"]}')
```

### Comparing `py_alpaca_api-0.5.8/py_alpaca_api/src/screener.py` & `py_alpaca_api-0.5.9/py_alpaca_api/src/screener.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 MONDAY = pendulum.MONDAY
 TUESDAY = pendulum.TUESDAY
 FRIDAY = pendulum.FRIDAY
 THURSDAY = pendulum.THURSDAY
 
 
 class Screener:
-    def __init__(
-        self, data_url: str, headers: Dict[str, str], asset: Asset
-    ) -> None:
+    def __init__(self, data_url: str, headers: Dict[str, str], asset: Asset) -> None:
         """Initialize Screener class3
 
         Parameters:
         ___________
         data_url: str
                 Alpaca Data API URL required
 
@@ -73,27 +71,21 @@
             trade_count_greater_than=3000, total_losers_returned=50)
         """
         self.set_dates()
 
         print(f"Yesterday was {self.yesterday}")
         print(f"Day before yesterday was {self.day_before_yesterday}")
 
-        losers_df = self._get_percentages(
-            start=self.day_before_yesterday, end=self.yesterday
-        )
+        losers_df = self._get_percentages(start=self.day_before_yesterday, end=self.yesterday)
 
         losers_df = losers_df[losers_df["price"] > price_greater_than]
         losers_df = losers_df[losers_df["change"] < change_less_than]
         losers_df = losers_df[losers_df["volume"] > volume_greater_than]
         losers_df = losers_df[losers_df["trades"] > trade_count_greater_than]
-        return (
-            losers_df.sort_values(by="change", ascending=True)
-            .reset_index(drop=True)
-            .head(total_losers_returned)
-        )
+        return losers_df.sort_values(by="change", ascending=True).reset_index(drop=True).head(total_losers_returned)
 
     def gainers(
         self,
         price_greater_than: float = 5.0,
         change_greater_than: float = 2.0,
         volume_greater_than: int = 20000,
         trade_count_greater_than: int = 2000,
@@ -115,29 +107,21 @@
         Returns:
             pd.DataFrame: A DataFrame that contains the filtered gainers that satisfy the given thresholds.
             The DataFrame is sorted by the "change" column in descending order and is limited to the specified
             number of gainers.
         """
         self.set_dates()
 
-        gainers_df = self._get_percentages(
-            start=self.day_before_yesterday, end=self.yesterday
-        )
+        gainers_df = self._get_percentages(start=self.day_before_yesterday, end=self.yesterday)
 
         gainers_df = gainers_df[gainers_df["price"] > price_greater_than]
         gainers_df = gainers_df[gainers_df["change"] > change_greater_than]
         gainers_df = gainers_df[gainers_df["volume"] > volume_greater_than]
-        gainers_df = gainers_df[
-            gainers_df["trades"] > trade_count_greater_than
-        ]
-        return (
-            gainers_df.sort_values(by="change", ascending=False)
-            .reset_index(drop=True)
-            .head(total_gainers_returned)
-        )
+        gainers_df = gainers_df[gainers_df["trades"] > trade_count_greater_than]
+        return gainers_df.sort_values(by="change", ascending=False).reset_index(drop=True).head(total_gainers_returned)
 
     def _get_percentages(
         self,
         start: str,
         end: str,
         timeframe: str = "1Day",
     ) -> pd.DataFrame:
@@ -182,17 +166,15 @@
             res = json.loads(response.text)
 
             bars_df = pd.DataFrame.from_dict(res["bars"], orient="index")
             page_token = res["next_page_token"]
 
             while page_token:
                 params["page_token"] = page_token
-                response = requests.get(
-                    url, headers=self.headers, params=params
-                )
+                response = requests.get(url, headers=self.headers, params=params)
                 res = json.loads(response.text)
                 bars_df = pd.concat(
                     [
                         bars_df,
                         pd.DataFrame.from_dict(res["bars"], orient="index"),
                     ]
                 )
@@ -201,39 +183,34 @@
             bars_df.reset_index()
 
             all_bars_df = pd.DataFrame()
 
             for bar in bars_df.iterrows():
                 try:
                     change = round(
-                        ((bar[1][1]["c"] - bar[1][0]["c"]) / bar[1][0]["c"])
-                        * 100,
+                        ((bar[1][1]["c"] - bar[1][0]["c"]) / bar[1][0]["c"]) * 100,
                         2,
                     )
                     symbol = bar[0]
 
                     sym_data = {
                         "symbol": symbol,
                         "change": change,
                         "price": bar[1][1]["c"],
                         "volume": bar[1][1]["v"],
                         "trades": bar[1][1]["n"],
                     }
-                    all_bars_df = pd.concat(
-                        [all_bars_df, pd.DataFrame([sym_data])]
-                    )
+                    all_bars_df = pd.concat([all_bars_df, pd.DataFrame([sym_data])])
 
                 except Exception:
                     pass
             all_bars_df.reset_index(drop=True, inplace=True)
             return all_bars_df
         else:
-            raise ValueError(
-                f"Failed to get assets. Response: {response.text}"
-            )
+            raise ValueError(f"Failed to get assets. Response: {response.text}")
 
     @staticmethod
     def get_previous_date(current_date, day_to_look):
         """
         Get the previous date based on the day_to_look from the current_date.
         """
         return current_date.previous(day_to_look).strftime("%Y-%m-%d")
@@ -256,13 +233,9 @@
         if today.day_of_week in [SUNDAY, MONDAY]:
             self.yesterday = self.get_previous_date(today, FRIDAY)
             self.day_before_yesterday = self.get_previous_date(today, THURSDAY)
         elif today.day_of_week == TUESDAY:
             self.yesterday = self.get_previous_date(today, MONDAY)
             self.day_before_yesterday = self.get_previous_date(today, FRIDAY)
         else:
-            self.yesterday = self.get_previous_date(
-                today, today.day_of_week - 1
-            )
-            self.day_before_yesterday = self.get_previous_date(
-                today, today.day_of_week - 2
-            )
+            self.yesterday = self.get_previous_date(today, today.day_of_week - 1)
+            self.day_before_yesterday = self.get_previous_date(today, today.day_of_week - 2)
```

### Comparing `py_alpaca_api-0.5.8/py_alpaca_api/src/watchlist.py` & `py_alpaca_api-0.5.9/py_alpaca_api/src/watchlist.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,17 +21,15 @@
         self.trade_url = trade_url
         self.headers = headers
 
     ########################################################
     # ///////////// Helper functions //////////////////////#
     ########################################################
     @staticmethod
-    def _handle_response(
-        response: dict, no_content_msg: str
-    ) -> Union[WatchlistClass, str]:
+    def _handle_response(response: dict, no_content_msg: str) -> Union[WatchlistClass, str]:
         """
         Handles the response from the API and returns a WatchlistClass object
         if the response is not empty, otherwise returns the specified no_content_msg.
 
         Args:
             response (dict): The response from the API.
             no_content_msg (str): The message to return if the response is empty.
@@ -43,17 +41,15 @@
             return watchlist_class_from_dict(response)
         else:
             return no_content_msg
 
     ########################################################
     # ///////////// Send a request to the API //////////////#
     ########################################################
-    def _request(
-        self, method: str, url: str, payload: dict = None, params: dict = None
-    ) -> Dict:
+    def _request(self, method: str, url: str, payload: dict = None, params: dict = None) -> Dict:
         """
         Sends a request to the specified URL using the specified HTTP method.
 
         Args:
             method (str): The HTTP method to use for the request (e.g., 'GET', 'POST', 'PUT', 'DELETE').
             url (str): The URL to send the request to.
             payload (dict, optional): The payload to include in the request body. Defaults to None.
@@ -78,49 +74,41 @@
             return {}
         else:
             raise Exception(response.text)
 
     ########################################################
     # //////////////// Get a  watchlist ///////////////////#
     ########################################################
-    def get(
-        self, watchlist_id: str = None, watchlist_name: str = None
-    ) -> WatchlistClass:
+    def get(self, watchlist_id: str = None, watchlist_name: str = None) -> WatchlistClass:
         """
         Retrieves a watchlist based on the provided watchlist ID or name.
 
         Args:
             watchlist_id (str, optional): The ID of the watchlist to retrieve.
             watchlist_name (str, optional): The name of the watchlist to retrieve.
 
         Returns:
             WatchlistClass: The retrieved watchlist.
 
         Raises:
             ValueError: If both watchlist_id and watchlist_name are provided, or if neither is provided.
 
         """
-        if (
-            watchlist_id
-            and watchlist_name
-            or (not watchlist_id and not watchlist_name)
-        ):
+        if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
             raise ValueError("Watchlist ID or Name is required, not both.")
 
         if watchlist_id:
             url = f"{self.trade_url}/watchlists/{watchlist_id}"
         else:
             url = f"{self.trade_url}/watchlists:by_name"
 
         params = {"name": watchlist_name} if watchlist_name else None
 
         response = self._request(method="GET", url=url, params=params)
-        return self._handle_response(
-            response=response, no_content_msg="No watchlist was found."
-        )
+        return self._handle_response(response=response, no_content_msg="No watchlist was found.")
 
     ########################################################
     # ///////////// Get all watchlists ////////////////////#
     ########################################################
     def get_all(self) -> list[WatchlistClass]:
         """
         Retrieves all watchlists.
@@ -165,17 +153,15 @@
         # Create the URL
         url = f"{self.trade_url}/watchlists"
         # Split the symbols and remove any spaces
         symbols = symbols.replace(" ", "").split(",") if symbols else []
 
         payload = {"symbols": symbols, "name": name}
         response = self._request(method="POST", url=url, payload=payload)
-        return self._handle_response(
-            response=response, no_content_msg="The watchlist was not created."
-        )
+        return self._handle_response(response=response, no_content_msg="The watchlist was not created.")
 
     ########################################################
     # ///////////// Update a watchlist ////////////////////#
     ########################################################
     def update(
         self,
         watchlist_id: str = None,
@@ -197,19 +183,15 @@
             WatchlistClass: The updated watchlist.
 
         Raises:
             ValueError: If both `watchlist_id` and `watchlist_name` are provided, or if neither `watchlist_id` nor `watchlist_name` are provided.
 
         """
         # Check if both watchlist_id and watchlist_name are provided and raise an error if they are
-        if (
-            watchlist_id
-            and watchlist_name
-            or (not watchlist_id and not watchlist_name)
-        ):
+        if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
             raise ValueError("Watchlist ID or Name is required, not both.")
         # Check if watchlist_id is provided
         if watchlist_id:
             watchlist = self.get(watchlist_id=watchlist_id)
             url = f"{self.trade_url}/watchlists/{watchlist_id}"
         else:
             watchlist = self.get(watchlist_name=watchlist_name)
@@ -221,46 +203,36 @@
             symbols = symbols.replace(" ", "").split(",")
         else:
             symbols = ",".join([o.symbol for o in watchlist.assets])
 
         payload = {"name": name, "symbols": symbols}
         params = {"name": watchlist_name} if watchlist_name else None
 
-        response = self._request(
-            method="PUT", url=url, payload=payload, params=params
-        )
-        return self._handle_response(
-            response=response, no_content_msg="The watchlist was not updated."
-        )
+        response = self._request(method="PUT", url=url, payload=payload, params=params)
+        return self._handle_response(response=response, no_content_msg="The watchlist was not updated.")
 
     ########################################################
     # ///////////// Delete a watchlist ////////////////////#
     ########################################################
-    def delete(
-        self, watchlist_id: str = None, watchlist_name: str = None
-    ) -> str:
+    def delete(self, watchlist_id: str = None, watchlist_name: str = None) -> str:
         """
         Deletes a watchlist.
 
         Args:
             watchlist_id (str, optional): The ID of the watchlist to delete.
             watchlist_name (str, optional): The name of the watchlist to delete.
 
         Returns:
             str: A message indicating the successful deletion of the watchlist.
 
         Raises:
             ValueError: If both watchlist_id and watchlist_name are provided or if neither is provided.
 
         """
-        if (
-            watchlist_id
-            and watchlist_name
-            or (not watchlist_id and not watchlist_name)
-        ):
+        if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
             raise ValueError("Watchlist ID or Name is required, not both.")
 
         if watchlist_id:
             url = f"{self.trade_url}/watchlists/{watchlist_id}"
         else:
             url = f"{self.trade_url}/watchlists:by_name"
 
@@ -291,35 +263,29 @@
 
         Returns:
             WatchlistClass: The updated watchlist object.
 
         Raises:
             ValueError: If both watchlist_id and watchlist_name are provided, or if symbol is not provided.
         """
-        if (
-            watchlist_id
-            and watchlist_name
-            or (not watchlist_id and not watchlist_name)
-        ):
+        if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
             raise ValueError("Watchlist ID or Name is required, not both.")
 
         if not symbol:
             raise ValueError("Symbol is required")
 
         if watchlist_id:
             url = f"{self.trade_url}/watchlists/{watchlist_id}"
         else:
             url = f"{self.trade_url}/watchlists:by_name"
 
         params = {"name": watchlist_name} if watchlist_name else None
         payload = {"symbol": symbol}
 
-        response = self._request(
-            method="POST", url=url, payload=payload, params=params
-        )
+        response = self._request(method="POST", url=url, payload=payload, params=params)
         return self._handle_response(
             response=response,
             no_content_msg="Failed to add asset to watchlist.",
         )
 
     ########################################################
     # /////////// Remove a Asset from  watchlist //////////#
@@ -342,19 +308,15 @@
 
         Returns:
             WatchlistClass: The updated watchlist object.
 
         Raises:
             ValueError: If both watchlist_id and watchlist_name are provided, or if symbol is not provided.
         """
-        if (
-            watchlist_id
-            and watchlist_name
-            or (not watchlist_id and not watchlist_name)
-        ):
+        if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
             raise ValueError("Watchlist ID or Name is required, not both.")
 
         if not symbol:
             raise ValueError("Symbol is required")
 
         if not watchlist_id:
             watchlist_id = self.get(watchlist_name=watchlist_name).id
@@ -366,17 +328,15 @@
             response=response,
             no_content_msg="Failed to remove asset from watchlist.",
         )
 
     ########################################################
     # /////////// Get Assets from a watchlist /////////////#
     ########################################################
-    def get_assets(
-        self, watchlist_id: str = None, watchlist_name: str = None
-    ) -> list:
+    def get_assets(self, watchlist_id: str = None, watchlist_name: str = None) -> list:
         """
         Retrieves the symbols of assets in a watchlist.
 
         Args:
             watchlist_id (str, optional): The ID of the watchlist. Either `watchlist_id` or `watchlist_name` should be provided,
             not both. Defaults to None.
             watchlist_name (str, optional): The name of the watchlist. Either `watchlist_id` or `watchlist_name` should be
```

### Comparing `py_alpaca_api-0.5.8/pyproject.toml` & `py_alpaca_api-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.5.8"
+version = "0.5.9"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
```

### Comparing `py_alpaca_api-0.5.8/PKG-INFO` & `py_alpaca_api-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
```

