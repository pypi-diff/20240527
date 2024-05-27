# Comparing `tmp/maticalgos-spark-0.1.5.tar.gz` & `tmp/maticalgos-spark-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maticalgos-spark-0.1.5.tar", last modified: Thu May 16 09:06:01 2024, max compression
+gzip compressed data, was "maticalgos-spark-0.1.6.tar", last modified: Mon May 27 10:47:31 2024, max compression
```

## Comparing `maticalgos-spark-0.1.5.tar` & `maticalgos-spark-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 09:06:01.072623 maticalgos-spark-0.1.5/
--rw-rw-rw-   0        0        0      241 2024-05-16 08:21:15.000000 maticalgos-spark-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0    34977 2024-05-16 09:06:01.064094 maticalgos-spark-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    34450 2024-05-16 09:05:44.000000 maticalgos-spark-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 09:06:01.043002 maticalgos-spark-0.1.5/maticalgos/
--rw-rw-rw-   0        0        0       45 2024-05-16 08:57:44.000000 maticalgos-spark-0.1.5/maticalgos/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 09:06:01.054775 maticalgos-spark-0.1.5/maticalgos/sparkLib/
--rw-rw-rw-   0        0        0       72 2024-05-16 07:33:27.000000 maticalgos-spark-0.1.5/maticalgos/sparkLib/__init__.py
--rw-rw-rw-   0        0        0     4206 2024-05-16 07:20:34.000000 maticalgos-spark-0.1.5/maticalgos/sparkLib/order_websocket.py
--rw-rw-rw-   0        0        0    19695 2024-05-16 08:42:53.000000 maticalgos-spark-0.1.5/maticalgos/sparkLib/sparkLib.py
-drwxrwxrwx   0        0        0        0 2024-05-16 09:06:01.064094 maticalgos-spark-0.1.5/maticalgos_spark.egg-info/
--rw-rw-rw-   0        0        0    34977 2024-05-16 09:06:00.000000 maticalgos-spark-0.1.5/maticalgos_spark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2024-05-16 09:06:00.000000 maticalgos-spark-0.1.5/maticalgos_spark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 09:06:00.000000 maticalgos-spark-0.1.5/maticalgos_spark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 09:06:00.000000 maticalgos-spark-0.1.5/maticalgos_spark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       58 2024-05-16 07:20:34.000000 maticalgos-spark-0.1.5/requirementx.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 09:06:01.073851 maticalgos-spark-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      763 2024-05-16 09:05:48.000000 maticalgos-spark-0.1.5/setup.py
--rw-rw-rw-   0        0        0      739 2024-05-16 08:42:59.000000 maticalgos-spark-0.1.5/testWS.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:47:31.153818 maticalgos-spark-0.1.6/
+-rw-rw-rw-   0        0        0      241 2024-05-16 08:21:15.000000 maticalgos-spark-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    38592 2024-05-27 10:47:31.152827 maticalgos-spark-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    38065 2024-05-27 10:46:28.000000 maticalgos-spark-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 10:47:31.135141 maticalgos-spark-0.1.6/maticalgos/
+-rw-rw-rw-   0        0        0       45 2024-05-16 08:57:44.000000 maticalgos-spark-0.1.6/maticalgos/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:47:31.139135 maticalgos-spark-0.1.6/maticalgos/sparkLib/
+-rw-rw-rw-   0        0        0       72 2024-05-16 07:33:27.000000 maticalgos-spark-0.1.6/maticalgos/sparkLib/__init__.py
+-rw-rw-rw-   0        0        0     4206 2024-05-16 07:20:34.000000 maticalgos-spark-0.1.6/maticalgos/sparkLib/order_websocket.py
+-rw-rw-rw-   0        0        0    24301 2024-05-27 10:45:40.000000 maticalgos-spark-0.1.6/maticalgos/sparkLib/sparkLib.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:47:31.150663 maticalgos-spark-0.1.6/maticalgos_spark.egg-info/
+-rw-rw-rw-   0        0        0    38592 2024-05-27 10:47:30.000000 maticalgos-spark-0.1.6/maticalgos_spark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2024-05-27 10:47:31.000000 maticalgos-spark-0.1.6/maticalgos_spark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:47:30.000000 maticalgos-spark-0.1.6/maticalgos_spark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 10:47:30.000000 maticalgos-spark-0.1.6/maticalgos_spark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       58 2024-05-16 07:20:34.000000 maticalgos-spark-0.1.6/requirementx.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:47:31.153818 maticalgos-spark-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      763 2024-05-27 10:46:47.000000 maticalgos-spark-0.1.6/setup.py
+-rw-rw-rw-   0        0        0      742 2024-05-16 09:48:29.000000 maticalgos-spark-0.1.6/testWS.py
```

### Comparing `maticalgos-spark-0.1.5/PKG-INFO` & `maticalgos-spark-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maticalgos-spark
-Version: 0.1.5
+Version: 0.1.6
 Summary: SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
 Author: Niraj Munot
 Author-email: nirajmunot28@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -128,25 +128,25 @@
 
 ```python
 from maticalgos.sparkLib import SparkLib, OrderSocket
 ```
 
 2. **Create a Spark object**
 ```python
-spark_object = SparkLib(userid = "Your Emailid", 
+spark = SparkLib(userid = "Your Emailid", 
                          password = "Your Password")
 
 # OR
 
-spark_object = SparkLib(apikeys = "Your API Keys")
+spark = SparkLib(apikeys = "Your API Keys")
 ```
 
 3. **Generate a access token**
 ```python
-spark_object.generate_token()
+spark.generate_token()
 ```
 
 ## API Methods
 1. [Profile](#profile)
 2. [Account Info](#account-info)
    1. [All Accounts](#all-accounts)
    2. [One Account](#one-account)
@@ -157,42 +157,51 @@
    1. [Create Strategy](#create-strategy)
    2. [Get Strategies](#get-strategies)
    3. [Modify Strategy](#modify-strategy)
    4. [Delete Strategy](#delete-strategy)
 5. [Linked Strategies](#linked-strategies)
    1. [Link Account to Strategy](#link-account-to-strategy)
    2. [Get Linked Strategies](#get-linked-strategies)
-   3. [Modify Linked Strategy](#modify-linked-strategy)
+   3. [Get Linked Strategies By Account](#get-linked-strategies-by-account)
+   4. [Modify Linked Strategy](#modify-linked-strategy)
       1. Modify Linked Strategy
       2. Activate Linked Strategy
       3. Deactivate Linked Strategy
-   4. [Delete Linked Strategy](#delete-linked-strategy)
+   5. [Delete Linked Strategy](#delete-linked-strategy)
 
 6. [Expiry Dates](#get-expiry-dates)
 7. [Tokens](#get-tokens)
 8. [Order Management](#order-management)
    1. [LTP](#ltp)
    1. [Place order](#place-an-order)
    2. [Modify order](#modify-order)
    3. [Cancel order](#cancel-an-order)
    4. [Square off All Orders](#square-off)
    5. [Cancel All Orders](#cancel-all-orders)
+   6. [Stop Operation](#stop-operation)
+   7. [Square Off Single](#square-off-single)
+   8. [Delete Trade](#delete-order)
+   9. [Manual Square Off](#manual-square-off)
 
 10. [Orderbook](#orderbook)
 11. [Tradebook](#get-tradebook)
 12. [Netposition](#netposition)
 13. [Execution Logs](#get-excution-logs)
+14. [Holiday List](#get-holiday-list)
+15. [Freeze Quantity](#freeze-quantity)
+16. [Reconnect Order Websocket](#reconnect-order-websocket)
+17. [Contract Master File](#contract-master-file)
 
 ### Profile
 
 This method is used to get the profile of the user.
 
 Code
 ```python
-print(spark_object.profile()) # get profile
+print(spark.profile()) # get profile
 ```
 Sample response
 ```
 {'status': True, 'error': False, 'message': 'User exists', 'data': [{'ID': 10, 'Name': 'Your Name', 'Email': 'Your Email', 'PhoneNo': 'Your Phone No', 'LastLogin': '2024-04-02', 'CreatedOn': '2024-02-27', 'UCC': 'Your Unique User Code', 'Disabled': 0, 'UserType': 'admin', 'acLimit': 10, 'stLimit': 20}]}
 ```
 
 
@@ -200,26 +209,26 @@
 We can get the account information using the following methods
 of all accounts and one account.
 1. [All Accounts](#all-accounts)
 2. [one Account](#one-account)
 
 #### All Accounts
 ```python
-print(spark_object.getAllAccounts())
+print(spark.getAllAccounts())
 ```
 Sample response
 
 ```
 {'status': True, 'error': False, 'data': [{'Clientid': 'Your Client ID', 'AccountName': 'Your Account Name', 'LastLogin': '2024-04-03', 'UCC': 'Your Unique User Code', 'Trade': True, 'Broker': 'Your Broker'}], 'message': 'Data Received'}
 ```
 
 #### One Account
 We have to pass the account name to get the account information.
 ```python
-print(spark_object.getOneAccount(accountName='Your Account Name'))
+print(spark.getOneAccount(accountName='Your Account Name'))
 ```
 Sample response
 ```
 {'status': True, 'error': False, 'data': [{'Clientid': 'Your Client ID', 'Password': None, 'ApiKey':'Your API Key', 'ApiSecret': 'Your API Secret', 'Totp': 'na', 'AccountName': 'Your Account Name', 'LastLogin': '2024-04-03', 'UCC': 'Your Unique User Code', 'Chatid': 'Your Chat ID', 'BotKeys': 'Your Telegram Bot Key', 'Sessionid': 'Your Session ID', 'Trade': 'Y', 'Broker': 'Your Broker', 'Redirecturl': 'http://spark.maticalgos.com/auth_code/<Your Broker>', 'Pin': 'na'}], 'message': 'Data Received'}
 ```
 
 ## Account Management
@@ -315,19 +324,20 @@
 | StrategyType    | 'Intraday', 'Positional' | String    | Type of strategy (Intraday or Positional)      |
 | Display         | 'Private', 'Public'     | String    | Display setting for the strategy               |
 | ForwardTest     | 'Y', 'N'                | String    | Whether forward testing is enabled             |
 
 ## Linked Strategies
 1. [Link Account to Strategy](#link-account-to-strategy)
 2. [Get Linked Strategies](#get-linked-strategies)
-3. [Modify Linked Strategy](#modify-linked-strategy)
+3. [Get Linked Strategies By Account](#get-linked-strategies-by-account)
+4. [Modify Linked Strategy](#modify-linked-strategy)
    1. Modify Linked Strategy
    2. Activate Linked Strategy
    3. Deactivate Linked Strategy
-4. [Delete Linked Strategy](#delete-linked-strategy)
+5. [Delete Linked Strategy](#delete-linked-strategy)
 
 
 ### Link Account to Strategy
 ```python
 print(spark.addlinkStrategy(strategyName='Your Strategy Name',
                             accountName='Your Account Name',
                             Multiplier=1,
@@ -346,14 +356,24 @@
 ```
 
 Sample response
 ```
 {'status': True, 'error': False, 'data': [{'StrategyName': 'Your Strategy Name', 'AccountName': 'Your Account Name', 'UCC': 'Your UCC', 'Multiplier': 1, 'Activate': 1, 'Capital': 0.0}], 'message': 'Data Received'}
 ```
 
+### Get Linked Strategies By Account
+```python
+print(spark.spark.getlinkStrategyAccount(accountName='Your Account Name'))
+```
+
+Sample response
+```
+{'status': True, 'error': False, 'data': [{'StrategyName': 'Your Strategy Name', 'AccountName': 'Your Account Name', 'UCC': 'Your UCC', 'Multiplier': 1, 'Activate': 1, 'Capital': 0.0}], 'message': 'Data Received'}
+```
+
 ### Modify Linked Strategy
 ```python
 # Modify Linked Strategy
 print(spark.modifyLinkedStrategy(strategyName='Your Strategy Name',
                                 accountName='Your Account Name',
                                 Multiplier=1,
                                 Activate='Y',
@@ -445,17 +465,21 @@
 ## Order Management
 1. [LTP](#LTP)
 1. [Place order](#place-an-order)
 2. [Modify order](#modify-order)
 3. [Cancel order](#cancel-an-order)
 4. [Square off All Orders](#square-off)
 5. [Cancel All Orders](#cancel-all-orders)
-6. [Orderbook](#orderbook)
-7. [Tradebook](#get-tradebook)
-8. [Netposition](#netposition)
+6. [Stop Operation](#stop-operation)
+7. [Square Off Single](#square-off-single)
+8. [Delete Trade](#delete-order)
+9. [Manual Square Off](#manual-square-off)
+10. [Orderbook](#orderbook)
+11. [Tradebook](#get-tradebook)
+12. [Netposition](#netposition)
 
 ### LTP
 Get the last traded price of the token.
 Token format is 'Exchange:Token'
 ```python
 print(spark.ltp(Tokens='NSE:212'))
 ```
@@ -465,30 +489,30 @@
 1. Limit Order
 2. Market Order
 3. SL-Limit Order
 
 Code
 ```python
 # Limit Order
-print(spark_object.place_order(strategyName = "Your Strategy Name",
+print(spark.place_order(strategyName = "Your Strategy Name",
                                 transType = "Buy",
                                 token = "NSE:212", 
                                 qty = 1,
                                 orderType = "Limit",
                                 productType = "Intraday",
                                 limitPrice = 500.0))
 # Market Order
-print(spark_object.place_order(strategyName = "Your Strategy Name",
+print(spark.place_order(strategyName = "Your Strategy Name",
                                transType = "Sell",
                                token = "NSE:212",
                                qty = 1,
                                orderType = "Market",
                                productType = "Intraday"))
 # SL-Limit Order
-print(spark_object.place_order(strategyName = "Your Strategy Name",
+print(spark.place_order(strategyName = "Your Strategy Name",
                                transType = "Buy",
                                token = "NSE:212",
                                qty = 1,
                                orderType = "SL-Limit",
                                productType = "Intraday",
                                triggerPrice = 220,
                                limitPrice = 210))
@@ -508,27 +532,27 @@
 | productType     | "Intraday", "Delivery"             | String    | Product type (Intraday, Delivery, etc.)              |
 | limitPrice      | Float                              | Float     | Price specified for Limit and SL-Limit orders         |
 | triggerPrice    | Float                              | Float     | Trigger price specified for SL-Limit orders          |
 | strefID         | Integer                            | Integer   | Reference ID of the order placed                      |
 
 #### Modify Order
 ```python
-print(spark_object.modify_order(strategyName='Your Strategy Name',
+print(spark.modify_order(strategyName='Your Strategy Name',
                                 strefID=2328,
                                 orderType='SL-Limit',
                                 limitPrice=190))
 ```
 Sample response of modify order
 ```
 {'status': True, 'error': False, 'data': [{'strefID': 2328}], 'message': 'Order Modified.'}
 ```
 
 #### Cancel order
 ```python
-print(spark_object.cancel_order(strategyName='Your Strategy Name',strefID=2328))
+print(spark.cancel_order(strategyName='Your Strategy Name',strefID=2328))
 ```
 Sample response of cancel order
 ```
 {'status': True, 'error': True, 'data': [{'strefID': 2328}], 'message': 'Order Cancelled.'}
 ```
 
 ### Square off
@@ -555,47 +579,89 @@
 
 response
 ```
 {'status': True, 'error': False, 'data': [], 'message': 'Request sent to Cancel All Orders in StrategyName : Your Strategy Name with AccountName : Your Account Name'}
 {'status': True, 'error': False, 'data': [], 'message': 'Request sent to Cancel All Orders in AccountNamme : Your Account Name'}
 ```
 
+### Stop Operation
+
+```python
+print(spark.stopOperation(strategyName='Your Strategy Name', strefID='Your order Reference ID'))
+```
+
+Sample response
+```
+{'status': True, 'error': False, 'data': [{'strefID':Your order Reference ID }], 'message': 'Operations stopped on {Your order Reference ID}'}
+```
+
+### Square Off Single
+```python
+print(spark.squareOffSingle(accountName='You Account Name', strategyName='Your Strategy Name', token='NSE:13528', positionType='Intraday', at_limit='true'))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[{"strefID":308}],"message":"Order Placed, Position Squared off"}
+```
+
+### Delete Trade
+```python
+print(spark.deleteTrade(TDno='Your Trade Number'))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[],"message":"Trade Deleted"}
+```
+
+### Manual Square Off
+```python
+print(spark.manualSquareOff(accountName='Your Account Name', strategyName='Your Strategy Name', token='NSE:13528', positionType='Intraday', tradedPrice=0, tradedAt=0, ordersPlaced=0, qty=1))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[],"message":"Position closed manually."}
+```
+
+
 ### orderbook
 ```python
-print(spark_object.orderbook(accountName='Your Account Name',
+print(spark.orderbook(accountName='Your Account Name',
                              strategyName='Your Strategy Name',
                              strefid=2000, # Optional : order id
                              reftag='Your Reference Tag', # Optional : Reference Tag    
                              withorders='Y')) # Optional : 'Y' to get all orders 
-print(spark_object.orderbook(accountName='Your Account Name',
+print(spark.orderbook(accountName='Your Account Name',
                              strategyName='Your Strategy Name'))
 ```
 
 Sample response
 ```
 {'status': True, 'error': False, 'data': [{'UCC': 'Your UCC', 'AccountName': 'Your Account Name', 'strefID': 2240, 'reftag': 1939, 'StrategyName': 'Your Strategy Name', 'orderType': 'Limit', 'productType': 'Intraday', 'price': 171.25, 'limitPrice': 170.0, 'triggerPrice': 0.0, 'token': 'NSE:212', 'segment': 'C', 'symbol': 'ASHOKLEY-EQ', 'qty': 1, 'transType': 'Buy', 'splitby': 0, 'Operations': '{"timeLimit": 0, "shouldExecute": false, "priceBuffer": 0.0}', 'ordersplaced': 1, 'ordersdone': 1, 'ordersexecuted': 0, 'placed_at': '2024-03-29T10:54:08', 'recon_at': None, 'trade_at': None, 'filledQty': 0, 'tradedQty': None, 'tradeValue': None, 'tradePrice': 0.0, 'status': 'Error', 'active': 0, 'ForwardTest': None}], 'message': 'Data received'}
 ```
 
 ### Get tradebook
 ```python
-print(spark_object.tradebook(startDate='2024-04-01',
+print(spark.tradebook(startDate='2024-04-01',
                              endDate='2024-04-03',
                              strategyName='Your Strategy Name',
                              accountName='Your Account Name'))
 
 ```
 
 Sample response
 ```
 {'status': True, 'error': False, 'data': [], 'message': 'Tradebook data received'}
 ```
 
 ### Netposition
 ```python
-print(spark_object.netposition(accountName='Your Account Name',
+print(spark.netposition(accountName='Your Account Name',
                                strategyName='Your Strategy Name'))
 ```
 
 Sample response
 ```
 {'status': True, 'error': False, 'data': [{'Your Account Name': {'bookedpnl': 0.816660000000013, 'openpnl': None, 'totalpnl': None, 'totalpositions': 1, 'openpositions': 1}}], 'message': 'Data Received'}
 ```
@@ -606,14 +672,50 @@
 ```
 
 Sample response
 ```
 {'status': True, 'error': True, 'data': [{'Datetime': '2024-04-06T09:36:00', 'UCC': 'Your UCC', 'Name': 'Strategy Name', 'Alert Type': 'DEBUG', 'Message': "Endpoint Called : ModifyOrder. Payload Received : {'UCC': 'Your UCC', 'StrategyName': 'Strategy Name', 'strefID': 2327, 'orderType': 'Market', 'limitPrice': 0.0, 'triggerPrice': 0.0, 'identifier': ''}"}], 'message': 'Data Received'}
 ```
 
+### Reconnect Order Websocket
+```python
+print(spark.reconnect_orderWS(accountName='Your Account Name'))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[],"message":"Reconnecting to WS"}
+```
+
+### Holiday List
+```python
+print(spark.isHoliday(exch='NFO'))
+```
+
+Sample response
+```
+{'status': True, 'error': False, 'data': ['2024-04-02', '2024-04-06', '2024-04-13', '2024-04-14', '2024-04-19', '2024-04-21', '2024-04-28'], 'message': 'Data Received'}
+```
+
+### Freeze Quantity
+```python
+print(spark.freezeqty(symbol='BANKNIFTY'))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[{"freezeQty":900}],"message":"Data Received"}
+```
+
+### Contract Master File
+```python
+print(spark.contractMaster())
+```
+
+
 ## Sample Code
 ```python
 from SparkLib import SparkLib
 
 if __name__ == '__main__':
     spark = SparkLib(userid = 'Your User ID', password = 'Your Password', apikeys = 'Your API Keys')
     spark.generate_token()
@@ -628,14 +730,17 @@
                             limitPrice = 210,
                            ))
     print(spark.modifyorder(strategyName='Your Strategy Name',
                             strefID=2328,
                             orderType='SL-Limit',
                             limitPrice=190))
     print(spark.cancelorder(strategyName='Your Strategy Name',strefID=2328))
+    print(spark.stopOperation(strategyName='Your Strategy Name', strefID='Your order Reference ID'))
+    print(spark.deleteTrade(TDno='Your Trade Number'))
+    print(spark.manualSquareOff(accountName='Your Account Name', strategyName='Your Strategy Name', token='NSE:13528', positionType='Intraday', tradedPrice=0, tradedAt=0, ordersPlaced=0, qty=1))    
 
     print(spark.getExpiry(symbol='NIFTY',exchange='NFO',instrument='OPT'))
     print(spark.getExpiry(symbol='SBIN',exchange='NFO',instrument='FUT'))
     print(spark.getExpiry(symbol='SENSEX',exchange='BFO',instrument='FUT'))
     print(spark.getExpiry(symbol='SENSEX',exchange='BFO',instrument='OPT'))
     print(spark.getExpiry(symbol='USDINR',exchange='CDS',instrument='FUT'))
 
@@ -671,26 +776,36 @@
     print(spark.deletelinkStrategy(strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.CancalAll(ctype='strategy',strategyName='Your Strategy Name',accountName='Your Account Name'))
     print(spark.CancalAll(ctype='account',accountName='Your Account Name'))
 
     print(spark.SquareOff(ctype='strategy',strategyName='Your Strategy Name',accountName='Your Account Name'))
     print(spark.SquareOff(ctype='account',accountName='Your Account Name'))
-
+    print(spark.squareOffSingle(accountName='You Account Name', strategyName='Your Strategy Name', token='NSE:13528', positionType='Intraday', at_limit='true'))
+    
     print(spark.ltp(Tokens='NSE:212'))
 
     print(spark.intradaypnl(strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.netposition(strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.tradebook(startDate='2024-04-01',endDate='2024-04-04',strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.orderbook(strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.excutionLogs())
+
+    print(spark.reconnect_orderWS(accountName='Your Account Name'))
+    
+    print(spark.isHoliday(exch='NFO'))
+    
+    print(spark.freezeqty(symbol='BANKNIFTY'))
+    
+    print(spark.contractMaster())
+
 ```
 
 
 
 # Order Websocket
 
 The order websocket is a real-time communication protocol used to receive order-related messages from the Spark platform. It provides users with updates on order status, execution, and other pertinent information related to their trading activity. The websocket operates by continuously listening for incoming messages from the Spark platform and relaying them to the user in real-time.
```

### Comparing `maticalgos-spark-0.1.5/README.md` & `maticalgos-spark-0.1.6/maticalgos_spark.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: maticalgos-spark
+Version: 0.1.6
+Summary: SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
+Author: Niraj Munot
+Author-email: nirajmunot28@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # SparkLib - MaticAlgos Python Client
 
 SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
 
 ## Installation
 
 You can install the pre release via pip
@@ -116,25 +128,25 @@
 
 ```python
 from maticalgos.sparkLib import SparkLib, OrderSocket
 ```
 
 2. **Create a Spark object**
 ```python
-spark_object = SparkLib(userid = "Your Emailid", 
+spark = SparkLib(userid = "Your Emailid", 
                          password = "Your Password")
 
 # OR
 
-spark_object = SparkLib(apikeys = "Your API Keys")
+spark = SparkLib(apikeys = "Your API Keys")
 ```
 
 3. **Generate a access token**
 ```python
-spark_object.generate_token()
+spark.generate_token()
 ```
 
 ## API Methods
 1. [Profile](#profile)
 2. [Account Info](#account-info)
    1. [All Accounts](#all-accounts)
    2. [One Account](#one-account)
@@ -145,42 +157,51 @@
    1. [Create Strategy](#create-strategy)
    2. [Get Strategies](#get-strategies)
    3. [Modify Strategy](#modify-strategy)
    4. [Delete Strategy](#delete-strategy)
 5. [Linked Strategies](#linked-strategies)
    1. [Link Account to Strategy](#link-account-to-strategy)
    2. [Get Linked Strategies](#get-linked-strategies)
-   3. [Modify Linked Strategy](#modify-linked-strategy)
+   3. [Get Linked Strategies By Account](#get-linked-strategies-by-account)
+   4. [Modify Linked Strategy](#modify-linked-strategy)
       1. Modify Linked Strategy
       2. Activate Linked Strategy
       3. Deactivate Linked Strategy
-   4. [Delete Linked Strategy](#delete-linked-strategy)
+   5. [Delete Linked Strategy](#delete-linked-strategy)
 
 6. [Expiry Dates](#get-expiry-dates)
 7. [Tokens](#get-tokens)
 8. [Order Management](#order-management)
    1. [LTP](#ltp)
    1. [Place order](#place-an-order)
    2. [Modify order](#modify-order)
    3. [Cancel order](#cancel-an-order)
    4. [Square off All Orders](#square-off)
    5. [Cancel All Orders](#cancel-all-orders)
+   6. [Stop Operation](#stop-operation)
+   7. [Square Off Single](#square-off-single)
+   8. [Delete Trade](#delete-order)
+   9. [Manual Square Off](#manual-square-off)
 
 10. [Orderbook](#orderbook)
 11. [Tradebook](#get-tradebook)
 12. [Netposition](#netposition)
 13. [Execution Logs](#get-excution-logs)
+14. [Holiday List](#get-holiday-list)
+15. [Freeze Quantity](#freeze-quantity)
+16. [Reconnect Order Websocket](#reconnect-order-websocket)
+17. [Contract Master File](#contract-master-file)
 
 ### Profile
 
 This method is used to get the profile of the user.
 
 Code
 ```python
-print(spark_object.profile()) # get profile
+print(spark.profile()) # get profile
 ```
 Sample response
 ```
 {'status': True, 'error': False, 'message': 'User exists', 'data': [{'ID': 10, 'Name': 'Your Name', 'Email': 'Your Email', 'PhoneNo': 'Your Phone No', 'LastLogin': '2024-04-02', 'CreatedOn': '2024-02-27', 'UCC': 'Your Unique User Code', 'Disabled': 0, 'UserType': 'admin', 'acLimit': 10, 'stLimit': 20}]}
 ```
 
 
@@ -188,26 +209,26 @@
 We can get the account information using the following methods
 of all accounts and one account.
 1. [All Accounts](#all-accounts)
 2. [one Account](#one-account)
 
 #### All Accounts
 ```python
-print(spark_object.getAllAccounts())
+print(spark.getAllAccounts())
 ```
 Sample response
 
 ```
 {'status': True, 'error': False, 'data': [{'Clientid': 'Your Client ID', 'AccountName': 'Your Account Name', 'LastLogin': '2024-04-03', 'UCC': 'Your Unique User Code', 'Trade': True, 'Broker': 'Your Broker'}], 'message': 'Data Received'}
 ```
 
 #### One Account
 We have to pass the account name to get the account information.
 ```python
-print(spark_object.getOneAccount(accountName='Your Account Name'))
+print(spark.getOneAccount(accountName='Your Account Name'))
 ```
 Sample response
 ```
 {'status': True, 'error': False, 'data': [{'Clientid': 'Your Client ID', 'Password': None, 'ApiKey':'Your API Key', 'ApiSecret': 'Your API Secret', 'Totp': 'na', 'AccountName': 'Your Account Name', 'LastLogin': '2024-04-03', 'UCC': 'Your Unique User Code', 'Chatid': 'Your Chat ID', 'BotKeys': 'Your Telegram Bot Key', 'Sessionid': 'Your Session ID', 'Trade': 'Y', 'Broker': 'Your Broker', 'Redirecturl': 'http://spark.maticalgos.com/auth_code/<Your Broker>', 'Pin': 'na'}], 'message': 'Data Received'}
 ```
 
 ## Account Management
@@ -303,19 +324,20 @@
 | StrategyType    | 'Intraday', 'Positional' | String    | Type of strategy (Intraday or Positional)      |
 | Display         | 'Private', 'Public'     | String    | Display setting for the strategy               |
 | ForwardTest     | 'Y', 'N'                | String    | Whether forward testing is enabled             |
 
 ## Linked Strategies
 1. [Link Account to Strategy](#link-account-to-strategy)
 2. [Get Linked Strategies](#get-linked-strategies)
-3. [Modify Linked Strategy](#modify-linked-strategy)
+3. [Get Linked Strategies By Account](#get-linked-strategies-by-account)
+4. [Modify Linked Strategy](#modify-linked-strategy)
    1. Modify Linked Strategy
    2. Activate Linked Strategy
    3. Deactivate Linked Strategy
-4. [Delete Linked Strategy](#delete-linked-strategy)
+5. [Delete Linked Strategy](#delete-linked-strategy)
 
 
 ### Link Account to Strategy
 ```python
 print(spark.addlinkStrategy(strategyName='Your Strategy Name',
                             accountName='Your Account Name',
                             Multiplier=1,
@@ -334,14 +356,24 @@
 ```
 
 Sample response
 ```
 {'status': True, 'error': False, 'data': [{'StrategyName': 'Your Strategy Name', 'AccountName': 'Your Account Name', 'UCC': 'Your UCC', 'Multiplier': 1, 'Activate': 1, 'Capital': 0.0}], 'message': 'Data Received'}
 ```
 
+### Get Linked Strategies By Account
+```python
+print(spark.spark.getlinkStrategyAccount(accountName='Your Account Name'))
+```
+
+Sample response
+```
+{'status': True, 'error': False, 'data': [{'StrategyName': 'Your Strategy Name', 'AccountName': 'Your Account Name', 'UCC': 'Your UCC', 'Multiplier': 1, 'Activate': 1, 'Capital': 0.0}], 'message': 'Data Received'}
+```
+
 ### Modify Linked Strategy
 ```python
 # Modify Linked Strategy
 print(spark.modifyLinkedStrategy(strategyName='Your Strategy Name',
                                 accountName='Your Account Name',
                                 Multiplier=1,
                                 Activate='Y',
@@ -433,17 +465,21 @@
 ## Order Management
 1. [LTP](#LTP)
 1. [Place order](#place-an-order)
 2. [Modify order](#modify-order)
 3. [Cancel order](#cancel-an-order)
 4. [Square off All Orders](#square-off)
 5. [Cancel All Orders](#cancel-all-orders)
-6. [Orderbook](#orderbook)
-7. [Tradebook](#get-tradebook)
-8. [Netposition](#netposition)
+6. [Stop Operation](#stop-operation)
+7. [Square Off Single](#square-off-single)
+8. [Delete Trade](#delete-order)
+9. [Manual Square Off](#manual-square-off)
+10. [Orderbook](#orderbook)
+11. [Tradebook](#get-tradebook)
+12. [Netposition](#netposition)
 
 ### LTP
 Get the last traded price of the token.
 Token format is 'Exchange:Token'
 ```python
 print(spark.ltp(Tokens='NSE:212'))
 ```
@@ -453,30 +489,30 @@
 1. Limit Order
 2. Market Order
 3. SL-Limit Order
 
 Code
 ```python
 # Limit Order
-print(spark_object.place_order(strategyName = "Your Strategy Name",
+print(spark.place_order(strategyName = "Your Strategy Name",
                                 transType = "Buy",
                                 token = "NSE:212", 
                                 qty = 1,
                                 orderType = "Limit",
                                 productType = "Intraday",
                                 limitPrice = 500.0))
 # Market Order
-print(spark_object.place_order(strategyName = "Your Strategy Name",
+print(spark.place_order(strategyName = "Your Strategy Name",
                                transType = "Sell",
                                token = "NSE:212",
                                qty = 1,
                                orderType = "Market",
                                productType = "Intraday"))
 # SL-Limit Order
-print(spark_object.place_order(strategyName = "Your Strategy Name",
+print(spark.place_order(strategyName = "Your Strategy Name",
                                transType = "Buy",
                                token = "NSE:212",
                                qty = 1,
                                orderType = "SL-Limit",
                                productType = "Intraday",
                                triggerPrice = 220,
                                limitPrice = 210))
@@ -496,27 +532,27 @@
 | productType     | "Intraday", "Delivery"             | String    | Product type (Intraday, Delivery, etc.)              |
 | limitPrice      | Float                              | Float     | Price specified for Limit and SL-Limit orders         |
 | triggerPrice    | Float                              | Float     | Trigger price specified for SL-Limit orders          |
 | strefID         | Integer                            | Integer   | Reference ID of the order placed                      |
 
 #### Modify Order
 ```python
-print(spark_object.modify_order(strategyName='Your Strategy Name',
+print(spark.modify_order(strategyName='Your Strategy Name',
                                 strefID=2328,
                                 orderType='SL-Limit',
                                 limitPrice=190))
 ```
 Sample response of modify order
 ```
 {'status': True, 'error': False, 'data': [{'strefID': 2328}], 'message': 'Order Modified.'}
 ```
 
 #### Cancel order
 ```python
-print(spark_object.cancel_order(strategyName='Your Strategy Name',strefID=2328))
+print(spark.cancel_order(strategyName='Your Strategy Name',strefID=2328))
 ```
 Sample response of cancel order
 ```
 {'status': True, 'error': True, 'data': [{'strefID': 2328}], 'message': 'Order Cancelled.'}
 ```
 
 ### Square off
@@ -543,47 +579,89 @@
 
 response
 ```
 {'status': True, 'error': False, 'data': [], 'message': 'Request sent to Cancel All Orders in StrategyName : Your Strategy Name with AccountName : Your Account Name'}
 {'status': True, 'error': False, 'data': [], 'message': 'Request sent to Cancel All Orders in AccountNamme : Your Account Name'}
 ```
 
+### Stop Operation
+
+```python
+print(spark.stopOperation(strategyName='Your Strategy Name', strefID='Your order Reference ID'))
+```
+
+Sample response
+```
+{'status': True, 'error': False, 'data': [{'strefID':Your order Reference ID }], 'message': 'Operations stopped on {Your order Reference ID}'}
+```
+
+### Square Off Single
+```python
+print(spark.squareOffSingle(accountName='You Account Name', strategyName='Your Strategy Name', token='NSE:13528', positionType='Intraday', at_limit='true'))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[{"strefID":308}],"message":"Order Placed, Position Squared off"}
+```
+
+### Delete Trade
+```python
+print(spark.deleteTrade(TDno='Your Trade Number'))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[],"message":"Trade Deleted"}
+```
+
+### Manual Square Off
+```python
+print(spark.manualSquareOff(accountName='Your Account Name', strategyName='Your Strategy Name', token='NSE:13528', positionType='Intraday', tradedPrice=0, tradedAt=0, ordersPlaced=0, qty=1))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[],"message":"Position closed manually."}
+```
+
+
 ### orderbook
 ```python
-print(spark_object.orderbook(accountName='Your Account Name',
+print(spark.orderbook(accountName='Your Account Name',
                              strategyName='Your Strategy Name',
                              strefid=2000, # Optional : order id
                              reftag='Your Reference Tag', # Optional : Reference Tag    
                              withorders='Y')) # Optional : 'Y' to get all orders 
-print(spark_object.orderbook(accountName='Your Account Name',
+print(spark.orderbook(accountName='Your Account Name',
                              strategyName='Your Strategy Name'))
 ```
 
 Sample response
 ```
 {'status': True, 'error': False, 'data': [{'UCC': 'Your UCC', 'AccountName': 'Your Account Name', 'strefID': 2240, 'reftag': 1939, 'StrategyName': 'Your Strategy Name', 'orderType': 'Limit', 'productType': 'Intraday', 'price': 171.25, 'limitPrice': 170.0, 'triggerPrice': 0.0, 'token': 'NSE:212', 'segment': 'C', 'symbol': 'ASHOKLEY-EQ', 'qty': 1, 'transType': 'Buy', 'splitby': 0, 'Operations': '{"timeLimit": 0, "shouldExecute": false, "priceBuffer": 0.0}', 'ordersplaced': 1, 'ordersdone': 1, 'ordersexecuted': 0, 'placed_at': '2024-03-29T10:54:08', 'recon_at': None, 'trade_at': None, 'filledQty': 0, 'tradedQty': None, 'tradeValue': None, 'tradePrice': 0.0, 'status': 'Error', 'active': 0, 'ForwardTest': None}], 'message': 'Data received'}
 ```
 
 ### Get tradebook
 ```python
-print(spark_object.tradebook(startDate='2024-04-01',
+print(spark.tradebook(startDate='2024-04-01',
                              endDate='2024-04-03',
                              strategyName='Your Strategy Name',
                              accountName='Your Account Name'))
 
 ```
 
 Sample response
 ```
 {'status': True, 'error': False, 'data': [], 'message': 'Tradebook data received'}
 ```
 
 ### Netposition
 ```python
-print(spark_object.netposition(accountName='Your Account Name',
+print(spark.netposition(accountName='Your Account Name',
                                strategyName='Your Strategy Name'))
 ```
 
 Sample response
 ```
 {'status': True, 'error': False, 'data': [{'Your Account Name': {'bookedpnl': 0.816660000000013, 'openpnl': None, 'totalpnl': None, 'totalpositions': 1, 'openpositions': 1}}], 'message': 'Data Received'}
 ```
@@ -594,14 +672,50 @@
 ```
 
 Sample response
 ```
 {'status': True, 'error': True, 'data': [{'Datetime': '2024-04-06T09:36:00', 'UCC': 'Your UCC', 'Name': 'Strategy Name', 'Alert Type': 'DEBUG', 'Message': "Endpoint Called : ModifyOrder. Payload Received : {'UCC': 'Your UCC', 'StrategyName': 'Strategy Name', 'strefID': 2327, 'orderType': 'Market', 'limitPrice': 0.0, 'triggerPrice': 0.0, 'identifier': ''}"}], 'message': 'Data Received'}
 ```
 
+### Reconnect Order Websocket
+```python
+print(spark.reconnect_orderWS(accountName='Your Account Name'))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[],"message":"Reconnecting to WS"}
+```
+
+### Holiday List
+```python
+print(spark.isHoliday(exch='NFO'))
+```
+
+Sample response
+```
+{'status': True, 'error': False, 'data': ['2024-04-02', '2024-04-06', '2024-04-13', '2024-04-14', '2024-04-19', '2024-04-21', '2024-04-28'], 'message': 'Data Received'}
+```
+
+### Freeze Quantity
+```python
+print(spark.freezeqty(symbol='BANKNIFTY'))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[{"freezeQty":900}],"message":"Data Received"}
+```
+
+### Contract Master File
+```python
+print(spark.contractMaster())
+```
+
+
 ## Sample Code
 ```python
 from SparkLib import SparkLib
 
 if __name__ == '__main__':
     spark = SparkLib(userid = 'Your User ID', password = 'Your Password', apikeys = 'Your API Keys')
     spark.generate_token()
@@ -616,14 +730,17 @@
                             limitPrice = 210,
                            ))
     print(spark.modifyorder(strategyName='Your Strategy Name',
                             strefID=2328,
                             orderType='SL-Limit',
                             limitPrice=190))
     print(spark.cancelorder(strategyName='Your Strategy Name',strefID=2328))
+    print(spark.stopOperation(strategyName='Your Strategy Name', strefID='Your order Reference ID'))
+    print(spark.deleteTrade(TDno='Your Trade Number'))
+    print(spark.manualSquareOff(accountName='Your Account Name', strategyName='Your Strategy Name', token='NSE:13528', positionType='Intraday', tradedPrice=0, tradedAt=0, ordersPlaced=0, qty=1))    
 
     print(spark.getExpiry(symbol='NIFTY',exchange='NFO',instrument='OPT'))
     print(spark.getExpiry(symbol='SBIN',exchange='NFO',instrument='FUT'))
     print(spark.getExpiry(symbol='SENSEX',exchange='BFO',instrument='FUT'))
     print(spark.getExpiry(symbol='SENSEX',exchange='BFO',instrument='OPT'))
     print(spark.getExpiry(symbol='USDINR',exchange='CDS',instrument='FUT'))
 
@@ -659,26 +776,36 @@
     print(spark.deletelinkStrategy(strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.CancalAll(ctype='strategy',strategyName='Your Strategy Name',accountName='Your Account Name'))
     print(spark.CancalAll(ctype='account',accountName='Your Account Name'))
 
     print(spark.SquareOff(ctype='strategy',strategyName='Your Strategy Name',accountName='Your Account Name'))
     print(spark.SquareOff(ctype='account',accountName='Your Account Name'))
-
+    print(spark.squareOffSingle(accountName='You Account Name', strategyName='Your Strategy Name', token='NSE:13528', positionType='Intraday', at_limit='true'))
+    
     print(spark.ltp(Tokens='NSE:212'))
 
     print(spark.intradaypnl(strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.netposition(strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.tradebook(startDate='2024-04-01',endDate='2024-04-04',strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.orderbook(strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.excutionLogs())
+
+    print(spark.reconnect_orderWS(accountName='Your Account Name'))
+    
+    print(spark.isHoliday(exch='NFO'))
+    
+    print(spark.freezeqty(symbol='BANKNIFTY'))
+    
+    print(spark.contractMaster())
+
 ```
 
 
 
 # Order Websocket
 
 The order websocket is a real-time communication protocol used to receive order-related messages from the Spark platform. It provides users with updates on order status, execution, and other pertinent information related to their trading activity. The websocket operates by continuously listening for incoming messages from the Spark platform and relaying them to the user in real-time.
@@ -743,8 +870,8 @@
   - This parameter specifies the maximum number of reconnection attempts that the websocket should make before giving up. By default, it is set to 20.
 - **access_token**: 
   - This parameter specifies the access token required to establish a connection to the Spark platform.
 - **connect()**: 
   - This method is used to establish a connection to the Spark platform using the access token.
 - **close_connection()**: 
   - This method is used to close the websocket connection to the Spark platform.
-  
+
```

### Comparing `maticalgos-spark-0.1.5/maticalgos/sparkLib/order_websocket.py` & `maticalgos-spark-0.1.6/maticalgos/sparkLib/order_websocket.py`

 * *Files identical despite different names*

### Comparing `maticalgos-spark-0.1.5/maticalgos/sparkLib/sparkLib.py` & `maticalgos-spark-0.1.6/maticalgos/sparkLib/sparkLib.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,42 +19,51 @@
         "order.modify" : "/order",
         "master.expiry" : "/expiry?symbol={symbol}&exchange={exchange}&instrument={instrument}",
         "master.token" : "/master-tokens?{body}",
         "account.all" : "/account",
         "account.one" : "/account/{accountName}",
         "account.activate": "/activate-account/{account}/{yn}",
         "authcode.validate" : "/validate_authcode/{broker}",
+        "authcode.generate" : "/login/{account}",
         "strategy" : "/strategy",
         "strategy.create" : "/strategy",
         "strategy.modify" : "/strategy/{strategyname}",
         "strategy.delete" : "/strategy/{strategyname}",
         "linkstartegy" : "/linkstrategy",
-        "linkstrategyaccount" : "/link-strategy-account",
+        "linkstrategyaccount" : "/link-strategy-account?ac={acname}",
         "modifylinkstrategy" : "/linkstrategy?st={st}&ac={ac}",
         "deleteLinkStrategy" : "/linkstrategy?st={st}&ac={ac}",
         "CancalAll_url" : "/CancelAll/{ctype}?stname={stname}&acname={acname}",
         "SquareOff_url" : "/SquareOff/{ctype}?stname={stname}&acname={acname}",
         "orderbook" : "/orderbook/?acname={acname}&stname={stname}",
         "tradebook" : "/tradebook/?startDate={startDate}&endDate={endDate}&stname={stname}&acname={acname}",
         "netposition" : "/netposition/",
         "pushtrades" : "/pushtrades/",
         "overview" : "/overview/",
         "ltp" : "/ltp?Tokens={Tokens}",
         "excutionLogs" : "/ExecutionLogs",
-        "intradaypnl" : "/intradaypnl?acname={acname}&stname={stname}"
+        "intradaypnl" : "/intradaypnl?acname={acname}&stname={stname}",
+        "reconnectOrderWS":"/reconnectWS/?acname={acname}",
+        "stopOperation":"/stopOperation",
+        "squareOffSingle":"/SquareOffSingle?acname={acname}&stname={stname}&token={token}&positionType={positionType}&at_limit={at_limit}",
+        "trade.delete" : "/trade/?TDno={TDno}",
+        "manualSquareOff" : "/manual-squareoff/?acname={acname}&stname={stname}&token={token}&positionType={positionType}",
+        "isHoliday" : "/isHoliday/?exch={exch}",
+        "freezeqty" : "/master-freezeqty?symbol={symbol}",
+        "contractMaster" : "/contract-master/",
     }
     _timeout = 15
 
     def __init__(self, userid = None, password = None, apikeys = None, access_token = None):
         self.userid = userid
         self.password = password
         self.apikeys = apikeys
         self.reqsession = requests.Session()
         self.header = {}
-        if not access_token :
+        if access_token:
             self.set_AccessToken(access_token)
 
     def set_AccessToken(self, access_token):
         """
         Set the access token for the session
 
         Args:
@@ -82,15 +91,15 @@
 
         resp = self._request("POST", url, data = data)
 
         if not resp.get("access_token") :
             return resp
         else :
             self.set_AccessToken(resp['access_token'])
-            return {"stutus" : True, "error" : False, "data" : [], "message" : "User Authorized"}
+            return {"stutus" : True, "error" : False, "data" : [resp], "message" : "User Authorized"}
 
     def profile(self):
         """
         Get the profile of the user
 
         Returns
         -------
@@ -208,15 +217,14 @@
         for p in data:
             st = st + p + "=" + data[p] + "&"
         st = st[:-1]
 
         url = "".join([self.BASEURL, self._routes['master.token'].format(body = st)])
         return self._request("GET", url)
 
-
     def getAllAccounts(self):
         """
         Get all accounts
         """
         url = "".join([self.BASEURL, self._routes['account.all']])
         return self._request("GET", url)
 
@@ -226,14 +234,24 @@
 
         Args:
             AccountName (str): Name of the account
         """
         url = "".join([self.BASEURL, self._routes['account.one'].format(accountName = accountName)])
         return self._request("GET", url)
 
+    def generateAuthcode(self, accountName):
+        """
+        Generate the auth code
+
+        Args:
+            accountName (str): Name of the account
+        """
+        url = "".join([self.BASEURL, self._routes['authcode.generate'].format(account = accountName)])
+        return self._request("POST", url)
+
     def validateAuthcode(self, broker, authcode):
         """
         Validate the auth code
 
         Args:
             broker (str): Name of the broker
             authcode (str): Auth code
@@ -357,20 +375,20 @@
             accountName (str): Name of the account
         """
         url = "".join([self.BASEURL, self._routes['deleteLinkStrategy']]).format(st = strategyName, ac = accountName)
         return self._request("DELETE", url)
 
     def getlinkStrategyAccount(self, accountName):
         """
-        Get the link strategy account
+        Get the linked Strategy Per Account
 
         Args:
             accountName (str): Name of the account
         """
-        url = "".join([self.BASEURL, self._routes['linkstrategyaccount']]).format(ac = accountName)
+        url = "".join([self.BASEURL, self._routes['linkstrategyaccount']]).format(acname = accountName)
         return self._request("GET", url)
 
     def CancalAll(self, ctype, accountName ,strategyName = 'undefined'):
         """
         Cancel all the orders
 
         Args:
@@ -478,14 +496,107 @@
         Args:
             accountName (str): Name of the account
             strategyName (str): Name of the strategy
         """
         url = "".join([self.BASEURL, self._routes['intradaypnl']]).format(acname = accountName, stname = strategyName)
         return self._request("GET", url)
 
+    def reconnect_orderWS(self,accountName):
+        """
+        Reconnect the order WS
+
+        Args:
+            accountName (str): Name of the account
+        """
+        url = "".join([self.BASEURL, self._routes['reconnectOrderWS']]).format(acname = accountName)
+        return self._request("POST", url)
+
+    def stopOperation(self,strategyName,strefID):
+        """
+        Stop the operation
+
+        Args:
+            strategyName (str): Name of the strategy
+            strefID (str): Reference ID of the order
+        """
+        body = {"strategyname": strategyName, "strefID": strefID}
+        url = "".join([self.BASEURL, self._routes['stopOperation']])
+        return self._request("POST", url, body = body)
+
+    def squareOffSingle(self,accountName,strategyName,token,positionType,at_limit):
+        """
+        Square off the single order
+
+        Args:
+            accountName (str): Name of the account
+            strategyName (str): Name of the strategy
+            token (str): Token of the Symbol
+            positionType (str): Position type of the order
+            at_limit (str): At limit [true, false]
+        """
+        at_limit = at_limit if at_limit in ['true','false'] else '--'
+        url = "".join([self.BASEURL, self._routes['squareOffSingle']]).format(acname = accountName, stname = strategyName, token = token, positionType = positionType, at_limit = at_limit)
+        return self._request("POST", url)
+
+    def manualSquareOff(self,accountName,strategyName,token,positionType,tradedPrice,tradedAt,ordersPlaced,qty):
+        """
+        Manual square off
+
+        Args:
+            accountName (str): Name of the account
+            strategyName (str): Name of the strategy
+            token (str): Token of the Symbol
+            positionType (str): Position type of the order
+            tradedPrice (float): Traded price
+            tradedAt (float): Traded at
+            ordersPlaced (float): Orders placed
+            qty (int): Quantity
+        """
+        body = {"tradedPrice": tradedPrice, "tradedAt": tradedAt, "ordersPlaced": ordersPlaced, "qty": qty}
+        url = "".join([self.BASEURL, self._routes['manualSquareOff']]).format(acname = accountName, stname = strategyName, token = token, positionType = positionType)
+        return self._request("POST", url, body = body)
+
+    def deleteTrade(self,TDno):
+        """
+        Delete the trade
+
+        Args:
+            TDno (str): Trade number
+        """
+        url = "".join([self.BASEURL, self._routes['trade.delete']]).format(TDno = TDno)
+        return self._request("DELETE", url)
+
+    def isHoliday(self,exch):
+        """
+        Get Holiday Dates list
+
+        Args:
+            exch (str): Exchange name
+        """
+        url = "".join([self.BASEURL, self._routes['isHoliday']]).format(exch = exch)
+        return self._request("GET", url)
+
+    def freezeqty(self,symbol):
+        """
+        Get the freeze quantity for the symbol
+
+        Args:
+            symbol (str): Symbol of the instrument
+        """
+        url = "".join([self.BASEURL, self._routes['freezeqty']]).format(symbol = symbol)
+        return self._request("GET", url)
+
+    def contractMaster(self):
+        """
+        Get the File containing all the contracts information
+
+        """
+        url = "".join([self.BASEURL, self._routes['contractMaster']])
+        return self._request("GET", url)
+
     def _request(self, method, url, body = None, data = None, is_header = True, timeout = _timeout):
         """
         Make the request to the server
 
         Args:
             method (str): Method of the request
             url (str): URL of the request
@@ -504,10 +615,14 @@
             # print(resp.text)
             data = resp.json()
             return data
 
         except requests.exceptions.Timeout:
             return {"status" : False, "data" : [], "error" : True, "message" : "Timeout error"}
 
+        except requests.exceptions.ConnectionError:
+            return {"status" : False, "data" : [], "error" : True, "message" : "Connection error"}
+
         except Exception as e :
             return {"status" : False, "data" : [], "error" : True, "message" : e}
 
+
```

### Comparing `maticalgos-spark-0.1.5/maticalgos_spark.egg-info/PKG-INFO` & `maticalgos-spark-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: maticalgos-spark
-Version: 0.1.5
-Summary: SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
-Author: Niraj Munot
-Author-email: nirajmunot28@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # SparkLib - MaticAlgos Python Client
 
 SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.
 
 ## Installation
 
 You can install the pre release via pip
@@ -128,25 +116,25 @@
 
 ```python
 from maticalgos.sparkLib import SparkLib, OrderSocket
 ```
 
 2. **Create a Spark object**
 ```python
-spark_object = SparkLib(userid = "Your Emailid", 
+spark = SparkLib(userid = "Your Emailid", 
                          password = "Your Password")
 
 # OR
 
-spark_object = SparkLib(apikeys = "Your API Keys")
+spark = SparkLib(apikeys = "Your API Keys")
 ```
 
 3. **Generate a access token**
 ```python
-spark_object.generate_token()
+spark.generate_token()
 ```
 
 ## API Methods
 1. [Profile](#profile)
 2. [Account Info](#account-info)
    1. [All Accounts](#all-accounts)
    2. [One Account](#one-account)
@@ -157,42 +145,51 @@
    1. [Create Strategy](#create-strategy)
    2. [Get Strategies](#get-strategies)
    3. [Modify Strategy](#modify-strategy)
    4. [Delete Strategy](#delete-strategy)
 5. [Linked Strategies](#linked-strategies)
    1. [Link Account to Strategy](#link-account-to-strategy)
    2. [Get Linked Strategies](#get-linked-strategies)
-   3. [Modify Linked Strategy](#modify-linked-strategy)
+   3. [Get Linked Strategies By Account](#get-linked-strategies-by-account)
+   4. [Modify Linked Strategy](#modify-linked-strategy)
       1. Modify Linked Strategy
       2. Activate Linked Strategy
       3. Deactivate Linked Strategy
-   4. [Delete Linked Strategy](#delete-linked-strategy)
+   5. [Delete Linked Strategy](#delete-linked-strategy)
 
 6. [Expiry Dates](#get-expiry-dates)
 7. [Tokens](#get-tokens)
 8. [Order Management](#order-management)
    1. [LTP](#ltp)
    1. [Place order](#place-an-order)
    2. [Modify order](#modify-order)
    3. [Cancel order](#cancel-an-order)
    4. [Square off All Orders](#square-off)
    5. [Cancel All Orders](#cancel-all-orders)
+   6. [Stop Operation](#stop-operation)
+   7. [Square Off Single](#square-off-single)
+   8. [Delete Trade](#delete-order)
+   9. [Manual Square Off](#manual-square-off)
 
 10. [Orderbook](#orderbook)
 11. [Tradebook](#get-tradebook)
 12. [Netposition](#netposition)
 13. [Execution Logs](#get-excution-logs)
+14. [Holiday List](#get-holiday-list)
+15. [Freeze Quantity](#freeze-quantity)
+16. [Reconnect Order Websocket](#reconnect-order-websocket)
+17. [Contract Master File](#contract-master-file)
 
 ### Profile
 
 This method is used to get the profile of the user.
 
 Code
 ```python
-print(spark_object.profile()) # get profile
+print(spark.profile()) # get profile
 ```
 Sample response
 ```
 {'status': True, 'error': False, 'message': 'User exists', 'data': [{'ID': 10, 'Name': 'Your Name', 'Email': 'Your Email', 'PhoneNo': 'Your Phone No', 'LastLogin': '2024-04-02', 'CreatedOn': '2024-02-27', 'UCC': 'Your Unique User Code', 'Disabled': 0, 'UserType': 'admin', 'acLimit': 10, 'stLimit': 20}]}
 ```
 
 
@@ -200,26 +197,26 @@
 We can get the account information using the following methods
 of all accounts and one account.
 1. [All Accounts](#all-accounts)
 2. [one Account](#one-account)
 
 #### All Accounts
 ```python
-print(spark_object.getAllAccounts())
+print(spark.getAllAccounts())
 ```
 Sample response
 
 ```
 {'status': True, 'error': False, 'data': [{'Clientid': 'Your Client ID', 'AccountName': 'Your Account Name', 'LastLogin': '2024-04-03', 'UCC': 'Your Unique User Code', 'Trade': True, 'Broker': 'Your Broker'}], 'message': 'Data Received'}
 ```
 
 #### One Account
 We have to pass the account name to get the account information.
 ```python
-print(spark_object.getOneAccount(accountName='Your Account Name'))
+print(spark.getOneAccount(accountName='Your Account Name'))
 ```
 Sample response
 ```
 {'status': True, 'error': False, 'data': [{'Clientid': 'Your Client ID', 'Password': None, 'ApiKey':'Your API Key', 'ApiSecret': 'Your API Secret', 'Totp': 'na', 'AccountName': 'Your Account Name', 'LastLogin': '2024-04-03', 'UCC': 'Your Unique User Code', 'Chatid': 'Your Chat ID', 'BotKeys': 'Your Telegram Bot Key', 'Sessionid': 'Your Session ID', 'Trade': 'Y', 'Broker': 'Your Broker', 'Redirecturl': 'http://spark.maticalgos.com/auth_code/<Your Broker>', 'Pin': 'na'}], 'message': 'Data Received'}
 ```
 
 ## Account Management
@@ -315,19 +312,20 @@
 | StrategyType    | 'Intraday', 'Positional' | String    | Type of strategy (Intraday or Positional)      |
 | Display         | 'Private', 'Public'     | String    | Display setting for the strategy               |
 | ForwardTest     | 'Y', 'N'                | String    | Whether forward testing is enabled             |
 
 ## Linked Strategies
 1. [Link Account to Strategy](#link-account-to-strategy)
 2. [Get Linked Strategies](#get-linked-strategies)
-3. [Modify Linked Strategy](#modify-linked-strategy)
+3. [Get Linked Strategies By Account](#get-linked-strategies-by-account)
+4. [Modify Linked Strategy](#modify-linked-strategy)
    1. Modify Linked Strategy
    2. Activate Linked Strategy
    3. Deactivate Linked Strategy
-4. [Delete Linked Strategy](#delete-linked-strategy)
+5. [Delete Linked Strategy](#delete-linked-strategy)
 
 
 ### Link Account to Strategy
 ```python
 print(spark.addlinkStrategy(strategyName='Your Strategy Name',
                             accountName='Your Account Name',
                             Multiplier=1,
@@ -346,14 +344,24 @@
 ```
 
 Sample response
 ```
 {'status': True, 'error': False, 'data': [{'StrategyName': 'Your Strategy Name', 'AccountName': 'Your Account Name', 'UCC': 'Your UCC', 'Multiplier': 1, 'Activate': 1, 'Capital': 0.0}], 'message': 'Data Received'}
 ```
 
+### Get Linked Strategies By Account
+```python
+print(spark.spark.getlinkStrategyAccount(accountName='Your Account Name'))
+```
+
+Sample response
+```
+{'status': True, 'error': False, 'data': [{'StrategyName': 'Your Strategy Name', 'AccountName': 'Your Account Name', 'UCC': 'Your UCC', 'Multiplier': 1, 'Activate': 1, 'Capital': 0.0}], 'message': 'Data Received'}
+```
+
 ### Modify Linked Strategy
 ```python
 # Modify Linked Strategy
 print(spark.modifyLinkedStrategy(strategyName='Your Strategy Name',
                                 accountName='Your Account Name',
                                 Multiplier=1,
                                 Activate='Y',
@@ -445,17 +453,21 @@
 ## Order Management
 1. [LTP](#LTP)
 1. [Place order](#place-an-order)
 2. [Modify order](#modify-order)
 3. [Cancel order](#cancel-an-order)
 4. [Square off All Orders](#square-off)
 5. [Cancel All Orders](#cancel-all-orders)
-6. [Orderbook](#orderbook)
-7. [Tradebook](#get-tradebook)
-8. [Netposition](#netposition)
+6. [Stop Operation](#stop-operation)
+7. [Square Off Single](#square-off-single)
+8. [Delete Trade](#delete-order)
+9. [Manual Square Off](#manual-square-off)
+10. [Orderbook](#orderbook)
+11. [Tradebook](#get-tradebook)
+12. [Netposition](#netposition)
 
 ### LTP
 Get the last traded price of the token.
 Token format is 'Exchange:Token'
 ```python
 print(spark.ltp(Tokens='NSE:212'))
 ```
@@ -465,30 +477,30 @@
 1. Limit Order
 2. Market Order
 3. SL-Limit Order
 
 Code
 ```python
 # Limit Order
-print(spark_object.place_order(strategyName = "Your Strategy Name",
+print(spark.place_order(strategyName = "Your Strategy Name",
                                 transType = "Buy",
                                 token = "NSE:212", 
                                 qty = 1,
                                 orderType = "Limit",
                                 productType = "Intraday",
                                 limitPrice = 500.0))
 # Market Order
-print(spark_object.place_order(strategyName = "Your Strategy Name",
+print(spark.place_order(strategyName = "Your Strategy Name",
                                transType = "Sell",
                                token = "NSE:212",
                                qty = 1,
                                orderType = "Market",
                                productType = "Intraday"))
 # SL-Limit Order
-print(spark_object.place_order(strategyName = "Your Strategy Name",
+print(spark.place_order(strategyName = "Your Strategy Name",
                                transType = "Buy",
                                token = "NSE:212",
                                qty = 1,
                                orderType = "SL-Limit",
                                productType = "Intraday",
                                triggerPrice = 220,
                                limitPrice = 210))
@@ -508,27 +520,27 @@
 | productType     | "Intraday", "Delivery"             | String    | Product type (Intraday, Delivery, etc.)              |
 | limitPrice      | Float                              | Float     | Price specified for Limit and SL-Limit orders         |
 | triggerPrice    | Float                              | Float     | Trigger price specified for SL-Limit orders          |
 | strefID         | Integer                            | Integer   | Reference ID of the order placed                      |
 
 #### Modify Order
 ```python
-print(spark_object.modify_order(strategyName='Your Strategy Name',
+print(spark.modify_order(strategyName='Your Strategy Name',
                                 strefID=2328,
                                 orderType='SL-Limit',
                                 limitPrice=190))
 ```
 Sample response of modify order
 ```
 {'status': True, 'error': False, 'data': [{'strefID': 2328}], 'message': 'Order Modified.'}
 ```
 
 #### Cancel order
 ```python
-print(spark_object.cancel_order(strategyName='Your Strategy Name',strefID=2328))
+print(spark.cancel_order(strategyName='Your Strategy Name',strefID=2328))
 ```
 Sample response of cancel order
 ```
 {'status': True, 'error': True, 'data': [{'strefID': 2328}], 'message': 'Order Cancelled.'}
 ```
 
 ### Square off
@@ -555,47 +567,89 @@
 
 response
 ```
 {'status': True, 'error': False, 'data': [], 'message': 'Request sent to Cancel All Orders in StrategyName : Your Strategy Name with AccountName : Your Account Name'}
 {'status': True, 'error': False, 'data': [], 'message': 'Request sent to Cancel All Orders in AccountNamme : Your Account Name'}
 ```
 
+### Stop Operation
+
+```python
+print(spark.stopOperation(strategyName='Your Strategy Name', strefID='Your order Reference ID'))
+```
+
+Sample response
+```
+{'status': True, 'error': False, 'data': [{'strefID':Your order Reference ID }], 'message': 'Operations stopped on {Your order Reference ID}'}
+```
+
+### Square Off Single
+```python
+print(spark.squareOffSingle(accountName='You Account Name', strategyName='Your Strategy Name', token='NSE:13528', positionType='Intraday', at_limit='true'))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[{"strefID":308}],"message":"Order Placed, Position Squared off"}
+```
+
+### Delete Trade
+```python
+print(spark.deleteTrade(TDno='Your Trade Number'))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[],"message":"Trade Deleted"}
+```
+
+### Manual Square Off
+```python
+print(spark.manualSquareOff(accountName='Your Account Name', strategyName='Your Strategy Name', token='NSE:13528', positionType='Intraday', tradedPrice=0, tradedAt=0, ordersPlaced=0, qty=1))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[],"message":"Position closed manually."}
+```
+
+
 ### orderbook
 ```python
-print(spark_object.orderbook(accountName='Your Account Name',
+print(spark.orderbook(accountName='Your Account Name',
                              strategyName='Your Strategy Name',
                              strefid=2000, # Optional : order id
                              reftag='Your Reference Tag', # Optional : Reference Tag    
                              withorders='Y')) # Optional : 'Y' to get all orders 
-print(spark_object.orderbook(accountName='Your Account Name',
+print(spark.orderbook(accountName='Your Account Name',
                              strategyName='Your Strategy Name'))
 ```
 
 Sample response
 ```
 {'status': True, 'error': False, 'data': [{'UCC': 'Your UCC', 'AccountName': 'Your Account Name', 'strefID': 2240, 'reftag': 1939, 'StrategyName': 'Your Strategy Name', 'orderType': 'Limit', 'productType': 'Intraday', 'price': 171.25, 'limitPrice': 170.0, 'triggerPrice': 0.0, 'token': 'NSE:212', 'segment': 'C', 'symbol': 'ASHOKLEY-EQ', 'qty': 1, 'transType': 'Buy', 'splitby': 0, 'Operations': '{"timeLimit": 0, "shouldExecute": false, "priceBuffer": 0.0}', 'ordersplaced': 1, 'ordersdone': 1, 'ordersexecuted': 0, 'placed_at': '2024-03-29T10:54:08', 'recon_at': None, 'trade_at': None, 'filledQty': 0, 'tradedQty': None, 'tradeValue': None, 'tradePrice': 0.0, 'status': 'Error', 'active': 0, 'ForwardTest': None}], 'message': 'Data received'}
 ```
 
 ### Get tradebook
 ```python
-print(spark_object.tradebook(startDate='2024-04-01',
+print(spark.tradebook(startDate='2024-04-01',
                              endDate='2024-04-03',
                              strategyName='Your Strategy Name',
                              accountName='Your Account Name'))
 
 ```
 
 Sample response
 ```
 {'status': True, 'error': False, 'data': [], 'message': 'Tradebook data received'}
 ```
 
 ### Netposition
 ```python
-print(spark_object.netposition(accountName='Your Account Name',
+print(spark.netposition(accountName='Your Account Name',
                                strategyName='Your Strategy Name'))
 ```
 
 Sample response
 ```
 {'status': True, 'error': False, 'data': [{'Your Account Name': {'bookedpnl': 0.816660000000013, 'openpnl': None, 'totalpnl': None, 'totalpositions': 1, 'openpositions': 1}}], 'message': 'Data Received'}
 ```
@@ -606,14 +660,50 @@
 ```
 
 Sample response
 ```
 {'status': True, 'error': True, 'data': [{'Datetime': '2024-04-06T09:36:00', 'UCC': 'Your UCC', 'Name': 'Strategy Name', 'Alert Type': 'DEBUG', 'Message': "Endpoint Called : ModifyOrder. Payload Received : {'UCC': 'Your UCC', 'StrategyName': 'Strategy Name', 'strefID': 2327, 'orderType': 'Market', 'limitPrice': 0.0, 'triggerPrice': 0.0, 'identifier': ''}"}], 'message': 'Data Received'}
 ```
 
+### Reconnect Order Websocket
+```python
+print(spark.reconnect_orderWS(accountName='Your Account Name'))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[],"message":"Reconnecting to WS"}
+```
+
+### Holiday List
+```python
+print(spark.isHoliday(exch='NFO'))
+```
+
+Sample response
+```
+{'status': True, 'error': False, 'data': ['2024-04-02', '2024-04-06', '2024-04-13', '2024-04-14', '2024-04-19', '2024-04-21', '2024-04-28'], 'message': 'Data Received'}
+```
+
+### Freeze Quantity
+```python
+print(spark.freezeqty(symbol='BANKNIFTY'))
+```
+
+Sample response
+```
+{"status":true,"error":false,"data":[{"freezeQty":900}],"message":"Data Received"}
+```
+
+### Contract Master File
+```python
+print(spark.contractMaster())
+```
+
+
 ## Sample Code
 ```python
 from SparkLib import SparkLib
 
 if __name__ == '__main__':
     spark = SparkLib(userid = 'Your User ID', password = 'Your Password', apikeys = 'Your API Keys')
     spark.generate_token()
@@ -628,14 +718,17 @@
                             limitPrice = 210,
                            ))
     print(spark.modifyorder(strategyName='Your Strategy Name',
                             strefID=2328,
                             orderType='SL-Limit',
                             limitPrice=190))
     print(spark.cancelorder(strategyName='Your Strategy Name',strefID=2328))
+    print(spark.stopOperation(strategyName='Your Strategy Name', strefID='Your order Reference ID'))
+    print(spark.deleteTrade(TDno='Your Trade Number'))
+    print(spark.manualSquareOff(accountName='Your Account Name', strategyName='Your Strategy Name', token='NSE:13528', positionType='Intraday', tradedPrice=0, tradedAt=0, ordersPlaced=0, qty=1))    
 
     print(spark.getExpiry(symbol='NIFTY',exchange='NFO',instrument='OPT'))
     print(spark.getExpiry(symbol='SBIN',exchange='NFO',instrument='FUT'))
     print(spark.getExpiry(symbol='SENSEX',exchange='BFO',instrument='FUT'))
     print(spark.getExpiry(symbol='SENSEX',exchange='BFO',instrument='OPT'))
     print(spark.getExpiry(symbol='USDINR',exchange='CDS',instrument='FUT'))
 
@@ -671,26 +764,36 @@
     print(spark.deletelinkStrategy(strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.CancalAll(ctype='strategy',strategyName='Your Strategy Name',accountName='Your Account Name'))
     print(spark.CancalAll(ctype='account',accountName='Your Account Name'))
 
     print(spark.SquareOff(ctype='strategy',strategyName='Your Strategy Name',accountName='Your Account Name'))
     print(spark.SquareOff(ctype='account',accountName='Your Account Name'))
-
+    print(spark.squareOffSingle(accountName='You Account Name', strategyName='Your Strategy Name', token='NSE:13528', positionType='Intraday', at_limit='true'))
+    
     print(spark.ltp(Tokens='NSE:212'))
 
     print(spark.intradaypnl(strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.netposition(strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.tradebook(startDate='2024-04-01',endDate='2024-04-04',strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.orderbook(strategyName='Your Strategy Name',accountName='Your Account Name'))
 
     print(spark.excutionLogs())
+
+    print(spark.reconnect_orderWS(accountName='Your Account Name'))
+    
+    print(spark.isHoliday(exch='NFO'))
+    
+    print(spark.freezeqty(symbol='BANKNIFTY'))
+    
+    print(spark.contractMaster())
+
 ```
 
 
 
 # Order Websocket
 
 The order websocket is a real-time communication protocol used to receive order-related messages from the Spark platform. It provides users with updates on order status, execution, and other pertinent information related to their trading activity. The websocket operates by continuously listening for incoming messages from the Spark platform and relaying them to the user in real-time.
@@ -755,8 +858,8 @@
   - This parameter specifies the maximum number of reconnection attempts that the websocket should make before giving up. By default, it is set to 20.
 - **access_token**: 
   - This parameter specifies the access token required to establish a connection to the Spark platform.
 - **connect()**: 
   - This method is used to establish a connection to the Spark platform using the access token.
 - **close_connection()**: 
   - This method is used to close the websocket connection to the Spark platform.
-  
+
```

### Comparing `maticalgos-spark-0.1.5/setup.py` & `maticalgos-spark-0.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "readme.md").read_text()
 
 setup(
 name='maticalgos-spark',
-version='0.1.5',
+version='0.1.6',
 author='Niraj Munot',
 author_email='nirajmunot28@gmail.com',
 description='SparkLib is a Python client library for interacting with https://spark.maticalgos.com . It provides functionalities to manage accounts, strategies, place orders, and much more.',
 long_description=long_description,
 long_description_content_type='text/markdown',
 packages=find_packages(),
 classifiers=[
```

### Comparing `maticalgos-spark-0.1.5/testWS.py` & `maticalgos-spark-0.1.6/testWS.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 
-from maticalgos_spark import OrderSocket
+from maticalgos.sparkLib import OrderSocket
 # from sparkLib import SparkLib
 import time
 
 def on_order(message):
     print('test message', message)
 
 def on_error(error):
```

