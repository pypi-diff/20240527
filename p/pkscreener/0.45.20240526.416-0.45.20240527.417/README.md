# Comparing `tmp/pkscreener-0.45.20240526.416.tar.gz` & `tmp/pkscreener-0.45.20240527.417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240526.416.tar", last modified: Sun May 26 22:22:20 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240527.417.tar", last modified: Mon May 27 08:33:11 2024, max compression
```

## Comparing `pkscreener-0.45.20240526.416.tar` & `pkscreener-0.45.20240527.417.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:22:20.604101 pkscreener-0.45.20240526.416/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/LICENSE-Others
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-26 22:22:20.604101 pkscreener-0.45.20240526.416/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:22:20.600101 pkscreener-0.45.20240526.416/pkscreener/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:22:20.604101 pkscreener-0.45.20240526.416/pkscreener/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/ArtTexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Barometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/CandlePatterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)    33644 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/MarketMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/MarketStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    44414 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/MenuOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/OtaUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PKScanRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PKScheduledTaskProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PKScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PKSpreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PKTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    18470 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Pktalib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/PortfolioXRay.py
--rw-r--r--   0 runner    (1001) docker     (127)   154008 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/ScreeningStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    55902 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/StockScreener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/UserMenuChoicesHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    85488 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/WorkflowManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-26 22:22:14.000000 pkscreener-0.45.20240526.416/pkscreener/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/classes/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/courbd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   145155 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/pkscreener.ini
--rw-r--r--   0 runner    (1001) docker     (127)    53262 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/pkscreenerbot.py
--rw-r--r--   0 runner    (1001) docker     (127)    33987 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/pkscreener/pkscreenercli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 22:22:20.600101 pkscreener-0.45.20240526.416/pkscreener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 22:22:20.000000 pkscreener-0.45.20240526.416/pkscreener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-26 22:22:20.604101 pkscreener-0.45.20240526.416/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-26 22:20:47.000000 pkscreener-0.45.20240526.416/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:33:11.791841 pkscreener-0.45.20240527.417/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/LICENSE-Others
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-27 08:33:11.791841 pkscreener-0.45.20240527.417/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:33:11.787841 pkscreener-0.45.20240527.417/pkscreener/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:33:11.791841 pkscreener-0.45.20240527.417/pkscreener/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/ArtTexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Barometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/CandlePatterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33644 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/MarketMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/MarketStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44414 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/MenuOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/OtaUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PKScanRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PKScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PKSpreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PKTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18470 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Pktalib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PortfolioXRay.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154008 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/ScreeningStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55902 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/StockScreener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85488 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/WorkflowManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 08:33:05.000000 pkscreener-0.45.20240527.417/pkscreener/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/courbd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   145155 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-27 08:31:40.000000 pkscreener-0.45.20240527.417/pkscreener/pkscreener.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    53262 2024-05-27 08:31:40.000000 pkscreener-0.45.20240527.417/pkscreener/pkscreenerbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33987 2024-05-27 08:31:40.000000 pkscreener-0.45.20240527.417/pkscreener/pkscreenercli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:33:11.787841 pkscreener-0.45.20240527.417/pkscreener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 08:33:11.791841 pkscreener-0.45.20240527.417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-27 08:31:40.000000 pkscreener-0.45.20240527.417/setup.py
```

### Comparing `pkscreener-0.45.20240526.416/LICENSE` & `pkscreener-0.45.20240527.417/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/LICENSE-Others` & `pkscreener-0.45.20240527.417/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/PKG-INFO` & `pkscreener-0.45.20240527.417/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240526.416
+Version: 0.45.20240527.417
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240526.416.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240527.417.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240526.416/README.md` & `pkscreener-0.45.20240527.417/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240526.416/pkscreener/__init__.py` & `pkscreener-0.45.20240527.417/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/WorkflowManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 + '","ref":"main"}}'
             )
     elif workflowType == "R":
         workflow_name = "w3-workflow-bot.yml"
         data = (
                 '{"ref":"'
                 + branch
-                + '","inputs":{"branch-name":"main"}}'
+                + '","inputs":{"branch-name":"main","cliOptions":""}}'
             )
     _, _, _, ghp_token = get_secrets()
     url = f"https://api.github.com/repos/{owner}/{repo}/actions/workflows/{workflow_name}/dispatches"
 
     headers = {
         "Accept": "application/vnd.github+json",
         "Authorization": f"Bearer {ghp_token}",
```

### Comparing `pkscreener-0.45.20240526.416/pkscreener/classes/keys.py` & `pkscreener-0.45.20240527.417/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/courbd.ttf` & `pkscreener-0.45.20240527.417/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/globals.py` & `pkscreener-0.45.20240527.417/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240527.417/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240527.417/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240527.417/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240527.417/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240526.416
+Version: 0.45.20240527.417
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240526.416.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240527.417.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.415/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240526.416/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240527.417/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240526.416/setup.py` & `pkscreener-0.45.20240527.417/setup.py`

 * *Files identical despite different names*

