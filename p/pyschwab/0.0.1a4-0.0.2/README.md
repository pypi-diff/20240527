# Comparing `tmp/pyschwab-0.0.1a4.tar.gz` & `tmp/pyschwab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyschwab-0.0.1a4.tar", max compression
+gzip compressed data, was "pyschwab-0.0.2.tar", max compression
```

## Comparing `pyschwab-0.0.1a4.tar` & `pyschwab-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-05-24 18:04:34.866068 pyschwab-0.0.1a4/LICENSE
--rw-r--r--   0        0        0     3628 2024-05-24 18:04:34.866068 pyschwab-0.0.1a4/README.md
--rw-r--r--   0        0        0     1033 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/__init__.py
--rw-r--r--   0        0        0     5685 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/auth.py
--rw-r--r--   0        0        0     1049 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/exceptions.py
--rw-r--r--   0        0        0      372 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/log.py
--rw-r--r--   0        0        0     5736 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/market.py
--rw-r--r--   0        0        0    13261 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/market_models.py
--rw-r--r--   0        0        0    10612 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/trading.py
--rw-r--r--   0        0        0    19645 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/trading_models.py
--rw-r--r--   0        0        0     9711 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/types.py
--rw-r--r--   0        0        0     1013 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/user_input.py
--rw-r--r--   0        0        0     7131 2024-05-24 18:04:34.870069 pyschwab-0.0.1a4/pyschwab/utils.py
--rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 pyschwab-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-27 03:12:40.712567 pyschwab-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4621 2024-05-27 03:12:40.712567 pyschwab-0.0.2/README.md
+-rw-r--r--   0        0        0     1031 2024-05-27 03:12:40.712567 pyschwab-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 03:12:40.712567 pyschwab-0.0.2/pyschwab/__init__.py
+-rw-r--r--   0        0        0     5685 2024-05-27 03:12:40.712567 pyschwab-0.0.2/pyschwab/auth.py
+-rw-r--r--   0        0        0     1049 2024-05-27 03:12:40.712567 pyschwab-0.0.2/pyschwab/exceptions.py
+-rw-r--r--   0        0        0      372 2024-05-27 03:12:40.712567 pyschwab-0.0.2/pyschwab/log.py
+-rw-r--r--   0        0        0     5736 2024-05-27 03:12:40.712567 pyschwab-0.0.2/pyschwab/market.py
+-rw-r--r--   0        0        0    13261 2024-05-27 03:12:40.712567 pyschwab-0.0.2/pyschwab/market_models.py
+-rw-r--r--   0        0        0    14477 2024-05-27 03:12:40.712567 pyschwab-0.0.2/pyschwab/trading.py
+-rw-r--r--   0        0        0    19797 2024-05-27 03:12:40.716567 pyschwab-0.0.2/pyschwab/trading_models.py
+-rw-r--r--   0        0        0    11169 2024-05-27 03:12:40.716567 pyschwab-0.0.2/pyschwab/types.py
+-rw-r--r--   0        0        0     1013 2024-05-27 03:12:40.716567 pyschwab-0.0.2/pyschwab/user_input.py
+-rw-r--r--   0        0        0     7728 2024-05-27 03:12:40.716567 pyschwab-0.0.2/pyschwab/utils.py
+-rw-r--r--   0        0        0     5671 1970-01-01 00:00:00.000000 pyschwab-0.0.2/PKG-INFO
```

### Comparing `pyschwab-0.0.1a4/LICENSE` & `pyschwab-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a4/README.md` & `pyschwab-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -20,23 +20,27 @@
 
 ## Preparation
 
 1. Change directory to your project directory
 2. Copy [pyschwab.yaml](https://github.com/hzheng/pyschwab/blob/main/config/pyschwab.yaml) to your project's `config` directory.
 3. Copy [env_example](https://github.com/hzheng/pyschwab/blob/main/env_example) to `.env` and replace the placeholders with your settings.
 
+## Warning
+**WARNING**: This library can place real orders on your Schwab brokerage account. Use this API at your own risk. The author and contributors are not responsible for any financial losses or unintended trades that may occur as a result of using this library. Ensure you fully understand the functionality and risks before using it in a live trading environment.
+
 ## Usage
 
 Here are some sample usages:
 
 ```python
 import yaml
 
 from pyschwab.auth import Authorizer
 from pyschwab.trading import TradingApi
+from pyschwab.types import Symbol
 from pyschwab.market import MarketApi
 
 # Load configuration
 with open("config/pyschwab.yaml", 'r') as file:
     app_config = yaml.safe_load(file)
 
 # Authorization
@@ -46,28 +50,36 @@
 authorizer = Authorizer(app_config['auth'])
 
 access_token = authorizer.get_access_token()
 print(access_token)
 
 # Example usage of trading APIs
 trading_api = TradingApi(access_token, app_config['trading'])
-
-account_num = 0 # CHANGE this to your actual account number
-trading_api.set_current_account_number(account_num)
 trading_data = trading_api.fetch_trading_data()
 # List positions
 for position in trading_data.positions:
     print("position:", position)
 
 # List transactions 
 for transaction in trading_api.get_transactions():
     print("transaction:", transaction)
 
-# Place order
-trading_api.buy_equity("TSLA", quantity=1, price=100)
+# Buy/Sell equity
+trading_api.buy_equity("TSLA", quantity=10, price=100)
+trading_api.sell_equity("TSLA", quantity=10, price=200)
+
+# Buy/Sell option
+symbol = Symbol("RDDT", expiration="260116", call_put=True, strike=50.00)
+trading_api.buy_single_option(symbol, quantity=1, price=10)
+# Or: trading_api.buy_option("RDDT  260116C00050000", quantity=1, price=10)
+
+trading_api.sell_single_option(symbol, quantity=1, price=30)
+
+# Buy Call Spread
+trading_api.trade_spread("TSLA", 0.9,  "2024-05-31", buy_sell=True, call_put=True, strikes=[177.5, 180], quantity=1)
 
 # List orders
 for order in trading_api.get_orders():
     print("order:", order)
 
 # Example usage of market APIs
 market_api = MarketApi(access_token, app_config['market'])
@@ -83,14 +95,24 @@
 print(option_chain)
 
 # Get price history 
 history = market_api.get_price_history('TSLA')
 print(history)
 ```
 
+## Tests
+
+To run the tests, use the following command:
+
+```bash
+pytest -s
+```
+
+You can customize the tests by editing the `test_api.json` file. Each test case has enabled/dry_run attribute that you can toggle. 
+
 ---
 
 ## License
 
 MIT License
 
 ```
```

### Comparing `pyschwab-0.0.1a4/pyproject.toml` & `pyschwab-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyschwab"
-version = "0.0.1a4"
+version = "0.0.2"
 description = "A Python library for the Schwab trading API"
 authors = ["Hui Zheng <xyz.dll@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hzheng/pyschwab"
 documentation = "https://pyschwab.readthedocs.io"
 keywords = ["finance", "trading", "schwab", "api", "python"]
```

### Comparing `pyschwab-0.0.1a4/pyschwab/auth.py` & `pyschwab-0.0.2/pyschwab/auth.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a4/pyschwab/exceptions.py` & `pyschwab-0.0.2/pyschwab/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a4/pyschwab/market.py` & `pyschwab-0.0.2/pyschwab/market.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a4/pyschwab/market_models.py` & `pyschwab-0.0.2/pyschwab/market_models.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a4/pyschwab/trading.py` & `pyschwab-0.0.2/pyschwab/trading.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from datetime import datetime, timedelta
 from typing import Any, Dict, List
 
 from dotenv import load_dotenv
 
-from .utils import format_params, remove_none_values, request, time_to_str, to_json_str
-from .trading_models import Instrument, Order, OrderLeg, SecuritiesAccount, TradingData, Transaction, UserPreference
-from .types import AssetType, ExecutionType, MarketSession, OrderDuration, OrderInstruction, OrderStatus, OrderStrategyType, OrderType, TransactionType
+from .utils import format_params, remove_none_values, request, time_to_str, to_date, to_json_str
+from .trading_models import AccountInfo, Instrument, Order, OrderLeg, SecuritiesAccount, TradingData, Transaction, UserPreference
+from .types import AssetType, ExecutionType, MarketSession, OrderDuration, OrderInstruction, OrderStatus, \
+    OrderStrategyType, OrderType, Symbol, TransactionType
 
 
 """
 Schwab Trading API
 
 Reference: https://developer.schwab.com/products/trader-api--individual/details/specifications/Retail%20Trader%20API%20Production
 """
@@ -17,69 +18,90 @@
     base_trader_url: str
 
     def __init__(self, access_token: str, trading_config: Dict[str, Any]):
         load_dotenv()
         self.base_trader_url = trading_config['base_trader_url']
         self.auth = {'Authorization': f'Bearer {access_token}'}
         self.auth2 = {**self.auth, 'Content-Type': 'application/json'}
-        response = request(f'{self.base_trader_url}/accounts/accountNumbers', headers=self.auth).json()
-        self.accounts_hash = {account.get('accountNumber'): account.get('hashValue') for account in response}
-        self.accounts: Dict[str, SecuritiesAccount] = {}
         self.current_account_num = None
+        self.primary_account_num = None
+        self.securities_accounts: Dict[str, SecuritiesAccount] = {}
+        self.accounts_info: Dict[str, AccountInfo] = {}
+        self._init_accounts()
+
+    def _init_accounts(self) -> None:
+        response = request(f'{self.base_trader_url}/accounts/accountNumbers', headers=self.auth).json()
+        accounts_hash = {account.get('accountNumber'): account.get('hashValue') for account in response}
+        for account in self.get_user_preference().accounts:
+            account_num = account.account_number
+            account_hash = accounts_hash.get(account_num, None)
+            is_primary = account.primary_account
+            self.accounts_info[account_num] = AccountInfo(account_number=account_num,
+                                                          account_hash=account_hash,
+                                                          is_primary=is_primary,
+                                                          type=account.type,
+                                                          nick_name=account.nick_name,
+                                                          display_id=account.display_acct_id)
+            if is_primary:
+                self.current_account_num = self.primary_account_num = account_num
+ 
+    def get_accounts_info(self) -> Dict[str, AccountInfo]:
+        return self.accounts_info
+ 
+    def get_account_info(self, account_num: int | str) -> AccountInfo:
+        account_info = self.accounts_info.get(str(account_num), None)
+        if account_info is None:
+            raise ValueError(f"Account number {account_num} not found.")
+
+        return account_info
  
-    def get_accounts_hash(self) -> Dict[str, str]:
-        return self.accounts_hash
- 
-    def set_current_account_number(self, account_number: str) -> None:
-        self.current_account_num = account_number
+    def set_current_account_number(self, account_number: str=None) -> None:
+        """Set the current account number. If not provided, it will be set to primary account's number."""
+        self.current_account_num = account_number or self.primary_account_num
 
     def get_current_account_number(self) -> str:
+        """Get the current account number. Initially it's primary account's number"""
         return self.current_account_num
 
-    def get_account_hash(self, account_number: str=None) -> str:
-        return self.accounts_hash.get(account_number or self.current_account_num, None)
- 
-    def get_accounts(self) -> Dict[str, SecuritiesAccount]:
-        return self.accounts
+    def get_securities_accounts(self) -> Dict[str, SecuritiesAccount]:
+        return self.securities_accounts
  
-    def get_account(self, account_number: str=None) -> SecuritiesAccount:
-        return self.accounts.get(account_number or self.current_account_num, None)
+    def get_securities_account(self, account_number: str=None) -> SecuritiesAccount:
+        return self.securities_accounts.get(account_number or self.current_account_num, None)
 
     def _get_account_hash(self, account_num: int | str=None) -> str:
         account_num = account_num or self.current_account_num
         if not account_num:
             raise ValueError("Account number not set")
 
-        account_hash = self.accounts_hash.get(str(account_num), None)
-        if account_hash is None:
-            raise ValueError(f"Account number {account_num} not found.")
-        return account_hash
+        account_info = self.get_account_info(account_num)
+        return account_info.account_hash
  
-    def get_user_preference(self):
+    def get_user_preference(self) -> UserPreference:
         response = request(f'{self.base_trader_url}/userPreference', headers=self.auth).json()
         return UserPreference.from_dict(response)
 
     def fetch_trading_data(self, include_pos: bool=True) -> TradingData:
         account_hash = self._get_account_hash()
         params = {'fields': ['positions'] if include_pos else []}
         resp = request(f'{self.base_trader_url}/accounts/{account_hash}', headers=self.auth, params=params).json()
         trading_data = TradingData.from_dict(resp)
         account = trading_data.account
-        self.accounts[account.account_number] = account
+        self.securities_accounts[account.account_number] = account
         return trading_data
 
     def fetch_all_trading_data(self, include_pos: bool=True) -> Dict[str, TradingData]:
         params = {'fields': ['positions'] if include_pos else []}
         trading_data_map = {}
         for resp in request(f'{self.base_trader_url}/accounts/', headers=self.auth, params=params).json():
             trading_data = TradingData.from_dict(resp)
             account = trading_data.account
             account_num = account.account_number
             trading_data_map[account_num] = trading_data
-            self.accounts[account_num] = account
+            self.securities_accounts[account_num] = account
         return trading_data_map
 
     def get_all_orders(self, start_time: datetime=None, end_time: datetime=None, status: OrderStatus=None, max_results: int=None) -> List[Order]:
         now = datetime.now()
         start = time_to_str(start_time or now - timedelta(days=60))
         end = time_to_str(end_time or now + timedelta(days=1))
         params = {'maxResults': max_results, 'fromEnteredTime': start, 'toEnteredTime': end, 'status': status}
@@ -102,16 +124,19 @@
 
         activities = order.order_activity_collection
         if activities:
             if activities[0].execution_type == ExecutionType.CANCELED:
                 return False
         return order.cancel_time is None
 
-    def get_working_orders(self, start_time: datetime=None, end_time: datetime=None) -> List[Order]:
-        return self.get_orders(start_time, end_time, status=OrderStatus.WORKING)
+    def get_open_orders(self, start_time: datetime=None, end_time: datetime=None) -> List[Order]:
+        orders = []
+        for status in [OrderStatus.WORKING, OrderStatus.PENDING_ACTIVATION]:
+            orders.extend(self.get_orders(start_time, end_time, status=status))
+        return orders
 
     def get_order(self, order_id: str, account_num: int | str=None) -> Order:
         account_hash = self._get_account_hash(account_num)
         order = request(f'{self.base_trader_url}/accounts/{account_hash}/orders/{order_id}', headers=self.auth).json()
         return Order.from_dict(order)
 
     def place_order(self, order: Dict[str, Any] | Order) -> None:
@@ -139,14 +164,47 @@
         self.place_single_order(symbol=symbol, quantity=quantity, price=price, instruction=OrderInstruction.BUY,
                                 order_type=order_type, duration=duration, session=session)
  
     def sell_equity(self, symbol: str, price: float, quantity: int, order_type: OrderType=OrderType.LIMIT,
                    duration: OrderDuration=OrderDuration.DAY, session: MarketSession=MarketSession.NORMAL) -> None:
         self.place_single_order(symbol=symbol, quantity=quantity, price=price, instruction=OrderInstruction.SELL,
                                 order_type=order_type, duration=duration, session=session)
+ 
+    def buy_single_option(self, symbol: Symbol | str, quantity: int, price: float, order_type: OrderType=OrderType.LIMIT,
+                          duration: OrderDuration=OrderDuration.DAY, session: MarketSession=MarketSession.NORMAL) -> None:
+        self.place_single_order(symbol=str(symbol), quantity=quantity, price=price, instruction=OrderInstruction.BUY_TO_OPEN,
+                                asset_type=AssetType.OPTION, order_type=order_type, duration=duration, session=session)
+ 
+    def sell_single_option(self, symbol: Symbol | str, quantity: int, price: float, order_type: OrderType=OrderType.LIMIT,
+                           duration: OrderDuration=OrderDuration.DAY, session: MarketSession=MarketSession.NORMAL) -> None:
+        self.place_single_order(symbol=str(symbol), quantity=quantity, price=price, instruction=OrderInstruction.SELL_TO_CLOSE,
+                                asset_type=AssetType.OPTION, order_type=order_type, duration=duration, session=session)
+ 
+    def trade_spread(self, underlying: str, price: float, expiration: datetime | str, buy_sell: bool, call_put: bool, strikes: List[float], quantity: int,
+                    duration: OrderDuration=OrderDuration.DAY, session: MarketSession=MarketSession.NORMAL) -> None:
+        if len(strikes) != 2:
+            raise ValueError("Must provide 2 strikes for a spread order.")
+
+        if buy_sell ^ call_put: # For bear call spreads and bull put spreads, reverse the order
+            strikes.reverse()
+        else:
+            strikes.sort()
+        order_type = OrderType.NET_DEBIT if buy_sell else OrderType.NET_CREDIT
+        instructions = [OrderInstruction.BUY_TO_OPEN, OrderInstruction.SELL_TO_OPEN]
+        
+        expiration_dt = to_date(expiration)
+        leg_collection = []
+        for i in range(2):
+            symbol = Symbol(underlying, expiration=expiration_dt, call_put=call_put, strike=strikes[i])
+            instrument = Instrument(symbol=str(symbol), asset_type=AssetType.OPTION)
+            leg = OrderLeg(instrument=instrument, quantity=quantity, instruction=instructions[i])
+            leg_collection.append(leg)
+        order = Order(price=price, order_leg_collection=leg_collection, order_strategy_type=OrderStrategyType.SINGLE,
+                      order_type=order_type, duration=duration, session=session)
+        self.place_order(order)
 
     def cancel_order(self, order_id: int | str) -> None:
         account_hash = self._get_account_hash()
         request(f'{self.base_trader_url}/accounts/{account_hash}/orders/{order_id}', method='DELETE', headers=self.auth)
 
     def replace_order(self, order: Dict[str, Any] | Order) -> None:
         order_dict = self._convert_order(order)
```

### Comparing `pyschwab-0.0.1a4/pyschwab/trading_models.py` & `pyschwab-0.0.2/pyschwab/trading_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -514,7 +514,17 @@
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> 'Offer':
         converted_data = {camel_to_snake(key): value for key, value in data.items()}
         converted_data['accounts'] = [Account.from_dict(account) for account in converted_data['accounts']]
         converted_data['streamer_info'] = [StreamerInfo.from_dict(streamer) for streamer in converted_data['streamer_info']]
         converted_data['offers'] = [Offer.from_dict(offer) for offer in converted_data['offers']]
         return cls(**converted_data)
+
+
+@dataclass
+class AccountInfo:
+    account_number: str
+    account_hash: str
+    is_primary: bool
+    type: str
+    nick_name: str
+    display_id: str
```

### Comparing `pyschwab-0.0.1a4/pyschwab/types.py` & `pyschwab-0.0.2/pyschwab/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from enum import Enum, auto
 from typing import Optional, Type, TypeVar
 
 from pydantic import BaseModel, Field, field_validator, model_validator
 
 
 class PeriodFrequency(BaseModel):
@@ -92,14 +93,55 @@
             if not valid_frequency:
                 raise ValueError(f'Invalid frequency type: {frequency_type}')
             if v not in valid_frequency:
                 raise ValueError(f'Invalid frequency for frequency_type {frequency_type}, must be one of: {valid_frequency}')
         return v
 
 
+class Symbol(BaseModel):
+    underlying: str = Field(max_length=6)
+    expiration: datetime
+    call_put: bool
+    strike: float
+
+    def __init__(self, underlying: str, **data):
+        super().__init__(underlying=underlying, **data)
+
+    @field_validator('underlying', mode='before')
+    def validate_underlying(cls, v):
+        if len(v) > 6:
+            raise ValueError("Underlying symbol cannot be more than 6 characters")
+        return v
+
+    @field_validator('expiration', mode='before')
+    def validate_expiration(cls, v):
+        if isinstance(v, str):
+            return datetime.strptime(v, '%y%m%d')
+        return v
+
+    @field_validator('call_put', mode='before')
+    def validate_call_put(cls, v):
+        if not isinstance(v, bool):
+            raise ValueError("Call/Put must be a boolean")
+        return v
+
+    @field_validator('strike', mode='before')
+    def validate_strike(cls, v):
+        if not (0 <= v <= 99999.999):
+            raise ValueError("Strike price must be between 0 and 99999.999")
+        return v
+
+    def __str__(self):
+        underlying_padded = self.underlying.ljust(6)
+        expiration_formatted = self.expiration.strftime('%y%m%d')
+        call_put_formatted = 'C' if self.call_put else 'P'
+        strike_formatted = f"{int(self.strike * 1000):08d}"
+        return f"{underlying_padded}{expiration_formatted}{call_put_formatted}{strike_formatted}"
+
+
 T = TypeVar('T', bound='AutoName')
 
 
 class AutoName(Enum):
     @staticmethod
     def _generate_next_value_(name, start, count, last_values):
         return name
@@ -173,14 +215,15 @@
     SINGLE = auto()
     CANCEL = auto()
     RECALL = auto()
     PAIR = auto()
     FLATTEN = auto()
     TWO_DAY_SWAP = auto()
     BLAST_ALL = auto()
+    # One Cancels Another
     OCO = auto()
     TRIGGER = auto()
 
 
 class ComplexOrderStrategyType(AutoName):
     NONE = auto()
     COVERED = auto()
```

### Comparing `pyschwab-0.0.1a4/pyschwab/user_input.py` & `pyschwab-0.0.2/pyschwab/user_input.py`

 * *Files identical despite different names*

### Comparing `pyschwab-0.0.1a4/pyschwab/utils.py` & `pyschwab-0.0.2/pyschwab/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,14 +116,24 @@
 
     if isinstance(dt, str):
         return datetime.fromisoformat(dt)
  
     raise ValueError("Invalid datetime format.")
 
 
+def to_date(dt: datetime | str) -> datetime:
+    if dt is None or isinstance(dt, datetime):
+        return dt
+
+    if isinstance(dt, str):
+        return datetime.strptime(dt, '%Y-%m-%d')
+ 
+    raise ValueError("Invalid datetime format.")
+
+
 def next_sunday():
     today = datetime.now()
     days_until_sunday = (6 - today.weekday()) % 7
     days_until_sunday = 7 if days_until_sunday == 0 else days_until_sunday
     return today + timedelta(days=days_until_sunday)
 
 
@@ -134,14 +144,22 @@
     while True:
         if next_day.weekday() not in [5, 6] and next_day not in us_holidays:
             return next_day
 
         next_day += timedelta(days=1)
 
 
+def is_market_closed(dt: datetime=None) -> bool:
+    dt = dt if dt else datetime.now()
+    if dt.weekday() in [5, 6]:
+        return True
+
+    return dt in holidays.US(years=[dt.year, dt.year + 1])
+
+
 def format_param(param: Any) -> str | List[str]:
     if param is None:
         return ""
 
     if isinstance(param, Enum):
         return param.value
 
@@ -204,22 +222,32 @@
         if isinstance(obj, datetime) or isinstance(obj, date):
             return obj.isoformat()
 
         return obj 
 
     return json.dumps(obj, default=json_encode)
 
+
+def get_message(msg: str):
+    try:
+        return json.loads(msg)['message']
+    except Exception:
+        return msg
+
+
 def request(url, method='GET', headers=None, params=None, data=None, json=None) -> requests.Response:
     try:
         response = requests.request(method=method, url=url, headers=headers, params=params, data=data, json=json)
         response.raise_for_status()  # Raises an HTTPError for bad responses
         return response
     except requests.exceptions.HTTPError as e:
+        message = get_message(response.text)
+        error_msg = f"{response.status_code} {response.reason} - {message}"
         if 400 <= response.status_code < 500:
-            raise BadRequestException(f"Client error: {response.status_code} {response.reason}")
+            raise BadRequestException(f"Client error: {error_msg}")
         if 500 <= response.status_code < 600:
-            raise ServerErrorException(f"Server error: {response.status_code} {response.reason}")
-        raise HTTPErrorException(f"HTTP error {response.status_code}: {response.reason}")
+            raise ServerErrorException(f"Server error: {error_msg}")
+        raise HTTPErrorException(f"HTTP error: {error_msg}")
     except requests.exceptions.ConnectionError:
         raise InternetConnectionException("Check your internet connection.")
     except requests.exceptions.RequestException as e:
         raise BrokerAPIException(f"An error occurred while making a request: {str(e)}")
```

### Comparing `pyschwab-0.0.1a4/PKG-INFO` & `pyschwab-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyschwab
-Version: 0.0.1a4
+Version: 0.0.2
 Summary: A Python library for the Schwab trading API
 Home-page: https://github.com/hzheng/pyschwab
 License: MIT
 Keywords: finance,trading,schwab,api,python
 Author: Hui Zheng
 Author-email: xyz.dll@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -47,23 +47,27 @@
 
 ## Preparation
 
 1. Change directory to your project directory
 2. Copy [pyschwab.yaml](https://github.com/hzheng/pyschwab/blob/main/config/pyschwab.yaml) to your project's `config` directory.
 3. Copy [env_example](https://github.com/hzheng/pyschwab/blob/main/env_example) to `.env` and replace the placeholders with your settings.
 
+## Warning
+**WARNING**: This library can place real orders on your Schwab brokerage account. Use this API at your own risk. The author and contributors are not responsible for any financial losses or unintended trades that may occur as a result of using this library. Ensure you fully understand the functionality and risks before using it in a live trading environment.
+
 ## Usage
 
 Here are some sample usages:
 
 ```python
 import yaml
 
 from pyschwab.auth import Authorizer
 from pyschwab.trading import TradingApi
+from pyschwab.types import Symbol
 from pyschwab.market import MarketApi
 
 # Load configuration
 with open("config/pyschwab.yaml", 'r') as file:
     app_config = yaml.safe_load(file)
 
 # Authorization
@@ -73,28 +77,36 @@
 authorizer = Authorizer(app_config['auth'])
 
 access_token = authorizer.get_access_token()
 print(access_token)
 
 # Example usage of trading APIs
 trading_api = TradingApi(access_token, app_config['trading'])
-
-account_num = 0 # CHANGE this to your actual account number
-trading_api.set_current_account_number(account_num)
 trading_data = trading_api.fetch_trading_data()
 # List positions
 for position in trading_data.positions:
     print("position:", position)
 
 # List transactions 
 for transaction in trading_api.get_transactions():
     print("transaction:", transaction)
 
-# Place order
-trading_api.buy_equity("TSLA", quantity=1, price=100)
+# Buy/Sell equity
+trading_api.buy_equity("TSLA", quantity=10, price=100)
+trading_api.sell_equity("TSLA", quantity=10, price=200)
+
+# Buy/Sell option
+symbol = Symbol("RDDT", expiration="260116", call_put=True, strike=50.00)
+trading_api.buy_single_option(symbol, quantity=1, price=10)
+# Or: trading_api.buy_option("RDDT  260116C00050000", quantity=1, price=10)
+
+trading_api.sell_single_option(symbol, quantity=1, price=30)
+
+# Buy Call Spread
+trading_api.trade_spread("TSLA", 0.9,  "2024-05-31", buy_sell=True, call_put=True, strikes=[177.5, 180], quantity=1)
 
 # List orders
 for order in trading_api.get_orders():
     print("order:", order)
 
 # Example usage of market APIs
 market_api = MarketApi(access_token, app_config['market'])
@@ -110,14 +122,24 @@
 print(option_chain)
 
 # Get price history 
 history = market_api.get_price_history('TSLA')
 print(history)
 ```
 
+## Tests
+
+To run the tests, use the following command:
+
+```bash
+pytest -s
+```
+
+You can customize the tests by editing the `test_api.json` file. Each test case has enabled/dry_run attribute that you can toggle. 
+
 ---
 
 ## License
 
 MIT License
 
 ```
```

