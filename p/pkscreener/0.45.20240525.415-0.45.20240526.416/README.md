# Comparing `tmp/pkscreener-0.45.20240525.415.tar.gz` & `tmp/pkscreener-0.45.20240526.416.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240525.415.tar", last modified: Sat May 25 18:49:41 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240526.416.tar", last modified: Sun May 26 22:22:20 2024, max compression
```

## Comparing `pkscreener-0.45.20240525.415.tar` & `pkscreener-0.45.20240526.416.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:49:41.363372 pkscreener-0.45.20240525.415/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/LICENSE-Others
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-25 18:49:41.363372 pkscreener-0.45.20240525.415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:49:41.359372 pkscreener-0.45.20240525.415/pkscreener/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:49:41.363372 pkscreener-0.45.20240525.415/pkscreener/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/ArtTexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Barometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/CandlePatterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)    33644 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/MarketMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/MarketStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    44414 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/MenuOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/OtaUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PKScanRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PKScheduledTaskProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PKScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PKSpreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PKTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    18470 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Pktalib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PortfolioXRay.py
--rw-r--r--   0 runner    (1001) docker     (127)   154008 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/ScreeningStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    55902 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/StockScreener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/UserMenuChoicesHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    84541 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/WorkflowManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-25 18:49:35.000000 pkscreener-0.45.20240525.415/pkscreener/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/courbd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   144558 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/pkscreener.ini
--rw-r--r--   0 runner    (1001) docker     (127)    53262 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/pkscreenerbot.py
--rw-r--r--   0 runner    (1001) docker     (127)    33987 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/pkscreenercli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:49:41.359372 pkscreener-0.45.20240525.415/pkscreener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-25 18:49:41.363372 pkscreener-0.45.20240525.415/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:22:20.604101 pkscreener-0.45.20240526.416/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/LICENSE-Others
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-26 22:22:20.604101 pkscreener-0.45.20240526.416/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:22:20.600101 pkscreener-0.45.20240526.416/pkscreener/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:22:20.604101 pkscreener-0.45.20240526.416/pkscreener/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/ArtTexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Barometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/CandlePatterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33644 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/MarketMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/MarketStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44414 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/MenuOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/OtaUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PKScanRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PKScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PKSpreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PKTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18470 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Pktalib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PortfolioXRay.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154008 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/ScreeningStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55902 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/StockScreener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85488 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/WorkflowManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-26 22:22:14.000000 pkscreener-0.45.20240526.416/pkscreener/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/courbd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   145155 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/pkscreener.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    53262 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/pkscreenerbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33987 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/pkscreenercli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:22:20.600101 pkscreener-0.45.20240526.416/pkscreener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-26 22:22:20.604101 pkscreener-0.45.20240526.416/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/setup.py
```

### Comparing `pkscreener-0.45.20240525.415/LICENSE` & `pkscreener-0.45.20240526.416/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/LICENSE-Others` & `pkscreener-0.45.20240526.416/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/PKG-INFO` & `pkscreener-0.45.20240526.416/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240525.415
+Version: 0.45.20240526.416
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240525.415.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240526.416.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240525.415/README.md` & `pkscreener-0.45.20240526.416/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240525.415/pkscreener/__init__.py` & `pkscreener-0.45.20240526.416/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,36 +154,44 @@
         except Exception as e:# pragma: no cover
             default_logger().debug(e, exc_info=True)
             pass
 
     # Print about developers and repository
     def showDevInfo(defaultAnswer=None):
         OutputControls().printOutput("\n" + Changelog.changelog())
-        devInfo = "\n[+] Developer: PK (PKScreener)"
-        versionInfo = "[+] Version: %s" % VERSION
-        homePage = "[+] Home Page: https://github.com/pkjmesra/PKScreener\n[+] Telegram Bot:@nse_pkscreener_bot\n[+] Channel:https://t.me/PKScreener\n[+] Discussions:https://t.me/PKScreeners"
+        devInfo = "\n[👨🏻‍💻] Developer: PK (PKScreener) 🇮🇳"
+        versionInfo = "[🚦] Version: %s" % VERSION
+        homePage = "[🏡] Home Page: https://github.com/pkjmesra/PKScreener\n[🤖] Telegram Bot:@nse_pkscreener_bot\n[🚨] Channel:https://t.me/PKScreener\n[💬] Discussions:https://t.me/PKScreeners"
         issuesInfo = (
-            "[+] Read/Post Issues here: https://github.com/pkjmesra/PKScreener/issues"
+            "[🚩] Read/Post Issues here: https://github.com/pkjmesra/PKScreener/issues"
         )
