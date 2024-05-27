# Comparing `tmp/nfinance-0.4.2.tar.gz` & `tmp/nfinance-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nfinance-0.4.2.tar", last modified: Thu May 23 07:22:06 2024, max compression
+gzip compressed data, was "nfinance-0.4.3.tar", last modified: Mon May 27 08:18:51 2024, max compression
```

## Comparing `nfinance-0.4.2.tar` & `nfinance-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:22:06.661685 nfinance-0.4.2/
--rw-r--r--   0 root         (0) root         (0)     1064 2024-05-23 07:19:34.000000 nfinance-0.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3562 2024-05-23 07:22:06.661685 nfinance-0.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2962 2024-05-23 07:19:34.000000 nfinance-0.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:22:06.659685 nfinance-0.4.2/nfinance/
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-23 07:19:34.000000 nfinance-0.4.2/nfinance/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-05-23 07:19:34.000000 nfinance-0.4.2/nfinance/financials.py
--rw-r--r--   0 root         (0) root         (0)      481 2024-05-23 07:19:34.000000 nfinance-0.4.2/nfinance/rsi.py
--rw-r--r--   0 root         (0) root         (0)     1727 2024-05-23 07:19:34.000000 nfinance-0.4.2/nfinance/stock_data.py
--rw-r--r--   0 root         (0) root         (0)     3914 2024-05-23 07:20:24.000000 nfinance-0.4.2/nfinance/stock_listing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:22:06.660685 nfinance-0.4.2/nfinance.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3562 2024-05-23 07:22:06.000000 nfinance-0.4.2/nfinance.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      337 2024-05-23 07:22:06.000000 nfinance-0.4.2/nfinance.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 07:22:06.000000 nfinance-0.4.2/nfinance.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-23 07:22:06.000000 nfinance-0.4.2/nfinance.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-23 07:22:06.000000 nfinance-0.4.2/nfinance.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 07:22:06.661685 nfinance-0.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-23 07:20:03.000000 nfinance-0.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 07:22:06.661685 nfinance-0.4.2/tests/
--rw-r--r--   0 root         (0) root         (0)       45 2024-05-23 07:19:34.000000 nfinance-0.4.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1485 2024-05-23 07:19:34.000000 nfinance-0.4.2/tests/test_stock_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:18:51.701624 nfinance-0.4.3/
+-rw-r--r--   0 root         (0) root         (0)     1064 2024-05-27 08:16:35.000000 nfinance-0.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3562 2024-05-27 08:18:51.701624 nfinance-0.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-05-27 08:16:35.000000 nfinance-0.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:18:51.699623 nfinance-0.4.3/nfinance/
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-27 08:16:35.000000 nfinance-0.4.3/nfinance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-05-27 08:16:35.000000 nfinance-0.4.3/nfinance/financials.py
+-rw-r--r--   0 root         (0) root         (0)      481 2024-05-27 08:16:35.000000 nfinance-0.4.3/nfinance/rsi.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2024-05-27 08:16:35.000000 nfinance-0.4.3/nfinance/stock_data.py
+-rw-r--r--   0 root         (0) root         (0)     4027 2024-05-27 08:17:13.000000 nfinance-0.4.3/nfinance/stock_listing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:18:51.700624 nfinance-0.4.3/nfinance.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3562 2024-05-27 08:18:51.000000 nfinance-0.4.3/nfinance.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-27 08:18:51.000000 nfinance-0.4.3/nfinance.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 08:18:51.000000 nfinance-0.4.3/nfinance.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-27 08:18:51.000000 nfinance-0.4.3/nfinance.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-27 08:18:51.000000 nfinance-0.4.3/nfinance.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 08:18:51.701624 nfinance-0.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-27 08:16:54.000000 nfinance-0.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 08:18:51.700624 nfinance-0.4.3/tests/
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-27 08:16:35.000000 nfinance-0.4.3/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-05-27 08:16:35.000000 nfinance-0.4.3/tests/test_stock_data.py
```

### Comparing `nfinance-0.4.2/LICENSE` & `nfinance-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nfinance-0.4.2/PKG-INFO` & `nfinance-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfinance
-Version: 0.4.2
+Version: 0.4.3
 Summary: A simple finance data fetching library for Naver Finance data.
 Home-page: https://github.com/lega001/nfinance
 Author: lega001
 Author-email: lega01077970523@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nfinance-0.4.2/README.md` & `nfinance-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `nfinance-0.4.2/nfinance/financials.py` & `nfinance-0.4.3/nfinance/financials.py`

 * *Files identical despite different names*

### Comparing `nfinance-0.4.2/nfinance/stock_data.py` & `nfinance-0.4.3/nfinance/stock_data.py`

 * *Files identical despite different names*

### Comparing `nfinance-0.4.2/nfinance/stock_listing.py` & `nfinance-0.4.3/nfinance/stock_listing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import requests
 import pandas as pd
 from tqdm import tqdm
 
 class StockListing:
     def __init__(self, market):
         self.market = market
@@ -24,15 +23,15 @@
             "largeCode": "https://api.stock.naver.com/etf/priceTop?page={page}&pageSize=20&{market}"
         }
         if self.market.startswith('largeCode'):
             self.url = self.base_urls.get("largeCode")
         else:
             self.url = self.base_urls.get(self.market.split('=')[0], "https://m.stock.naver.com/api/stocks/marketValue/{market}?page={page}&pageSize=20")
 
-    def fetch_stocks(self):
+    def fetch_stocks(self, show_progress=False):
         special_stock_list = ['.DJI', '.INX', '.SOX']
         special_stock_pages = {'.DJI': 4, '.INX': 51, '.SOX': 4}
 
         if self.market in special_stock_list:
             total_pages = special_stock_pages[self.market]
             page_size = 10
         else:
@@ -42,15 +41,15 @@
             json_data = response.json()
             total_stocks = json_data.get('totalCount', 0)
             total_pages = (total_stocks // 20) + 1 if total_stocks % 20 != 0 else total_stocks // 20
             page_size = 20
 
         stocks = []
 
-        for page in tqdm(range(1, total_pages + 1), desc=f"Fetching {self.market} stocks"):
+        for page in tqdm(range(1, total_pages + 1), desc=f"Fetching {self.market} stocks", disable=not show_progress):
             formatted_url = self.url.format(market=self.market, page=page)
             response = requests.get(formatted_url)
             if response.status_code != 200:
                 continue  # Skip to next iteration if there's an error
             json_data = response.json()
             if self.market == 'etf' or self.market.startswith('largeCode'):
                 new_stocks = pd.json_normalize(json_data.get("etfs", []))
@@ -60,16 +59,16 @@
                 stocks.append(new_stocks)
 
         return pd.concat(stocks, ignore_index=True) if stocks else pd.DataFrame()
 
     def __str__(self):
         return f'StockListing for {self.market}'
 
-# Example usage:
+# Example usage with progress bar enabled:
 # listing = StockListing("KOSPI")
-# stocks_df = listing.fetch_stocks()
+# stocks_df = listing.fetch_stocks(show_progress=True)
 # print(stocks_df)
 
-# Special stocks fetching example:
+# Example usage without progress bar:
 # listing = StockListing(".DJI")
-# stocks_df = listing.fetch_stocks()
+# stocks_df = listing.fetch_stocks(show_progress=False)
 # stocks_df.to_csv('.DJI.csv', index=False)
```

### Comparing `nfinance-0.4.2/nfinance.egg-info/PKG-INFO` & `nfinance-0.4.3/nfinance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfinance
-Version: 0.4.2
+Version: 0.4.3
 Summary: A simple finance data fetching library for Naver Finance data.
 Home-page: https://github.com/lega001/nfinance
 Author: lega001
 Author-email: lega01077970523@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nfinance-0.4.2/setup.py` & `nfinance-0.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='nfinance',
-    version='0.4.2',
+    version='0.4.3',
     author='lega001',
     author_email='lega01077970523@gmail.com',
     packages=find_packages(),
     install_requires=[
         'pandas',  # 예시: pandas 라이브러리가 필요한 경우
         'requests',  # 예시: HTTP 요청을 위해 requests 라이브러리가 필요한 경우
         'tqdm',
```

### Comparing `nfinance-0.4.2/tests/test_stock_data.py` & `nfinance-0.4.3/tests/test_stock_data.py`

 * *Files identical despite different names*