-        communityInfo = "[+] Join Community Discussions: https://github.com/pkjmesra/PKScreener/discussions"
-        latestInfo = "[+] Download latest software from https://github.com/pkjmesra/PKScreener/releases/latest"
+        communityInfo = "[📢] Join Community Discussions: https://github.com/pkjmesra/PKScreener/discussions"
+        latestInfo = "[⏰] Download latest software from https://github.com/pkjmesra/PKScreener/releases/latest"
+        donationInfo = "[💰] PKScreener is and will always remain free for everyone. Hosting servers and running services costs money.\n[💸] Please donate whatever you can: 8007162973@APL using UPI(India) or https://github.com/sponsors/pkjmesra 🙏🏻"
+        totalDownloads = "200k+"
+        respPepyTech = fetcher.fetchURL(url="https://static.pepy.tech/badge/pkscreener",headers={'user-agent': f'{random_user_agent()}'},timeout=2)
+        if respPepyTech is not None and respPepyTech.status_code == 200:
+            totalDownloads = respPepyTech.text.split("</text>")[-2].split(">")[-1]
+        downloadsInfo = f"[🔥] Total Downloads: {totalDownloads}"
         OutputControls().printOutput(colorText.BOLD + colorText.WARN + devInfo + colorText.END)
         OutputControls().printOutput(colorText.BOLD + colorText.WARN + versionInfo + colorText.END)
+        OutputControls().printOutput(colorText.BOLD + colorText.GREEN + downloadsInfo + colorText.END)
         OutputControls().printOutput(colorText.BOLD + homePage + colorText.END)
         OutputControls().printOutput(colorText.BOLD + colorText.FAIL + issuesInfo + colorText.END)
         OutputControls().printOutput(colorText.BOLD + colorText.GREEN + communityInfo + colorText.END)
         OutputControls().printOutput(colorText.BOLD + colorText.BLUE + latestInfo + colorText.END)
+        OutputControls().printOutput(colorText.BOLD + colorText.FAIL + donationInfo + colorText.END)
         if defaultAnswer is None:
             input(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] Press <Enter> to continue!"
                 + colorText.END
             )
-        return f"\n{Changelog.changelog()}\n\n{devInfo}\n{versionInfo}\n\n{homePage}\n{issuesInfo}\n{communityInfo}\n{latestInfo}"
+        return f"\n{Changelog.changelog()}\n\n{devInfo}\n{versionInfo}\n\n{downloadsInfo}\n{homePage}\n{issuesInfo}\n{communityInfo}\n{latestInfo}\n{donationInfo}"
 
     # Save last screened result to pickle file
     def setLastScreenedResults(df, df_save=None, choices=None):
         try:
             finalStocks = ""
             outputFolder = os.path.join(os.getcwd(),'actions-data-scan')
             if not os.path.isdir(outputFolder):
```

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/classes/keys.py` & `pkscreener-0.45.20240526.416/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/courbd.ttf` & `pkscreener-0.45.20240526.416/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/globals.py` & `pkscreener-0.45.20240526.416/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1206,14 +1206,28 @@
         ca_dfs = [dividend_df, bonus_df, stockSplit_df]
         listStockCodes = []
         for df in ca_dfs:
             df = df[
                 df["Stock"].astype(str).str.contains("BSE:") == False
             ]
             listStockCodes.extend(list(df["Stock"]))
+    if executeOption == 29 and not PKDateUtilities.isTradingTime():
+        message = "\n[👉🏻] Bid/Ask build up report can only be generated during trading hours."
+        OutputControls().printOutput(
+            colorText.BOLD
+            + colorText.FAIL
+            + message
+            + colorText.END
+        )
+        if defaultAnswer is None:
+            input("Press <Enter> to continue...")
+        if userPassedArgs is not None and userPassedArgs.user is not None:
+            sendMessageToTelegramChannel(message=message, user=userPassedArgs.user)
+        return None, None
+    
     if executeOption == 30:
         selectedMenu = m2.find(str(executeOption))
         if len(options) >= 4:
             if str(options[3]).isnumeric():
                 maLength = int(options[3])
             elif str(options[3]).upper() == "D":
                 maLength = 1
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pkscreener-0.45.20240525.415/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240526.416/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240526.416/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240526.416/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240526.416/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240525.415
+Version: 0.45.20240526.416
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240525.415.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240526.416.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240525.415/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240526.416/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.415/setup.py` & `pkscreener-0.45.20240526.416/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     long_description = fh.read()
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read().splitlines()
     install_requires.append("advanced_ta")
 
 if "Windows" in platform.system():
     install_requires = [
-        ".github/dependencies/TA_Lib-0.4.28-cp311-cp311-win_amd64.whl"
+        ".github/dependencies/TA_Lib-0.4.29-cp311-cp311-win_amd64.whl"
     ].extend(install_requires)
 elif "Linux" in platform.system():
     subprocess.Popen(["chmod", "+x", ".github/dependencies/build_tools/github/talib.sh"])
     subprocess.Popen("start .github/dependencies/build_tools/github/talib.sh", shell=True)
 # For Darwin, brew install ta-lib will work
 
 SYS_MAJOR_VERSION = str(sys.version_info.major)
```

