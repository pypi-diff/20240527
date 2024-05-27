# Comparing `tmp/pkscreener-0.45.20240527.417.tar.gz` & `tmp/pkscreener-0.45.20240527.418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240527.417.tar", last modified: Mon May 27 08:33:11 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240527.418.tar", last modified: Mon May 27 21:27:14 2024, max compression
```

## Comparing `pkscreener-0.45.20240527.417.tar` & `pkscreener-0.45.20240527.418.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:33:11.791841 pkscreener-0.45.20240527.417/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/LICENSE-Others
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-27 08:33:11.791841 pkscreener-0.45.20240527.417/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:33:11.787841 pkscreener-0.45.20240527.417/pkscreener/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:33:11.791841 pkscreener-0.45.20240527.417/pkscreener/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/ArtTexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Barometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/CandlePatterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)    33644 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/MarketMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/MarketStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    44414 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/MenuOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/OtaUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PKScanRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PKScheduledTaskProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PKScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PKSpreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PKTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    18470 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Pktalib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/PortfolioXRay.py
--rw-r--r--   0 runner    (1001) docker     (127)   154008 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/ScreeningStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    55902 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/StockScreener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/UserMenuChoicesHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    85488 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/WorkflowManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 08:33:05.000000 pkscreener-0.45.20240527.417/pkscreener/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/classes/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/courbd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   145155 2024-05-27 08:31:39.000000 pkscreener-0.45.20240527.417/pkscreener/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-27 08:31:40.000000 pkscreener-0.45.20240527.417/pkscreener/pkscreener.ini
--rw-r--r--   0 runner    (1001) docker     (127)    53262 2024-05-27 08:31:40.000000 pkscreener-0.45.20240527.417/pkscreener/pkscreenerbot.py
--rw-r--r--   0 runner    (1001) docker     (127)    33987 2024-05-27 08:31:40.000000 pkscreener-0.45.20240527.417/pkscreener/pkscreenercli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:33:11.787841 pkscreener-0.45.20240527.417/pkscreener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 08:33:11.000000 pkscreener-0.45.20240527.417/pkscreener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 08:33:11.791841 pkscreener-0.45.20240527.417/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-27 08:31:40.000000 pkscreener-0.45.20240527.417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:27:14.356891 pkscreener-0.45.20240527.418/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/LICENSE-Others
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-27 21:27:14.356891 pkscreener-0.45.20240527.418/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:27:14.348892 pkscreener-0.45.20240527.418/pkscreener/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:27:14.356891 pkscreener-0.45.20240527.418/pkscreener/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/ArtTexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Barometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/CandlePatterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33678 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/MarketMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/MarketStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46722 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/MenuOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/OtaUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PKScanRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PKScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PKSpreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PKTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Pktalib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PortfolioXRay.py
+-rw-r--r--   0 runner    (1001) docker     (127)   158196 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/ScreeningStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56970 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/StockScreener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85524 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/WorkflowManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 21:27:08.000000 pkscreener-0.45.20240527.418/pkscreener/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/courbd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   145709 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/pkscreener.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    53279 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/pkscreenerbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33987 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/pkscreenercli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:27:14.352892 pkscreener-0.45.20240527.418/pkscreener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 21:27:14.356891 pkscreener-0.45.20240527.418/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-27 21:25:46.000000 pkscreener-0.45.20240527.418/setup.py
```

### Comparing `pkscreener-0.45.20240527.417/LICENSE` & `pkscreener-0.45.20240527.418/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/LICENSE-Others` & `pkscreener-0.45.20240527.418/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/PKG-INFO` & `pkscreener-0.45.20240527.418/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240527.417
+Version: 0.45.20240527.418
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240527.417.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240527.418.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240527.417/README.md` & `pkscreener-0.45.20240527.418/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240527.417/pkscreener/__init__.py` & `pkscreener-0.45.20240527.418/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/ConfigManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,18 +72,18 @@
         self.atrTrailingStopSensitivity = 1
         self.atrTrailingStopPeriod = 10
         self.atrTrailingStopEMAPeriod = 200
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
-        self.maxDashboardWidgetsPerRow = 5
+        self.maxDashboardWidgetsPerRow = 7
         self.maxNumResultRowsInMonitor = 3
         self.calculatersiintraday = False
-        self.defaultMonitorOptions = "X:12:9:2.5~X:12:23~X:12:28~X:12:31~|{1}X:0:23:>|X:0:27:>|X:0:31:~|{2}X:0:31:~|{3}X:0:27:~X:12:7:3:.01:1~|{5}X:0:5:0:35:~X:12:7:6:1~X:12:11:~X:12:12:i 5m~X:12:17~X:12:24~X:12:6:7:1~X:12:6:3~X:12:6:8~X:12:6:9~X:12:6:10:1~X:12:7:3:.02:1~X:12:13:i 1m~X:12:2~|{1}X:0:29:"
+        self.defaultMonitorOptions = "X:12:9:2.5~X:12:23~X:12:28~X:12:31~|{1}X:0:23:>|X:0:27:>|X:0:31:~|{2}X:0:31:~|{3}X:0:27:~X:12:7:3:.01:1~|{5}X:0:5:0:35:~X:12:7:6:1~X:12:11:~X:12:12:i 5m~X:12:17~X:12:24~X:12:6:7:1~X:12:6:3~X:12:6:8~X:12:6:9~X:12:2:>|X:12:7:8:>|X:12:7:9:1:1:~X:12:6:10:1~X:12:7:3:.02:1~X:12:13:i 1m~X:12:2~|{1}X:0:29:"
         self.minimumChangePercentage = 0
         self.daysToLookback = 22 * self.backtestPeriodFactor  # 1 month
         self.periods = [1,2,3,4,5,10,15,22,30]
         if self.maxBacktestWindow > self.periods[-1]:
             self.periods.extend(self.maxBacktestWindow)
 
     @property
```

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/MenuOptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,27 +57,30 @@
 }
 level1_P_MenuDict = {
     "1": "Predefined Piped Scanners",
     "2": "Define my custom Piped Scanner",
     "3": "Run Piped Scans Saved So Far",
     "M": "Back to the Top/Main menu",
 }
-PREDEFINED_SCAN_MENU_KEYS = ["1","2","3","4","5","6","7","8","9","10","11"]
+PREDEFINED_SCAN_MENU_KEYS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14"]
 PREDEFINED_SCAN_MENU_TEXTS = [
     "Volume Scanners | High Momentum | Breaking Out Now | ATR Cross     ",
     "Volume Scanners | High Momentum | ATR Cross",
     "Volume Scanners | High Momentum                                    ",
     "Volume Scanners | ATR Cross",
     "Volume Scanners | High Bid/Ask Build Up                            ",
     "High Momentum | ATR Cross",
     "High Momentum | ATR Trailing Stop                                  ",
     "ATR Cross | ATR Trailing Stop",
     "TTM Sqeeze Buy | Intraday RSI b/w 0 to 54                          ",
     "Volume Scanners | High Momentum | Breaking Out Now | ATR Cross | Intraday RSI b/w 0 to 54",
     "Volume Scanners | ATR Cross | Intraday RSI b/w 0 to 54             ",
+    "VCP (Mark Minervini) | Chart Patterns | MA Support",
+    "VCP | Chart Patterns | MA Support                                  ",
+    "Already Breaking out | VCP (Mark Minervini) | Chart Patterns | MA Support",
 ]
 level2_P_MenuDict = {}
 for key in PREDEFINED_SCAN_MENU_KEYS:
     level2_P_MenuDict[key] = PREDEFINED_SCAN_MENU_TEXTS[int(key)-1]
 level2_P_MenuDict["M"] = "Back to the Top/Main menu"
 PREDEFINED_SCAN_MENU_VALUES =[
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:23:>|X:0:27:'",
@@ -87,14 +90,17 @@
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:29:'",
     "--systemlaunched -a y -e -o 'X:12:31:>|X:0:27:'",
     "--systemlaunched -a y -e -o 'X:12:31:>|X:0:30:1:'",
     "--systemlaunched -a y -e -o 'X:12:27:>|X:0:30:1:'",
     "--systemlaunched -a y -e -o 'X:12:7:6:1:>|X:0:5:0:54:i 1m'",
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:31:>|X:0:23:>|X:0:27:>|X:0:5:0:54:i 1m'",
     "--systemlaunched -a y -e -o 'X:12:9:2.5:>|X:0:27:>|X:0:5:0:54:i 1m'",
+    "--systemlaunched -a y -e -o 'X:12:7:8:>|X:12:7:9:1:1:'",
+    "--systemlaunched -a y -e -o 'X:12:7:4:>|X:12:7:9:1:1:'",
+    "--systemlaunched -a y -e -o 'X:12:2:>|X:12:7:8:>|X:12:7:9:1:1:'"
 ]
 PIPED_SCANNERS = {}
 for key in PREDEFINED_SCAN_MENU_KEYS:
     PIPED_SCANNERS[key] = PREDEFINED_SCAN_MENU_VALUES[int(key)-1]
 
 level1_T_MenuDict = {
     "L": "Long Term",
@@ -202,17 +208,29 @@
     "0": "Cancel",
 }
 level3_X_ChartPattern_MenuDict = {
     "1": "Bullish Inside Bar (Flag) Pattern",
     "2": "Bearish Inside Bar (Flag) Pattern(Sell)",
     "3": "The Confluence (50 & 200 MA/EMA)",
     "4": "VCP (Volatility Contraction Pattern)",
-    "5": "Buying at Trendline (Ideal for Swing/Mid/Long term)",
+    "5": "Buying at Trendline Support (Ideal for Swing/Mid/Long term)",
     "6": "Bollinger Bands (TTM) Squeeze",
     "7": "Candle-stick Patterns",
+    "8": "VCP (Mark Minervini)",
+    "9": "Moving Average Signals",
+    "0": "Cancel",
+}
+
+level4_X_ChartPattern_MASignalMenuDict = {
+    "1": "MA-Support",
+    "2": "Bearish Signals",
+    "3": "Bullish Signals",
+    "4": "BearCross MA",
+    "5": "BullCross MA",
+    "6": "MA-Resist",
     "0": "Cancel",
 }
 
 level4_X_ChartPattern_BBands_SQZ_MenuDict = {
     "1": "TTM Squeeze-Buy",
     "2": "TTM In-Squeeze",
     "3": "TTM Squeeze-Sell",
@@ -578,14 +596,21 @@
                 if selectedMenu.parent.menuKey == "7" and selectedMenu.menuKey == "6":
                     return self.renderLevel4_X_ChartPattern_BBands_SQZ_Menus(
                         skip=skip,
                         asList=asList,
                         renderStyle=renderStyle,
                         parent=selectedMenu,
                     )
+                if selectedMenu.parent.menuKey == "7" and selectedMenu.menuKey == "9":
+                    return self.renderLevel4_X_ChartPattern_MASignal_Menus(
+                        skip=skip,
+                        asList=asList,
+                        renderStyle=renderStyle,
+                        parent=selectedMenu,
+                    )
                 
 
     def find(self, key=None):
         if key is not None:
             try:
                 return self.menuDict[str(key).upper()]
             except Exception as e:  # pragma: no cover
@@ -1151,15 +1176,48 @@
     Enter your choice > (default is """
                     + colorText.WARN
                     + (self.find("1") or menu().create('?','?')).keyTextLabel().strip() + ")"
                     + colorText.END
                 )
             return menuText
 
+    def renderLevel4_X_ChartPattern_MASignal_Menus(
+        self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
+    ):
+        menuText = self.fromDictionary(
+            level4_X_ChartPattern_MASignalMenuDict,
+            renderExceptionKeys=["0"],
+            renderStyle=renderStyle
+            if renderStyle is not None
+            else MenuRenderStyle.STANDALONE,
+            skip=skip,
+            parent=parent,
+        ).render(asList=asList, coloredValues=["1"])
+        if asList:
+            return menuText
+        else:
+            if OutputControls().enableMultipleLineOutput:
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + colorText.WARN
+                    + "[+] Select an option: "
+                    + colorText.END
+                )
+                OutputControls().printOutput(
+                    colorText.BOLD
+                    + menuText
+                    + """
 
+    Enter your choice > (default is """
+                    + colorText.WARN
+                    + (self.find("1") or menu().create('?','?')).keyTextLabel().strip() + ")"
+                    + colorText.END
+                )
+            return menuText
+        
     def renderLevel4_X_ChartPattern_Confluence_Menus(
         self, skip=[], asList=False, renderStyle=MenuRenderStyle.STANDALONE, parent=None
     ):
         menuText = self.fromDictionary(
             level4_X_ChartPattern_Confluence_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
```

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/Pktalib.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,23 @@
         try:
             return talib.ema(close, timeperiod)
         except Exception:  # pragma: no cover
             # default_logger().debug(e, exc_info=True)
             return talib.EMA(close, timeperiod)
 
     @classmethod
+    def VWAP(self, high, low, close, volume):
+        try:
+            import pandas_ta as talib
+            return talib.vwap(high, low, close, volume)
+        except Exception:  # pragma: no cover
+            # default_logger().debug(e, exc_info=True)
+            return None
+        
+    @classmethod
     def KeltnersChannel(self, high, low, close, timeperiod=20):
         try:
             low_kel = None
             upp_kel = None
             tr = pktalib.TRUERANGE(high, low, close)
             atr = pktalib.ATR(high, low, close, timeperiod=timeperiod)
             sma = pktalib.SMA(close=close, timeperiod=timeperiod)
@@ -114,14 +123,22 @@
         try:
             return talib.sma(close, timeperiod)
         except Exception:  # pragma: no cover
             # default_logger().debug(e, exc_info=True)
             return talib.SMA(close, timeperiod)
 
     @classmethod
+    def WMA(self, close, timeperiod):
+        try:
+            return talib.wma(close, timeperiod)
+        except Exception:  # pragma: no cover
+            # default_logger().debug(e, exc_info=True)
+            return talib.WMA(close, timeperiod)
+        
+    @classmethod
     def ATR(self, high, low, close, timeperiod=14):
         try:
             return talib.atr(high, low, close, length= timeperiod)
         except Exception:  # pragma: no cover
             # default_logger().debug(e, exc_info=True)
             return talib.ATR(high, low, close, timeperiod=timeperiod)
```

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/ScreeningStatistics.py`

 * *Files 3% similar despite different names*

```diff
@@ -3817,5810 +3817,6072 @@
 0000ee80: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
 0000ee90: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
 0000eea0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
 0000eeb0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
 0000eec0: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
 0000eed0: 206d 6152 616e 6765 203d 205b 392c 2031   maRange = [9, 1
 0000eee0: 302c 2032 302c 2035 302c 2032 3030 5d20  0, 20, 50, 200] 
-0000eef0: 6966 206d 614c 656e 6774 6820 6973 204e  if maLength is N
-0000ef00: 6f6e 6520 656c 7365 205b 6d61 4c65 6e67  one else [maLeng
-0000ef10: 7468 5d0a 2020 2020 2020 2020 7265 7375  th].        resu
-0000ef20: 6c74 7320 3d20 5b5d 0a20 2020 2020 2020  lts = [].       
-0000ef30: 2068 6173 5265 7665 7273 616c 7320 3d20   hasReversals = 
-0000ef40: 4661 6c73 650a 2020 2020 2020 2020 6461  False.        da
-0000ef50: 7461 203d 2064 6174 615b 3a3a 2d31 5d0a  ta = data[::-1].
-0000ef60: 2020 2020 2020 2020 7361 7665 6420 3d20          saved = 
-0000ef70: 7365 6c66 2e66 696e 6443 7572 7265 6e74  self.findCurrent
-0000ef80: 5361 7665 6456 616c 7565 2873 6372 6565  SavedValue(scree
-0000ef90: 6e44 6963 742c 7361 7665 4469 6374 2c20  nDict,saveDict, 
-0000efa0: 224d 412d 5369 676e 616c 2229 0a20 2020  "MA-Signal").   
-0000efb0: 2020 2020 2066 6f72 206d 614c 656e 6774       for maLengt
-0000efc0: 6820 696e 206d 6152 616e 6765 3a0a 2020  h in maRange:.  
-0000efd0: 2020 2020 2020 2020 2020 6461 7461 436f            dataCo
-0000efe0: 7079 203d 2064 6174 610a 2020 2020 2020  py = data.      
-0000eff0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-0000f000: 6e66 6967 4d61 6e61 6765 722e 7573 6545  nfigManager.useE
-0000f010: 4d41 206f 7220 6d61 4c65 6e67 7468 203d  MA or maLength =
-0000f020: 3d20 393a 0a20 2020 2020 2020 2020 2020  = 9:.           
-0000f030: 2020 2020 206d 6152 6576 203d 2070 6b74       maRev = pkt
-0000f040: 616c 6962 2e45 4d41 2864 6174 6143 6f70  alib.EMA(dataCop
-0000f050: 795b 2243 6c6f 7365 225d 2c20 7469 6d65  y["Close"], time
-0000f060: 7065 7269 6f64 3d6d 614c 656e 6774 6829  period=maLength)
-0000f070: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000f080: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000f090: 2020 206d 6152 6576 203d 2070 6b74 616c     maRev = pktal
-0000f0a0: 6962 2e4d 4128 6461 7461 436f 7079 5b22  ib.MA(dataCopy["
-0000f0b0: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-0000f0c0: 696f 643d 6d61 4c65 6e67 7468 290a 2020  iod=maLength).  
-0000f0d0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0000f0e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000f0f0: 6174 6143 6f70 792e 6472 6f70 2822 6d61  ataCopy.drop("ma
-0000f100: 5265 7622 2c20 6178 6973 3d31 2c20 696e  Rev", axis=1, in
-0000f110: 706c 6163 653d 5472 7565 2c20 6572 726f  place=True, erro
-0000f120: 7273 3d22 6967 6e6f 7265 2229 0a20 2020  rs="ignore").   
-0000f130: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-0000f140: 4578 6365 7074 696f 6e3a 2320 7072 6167  Exception:# prag
-0000f150: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
-0000f160: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-0000f170: 730a 2020 2020 2020 2020 2020 2020 6461  s.            da
-0000f180: 7461 436f 7079 2e69 6e73 6572 7428 6c65  taCopy.insert(le
-0000f190: 6e28 6461 7461 436f 7079 2e63 6f6c 756d  n(dataCopy.colum
-0000f1a0: 6e73 292c 2022 6d61 5265 7622 2c20 6d61  ns), "maRev", ma
-0000f1b0: 5265 7629 0a20 2020 2020 2020 2020 2020  Rev).           
-0000f1c0: 2064 6174 6143 6f70 7920 3d20 6461 7461   dataCopy = data
-0000f1d0: 436f 7079 5b3a 3a2d 315d 2e68 6561 6428  Copy[::-1].head(
-0000f1e0: 3429 0a20 2020 2020 2020 2020 2020 2062  4).            b
-0000f1f0: 756c 6c69 7368 4d41 5265 7665 7273 616c  ullishMAReversal
-0000f200: 203d 2064 6174 6143 6f70 795b 226d 6152   = dataCopy["maR
-0000f210: 6576 225d 2e69 6c6f 635b 305d 203e 3d20  ev"].iloc[0] >= 
-0000f220: 6461 7461 436f 7079 5b22 6d61 5265 7622  dataCopy["maRev"
-0000f230: 5d2e 696c 6f63 5b31 5d20 616e 6420 5c0a  ].iloc[1] and \.
-0000f240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f250: 6461 7461 436f 7079 5b22 6d61 5265 7622  dataCopy["maRev"
-0000f260: 5d2e 696c 6f63 5b31 5d20 3e3d 2064 6174  ].iloc[1] >= dat
-0000f270: 6143 6f70 795b 226d 6152 6576 225d 2e69  aCopy["maRev"].i
-0000f280: 6c6f 635b 325d 2061 6e64 205c 0a20 2020  loc[2] and \.   
-0000f290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2a0: 2064 6174 6143 6f70 795b 226d 6152 6576   dataCopy["maRev
-0000f2b0: 225d 2e69 6c6f 635b 325d 203c 2064 6174  "].iloc[2] < dat
-0000f2c0: 6143 6f70 795b 226d 6152 6576 225d 2e69  aCopy["maRev"].i
-0000f2d0: 6c6f 635b 335d 0a20 2020 2020 2020 2020  loc[3].         
-0000f2e0: 2020 2062 756c 6c69 7368 436c 6f73 6520     bullishClose 
-0000f2f0: 3d20 6461 7461 436f 7079 2e68 6561 6428  = dataCopy.head(
-0000f300: 3129 5b22 436c 6f73 6522 5d2e 696c 6f63  1)["Close"].iloc
-0000f310: 5b30 5d20 3e3d 2064 6174 6143 6f70 792e  [0] >= dataCopy.
-0000f320: 6865 6164 2831 295b 226d 6152 6576 225d  head(1)["maRev"]
-0000f330: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
-0000f340: 2020 2020 2062 6561 7269 7368 4d41 5265       bearishMARe
-0000f350: 7665 7273 616c 203d 2064 6174 6143 6f70  versal = dataCop
-0000f360: 795b 226d 6152 6576 225d 2e69 6c6f 635b  y["maRev"].iloc[
-0000f370: 305d 203c 3d20 6461 7461 436f 7079 5b22  0] <= dataCopy["
-0000f380: 6d61 5265 7622 5d2e 696c 6f63 5b31 5d20  maRev"].iloc[1] 
-0000f390: 616e 6420 5c0a 2020 2020 2020 2020 2020  and \.          
-0000f3a0: 2020 2020 2020 6461 7461 436f 7079 5b22        dataCopy["
-0000f3b0: 6d61 5265 7622 5d2e 696c 6f63 5b31 5d20  maRev"].iloc[1] 
-0000f3c0: 3c3d 2064 6174 6143 6f70 795b 226d 6152  <= dataCopy["maR
-0000f3d0: 6576 225d 2e69 6c6f 635b 325d 2061 6e64  ev"].iloc[2] and
-0000f3e0: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-0000f3f0: 2020 2020 2020 2064 6174 6143 6f70 795b         dataCopy[
-0000f400: 226d 6152 6576 225d 2e69 6c6f 635b 325d  "maRev"].iloc[2]
-0000f410: 203e 2064 6174 6143 6f70 795b 226d 6152   > dataCopy["maR
-0000f420: 6576 225d 2e69 6c6f 635b 335d 0a20 2020  ev"].iloc[3].   
-0000f430: 2020 2020 2020 2020 2069 7352 6563 656e           isRecen
-0000f440: 7443 6c6f 7365 5769 7468 696e 5065 7263  tCloseWithinPerc
-0000f450: 656e 7452 616e 6765 203d 2064 6174 6143  entRange = dataC
-0000f460: 6f70 792e 6571 7561 6c73 2864 6174 6143  opy.equals(dataC
-0000f470: 6f70 795b 2864 6174 6143 6f70 792e 436c  opy[(dataCopy.Cl
-0000f480: 6f73 6520 3e3d 2028 6461 7461 436f 7079  ose >= (dataCopy
-0000f490: 2e6d 6152 6576 202d 2028 6461 7461 436f  .maRev - (dataCo
-0000f4a0: 7079 2e6d 6152 6576 202a 2070 6572 6365  py.maRev * perce
-0000f4b0: 6e74 6167 6529 2929 2026 2028 6461 7461  ntage))) & (data
-0000f4c0: 436f 7079 2e43 6c6f 7365 203c 3d20 2864  Copy.Close <= (d
-0000f4d0: 6174 6143 6f70 792e 6d61 5265 7620 2b20  ataCopy.maRev + 
-0000f4e0: 2864 6174 6143 6f70 792e 6d61 5265 7620  (dataCopy.maRev 
-0000f4f0: 2a20 7065 7263 656e 7461 6765 2929 295d  * percentage)))]
-0000f500: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000f510: 2028 6973 5265 6365 6e74 436c 6f73 6557   (isRecentCloseW
-0000f520: 6974 6869 6e50 6572 6365 6e74 5261 6e67  ithinPercentRang
-0000f530: 6520 616e 6420 6275 6c6c 6973 6843 6c6f  e and bullishClo
-0000f540: 7365 2061 6e64 2062 756c 6c69 7368 4d41  se and bullishMA
-0000f550: 5265 7665 7273 616c 2920 6f72 205c 0a20  Reversal) or \. 
-0000f560: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0000f570: 6973 5265 6365 6e74 436c 6f73 6557 6974  isRecentCloseWit
-0000f580: 6869 6e50 6572 6365 6e74 5261 6e67 6520  hinPercentRange 
-0000f590: 616e 6420 6e6f 7420 6275 6c6c 6973 6843  and not bullishC
-0000f5a0: 6c6f 7365 2061 6e64 2062 6561 7269 7368  lose and bearish
-0000f5b0: 4d41 5265 7665 7273 616c 293a 0a20 2020  MAReversal):.   
-0000f5c0: 2020 2020 2020 2020 2020 2020 2068 6173               has
-0000f5d0: 5265 7665 7273 616c 7320 3d20 5472 7565  Reversals = True
-0000f5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f5f0: 2072 6573 756c 7473 2e61 7070 656e 6428   results.append(
-0000f600: 7374 7228 6d61 4c65 6e67 7468 2929 0a20  str(maLength)). 
-0000f610: 2020 2020 2020 2069 6620 6861 7352 6576         if hasRev
-0000f620: 6572 7361 6c73 3a0a 2020 2020 2020 2020  ersals:.        
-0000f630: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-0000f640: 4d41 2d53 6967 6e61 6c22 5d20 3d20 280a  MA-Signal"] = (.
-0000f650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f660: 7361 7665 645b 305d 200a 2020 2020 2020  saved[0] .      
-0000f670: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0000f680: 7254 6578 742e 424f 4c44 0a20 2020 2020  rText.BOLD.     
-0000f690: 2020 2020 2020 2020 2020 202b 2028 636f             + (co
-0000f6a0: 6c6f 7254 6578 742e 4752 4545 4e20 6966  lorText.GREEN if
-0000f6b0: 2062 756c 6c69 7368 4d41 5265 7665 7273   bullishMARevers
-0000f6c0: 616c 2065 6c73 6520 2863 6f6c 6f72 5465  al else (colorTe
-0000f6d0: 7874 2e46 4149 4c20 6966 2062 6561 7269  xt.FAIL if beari
-0000f6e0: 7368 4d41 5265 7665 7273 616c 2065 6c73  shMAReversal els
-0000f6f0: 6520 636f 6c6f 7254 6578 742e 5741 524e  e colorText.WARN
-0000f700: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0000f710: 2020 202b 2066 2252 6576 6572 7361 6c2d     + f"Reversal-
-0000f720: 5b7b 272c 272e 6a6f 696e 2872 6573 756c  [{','.join(resul
-0000f730: 7473 297d 5d7b 2745 4d41 2720 6966 2028  ts)}]{'EMA' if (
-0000f740: 6d61 4c65 6e67 7468 203d 3d20 3920 6f72  maLength == 9 or
-0000f750: 2073 656c 662e 636f 6e66 6967 4d61 6e61   self.configMana
-0000f760: 6765 722e 7573 6545 4d41 2920 656c 7365  ger.useEMA) else
-0000f770: 2027 4d41 277d 220a 2020 2020 2020 2020   'MA'}".        
-0000f780: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-0000f790: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
-0000f7a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000f7b0: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-0000f7c0: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-0000f7d0: 315d 202b 2066 2252 6576 6572 7361 6c2d  1] + f"Reversal-
-0000f7e0: 5b7b 272c 272e 6a6f 696e 2872 6573 756c  [{','.join(resul
-0000f7f0: 7473 297d 5d7b 2745 4d41 2720 6966 2028  ts)}]{'EMA' if (
-0000f800: 6d61 4c65 6e67 7468 203d 3d20 3920 6f72  maLength == 9 or
-0000f810: 2073 656c 662e 636f 6e66 6967 4d61 6e61   self.configMana
-0000f820: 6765 722e 7573 6545 4d41 2920 656c 7365  ger.useEMA) else
-0000f830: 2027 4d41 277d 220a 2020 2020 2020 2020   'MA'}".        
-0000f840: 7265 7475 726e 2068 6173 5265 7665 7273  return hasRevers
-0000f850: 616c 730a 0a20 2020 2064 6566 2066 696e  als..    def fin
-0000f860: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
-0000f870: 7565 2873 656c 662c 2073 6372 6565 6e44  ue(self, screenD
-0000f880: 6963 742c 2073 6176 6544 6963 742c 206b  ict, saveDict, k
-0000f890: 6579 293a 0a20 2020 2020 2020 2065 7869  ey):.        exi
-0000f8a0: 7374 696e 6753 6372 6565 6e20 3d20 7363  stingScreen = sc
-0000f8b0: 7265 656e 4469 6374 2e67 6574 286b 6579  reenDict.get(key
-0000f8c0: 290a 2020 2020 2020 2020 6578 6973 7469  ).        existi
-0000f8d0: 6e67 5361 7665 203d 2073 6176 6544 6963  ngSave = saveDic
-0000f8e0: 742e 6765 7428 6b65 7929 0a20 2020 2020  t.get(key).     
-0000f8f0: 2020 2065 7869 7374 696e 6753 6372 6565     existingScree
-0000f900: 6e20 3d20 6622 7b65 7869 7374 696e 6753  n = f"{existingS
-0000f910: 6372 6565 6e7d 2c20 2220 6966 2028 6578  creen}, " if (ex
-0000f920: 6973 7469 6e67 5363 7265 656e 2069 7320  istingScreen is 
-0000f930: 6e6f 7420 4e6f 6e65 2061 6e64 206c 656e  not None and len
-0000f940: 2865 7869 7374 696e 6753 6372 6565 6e29  (existingScreen)
-0000f950: 203e 2030 2920 656c 7365 2022 220a 2020   > 0) else "".  
-0000f960: 2020 2020 2020 6578 6973 7469 6e67 5361        existingSa
-0000f970: 7665 203d 2066 227b 6578 6973 7469 6e67  ve = f"{existing
-0000f980: 5361 7665 7d2c 2022 2069 6620 2865 7869  Save}, " if (exi
-0000f990: 7374 696e 6753 6176 6520 6973 206e 6f74  stingSave is not
-0000f9a0: 204e 6f6e 6520 616e 6420 6c65 6e28 6578   None and len(ex
-0000f9b0: 6973 7469 6e67 5361 7665 2920 3e20 3029  istingSave) > 0)
-0000f9c0: 2065 6c73 6520 2222 0a20 2020 2020 2020   else "".       
-0000f9d0: 2072 6574 7572 6e20 6578 6973 7469 6e67   return existing
-0000f9e0: 5363 7265 656e 2c20 6578 6973 7469 6e67  Screen, existing
-0000f9f0: 5361 7665 0a0a 2020 2020 2320 406d 6561  Save..    # @mea
-0000fa00: 7375 7265 5f74 696d 650a 2020 2020 6465  sure_time.    de
-0000fa10: 6620 6669 6e64 4262 616e 6473 5371 7565  f findBbandsSque
-0000fa20: 657a 6528 7365 6c66 2c66 756c 6c44 6174  eze(self,fullDat
-0000fa30: 612c 2073 6372 6565 6e44 6963 742c 2073  a, screenDict, s
-0000fa40: 6176 6544 6963 742c 2066 696c 7465 723d  aveDict, filter=
-0000fa50: 3429 3a0a 2020 2020 2020 2020 2222 220a  4):.        """.
-0000fa60: 2020 2020 2020 2020 5468 6520 5454 4d20          The TTM 
-0000fa70: 5371 7565 657a 6520 696e 6469 6361 746f  Squeeze indicato
-0000fa80: 7220 6d65 6173 7572 6573 2074 6865 2072  r measures the r
-0000fa90: 656c 6174 696f 6e73 6869 7020 6265 7477  elationship betw
-0000faa0: 6565 6e20 7468 6520 0a20 2020 2020 2020  een the .       
-0000fab0: 2042 6f6c 6c69 6e67 6572 2042 616e 6473   Bollinger Bands
-0000fac0: 2061 6e64 204b 656c 746e 6572 2773 2043   and Keltner's C
-0000fad0: 6861 6e6e 656c 2e20 5768 656e 2074 6865  hannel. When the
-0000fae0: 2076 6f6c 6174 696c 6974 7920 696e 6372   volatility incr
-0000faf0: 6561 7365 732c 200a 2020 2020 2020 2020  eases, .        
-0000fb00: 736f 2064 6f65 7320 7468 6520 6469 7374  so does the dist
-0000fb10: 616e 6365 2062 6574 7765 656e 2074 6865  ance between the
-0000fb20: 2062 616e 6473 2c20 616e 6420 636f 6e76   bands, and conv
-0000fb30: 6572 7365 6c79 2c20 7768 656e 2074 6865  ersely, when the
-0000fb40: 200a 2020 2020 2020 2020 766f 6c61 7469   .        volati
-0000fb50: 6c69 7479 2064 6563 6c69 6e65 732c 2074  lity declines, t
-0000fb60: 6865 2064 6973 7461 6e63 6520 616c 736f  he distance also
-0000fb70: 2064 6563 7265 6173 6573 2e20 5468 6520   decreases. The 
-0000fb80: 5371 7565 657a 6520 696e 6469 6361 746f  Squeeze indicato
-0000fb90: 7220 0a20 2020 2020 2020 2066 696e 6473  r .        finds
-0000fba0: 2073 6563 7469 6f6e 7320 6f66 2074 6865   sections of the
-0000fbb0: 2042 6f6c 6c69 6e67 6572 2042 616e 6473   Bollinger Bands
-0000fbc0: 2073 7475 6479 2077 6869 6368 2066 616c   study which fal
-0000fbd0: 6c20 696e 7369 6465 2074 6865 200a 2020  l inside the .  
-0000fbe0: 2020 2020 2020 4b65 6c74 6e65 7227 7320        Keltner's 
-0000fbf0: 4368 616e 6e65 6c73 2e0a 2020 2020 2020  Channels..      
-0000fc00: 2020 0a20 2020 2020 2020 2041 7420 7468    .        At th
-0000fc10: 6520 6d6f 6d65 6e74 2074 6869 7320 7371  e moment this sq
-0000fc20: 7565 657a 6520 6861 7070 656e 732c 2061  ueeze happens, a
-0000fc30: 2070 7269 6365 2062 7265 616b 6f75 7420   price breakout 
-0000fc40: 6672 6f6d 2074 6865 2075 7070 6572 200a  from the upper .
-0000fc50: 2020 2020 2020 2020 426f 6c6c 696e 6765          Bollinge
-0000fc60: 7220 4261 6e64 2077 6f75 6c64 2069 6e64  r Band would ind
-0000fc70: 6963 6174 6520 7468 6520 706f 7373 6962  icate the possib
-0000fc80: 696c 6974 7920 6f66 2061 6e20 7570 7472  ility of an uptr
-0000fc90: 656e 6420 696e 2074 6865 200a 2020 2020  end in the .    
-0000fca0: 2020 2020 6675 7475 7265 2e20 5468 6973      future. This
-0000fcb0: 2069 7320 6261 636b 6564 2062 7920 7468   is backed by th
-0000fcc0: 6520 6661 6374 2074 6861 7420 6f6e 6365  e fact that once
-0000fcd0: 2074 6865 2070 7269 6365 2073 7461 7274   the price start
-0000fce0: 7320 6272 6561 6b69 6e67 200a 2020 2020  s breaking .    
-0000fcf0: 2020 2020 6f75 7420 6f66 2074 6865 2062      out of the b
-0000fd00: 616e 6473 2c20 6974 2077 6f75 6c64 206d  ands, it would m
-0000fd10: 6561 6e20 6120 7265 6c61 7861 7469 6f6e  ean a relaxation
-0000fd20: 206f 6620 7468 6520 7371 7565 657a 6520   of the squeeze 
-0000fd30: 616e 6420 7468 6520 0a20 2020 2020 2020  and the .       
-0000fd40: 2070 6f73 7369 6269 6c69 7479 206f 6620   possibility of 
-0000fd50: 6869 6768 206d 6172 6b65 7420 766f 6c61  high market vola
-0000fd60: 7469 6c69 7479 2061 6e64 2070 7269 6365  tility and price
-0000fd70: 206d 6f76 656d 656e 7420 696e 2074 6865   movement in the
-0000fd80: 2066 7574 7572 652e 200a 2020 2020 2020   future. .      
-0000fd90: 2020 5369 6d69 6c61 726c 792c 2061 2070    Similarly, a p
-0000fda0: 7269 6365 2062 7265 616b 6f75 7420 6672  rice breakout fr
-0000fdb0: 6f6d 2074 6865 206c 6f77 6572 2042 6f6c  om the lower Bol
-0000fdc0: 6c69 6e67 6572 2042 616e 6420 6166 7465  linger Band afte
-0000fdd0: 7220 6120 7371 7565 657a 6520 0a20 2020  r a squeeze .   
-0000fde0: 2020 2020 2077 6f75 6c64 2069 6e64 6963       would indic
-0000fdf0: 6174 6520 7468 6520 706f 7373 6962 696c  ate the possibil
-0000fe00: 6974 7920 6f66 2061 2064 6f77 6e74 7265  ity of a downtre
-0000fe10: 6e64 2069 6e20 7468 6520 6675 7475 7265  nd in the future
-0000fe20: 2061 6e64 2061 6e20 0a20 2020 2020 2020   and an .       
-0000fe30: 2069 6e63 7265 6173 6564 206d 6172 6b65   increased marke
-0000fe40: 7420 766f 6c61 7469 6c69 7479 2069 6e20  t volatility in 
-0000fe50: 7468 6520 7361 6d65 2064 6972 6563 7469  the same directi
-0000fe60: 6f6e 2e20 5768 656e 2074 6865 206d 6172  on. When the mar
-0000fe70: 6b65 7420 0a20 2020 2020 2020 2066 696e  ket .        fin
-0000fe80: 6973 6865 7320 6120 6d6f 7665 2c20 7468  ishes a move, th
-0000fe90: 6520 696e 6469 6361 746f 7220 7475 726e  e indicator turn
-0000fea0: 7320 6f66 662c 2077 6869 6368 2063 6f72  s off, which cor
-0000feb0: 7265 7370 6f6e 6473 2074 6f20 6261 6e64  responds to band
-0000fec0: 7320 0a20 2020 2020 2020 2068 6176 696e  s .        havin
-0000fed0: 6720 7075 7368 6564 2077 656c 6c20 6f75  g pushed well ou
-0000fee0: 7473 6964 6520 7468 6520 7261 6e67 6520  tside the range 
-0000fef0: 6f66 204b 656c 746e 6572 2773 2043 6861  of Keltner's Cha
-0000ff00: 6e6e 656c 732e 0a20 2020 2020 2020 2022  nnels..        "
-0000ff10: 2222 0a20 2020 2020 2020 2069 6620 6675  "".        if fu
-0000ff20: 6c6c 4461 7461 2069 7320 4e6f 6e65 206f  llData is None o
-0000ff30: 7220 6c65 6e28 6675 6c6c 4461 7461 2920  r len(fullData) 
-0000ff40: 3c20 3230 3a0a 2020 2020 2020 2020 2020  < 20:.          
-0000ff50: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-0000ff60: 2020 2020 2020 206f 6c64 6573 7452 6563         oldestRec
-0000ff70: 6f72 6473 4669 7273 745f 6466 203d 2066  ordsFirst_df = f
-0000ff80: 756c 6c44 6174 612e 6865 6164 2833 3029  ullData.head(30)
-0000ff90: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
-0000ffa0: 6c61 7465 7374 5265 636f 7264 7346 6972  latestRecordsFir
-0000ffb0: 7374 5f64 6620 3d20 6f6c 6465 7374 5265  st_df = oldestRe
-0000ffc0: 636f 7264 7346 6972 7374 5f64 665b 3a3a  cordsFirst_df[::
-0000ffd0: 2d31 5d2e 7461 696c 2833 3029 0a20 2020  -1].tail(30).   
-0000ffe0: 2020 2020 206c 6174 6573 7452 6563 6f72       latestRecor
-0000fff0: 6473 4669 7273 745f 6466 203d 206c 6174  dsFirst_df = lat
-00010000: 6573 7452 6563 6f72 6473 4669 7273 745f  estRecordsFirst_
-00010010: 6466 2e66 696c 6c6e 6128 3029 0a20 2020  df.fillna(0).   
-00010020: 2020 2020 206c 6174 6573 7452 6563 6f72       latestRecor
-00010030: 6473 4669 7273 745f 6466 203d 206c 6174  dsFirst_df = lat
-00010040: 6573 7452 6563 6f72 6473 4669 7273 745f  estRecordsFirst_
-00010050: 6466 2e72 6570 6c61 6365 285b 6e70 2e69  df.replace([np.i
-00010060: 6e66 2c20 2d6e 702e 696e 665d 2c20 3029  nf, -np.inf], 0)
-00010070: 0a20 2020 2020 2020 2023 2042 6f6c 6c69  .        # Bolli
-00010080: 6e67 6572 2062 616e 6473 0a20 2020 2020  nger bands.     
-00010090: 2020 206c 6174 6573 7452 6563 6f72 6473     latestRecords
-000100a0: 4669 7273 745f 6466 2e6c 6f63 5b3a 2c27  First_df.loc[:,'
-000100b0: 4242 616e 6473 2d55 275d 2c20 6c61 7465  BBands-U'], late
-000100c0: 7374 5265 636f 7264 7346 6972 7374 5f64  stRecordsFirst_d
-000100d0: 662e 6c6f 635b 3a2c 2742 4261 6e64 732d  f.loc[:,'BBands-
-000100e0: 4d27 5d2c 206c 6174 6573 7452 6563 6f72  M'], latestRecor
-000100f0: 6473 4669 7273 745f 6466 2e6c 6f63 5b3a  dsFirst_df.loc[:
-00010100: 2c27 4242 616e 6473 2d4c 275d 203d 2070  ,'BBands-L'] = p
-00010110: 6b74 616c 6962 2e42 4241 4e44 5328 6c61  ktalib.BBANDS(la
-00010120: 7465 7374 5265 636f 7264 7346 6972 7374  testRecordsFirst
-00010130: 5f64 665b 2243 6c6f 7365 225d 2c20 3230  _df["Close"], 20
-00010140: 290a 2020 2020 2020 2020 2320 636f 6d70  ).        # comp
-00010150: 7574 6520 4b65 6c74 6e65 7227 7320 6368  ute Keltner's ch
-00010160: 616e 6e65 6c0a 2020 2020 2020 2020 6c61  annel.        la
-00010170: 7465 7374 5265 636f 7264 7346 6972 7374  testRecordsFirst
-00010180: 5f64 665b 276c 6f77 5f6b 656c 275d 2c20  _df['low_kel'], 
-00010190: 6c61 7465 7374 5265 636f 7264 7346 6972  latestRecordsFir
-000101a0: 7374 5f64 665b 2775 7070 5f6b 656c 275d  st_df['upp_kel']
-000101b0: 203d 2070 6b74 616c 6962 2e4b 656c 746e   = pktalib.Keltn
-000101c0: 6572 7343 6861 6e6e 656c 286c 6174 6573  ersChannel(lates
-000101d0: 7452 6563 6f72 6473 4669 7273 745f 6466  tRecordsFirst_df
-000101e0: 5b22 4869 6768 225d 2c20 6c61 7465 7374  ["High"], latest
-000101f0: 5265 636f 7264 7346 6972 7374 5f64 665b  RecordsFirst_df[
-00010200: 224c 6f77 225d 2c6c 6174 6573 7452 6563  "Low"],latestRec
-00010210: 6f72 6473 4669 7273 745f 6466 5b22 436c  ordsFirst_df["Cl
-00010220: 6f73 6522 5d2c 3230 290a 2020 2020 2020  ose"],20).      
-00010230: 2020 2320 7371 7565 657a 6520 696e 6469    # squeeze indi
-00010240: 6361 746f 720a 2020 2020 2020 2020 6465  cator.        de
-00010250: 6620 696e 5f73 7175 6565 7a65 2864 6629  f in_squeeze(df)
-00010260: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00010270: 7475 726e 2064 665b 276c 6f77 5f6b 656c  turn df['low_kel
-00010280: 275d 203c 2064 665b 2742 4261 6e64 732d  '] < df['BBands-
-00010290: 4c27 5d20 3c20 6466 5b27 4242 616e 6473  L'] < df['BBands
-000102a0: 2d55 275d 203c 2064 665b 2775 7070 5f6b  -U'] < df['upp_k
-000102b0: 656c 275d 0a0a 2020 2020 2020 2020 6c61  el']..        la
-000102c0: 7465 7374 5265 636f 7264 7346 6972 7374  testRecordsFirst
-000102d0: 5f64 665b 2773 7175 6565 7a65 275d 203d  _df['squeeze'] =
-000102e0: 206c 6174 6573 7452 6563 6f72 6473 4669   latestRecordsFi
-000102f0: 7273 745f 6466 2e61 7070 6c79 2869 6e5f  rst_df.apply(in_
-00010300: 7371 7565 657a 652c 2061 7869 733d 3129  squeeze, axis=1)
-00010310: 0a0a 2020 2020 2020 2020 2320 4c65 7427  ..        # Let'
-00010320: 7320 7265 7669 6577 206a 7573 7420 7468  s review just th
-00010330: 6520 7072 6576 696f 7573 2033 2063 616e  e previous 3 can
-00010340: 646c 6573 2069 6e63 6c75 6469 6e67 2074  dles including t
-00010350: 6f64 6179 2028 6174 2074 6865 2065 6e64  oday (at the end
-00010360: 290a 2020 2020 2020 2020 6c61 7465 7374  ).        latest
-00010370: 5265 636f 7264 7346 6972 7374 5f64 6620  RecordsFirst_df 
-00010380: 3d20 6c61 7465 7374 5265 636f 7264 7346  = latestRecordsF
-00010390: 6972 7374 5f64 662e 7461 696c 2833 290a  irst_df.tail(3).
-000103a0: 2020 2020 2020 2020 2320 7374 6f63 6b20          # stock 
-000103b0: 6973 2063 6f6d 696e 6720 6f75 7420 6f66  is coming out of
-000103c0: 2074 6865 2073 7175 6565 7a65 0a20 2020   the squeeze.   
-000103d0: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
-000103e0: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
-000103f0: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
-00010400: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
-00010410: 6174 7465 726e 2229 0a20 2020 2020 2020  attern").       
-00010420: 2063 616e 646c 6533 5371 7a20 3d20 6c61   candle3Sqz = la
-00010430: 7465 7374 5265 636f 7264 7346 6972 7374  testRecordsFirst
-00010440: 5f64 662e 696c 6f63 5b2d 335d 5b22 7371  _df.iloc[-3]["sq
-00010450: 7565 657a 6522 5d0a 2020 2020 2020 2020  ueeze"].        
-00010460: 6361 6e64 6c65 3153 717a 203d 206c 6174  candle1Sqz = lat
-00010470: 6573 7452 6563 6f72 6473 4669 7273 745f  estRecordsFirst_
-00010480: 6466 2e69 6c6f 635b 2d31 5d5b 2273 7175  df.iloc[-1]["squ
-00010490: 6565 7a65 225d 0a20 2020 2020 2020 2063  eeze"].        c
-000104a0: 616e 646c 6532 5371 7a20 3d20 6c61 7465  andle2Sqz = late
-000104b0: 7374 5265 636f 7264 7346 6972 7374 5f64  stRecordsFirst_d
-000104c0: 662e 696c 6f63 5b2d 325d 5b22 7371 7565  f.iloc[-2]["sque
-000104d0: 657a 6522 5d0a 2020 2020 2020 2020 6966  eze"].        if
-000104e0: 2063 616e 646c 6533 5371 7a20 616e 6420   candle3Sqz and 
-000104f0: 6e6f 7420 6361 6e64 6c65 3153 717a 3a0a  not candle1Sqz:.
-00010500: 2020 2020 2020 2020 2020 2020 2320 3372              # 3r
-00010510: 6420 6361 6e64 6c65 2066 726f 6d20 7468  d candle from th
-00010520: 6520 6d6f 7374 2072 6563 656e 7420 6f6e  e most recent on
-00010530: 6520 7761 7320 696e 2073 7175 6565 7a65  e was in squeeze
-00010540: 2062 7574 2074 6865 206d 6f73 7420 7265   but the most re
-00010550: 6365 6e74 206f 6e65 2069 7320 6e6f 742e  cent one is not.
-00010560: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00010570: 6669 6c74 6572 206e 6f74 2069 6e20 5b31  filter not in [1
-00010580: 2c33 2c34 5d3a 2023 2042 7579 2f53 656c  ,3,4]: # Buy/Sel
-00010590: 6c2f 416c 6c0a 2020 2020 2020 2020 2020  l/All.          
-000105a0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-000105b0: 7365 0a20 2020 2020 2020 2020 2020 2023  se.            #
-000105c0: 2064 6563 6964 6520 7768 6963 6820 6163   decide which ac
-000105d0: 7469 6f6e 2074 6f20 7461 6b65 2062 7920  tion to take by 
-000105e0: 636f 6d70 6172 696e 6720 6469 7374 616e  comparing distan
-000105f0: 6365 7320 2020 2020 2020 2020 2020 2020  ces             
-00010600: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00010610: 6469 7374 616e 6365 5f74 6f5f 7570 7065  distance_to_uppe
-00010620: 7220 3d20 6162 7328 6c61 7465 7374 5265  r = abs(latestRe
-00010630: 636f 7264 7346 6972 7374 5f64 665b 2742  cordsFirst_df['B
-00010640: 4261 6e64 732d 5527 5d2e 7661 6c75 6573  Bands-U'].values
-00010650: 5b2d 315d 202d 206c 6174 6573 7452 6563  [-1] - latestRec
-00010660: 6f72 6473 4669 7273 745f 6466 5b27 436c  ordsFirst_df['Cl
-00010670: 6f73 6527 5d2e 7661 6c75 6573 5b2d 315d  ose'].values[-1]
-00010680: 290a 2020 2020 2020 2020 2020 2020 6469  ).            di
-00010690: 7374 616e 6365 5f74 6f5f 6c6f 7765 7220  stance_to_lower 
-000106a0: 3d20 6162 7328 6c61 7465 7374 5265 636f  = abs(latestReco
-000106b0: 7264 7346 6972 7374 5f64 665b 2742 4261  rdsFirst_df['BBa
-000106c0: 6e64 732d 4c27 5d2e 7661 6c75 6573 5b2d  nds-L'].values[-
-000106d0: 315d 202d 206c 6174 6573 7452 6563 6f72  1] - latestRecor
-000106e0: 6473 4669 7273 745f 6466 5b27 436c 6f73  dsFirst_df['Clos
-000106f0: 6527 5d2e 7661 6c75 6573 5b2d 315d 290a  e'].values[-1]).
-00010700: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00010710: 2020 2020 2020 2020 2061 6374 696f 6e20           action 
-00010720: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-00010730: 2020 2020 6966 2064 6973 7461 6e63 655f      if distance_
-00010740: 746f 5f75 7070 6572 203c 2064 6973 7461  to_upper < dista
-00010750: 6e63 655f 746f 5f6c 6f77 6572 3a0a 2020  nce_to_lower:.  
-00010760: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010770: 2066 696c 7465 7220 6e6f 7420 696e 205b   filter not in [
-00010780: 312c 345d 3a20 2320 4275 792f 416c 6c0a  1,4]: # Buy/All.
-00010790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107a0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000107b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000107c0: 2061 6374 696f 6e20 3d20 5472 7565 0a20   action = True. 
-000107d0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000107e0: 6669 6c74 6572 206e 6f74 2069 6e20 5b33  filter not in [3
-000107f0: 2c34 5d3a 2023 2053 656c 6c2f 416c 6c0a  ,4]: # Sell/All.
-00010800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010810: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-00010820: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00010830: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
-00010840: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
-00010850: 7254 6578 742e 424f 4c44 202b 2028 636f  rText.BOLD + (co
-00010860: 6c6f 7254 6578 742e 4752 4545 4e20 6966  lorText.GREEN if
-00010870: 2061 6374 696f 6e20 656c 7365 2063 6f6c   action else col
-00010880: 6f72 5465 7874 2e46 4149 4c29 202b 2066  orText.FAIL) + f
-00010890: 2242 4261 6e64 732d 5351 5a2d 7b27 4275  "BBands-SQZ-{'Bu
-000108a0: 7927 2069 6620 6163 7469 6f6e 2065 6c73  y' if action els
-000108b0: 6520 2753 656c 6c27 7d22 202b 2063 6f6c  e 'Sell'}" + col
-000108c0: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
-000108d0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-000108e0: 2250 6174 7465 726e 225d 203d 2073 6176  "Pattern"] = sav
-000108f0: 6564 5b31 5d20 2b20 6622 5454 4d2d 5351  ed[1] + f"TTM-SQ
-00010900: 5a2d 7b27 4275 7927 2069 6620 6163 7469  Z-{'Buy' if acti
-00010910: 6f6e 2065 6c73 6520 2753 656c 6c27 7d22  on else 'Sell'}"
-00010920: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00010930: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
-00010940: 2065 6c69 6620 6361 6e64 6c65 3353 717a   elif candle3Sqz
-00010950: 2061 6e64 2063 616e 646c 6532 5371 7a20   and candle2Sqz 
-00010960: 616e 6420 6361 6e64 6c65 3153 717a 3a0a  and candle1Sqz:.
-00010970: 2020 2020 2020 2020 2020 2020 2320 4c61              # La
-00010980: 7374 2033 2063 616e 646c 6573 2069 6e20  st 3 candles in 
-00010990: 7371 7565 657a 650a 2020 2020 2020 2020  squeeze.        
-000109a0: 2020 2020 6966 2066 696c 7465 7220 6e6f      if filter no
-000109b0: 7420 696e 205b 322c 345d 3a20 2320 5371  t in [2,4]: # Sq
-000109c0: 5a2f 416c 6c0a 2020 2020 2020 2020 2020  Z/All.          
-000109d0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-000109e0: 7365 0a20 2020 2020 2020 2020 2020 2073  se.            s
-000109f0: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
-00010a00: 726e 225d 203d 2066 277b 7361 7665 645b  rn"] = f'{saved[
-00010a10: 305d 7d7b 636f 6c6f 7254 6578 742e 424f  0]}{colorText.BO
-00010a20: 4c44 7d7b 636f 6c6f 7254 6578 742e 5741  LD}{colorText.WA
-00010a30: 524e 7d54 544d 2d53 515a 7b63 6f6c 6f72  RN}TTM-SQZ{color
-00010a40: 5465 7874 2e45 4e44 7d27 0a20 2020 2020  Text.END}'.     
-00010a50: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-00010a60: 2250 6174 7465 726e 225d 203d 2066 277b  "Pattern"] = f'{
-00010a70: 7361 7665 645b 315d 7d54 544d 2d53 515a  saved[1]}TTM-SQZ
-00010a80: 270a 2020 2020 2020 2020 2020 2020 7265  '.            re
-00010a90: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-00010aa0: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-00010ab0: 2020 2020 6465 6620 6669 6e64 496e 7472      def findIntr
-00010ac0: 6164 6179 4869 6768 4372 6f73 736f 7665  adayHighCrossove
-00010ad0: 7228 7365 6c66 2c20 6466 2c20 6166 7465  r(self, df, afte
-00010ae0: 7254 696d 6573 7461 6d70 3d4e 6f6e 6529  rTimestamp=None)
-00010af0: 3a0a 2020 2020 2020 2020 6966 2064 6620  :.        if df 
-00010b00: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-00010b10: 6629 203d 3d20 303a 0a20 2020 2020 2020  f) == 0:.       
-00010b20: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00010b30: 650a 2020 2020 2020 2020 6461 7461 203d  e.        data =
-00010b40: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
-00010b50: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
-00010b60: 696c 6c6e 6128 3029 0a20 2020 2020 2020  illna(0).       
-00010b70: 2064 6174 6120 3d20 6461 7461 2e72 6570   data = data.rep
-00010b80: 6c61 6365 285b 6e70 2e69 6e66 2c20 2d6e  lace([np.inf, -n
-00010b90: 702e 696e 665d 2c20 3029 0a20 2020 2020  p.inf], 0).     
-00010ba0: 2020 2064 6174 6120 3d20 6461 7461 5b3a     data = data[:
-00010bb0: 3a2d 315d 2020 2320 5265 7665 7273 6520  :-1]  # Reverse 
-00010bc0: 7468 6520 6461 7461 6672 616d 6520 736f  the dataframe so
-00010bd0: 2074 6861 7420 6974 7320 7468 6520 6f6c   that its the ol
-00010be0: 6465 7374 2064 6174 6520 6669 7273 740a  dest date first.
-00010bf0: 2020 2020 2020 2020 6469 6666 5f64 6620          diff_df 
-00010c00: 3d20 4e6f 6e65 0a20 2020 2020 2020 2074  = None.        t
-00010c10: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00010c20: 2320 4c65 7427 7320 6f6e 6c79 2063 6f6e  # Let's only con
-00010c30: 7369 6465 7220 7468 6f73 6520 6361 6e64  sider those cand
-00010c40: 6c65 7320 7468 6174 2061 7265 2061 6674  les that are aft
-00010c50: 6572 2074 6865 2061 6c65 7274 2069 7373  er the alert iss
-00010c60: 7565 2d74 696d 6520 696e 2074 6865 206d  ue-time in the m
-00010c70: 6f72 6e69 6e67 7320 2b20 3220 6361 6e64  ornings + 2 cand
-00010c80: 6c65 7320 2866 6f72 2062 7579 2f73 656c  les (for buy/sel
-00010c90: 6c29 0a20 2020 2020 2020 2020 2020 2064  l).            d
-00010ca0: 6966 665f 6466 203d 2064 6174 615b 6461  iff_df = data[da
-00010cb0: 7461 2e69 6e64 6578 203e 3d20 2070 642e  ta.index >=  pd.
-00010cc0: 746f 5f64 6174 6574 696d 6528 6627 7b50  to_datetime(f'{P
-00010cd0: 4b44 6174 6555 7469 6c69 7469 6573 2e74  KDateUtilities.t
-00010ce0: 7261 6469 6e67 4461 7465 2829 2e73 7472  radingDate().str
-00010cf0: 6674 696d 6528 6622 2559 2d25 6d2d 2564  ftime(f"%Y-%m-%d
-00010d00: 2229 7d20 3039 3a7b 3135 2b73 656c 662e  ")} 09:{15+self.
-00010d10: 636f 6e66 6967 4d61 6e61 6765 722e 6d6f  configManager.mo
-00010d20: 726e 696e 6761 6e61 6c79 7369 7363 616e  rninganalysiscan
-00010d30: 646c 656e 756d 6265 7220 2b20 327d 3a30  dlenumber + 2}:0
-00010d40: 302b 3035 3a33 3027 292e 746f 5f64 6174  0+05:30').to_dat
-00010d50: 6574 696d 6536 3428 295d 0a20 2020 2020  etime64()].     
-00010d60: 2020 2020 2020 2023 2062 726f 6b65 7253         # brokerS
-00010d70: 7172 4f66 6674 696d 6520 3d20 7064 2e74  qrOfftime = pd.t
-00010d80: 6f5f 6461 7465 7469 6d65 2866 277b 504b  o_datetime(f'{PK
-00010d90: 4461 7465 5574 696c 6974 6965 732e 7472  DateUtilities.tr
-00010da0: 6164 696e 6744 6174 6528 292e 7374 7266  adingDate().strf
-00010db0: 7469 6d65 2866 2225 592d 256d 2d25 6422  time(f"%Y-%m-%d"
-00010dc0: 297d 2031 353a 3134 3a30 302b 3035 3a33  )} 15:14:00+05:3
-00010dd0: 3027 292e 746f 5f64 6174 6574 696d 6536  0').to_datetime6
-00010de0: 3428 290a 2020 2020 2020 2020 6578 6365  4().        exce
-00010df0: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-00010e00: 6469 6666 5f64 6620 3d20 6461 7461 5b64  diff_df = data[d
-00010e10: 6174 612e 696e 6465 7820 3e3d 2020 7064  ata.index >=  pd
-00010e20: 2e74 6f5f 6461 7465 7469 6d65 2866 277b  .to_datetime(f'{
-00010e30: 504b 4461 7465 5574 696c 6974 6965 732e  PKDateUtilities.
-00010e40: 7472 6164 696e 6744 6174 6528 292e 7374  tradingDate().st
-00010e50: 7266 7469 6d65 2866 2225 592d 256d 2d25  rftime(f"%Y-%m-%
-00010e60: 6422 297d 2030 393a 7b31 352b 7365 6c66  d")} 09:{15+self
-00010e70: 2e63 6f6e 6669 674d 616e 6167 6572 2e6d  .configManager.m
-00010e80: 6f72 6e69 6e67 616e 616c 7973 6973 6361  orninganalysisca
-00010e90: 6e64 6c65 6e75 6d62 6572 202b 2032 7d3a  ndlenumber + 2}:
-00010ea0: 3030 2b30 353a 3330 272c 2075 7463 3d54  00+05:30', utc=T
-00010eb0: 7275 6529 5d0a 2020 2020 2020 2020 2020  rue)].          
-00010ec0: 2020 2320 6272 6f6b 6572 5371 724f 6666    # brokerSqrOff
-00010ed0: 7469 6d65 203d 2070 642e 746f 5f64 6174  time = pd.to_dat
-00010ee0: 6574 696d 6528 6627 7b50 4b44 6174 6555  etime(f'{PKDateU
-00010ef0: 7469 6c69 7469 6573 2e74 7261 6469 6e67  tilities.trading
-00010f00: 4461 7465 2829 2e73 7472 6674 696d 6528  Date().strftime(
-00010f10: 6622 2559 2d25 6d2d 2564 2229 7d20 3135  f"%Y-%m-%d")} 15
-00010f20: 3a31 343a 3030 2b30 353a 3330 272c 2075  :14:00+05:30', u
-00010f30: 7463 3d54 7275 6529 0a20 2020 2020 2020  tc=True).       
-00010f40: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-00010f50: 2020 6461 7948 6967 6841 6674 6572 416c    dayHighAfterAl
-00010f60: 6572 7420 3d20 6469 6666 5f64 665b 2248  ert = diff_df["H
-00010f70: 6967 6822 5d2e 6d61 7828 290a 2020 2020  igh"].max().    
-00010f80: 2020 2020 6869 6768 526f 7720 3d20 6469      highRow = di
-00010f90: 6666 5f64 665b 6469 6666 5f64 665b 2248  ff_df[diff_df["H
-00010fa0: 6967 6822 5d20 3e3d 2064 6179 4869 6768  igh"] >= dayHigh
-00010fb0: 4166 7465 7241 6c65 7274 5d0a 2020 2020  AfterAlert].    
-00010fc0: 2020 2020 6966 2068 6967 6852 6f77 2069      if highRow i
-00010fd0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206c  s not None and l
-00010fe0: 656e 2868 6967 6852 6f77 2920 3e20 303a  en(highRow) > 0:
-00010ff0: 0a20 2020 2020 2020 2020 2020 2068 6967  .            hig
-00011000: 6852 6f77 203d 2068 6967 6852 6f77 2e74  hRow = highRow.t
-00011010: 6169 6c28 3129 0a20 2020 2020 2020 2072  ail(1).        r
-00011020: 6574 7572 6e20 6869 6768 526f 772e 696e  eturn highRow.in
-00011030: 6465 785b 2d31 5d2c 2068 6967 6852 6f77  dex[-1], highRow
-00011040: 0a0a 0a20 2020 2064 6566 2066 696e 644d  ...    def findM
-00011050: 4143 4443 726f 7373 6f76 6572 2873 656c  ACDCrossover(sel
-00011060: 662c 2064 662c 2061 6674 6572 5469 6d65  f, df, afterTime
-00011070: 7374 616d 703d 4e6f 6e65 2c20 6e74 6843  stamp=None, nthC
-00011080: 726f 7373 6f76 6572 3d31 2c20 7570 4469  rossover=1, upDi
-00011090: 7265 6374 696f 6e3d 5472 7565 2c20 6d69  rection=True, mi
-000110a0: 6e52 5349 3d36 3029 3a0a 2020 2020 2020  nRSI=60):.      
-000110b0: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
-000110c0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
-000110d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000110e0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-000110f0: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
-00011100: 2829 0a20 2020 2020 2020 2064 6174 6120  ().        data 
-00011110: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
-00011120: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00011130: 6461 7461 2e72 6570 6c61 6365 285b 6e70  data.replace([np
-00011140: 2e69 6e66 2c20 2d6e 702e 696e 665d 2c20  .inf, -np.inf], 
-00011150: 3029 0a20 2020 2020 2020 2064 6174 612e  0).        data.
-00011160: 6472 6f70 6e61 2861 7869 733d 302c 2068  dropna(axis=0, h
-00011170: 6f77 3d22 616c 6c22 2c20 696e 706c 6163  ow="all", inplac
-00011180: 653d 5472 7565 2920 2320 4d61 7962 6520  e=True) # Maybe 
-00011190: 7468 6572 6520 7761 7320 6e6f 2074 7261  there was no tra
-000111a0: 6465 2064 6f6e 6520 6174 2074 6865 7365  de done at these
-000111b0: 2074 696d 6573 3f0a 2020 2020 2020 2020   times?.        
-000111c0: 6461 7461 203d 2064 6174 615b 3a3a 2d31  data = data[::-1
-000111d0: 5d20 2023 2052 6576 6572 7365 2074 6865  ]  # Reverse the
-000111e0: 2064 6174 6166 7261 6d65 2073 6f20 7468   dataframe so th
-000111f0: 6174 2069 7473 2074 6865 206f 6c64 6573  at its the oldes
-00011200: 7420 6461 7465 2066 6972 7374 0a20 2020  t date first.   
-00011210: 2020 2020 206d 6163 644c 696e 652c 206d       macdLine, m
-00011220: 6163 6453 6967 6e61 6c2c 206d 6163 6448  acdSignal, macdH
-00011230: 6973 7420 3d20 706b 7461 6c69 622e 4d41  ist = pktalib.MA
-00011240: 4344 2864 6174 615b 2243 6c6f 7365 225d  CD(data["Close"]
-00011250: 2c20 3132 2c20 3236 2c20 3929 0a20 2020  , 12, 26, 9).   
-00011260: 2020 2020 2023 2072 7369 5f64 6620 3d20       # rsi_df = 
-00011270: 706b 7461 6c69 622e 5253 4928 6461 7461  pktalib.RSI(data
-00011280: 5b22 436c 6f73 6522 5d2c 2031 3429 0a20  ["Close"], 14). 
-00011290: 2020 2020 2020 206c 696e 655f 6466 203d         line_df =
-000112a0: 2070 642e 4461 7461 4672 616d 6528 6d61   pd.DataFrame(ma
-000112b0: 6364 4c69 6e65 290a 2020 2020 2020 2020  cdLine).        
-000112c0: 7369 676e 616c 5f64 6620 3d20 7064 2e44  signal_df = pd.D
-000112d0: 6174 6146 7261 6d65 286d 6163 6453 6967  ataFrame(macdSig
-000112e0: 6e61 6c29 0a20 2020 2020 2020 2076 6f6c  nal).        vol
-000112f0: 5f64 6620 3d20 6461 7461 5b22 566f 6c75  _df = data["Volu
-00011300: 6d65 225d 0a20 2020 2020 2020 2064 6966  me"].        dif
-00011310: 665f 6466 203d 2070 642e 636f 6e63 6174  f_df = pd.concat
-00011320: 285b 6c69 6e65 5f64 662c 2073 6967 6e61  ([line_df, signa
-00011330: 6c5f 6466 2c20 7369 676e 616c 5f64 662d  l_df, signal_df-
-00011340: 6c69 6e65 5f64 662c 766f 6c5f 6466 5d2c  line_df,vol_df],
-00011350: 2061 7869 733d 3129 0a20 2020 2020 2020   axis=1).       
-00011360: 2064 6966 665f 6466 2e63 6f6c 756d 6e73   diff_df.columns
-00011370: 203d 205b 226c 696e 6522 2c22 7369 676e   = ["line","sign
-00011380: 616c 222c 2264 6966 6622 2c22 766f 6c22  al","diff","vol"
-00011390: 5d0a 2020 2020 2020 2020 6469 6666 5f64  ].        diff_d
-000113a0: 6620 3d20 6469 6666 5f64 665b 6469 6666  f = diff_df[diff
-000113b0: 5f64 665b 2276 6f6c 225d 203e 2030 5d20  _df["vol"] > 0] 
-000113c0: 2320 5765 2772 6520 6e6f 7420 676f 696e  # We're not goin
-000113d0: 6720 746f 2064 6f20 616e 7974 6869 6e67  g to do anything
-000113e0: 2077 6974 6820 6120 6361 6e64 6c65 2077   with a candle w
-000113f0: 6865 7265 2074 6865 7265 2077 6173 206e  here there was n
-00011400: 6f20 7472 6164 652e 0a20 2020 2020 2020  o trade..       
-00011410: 2023 2062 726f 6b65 7253 7172 4f66 6674   # brokerSqrOfft
-00011420: 696d 6520 3d20 4e6f 6e65 0a20 2020 2020  ime = None.     
-00011430: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00011440: 2020 2020 2320 4c65 7427 7320 6f6e 6c79      # Let's only
-00011450: 2063 6f6e 7369 6465 7220 7468 6f73 6520   consider those 
-00011460: 6361 6e64 6c65 7320 7468 6174 2061 7265  candles that are
-00011470: 2061 6674 6572 2074 6865 2061 6c65 7274   after the alert
-00011480: 2069 7373 7565 2d74 696d 6520 696e 2074   issue-time in t
-00011490: 6865 206d 6f72 6e69 6e67 7320 2b20 3220  he mornings + 2 
-000114a0: 6361 6e64 6c65 7320 2866 6f72 2062 7579  candles (for buy
-000114b0: 2f73 656c 6c29 0a20 2020 2020 2020 2020  /sell).         
-000114c0: 2020 2064 6966 665f 6466 203d 2064 6966     diff_df = dif
-000114d0: 665f 6466 5b64 6966 665f 6466 2e69 6e64  f_df[diff_df.ind
-000114e0: 6578 203e 3d20 2070 642e 746f 5f64 6174  ex >=  pd.to_dat
-000114f0: 6574 696d 6528 6627 7b50 4b44 6174 6555  etime(f'{PKDateU
-00011500: 7469 6c69 7469 6573 2e74 7261 6469 6e67  tilities.trading
-00011510: 4461 7465 2829 2e73 7472 6674 696d 6528  Date().strftime(
-00011520: 6622 2559 2d25 6d2d 2564 2229 7d20 3039  f"%Y-%m-%d")} 09
-00011530: 3a7b 3135 2b73 656c 662e 636f 6e66 6967  :{15+self.config
-00011540: 4d61 6e61 6765 722e 6d6f 726e 696e 6761  Manager.morninga
-00011550: 6e61 6c79 7369 7363 616e 646c 656e 756d  nalysiscandlenum
-00011560: 6265 7220 2b20 327d 3a30 302b 3035 3a33  ber + 2}:00+05:3
-00011570: 3027 292e 746f 5f64 6174 6574 696d 6536  0').to_datetime6
-00011580: 3428 295d 0a20 2020 2020 2020 2020 2020  4()].           
-00011590: 2023 2062 726f 6b65 7253 7172 4f66 6674   # brokerSqrOfft
-000115a0: 696d 6520 3d20 7064 2e74 6f5f 6461 7465  ime = pd.to_date
-000115b0: 7469 6d65 2866 277b 504b 4461 7465 5574  time(f'{PKDateUt
-000115c0: 696c 6974 6965 732e 7472 6164 696e 6744  ilities.tradingD
-000115d0: 6174 6528 292e 7374 7266 7469 6d65 2866  ate().strftime(f
-000115e0: 2225 592d 256d 2d25 6422 297d 2031 353a  "%Y-%m-%d")} 15:
-000115f0: 3134 3a30 302b 3035 3a33 3027 292e 746f  14:00+05:30').to
-00011600: 5f64 6174 6574 696d 6536 3428 290a 2020  _datetime64().  
-00011610: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-00011620: 2020 2020 2020 2020 2020 6469 6666 5f64            diff_d
-00011630: 6620 3d20 6469 6666 5f64 665b 6469 6666  f = diff_df[diff
-00011640: 5f64 662e 696e 6465 7820 3e3d 2020 7064  _df.index >=  pd
-00011650: 2e74 6f5f 6461 7465 7469 6d65 2866 277b  .to_datetime(f'{
-00011660: 504b 4461 7465 5574 696c 6974 6965 732e  PKDateUtilities.
-00011670: 7472 6164 696e 6744 6174 6528 292e 7374  tradingDate().st
-00011680: 7266 7469 6d65 2866 2225 592d 256d 2d25  rftime(f"%Y-%m-%
-00011690: 6422 297d 2030 393a 7b31 352b 7365 6c66  d")} 09:{15+self
-000116a0: 2e63 6f6e 6669 674d 616e 6167 6572 2e6d  .configManager.m
-000116b0: 6f72 6e69 6e67 616e 616c 7973 6973 6361  orninganalysisca
-000116c0: 6e64 6c65 6e75 6d62 6572 202b 2032 7d3a  ndlenumber + 2}:
-000116d0: 3030 2b30 353a 3330 272c 2075 7463 3d54  00+05:30', utc=T
-000116e0: 7275 6529 5d0a 2020 2020 2020 2020 2020  rue)].          
-000116f0: 2020 2320 6272 6f6b 6572 5371 724f 6666    # brokerSqrOff
-00011700: 7469 6d65 203d 2070 642e 746f 5f64 6174  time = pd.to_dat
-00011710: 6574 696d 6528 6627 7b50 4b44 6174 6555  etime(f'{PKDateU
-00011720: 7469 6c69 7469 6573 2e74 7261 6469 6e67  tilities.trading
-00011730: 4461 7465 2829 2e73 7472 6674 696d 6528  Date().strftime(
-00011740: 6622 2559 2d25 6d2d 2564 2229 7d20 3135  f"%Y-%m-%d")} 15
-00011750: 3a31 343a 3030 2b30 353a 3330 272c 2075  :14:00+05:30', u
-00011760: 7463 3d54 7275 6529 0a20 2020 2020 2020  tc=True).       
-00011770: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-00011780: 2020 696e 6465 7820 3d20 6c65 6e28 6469    index = len(di
-00011790: 6666 5f64 6629 0a20 2020 2020 2020 2063  ff_df).        c
-000117a0: 726f 7373 4f76 6572 203d 2030 0a20 2020  rossOver = 0.   
-000117b0: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-000117c0: 4c6f 6f70 2075 6e74 696c 2077 6527 7665  Loop until we've
-000117d0: 2066 6f75 6e64 2074 6865 206e 7468 2063   found the nth c
-000117e0: 726f 7373 6f76 6572 2066 6f72 204d 4143  rossover for MAC
-000117f0: 4420 6f72 2077 6527 7665 2072 6561 6368  D or we've reach
-00011800: 6564 2074 6865 206c 6173 7420 706f 696e  ed the last poin
-00011810: 7420 696e 2074 696d 650a 2020 2020 2020  t in time.      
-00011820: 2020 7768 696c 6520 2863 726f 7373 4f76    while (crossOv
-00011830: 6572 203c 206e 7468 4372 6f73 736f 7665  er < nthCrossove
-00011840: 7220 616e 6420 696e 6465 7820 3e3d 3029  r and index >=0)
-00011850: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00011860: 2064 6966 665f 6466 5b22 6469 6666 225d   diff_df["diff"]
-00011870: 5b69 6e64 6578 2d31 5d20 3c20 303a 2023  [index-1] < 0: #
-00011880: 2053 6967 6e61 6c20 6c69 6e65 2068 6173   Signal line has
-00011890: 206e 6f74 2063 726f 7373 6564 2079 6574   not crossed yet
-000118a0: 2061 6e64 2069 7320 6265 6c6f 7720 7468   and is below th
-000118b0: 6520 7a65 726f 206c 696e 650a 2020 2020  e zero line.    
-000118c0: 2020 2020 2020 2020 2020 2020 7768 696c              whil
-000118d0: 6528 2864 6966 665f 6466 5b22 6469 6666  e((diff_df["diff
-000118e0: 225d 5b69 6e64 6578 2d31 5d20 3c20 3020  "][index-1] < 0 
-000118f0: 616e 6420 696e 6465 7820 3e3d 3029 293a  and index >=0)):
-00011900: 2023 2061 6e64 2064 6966 665f 6466 2e69   # and diff_df.i
-00011910: 6e64 6578 203c 3d20 6272 6f6b 6572 5371  ndex <= brokerSq
-00011920: 724f 6666 7469 6d65 293a 2023 206f 7220  rOfftime): # or 
-00011930: 6469 6666 5f64 665b 2272 7369 225d 5b69  diff_df["rsi"][i
-00011940: 6e64 6578 2d31 5d20 3c3d 206d 696e 5253  ndex-1] <= minRS
-00011950: 4929 3a0a 2020 2020 2020 2020 2020 2020  I):.            
-00011960: 2020 2020 2020 2020 2320 4c6f 6f70 2077          # Loop w
-00011970: 6869 6c65 2053 6967 6e61 6c20 6c69 6e65  hile Signal line
-00011980: 2068 6173 206e 6f74 2063 726f 7373 6564   has not crossed
-00011990: 2079 6574 2061 6e64 2069 7320 6265 6c6f   yet and is belo
-000119a0: 7720 7468 6520 7a65 726f 206c 696e 6520  w the zero line 
-000119b0: 616e 6420 7765 2776 6520 6e6f 7420 7265  and we've not re
-000119c0: 6163 6865 6420 7468 6520 6c61 7374 2070  ached the last p
-000119d0: 6f69 6e74 0a20 2020 2020 2020 2020 2020  oint.           
-000119e0: 2020 2020 2020 2020 2069 6e64 6578 202d           index -
-000119f0: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00011a00: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00011a10: 2020 2020 2020 7768 696c 6528 2864 6966        while((dif
-00011a20: 665f 6466 5b22 6469 6666 225d 5b69 6e64  f_df["diff"][ind
-00011a30: 6578 2d31 5d20 3e3d 2030 2061 6e64 2069  ex-1] >= 0 and i
-00011a40: 6e64 6578 203e 3d30 2929 3a20 2320 616e  ndex >=0)): # an
-00011a50: 6420 6469 6666 5f64 662e 696e 6465 7820  d diff_df.index 
-00011a60: 3c3d 2062 726f 6b65 7253 7172 4f66 6674  <= brokerSqrOfft
-00011a70: 696d 6529 3a20 2320 6f72 2064 6966 665f  ime): # or diff_
-00011a80: 6466 5b22 7273 6922 5d5b 696e 6465 782d  df["rsi"][index-
-00011a90: 315d 203c 3d20 6d69 6e52 5349 293a 0a20  1] <= minRSI):. 
-00011aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ab0: 2020 2023 204c 6f6f 7020 756e 7469 6c20     # Loop until 
-00011ac0: 7369 676e 616c 206c 696e 6520 6861 7320  signal line has 
-00011ad0: 6e6f 7420 6372 6f73 7365 6420 7965 7420  not crossed yet 
-00011ae0: 616e 6420 6973 2061 626f 7665 2074 6865  and is above the
-00011af0: 207a 6572 6f20 6c69 6e65 0a20 2020 2020   zero line.     
-00011b00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00011b10: 6e64 6578 202d 3d20 310a 2020 2020 2020  ndex -= 1.      
-00011b20: 2020 2020 2020 6372 6f73 734f 7665 7220        crossOver 
-00011b30: 2b3d 2031 0a20 2020 2020 2020 2074 7320  += 1.        ts 
-00011b40: 3d20 6469 6666 5f64 662e 7461 696c 286c  = diff_df.tail(l
-00011b50: 656e 2864 6966 665f 6466 292d 696e 6465  en(diff_df)-inde
-00011b60: 7820 2b31 292e 6865 6164 2831 292e 696e  x +1).head(1).in
-00011b70: 6465 785b 2d31 5d0a 2020 2020 2020 2020  dex[-1].        
-00011b80: 7265 7475 726e 2074 732c 2064 6174 615b  return ts, data[
-00011b90: 6461 7461 2e69 6e64 6578 203d 3d20 7473  data.index == ts
-00011ba0: 5d20 2364 662e 6865 6164 286c 656e 2864  ] #df.head(len(d
-00011bb0: 6629 202d 696e 6465 7820 2b31 292e 7461  f) -index +1).ta
-00011bc0: 696c 2831 290a 2020 2020 0a20 2020 2023  il(1).    .    #
-00011bd0: 2046 696e 6420 7374 6f63 6b20 7368 6f77   Find stock show
-00011be0: 696e 6720 5253 4920 6372 6f73 7369 6e67  ing RSI crossing
-00011bf0: 2077 6974 6820 5253 4920 3920 534d 410a   with RSI 9 SMA.
-00011c00: 2020 2020 6465 6620 6669 6e64 5253 4943      def findRSIC
-00011c10: 726f 7373 696e 674d 4128 7365 6c66 2c20  rossingMA(self, 
-00011c20: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
-00011c30: 7361 7665 4469 6374 2c6c 6f6f 6b46 6f72  saveDict,lookFor
-00011c40: 3d31 2c20 6d61 4c65 6e67 7468 3d39 2c20  =1, maLength=9, 
-00011c50: 7273 694b 6579 3d22 5253 4922 293a 0a20  rsiKey="RSI"):. 
-00011c60: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
-00011c70: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
-00011c80: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-00011c90: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-00011ca0: 2020 2020 2020 2069 6620 7273 694b 6579         if rsiKey
-00011cb0: 206e 6f74 2069 6e20 6466 2e63 6f6c 756d   not in df.colum
-00011cc0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00011cd0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-00011ce0: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
-00011cf0: 6f70 7928 290a 2020 2020 2020 2020 6461  opy().        da
-00011d00: 7461 203d 2064 6174 615b 3a3a 2d31 5d0a  ta = data[::-1].
-00011d10: 2020 2020 2020 2020 6d61 5273 6920 3d20          maRsi = 
-00011d20: 706b 7461 6c69 622e 4d41 2864 6174 615b  pktalib.MA(data[
-00011d30: 7273 694b 6579 5d2c 2074 696d 6570 6572  rsiKey], timeper
-00011d40: 696f 643d 6d61 4c65 6e67 7468 290a 2020  iod=maLength).  
-00011d50: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00011d60: 615b 3a3a 2d31 5d2e 6865 6164 2833 290a  a[::-1].head(3).
-00011d70: 2020 2020 2020 2020 6d61 5273 6920 3d20          maRsi = 
-00011d80: 6d61 5273 695b 3a3a 2d31 5d2e 6865 6164  maRsi[::-1].head
-00011d90: 2833 290a 2020 2020 2020 2020 7361 7665  (3).        save
-00011da0: 6420 3d20 7365 6c66 2e66 696e 6443 7572  d = self.findCur
-00011db0: 7265 6e74 5361 7665 6456 616c 7565 2873  rentSavedValue(s
-00011dc0: 6372 6565 6e44 6963 742c 7361 7665 4469  creenDict,saveDi
-00011dd0: 6374 2c22 5472 656e 6422 290a 2020 2020  ct,"Trend").    
-00011de0: 2020 2020 6966 206c 6f6f 6b46 6f72 2069      if lookFor i
-00011df0: 6e20 5b31 2c33 5d20 616e 6420 6d61 5273  n [1,3] and maRs
-00011e00: 692e 696c 6f63 5b30 5d20 3c3d 2064 6174  i.iloc[0] <= dat
-00011e10: 615b 7273 694b 6579 5d2e 696c 6f63 5b30  a[rsiKey].iloc[0
-00011e20: 5d20 616e 6420 6d61 5273 692e 696c 6f63  ] and maRsi.iloc
-00011e30: 5b31 5d20 3e20 6461 7461 5b72 7369 4b65  [1] > data[rsiKe
-00011e40: 795d 2e69 6c6f 635b 315d 3a0a 2020 2020  y].iloc[1]:.    
-00011e50: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-00011e60: 6374 5b27 4d41 2d53 6967 6e61 6c27 5d20  ct['MA-Signal'] 
-00011e70: 3d20 7361 7665 645b 305d 202b 2063 6f6c  = saved[0] + col
-00011e80: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-00011e90: 6c6f 7254 6578 742e 4752 4545 4e20 2b20  lorText.GREEN + 
-00011ea0: 6627 5253 492d 4d41 2d42 7579 2720 2b20  f'RSI-MA-Buy' + 
-00011eb0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-00011ec0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00011ed0: 6374 5b27 4d41 2d53 6967 6e61 6c27 5d20  ct['MA-Signal'] 
-00011ee0: 3d20 7361 7665 645b 315d 202b 2066 2752  = saved[1] + f'R
-00011ef0: 5349 2d4d 412d 4275 7927 0a20 2020 2020  SI-MA-Buy'.     
-00011f00: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00011f10: 7565 2069 6620 2872 7369 4b65 7920 3d3d  ue if (rsiKey ==
-00011f20: 2022 5253 4969 2229 2065 6c73 6520 2873   "RSIi") else (s
-00011f30: 656c 662e 6669 6e64 5253 4943 726f 7373  elf.findRSICross
-00011f40: 696e 674d 4128 6466 2c20 7363 7265 656e  ingMA(df, screen
-00011f50: 4469 6374 2c20 7361 7665 4469 6374 2c6c  Dict, saveDict,l
-00011f60: 6f6f 6b46 6f72 3d6c 6f6f 6b46 6f72 2c20  ookFor=lookFor, 
-00011f70: 6d61 4c65 6e67 7468 3d6d 614c 656e 6774  maLength=maLengt
-00011f80: 682c 2072 7369 4b65 793d 2252 5349 6922  h, rsiKey="RSIi"
-00011f90: 2920 6f72 2054 7275 6529 0a20 2020 2020  ) or True).     
-00011fa0: 2020 2065 6c69 6620 6c6f 6f6b 466f 7220     elif lookFor 
-00011fb0: 696e 205b 322c 335d 2061 6e64 206d 6152  in [2,3] and maR
-00011fc0: 7369 2e69 6c6f 635b 305d 203e 3d20 6461  si.iloc[0] >= da
-00011fd0: 7461 5b72 7369 4b65 795d 2e69 6c6f 635b  ta[rsiKey].iloc[
-00011fe0: 305d 2061 6e64 206d 6152 7369 2e69 6c6f  0] and maRsi.ilo
-00011ff0: 635b 315d 203c 2064 6174 615b 7273 694b  c[1] < data[rsiK
-00012000: 6579 5d2e 696c 6f63 5b31 5d3a 0a20 2020  ey].iloc[1]:.   
-00012010: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00012020: 6963 745b 274d 412d 5369 676e 616c 275d  ict['MA-Signal']
-00012030: 203d 2073 6176 6564 5b30 5d20 2b20 636f   = saved[0] + co
-00012040: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
-00012050: 6f6c 6f72 5465 7874 2e46 4149 4c20 2b20  olorText.FAIL + 
-00012060: 6627 5253 492d 4d41 2d53 656c 6c27 202b  f'RSI-MA-Sell' +
-00012070: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
-00012080: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-00012090: 6963 745b 274d 412d 5369 676e 616c 275d  ict['MA-Signal']
-000120a0: 203d 2073 6176 6564 5b31 5d20 2b20 6627   = saved[1] + f'
-000120b0: 5253 492d 4d41 2d53 656c 6c27 0a20 2020  RSI-MA-Sell'.   
-000120c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000120d0: 5472 7565 2069 6620 2872 7369 4b65 7920  True if (rsiKey 
-000120e0: 3d3d 2022 5253 4969 2229 2065 6c73 6520  == "RSIi") else 
-000120f0: 2873 656c 662e 6669 6e64 5253 4943 726f  (self.findRSICro
-00012100: 7373 696e 674d 4128 6466 2c20 7363 7265  ssingMA(df, scre
-00012110: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-00012120: 2c6c 6f6f 6b46 6f72 3d6c 6f6f 6b46 6f72  ,lookFor=lookFor
-00012130: 2c20 6d61 4c65 6e67 7468 3d6d 614c 656e  , maLength=maLen
-00012140: 6774 682c 2072 7369 4b65 793d 2252 5349  gth, rsiKey="RSI
-00012150: 6922 2920 6f72 2054 7275 6529 0a20 2020  i") or True).   
-00012160: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00012170: 6520 6966 2028 7273 694b 6579 203d 3d20  e if (rsiKey == 
-00012180: 2252 5349 6922 2920 656c 7365 2028 7365  "RSIi") else (se
-00012190: 6c66 2e66 696e 6452 5349 4372 6f73 7369  lf.findRSICrossi
-000121a0: 6e67 4d41 2864 662c 2073 6372 6565 6e44  ngMA(df, screenD
-000121b0: 6963 742c 2073 6176 6544 6963 742c 6c6f  ict, saveDict,lo
-000121c0: 6f6b 466f 723d 6c6f 6f6b 466f 722c 206d  okFor=lookFor, m
-000121d0: 614c 656e 6774 683d 6d61 4c65 6e67 7468  aLength=maLength
-000121e0: 2c20 7273 694b 6579 3d22 5253 4969 2229  , rsiKey="RSIi")
-000121f0: 290a 2020 2020 0a20 2020 2023 2046 696e  ).    .    # Fin
-00012200: 6420 7374 6f63 6b73 2077 6974 6820 7269  d stocks with ri
-00012210: 7369 6e67 2052 5349 2066 726f 6d20 6c6f  sing RSI from lo
-00012220: 7765 7220 6c65 7665 6c73 0a20 2020 2064  wer levels.    d
-00012230: 6566 2066 696e 6452 6973 696e 6752 5349  ef findRisingRSI
-00012240: 2873 656c 662c 2064 662c 2072 7369 4b65  (self, df, rsiKe
-00012250: 793d 2252 5349 2229 3a0a 2020 2020 2020  y="RSI"):.      
-00012260: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
-00012270: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
-00012280: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00012290: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-000122a0: 2020 6966 2072 7369 4b65 7920 6e6f 7420    if rsiKey not 
-000122b0: 696e 2064 662e 636f 6c75 6d6e 733a 0a20  in df.columns:. 
-000122c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000122d0: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-000122e0: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
-000122f0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00012300: 6461 7461 5b3a 3a2d 315d 0a20 2020 2020  data[::-1].     
-00012310: 2020 2064 6174 6120 3d20 6461 7461 2e74     data = data.t
-00012320: 6169 6c28 3329 0a20 2020 2020 2020 2069  ail(3).        i
-00012330: 6620 6c65 6e28 6461 7461 2920 3c20 333a  f len(data) < 3:
-00012340: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00012350: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-00012360: 2020 6461 794d 696e 7573 3252 5349 203d    dayMinus2RSI =
-00012370: 2064 6174 615b 2252 5349 225d 2e69 6c6f   data["RSI"].ilo
-00012380: 635b 305d 0a20 2020 2020 2020 2064 6179  c[0].        day
-00012390: 4d69 6e75 7331 5253 4920 3d20 6461 7461  Minus1RSI = data
-000123a0: 5b22 5253 4922 5d2e 696c 6f63 5b31 5d0a  ["RSI"].iloc[1].
-000123b0: 2020 2020 2020 2020 6461 7952 5349 203d          dayRSI =
-000123c0: 2064 6174 615b 2252 5349 225d 2e69 6c6f   data["RSI"].ilo
-000123d0: 635b 325d 0a20 2020 2020 2020 2072 6574  c[2].        ret
-000123e0: 7572 6e56 616c 7565 203d 2028 6461 794d  urnValue = (dayM
-000123f0: 696e 7573 3252 5349 203c 3d20 3335 2061  inus2RSI <= 35 a
-00012400: 6e64 2064 6179 4d69 6e75 7331 5253 4920  nd dayMinus1RSI 
-00012410: 3e20 6461 794d 696e 7573 3252 5349 2061  > dayMinus2RSI a
-00012420: 6e64 2064 6179 5253 4920 3e20 6461 794d  nd dayRSI > dayM
-00012430: 696e 7573 3152 5349 2920 6f72 205c 0a20  inus1RSI) or \. 
-00012440: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00012450: 6461 794d 696e 7573 3152 5349 203c 3d20  dayMinus1RSI <= 
-00012460: 3335 2061 6e64 2064 6179 5253 4920 3e20  35 and dayRSI > 
-00012470: 6461 794d 696e 7573 3152 5349 290a 2020  dayMinus1RSI).  
-00012480: 2020 2020 2020 6966 2072 7369 4b65 7920        if rsiKey 
-00012490: 3d3d 2022 5253 4922 3a0a 2020 2020 2020  == "RSI":.      
-000124a0: 2020 2020 2020 7265 7475 726e 5661 6c75        returnValu
-000124b0: 6520 3d20 7365 6c66 2e66 696e 6452 6973  e = self.findRis
-000124c0: 696e 6752 5349 2864 662c 2072 7369 4b65  ingRSI(df, rsiKe
-000124d0: 793d 2252 5349 6922 2920 6f72 2072 6574  y="RSIi") or ret
-000124e0: 7572 6e56 616c 7565 0a20 2020 2020 2020  urnValue.       
-000124f0: 2072 6574 7572 6e20 7265 7475 726e 5661   return returnVa
-00012500: 6c75 650a 0a20 2020 2023 406d 6561 7375  lue..    #@measu
-00012510: 7265 5f74 696d 650a 2020 2020 2320 4669  re_time.    # Fi
-00012520: 6e64 206f 7574 2074 7265 6e64 2066 6f72  nd out trend for
-00012530: 2064 6179 7320 746f 206c 6f6f 6b62 6163   days to lookbac
-00012540: 6b0a 2020 2020 6465 6620 6669 6e64 5472  k.    def findTr
-00012550: 656e 6428 7365 6c66 2c20 6466 2c20 7363  end(self, df, sc
-00012560: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
-00012570: 6374 2c20 6461 7973 546f 4c6f 6f6b 6261  ct, daysToLookba
-00012580: 636b 3d4e 6f6e 652c 2073 746f 636b 4e61  ck=None, stockNa
-00012590: 6d65 3d22 2229 3a0a 2020 2020 2020 2020  me=""):.        
-000125a0: 6966 2064 6620 6973 204e 6f6e 6520 6f72  if df is None or
-000125b0: 206c 656e 2864 6629 203d 3d20 303a 0a20   len(df) == 0:. 
-000125c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000125d0: 6e20 2255 6e6b 6e6f 776e 220a 2020 2020  n "Unknown".    
-000125e0: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
-000125f0: 7079 2829 0a20 2020 2020 2020 2069 6620  py().        if 
-00012600: 6461 7973 546f 4c6f 6f6b 6261 636b 2069  daysToLookback i
-00012610: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00012620: 2020 2020 6461 7973 546f 4c6f 6f6b 6261      daysToLookba
-00012630: 636b 203d 2073 656c 662e 636f 6e66 6967  ck = self.config
-00012640: 4d61 6e61 6765 722e 6461 7973 546f 4c6f  Manager.daysToLo
-00012650: 6f6b 6261 636b 0a20 2020 2020 2020 2064  okback.        d
-00012660: 6174 6120 3d20 6461 7461 2e68 6561 6428  ata = data.head(
-00012670: 6461 7973 546f 4c6f 6f6b 6261 636b 290a  daysToLookback).
-00012680: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00012690: 6174 615b 3a3a 2d31 5d0a 2020 2020 2020  ata[::-1].      
-000126a0: 2020 6461 7461 203d 2064 6174 612e 7365    data = data.se
-000126b0: 745f 696e 6465 7828 6e70 2e61 7261 6e67  t_index(np.arang
-000126c0: 6528 6c65 6e28 6461 7461 2929 290a 2020  e(len(data))).  
-000126d0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-000126e0: 612e 6669 6c6c 6e61 2830 290a 2020 2020  a.fillna(0).    
-000126f0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
-00012700: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
-00012710: 202d 6e70 2e69 6e66 5d2c 2030 290a 2020   -np.inf], 0).  
-00012720: 2020 2020 2020 7361 7665 6420 3d20 7365        saved = se
-00012730: 6c66 2e66 696e 6443 7572 7265 6e74 5361  lf.findCurrentSa
-00012740: 7665 6456 616c 7565 2873 6372 6565 6e44  vedValue(screenD
-00012750: 6963 742c 7361 7665 4469 6374 2c22 5472  ict,saveDict,"Tr
-00012760: 656e 6422 290a 2020 2020 2020 2020 7472  end").        tr
-00012770: 793a 0a20 2020 2020 2020 2020 2020 2077  y:.            w
-00012780: 6974 6820 5375 7070 7265 7373 4f75 7470  ith SuppressOutp
-00012790: 7574 2873 7570 7072 6573 735f 7374 646f  ut(suppress_stdo
-000127a0: 7574 3d54 7275 652c 2073 7570 7072 6573  ut=True, suppres
-000127b0: 735f 7374 6465 7272 3d54 7275 6529 3a0a  s_stderr=True):.
-000127c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127d0: 6461 7461 5b22 746f 7073 225d 203d 2064  data["tops"] = d
-000127e0: 6174 615b 2243 6c6f 7365 225d 2e69 6c6f  ata["Close"].ilo
-000127f0: 635b 0a20 2020 2020 2020 2020 2020 2020  c[.             
-00012800: 2020 2020 2020 206c 6973 7428 0a20 2020         list(.   
+0000eef0: 6966 206d 614c 656e 6774 6820 696e 205b  if maLength in [
+0000ef00: 392c 3130 2c32 302c 3530 2c31 3030 5d20  9,10,20,50,100] 
+0000ef10: 656c 7365 205b 392c 3130 2c32 302c 3530  else [9,10,20,50
+0000ef20: 2c31 3030 2c6d 6152 616e 6765 5d0a 2020  ,100,maRange].  
+0000ef30: 2020 2020 2020 7265 7375 6c74 7320 3d20        results = 
+0000ef40: 5b5d 0a20 2020 2020 2020 2068 6173 5265  [].        hasRe
+0000ef50: 7665 7273 616c 7320 3d20 4661 6c73 650a  versals = False.
+0000ef60: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0000ef70: 6174 615b 3a3a 2d31 5d0a 2020 2020 2020  ata[::-1].      
+0000ef80: 2020 7361 7665 6420 3d20 7365 6c66 2e66    saved = self.f
+0000ef90: 696e 6443 7572 7265 6e74 5361 7665 6456  indCurrentSavedV
+0000efa0: 616c 7565 2873 6372 6565 6e44 6963 742c  alue(screenDict,
+0000efb0: 7361 7665 4469 6374 2c20 224d 412d 5369  saveDict, "MA-Si
+0000efc0: 676e 616c 2229 0a20 2020 2020 2020 2066  gnal").        f
+0000efd0: 6f72 206d 614c 656e 6774 6820 696e 206d  or maLength in m
+0000efe0: 6152 616e 6765 3a0a 2020 2020 2020 2020  aRange:.        
+0000eff0: 2020 2020 6461 7461 436f 7079 203d 2064      dataCopy = d
+0000f000: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
+0000f010: 6966 2073 656c 662e 636f 6e66 6967 4d61  if self.configMa
+0000f020: 6e61 6765 722e 7573 6545 4d41 206f 7220  nager.useEMA or 
+0000f030: 6d61 4c65 6e67 7468 203d 3d20 393a 0a20  maLength == 9:. 
+0000f040: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000f050: 6152 6576 203d 2070 6b74 616c 6962 2e45  aRev = pktalib.E
+0000f060: 4d41 2864 6174 6143 6f70 795b 2243 6c6f  MA(dataCopy["Clo
+0000f070: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
+0000f080: 3d6d 614c 656e 6774 6829 0a20 2020 2020  =maLength).     
+0000f090: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000f0a0: 2020 2020 2020 2020 2020 2020 206d 6152               maR
+0000f0b0: 6576 203d 2070 6b74 616c 6962 2e4d 4128  ev = pktalib.MA(
+0000f0c0: 6461 7461 436f 7079 5b22 436c 6f73 6522  dataCopy["Close"
+0000f0d0: 5d2c 2074 696d 6570 6572 696f 643d 6d61  ], timeperiod=ma
+0000f0e0: 4c65 6e67 7468 290a 2020 2020 2020 2020  Length).        
+0000f0f0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000f100: 2020 2020 2020 2020 2064 6174 6143 6f70           dataCop
+0000f110: 792e 6472 6f70 2822 6d61 5265 7622 2c20  y.drop("maRev", 
+0000f120: 6178 6973 3d31 2c20 696e 706c 6163 653d  axis=1, inplace=
+0000f130: 5472 7565 2c20 6572 726f 7273 3d22 6967  True, errors="ig
+0000f140: 6e6f 7265 2229 0a20 2020 2020 2020 2020  nore").         
+0000f150: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+0000f160: 696f 6e3a 2320 7072 6167 6d61 3a20 6e6f  ion:# pragma: no
+0000f170: 2063 6f76 6572 0a20 2020 2020 2020 2020   cover.         
+0000f180: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+0000f190: 2020 2020 2020 2020 6461 7461 436f 7079          dataCopy
+0000f1a0: 2e69 6e73 6572 7428 6c65 6e28 6461 7461  .insert(len(data
+0000f1b0: 436f 7079 2e63 6f6c 756d 6e73 292c 2022  Copy.columns), "
+0000f1c0: 6d61 5265 7622 2c20 6d61 5265 7629 0a20  maRev", maRev). 
+0000f1d0: 2020 2020 2020 2020 2020 2064 6174 6143             dataC
+0000f1e0: 6f70 7920 3d20 6461 7461 436f 7079 5b3a  opy = dataCopy[:
+0000f1f0: 3a2d 315d 2e68 6561 6428 3429 0a20 2020  :-1].head(4).   
+0000f200: 2020 2020 2020 2020 2062 756c 6c69 7368           bullish
+0000f210: 4d41 5265 7665 7273 616c 203d 2064 6174  MAReversal = dat
+0000f220: 6143 6f70 795b 226d 6152 6576 225d 2e69  aCopy["maRev"].i
+0000f230: 6c6f 635b 305d 203e 3d20 6461 7461 436f  loc[0] >= dataCo
+0000f240: 7079 5b22 6d61 5265 7622 5d2e 696c 6f63  py["maRev"].iloc
+0000f250: 5b31 5d20 616e 6420 5c0a 2020 2020 2020  [1] and \.      
+0000f260: 2020 2020 2020 2020 2020 6461 7461 436f            dataCo
+0000f270: 7079 5b22 6d61 5265 7622 5d2e 696c 6f63  py["maRev"].iloc
+0000f280: 5b31 5d20 3e3d 2064 6174 6143 6f70 795b  [1] >= dataCopy[
+0000f290: 226d 6152 6576 225d 2e69 6c6f 635b 325d  "maRev"].iloc[2]
+0000f2a0: 2061 6e64 205c 0a20 2020 2020 2020 2020   and \.         
+0000f2b0: 2020 2020 2020 2020 2020 2064 6174 6143             dataC
+0000f2c0: 6f70 795b 226d 6152 6576 225d 2e69 6c6f  opy["maRev"].ilo
+0000f2d0: 635b 325d 203c 2064 6174 6143 6f70 795b  c[2] < dataCopy[
+0000f2e0: 226d 6152 6576 225d 2e69 6c6f 635b 335d  "maRev"].iloc[3]
+0000f2f0: 0a20 2020 2020 2020 2020 2020 2062 756c  .            bul
+0000f300: 6c69 7368 436c 6f73 6520 3d20 6461 7461  lishClose = data
+0000f310: 436f 7079 2e68 6561 6428 3129 5b22 436c  Copy.head(1)["Cl
+0000f320: 6f73 6522 5d2e 696c 6f63 5b30 5d20 3e3d  ose"].iloc[0] >=
+0000f330: 2064 6174 6143 6f70 792e 6865 6164 2831   dataCopy.head(1
+0000f340: 295b 226d 6152 6576 225d 2e69 6c6f 635b  )["maRev"].iloc[
+0000f350: 305d 0a20 2020 2020 2020 2020 2020 2062  0].            b
+0000f360: 6561 7269 7368 4d41 5265 7665 7273 616c  earishMAReversal
+0000f370: 203d 2064 6174 6143 6f70 795b 226d 6152   = dataCopy["maR
+0000f380: 6576 225d 2e69 6c6f 635b 305d 203c 3d20  ev"].iloc[0] <= 
+0000f390: 6461 7461 436f 7079 5b22 6d61 5265 7622  dataCopy["maRev"
+0000f3a0: 5d2e 696c 6f63 5b31 5d20 616e 6420 5c0a  ].iloc[1] and \.
+0000f3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3c0: 6461 7461 436f 7079 5b22 6d61 5265 7622  dataCopy["maRev"
+0000f3d0: 5d2e 696c 6f63 5b31 5d20 3c3d 2064 6174  ].iloc[1] <= dat
+0000f3e0: 6143 6f70 795b 226d 6152 6576 225d 2e69  aCopy["maRev"].i
+0000f3f0: 6c6f 635b 325d 2061 6e64 205c 0a20 2020  loc[2] and \.   
+0000f400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f410: 2064 6174 6143 6f70 795b 226d 6152 6576   dataCopy["maRev
+0000f420: 225d 2e69 6c6f 635b 325d 203e 2064 6174  "].iloc[2] > dat
+0000f430: 6143 6f70 795b 226d 6152 6576 225d 2e69  aCopy["maRev"].i
+0000f440: 6c6f 635b 335d 0a20 2020 2020 2020 2020  loc[3].         
+0000f450: 2020 2069 7352 6563 656e 7443 6c6f 7365     isRecentClose
+0000f460: 5769 7468 696e 5065 7263 656e 7452 616e  WithinPercentRan
+0000f470: 6765 203d 2064 6174 6143 6f70 792e 6571  ge = dataCopy.eq
+0000f480: 7561 6c73 2864 6174 6143 6f70 795b 2864  uals(dataCopy[(d
+0000f490: 6174 6143 6f70 792e 436c 6f73 6520 3e3d  ataCopy.Close >=
+0000f4a0: 2028 6461 7461 436f 7079 2e6d 6152 6576   (dataCopy.maRev
+0000f4b0: 202d 2028 6461 7461 436f 7079 2e6d 6152   - (dataCopy.maR
+0000f4c0: 6576 202a 2070 6572 6365 6e74 6167 6529  ev * percentage)
+0000f4d0: 2929 2026 2028 6461 7461 436f 7079 2e43  )) & (dataCopy.C
+0000f4e0: 6c6f 7365 203c 3d20 2864 6174 6143 6f70  lose <= (dataCop
+0000f4f0: 792e 6d61 5265 7620 2b20 2864 6174 6143  y.maRev + (dataC
+0000f500: 6f70 792e 6d61 5265 7620 2a20 7065 7263  opy.maRev * perc
+0000f510: 656e 7461 6765 2929 295d 290a 2020 2020  entage)))]).    
+0000f520: 2020 2020 2020 2020 6966 2028 6973 5265          if (isRe
+0000f530: 6365 6e74 436c 6f73 6557 6974 6869 6e50  centCloseWithinP
+0000f540: 6572 6365 6e74 5261 6e67 6520 616e 6420  ercentRange and 
+0000f550: 6275 6c6c 6973 6843 6c6f 7365 2061 6e64  bullishClose and
+0000f560: 2062 756c 6c69 7368 4d41 5265 7665 7273   bullishMARevers
+0000f570: 616c 2920 6f72 205c 0a20 2020 2020 2020  al) or \.       
+0000f580: 2020 2020 2020 2020 2028 6973 5265 6365           (isRece
+0000f590: 6e74 436c 6f73 6557 6974 6869 6e50 6572  ntCloseWithinPer
+0000f5a0: 6365 6e74 5261 6e67 6520 616e 6420 6e6f  centRange and no
+0000f5b0: 7420 6275 6c6c 6973 6843 6c6f 7365 2061  t bullishClose a
+0000f5c0: 6e64 2062 6561 7269 7368 4d41 5265 7665  nd bearishMAReve
+0000f5d0: 7273 616c 293a 0a20 2020 2020 2020 2020  rsal):.         
+0000f5e0: 2020 2020 2020 2068 6173 5265 7665 7273         hasRevers
+0000f5f0: 616c 7320 3d20 5472 7565 0a20 2020 2020  als = True.     
+0000f600: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0000f610: 7473 2e61 7070 656e 6428 7374 7228 6d61  ts.append(str(ma
+0000f620: 4c65 6e67 7468 2929 0a20 2020 2020 2020  Length)).       
+0000f630: 2069 6620 6861 7352 6576 6572 7361 6c73   if hasReversals
+0000f640: 3a0a 2020 2020 2020 2020 2020 2020 7363  :.            sc
+0000f650: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
+0000f660: 6e61 6c22 5d20 3d20 280a 2020 2020 2020  nal"] = (.      
+0000f670: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+0000f680: 305d 200a 2020 2020 2020 2020 2020 2020  0] .            
+0000f690: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+0000f6a0: 424f 4c44 0a20 2020 2020 2020 2020 2020  BOLD.           
+0000f6b0: 2020 2020 202b 2028 636f 6c6f 7254 6578       + (colorTex
+0000f6c0: 742e 4752 4545 4e20 6966 2062 756c 6c69  t.GREEN if bulli
+0000f6d0: 7368 4d41 5265 7665 7273 616c 2065 6c73  shMAReversal els
+0000f6e0: 6520 2863 6f6c 6f72 5465 7874 2e46 4149  e (colorText.FAI
+0000f6f0: 4c20 6966 2062 6561 7269 7368 4d41 5265  L if bearishMARe
+0000f700: 7665 7273 616c 2065 6c73 6520 636f 6c6f  versal else colo
+0000f710: 7254 6578 742e 5741 524e 2929 0a20 2020  rText.WARN)).   
+0000f720: 2020 2020 2020 2020 2020 2020 202b 2066               + f
+0000f730: 2252 6576 6572 7361 6c2d 5b7b 272c 272e  "Reversal-[{','.
+0000f740: 6a6f 696e 2872 6573 756c 7473 297d 5d7b  join(results)}]{
+0000f750: 2745 4d41 2720 6966 2028 6d61 4c65 6e67  'EMA' if (maLeng
+0000f760: 7468 203d 3d20 3920 6f72 2073 656c 662e  th == 9 or self.
+0000f770: 636f 6e66 6967 4d61 6e61 6765 722e 7573  configManager.us
+0000f780: 6545 4d41 2920 656c 7365 2027 4d41 277d  eEMA) else 'MA'}
+0000f790: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000f7a0: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+0000f7b0: 440a 2020 2020 2020 2020 2020 2020 290a  D.            ).
+0000f7c0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+0000f7d0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+0000f7e0: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
+0000f7f0: 2252 6576 6572 7361 6c2d 5b7b 272c 272e  "Reversal-[{','.
+0000f800: 6a6f 696e 2872 6573 756c 7473 297d 5d7b  join(results)}]{
+0000f810: 2745 4d41 2720 6966 2028 6d61 4c65 6e67  'EMA' if (maLeng
+0000f820: 7468 203d 3d20 3920 6f72 2073 656c 662e  th == 9 or self.
+0000f830: 636f 6e66 6967 4d61 6e61 6765 722e 7573  configManager.us
+0000f840: 6545 4d41 2920 656c 7365 2027 4d41 277d  eEMA) else 'MA'}
+0000f850: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+0000f860: 2068 6173 5265 7665 7273 616c 730a 0a20   hasReversals.. 
+0000f870: 2020 2064 6566 2066 696e 6443 7572 7265     def findCurre
+0000f880: 6e74 5361 7665 6456 616c 7565 2873 656c  ntSavedValue(sel
+0000f890: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
+0000f8a0: 6176 6544 6963 742c 206b 6579 293a 0a20  aveDict, key):. 
+0000f8b0: 2020 2020 2020 2065 7869 7374 696e 6753         existingS
+0000f8c0: 6372 6565 6e20 3d20 7363 7265 656e 4469  creen = screenDi
+0000f8d0: 6374 2e67 6574 286b 6579 290a 2020 2020  ct.get(key).    
+0000f8e0: 2020 2020 6578 6973 7469 6e67 5361 7665      existingSave
+0000f8f0: 203d 2073 6176 6544 6963 742e 6765 7428   = saveDict.get(
+0000f900: 6b65 7929 0a20 2020 2020 2020 2065 7869  key).        exi
+0000f910: 7374 696e 6753 6372 6565 6e20 3d20 6622  stingScreen = f"
+0000f920: 7b65 7869 7374 696e 6753 6372 6565 6e7d  {existingScreen}
+0000f930: 2c20 2220 6966 2028 6578 6973 7469 6e67  , " if (existing
+0000f940: 5363 7265 656e 2069 7320 6e6f 7420 4e6f  Screen is not No
+0000f950: 6e65 2061 6e64 206c 656e 2865 7869 7374  ne and len(exist
+0000f960: 696e 6753 6372 6565 6e29 203e 2030 2920  ingScreen) > 0) 
+0000f970: 656c 7365 2022 220a 2020 2020 2020 2020  else "".        
+0000f980: 6578 6973 7469 6e67 5361 7665 203d 2066  existingSave = f
+0000f990: 227b 6578 6973 7469 6e67 5361 7665 7d2c  "{existingSave},
+0000f9a0: 2022 2069 6620 2865 7869 7374 696e 6753   " if (existingS
+0000f9b0: 6176 6520 6973 206e 6f74 204e 6f6e 6520  ave is not None 
+0000f9c0: 616e 6420 6c65 6e28 6578 6973 7469 6e67  and len(existing
+0000f9d0: 5361 7665 2920 3e20 3029 2065 6c73 6520  Save) > 0) else 
+0000f9e0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0000f9f0: 6e20 6578 6973 7469 6e67 5363 7265 656e  n existingScreen
+0000fa00: 2c20 6578 6973 7469 6e67 5361 7665 0a0a  , existingSave..
+0000fa10: 2020 2020 2320 406d 6561 7375 7265 5f74      # @measure_t
+0000fa20: 696d 650a 2020 2020 6465 6620 6669 6e64  ime.    def find
+0000fa30: 4262 616e 6473 5371 7565 657a 6528 7365  BbandsSqueeze(se
+0000fa40: 6c66 2c66 756c 6c44 6174 612c 2073 6372  lf,fullData, scr
+0000fa50: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+0000fa60: 742c 2066 696c 7465 723d 3429 3a0a 2020  t, filter=4):.  
+0000fa70: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000fa80: 2020 5468 6520 5454 4d20 5371 7565 657a    The TTM Squeez
+0000fa90: 6520 696e 6469 6361 746f 7220 6d65 6173  e indicator meas
+0000faa0: 7572 6573 2074 6865 2072 656c 6174 696f  ures the relatio
+0000fab0: 6e73 6869 7020 6265 7477 6565 6e20 7468  nship between th
+0000fac0: 6520 0a20 2020 2020 2020 2042 6f6c 6c69  e .        Bolli
+0000fad0: 6e67 6572 2042 616e 6473 2061 6e64 204b  nger Bands and K
+0000fae0: 656c 746e 6572 2773 2043 6861 6e6e 656c  eltner's Channel
+0000faf0: 2e20 5768 656e 2074 6865 2076 6f6c 6174  . When the volat
+0000fb00: 696c 6974 7920 696e 6372 6561 7365 732c  ility increases,
+0000fb10: 200a 2020 2020 2020 2020 736f 2064 6f65   .        so doe
+0000fb20: 7320 7468 6520 6469 7374 616e 6365 2062  s the distance b
+0000fb30: 6574 7765 656e 2074 6865 2062 616e 6473  etween the bands
+0000fb40: 2c20 616e 6420 636f 6e76 6572 7365 6c79  , and conversely
+0000fb50: 2c20 7768 656e 2074 6865 200a 2020 2020  , when the .    
+0000fb60: 2020 2020 766f 6c61 7469 6c69 7479 2064      volatility d
+0000fb70: 6563 6c69 6e65 732c 2074 6865 2064 6973  eclines, the dis
+0000fb80: 7461 6e63 6520 616c 736f 2064 6563 7265  tance also decre
+0000fb90: 6173 6573 2e20 5468 6520 5371 7565 657a  ases. The Squeez
+0000fba0: 6520 696e 6469 6361 746f 7220 0a20 2020  e indicator .   
+0000fbb0: 2020 2020 2066 696e 6473 2073 6563 7469       finds secti
+0000fbc0: 6f6e 7320 6f66 2074 6865 2042 6f6c 6c69  ons of the Bolli
+0000fbd0: 6e67 6572 2042 616e 6473 2073 7475 6479  nger Bands study
+0000fbe0: 2077 6869 6368 2066 616c 6c20 696e 7369   which fall insi
+0000fbf0: 6465 2074 6865 200a 2020 2020 2020 2020  de the .        
+0000fc00: 4b65 6c74 6e65 7227 7320 4368 616e 6e65  Keltner's Channe
+0000fc10: 6c73 2e0a 2020 2020 2020 2020 0a20 2020  ls..        .   
+0000fc20: 2020 2020 2041 7420 7468 6520 6d6f 6d65       At the mome
+0000fc30: 6e74 2074 6869 7320 7371 7565 657a 6520  nt this squeeze 
+0000fc40: 6861 7070 656e 732c 2061 2070 7269 6365  happens, a price
+0000fc50: 2062 7265 616b 6f75 7420 6672 6f6d 2074   breakout from t
+0000fc60: 6865 2075 7070 6572 200a 2020 2020 2020  he upper .      
+0000fc70: 2020 426f 6c6c 696e 6765 7220 4261 6e64    Bollinger Band
+0000fc80: 2077 6f75 6c64 2069 6e64 6963 6174 6520   would indicate 
+0000fc90: 7468 6520 706f 7373 6962 696c 6974 7920  the possibility 
+0000fca0: 6f66 2061 6e20 7570 7472 656e 6420 696e  of an uptrend in
+0000fcb0: 2074 6865 200a 2020 2020 2020 2020 6675   the .        fu
+0000fcc0: 7475 7265 2e20 5468 6973 2069 7320 6261  ture. This is ba
+0000fcd0: 636b 6564 2062 7920 7468 6520 6661 6374  cked by the fact
+0000fce0: 2074 6861 7420 6f6e 6365 2074 6865 2070   that once the p
+0000fcf0: 7269 6365 2073 7461 7274 7320 6272 6561  rice starts brea
+0000fd00: 6b69 6e67 200a 2020 2020 2020 2020 6f75  king .        ou
+0000fd10: 7420 6f66 2074 6865 2062 616e 6473 2c20  t of the bands, 
+0000fd20: 6974 2077 6f75 6c64 206d 6561 6e20 6120  it would mean a 
+0000fd30: 7265 6c61 7861 7469 6f6e 206f 6620 7468  relaxation of th
+0000fd40: 6520 7371 7565 657a 6520 616e 6420 7468  e squeeze and th
+0000fd50: 6520 0a20 2020 2020 2020 2070 6f73 7369  e .        possi
+0000fd60: 6269 6c69 7479 206f 6620 6869 6768 206d  bility of high m
+0000fd70: 6172 6b65 7420 766f 6c61 7469 6c69 7479  arket volatility
+0000fd80: 2061 6e64 2070 7269 6365 206d 6f76 656d   and price movem
+0000fd90: 656e 7420 696e 2074 6865 2066 7574 7572  ent in the futur
+0000fda0: 652e 200a 2020 2020 2020 2020 5369 6d69  e. .        Simi
+0000fdb0: 6c61 726c 792c 2061 2070 7269 6365 2062  larly, a price b
+0000fdc0: 7265 616b 6f75 7420 6672 6f6d 2074 6865  reakout from the
+0000fdd0: 206c 6f77 6572 2042 6f6c 6c69 6e67 6572   lower Bollinger
+0000fde0: 2042 616e 6420 6166 7465 7220 6120 7371   Band after a sq
+0000fdf0: 7565 657a 6520 0a20 2020 2020 2020 2077  ueeze .        w
+0000fe00: 6f75 6c64 2069 6e64 6963 6174 6520 7468  ould indicate th
+0000fe10: 6520 706f 7373 6962 696c 6974 7920 6f66  e possibility of
+0000fe20: 2061 2064 6f77 6e74 7265 6e64 2069 6e20   a downtrend in 
+0000fe30: 7468 6520 6675 7475 7265 2061 6e64 2061  the future and a
+0000fe40: 6e20 0a20 2020 2020 2020 2069 6e63 7265  n .        incre
+0000fe50: 6173 6564 206d 6172 6b65 7420 766f 6c61  ased market vola
+0000fe60: 7469 6c69 7479 2069 6e20 7468 6520 7361  tility in the sa
+0000fe70: 6d65 2064 6972 6563 7469 6f6e 2e20 5768  me direction. Wh
+0000fe80: 656e 2074 6865 206d 6172 6b65 7420 0a20  en the market . 
+0000fe90: 2020 2020 2020 2066 696e 6973 6865 7320         finishes 
+0000fea0: 6120 6d6f 7665 2c20 7468 6520 696e 6469  a move, the indi
+0000feb0: 6361 746f 7220 7475 726e 7320 6f66 662c  cator turns off,
+0000fec0: 2077 6869 6368 2063 6f72 7265 7370 6f6e   which correspon
+0000fed0: 6473 2074 6f20 6261 6e64 7320 0a20 2020  ds to bands .   
+0000fee0: 2020 2020 2068 6176 696e 6720 7075 7368       having push
+0000fef0: 6564 2077 656c 6c20 6f75 7473 6964 6520  ed well outside 
+0000ff00: 7468 6520 7261 6e67 6520 6f66 204b 656c  the range of Kel
+0000ff10: 746e 6572 2773 2043 6861 6e6e 656c 732e  tner's Channels.
+0000ff20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000ff30: 2020 2020 2069 6620 6675 6c6c 4461 7461       if fullData
+0000ff40: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
+0000ff50: 6675 6c6c 4461 7461 2920 3c20 3230 3a0a  fullData) < 20:.
+0000ff60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000ff70: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0000ff80: 206f 6c64 6573 7452 6563 6f72 6473 4669   oldestRecordsFi
+0000ff90: 7273 745f 6466 203d 2066 756c 6c44 6174  rst_df = fullDat
+0000ffa0: 612e 6865 6164 2833 3029 2e63 6f70 7928  a.head(30).copy(
+0000ffb0: 290a 2020 2020 2020 2020 6c61 7465 7374  ).        latest
+0000ffc0: 5265 636f 7264 7346 6972 7374 5f64 6620  RecordsFirst_df 
+0000ffd0: 3d20 6f6c 6465 7374 5265 636f 7264 7346  = oldestRecordsF
+0000ffe0: 6972 7374 5f64 665b 3a3a 2d31 5d2e 7461  irst_df[::-1].ta
+0000fff0: 696c 2833 3029 0a20 2020 2020 2020 206c  il(30).        l
+00010000: 6174 6573 7452 6563 6f72 6473 4669 7273  atestRecordsFirs
+00010010: 745f 6466 203d 206c 6174 6573 7452 6563  t_df = latestRec
+00010020: 6f72 6473 4669 7273 745f 6466 2e66 696c  ordsFirst_df.fil
+00010030: 6c6e 6128 3029 0a20 2020 2020 2020 206c  lna(0).        l
+00010040: 6174 6573 7452 6563 6f72 6473 4669 7273  atestRecordsFirs
+00010050: 745f 6466 203d 206c 6174 6573 7452 6563  t_df = latestRec
+00010060: 6f72 6473 4669 7273 745f 6466 2e72 6570  ordsFirst_df.rep
+00010070: 6c61 6365 285b 6e70 2e69 6e66 2c20 2d6e  lace([np.inf, -n
+00010080: 702e 696e 665d 2c20 3029 0a20 2020 2020  p.inf], 0).     
+00010090: 2020 2023 2042 6f6c 6c69 6e67 6572 2062     # Bollinger b
+000100a0: 616e 6473 0a20 2020 2020 2020 206c 6174  ands.        lat
+000100b0: 6573 7452 6563 6f72 6473 4669 7273 745f  estRecordsFirst_
+000100c0: 6466 2e6c 6f63 5b3a 2c27 4242 616e 6473  df.loc[:,'BBands
+000100d0: 2d55 275d 2c20 6c61 7465 7374 5265 636f  -U'], latestReco
+000100e0: 7264 7346 6972 7374 5f64 662e 6c6f 635b  rdsFirst_df.loc[
+000100f0: 3a2c 2742 4261 6e64 732d 4d27 5d2c 206c  :,'BBands-M'], l
+00010100: 6174 6573 7452 6563 6f72 6473 4669 7273  atestRecordsFirs
+00010110: 745f 6466 2e6c 6f63 5b3a 2c27 4242 616e  t_df.loc[:,'BBan
+00010120: 6473 2d4c 275d 203d 2070 6b74 616c 6962  ds-L'] = pktalib
+00010130: 2e42 4241 4e44 5328 6c61 7465 7374 5265  .BBANDS(latestRe
+00010140: 636f 7264 7346 6972 7374 5f64 665b 2243  cordsFirst_df["C
+00010150: 6c6f 7365 225d 2c20 3230 290a 2020 2020  lose"], 20).    
+00010160: 2020 2020 2320 636f 6d70 7574 6520 4b65      # compute Ke
+00010170: 6c74 6e65 7227 7320 6368 616e 6e65 6c0a  ltner's channel.
+00010180: 2020 2020 2020 2020 6c61 7465 7374 5265          latestRe
+00010190: 636f 7264 7346 6972 7374 5f64 665b 276c  cordsFirst_df['l
+000101a0: 6f77 5f6b 656c 275d 2c20 6c61 7465 7374  ow_kel'], latest
+000101b0: 5265 636f 7264 7346 6972 7374 5f64 665b  RecordsFirst_df[
+000101c0: 2775 7070 5f6b 656c 275d 203d 2070 6b74  'upp_kel'] = pkt
+000101d0: 616c 6962 2e4b 656c 746e 6572 7343 6861  alib.KeltnersCha
+000101e0: 6e6e 656c 286c 6174 6573 7452 6563 6f72  nnel(latestRecor
+000101f0: 6473 4669 7273 745f 6466 5b22 4869 6768  dsFirst_df["High
+00010200: 225d 2c20 6c61 7465 7374 5265 636f 7264  "], latestRecord
+00010210: 7346 6972 7374 5f64 665b 224c 6f77 225d  sFirst_df["Low"]
+00010220: 2c6c 6174 6573 7452 6563 6f72 6473 4669  ,latestRecordsFi
+00010230: 7273 745f 6466 5b22 436c 6f73 6522 5d2c  rst_df["Close"],
+00010240: 3230 290a 2020 2020 2020 2020 2320 7371  20).        # sq
+00010250: 7565 657a 6520 696e 6469 6361 746f 720a  ueeze indicator.
+00010260: 2020 2020 2020 2020 6465 6620 696e 5f73          def in_s
+00010270: 7175 6565 7a65 2864 6629 3a0a 2020 2020  queeze(df):.    
+00010280: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00010290: 665b 276c 6f77 5f6b 656c 275d 203c 2064  f['low_kel'] < d
+000102a0: 665b 2742 4261 6e64 732d 4c27 5d20 3c20  f['BBands-L'] < 
+000102b0: 6466 5b27 4242 616e 6473 2d55 275d 203c  df['BBands-U'] <
+000102c0: 2064 665b 2775 7070 5f6b 656c 275d 0a0a   df['upp_kel']..
+000102d0: 2020 2020 2020 2020 6c61 7465 7374 5265          latestRe
+000102e0: 636f 7264 7346 6972 7374 5f64 665b 2773  cordsFirst_df['s
+000102f0: 7175 6565 7a65 275d 203d 206c 6174 6573  queeze'] = lates
+00010300: 7452 6563 6f72 6473 4669 7273 745f 6466  tRecordsFirst_df
+00010310: 2e61 7070 6c79 2869 6e5f 7371 7565 657a  .apply(in_squeez
+00010320: 652c 2061 7869 733d 3129 0a0a 2020 2020  e, axis=1)..    
+00010330: 2020 2020 2320 4c65 7427 7320 7265 7669      # Let's revi
+00010340: 6577 206a 7573 7420 7468 6520 7072 6576  ew just the prev
+00010350: 696f 7573 2033 2063 616e 646c 6573 2069  ious 3 candles i
+00010360: 6e63 6c75 6469 6e67 2074 6f64 6179 2028  ncluding today (
+00010370: 6174 2074 6865 2065 6e64 290a 2020 2020  at the end).    
+00010380: 2020 2020 6c61 7465 7374 5265 636f 7264      latestRecord
+00010390: 7346 6972 7374 5f64 6620 3d20 6c61 7465  sFirst_df = late
+000103a0: 7374 5265 636f 7264 7346 6972 7374 5f64  stRecordsFirst_d
+000103b0: 662e 7461 696c 2833 290a 2020 2020 2020  f.tail(3).      
+000103c0: 2020 2320 7374 6f63 6b20 6973 2063 6f6d    # stock is com
+000103d0: 696e 6720 6f75 7420 6f66 2074 6865 2073  ing out of the s
+000103e0: 7175 6565 7a65 0a20 2020 2020 2020 2073  queeze.        s
+000103f0: 6176 6564 203d 2073 656c 662e 6669 6e64  aved = self.find
+00010400: 4375 7272 656e 7453 6176 6564 5661 6c75  CurrentSavedValu
+00010410: 6528 7363 7265 656e 4469 6374 2c20 7361  e(screenDict, sa
+00010420: 7665 4469 6374 2c20 2250 6174 7465 726e  veDict, "Pattern
+00010430: 2229 0a20 2020 2020 2020 2063 616e 646c  ").        candl
+00010440: 6533 5371 7a20 3d20 6c61 7465 7374 5265  e3Sqz = latestRe
+00010450: 636f 7264 7346 6972 7374 5f64 662e 696c  cordsFirst_df.il
+00010460: 6f63 5b2d 335d 5b22 7371 7565 657a 6522  oc[-3]["squeeze"
+00010470: 5d0a 2020 2020 2020 2020 6361 6e64 6c65  ].        candle
+00010480: 3153 717a 203d 206c 6174 6573 7452 6563  1Sqz = latestRec
+00010490: 6f72 6473 4669 7273 745f 6466 2e69 6c6f  ordsFirst_df.ilo
+000104a0: 635b 2d31 5d5b 2273 7175 6565 7a65 225d  c[-1]["squeeze"]
+000104b0: 0a20 2020 2020 2020 2063 616e 646c 6532  .        candle2
+000104c0: 5371 7a20 3d20 6c61 7465 7374 5265 636f  Sqz = latestReco
+000104d0: 7264 7346 6972 7374 5f64 662e 696c 6f63  rdsFirst_df.iloc
+000104e0: 5b2d 325d 5b22 7371 7565 657a 6522 5d0a  [-2]["squeeze"].
+000104f0: 2020 2020 2020 2020 6966 2063 616e 646c          if candl
+00010500: 6533 5371 7a20 616e 6420 6e6f 7420 6361  e3Sqz and not ca
+00010510: 6e64 6c65 3153 717a 3a0a 2020 2020 2020  ndle1Sqz:.      
+00010520: 2020 2020 2020 2320 3372 6420 6361 6e64        # 3rd cand
+00010530: 6c65 2066 726f 6d20 7468 6520 6d6f 7374  le from the most
+00010540: 2072 6563 656e 7420 6f6e 6520 7761 7320   recent one was 
+00010550: 696e 2073 7175 6565 7a65 2062 7574 2074  in squeeze but t
+00010560: 6865 206d 6f73 7420 7265 6365 6e74 206f  he most recent o
+00010570: 6e65 2069 7320 6e6f 742e 0a20 2020 2020  ne is not..     
+00010580: 2020 2020 2020 2069 6620 6669 6c74 6572         if filter
+00010590: 206e 6f74 2069 6e20 5b31 2c33 2c34 5d3a   not in [1,3,4]:
+000105a0: 2023 2042 7579 2f53 656c 6c2f 416c 6c0a   # Buy/Sell/All.
+000105b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105c0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+000105d0: 2020 2020 2020 2020 2023 2064 6563 6964           # decid
+000105e0: 6520 7768 6963 6820 6163 7469 6f6e 2074  e which action t
+000105f0: 6f20 7461 6b65 2062 7920 636f 6d70 6172  o take by compar
+00010600: 696e 6720 6469 7374 616e 6365 7320 2020  ing distances   
+00010610: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00010620: 2020 2020 2020 2020 2020 6469 7374 616e            distan
+00010630: 6365 5f74 6f5f 7570 7065 7220 3d20 6162  ce_to_upper = ab
+00010640: 7328 6c61 7465 7374 5265 636f 7264 7346  s(latestRecordsF
+00010650: 6972 7374 5f64 665b 2742 4261 6e64 732d  irst_df['BBands-
+00010660: 5527 5d2e 7661 6c75 6573 5b2d 315d 202d  U'].values[-1] -
+00010670: 206c 6174 6573 7452 6563 6f72 6473 4669   latestRecordsFi
+00010680: 7273 745f 6466 5b27 436c 6f73 6527 5d2e  rst_df['Close'].
+00010690: 7661 6c75 6573 5b2d 315d 290a 2020 2020  values[-1]).    
+000106a0: 2020 2020 2020 2020 6469 7374 616e 6365          distance
+000106b0: 5f74 6f5f 6c6f 7765 7220 3d20 6162 7328  _to_lower = abs(
+000106c0: 6c61 7465 7374 5265 636f 7264 7346 6972  latestRecordsFir
+000106d0: 7374 5f64 665b 2742 4261 6e64 732d 4c27  st_df['BBands-L'
+000106e0: 5d2e 7661 6c75 6573 5b2d 315d 202d 206c  ].values[-1] - l
+000106f0: 6174 6573 7452 6563 6f72 6473 4669 7273  atestRecordsFirs
+00010700: 745f 6466 5b27 436c 6f73 6527 5d2e 7661  t_df['Close'].va
+00010710: 6c75 6573 5b2d 315d 290a 2020 2020 2020  lues[-1]).      
+00010720: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00010730: 2020 2061 6374 696f 6e20 3d20 4661 6c73     action = Fals
+00010740: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+00010750: 2064 6973 7461 6e63 655f 746f 5f75 7070   distance_to_upp
+00010760: 6572 203c 2064 6973 7461 6e63 655f 746f  er < distance_to
+00010770: 5f6c 6f77 6572 3a0a 2020 2020 2020 2020  _lower:.        
+00010780: 2020 2020 2020 2020 6966 2066 696c 7465          if filte
+00010790: 7220 6e6f 7420 696e 205b 312c 345d 3a20  r not in [1,4]: 
+000107a0: 2320 4275 792f 416c 6c0a 2020 2020 2020  # Buy/All.      
+000107b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000107c0: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+000107d0: 2020 2020 2020 2020 2020 2061 6374 696f             actio
+000107e0: 6e20 3d20 5472 7565 0a20 2020 2020 2020  n = True.       
+000107f0: 2020 2020 2065 6c69 6620 6669 6c74 6572       elif filter
+00010800: 206e 6f74 2069 6e20 5b33 2c34 5d3a 2023   not in [3,4]: #
+00010810: 2053 656c 6c2f 416c 6c0a 2020 2020 2020   Sell/All.      
+00010820: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00010830: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+00010840: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
+00010850: 6174 7465 726e 225d 203d 2073 6176 6564  attern"] = saved
+00010860: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
+00010870: 424f 4c44 202b 2028 636f 6c6f 7254 6578  BOLD + (colorTex
+00010880: 742e 4752 4545 4e20 6966 2061 6374 696f  t.GREEN if actio
+00010890: 6e20 656c 7365 2063 6f6c 6f72 5465 7874  n else colorText
+000108a0: 2e46 4149 4c29 202b 2066 2242 4261 6e64  .FAIL) + f"BBand
+000108b0: 732d 5351 5a2d 7b27 4275 7927 2069 6620  s-SQZ-{'Buy' if 
+000108c0: 6163 7469 6f6e 2065 6c73 6520 2753 656c  action else 'Sel
+000108d0: 6c27 7d22 202b 2063 6f6c 6f72 5465 7874  l'}" + colorText
+000108e0: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
+000108f0: 2073 6176 6544 6963 745b 2250 6174 7465   saveDict["Patte
+00010900: 726e 225d 203d 2073 6176 6564 5b31 5d20  rn"] = saved[1] 
+00010910: 2b20 6622 5454 4d2d 5351 5a2d 7b27 4275  + f"TTM-SQZ-{'Bu
+00010920: 7927 2069 6620 6163 7469 6f6e 2065 6c73  y' if action els
+00010930: 6520 2753 656c 6c27 7d22 0a20 2020 2020  e 'Sell'}".     
+00010940: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00010950: 7565 0a20 2020 2020 2020 2065 6c69 6620  ue.        elif 
+00010960: 6361 6e64 6c65 3353 717a 2061 6e64 2063  candle3Sqz and c
+00010970: 616e 646c 6532 5371 7a20 616e 6420 6361  andle2Sqz and ca
+00010980: 6e64 6c65 3153 717a 3a0a 2020 2020 2020  ndle1Sqz:.      
+00010990: 2020 2020 2020 2320 4c61 7374 2033 2063        # Last 3 c
+000109a0: 616e 646c 6573 2069 6e20 7371 7565 657a  andles in squeez
+000109b0: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+000109c0: 2066 696c 7465 7220 6e6f 7420 696e 205b   filter not in [
+000109d0: 322c 345d 3a20 2320 5371 5a2f 416c 6c0a  2,4]: # SqZ/All.
+000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109f0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+00010a00: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+00010a10: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+00010a20: 2066 277b 7361 7665 645b 305d 7d7b 636f   f'{saved[0]}{co
+00010a30: 6c6f 7254 6578 742e 424f 4c44 7d7b 636f  lorText.BOLD}{co
+00010a40: 6c6f 7254 6578 742e 5741 524e 7d54 544d  lorText.WARN}TTM
+00010a50: 2d53 515a 7b63 6f6c 6f72 5465 7874 2e45  -SQZ{colorText.E
+00010a60: 4e44 7d27 0a20 2020 2020 2020 2020 2020  ND}'.           
+00010a70: 2073 6176 6544 6963 745b 2250 6174 7465   saveDict["Patte
+00010a80: 726e 225d 203d 2066 277b 7361 7665 645b  rn"] = f'{saved[
+00010a90: 315d 7d54 544d 2d53 515a 270a 2020 2020  1]}TTM-SQZ'.    
+00010aa0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00010ab0: 7275 650a 2020 2020 2020 2020 7265 7475  rue.        retu
+00010ac0: 726e 2046 616c 7365 0a0a 2020 2020 6465  rn False..    de
+00010ad0: 6620 6669 6e64 496e 7472 6164 6179 4869  f findIntradayHi
+00010ae0: 6768 4372 6f73 736f 7665 7228 7365 6c66  ghCrossover(self
+00010af0: 2c20 6466 2c20 6166 7465 7254 696d 6573  , df, afterTimes
+00010b00: 7461 6d70 3d4e 6f6e 6529 3a0a 2020 2020  tamp=None):.    
+00010b10: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
+00010b20: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
+00010b30: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+00010b40: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+00010b50: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
+00010b60: 7079 2829 0a20 2020 2020 2020 2064 6174  py().        dat
+00010b70: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
+00010b80: 3029 0a20 2020 2020 2020 2064 6174 6120  0).        data 
+00010b90: 3d20 6461 7461 2e72 6570 6c61 6365 285b  = data.replace([
+00010ba0: 6e70 2e69 6e66 2c20 2d6e 702e 696e 665d  np.inf, -np.inf]
+00010bb0: 2c20 3029 0a20 2020 2020 2020 2064 6174  , 0).        dat
+00010bc0: 6120 3d20 6461 7461 5b3a 3a2d 315d 2020  a = data[::-1]  
+00010bd0: 2320 5265 7665 7273 6520 7468 6520 6461  # Reverse the da
+00010be0: 7461 6672 616d 6520 736f 2074 6861 7420  taframe so that 
+00010bf0: 6974 7320 7468 6520 6f6c 6465 7374 2064  its the oldest d
+00010c00: 6174 6520 6669 7273 740a 2020 2020 2020  ate first.      
+00010c10: 2020 6469 6666 5f64 6620 3d20 4e6f 6e65    diff_df = None
+00010c20: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00010c30: 2020 2020 2020 2020 2020 2320 4c65 7427            # Let'
+00010c40: 7320 6f6e 6c79 2063 6f6e 7369 6465 7220  s only consider 
+00010c50: 7468 6f73 6520 6361 6e64 6c65 7320 7468  those candles th
+00010c60: 6174 2061 7265 2061 6674 6572 2074 6865  at are after the
+00010c70: 2061 6c65 7274 2069 7373 7565 2d74 696d   alert issue-tim
+00010c80: 6520 696e 2074 6865 206d 6f72 6e69 6e67  e in the morning
+00010c90: 7320 2b20 3220 6361 6e64 6c65 7320 2866  s + 2 candles (f
+00010ca0: 6f72 2062 7579 2f73 656c 6c29 0a20 2020  or buy/sell).   
+00010cb0: 2020 2020 2020 2020 2064 6966 665f 6466           diff_df
+00010cc0: 203d 2064 6174 615b 6461 7461 2e69 6e64   = data[data.ind
+00010cd0: 6578 203e 3d20 2070 642e 746f 5f64 6174  ex >=  pd.to_dat
+00010ce0: 6574 696d 6528 6627 7b50 4b44 6174 6555  etime(f'{PKDateU
+00010cf0: 7469 6c69 7469 6573 2e74 7261 6469 6e67  tilities.trading
+00010d00: 4461 7465 2829 2e73 7472 6674 696d 6528  Date().strftime(
+00010d10: 6622 2559 2d25 6d2d 2564 2229 7d20 3039  f"%Y-%m-%d")} 09
+00010d20: 3a7b 3135 2b73 656c 662e 636f 6e66 6967  :{15+self.config
+00010d30: 4d61 6e61 6765 722e 6d6f 726e 696e 6761  Manager.morninga
+00010d40: 6e61 6c79 7369 7363 616e 646c 656e 756d  nalysiscandlenum
+00010d50: 6265 7220 2b20 327d 3a30 302b 3035 3a33  ber + 2}:00+05:3
+00010d60: 3027 292e 746f 5f64 6174 6574 696d 6536  0').to_datetime6
+00010d70: 3428 295d 0a20 2020 2020 2020 2020 2020  4()].           
+00010d80: 2023 2062 726f 6b65 7253 7172 4f66 6674   # brokerSqrOfft
+00010d90: 696d 6520 3d20 7064 2e74 6f5f 6461 7465  ime = pd.to_date
+00010da0: 7469 6d65 2866 277b 504b 4461 7465 5574  time(f'{PKDateUt
+00010db0: 696c 6974 6965 732e 7472 6164 696e 6744  ilities.tradingD
+00010dc0: 6174 6528 292e 7374 7266 7469 6d65 2866  ate().strftime(f
+00010dd0: 2225 592d 256d 2d25 6422 297d 2031 353a  "%Y-%m-%d")} 15:
+00010de0: 3134 3a30 302b 3035 3a33 3027 292e 746f  14:00+05:30').to
+00010df0: 5f64 6174 6574 696d 6536 3428 290a 2020  _datetime64().  
+00010e00: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00010e10: 2020 2020 2020 2020 2020 6469 6666 5f64            diff_d
+00010e20: 6620 3d20 6461 7461 5b64 6174 612e 696e  f = data[data.in
+00010e30: 6465 7820 3e3d 2020 7064 2e74 6f5f 6461  dex >=  pd.to_da
+00010e40: 7465 7469 6d65 2866 277b 504b 4461 7465  tetime(f'{PKDate
+00010e50: 5574 696c 6974 6965 732e 7472 6164 696e  Utilities.tradin
+00010e60: 6744 6174 6528 292e 7374 7266 7469 6d65  gDate().strftime
+00010e70: 2866 2225 592d 256d 2d25 6422 297d 2030  (f"%Y-%m-%d")} 0
+00010e80: 393a 7b31 352b 7365 6c66 2e63 6f6e 6669  9:{15+self.confi
+00010e90: 674d 616e 6167 6572 2e6d 6f72 6e69 6e67  gManager.morning
+00010ea0: 616e 616c 7973 6973 6361 6e64 6c65 6e75  analysiscandlenu
+00010eb0: 6d62 6572 202b 2032 7d3a 3030 2b30 353a  mber + 2}:00+05:
+00010ec0: 3330 272c 2075 7463 3d54 7275 6529 5d0a  30', utc=True)].
+00010ed0: 2020 2020 2020 2020 2020 2020 2320 6272              # br
+00010ee0: 6f6b 6572 5371 724f 6666 7469 6d65 203d  okerSqrOfftime =
+00010ef0: 2070 642e 746f 5f64 6174 6574 696d 6528   pd.to_datetime(
+00010f00: 6627 7b50 4b44 6174 6555 7469 6c69 7469  f'{PKDateUtiliti
+00010f10: 6573 2e74 7261 6469 6e67 4461 7465 2829  es.tradingDate()
+00010f20: 2e73 7472 6674 696d 6528 6622 2559 2d25  .strftime(f"%Y-%
+00010f30: 6d2d 2564 2229 7d20 3135 3a31 343a 3030  m-%d")} 15:14:00
+00010f40: 2b30 353a 3330 272c 2075 7463 3d54 7275  +05:30', utc=Tru
+00010f50: 6529 0a20 2020 2020 2020 2020 2020 2070  e).            p
+00010f60: 6173 730a 2020 2020 2020 2020 6461 7948  ass.        dayH
+00010f70: 6967 6841 6674 6572 416c 6572 7420 3d20  ighAfterAlert = 
+00010f80: 6469 6666 5f64 665b 2248 6967 6822 5d2e  diff_df["High"].
+00010f90: 6d61 7828 290a 2020 2020 2020 2020 6869  max().        hi
+00010fa0: 6768 526f 7720 3d20 6469 6666 5f64 665b  ghRow = diff_df[
+00010fb0: 6469 6666 5f64 665b 2248 6967 6822 5d20  diff_df["High"] 
+00010fc0: 3e3d 2064 6179 4869 6768 4166 7465 7241  >= dayHighAfterA
+00010fd0: 6c65 7274 5d0a 2020 2020 2020 2020 6966  lert].        if
+00010fe0: 2068 6967 6852 6f77 2069 7320 6e6f 7420   highRow is not 
+00010ff0: 4e6f 6e65 2061 6e64 206c 656e 2868 6967  None and len(hig
+00011000: 6852 6f77 2920 3e20 303a 0a20 2020 2020  hRow) > 0:.     
+00011010: 2020 2020 2020 2068 6967 6852 6f77 203d         highRow =
+00011020: 2068 6967 6852 6f77 2e74 6169 6c28 3129   highRow.tail(1)
+00011030: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011040: 6869 6768 526f 772e 696e 6465 785b 2d31  highRow.index[-1
+00011050: 5d2c 2068 6967 6852 6f77 0a0a 0a20 2020  ], highRow...   
+00011060: 2064 6566 2066 696e 644d 4143 4443 726f   def findMACDCro
+00011070: 7373 6f76 6572 2873 656c 662c 2064 662c  ssover(self, df,
+00011080: 2061 6674 6572 5469 6d65 7374 616d 703d   afterTimestamp=
+00011090: 4e6f 6e65 2c20 6e74 6843 726f 7373 6f76  None, nthCrossov
+000110a0: 6572 3d31 2c20 7570 4469 7265 6374 696f  er=1, upDirectio
+000110b0: 6e3d 5472 7565 2c20 6d69 6e52 5349 3d36  n=True, minRSI=6
+000110c0: 3029 3a0a 2020 2020 2020 2020 6966 2064  0):.        if d
+000110d0: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+000110e0: 2864 6629 203d 3d20 303a 0a20 2020 2020  (df) == 0:.     
+000110f0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00011100: 6c73 650a 2020 2020 2020 2020 6461 7461  lse.        data
+00011110: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
+00011120: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+00011130: 2e66 696c 6c6e 6128 3029 0a20 2020 2020  .fillna(0).     
+00011140: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+00011150: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
+00011160: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
+00011170: 2020 2020 2064 6174 612e 6472 6f70 6e61       data.dropna
+00011180: 2861 7869 733d 302c 2068 6f77 3d22 616c  (axis=0, how="al
+00011190: 6c22 2c20 696e 706c 6163 653d 5472 7565  l", inplace=True
+000111a0: 2920 2320 4d61 7962 6520 7468 6572 6520  ) # Maybe there 
+000111b0: 7761 7320 6e6f 2074 7261 6465 2064 6f6e  was no trade don
+000111c0: 6520 6174 2074 6865 7365 2074 696d 6573  e at these times
+000111d0: 3f0a 2020 2020 2020 2020 6461 7461 203d  ?.        data =
+000111e0: 2064 6174 615b 3a3a 2d31 5d20 2023 2052   data[::-1]  # R
+000111f0: 6576 6572 7365 2074 6865 2064 6174 6166  everse the dataf
+00011200: 7261 6d65 2073 6f20 7468 6174 2069 7473  rame so that its
+00011210: 2074 6865 206f 6c64 6573 7420 6461 7465   the oldest date
+00011220: 2066 6972 7374 0a20 2020 2020 2020 206d   first.        m
+00011230: 6163 644c 696e 652c 206d 6163 6453 6967  acdLine, macdSig
+00011240: 6e61 6c2c 206d 6163 6448 6973 7420 3d20  nal, macdHist = 
+00011250: 706b 7461 6c69 622e 4d41 4344 2864 6174  pktalib.MACD(dat
+00011260: 615b 2243 6c6f 7365 225d 2c20 3132 2c20  a["Close"], 12, 
+00011270: 3236 2c20 3929 0a20 2020 2020 2020 2023  26, 9).        #
+00011280: 2072 7369 5f64 6620 3d20 706b 7461 6c69   rsi_df = pktali
+00011290: 622e 5253 4928 6461 7461 5b22 436c 6f73  b.RSI(data["Clos
+000112a0: 6522 5d2c 2031 3429 0a20 2020 2020 2020  e"], 14).       
+000112b0: 206c 696e 655f 6466 203d 2070 642e 4461   line_df = pd.Da
+000112c0: 7461 4672 616d 6528 6d61 6364 4c69 6e65  taFrame(macdLine
+000112d0: 290a 2020 2020 2020 2020 7369 676e 616c  ).        signal
+000112e0: 5f64 6620 3d20 7064 2e44 6174 6146 7261  _df = pd.DataFra
+000112f0: 6d65 286d 6163 6453 6967 6e61 6c29 0a20  me(macdSignal). 
+00011300: 2020 2020 2020 2076 6f6c 5f64 6620 3d20         vol_df = 
+00011310: 6461 7461 5b22 566f 6c75 6d65 225d 0a20  data["Volume"]. 
+00011320: 2020 2020 2020 2064 6966 665f 6466 203d         diff_df =
+00011330: 2070 642e 636f 6e63 6174 285b 6c69 6e65   pd.concat([line
+00011340: 5f64 662c 2073 6967 6e61 6c5f 6466 2c20  _df, signal_df, 
+00011350: 7369 676e 616c 5f64 662d 6c69 6e65 5f64  signal_df-line_d
+00011360: 662c 766f 6c5f 6466 5d2c 2061 7869 733d  f,vol_df], axis=
+00011370: 3129 0a20 2020 2020 2020 2064 6966 665f  1).        diff_
+00011380: 6466 2e63 6f6c 756d 6e73 203d 205b 226c  df.columns = ["l
+00011390: 696e 6522 2c22 7369 676e 616c 222c 2264  ine","signal","d
+000113a0: 6966 6622 2c22 766f 6c22 5d0a 2020 2020  iff","vol"].    
+000113b0: 2020 2020 6469 6666 5f64 6620 3d20 6469      diff_df = di
+000113c0: 6666 5f64 665b 6469 6666 5f64 665b 2276  ff_df[diff_df["v
+000113d0: 6f6c 225d 203e 2030 5d20 2320 5765 2772  ol"] > 0] # We'r
+000113e0: 6520 6e6f 7420 676f 696e 6720 746f 2064  e not going to d
+000113f0: 6f20 616e 7974 6869 6e67 2077 6974 6820  o anything with 
+00011400: 6120 6361 6e64 6c65 2077 6865 7265 2074  a candle where t
+00011410: 6865 7265 2077 6173 206e 6f20 7472 6164  here was no trad
+00011420: 652e 0a20 2020 2020 2020 2023 2062 726f  e..        # bro
+00011430: 6b65 7253 7172 4f66 6674 696d 6520 3d20  kerSqrOfftime = 
+00011440: 4e6f 6e65 0a20 2020 2020 2020 2074 7279  None.        try
+00011450: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00011460: 4c65 7427 7320 6f6e 6c79 2063 6f6e 7369  Let's only consi
+00011470: 6465 7220 7468 6f73 6520 6361 6e64 6c65  der those candle
+00011480: 7320 7468 6174 2061 7265 2061 6674 6572  s that are after
+00011490: 2074 6865 2061 6c65 7274 2069 7373 7565   the alert issue
+000114a0: 2d74 696d 6520 696e 2074 6865 206d 6f72  -time in the mor
+000114b0: 6e69 6e67 7320 2b20 3220 6361 6e64 6c65  nings + 2 candle
+000114c0: 7320 2866 6f72 2062 7579 2f73 656c 6c29  s (for buy/sell)
+000114d0: 0a20 2020 2020 2020 2020 2020 2064 6966  .            dif
+000114e0: 665f 6466 203d 2064 6966 665f 6466 5b64  f_df = diff_df[d
+000114f0: 6966 665f 6466 2e69 6e64 6578 203e 3d20  iff_df.index >= 
+00011500: 2070 642e 746f 5f64 6174 6574 696d 6528   pd.to_datetime(
+00011510: 6627 7b50 4b44 6174 6555 7469 6c69 7469  f'{PKDateUtiliti
+00011520: 6573 2e74 7261 6469 6e67 4461 7465 2829  es.tradingDate()
+00011530: 2e73 7472 6674 696d 6528 6622 2559 2d25  .strftime(f"%Y-%
+00011540: 6d2d 2564 2229 7d20 3039 3a7b 3135 2b73  m-%d")} 09:{15+s
+00011550: 656c 662e 636f 6e66 6967 4d61 6e61 6765  elf.configManage
+00011560: 722e 6d6f 726e 696e 6761 6e61 6c79 7369  r.morninganalysi
+00011570: 7363 616e 646c 656e 756d 6265 7220 2b20  scandlenumber + 
+00011580: 327d 3a30 302b 3035 3a33 3027 292e 746f  2}:00+05:30').to
+00011590: 5f64 6174 6574 696d 6536 3428 295d 0a20  _datetime64()]. 
+000115a0: 2020 2020 2020 2020 2020 2023 2062 726f             # bro
+000115b0: 6b65 7253 7172 4f66 6674 696d 6520 3d20  kerSqrOfftime = 
+000115c0: 7064 2e74 6f5f 6461 7465 7469 6d65 2866  pd.to_datetime(f
+000115d0: 277b 504b 4461 7465 5574 696c 6974 6965  '{PKDateUtilitie
+000115e0: 732e 7472 6164 696e 6744 6174 6528 292e  s.tradingDate().
+000115f0: 7374 7266 7469 6d65 2866 2225 592d 256d  strftime(f"%Y-%m
+00011600: 2d25 6422 297d 2031 353a 3134 3a30 302b  -%d")} 15:14:00+
+00011610: 3035 3a33 3027 292e 746f 5f64 6174 6574  05:30').to_datet
+00011620: 696d 6536 3428 290a 2020 2020 2020 2020  ime64().        
+00011630: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+00011640: 2020 2020 6469 6666 5f64 6620 3d20 6469      diff_df = di
+00011650: 6666 5f64 665b 6469 6666 5f64 662e 696e  ff_df[diff_df.in
+00011660: 6465 7820 3e3d 2020 7064 2e74 6f5f 6461  dex >=  pd.to_da
+00011670: 7465 7469 6d65 2866 277b 504b 4461 7465  tetime(f'{PKDate
+00011680: 5574 696c 6974 6965 732e 7472 6164 696e  Utilities.tradin
+00011690: 6744 6174 6528 292e 7374 7266 7469 6d65  gDate().strftime
+000116a0: 2866 2225 592d 256d 2d25 6422 297d 2030  (f"%Y-%m-%d")} 0
+000116b0: 393a 7b31 352b 7365 6c66 2e63 6f6e 6669  9:{15+self.confi
+000116c0: 674d 616e 6167 6572 2e6d 6f72 6e69 6e67  gManager.morning
+000116d0: 616e 616c 7973 6973 6361 6e64 6c65 6e75  analysiscandlenu
+000116e0: 6d62 6572 202b 2032 7d3a 3030 2b30 353a  mber + 2}:00+05:
+000116f0: 3330 272c 2075 7463 3d54 7275 6529 5d0a  30', utc=True)].
+00011700: 2020 2020 2020 2020 2020 2020 2320 6272              # br
+00011710: 6f6b 6572 5371 724f 6666 7469 6d65 203d  okerSqrOfftime =
+00011720: 2070 642e 746f 5f64 6174 6574 696d 6528   pd.to_datetime(
+00011730: 6627 7b50 4b44 6174 6555 7469 6c69 7469  f'{PKDateUtiliti
+00011740: 6573 2e74 7261 6469 6e67 4461 7465 2829  es.tradingDate()
+00011750: 2e73 7472 6674 696d 6528 6622 2559 2d25  .strftime(f"%Y-%
+00011760: 6d2d 2564 2229 7d20 3135 3a31 343a 3030  m-%d")} 15:14:00
+00011770: 2b30 353a 3330 272c 2075 7463 3d54 7275  +05:30', utc=Tru
+00011780: 6529 0a20 2020 2020 2020 2020 2020 2070  e).            p
+00011790: 6173 730a 2020 2020 2020 2020 696e 6465  ass.        inde
+000117a0: 7820 3d20 6c65 6e28 6469 6666 5f64 6629  x = len(diff_df)
+000117b0: 0a20 2020 2020 2020 2063 726f 7373 4f76  .        crossOv
+000117c0: 6572 203d 2030 0a20 2020 2020 2020 200a  er = 0.        .
+000117d0: 2020 2020 2020 2020 2320 4c6f 6f70 2075          # Loop u
+000117e0: 6e74 696c 2077 6527 7665 2066 6f75 6e64  ntil we've found
+000117f0: 2074 6865 206e 7468 2063 726f 7373 6f76   the nth crossov
+00011800: 6572 2066 6f72 204d 4143 4420 6f72 2077  er for MACD or w
+00011810: 6527 7665 2072 6561 6368 6564 2074 6865  e've reached the
+00011820: 206c 6173 7420 706f 696e 7420 696e 2074   last point in t
+00011830: 696d 650a 2020 2020 2020 2020 7768 696c  ime.        whil
+00011840: 6520 2863 726f 7373 4f76 6572 203c 206e  e (crossOver < n
+00011850: 7468 4372 6f73 736f 7665 7220 616e 6420  thCrossover and 
+00011860: 696e 6465 7820 3e3d 3029 3a0a 2020 2020  index >=0):.    
+00011870: 2020 2020 2020 2020 6966 2064 6966 665f          if diff_
+00011880: 6466 5b22 6469 6666 225d 5b69 6e64 6578  df["diff"][index
+00011890: 2d31 5d20 3c20 303a 2023 2053 6967 6e61  -1] < 0: # Signa
+000118a0: 6c20 6c69 6e65 2068 6173 206e 6f74 2063  l line has not c
+000118b0: 726f 7373 6564 2079 6574 2061 6e64 2069  rossed yet and i
+000118c0: 7320 6265 6c6f 7720 7468 6520 7a65 726f  s below the zero
+000118d0: 206c 696e 650a 2020 2020 2020 2020 2020   line.          
+000118e0: 2020 2020 2020 7768 696c 6528 2864 6966        while((dif
+000118f0: 665f 6466 5b22 6469 6666 225d 5b69 6e64  f_df["diff"][ind
+00011900: 6578 2d31 5d20 3c20 3020 616e 6420 696e  ex-1] < 0 and in
+00011910: 6465 7820 3e3d 3029 293a 2023 2061 6e64  dex >=0)): # and
+00011920: 2064 6966 665f 6466 2e69 6e64 6578 203c   diff_df.index <
+00011930: 3d20 6272 6f6b 6572 5371 724f 6666 7469  = brokerSqrOffti
+00011940: 6d65 293a 2023 206f 7220 6469 6666 5f64  me): # or diff_d
+00011950: 665b 2272 7369 225d 5b69 6e64 6578 2d31  f["rsi"][index-1
+00011960: 5d20 3c3d 206d 696e 5253 4929 3a0a 2020  ] <= minRSI):.  
+00011970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011980: 2020 2320 4c6f 6f70 2077 6869 6c65 2053    # Loop while S
+00011990: 6967 6e61 6c20 6c69 6e65 2068 6173 206e  ignal line has n
+000119a0: 6f74 2063 726f 7373 6564 2079 6574 2061  ot crossed yet a
+000119b0: 6e64 2069 7320 6265 6c6f 7720 7468 6520  nd is below the 
+000119c0: 7a65 726f 206c 696e 6520 616e 6420 7765  zero line and we
+000119d0: 2776 6520 6e6f 7420 7265 6163 6865 6420  've not reached 
+000119e0: 7468 6520 6c61 7374 2070 6f69 6e74 0a20  the last point. 
+000119f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a00: 2020 2069 6e64 6578 202d 3d20 310a 2020     index -= 1.  
+00011a10: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00011a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a30: 7768 696c 6528 2864 6966 665f 6466 5b22  while((diff_df["
+00011a40: 6469 6666 225d 5b69 6e64 6578 2d31 5d20  diff"][index-1] 
+00011a50: 3e3d 2030 2061 6e64 2069 6e64 6578 203e  >= 0 and index >
+00011a60: 3d30 2929 3a20 2320 616e 6420 6469 6666  =0)): # and diff
+00011a70: 5f64 662e 696e 6465 7820 3c3d 2062 726f  _df.index <= bro
+00011a80: 6b65 7253 7172 4f66 6674 696d 6529 3a20  kerSqrOfftime): 
+00011a90: 2320 6f72 2064 6966 665f 6466 5b22 7273  # or diff_df["rs
+00011aa0: 6922 5d5b 696e 6465 782d 315d 203c 3d20  i"][index-1] <= 
+00011ab0: 6d69 6e52 5349 293a 0a20 2020 2020 2020  minRSI):.       
+00011ac0: 2020 2020 2020 2020 2020 2020 2023 204c               # L
+00011ad0: 6f6f 7020 756e 7469 6c20 7369 676e 616c  oop until signal
+00011ae0: 206c 696e 6520 6861 7320 6e6f 7420 6372   line has not cr
+00011af0: 6f73 7365 6420 7965 7420 616e 6420 6973  ossed yet and is
+00011b00: 2061 626f 7665 2074 6865 207a 6572 6f20   above the zero 
+00011b10: 6c69 6e65 0a20 2020 2020 2020 2020 2020  line.           
+00011b20: 2020 2020 2020 2020 2069 6e64 6578 202d           index -
+00011b30: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00011b40: 6372 6f73 734f 7665 7220 2b3d 2031 0a20  crossOver += 1. 
+00011b50: 2020 2020 2020 2074 7320 3d20 6469 6666         ts = diff
+00011b60: 5f64 662e 7461 696c 286c 656e 2864 6966  _df.tail(len(dif
+00011b70: 665f 6466 292d 696e 6465 7820 2b31 292e  f_df)-index +1).
+00011b80: 6865 6164 2831 292e 696e 6465 785b 2d31  head(1).index[-1
+00011b90: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
+00011ba0: 2074 732c 2064 6174 615b 6461 7461 2e69   ts, data[data.i
+00011bb0: 6e64 6578 203d 3d20 7473 5d20 2364 662e  ndex == ts] #df.
+00011bc0: 6865 6164 286c 656e 2864 6629 202d 696e  head(len(df) -in
+00011bd0: 6465 7820 2b31 292e 7461 696c 2831 290a  dex +1).tail(1).
+00011be0: 2020 2020 0a20 2020 2023 2046 696e 6420      .    # Find 
+00011bf0: 7374 6f63 6b20 7368 6f77 696e 6720 5253  stock showing RS
+00011c00: 4920 6372 6f73 7369 6e67 2077 6974 6820  I crossing with 
+00011c10: 5253 4920 3920 534d 410a 2020 2020 6465  RSI 9 SMA.    de
+00011c20: 6620 6669 6e64 5253 4943 726f 7373 696e  f findRSICrossin
+00011c30: 674d 4128 7365 6c66 2c20 6466 2c20 7363  gMA(self, df, sc
+00011c40: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
+00011c50: 6374 2c6c 6f6f 6b46 6f72 3d31 2c20 6d61  ct,lookFor=1, ma
+00011c60: 4c65 6e67 7468 3d39 2c20 7273 694b 6579  Length=9, rsiKey
+00011c70: 3d22 5253 4922 293a 0a20 2020 2020 2020  ="RSI"):.       
+00011c80: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
+00011c90: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
+00011ca0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00011cb0: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+00011cc0: 2069 6620 7273 694b 6579 206e 6f74 2069   if rsiKey not i
+00011cd0: 6e20 6466 2e63 6f6c 756d 6e73 3a0a 2020  n df.columns:.  
+00011ce0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011cf0: 2046 616c 7365 0a20 2020 2020 2020 2064   False.        d
+00011d00: 6174 6120 3d20 6466 2e63 6f70 7928 290a  ata = df.copy().
+00011d10: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00011d20: 6174 615b 3a3a 2d31 5d0a 2020 2020 2020  ata[::-1].      
+00011d30: 2020 6d61 5273 6920 3d20 706b 7461 6c69    maRsi = pktali
+00011d40: 622e 4d41 2864 6174 615b 7273 694b 6579  b.MA(data[rsiKey
+00011d50: 5d2c 2074 696d 6570 6572 696f 643d 6d61  ], timeperiod=ma
+00011d60: 4c65 6e67 7468 290a 2020 2020 2020 2020  Length).        
+00011d70: 6461 7461 203d 2064 6174 615b 3a3a 2d31  data = data[::-1
+00011d80: 5d2e 6865 6164 2833 290a 2020 2020 2020  ].head(3).      
+00011d90: 2020 6d61 5273 6920 3d20 6d61 5273 695b    maRsi = maRsi[
+00011da0: 3a3a 2d31 5d2e 6865 6164 2833 290a 2020  ::-1].head(3).  
+00011db0: 2020 2020 2020 7361 7665 6420 3d20 7365        saved = se
+00011dc0: 6c66 2e66 696e 6443 7572 7265 6e74 5361  lf.findCurrentSa
+00011dd0: 7665 6456 616c 7565 2873 6372 6565 6e44  vedValue(screenD
+00011de0: 6963 742c 7361 7665 4469 6374 2c22 5472  ict,saveDict,"Tr
+00011df0: 656e 6422 290a 2020 2020 2020 2020 6966  end").        if
+00011e00: 206c 6f6f 6b46 6f72 2069 6e20 5b31 2c33   lookFor in [1,3
+00011e10: 5d20 616e 6420 6d61 5273 692e 696c 6f63  ] and maRsi.iloc
+00011e20: 5b30 5d20 3c3d 2064 6174 615b 7273 694b  [0] <= data[rsiK
+00011e30: 6579 5d2e 696c 6f63 5b30 5d20 616e 6420  ey].iloc[0] and 
+00011e40: 6d61 5273 692e 696c 6f63 5b31 5d20 3e20  maRsi.iloc[1] > 
+00011e50: 6461 7461 5b72 7369 4b65 795d 2e69 6c6f  data[rsiKey].ilo
+00011e60: 635b 315d 3a0a 2020 2020 2020 2020 2020  c[1]:.          
+00011e70: 2020 7363 7265 656e 4469 6374 5b27 4d41    screenDict['MA
+00011e80: 2d53 6967 6e61 6c27 5d20 3d20 7361 7665  -Signal'] = save
+00011e90: 645b 305d 202b 2063 6f6c 6f72 5465 7874  d[0] + colorText
+00011ea0: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
+00011eb0: 742e 4752 4545 4e20 2b20 6627 5253 492d  t.GREEN + f'RSI-
+00011ec0: 4d41 2d42 7579 2720 2b20 636f 6c6f 7254  MA-Buy' + colorT
+00011ed0: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+00011ee0: 2020 2020 7361 7665 4469 6374 5b27 4d41      saveDict['MA
+00011ef0: 2d53 6967 6e61 6c27 5d20 3d20 7361 7665  -Signal'] = save
+00011f00: 645b 315d 202b 2066 2752 5349 2d4d 412d  d[1] + f'RSI-MA-
+00011f10: 4275 7927 0a20 2020 2020 2020 2020 2020  Buy'.           
+00011f20: 2072 6574 7572 6e20 5472 7565 2069 6620   return True if 
+00011f30: 2872 7369 4b65 7920 3d3d 2022 5253 4969  (rsiKey == "RSIi
+00011f40: 2229 2065 6c73 6520 2873 656c 662e 6669  ") else (self.fi
+00011f50: 6e64 5253 4943 726f 7373 696e 674d 4128  ndRSICrossingMA(
+00011f60: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
+00011f70: 7361 7665 4469 6374 2c6c 6f6f 6b46 6f72  saveDict,lookFor
+00011f80: 3d6c 6f6f 6b46 6f72 2c20 6d61 4c65 6e67  =lookFor, maLeng
+00011f90: 7468 3d6d 614c 656e 6774 682c 2072 7369  th=maLength, rsi
+00011fa0: 4b65 793d 2252 5349 6922 2920 6f72 2054  Key="RSIi") or T
+00011fb0: 7275 6529 0a20 2020 2020 2020 2065 6c69  rue).        eli
+00011fc0: 6620 6c6f 6f6b 466f 7220 696e 205b 322c  f lookFor in [2,
+00011fd0: 335d 2061 6e64 206d 6152 7369 2e69 6c6f  3] and maRsi.ilo
+00011fe0: 635b 305d 203e 3d20 6461 7461 5b72 7369  c[0] >= data[rsi
+00011ff0: 4b65 795d 2e69 6c6f 635b 305d 2061 6e64  Key].iloc[0] and
+00012000: 206d 6152 7369 2e69 6c6f 635b 315d 203c   maRsi.iloc[1] <
+00012010: 2064 6174 615b 7273 694b 6579 5d2e 696c   data[rsiKey].il
+00012020: 6f63 5b31 5d3a 0a20 2020 2020 2020 2020  oc[1]:.         
+00012030: 2020 2073 6372 6565 6e44 6963 745b 274d     screenDict['M
+00012040: 412d 5369 676e 616c 275d 203d 2073 6176  A-Signal'] = sav
+00012050: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
+00012060: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
+00012070: 7874 2e46 4149 4c20 2b20 6627 5253 492d  xt.FAIL + f'RSI-
+00012080: 4d41 2d53 656c 6c27 202b 2063 6f6c 6f72  MA-Sell' + color
+00012090: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+000120a0: 2020 2020 2073 6176 6544 6963 745b 274d       saveDict['M
+000120b0: 412d 5369 676e 616c 275d 203d 2073 6176  A-Signal'] = sav
+000120c0: 6564 5b31 5d20 2b20 6627 5253 492d 4d41  ed[1] + f'RSI-MA
+000120d0: 2d53 656c 6c27 0a20 2020 2020 2020 2020  -Sell'.         
+000120e0: 2020 2072 6574 7572 6e20 5472 7565 2069     return True i
+000120f0: 6620 2872 7369 4b65 7920 3d3d 2022 5253  f (rsiKey == "RS
+00012100: 4969 2229 2065 6c73 6520 2873 656c 662e  Ii") else (self.
+00012110: 6669 6e64 5253 4943 726f 7373 696e 674d  findRSICrossingM
+00012120: 4128 6466 2c20 7363 7265 656e 4469 6374  A(df, screenDict
+00012130: 2c20 7361 7665 4469 6374 2c6c 6f6f 6b46  , saveDict,lookF
+00012140: 6f72 3d6c 6f6f 6b46 6f72 2c20 6d61 4c65  or=lookFor, maLe
+00012150: 6e67 7468 3d6d 614c 656e 6774 682c 2072  ngth=maLength, r
+00012160: 7369 4b65 793d 2252 5349 6922 2920 6f72  siKey="RSIi") or
+00012170: 2054 7275 6529 0a20 2020 2020 2020 2072   True).        r
+00012180: 6574 7572 6e20 4661 6c73 6520 6966 2028  eturn False if (
+00012190: 7273 694b 6579 203d 3d20 2252 5349 6922  rsiKey == "RSIi"
+000121a0: 2920 656c 7365 2028 7365 6c66 2e66 696e  ) else (self.fin
+000121b0: 6452 5349 4372 6f73 7369 6e67 4d41 2864  dRSICrossingMA(d
+000121c0: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
+000121d0: 6176 6544 6963 742c 6c6f 6f6b 466f 723d  aveDict,lookFor=
+000121e0: 6c6f 6f6b 466f 722c 206d 614c 656e 6774  lookFor, maLengt
+000121f0: 683d 6d61 4c65 6e67 7468 2c20 7273 694b  h=maLength, rsiK
+00012200: 6579 3d22 5253 4969 2229 290a 2020 2020  ey="RSIi")).    
+00012210: 0a20 2020 2023 2046 696e 6420 7374 6f63  .    # Find stoc
+00012220: 6b73 2077 6974 6820 7269 7369 6e67 2052  ks with rising R
+00012230: 5349 2066 726f 6d20 6c6f 7765 7220 6c65  SI from lower le
+00012240: 7665 6c73 0a20 2020 2064 6566 2066 696e  vels.    def fin
+00012250: 6452 6973 696e 6752 5349 2873 656c 662c  dRisingRSI(self,
+00012260: 2064 662c 2072 7369 4b65 793d 2252 5349   df, rsiKey="RSI
+00012270: 2229 3a0a 2020 2020 2020 2020 6966 2064  "):.        if d
+00012280: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+00012290: 2864 6629 203d 3d20 303a 0a20 2020 2020  (df) == 0:.     
+000122a0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+000122b0: 6c73 650a 2020 2020 2020 2020 6966 2072  lse.        if r
+000122c0: 7369 4b65 7920 6e6f 7420 696e 2064 662e  siKey not in df.
+000122d0: 636f 6c75 6d6e 733a 0a20 2020 2020 2020  columns:.       
+000122e0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+000122f0: 650a 2020 2020 2020 2020 6461 7461 203d  e.        data =
+00012300: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
+00012310: 2020 2064 6174 6120 3d20 6461 7461 5b3a     data = data[:
+00012320: 3a2d 315d 0a20 2020 2020 2020 2064 6174  :-1].        dat
+00012330: 6120 3d20 6461 7461 2e74 6169 6c28 3329  a = data.tail(3)
+00012340: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+00012350: 6461 7461 2920 3c20 333a 0a20 2020 2020  data) < 3:.     
+00012360: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00012370: 6c73 650a 2020 2020 2020 2020 6461 794d  lse.        dayM
+00012380: 696e 7573 3252 5349 203d 2064 6174 615b  inus2RSI = data[
+00012390: 2252 5349 225d 2e69 6c6f 635b 305d 0a20  "RSI"].iloc[0]. 
+000123a0: 2020 2020 2020 2064 6179 4d69 6e75 7331         dayMinus1
+000123b0: 5253 4920 3d20 6461 7461 5b22 5253 4922  RSI = data["RSI"
+000123c0: 5d2e 696c 6f63 5b31 5d0a 2020 2020 2020  ].iloc[1].      
+000123d0: 2020 6461 7952 5349 203d 2064 6174 615b    dayRSI = data[
+000123e0: 2252 5349 225d 2e69 6c6f 635b 325d 0a20  "RSI"].iloc[2]. 
+000123f0: 2020 2020 2020 2072 6574 7572 6e56 616c         returnVal
+00012400: 7565 203d 2028 6461 794d 696e 7573 3252  ue = (dayMinus2R
+00012410: 5349 203c 3d20 3335 2061 6e64 2064 6179  SI <= 35 and day
+00012420: 4d69 6e75 7331 5253 4920 3e20 6461 794d  Minus1RSI > dayM
+00012430: 696e 7573 3252 5349 2061 6e64 2064 6179  inus2RSI and day
+00012440: 5253 4920 3e20 6461 794d 696e 7573 3152  RSI > dayMinus1R
+00012450: 5349 2920 6f72 205c 0a20 2020 2020 2020  SI) or \.       
+00012460: 2020 2020 2020 2020 2028 6461 794d 696e           (dayMin
+00012470: 7573 3152 5349 203c 3d20 3335 2061 6e64  us1RSI <= 35 and
+00012480: 2064 6179 5253 4920 3e20 6461 794d 696e   dayRSI > dayMin
+00012490: 7573 3152 5349 290a 2020 2020 2020 2020  us1RSI).        
+000124a0: 6966 2072 7369 4b65 7920 3d3d 2022 5253  if rsiKey == "RS
+000124b0: 4922 3a0a 2020 2020 2020 2020 2020 2020  I":.            
+000124c0: 7265 7475 726e 5661 6c75 6520 3d20 7365  returnValue = se
+000124d0: 6c66 2e66 696e 6452 6973 696e 6752 5349  lf.findRisingRSI
+000124e0: 2864 662c 2072 7369 4b65 793d 2252 5349  (df, rsiKey="RSI
+000124f0: 6922 2920 6f72 2072 6574 7572 6e56 616c  i") or returnVal
+00012500: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+00012510: 6e20 7265 7475 726e 5661 6c75 650a 0a20  n returnValue.. 
+00012520: 2020 2023 406d 6561 7375 7265 5f74 696d     #@measure_tim
+00012530: 650a 2020 2020 2320 4669 6e64 206f 7574  e.    # Find out
+00012540: 2074 7265 6e64 2066 6f72 2064 6179 7320   trend for days 
+00012550: 746f 206c 6f6f 6b62 6163 6b0a 2020 2020  to lookback.    
+00012560: 6465 6620 6669 6e64 5472 656e 6428 7365  def findTrend(se
+00012570: 6c66 2c20 6466 2c20 7363 7265 656e 4469  lf, df, screenDi
+00012580: 6374 2c20 7361 7665 4469 6374 2c20 6461  ct, saveDict, da
+00012590: 7973 546f 4c6f 6f6b 6261 636b 3d4e 6f6e  ysToLookback=Non
+000125a0: 652c 2073 746f 636b 4e61 6d65 3d22 2229  e, stockName="")
+000125b0: 3a0a 2020 2020 2020 2020 6966 2064 6620  :.        if df 
+000125c0: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+000125d0: 6629 203d 3d20 303a 0a20 2020 2020 2020  f) == 0:.       
+000125e0: 2020 2020 2072 6574 7572 6e20 2255 6e6b       return "Unk
+000125f0: 6e6f 776e 220a 2020 2020 2020 2020 6461  nown".        da
+00012600: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
+00012610: 2020 2020 2020 2069 6620 6461 7973 546f         if daysTo
+00012620: 4c6f 6f6b 6261 636b 2069 7320 4e6f 6e65  Lookback is None
+00012630: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
+00012640: 7973 546f 4c6f 6f6b 6261 636b 203d 2073  ysToLookback = s
+00012650: 656c 662e 636f 6e66 6967 4d61 6e61 6765  elf.configManage
+00012660: 722e 6461 7973 546f 4c6f 6f6b 6261 636b  r.daysToLookback
+00012670: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00012680: 6461 7461 2e68 6561 6428 6461 7973 546f  data.head(daysTo
+00012690: 4c6f 6f6b 6261 636b 290a 2020 2020 2020  Lookback).      
+000126a0: 2020 6461 7461 203d 2064 6174 615b 3a3a    data = data[::
+000126b0: 2d31 5d0a 2020 2020 2020 2020 6461 7461  -1].        data
+000126c0: 203d 2064 6174 612e 7365 745f 696e 6465   = data.set_inde
+000126d0: 7828 6e70 2e61 7261 6e67 6528 6c65 6e28  x(np.arange(len(
+000126e0: 6461 7461 2929 290a 2020 2020 2020 2020  data))).        
+000126f0: 6461 7461 203d 2064 6174 612e 6669 6c6c  data = data.fill
+00012700: 6e61 2830 290a 2020 2020 2020 2020 6461  na(0).        da
+00012710: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
+00012720: 6528 5b6e 702e 696e 662c 202d 6e70 2e69  e([np.inf, -np.i
+00012730: 6e66 5d2c 2030 290a 2020 2020 2020 2020  nf], 0).        
+00012740: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
+00012750: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
+00012760: 7565 2873 6372 6565 6e44 6963 742c 7361  ue(screenDict,sa
+00012770: 7665 4469 6374 2c22 5472 656e 6422 290a  veDict,"Trend").
+00012780: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00012790: 2020 2020 2020 2020 2077 6974 6820 5375           with Su
+000127a0: 7070 7265 7373 4f75 7470 7574 2873 7570  ppressOutput(sup
+000127b0: 7072 6573 735f 7374 646f 7574 3d54 7275  press_stdout=Tru
+000127c0: 652c 2073 7570 7072 6573 735f 7374 6465  e, suppress_stde
+000127d0: 7272 3d54 7275 6529 3a0a 2020 2020 2020  rr=True):.      
+000127e0: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
+000127f0: 746f 7073 225d 203d 2064 6174 615b 2243  tops"] = data["C
+00012800: 6c6f 7365 225d 2e69 6c6f 635b 0a20 2020  lose"].iloc[.   
 00012810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012820: 2020 2020 2070 6b74 616c 6962 2e61 7267       pktalib.arg
-00012830: 7265 6c65 7874 7265 6d61 280a 2020 2020  relextrema(.    
-00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012850: 2020 2020 2020 2020 6e70 2e61 7272 6179          np.array
-00012860: 2864 6174 615b 2243 6c6f 7365 225d 292c  (data["Close"]),
-00012870: 206e 702e 6772 6561 7465 725f 6571 7561   np.greater_equa
-00012880: 6c2c 206f 7264 6572 3d31 0a20 2020 2020  l, order=1.     
-00012890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128a0: 2020 2029 5b30 5d0a 2020 2020 2020 2020     )[0].        
-000128b0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000128c0: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-000128d0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000128e0: 203d 2064 6174 612e 6669 6c6c 6e61 2830   = data.fillna(0
-000128f0: 290a 2020 2020 2020 2020 2020 2020 6461  ).            da
-00012900: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
-00012910: 6528 5b6e 702e 696e 662c 202d 6e70 2e69  e([np.inf, -np.i
-00012920: 6e66 5d2c 2030 290a 0a20 2020 2020 2020  nf], 0)..       
-00012930: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00012940: 2020 2020 2020 2020 2020 2320 6966 206c            # if l
-00012950: 656e 2864 6174 6129 203c 2064 6179 7354  en(data) < daysT
-00012960: 6f4c 6f6f 6b62 6163 6b3a 0a20 2020 2020  oLookback:.     
-00012970: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00012980: 2073 656c 662e 6465 6661 756c 745f 6c6f   self.default_lo
-00012990: 6767 6572 2e64 6562 7567 2864 6174 6129  gger.debug(data)
-000129a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000129b0: 2023 2020 2020 2072 6169 7365 2053 746f   #     raise Sto
-000129c0: 636b 4461 7461 4e6f 7441 6465 7175 6174  ckDataNotAdequat
-000129d0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000129e0: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
-000129f0: 706c 6163 6528 6e70 2e69 6e66 2c20 6e70  place(np.inf, np
-00012a00: 2e6e 616e 292e 7265 706c 6163 6528 2d6e  .nan).replace(-n
-00012a10: 702e 696e 662c 206e 702e 6e61 6e29 2e64  p.inf, np.nan).d
-00012a20: 726f 706e 6128 290a 2020 2020 2020 2020  ropna().        
-00012a30: 2020 2020 2020 2020 6966 206c 656e 2864          if len(d
-00012a40: 6174 615b 2274 6f70 7322 5d5b 6461 7461  ata["tops"][data
-00012a50: 2e74 6f70 7320 3e20 305d 2920 3e20 313a  .tops > 0]) > 1:
-00012a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012a70: 2020 2020 2073 6c6f 7065 203d 206e 702e       slope = np.
-00012a80: 706f 6c79 6669 7428 0a20 2020 2020 2020  polyfit(.       
-00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012aa0: 2064 6174 612e 696e 6465 785b 6461 7461   data.index[data
-00012ab0: 2e74 6f70 7320 3e20 305d 2c20 6461 7461  .tops > 0], data
-00012ac0: 5b22 746f 7073 225d 5b64 6174 612e 746f  ["tops"][data.to
-00012ad0: 7073 203e 2030 5d2c 2031 0a20 2020 2020  ps > 0], 1.     
-00012ae0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00012af0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00012b00: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00012b10: 2020 2020 2020 2020 2020 2020 2020 736c                sl
-00012b20: 6f70 6520 3d20 300a 2020 2020 2020 2020  ope = 0.        
-00012b30: 2020 2020 6578 6365 7074 206e 702e 6c69      except np.li
-00012b40: 6e61 6c67 2e4c 696e 416c 6745 7272 6f72  nalg.LinAlgError
-00012b50: 2061 7320 653a 2023 2070 7261 676d 613a   as e: # pragma:
-00012b60: 206e 6f20 636f 7665 720a 2020 2020 2020   no cover.      
-00012b70: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00012b80: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
-00012b90: 6275 6728 652c 2065 7863 5f69 6e66 6f3d  bug(e, exc_info=
-00012ba0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-00012bb0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-00012bc0: 5b22 5472 656e 6422 5d20 3d20 280a 2020  ["Trend"] = (.  
-00012bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012be0: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
-00012bf0: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-00012c00: 6c6f 7254 6578 742e 5741 524e 202b 2022  lorText.WARN + "
-00012c10: 556e 6b6e 6f77 6e22 202b 2063 6f6c 6f72  Unknown" + color
-00012c20: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-00012c30: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00012c40: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-00012c50: 6963 745b 2254 7265 6e64 225d 203d 2073  ict["Trend"] = s
-00012c60: 6176 6564 5b31 5d20 2b20 2255 6e6b 6e6f  aved[1] + "Unkno
-00012c70: 776e 220a 2020 2020 2020 2020 2020 2020  wn".            
-00012c80: 2020 2020 7265 7475 726e 2073 6176 6544      return saveD
-00012c90: 6963 745b 2254 7265 6e64 225d 0a20 2020  ict["Trend"].   
-00012ca0: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00012cb0: 4578 6365 7074 696f 6e20 6173 2065 3a20  Exception as e: 
-00012cc0: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
-00012cd0: 7665 720a 2020 2020 2020 2020 2020 2020  ver.            
-00012ce0: 2020 2020 7365 6c66 2e64 6566 6175 6c74      self.default
-00012cf0: 5f6c 6f67 6765 722e 6465 6275 6728 652c  _logger.debug(e,
-00012d00: 2065 7863 5f69 6e66 6f3d 5472 7565 290a   exc_info=True).
-00012d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d20: 736c 6f70 652c 205f 203d 2030 2c20 300a  slope, _ = 0, 0.
-00012d30: 2020 2020 2020 2020 2020 2020 616e 676c              angl
-00012d40: 6520 3d20 6e70 2e72 6164 3264 6567 286e  e = np.rad2deg(n
-00012d50: 702e 6172 6374 616e 2873 6c6f 7065 2929  p.arctan(slope))
-00012d60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00012d70: 616e 676c 6520 3d3d 2030 3a0a 2020 2020  angle == 0:.    
-00012d80: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-00012d90: 656e 4469 6374 5b22 5472 656e 6422 5d20  enDict["Trend"] 
-00012da0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00012db0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00012dc0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00012dd0: 4420 2b20 636f 6c6f 7254 6578 742e 5741  D + colorText.WA
-00012de0: 524e 202b 2022 556e 6b6e 6f77 6e22 202b  RN + "Unknown" +
-00012df0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
-00012e00: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00012e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012e20: 2073 6176 6544 6963 745b 2254 7265 6e64   saveDict["Trend
-00012e30: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-00012e40: 2255 6e6b 6e6f 776e 220a 2020 2020 2020  "Unknown".      
-00012e50: 2020 2020 2020 656c 6966 2061 6e67 6c65        elif angle
-00012e60: 203c 3d20 3330 2061 6e64 2061 6e67 6c65   <= 30 and angle
-00012e70: 203e 3d20 2d33 303a 0a20 2020 2020 2020   >= -30:.       
-00012e80: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00012e90: 6963 745b 2254 7265 6e64 225d 203d 2028  ict["Trend"] = (
-00012ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012eb0: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
-00012ec0: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
-00012ed0: 2063 6f6c 6f72 5465 7874 2e57 4152 4e20   colorText.WARN 
-00012ee0: 2b20 2253 6964 6577 6179 7322 202b 2063  + "Sideways" + c
-00012ef0: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
-00012f00: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00012f10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012f20: 6176 6544 6963 745b 2254 7265 6e64 225d  aveDict["Trend"]
-00012f30: 203d 2073 6176 6564 5b31 5d20 2b20 2253   = saved[1] + "S
-00012f40: 6964 6577 6179 7322 0a20 2020 2020 2020  ideways".       
-00012f50: 2020 2020 2065 6c69 6620 616e 676c 6520       elif angle 
-00012f60: 3e3d 2033 3020 616e 6420 616e 676c 6520  >= 30 and angle 
-00012f70: 3c20 3631 3a0a 2020 2020 2020 2020 2020  < 61:.          
-00012f80: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-00012f90: 5b22 5472 656e 6422 5d20 3d20 280a 2020  ["Trend"] = (.  
-00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fb0: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
-00012fc0: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-00012fd0: 6c6f 7254 6578 742e 4752 4545 4e20 2b20  lorText.GREEN + 
-00012fe0: 2257 6561 6b20 5570 2220 2b20 636f 6c6f  "Weak Up" + colo
-00012ff0: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
-00013000: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00013010: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00013020: 4469 6374 5b22 5472 656e 6422 5d20 3d20  Dict["Trend"] = 
-00013030: 7361 7665 645b 315d 202b 2022 5765 616b  saved[1] + "Weak
-00013040: 2055 7022 0a20 2020 2020 2020 2020 2020   Up".           
-00013050: 2065 6c69 6620 616e 676c 6520 3e3d 2036   elif angle >= 6
-00013060: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-00013070: 2020 2073 6372 6565 6e44 6963 745b 2254     screenDict["T
-00013080: 7265 6e64 225d 203d 2028 0a20 2020 2020  rend"] = (.     
-00013090: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000130a0: 6176 6564 5b30 5d20 2b20 636f 6c6f 7254  aved[0] + colorT
-000130b0: 6578 742e 424f 4c44 202b 2063 6f6c 6f72  ext.BOLD + color
-000130c0: 5465 7874 2e47 5245 454e 202b 2022 5374  Text.GREEN + "St
-000130d0: 726f 6e67 2055 7022 202b 2063 6f6c 6f72  rong Up" + color
-000130e0: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-000130f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00013100: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-00013110: 6963 745b 2254 7265 6e64 225d 203d 2073  ict["Trend"] = s
-00013120: 6176 6564 5b31 5d20 2b20 2253 7472 6f6e  aved[1] + "Stron
-00013130: 6720 5570 220a 2020 2020 2020 2020 2020  g Up".          
-00013140: 2020 656c 6966 2061 6e67 6c65 203c 3d20    elif angle <= 
-00013150: 2d33 3020 616e 6420 616e 676c 6520 3e20  -30 and angle > 
-00013160: 2d36 313a 0a20 2020 2020 2020 2020 2020  -61:.           
-00013170: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00013180: 2254 7265 6e64 225d 203d 2028 0a20 2020  "Trend"] = (.   
-00013190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131a0: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
-000131b0: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
-000131c0: 6f72 5465 7874 2e46 4149 4c20 2b20 2257  orText.FAIL + "W
-000131d0: 6561 6b20 446f 776e 2220 2b20 636f 6c6f  eak Down" + colo
-000131e0: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
-000131f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00013200: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00013210: 4469 6374 5b22 5472 656e 6422 5d20 3d20  Dict["Trend"] = 
-00013220: 7361 7665 645b 315d 202b 2022 5765 616b  saved[1] + "Weak
-00013230: 2044 6f77 6e22 0a20 2020 2020 2020 2020   Down".         
-00013240: 2020 2065 6c69 6620 616e 676c 6520 3c20     elif angle < 
-00013250: 2d36 303a 0a20 2020 2020 2020 2020 2020  -60:.           
-00013260: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00013270: 2254 7265 6e64 225d 203d 2028 0a20 2020  "Trend"] = (.   
-00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013290: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
-000132a0: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
-000132b0: 6f72 5465 7874 2e46 4149 4c20 2b20 2253  orText.FAIL + "S
-000132c0: 7472 6f6e 6720 446f 776e 2220 2b20 636f  trong Down" + co
-000132d0: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
-000132e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000132f0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00013300: 7665 4469 6374 5b22 5472 656e 6422 5d20  veDict["Trend"] 
-00013310: 3d20 7361 7665 645b 315d 202b 2022 5374  = saved[1] + "St
-00013320: 726f 6e67 2044 6f77 6e22 0a20 2020 2020  rong Down".     
-00013330: 2020 2065 7863 6570 7420 6e70 2e6c 696e     except np.lin
-00013340: 616c 672e 4c69 6e41 6c67 4572 726f 7220  alg.LinAlgError 
-00013350: 6173 2065 3a20 2320 7072 6167 6d61 3a20  as e: # pragma: 
-00013360: 6e6f 2063 6f76 6572 0a20 2020 2020 2020  no cover.       
-00013370: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
-00013380: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
-00013390: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
-000133a0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-000133b0: 6565 6e44 6963 745b 2254 7265 6e64 225d  eenDict["Trend"]
-000133c0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-000133d0: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
-000133e0: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
-000133f0: 2063 6f6c 6f72 5465 7874 2e57 4152 4e20   colorText.WARN 
-00013400: 2b20 2255 6e6b 6e6f 776e 2220 2b20 636f  + "Unknown" + co
-00013410: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
-00013420: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00013430: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-00013440: 5472 656e 6422 5d20 3d20 7361 7665 645b  Trend"] = saved[
-00013450: 315d 202b 2022 556e 6b6e 6f77 6e22 0a20  1] + "Unknown". 
-00013460: 2020 2020 2020 2072 6574 7572 6e20 7361         return sa
-00013470: 7665 4469 6374 5b22 5472 656e 6422 5d0a  veDict["Trend"].
-00013480: 0a20 2020 2023 2046 696e 6420 7374 6f63  .    # Find stoc
-00013490: 6b73 2061 7070 726f 6368 696e 6720 746f  ks approching to
-000134a0: 206c 6f6e 6720 7465 726d 2074 7265 6e64   long term trend
-000134b0: 6c69 6e65 730a 2020 2020 6465 6620 6669  lines.    def fi
-000134c0: 6e64 5472 656e 646c 696e 6573 2873 656c  ndTrendlines(sel
-000134d0: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
-000134e0: 742c 2073 6176 6544 6963 742c 2070 6572  t, saveDict, per
-000134f0: 6365 6e74 6167 653d 302e 3035 293a 0a20  centage=0.05):. 
-00013500: 2020 2020 2020 2023 2070 6572 696f 6420         # period 
-00013510: 3d20 696e 7428 2222 2e6a 6f69 6e28 6320  = int("".join(c 
-00013520: 666f 7220 6320 696e 2073 656c 662e 636f  for c in self.co
-00013530: 6e66 6967 4d61 6e61 6765 722e 7065 7269  nfigManager.peri
-00013540: 6f64 2069 6620 632e 6973 6469 6769 7428  od if c.isdigit(
-00013550: 2929 290a 2020 2020 2020 2020 2320 6966  ))).        # if
-00013560: 206c 656e 2864 6174 6129 203c 2070 6572   len(data) < per
-00013570: 696f 643a 0a20 2020 2020 2020 2023 2020  iod:.        #  
-00013580: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00013590: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-000135a0: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-000135b0: 2064 6174 6120 3d20 6461 7461 5b3a 3a2d   data = data[::-
-000135c0: 315d 0a20 2020 2020 2020 2064 6174 615b  1].        data[
-000135d0: 224e 756d 6265 7222 5d20 3d20 6e70 2e61  "Number"] = np.a
-000135e0: 7261 6e67 6528 6c65 6e28 6461 7461 2929  range(len(data))
-000135f0: 202b 2031 0a20 2020 2020 2020 2064 6174   + 1.        dat
-00013600: 615f 6c6f 7720 3d20 6461 7461 2e63 6f70  a_low = data.cop
-00013610: 7928 290a 2020 2020 2020 2020 706f 696e  y().        poin
-00013620: 7473 203d 2033 300a 0a20 2020 2020 2020  ts = 30..       
-00013630: 2022 2222 2049 676e 6f72 696e 6720 7468   """ Ignoring th
-00013640: 6520 5265 7369 7461 6e63 6520 666f 7220  e Resitance for 
-00013650: 6c6f 6e67 2d74 6572 6d20 7075 7270 6f73  long-term purpos
-00013660: 650a 2020 2020 2020 2020 7768 696c 6520  e.        while 
-00013670: 6c65 6e28 6461 7461 5f68 6967 6829 203e  len(data_high) >
-00013680: 2070 6f69 6e74 733a 0a20 2020 2020 2020   points:.       
-00013690: 2020 2020 2073 6c6f 7065 2c20 696e 7465       slope, inte
-000136a0: 7263 6570 742c 2072 5f76 616c 7565 2c20  rcept, r_value, 
-000136b0: 705f 7661 6c75 652c 2073 7464 5f65 7272  p_value, std_err
-000136c0: 203d 206c 696e 7265 6772 6573 7328 783d   = linregress(x=
-000136d0: 6461 7461 5f68 6967 685b 274e 756d 6265  data_high['Numbe
-000136e0: 7227 5d2c 2079 3d64 6174 615f 6869 6768  r'], y=data_high
-000136f0: 5b27 4869 6768 275d 290a 2020 2020 2020  ['High']).      
-00013700: 2020 2020 2020 6461 7461 5f68 6967 6820        data_high 
-00013710: 3d20 6461 7461 5f68 6967 682e 6c6f 635b  = data_high.loc[
-00013720: 6461 7461 5f68 6967 685b 2748 6967 6827  data_high['High'
-00013730: 5d20 3e20 736c 6f70 6520 2a20 6461 7461  ] > slope * data
-00013740: 5f68 6967 685b 274e 756d 6265 7227 5d20  _high['Number'] 
-00013750: 2b20 696e 7465 7263 6570 745d 0a20 2020  + intercept].   
-00013760: 2020 2020 2073 6c6f 7065 2c20 696e 7465       slope, inte
-00013770: 7263 6570 742c 2072 5f76 616c 7565 2c20  rcept, r_value, 
-00013780: 705f 7661 6c75 652c 2073 7464 5f65 7272  p_value, std_err
-00013790: 203d 206c 696e 7265 6772 6573 7328 783d   = linregress(x=
-000137a0: 6461 7461 5f68 6967 685b 274e 756d 6265  data_high['Numbe
-000137b0: 7227 5d2c 2079 3d64 6174 615f 6869 6768  r'], y=data_high
-000137c0: 5b27 436c 6f73 6527 5d29 0a20 2020 2020  ['Close']).     
-000137d0: 2020 2064 6174 615b 2752 6573 6973 7461     data['Resista
-000137e0: 6e63 6527 5d20 3d20 736c 6f70 6520 2a20  nce'] = slope * 
-000137f0: 6461 7461 5b27 4e75 6d62 6572 275d 202b  data['Number'] +
-00013800: 2069 6e74 6572 6365 7074 0a20 2020 2020   intercept.     
-00013810: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00013820: 7768 696c 6520 6c65 6e28 6461 7461 5f6c  while len(data_l
-00013830: 6f77 2920 3e20 706f 696e 7473 3a0a 2020  ow) > points:.  
-00013840: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-00013850: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013860: 6c6f 7065 2c20 696e 7465 7263 6570 742c  lope, intercept,
-00013870: 2072 5f76 616c 7565 2c20 705f 7661 6c75   r_value, p_valu
-00013880: 652c 2073 7464 5f65 7272 203d 206c 696e  e, std_err = lin
-00013890: 7265 6772 6573 7328 0a20 2020 2020 2020  regress(.       
-000138a0: 2020 2020 2020 2020 2020 2020 2078 3d64               x=d
-000138b0: 6174 615f 6c6f 775b 224e 756d 6265 7222  ata_low["Number"
-000138c0: 5d2c 2079 3d64 6174 615f 6c6f 775b 224c  ], y=data_low["L
-000138d0: 6f77 225d 0a20 2020 2020 2020 2020 2020  ow"].           
-000138e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-000138f0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00013900: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
-00013910: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-00013920: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013930: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
-00013940: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
-00013950: 6e66 6f3d 5472 7565 290a 2020 2020 2020  nfo=True).      
-00013960: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00013970: 7565 0a20 2020 2020 2020 2020 2020 2064  ue.            d
-00013980: 6174 615f 6c6f 7720 3d20 6461 7461 5f6c  ata_low = data_l
-00013990: 6f77 2e6c 6f63 5b0a 2020 2020 2020 2020  ow.loc[.        
-000139a0: 2020 2020 2020 2020 6461 7461 5f6c 6f77          data_low
-000139b0: 5b22 4c6f 7722 5d20 3c20 736c 6f70 6520  ["Low"] < slope 
-000139c0: 2a20 6461 7461 5f6c 6f77 5b22 4e75 6d62  * data_low["Numb
-000139d0: 6572 225d 202b 2069 6e74 6572 6365 7074  er"] + intercept
-000139e0: 0a20 2020 2020 2020 2020 2020 205d 0a0a  .            ]..
-000139f0: 2020 2020 2020 2020 736c 6f70 652c 2069          slope, i
-00013a00: 6e74 6572 6365 7074 2c20 725f 7661 6c75  ntercept, r_valu
-00013a10: 652c 2070 5f76 616c 7565 2c20 7374 645f  e, p_value, std_
-00013a20: 6572 7220 3d20 6c69 6e72 6567 7265 7373  err = linregress
-00013a30: 280a 2020 2020 2020 2020 2020 2020 783d  (.            x=
-00013a40: 6461 7461 5f6c 6f77 5b22 4e75 6d62 6572  data_low["Number
-00013a50: 225d 2c20 793d 6461 7461 5f6c 6f77 5b22  "], y=data_low["
-00013a60: 436c 6f73 6522 5d0a 2020 2020 2020 2020  Close"].        
-00013a70: 290a 2020 2020 2020 2020 6461 7461 5b22  ).        data["
-00013a80: 5375 7070 6f72 7422 5d20 3d20 736c 6f70  Support"] = slop
-00013a90: 6520 2a20 6461 7461 5b22 4e75 6d62 6572  e * data["Number
-00013aa0: 225d 202b 2069 6e74 6572 6365 7074 0a20  "] + intercept. 
-00013ab0: 2020 2020 2020 206e 6f77 203d 2064 6174         now = dat
-00013ac0: 612e 7461 696c 2831 290a 0a20 2020 2020  a.tail(1)..     
-00013ad0: 2020 206c 696d 6974 5f75 7070 6572 203d     limit_upper =
-00013ae0: 206e 6f77 5b22 5375 7070 6f72 7422 5d2e   now["Support"].
-00013af0: 696c 6f63 5b30 5d20 2b20 286e 6f77 5b22  iloc[0] + (now["
+00012820: 206c 6973 7428 0a20 2020 2020 2020 2020   list(.         
+00012830: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00012840: 6b74 616c 6962 2e61 7267 7265 6c65 7874  ktalib.argrelext
+00012850: 7265 6d61 280a 2020 2020 2020 2020 2020  rema(.          
+00012860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012870: 2020 6e70 2e61 7272 6179 2864 6174 615b    np.array(data[
+00012880: 2243 6c6f 7365 225d 292c 206e 702e 6772  "Close"]), np.gr
+00012890: 6561 7465 725f 6571 7561 6c2c 206f 7264  eater_equal, ord
+000128a0: 6572 3d31 0a20 2020 2020 2020 2020 2020  er=1.           
+000128b0: 2020 2020 2020 2020 2020 2020 2029 5b30               )[0
+000128c0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000128d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000128e0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+000128f0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00012900: 612e 6669 6c6c 6e61 2830 290a 2020 2020  a.fillna(0).    
+00012910: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00012920: 6174 612e 7265 706c 6163 6528 5b6e 702e  ata.replace([np.
+00012930: 696e 662c 202d 6e70 2e69 6e66 5d2c 2030  inf, -np.inf], 0
+00012940: 290a 0a20 2020 2020 2020 2020 2020 2074  )..            t
+00012950: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00012960: 2020 2020 2320 6966 206c 656e 2864 6174      # if len(dat
+00012970: 6129 203c 2064 6179 7354 6f4c 6f6f 6b62  a) < daysToLookb
+00012980: 6163 6b3a 0a20 2020 2020 2020 2020 2020  ack:.           
+00012990: 2020 2020 2023 2020 2020 2073 656c 662e       #     self.
+000129a0: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
+000129b0: 6562 7567 2864 6174 6129 0a20 2020 2020  ebug(data).     
+000129c0: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+000129d0: 2072 6169 7365 2053 746f 636b 4461 7461   raise StockData
+000129e0: 4e6f 7441 6465 7175 6174 650a 2020 2020  NotAdequate.    
+000129f0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00012a00: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
+00012a10: 6e70 2e69 6e66 2c20 6e70 2e6e 616e 292e  np.inf, np.nan).
+00012a20: 7265 706c 6163 6528 2d6e 702e 696e 662c  replace(-np.inf,
+00012a30: 206e 702e 6e61 6e29 2e64 726f 706e 6128   np.nan).dropna(
+00012a40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012a50: 2020 6966 206c 656e 2864 6174 615b 2274    if len(data["t
+00012a60: 6f70 7322 5d5b 6461 7461 2e74 6f70 7320  ops"][data.tops 
+00012a70: 3e20 305d 2920 3e20 313a 0a20 2020 2020  > 0]) > 1:.     
+00012a80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012a90: 6c6f 7065 203d 206e 702e 706f 6c79 6669  lope = np.polyfi
+00012aa0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00012ab0: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+00012ac0: 696e 6465 785b 6461 7461 2e74 6f70 7320  index[data.tops 
+00012ad0: 3e20 305d 2c20 6461 7461 5b22 746f 7073  > 0], data["tops
+00012ae0: 225d 5b64 6174 612e 746f 7073 203e 2030  "][data.tops > 0
+00012af0: 5d2c 2031 0a20 2020 2020 2020 2020 2020  ], 1.           
+00012b00: 2020 2020 2020 2020 2029 5b30 5d0a 2020           )[0].  
+00012b10: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00012b20: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00012b30: 2020 2020 2020 2020 736c 6f70 6520 3d20          slope = 
+00012b40: 300a 2020 2020 2020 2020 2020 2020 6578  0.            ex
+00012b50: 6365 7074 206e 702e 6c69 6e61 6c67 2e4c  cept np.linalg.L
+00012b60: 696e 416c 6745 7272 6f72 2061 7320 653a  inAlgError as e:
+00012b70: 2023 2070 7261 676d 613a 206e 6f20 636f   # pragma: no co
+00012b80: 7665 720a 2020 2020 2020 2020 2020 2020  ver.            
+00012b90: 2020 2020 7365 6c66 2e64 6566 6175 6c74      self.default
+00012ba0: 5f6c 6f67 6765 722e 6465 6275 6728 652c  _logger.debug(e,
+00012bb0: 2065 7863 5f69 6e66 6f3d 5472 7565 290a   exc_info=True).
+00012bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bd0: 7363 7265 656e 4469 6374 5b22 5472 656e  screenDict["Tren
+00012be0: 6422 5d20 3d20 280a 2020 2020 2020 2020  d"] = (.        
+00012bf0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00012c00: 645b 305d 202b 2063 6f6c 6f72 5465 7874  d[0] + colorText
+00012c10: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
+00012c20: 742e 5741 524e 202b 2022 556e 6b6e 6f77  t.WARN + "Unknow
+00012c30: 6e22 202b 2063 6f6c 6f72 5465 7874 2e45  n" + colorText.E
+00012c40: 4e44 0a20 2020 2020 2020 2020 2020 2020  ND.             
+00012c50: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00012c60: 2020 2020 2073 6176 6544 6963 745b 2254       saveDict["T
+00012c70: 7265 6e64 225d 203d 2073 6176 6564 5b31  rend"] = saved[1
+00012c80: 5d20 2b20 2255 6e6b 6e6f 776e 220a 2020  ] + "Unknown".  
+00012c90: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00012ca0: 7475 726e 2073 6176 6544 6963 745b 2254  turn saveDict["T
+00012cb0: 7265 6e64 225d 0a20 2020 2020 2020 2020  rend"].         
+00012cc0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00012cd0: 696f 6e20 6173 2065 3a20 2023 2070 7261  ion as e:  # pra
+00012ce0: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
+00012cf0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012d00: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
+00012d10: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
+00012d20: 6e66 6f3d 5472 7565 290a 2020 2020 2020  nfo=True).      
+00012d30: 2020 2020 2020 2020 2020 736c 6f70 652c            slope,
+00012d40: 205f 203d 2030 2c20 300a 2020 2020 2020   _ = 0, 0.      
+00012d50: 2020 2020 2020 616e 676c 6520 3d20 6e70        angle = np
+00012d60: 2e72 6164 3264 6567 286e 702e 6172 6374  .rad2deg(np.arct
+00012d70: 616e 2873 6c6f 7065 2929 0a20 2020 2020  an(slope)).     
+00012d80: 2020 2020 2020 2069 6620 616e 676c 6520         if angle 
+00012d90: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00012da0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+00012db0: 5b22 5472 656e 6422 5d20 3d20 280a 2020  ["Trend"] = (.  
+00012dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012dd0: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
+00012de0: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
+00012df0: 6c6f 7254 6578 742e 5741 524e 202b 2022  lorText.WARN + "
+00012e00: 556e 6b6e 6f77 6e22 202b 2063 6f6c 6f72  Unknown" + color
+00012e10: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+00012e20: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00012e30: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+00012e40: 6963 745b 2254 7265 6e64 225d 203d 2073  ict["Trend"] = s
+00012e50: 6176 6564 5b31 5d20 2b20 2255 6e6b 6e6f  aved[1] + "Unkno
+00012e60: 776e 220a 2020 2020 2020 2020 2020 2020  wn".            
+00012e70: 656c 6966 2061 6e67 6c65 203c 3d20 3330  elif angle <= 30
+00012e80: 2061 6e64 2061 6e67 6c65 203e 3d20 2d33   and angle >= -3
+00012e90: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+00012ea0: 2020 2073 6372 6565 6e44 6963 745b 2254     screenDict["T
+00012eb0: 7265 6e64 225d 203d 2028 0a20 2020 2020  rend"] = (.     
+00012ec0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012ed0: 6176 6564 5b30 5d20 2b20 636f 6c6f 7254  aved[0] + colorT
+00012ee0: 6578 742e 424f 4c44 202b 2063 6f6c 6f72  ext.BOLD + color
+00012ef0: 5465 7874 2e57 4152 4e20 2b20 2253 6964  Text.WARN + "Sid
+00012f00: 6577 6179 7322 202b 2063 6f6c 6f72 5465  eways" + colorTe
+00012f10: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
+00012f20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00012f30: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00012f40: 745b 2254 7265 6e64 225d 203d 2073 6176  t["Trend"] = sav
+00012f50: 6564 5b31 5d20 2b20 2253 6964 6577 6179  ed[1] + "Sideway
+00012f60: 7322 0a20 2020 2020 2020 2020 2020 2065  s".            e
+00012f70: 6c69 6620 616e 676c 6520 3e3d 2033 3020  lif angle >= 30 
+00012f80: 616e 6420 616e 676c 6520 3c20 3631 3a0a  and angle < 61:.
+00012f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012fa0: 7363 7265 656e 4469 6374 5b22 5472 656e  screenDict["Tren
+00012fb0: 6422 5d20 3d20 280a 2020 2020 2020 2020  d"] = (.        
+00012fc0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00012fd0: 645b 305d 202b 2063 6f6c 6f72 5465 7874  d[0] + colorText
+00012fe0: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
+00012ff0: 742e 4752 4545 4e20 2b20 2257 6561 6b20  t.GREEN + "Weak 
+00013000: 5570 2220 2b20 636f 6c6f 7254 6578 742e  Up" + colorText.
+00013010: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
+00013020: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00013030: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
+00013040: 5472 656e 6422 5d20 3d20 7361 7665 645b  Trend"] = saved[
+00013050: 315d 202b 2022 5765 616b 2055 7022 0a20  1] + "Weak Up". 
+00013060: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00013070: 616e 676c 6520 3e3d 2036 303a 0a20 2020  angle >= 60:.   
+00013080: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00013090: 6565 6e44 6963 745b 2254 7265 6e64 225d  eenDict["Trend"]
+000130a0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+000130b0: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
+000130c0: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
+000130d0: 4c44 202b 2063 6f6c 6f72 5465 7874 2e47  LD + colorText.G
+000130e0: 5245 454e 202b 2022 5374 726f 6e67 2055  REEN + "Strong U
+000130f0: 7022 202b 2063 6f6c 6f72 5465 7874 2e45  p" + colorText.E
+00013100: 4e44 0a20 2020 2020 2020 2020 2020 2020  ND.             
+00013110: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00013120: 2020 2020 2073 6176 6544 6963 745b 2254       saveDict["T
+00013130: 7265 6e64 225d 203d 2073 6176 6564 5b31  rend"] = saved[1
+00013140: 5d20 2b20 2253 7472 6f6e 6720 5570 220a  ] + "Strong Up".
+00013150: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00013160: 2061 6e67 6c65 203c 3d20 2d33 3020 616e   angle <= -30 an
+00013170: 6420 616e 676c 6520 3e20 2d36 313a 0a20  d angle > -61:. 
+00013180: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013190: 6372 6565 6e44 6963 745b 2254 7265 6e64  creenDict["Trend
+000131a0: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
+000131b0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+000131c0: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
+000131d0: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
+000131e0: 2e46 4149 4c20 2b20 2257 6561 6b20 446f  .FAIL + "Weak Do
+000131f0: 776e 2220 2b20 636f 6c6f 7254 6578 742e  wn" + colorText.
+00013200: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
+00013210: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00013220: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
+00013230: 5472 656e 6422 5d20 3d20 7361 7665 645b  Trend"] = saved[
+00013240: 315d 202b 2022 5765 616b 2044 6f77 6e22  1] + "Weak Down"
+00013250: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00013260: 6620 616e 676c 6520 3c20 2d36 303a 0a20  f angle < -60:. 
+00013270: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013280: 6372 6565 6e44 6963 745b 2254 7265 6e64  creenDict["Trend
+00013290: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
+000132a0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+000132b0: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
+000132c0: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
+000132d0: 2e46 4149 4c20 2b20 2253 7472 6f6e 6720  .FAIL + "Strong 
+000132e0: 446f 776e 2220 2b20 636f 6c6f 7254 6578  Down" + colorTex
+000132f0: 742e 454e 440a 2020 2020 2020 2020 2020  t.END.          
+00013300: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00013310: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+00013320: 5b22 5472 656e 6422 5d20 3d20 7361 7665  ["Trend"] = save
+00013330: 645b 315d 202b 2022 5374 726f 6e67 2044  d[1] + "Strong D
+00013340: 6f77 6e22 0a20 2020 2020 2020 2065 7863  own".        exc
+00013350: 6570 7420 6e70 2e6c 696e 616c 672e 4c69  ept np.linalg.Li
+00013360: 6e41 6c67 4572 726f 7220 6173 2065 3a20  nAlgError as e: 
+00013370: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+00013380: 6572 0a20 2020 2020 2020 2020 2020 2073  er.            s
+00013390: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
+000133a0: 6572 2e64 6562 7567 2865 2c20 6578 635f  er.debug(e, exc_
+000133b0: 696e 666f 3d54 7275 6529 0a20 2020 2020  info=True).     
+000133c0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+000133d0: 745b 2254 7265 6e64 225d 203d 2028 0a20  t["Trend"] = (. 
+000133e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000133f0: 6176 6564 5b30 5d20 2b20 636f 6c6f 7254  aved[0] + colorT
+00013400: 6578 742e 424f 4c44 202b 2063 6f6c 6f72  ext.BOLD + color
+00013410: 5465 7874 2e57 4152 4e20 2b20 2255 6e6b  Text.WARN + "Unk
+00013420: 6e6f 776e 2220 2b20 636f 6c6f 7254 6578  nown" + colorTex
+00013430: 742e 454e 440a 2020 2020 2020 2020 2020  t.END.          
+00013440: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00013450: 7361 7665 4469 6374 5b22 5472 656e 6422  saveDict["Trend"
+00013460: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
+00013470: 556e 6b6e 6f77 6e22 0a20 2020 2020 2020  Unknown".       
+00013480: 2072 6574 7572 6e20 7361 7665 4469 6374   return saveDict
+00013490: 5b22 5472 656e 6422 5d0a 0a20 2020 2023  ["Trend"]..    #
+000134a0: 2046 696e 6420 7374 6f63 6b73 2061 7070   Find stocks app
+000134b0: 726f 6368 696e 6720 746f 206c 6f6e 6720  roching to long 
+000134c0: 7465 726d 2074 7265 6e64 6c69 6e65 730a  term trendlines.
+000134d0: 2020 2020 6465 6620 6669 6e64 5472 656e      def findTren
+000134e0: 646c 696e 6573 2873 656c 662c 2064 662c  dlines(self, df,
+000134f0: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
+00013500: 6544 6963 742c 2070 6572 6365 6e74 6167  eDict, percentag
+00013510: 653d 302e 3035 293a 0a20 2020 2020 2020  e=0.05):.       
+00013520: 2023 2070 6572 696f 6420 3d20 696e 7428   # period = int(
+00013530: 2222 2e6a 6f69 6e28 6320 666f 7220 6320  "".join(c for c 
+00013540: 696e 2073 656c 662e 636f 6e66 6967 4d61  in self.configMa
+00013550: 6e61 6765 722e 7065 7269 6f64 2069 6620  nager.period if 
+00013560: 632e 6973 6469 6769 7428 2929 290a 2020  c.isdigit())).  
+00013570: 2020 2020 2020 2320 6966 206c 656e 2864        # if len(d
+00013580: 6174 6129 203c 2070 6572 696f 643a 0a20  ata) < period:. 
+00013590: 2020 2020 2020 2023 2020 2020 2072 6574         #     ret
+000135a0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+000135b0: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
+000135c0: 2829 0a20 2020 2020 2020 2064 6174 6120  ().        data 
+000135d0: 3d20 6461 7461 5b3a 3a2d 315d 0a20 2020  = data[::-1].   
+000135e0: 2020 2020 2064 6174 615b 224e 756d 6265       data["Numbe
+000135f0: 7222 5d20 3d20 6e70 2e61 7261 6e67 6528  r"] = np.arange(
+00013600: 6c65 6e28 6461 7461 2929 202b 2031 0a20  len(data)) + 1. 
+00013610: 2020 2020 2020 2064 6174 615f 6c6f 7720         data_low 
+00013620: 3d20 6461 7461 2e63 6f70 7928 290a 2020  = data.copy().  
+00013630: 2020 2020 2020 706f 696e 7473 203d 2033        points = 3
+00013640: 300a 0a20 2020 2020 2020 2022 2222 2049  0..        """ I
+00013650: 676e 6f72 696e 6720 7468 6520 5265 7369  gnoring the Resi
+00013660: 7461 6e63 6520 666f 7220 6c6f 6e67 2d74  tance for long-t
+00013670: 6572 6d20 7075 7270 6f73 650a 2020 2020  erm purpose.    
+00013680: 2020 2020 7768 696c 6520 6c65 6e28 6461      while len(da
+00013690: 7461 5f68 6967 6829 203e 2070 6f69 6e74  ta_high) > point
+000136a0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+000136b0: 6c6f 7065 2c20 696e 7465 7263 6570 742c  lope, intercept,
+000136c0: 2072 5f76 616c 7565 2c20 705f 7661 6c75   r_value, p_valu
+000136d0: 652c 2073 7464 5f65 7272 203d 206c 696e  e, std_err = lin
+000136e0: 7265 6772 6573 7328 783d 6461 7461 5f68  regress(x=data_h
+000136f0: 6967 685b 274e 756d 6265 7227 5d2c 2079  igh['Number'], y
+00013700: 3d64 6174 615f 6869 6768 5b27 4869 6768  =data_high['High
+00013710: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
+00013720: 6461 7461 5f68 6967 6820 3d20 6461 7461  data_high = data
+00013730: 5f68 6967 682e 6c6f 635b 6461 7461 5f68  _high.loc[data_h
+00013740: 6967 685b 2748 6967 6827 5d20 3e20 736c  igh['High'] > sl
+00013750: 6f70 6520 2a20 6461 7461 5f68 6967 685b  ope * data_high[
+00013760: 274e 756d 6265 7227 5d20 2b20 696e 7465  'Number'] + inte
+00013770: 7263 6570 745d 0a20 2020 2020 2020 2073  rcept].        s
+00013780: 6c6f 7065 2c20 696e 7465 7263 6570 742c  lope, intercept,
+00013790: 2072 5f76 616c 7565 2c20 705f 7661 6c75   r_value, p_valu
+000137a0: 652c 2073 7464 5f65 7272 203d 206c 696e  e, std_err = lin
+000137b0: 7265 6772 6573 7328 783d 6461 7461 5f68  regress(x=data_h
+000137c0: 6967 685b 274e 756d 6265 7227 5d2c 2079  igh['Number'], y
+000137d0: 3d64 6174 615f 6869 6768 5b27 436c 6f73  =data_high['Clos
+000137e0: 6527 5d29 0a20 2020 2020 2020 2064 6174  e']).        dat
+000137f0: 615b 2752 6573 6973 7461 6e63 6527 5d20  a['Resistance'] 
+00013800: 3d20 736c 6f70 6520 2a20 6461 7461 5b27  = slope * data['
+00013810: 4e75 6d62 6572 275d 202b 2069 6e74 6572  Number'] + inter
+00013820: 6365 7074 0a20 2020 2020 2020 2022 2222  cept.        """
+00013830: 0a0a 2020 2020 2020 2020 7768 696c 6520  ..        while 
+00013840: 6c65 6e28 6461 7461 5f6c 6f77 2920 3e20  len(data_low) > 
+00013850: 706f 696e 7473 3a0a 2020 2020 2020 2020  points:.        
+00013860: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00013870: 2020 2020 2020 2020 2073 6c6f 7065 2c20           slope, 
+00013880: 696e 7465 7263 6570 742c 2072 5f76 616c  intercept, r_val
+00013890: 7565 2c20 705f 7661 6c75 652c 2073 7464  ue, p_value, std
+000138a0: 5f65 7272 203d 206c 696e 7265 6772 6573  _err = linregres
+000138b0: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+000138c0: 2020 2020 2020 2078 3d64 6174 615f 6c6f         x=data_lo
+000138d0: 775b 224e 756d 6265 7222 5d2c 2079 3d64  w["Number"], y=d
+000138e0: 6174 615f 6c6f 775b 224c 6f77 225d 0a20  ata_low["Low"]. 
+000138f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00013900: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00013910: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00013920: 2065 3a20 2023 2070 7261 676d 613a 206e   e:  # pragma: n
+00013930: 6f20 636f 7665 720a 2020 2020 2020 2020  o cover.        
+00013940: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
+00013950: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
+00013960: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
+00013970: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00013980: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+00013990: 2020 2020 2020 2020 2064 6174 615f 6c6f           data_lo
+000139a0: 7720 3d20 6461 7461 5f6c 6f77 2e6c 6f63  w = data_low.loc
+000139b0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+000139c0: 2020 6461 7461 5f6c 6f77 5b22 4c6f 7722    data_low["Low"
+000139d0: 5d20 3c20 736c 6f70 6520 2a20 6461 7461  ] < slope * data
+000139e0: 5f6c 6f77 5b22 4e75 6d62 6572 225d 202b  _low["Number"] +
+000139f0: 2069 6e74 6572 6365 7074 0a20 2020 2020   intercept.     
+00013a00: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
+00013a10: 2020 736c 6f70 652c 2069 6e74 6572 6365    slope, interce
+00013a20: 7074 2c20 725f 7661 6c75 652c 2070 5f76  pt, r_value, p_v
+00013a30: 616c 7565 2c20 7374 645f 6572 7220 3d20  alue, std_err = 
+00013a40: 6c69 6e72 6567 7265 7373 280a 2020 2020  linregress(.    
+00013a50: 2020 2020 2020 2020 783d 6461 7461 5f6c          x=data_l
+00013a60: 6f77 5b22 4e75 6d62 6572 225d 2c20 793d  ow["Number"], y=
+00013a70: 6461 7461 5f6c 6f77 5b22 436c 6f73 6522  data_low["Close"
+00013a80: 5d0a 2020 2020 2020 2020 290a 2020 2020  ].        ).    
+00013a90: 2020 2020 6461 7461 5b22 5375 7070 6f72      data["Suppor
+00013aa0: 7422 5d20 3d20 736c 6f70 6520 2a20 6461  t"] = slope * da
+00013ab0: 7461 5b22 4e75 6d62 6572 225d 202b 2069  ta["Number"] + i
+00013ac0: 6e74 6572 6365 7074 0a20 2020 2020 2020  ntercept.       
+00013ad0: 206e 6f77 203d 2064 6174 612e 7461 696c   now = data.tail
+00013ae0: 2831 290a 0a20 2020 2020 2020 206c 696d  (1)..        lim
+00013af0: 6974 5f75 7070 6572 203d 206e 6f77 5b22  it_upper = now["
 00013b00: 5375 7070 6f72 7422 5d2e 696c 6f63 5b30  Support"].iloc[0
-00013b10: 5d20 2a20 7065 7263 656e 7461 6765 290a  ] * percentage).
-00013b20: 2020 2020 2020 2020 6c69 6d69 745f 6c6f          limit_lo
-00013b30: 7765 7220 3d20 6e6f 775b 2253 7570 706f  wer = now["Suppo
-00013b40: 7274 225d 2e69 6c6f 635b 305d 202d 2028  rt"].iloc[0] - (
+00013b10: 5d20 2b20 286e 6f77 5b22 5375 7070 6f72  ] + (now["Suppor
+00013b20: 7422 5d2e 696c 6f63 5b30 5d20 2a20 7065  t"].iloc[0] * pe
+00013b30: 7263 656e 7461 6765 290a 2020 2020 2020  rcentage).      
+00013b40: 2020 6c69 6d69 745f 6c6f 7765 7220 3d20    limit_lower = 
 00013b50: 6e6f 775b 2253 7570 706f 7274 225d 2e69  now["Support"].i
-00013b60: 6c6f 635b 305d 202a 2070 6572 6365 6e74  loc[0] * percent
-00013b70: 6167 6529 0a20 2020 2020 2020 2073 6176  age).        sav
-00013b80: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
-00013b90: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
-00013ba0: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
-00013bb0: 4469 6374 2c20 2250 6174 7465 726e 2229  Dict, "Pattern")
-00013bc0: 0a20 2020 2020 2020 2069 6620 6c69 6d69  .        if limi
-00013bd0: 745f 6c6f 7765 7220 3c20 6e6f 775b 2243  t_lower < now["C
-00013be0: 6c6f 7365 225d 2e69 6c6f 635b 305d 203c  lose"].iloc[0] <
-00013bf0: 206c 696d 6974 5f75 7070 6572 2061 6e64   limit_upper and
-00013c00: 2073 6c6f 7065 203e 2030 2e31 353a 0a20   slope > 0.15:. 
-00013c10: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00013c20: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
-00013c30: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00013c40: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
-00013c50: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
-00013c60: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
-00013c70: 202b 2022 5472 656e 646c 696e 652d 5375   + "Trendline-Su
-00013c80: 7070 6f72 7422 202b 2063 6f6c 6f72 5465  pport" + colorTe
-00013c90: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
-00013ca0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00013cb0: 2073 6176 6544 6963 745b 2250 6174 7465   saveDict["Patte
-00013cc0: 726e 225d 203d 2073 6176 6564 5b31 5d20  rn"] = saved[1] 
-00013cd0: 2b20 2254 7265 6e64 6c69 6e65 2d53 7570  + "Trendline-Sup
-00013ce0: 706f 7274 220a 2020 2020 2020 2020 2020  port".          
-00013cf0: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
-00013d00: 2020 2020 2020 2022 2222 2050 6c6f 7473         """ Plots
-00013d10: 2066 6f72 2064 6562 7567 6769 6e67 0a20   for debugging. 
-00013d20: 2020 2020 2020 2069 6d70 6f72 7420 6d61         import ma
-00013d30: 7470 6c6f 746c 6962 2e70 7970 6c6f 7420  tplotlib.pyplot 
-00013d40: 6173 2070 6c74 0a20 2020 2020 2020 2066  as plt.        f
-00013d50: 6967 2c20 6178 3120 3d20 706c 742e 7375  ig, ax1 = plt.su
-00013d60: 6270 6c6f 7473 2866 6967 7369 7a65 3d28  bplots(figsize=(
-00013d70: 3135 2c31 3029 290a 2020 2020 2020 2020  15,10)).        
-00013d80: 636f 6c6f 7220 3d20 2774 6162 3a67 7265  color = 'tab:gre
-00013d90: 656e 270a 2020 2020 2020 2020 7864 6174  en'.        xdat
-00013da0: 6520 3d20 5b78 2e64 6174 6528 2920 666f  e = [x.date() fo
-00013db0: 7220 7820 696e 2064 6174 612e 696e 6465  r x in data.inde
-00013dc0: 785d 0a20 2020 2020 2020 2061 7831 2e73  x].        ax1.s
-00013dd0: 6574 5f78 6c61 6265 6c28 2744 6174 6527  et_xlabel('Date'
-00013de0: 2c20 636f 6c6f 723d 636f 6c6f 7229 0a20  , color=color). 
-00013df0: 2020 2020 2020 2061 7831 2e70 6c6f 7428         ax1.plot(
-00013e00: 7864 6174 652c 2064 6174 612e 436c 6f73  xdate, data.Clos
-00013e10: 652c 206c 6162 656c 3d22 636c 6f73 6522  e, label="close"
-00013e20: 2c20 636f 6c6f 723d 636f 6c6f 7229 0a20  , color=color). 
-00013e30: 2020 2020 2020 2061 7831 2e74 6963 6b5f         ax1.tick_
-00013e40: 7061 7261 6d73 2861 7869 733d 2778 272c  params(axis='x',
-00013e50: 206c 6162 656c 636f 6c6f 723d 636f 6c6f   labelcolor=colo
-00013e60: 7229 0a0a 2020 2020 2020 2020 6178 3220  r)..        ax2 
-00013e70: 3d20 6178 312e 7477 696e 7928 2920 2320  = ax1.twiny() # 
-00013e80: 6178 3220 616e 6420 6178 3120 7769 6c6c  ax2 and ax1 will
-00013e90: 2068 6176 6520 636f 6d6d 6f6e 2079 2061   have common y a
-00013ea0: 7869 7320 616e 6420 6469 6666 6572 656e  xis and differen
-00013eb0: 7420 7820 6178 6973 2c20 7477 696e 790a  t x axis, twiny.
-00013ec0: 2020 2020 2020 2020 6178 322e 706c 6f74          ax2.plot
-00013ed0: 2864 6174 612e 4e75 6d62 6572 2c20 6461  (data.Number, da
-00013ee0: 7461 2e52 6573 6973 7461 6e63 652c 206c  ta.Resistance, l
-00013ef0: 6162 656c 3d22 5265 7322 290a 2020 2020  abel="Res").    
-00013f00: 2020 2020 6178 322e 706c 6f74 2864 6174      ax2.plot(dat
-00013f10: 612e 4e75 6d62 6572 2c20 6461 7461 2e53  a.Number, data.S
-00013f20: 7570 706f 7274 2c20 6c61 6265 6c3d 2253  upport, label="S
-00013f30: 7570 2229 0a0a 2020 2020 2020 2020 706c  up")..        pl
-00013f40: 742e 6c65 6765 6e64 2829 0a20 2020 2020  t.legend().     
-00013f50: 2020 2070 6c74 2e67 7269 6428 290a 2020     plt.grid().  
-00013f60: 2020 2020 2020 706c 742e 7368 6f77 2829        plt.show()
-00013f70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013f80: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00013f90: 650a 0a20 2020 2023 2040 6d65 6173 7572  e..    # @measur
-00013fa0: 655f 7469 6d65 0a20 2020 2064 6566 2066  e_time.    def f
-00013fb0: 696e 6455 7074 7265 6e64 2873 656c 662c  indUptrend(self,
-00013fc0: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
-00013fd0: 2073 6176 6544 6963 742c 2074 6573 7469   saveDict, testi
-00013fe0: 6e67 2c20 7374 6f63 6b2c 6f6e 6c79 4d46  ng, stock,onlyMF
-00013ff0: 3d46 616c 7365 2c68 6f73 7444 6174 613d  =False,hostData=
-00014000: 4e6f 6e65 2c65 7863 6861 6e67 654e 616d  None,exchangeNam
-00014010: 653d 2249 4e44 4941 222c 7265 6672 6573  e="INDIA",refres
-00014020: 684d 4641 6e64 4656 3d54 7275 6529 3a0a  hMFAndFV=True):.
-00014030: 2020 2020 2020 2020 2320 7368 6f75 6c64          # should
-00014040: 5072 6f63 6565 6420 3d20 5472 7565 0a20  Proceed = True. 
-00014050: 2020 2020 2020 2069 7355 7074 7265 6e64         isUptrend
-00014060: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00014070: 2069 7344 6f77 6e74 7265 6e64 203d 2046   isDowntrend = F
-00014080: 616c 7365 0a20 2020 2020 2020 2069 7335  alse.        is5
-00014090: 3044 4d41 5570 7472 656e 6420 3d20 4661  0DMAUptrend = Fa
-000140a0: 6c73 650a 2020 2020 2020 2020 6973 3530  lse.        is50
-000140b0: 444d 4144 6f77 6e74 7265 6e64 203d 2046  DMADowntrend = F
-000140c0: 616c 7365 0a20 2020 2020 2020 2064 6563  alse.        dec
-000140d0: 6973 696f 6e20 3d20 2222 0a20 2020 2020  ision = "".     
-000140e0: 2020 2064 6d61 3530 6465 6369 7369 6f6e     dma50decision
-000140f0: 203d 2022 220a 2020 2020 2020 2020 6661   = "".        fa
-00014100: 6972 5661 6c75 6520 3d20 300a 2020 2020  irValue = 0.    
-00014110: 2020 2020 6661 6972 5661 6c75 6544 6966      fairValueDif
-00014120: 6620 3d20 300a 2020 2020 2020 2020 2320  f = 0.        # 
-00014130: 6966 2064 6620 6973 204e 6f6e 6520 6f72  if df is None or
-00014140: 206c 656e 2864 6629 203c 2032 3230 206f   len(df) < 220 o
-00014150: 7220 7465 7374 696e 673a 0a20 2020 2020  r testing:.     
-00014160: 2020 2023 2020 2020 2073 686f 756c 6450     #     shouldP
-00014170: 726f 6365 6564 203d 2046 616c 7365 0a20  roceed = False. 
-00014180: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
-00014190: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000141a0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-000141b0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-000141c0: 3d20 6466 2e63 6f70 7928 290a 2020 2020  = df.copy().    
-000141d0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000141e0: 203d 2064 6174 615b 3a3a 2d31 5d0a 2020   = data[::-1].  
-000141f0: 2020 2020 2020 2020 2020 2020 2020 746f                to
-00014200: 6461 795f 736d 6120 3d20 706b 7461 6c69  day_sma = pktali
-00014210: 622e 534d 4128 6461 7461 5b22 436c 6f73  b.SMA(data["Clos
-00014220: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
-00014230: 3530 290a 2020 2020 2020 2020 2020 2020  50).            
-00014240: 2020 2020 736d 615f 6d69 6e75 7339 203d      sma_minus9 =
-00014250: 2070 6b74 616c 6962 2e53 4d41 2864 6174   pktalib.SMA(dat
-00014260: 612e 6865 6164 286c 656e 2864 6174 6129  a.head(len(data)
-00014270: 2d39 295b 2243 6c6f 7365 225d 2c20 7469  -9)["Close"], ti
-00014280: 6d65 7065 7269 6f64 3d35 3029 0a20 2020  meperiod=50).   
-00014290: 2020 2020 2020 2020 2020 2020 2073 6d61               sma
-000142a0: 5f6d 696e 7573 3134 203d 2070 6b74 616c  _minus14 = pktal
-000142b0: 6962 2e53 4d41 2864 6174 612e 6865 6164  ib.SMA(data.head
-000142c0: 286c 656e 2864 6174 6129 2d31 3429 5b22  (len(data)-14)["
-000142d0: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-000142e0: 696f 643d 3530 290a 2020 2020 2020 2020  iod=50).        
-000142f0: 2020 2020 2020 2020 736d 615f 6d69 6e75          sma_minu
-00014300: 7332 3020 3d20 706b 7461 6c69 622e 534d  s20 = pktalib.SM
-00014310: 4128 6461 7461 2e68 6561 6428 6c65 6e28  A(data.head(len(
-00014320: 6461 7461 292d 3230 295b 2243 6c6f 7365  data)-20)["Close
-00014330: 225d 2c20 7469 6d65 7065 7269 6f64 3d35  "], timeperiod=5
-00014340: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
-00014350: 2020 2074 6f64 6179 5f6c 6d61 203d 2070     today_lma = p
-00014360: 6b74 616c 6962 2e53 4d41 2864 6174 615b  ktalib.SMA(data[
-00014370: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
-00014380: 7269 6f64 3d32 3030 290a 2020 2020 2020  riod=200).      
-00014390: 2020 2020 2020 2020 2020 6c6d 615f 6d69            lma_mi
-000143a0: 6e75 7332 3020 3d20 706b 7461 6c69 622e  nus20 = pktalib.
-000143b0: 534d 4128 6461 7461 2e68 6561 6428 6c65  SMA(data.head(le
-000143c0: 6e28 6461 7461 292d 3230 295b 2243 6c6f  n(data)-20)["Clo
-000143d0: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
-000143e0: 3d32 3030 290a 2020 2020 2020 2020 2020  =200).          
-000143f0: 2020 2020 2020 6c6d 615f 6d69 6e75 7338        lma_minus8
-00014400: 3020 3d20 706b 7461 6c69 622e 534d 4128  0 = pktalib.SMA(
-00014410: 6461 7461 2e68 6561 6428 6c65 6e28 6461  data.head(len(da
-00014420: 7461 292d 3830 295b 2243 6c6f 7365 225d  ta)-80)["Close"]
-00014430: 2c20 7469 6d65 7065 7269 6f64 3d32 3030  , timeperiod=200
-00014440: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014450: 2020 6c6d 615f 6d69 6e75 7331 3030 203d    lma_minus100 =
-00014460: 2070 6b74 616c 6962 2e53 4d41 2864 6174   pktalib.SMA(dat
-00014470: 612e 6865 6164 286c 656e 2864 6174 6129  a.head(len(data)
-00014480: 2d31 3030 295b 2243 6c6f 7365 225d 2c20  -100)["Close"], 
-00014490: 7469 6d65 7065 7269 6f64 3d32 3030 290a  timeperiod=200).
-000144a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144b0: 746f 6461 795f 6c6d 6120 3d20 746f 6461  today_lma = toda
-000144c0: 795f 6c6d 612e 696c 6f63 5b6c 656e 2874  y_lma.iloc[len(t
-000144d0: 6f64 6179 5f6c 6d61 292d 315d 2069 6620  oday_lma)-1] if 
-000144e0: 746f 6461 795f 6c6d 6120 6973 206e 6f74  today_lma is not
-000144f0: 204e 6f6e 6520 656c 7365 2030 0a20 2020   None else 0.   
-00014500: 2020 2020 2020 2020 2020 2020 206c 6d61               lma
-00014510: 5f6d 696e 7573 3230 203d 206c 6d61 5f6d  _minus20 = lma_m
-00014520: 696e 7573 3230 2e69 6c6f 635b 6c65 6e28  inus20.iloc[len(
-00014530: 6c6d 615f 6d69 6e75 7332 3029 2d31 5d20  lma_minus20)-1] 
-00014540: 6966 206c 6d61 5f6d 696e 7573 3230 2069  if lma_minus20 i
-00014550: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-00014560: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-00014570: 2020 6c6d 615f 6d69 6e75 7338 3020 3d20    lma_minus80 = 
-00014580: 6c6d 615f 6d69 6e75 7338 302e 696c 6f63  lma_minus80.iloc
-00014590: 5b6c 656e 286c 6d61 5f6d 696e 7573 3830  [len(lma_minus80
-000145a0: 292d 315d 2069 6620 6c6d 615f 6d69 6e75  )-1] if lma_minu
-000145b0: 7338 3020 6973 206e 6f74 204e 6f6e 6520  s80 is not None 
-000145c0: 656c 7365 2030 0a20 2020 2020 2020 2020  else 0.         
-000145d0: 2020 2020 2020 206c 6d61 5f6d 696e 7573         lma_minus
-000145e0: 3130 3020 3d20 6c6d 615f 6d69 6e75 7331  100 = lma_minus1
-000145f0: 3030 2e69 6c6f 635b 6c65 6e28 6c6d 615f  00.iloc[len(lma_
-00014600: 6d69 6e75 7331 3030 292d 315d 2069 6620  minus100)-1] if 
-00014610: 6c6d 615f 6d69 6e75 7331 3030 2069 7320  lma_minus100 is 
-00014620: 6e6f 7420 4e6f 6e65 2065 6c73 6520 300a  not None else 0.
-00014630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014640: 746f 6461 795f 736d 6120 3d20 746f 6461  today_sma = toda
-00014650: 795f 736d 612e 696c 6f63 5b6c 656e 2874  y_sma.iloc[len(t
-00014660: 6f64 6179 5f73 6d61 292d 315d 2069 6620  oday_sma)-1] if 
-00014670: 746f 6461 795f 736d 6120 6973 206e 6f74  today_sma is not
-00014680: 204e 6f6e 6520 656c 7365 2030 0a20 2020   None else 0.   
-00014690: 2020 2020 2020 2020 2020 2020 2073 6d61               sma
-000146a0: 5f6d 696e 7573 3920 3d20 736d 615f 6d69  _minus9 = sma_mi
-000146b0: 6e75 7339 2e69 6c6f 635b 6c65 6e28 736d  nus9.iloc[len(sm
-000146c0: 615f 6d69 6e75 7339 292d 315d 2069 6620  a_minus9)-1] if 
-000146d0: 736d 615f 6d69 6e75 7339 2069 7320 6e6f  sma_minus9 is no
-000146e0: 7420 4e6f 6e65 2065 6c73 6520 300a 2020  t None else 0.  
-000146f0: 2020 2020 2020 2020 2020 2020 2020 736d                sm
-00014700: 615f 6d69 6e75 7331 3420 3d20 736d 615f  a_minus14 = sma_
-00014710: 6d69 6e75 7331 342e 696c 6f63 5b6c 656e  minus14.iloc[len
-00014720: 2873 6d61 5f6d 696e 7573 3134 292d 315d  (sma_minus14)-1]
-00014730: 2069 6620 736d 615f 6d69 6e75 7331 3420   if sma_minus14 
-00014740: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
-00014750: 2030 0a20 2020 2020 2020 2020 2020 2020   0.             
-00014760: 2020 2073 6d61 5f6d 696e 7573 3230 203d     sma_minus20 =
-00014770: 2073 6d61 5f6d 696e 7573 3230 2e69 6c6f   sma_minus20.ilo
-00014780: 635b 6c65 6e28 736d 615f 6d69 6e75 7332  c[len(sma_minus2
-00014790: 3029 2d31 5d20 6966 2073 6d61 5f6d 696e  0)-1] if sma_min
-000147a0: 7573 3230 2069 7320 6e6f 7420 4e6f 6e65  us20 is not None
-000147b0: 2065 6c73 6520 300a 2020 2020 2020 2020   else 0.        
-000147c0: 2020 2020 2020 2020 6973 5570 7472 656e          isUptren
-000147d0: 6420 3d20 2874 6f64 6179 5f6c 6d61 203e  d = (today_lma >
-000147e0: 206c 6d61 5f6d 696e 7573 3230 2920 6f72   lma_minus20) or
-000147f0: 2028 746f 6461 795f 6c6d 6120 3e20 6c6d   (today_lma > lm
-00014800: 615f 6d69 6e75 7338 3029 206f 7220 2874  a_minus80) or (t
-00014810: 6f64 6179 5f6c 6d61 203e 206c 6d61 5f6d  oday_lma > lma_m
-00014820: 696e 7573 3130 3029 0a20 2020 2020 2020  inus100).       
-00014830: 2020 2020 2020 2020 2069 7344 6f77 6e74           isDownt
-00014840: 7265 6e64 203d 2028 746f 6461 795f 6c6d  rend = (today_lm
-00014850: 6120 3c20 6c6d 615f 6d69 6e75 7332 3029  a < lma_minus20)
-00014860: 2061 6e64 2028 746f 6461 795f 6c6d 6120   and (today_lma 
-00014870: 3c20 6c6d 615f 6d69 6e75 7338 3029 2061  < lma_minus80) a
-00014880: 6e64 2028 746f 6461 795f 6c6d 6120 3c20  nd (today_lma < 
-00014890: 6c6d 615f 6d69 6e75 7331 3030 290a 2020  lma_minus100).  
-000148a0: 2020 2020 2020 2020 2020 2020 2020 6973                is
-000148b0: 3530 444d 4155 7074 7265 6e64 203d 2028  50DMAUptrend = (
-000148c0: 746f 6461 795f 736d 6120 3e20 736d 615f  today_sma > sma_
-000148d0: 6d69 6e75 7339 2920 6f72 2028 746f 6461  minus9) or (toda
-000148e0: 795f 736d 6120 3e20 736d 615f 6d69 6e75  y_sma > sma_minu
-000148f0: 7331 3429 206f 7220 2874 6f64 6179 5f73  s14) or (today_s
-00014900: 6d61 203e 2073 6d61 5f6d 696e 7573 3230  ma > sma_minus20
-00014910: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014920: 2020 6973 3530 444d 4144 6f77 6e74 7265    is50DMADowntre
-00014930: 6e64 203d 2028 746f 6461 795f 736d 6120  nd = (today_sma 
-00014940: 3c20 736d 615f 6d69 6e75 7339 2920 616e  < sma_minus9) an
-00014950: 6420 2874 6f64 6179 5f73 6d61 203c 2073  d (today_sma < s
-00014960: 6d61 5f6d 696e 7573 3134 2920 616e 6420  ma_minus14) and 
-00014970: 2874 6f64 6179 5f73 6d61 203c 2073 6d61  (today_sma < sma
-00014980: 5f6d 696e 7573 3230 290a 2020 2020 2020  _minus20).      
-00014990: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-000149a0: 6570 7469 6f6e 3a20 2023 2070 7261 676d  eption:  # pragm
-000149b0: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
-000149c0: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-000149d0: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
-000149e0: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
-000149f0: 6e66 6f3d 5472 7565 290a 2020 2020 2020  nfo=True).      
-00014a00: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
-00014a10: 2020 2020 2020 2064 6563 6973 696f 6e20         decision 
-00014a20: 3d20 2754 3ae2 96b2 2720 6966 2069 7355  = 'T:...' if isU
-00014a30: 7074 7265 6e64 2065 6c73 6520 2827 543a  ptrend else ('T:
-00014a40: e296 bc27 2069 6620 6973 446f 776e 7472  ...' if isDowntr
-00014a50: 656e 6420 656c 7365 2027 2729 0a20 2020  end else '').   
-00014a60: 2020 2020 2064 6d61 3530 6465 6369 7369       dma50decisi
-00014a70: 6f6e 203d 2027 743a e296 b227 2069 6620  on = 't:...' if 
-00014a80: 6973 3530 444d 4155 7074 7265 6e64 2065  is50DMAUptrend e
-00014a90: 6c73 6520 2827 743a e296 bc27 2069 6620  lse ('t:...' if 
-00014aa0: 6973 3530 444d 4144 6f77 6e74 7265 6e64  is50DMADowntrend
-00014ab0: 2065 6c73 6520 2727 290a 2020 2020 2020   else '').      
-00014ac0: 2020 6d66 5f69 6e73 745f 6f77 6e65 7273    mf_inst_owners
-00014ad0: 6869 7043 6861 6e67 6520 3d20 300a 2020  hipChange = 0.  
-00014ae0: 2020 2020 2020 6368 616e 6765 5f6d 696c        change_mil
-00014af0: 6c69 6f6e 7320 3d22 220a 2020 2020 2020  lions ="".      
-00014b00: 2020 6d66 203d 2022 220a 2020 2020 2020    mf = "".      
-00014b10: 2020 6d66 7320 3d20 2222 0a20 2020 2020    mfs = "".     
-00014b20: 2020 2069 6620 7265 6672 6573 684d 4641     if refreshMFA
-00014b30: 6e64 4656 3a0a 2020 2020 2020 2020 2020  ndFV:.          
-00014b40: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00014b50: 2020 2020 2020 206d 665f 696e 7374 5f6f         mf_inst_o
-00014b60: 776e 6572 7368 6970 4368 616e 6765 203d  wnershipChange =
-00014b70: 2073 656c 662e 6765 744d 7574 7561 6c46   self.getMutualF
-00014b80: 756e 6453 7461 7475 7328 7374 6f63 6b2c  undStatus(stock,
-00014b90: 6f6e 6c79 4d46 3d6f 6e6c 794d 462c 686f  onlyMF=onlyMF,ho
-00014ba0: 7374 4461 7461 3d68 6f73 7444 6174 612c  stData=hostData,
-00014bb0: 666f 7263 653d 2868 6f73 7444 6174 6120  force=(hostData 
-00014bc0: 6973 204e 6f6e 6520 6f72 2068 6f73 7444  is None or hostD
-00014bd0: 6174 612e 656d 7074 7920 6f72 206e 6f74  ata.empty or not
-00014be0: 2028 224d 4622 2069 6e20 686f 7374 4461   ("MF" in hostDa
-00014bf0: 7461 2e63 6f6c 756d 6e73 206f 7220 2246  ta.columns or "F
-00014c00: 4949 2220 696e 2068 6f73 7444 6174 612e  II" in hostData.
-00014c10: 636f 6c75 6d6e 7329 292c 6578 6368 616e  columns)),exchan
-00014c20: 6765 4e61 6d65 3d65 7863 6861 6e67 654e  geName=exchangeN
-00014c30: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00014c40: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-00014c50: 6365 286d 665f 696e 7374 5f6f 776e 6572  ce(mf_inst_owner
-00014c60: 7368 6970 4368 616e 6765 2c20 7064 2e53  shipChange, pd.S
-00014c70: 6572 6965 7329 3a0a 2020 2020 2020 2020  eries):.        
-00014c80: 2020 2020 2020 2020 2020 2020 6d66 5f69              mf_i
-00014c90: 6e73 745f 6f77 6e65 7273 6869 7043 6861  nst_ownershipCha
-00014ca0: 6e67 6520 3d20 300a 2020 2020 2020 2020  nge = 0.        
-00014cb0: 2020 2020 2020 2020 726f 756e 644f 6666          roundOff
-00014cc0: 203d 2032 0a20 2020 2020 2020 2020 2020   = 2.           
-00014cd0: 2020 2020 206d 696c 6c69 6f6e 7320 3d20       millions = 
-00014ce0: 726f 756e 6428 6d66 5f69 6e73 745f 6f77  round(mf_inst_ow
-00014cf0: 6e65 7273 6869 7043 6861 6e67 652f 3130  nershipChange/10
-00014d00: 3030 3030 302c 726f 756e 644f 6666 290a  00000,roundOff).
-00014d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d20: 7768 696c 6520 666c 6f61 7428 6d69 6c6c  while float(mill
-00014d30: 696f 6e73 2920 3d3d 2030 2061 6e64 2072  ions) == 0 and r
-00014d40: 6f75 6e64 4f66 6620 3c3d 353a 0a20 2020  oundOff <=5:.   
-00014d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d60: 2072 6f75 6e64 4f66 6620 2b3d 310a 2020   roundOff +=1.  
-00014d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d80: 2020 6d69 6c6c 696f 6e73 203d 2072 6f75    millions = rou
-00014d90: 6e64 286d 665f 696e 7374 5f6f 776e 6572  nd(mf_inst_owner
-00014da0: 7368 6970 4368 616e 6765 2f31 3030 3030  shipChange/10000
-00014db0: 3030 2c72 6f75 6e64 4f66 6629 0a20 2020  00,roundOff).   
-00014dc0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00014dd0: 6e67 655f 6d69 6c6c 696f 6e73 203d 2066  nge_millions = f
-00014de0: 2228 7b6d 696c 6c69 6f6e 737d 4d29 220a  "({millions}M)".
-00014df0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00014e00: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00014e10: 653a 2020 2320 7072 6167 6d61 3a20 6e6f  e:  # pragma: no
-00014e20: 2063 6f76 6572 0a20 2020 2020 2020 2020   cover.         
-00014e30: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
-00014e40: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
-00014e50: 2865 2c20 6578 635f 696e 666f 3d54 7275  (e, exc_info=Tru
-00014e60: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00014e70: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-00014e80: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00014e90: 2020 2020 2020 2020 2023 4c65 7427 7320           #Let's 
-00014ea0: 6765 7420 7468 6520 6661 6972 2076 616c  get the fair val
-00014eb0: 7565 2c20 6569 7468 6572 2073 6176 6564  ue, either saved
-00014ec0: 206f 7220 6672 6573 6820 6672 6f6d 2073   or fresh from s
-00014ed0: 6572 7669 6365 0a20 2020 2020 2020 2020  ervice.         
-00014ee0: 2020 2020 2020 2066 6169 7256 616c 7565         fairValue
-00014ef0: 203d 2073 656c 662e 6765 7446 6169 7256   = self.getFairV
-00014f00: 616c 7565 2873 746f 636b 2c68 6f73 7444  alue(stock,hostD
-00014f10: 6174 612c 666f 7263 653d 2868 6f73 7444  ata,force=(hostD
-00014f20: 6174 6120 6973 204e 6f6e 6520 6f72 2068  ata is None or h
-00014f30: 6f73 7444 6174 612e 656d 7074 7920 6f72  ostData.empty or
-00014f40: 2022 4661 6972 5661 6c75 6522 206e 6f74   "FairValue" not
-00014f50: 2069 6e20 686f 7374 4461 7461 2e63 6f6c   in hostData.col
-00014f60: 756d 6e73 292c 6578 6368 616e 6765 4e61  umns),exchangeNa
-00014f70: 6d65 3d65 7863 6861 6e67 654e 616d 6529  me=exchangeName)
-00014f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014f90: 2069 6620 6661 6972 5661 6c75 6520 6973   if fairValue is
-00014fa0: 206e 6f74 204e 6f6e 6520 616e 6420 6661   not None and fa
-00014fb0: 6972 5661 6c75 6520 213d 2030 3a0a 2020  irValue != 0:.  
-00014fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fd0: 2020 6c74 7020 3d20 7361 7665 4469 6374    ltp = saveDict
-00014fe0: 5b22 4c54 5022 5d0a 2020 2020 2020 2020  ["LTP"].        
-00014ff0: 2020 2020 2020 2020 2020 2020 6661 6972              fair
-00015000: 5661 6c75 6544 6966 6620 3d20 726f 756e  ValueDiff = roun
-00015010: 6428 6661 6972 5661 6c75 6520 2d20 6c74  d(fairValue - lt
-00015020: 702c 3029 0a20 2020 2020 2020 2020 2020  p,0).           
-00015030: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00015040: 745b 2246 6169 7256 616c 7565 225d 203d  t["FairValue"] =
-00015050: 2073 7472 2866 6169 7256 616c 7565 290a   str(fairValue).
-00015060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015070: 2020 2020 7361 7665 4469 6374 5b22 4656      saveDict["FV
-00015080: 4469 6666 225d 203d 2066 6169 7256 616c  Diff"] = fairVal
-00015090: 7565 4469 6666 0a20 2020 2020 2020 2020  ueDiff.         
-000150a0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-000150b0: 6e44 6963 745b 2246 5644 6966 6622 5d20  nDict["FVDiff"] 
-000150c0: 3d20 6661 6972 5661 6c75 6544 6966 660a  = fairValueDiff.
-000150d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150e0: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-000150f0: 4661 6972 5661 6c75 6522 5d20 3d20 2863  FairValue"] = (c
-00015100: 6f6c 6f72 5465 7874 2e47 5245 454e 2069  olorText.GREEN i
-00015110: 6620 6661 6972 5661 6c75 6520 3e3d 206c  f fairValue >= l
-00015120: 7470 2065 6c73 6520 636f 6c6f 7254 6578  tp else colorTex
-00015130: 742e 4641 494c 2920 2b20 7361 7665 4469  t.FAIL) + saveDi
-00015140: 6374 5b22 4661 6972 5661 6c75 6522 5d20  ct["FairValue"] 
-00015150: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-00015160: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00015170: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00015180: 653a 2020 2320 7072 6167 6d61 3a20 6e6f  e:  # pragma: no
-00015190: 2063 6f76 6572 0a20 2020 2020 2020 2020   cover.         
-000151a0: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
-000151b0: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
-000151c0: 2865 2c20 6578 635f 696e 666f 3d54 7275  (e, exc_info=Tru
-000151d0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-000151e0: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-000151f0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00015200: 2069 6620 6d66 5f69 6e73 745f 6f77 6e65   if mf_inst_owne
-00015210: 7273 6869 7043 6861 6e67 6520 3e20 303a  rshipChange > 0:
-00015220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015230: 206d 6620 3d20 6622 4d46 493a e296 b220   mf = f"MFI:... 
-00015240: 7b63 6861 6e67 655f 6d69 6c6c 696f 6e73  {change_millions
-00015250: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-00015260: 2020 206d 6673 203d 2063 6f6c 6f72 5465     mfs = colorTe
-00015270: 7874 2e47 5245 454e 202b 206d 6620 2b20  xt.GREEN + mf + 
-00015280: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-00015290: 2020 2020 2020 2020 2020 656c 6966 206d            elif m
-000152a0: 665f 696e 7374 5f6f 776e 6572 7368 6970  f_inst_ownership
-000152b0: 4368 616e 6765 203c 2030 3a0a 2020 2020  Change < 0:.    
-000152c0: 2020 2020 2020 2020 2020 2020 6d66 203d              mf =
-000152d0: 2066 224d 4649 3ae2 96bc 207b 6368 616e   f"MFI:... {chan
-000152e0: 6765 5f6d 696c 6c69 6f6e 737d 220a 2020  ge_millions}".  
-000152f0: 2020 2020 2020 2020 2020 2020 2020 6d66                mf
-00015300: 7320 3d20 636f 6c6f 7254 6578 742e 4641  s = colorText.FA
-00015310: 494c 202b 206d 6620 2b20 636f 6c6f 7254  IL + mf + colorT
-00015320: 6578 742e 454e 440a 0a20 2020 2020 2020  ext.END..       
-00015330: 2073 6176 6564 203d 2073 656c 662e 6669   saved = self.fi
-00015340: 6e64 4375 7272 656e 7453 6176 6564 5661  ndCurrentSavedVa
-00015350: 6c75 6528 7363 7265 656e 4469 6374 2c73  lue(screenDict,s
-00015360: 6176 6544 6963 742c 2254 7265 6e64 2229  aveDict,"Trend")
-00015370: 0a20 2020 2020 2020 2064 6563 6973 696f  .        decisio
-00015380: 6e5f 7363 7220 3d20 2863 6f6c 6f72 5465  n_scr = (colorTe
-00015390: 7874 2e47 5245 454e 2069 6620 6973 5570  xt.GREEN if isUp
-000153a0: 7472 656e 6420 656c 7365 2028 636f 6c6f  trend else (colo
-000153b0: 7254 6578 742e 4641 494c 2069 6620 6973  rText.FAIL if is
-000153c0: 446f 776e 7472 656e 6420 656c 7365 2063  Downtrend else c
-000153d0: 6f6c 6f72 5465 7874 2e57 4152 4e29 2920  olorText.WARN)) 
-000153e0: 2b20 6622 7b64 6563 6973 696f 6e7d 2220  + f"{decision}" 
-000153f0: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-00015400: 2020 2020 2020 2020 646d 6135 3064 6563          dma50dec
-00015410: 6973 696f 6e5f 7363 7220 3d20 2863 6f6c  ision_scr = (col
-00015420: 6f72 5465 7874 2e47 5245 454e 2069 6620  orText.GREEN if 
-00015430: 6973 3530 444d 4155 7074 7265 6e64 2065  is50DMAUptrend e
-00015440: 6c73 6520 2863 6f6c 6f72 5465 7874 2e46  lse (colorText.F
-00015450: 4149 4c20 6966 2069 7335 3044 4d41 446f  AIL if is50DMADo
-00015460: 776e 7472 656e 6420 656c 7365 2063 6f6c  wntrend else col
-00015470: 6f72 5465 7874 2e57 4152 4e29 2920 2b20  orText.WARN)) + 
-00015480: 6622 7b64 6d61 3530 6465 6369 7369 6f6e  f"{dma50decision
-00015490: 7d22 202b 2063 6f6c 6f72 5465 7874 2e45  }" + colorText.E
-000154a0: 4e44 0a20 2020 2020 2020 2073 6176 6544  ND.        saveD
-000154b0: 6963 745b 2254 7265 6e64 225d 203d 2066  ict["Trend"] = f
-000154c0: 227b 7361 7665 645b 315d 7d20 7b64 6563  "{saved[1]} {dec
-000154d0: 6973 696f 6e7d 207b 646d 6135 3064 6563  ision} {dma50dec
-000154e0: 6973 696f 6e7d 207b 6d66 7d22 0a20 2020  ision} {mf}".   
-000154f0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00015500: 2254 7265 6e64 225d 203d 2066 227b 7361  "Trend"] = f"{sa
-00015510: 7665 645b 305d 7d20 7b64 6563 6973 696f  ved[0]} {decisio
-00015520: 6e5f 7363 727d 207b 646d 6135 3064 6563  n_scr} {dma50dec
-00015530: 6973 696f 6e5f 7363 727d 207b 6d66 737d  ision_scr} {mfs}
-00015540: 220a 2020 2020 2020 2020 7361 7665 4469  ".        saveDi
-00015550: 6374 5b22 4d46 4922 5d20 3d20 6d66 5f69  ct["MFI"] = mf_i
-00015560: 6e73 745f 6f77 6e65 7273 6869 7043 6861  nst_ownershipCha
-00015570: 6e67 650a 2020 2020 2020 2020 7363 7265  nge.        scre
-00015580: 656e 4469 6374 5b22 4d46 4922 5d20 3d20  enDict["MFI"] = 
-00015590: 6d66 5f69 6e73 745f 6f77 6e65 7273 6869  mf_inst_ownershi
-000155a0: 7043 6861 6e67 650a 2020 2020 2020 2020  pChange.        
-000155b0: 7265 7475 726e 2069 7355 7074 7265 6e64  return isUptrend
-000155c0: 2c20 6d66 5f69 6e73 745f 6f77 6e65 7273  , mf_inst_owners
-000155d0: 6869 7043 6861 6e67 652c 2066 6169 7256  hipChange, fairV
-000155e0: 616c 7565 4469 6666 0a20 2020 200a 2020  alueDiff.    .  
-000155f0: 2020 2320 5072 6976 6174 6520 6d65 7468    # Private meth
-00015600: 6f64 2074 6f20 6669 6e64 2063 616e 646c  od to find candl
-00015610: 6520 7479 7065 0a20 2020 2023 2054 7275  e type.    # Tru
-00015620: 6520 3d20 4275 6c6c 6973 682c 2046 616c  e = Bullish, Fal
-00015630: 7365 203d 2042 6561 7269 7368 0a20 2020  se = Bearish.   
-00015640: 2064 6566 2067 6574 4361 6e64 6c65 5479   def getCandleTy
-00015650: 7065 2873 656c 662c 2064 6169 6c79 4461  pe(self, dailyDa
-00015660: 7461 293a 0a20 2020 2020 2020 2072 6574  ta):.        ret
-00015670: 7572 6e20 626f 6f6c 2864 6169 6c79 4461  urn bool(dailyDa
-00015680: 7461 5b22 436c 6f73 6522 5d2e 696c 6f63  ta["Close"].iloc
-00015690: 5b30 5d20 3e3d 2064 6169 6c79 4461 7461  [0] >= dailyData
-000156a0: 5b22 4f70 656e 225d 2e69 6c6f 635b 305d  ["Open"].iloc[0]
-000156b0: 290a 0a20 2020 2064 6566 2067 6574 4361  )..    def getCa
-000156c0: 6e64 6c65 426f 6479 4865 6967 6874 2873  ndleBodyHeight(s
-000156d0: 656c 662c 2064 6169 6c79 4461 7461 293a  elf, dailyData):
-000156e0: 0a20 2020 2020 2020 2062 6f64 7948 6569  .        bodyHei
-000156f0: 6768 7420 3d20 6461 696c 7944 6174 615b  ght = dailyData[
-00015700: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
-00015710: 202d 2064 6169 6c79 4461 7461 5b22 4f70   - dailyData["Op
-00015720: 656e 225d 2e69 6c6f 635b 305d 0a20 2020  en"].iloc[0].   
-00015730: 2020 2020 2072 6574 7572 6e20 626f 6479       return body
-00015740: 4865 6967 6874 0a0a 2020 2020 6465 6620  Height..    def 
-00015750: 6765 7446 6169 7256 616c 7565 2873 656c  getFairValue(sel
-00015760: 662c 2073 746f 636b 2c20 686f 7374 4461  f, stock, hostDa
-00015770: 7461 3d4e 6f6e 652c 2066 6f72 6365 3d46  ta=None, force=F
-00015780: 616c 7365 2c65 7863 6861 6e67 654e 616d  alse,exchangeNam
-00015790: 653d 2249 4e44 4941 2229 3a0a 2020 2020  e="INDIA"):.    
-000157a0: 2020 2020 6966 2068 6f73 7444 6174 6120      if hostData 
-000157b0: 6973 204e 6f6e 6520 6f72 206c 656e 2868  is None or len(h
-000157c0: 6f73 7444 6174 6129 203c 2031 3a0a 2020  ostData) < 1:.  
-000157d0: 2020 2020 2020 2020 2020 686f 7374 4461            hostDa
-000157e0: 7461 203d 2070 642e 4461 7461 4672 616d  ta = pd.DataFram
-000157f0: 6528 290a 2020 2020 2020 2020 2320 4c65  e().        # Le
-00015800: 7427 7320 6c6f 6f6b 2066 6f72 2066 6169  t's look for fai
-00015810: 7220 7661 6c75 6573 0a20 2020 2020 2020  r values.       
-00015820: 2066 6169 7256 616c 7565 203d 2030 0a20   fairValue = 0. 
-00015830: 2020 2020 2020 2069 6620 2246 6169 7256         if "FairV
-00015840: 616c 7565 2220 696e 2068 6f73 7444 6174  alue" in hostDat
-00015850: 612e 636f 6c75 6d6e 7320 616e 6420 504b  a.columns and PK
-00015860: 4461 7465 5574 696c 6974 6965 732e 6375  DateUtilities.cu
-00015870: 7272 656e 7444 6174 6554 696d 6528 292e  rrentDateTime().
-00015880: 7765 656b 6461 7928 2920 3c3d 2034 3a0a  weekday() <= 4:.
-00015890: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000158a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000158b0: 2066 6169 7256 616c 7565 203d 2068 6f73   fairValue = hos
-000158c0: 7444 6174 612e 6c6f 635b 686f 7374 4461  tData.loc[hostDa
-000158d0: 7461 2e69 6e64 6578 5b2d 315d 2c22 4661  ta.index[-1],"Fa
-000158e0: 6972 5661 6c75 6522 5d0a 2020 2020 2020  irValue"].      
-000158f0: 2020 2020 2020 6578 6365 7074 2028 4b65        except (Ke
-00015900: 7945 7272 6f72 2c49 6e64 6578 4572 726f  yError,IndexErro
-00015910: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00015920: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-00015930: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00015940: 2020 2020 2020 2069 6620 504b 4461 7465         if PKDate
-00015950: 5574 696c 6974 6965 732e 6375 7272 656e  Utilities.curren
-00015960: 7444 6174 6554 696d 6528 292e 7765 656b  tDateTime().week
-00015970: 6461 7928 2920 3e3d 2035 206f 7220 666f  day() >= 5 or fo
-00015980: 7263 653a 0a20 2020 2020 2020 2020 2020  rce:.           
-00015990: 2020 2020 2073 6563 7572 6974 7920 3d20       security = 
-000159a0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-000159b0: 2020 2020 2023 2052 6566 7265 7368 2065       # Refresh e
-000159c0: 6163 6820 7361 7475 7264 6179 206f 7220  ach saturday or 
-000159d0: 7375 6e64 6179 206f 7220 7768 656e 206e  sunday or when n
-000159e0: 6f74 2066 6f75 6e64 2069 6e20 7361 7665  ot found in save
-000159f0: 6420 6461 7461 0a20 2020 2020 2020 2020  d data.         
-00015a00: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00015a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a20: 7769 7468 2053 7570 7072 6573 734f 7574  with SuppressOut
-00015a30: 7075 7428 7375 7070 7265 7373 5f73 7464  put(suppress_std
-00015a40: 6572 723d 5472 7565 2c20 7375 7070 7265  err=True, suppre
-00015a50: 7373 5f73 7464 6f75 743d 5472 7565 293a  ss_stdout=True):
-00015a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015a70: 2020 2020 2020 2020 2073 6563 7572 6974           securit
-00015a80: 7920 3d20 5374 6f63 6b28 7374 6f63 6b2c  y = Stock(stock,
-00015a90: 6578 6368 616e 6765 3d65 7863 6861 6e67  exchange=exchang
-00015aa0: 654e 616d 6529 0a20 2020 2020 2020 2020  eName).         
-00015ab0: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
-00015ac0: 6c75 6545 7272 6f72 3a20 2320 7072 6167  lueError: # prag
-00015ad0: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
-00015ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015af0: 2023 2057 6520 6469 6420 6e6f 7420 6669   # We did not fi
-00015b00: 6e64 2074 6865 2073 746f 636b 3f20 4974  nd the stock? It
-00015b10: 2773 206f 6b61 792e 204d 6f76 6520 6f6e  's okay. Move on
-00015b20: 2074 6f20 7468 6520 6e65 7874 206f 6e65   to the next one
-00015b30: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015b40: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-00015b50: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00015b60: 7420 2854 696d 656f 7574 4572 726f 722c  t (TimeoutError,
-00015b70: 2043 6f6e 6e65 6374 696f 6e45 7272 6f72   ConnectionError
-00015b80: 2920 6173 2065 3a0a 2020 2020 2020 2020  ) as e:.        
-00015b90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015ba0: 2e64 6566 6175 6c74 5f6c 6f67 6765 722e  .default_logger.
-00015bb0: 6465 6275 6728 652c 2065 7863 5f69 6e66  debug(e, exc_inf
-00015bc0: 6f3d 5472 7565 290a 2020 2020 2020 2020  o=True).        
-00015bd0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00015be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015bf0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00015c00: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
-00015c10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015c20: 2e64 6566 6175 6c74 5f6c 6f67 6765 722e  .default_logger.
-00015c30: 6465 6275 6728 652c 2065 7863 5f69 6e66  debug(e, exc_inf
-00015c40: 6f3d 5472 7565 290a 2020 2020 2020 2020  o=True).        
-00015c50: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00015c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015c70: 2069 6620 7365 6375 7269 7479 2069 7320   if security is 
-00015c80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00015c90: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00015ca0: 7468 2053 7570 7072 6573 734f 7574 7075  th SuppressOutpu
-00015cb0: 7428 7375 7070 7265 7373 5f73 7464 6572  t(suppress_stder
-00015cc0: 723d 5472 7565 2c20 7375 7070 7265 7373  r=True, suppress
-00015cd0: 5f73 7464 6f75 743d 5472 7565 293a 0a20  _stdout=True):. 
-00015ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cf0: 2020 2020 2020 2066 7620 3d20 7365 6375         fv = secu
-00015d00: 7269 7479 2e66 6169 7256 616c 7565 2829  rity.fairValue()
-00015d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015d20: 2020 2020 2069 6620 6676 2069 7320 6e6f       if fv is no
-00015d30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00015d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d50: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00015d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d70: 2066 7652 6573 706f 6e73 6556 616c 7565   fvResponseValue
-00015d80: 203d 2066 765b 226c 6174 6573 7446 6169   = fv["latestFai
-00015d90: 7256 616c 7565 225d 0a20 2020 2020 2020  rValue"].       
-00015da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015db0: 2020 2020 2069 6620 6676 5265 7370 6f6e       if fvRespon
-00015dc0: 7365 5661 6c75 6520 6973 206e 6f74 204e  seValue is not N
-00015dd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00015de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015df0: 2020 2020 2066 6169 7256 616c 7565 203d       fairValue =
-00015e00: 2066 6c6f 6174 2866 7652 6573 706f 6e73   float(fvRespons
-00015e10: 6556 616c 7565 290a 2020 2020 2020 2020  eValue).        
-00015e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e30: 6578 6365 7074 3a20 2320 7072 6167 6d61  except: # pragma
-00015e40: 3a20 6e6f 2063 6f76 6572 0a20 2020 2020  : no cover.     
-00015e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e60: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+00013b60: 6c6f 635b 305d 202d 2028 6e6f 775b 2253  loc[0] - (now["S
+00013b70: 7570 706f 7274 225d 2e69 6c6f 635b 305d  upport"].iloc[0]
+00013b80: 202a 2070 6572 6365 6e74 6167 6529 0a20   * percentage). 
+00013b90: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
+00013ba0: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
+00013bb0: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
+00013bc0: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
+00013bd0: 2250 6174 7465 726e 2229 0a20 2020 2020  "Pattern").     
+00013be0: 2020 2069 6620 6c69 6d69 745f 6c6f 7765     if limit_lowe
+00013bf0: 7220 3c20 6e6f 775b 2243 6c6f 7365 225d  r < now["Close"]
+00013c00: 2e69 6c6f 635b 305d 203c 206c 696d 6974  .iloc[0] < limit
+00013c10: 5f75 7070 6572 2061 6e64 2073 6c6f 7065  _upper and slope
+00013c20: 203e 2030 2e31 353a 0a20 2020 2020 2020   > 0.15:.       
+00013c30: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00013c40: 2250 6174 7465 726e 225d 203d 2028 0a20  "Pattern"] = (. 
+00013c50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013c60: 6176 6564 5b30 5d20 2b20 636f 6c6f 7254  aved[0] + colorT
+00013c70: 6578 742e 424f 4c44 202b 2063 6f6c 6f72  ext.BOLD + color
+00013c80: 5465 7874 2e47 5245 454e 202b 2022 5472  Text.GREEN + "Tr
+00013c90: 656e 646c 696e 652d 5375 7070 6f72 7422  endline-Support"
+00013ca0: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+00013cb0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00013cc0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+00013cd0: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+00013ce0: 2073 6176 6564 5b31 5d20 2b20 2254 7265   saved[1] + "Tre
+00013cf0: 6e64 6c69 6e65 2d53 7570 706f 7274 220a  ndline-Support".
+00013d00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013d10: 726e 2054 7275 650a 0a20 2020 2020 2020  rn True..       
+00013d20: 2022 2222 2050 6c6f 7473 2066 6f72 2064   """ Plots for d
+00013d30: 6562 7567 6769 6e67 0a20 2020 2020 2020  ebugging.       
+00013d40: 2069 6d70 6f72 7420 6d61 7470 6c6f 746c   import matplotl
+00013d50: 6962 2e70 7970 6c6f 7420 6173 2070 6c74  ib.pyplot as plt
+00013d60: 0a20 2020 2020 2020 2066 6967 2c20 6178  .        fig, ax
+00013d70: 3120 3d20 706c 742e 7375 6270 6c6f 7473  1 = plt.subplots
+00013d80: 2866 6967 7369 7a65 3d28 3135 2c31 3029  (figsize=(15,10)
+00013d90: 290a 2020 2020 2020 2020 636f 6c6f 7220  ).        color 
+00013da0: 3d20 2774 6162 3a67 7265 656e 270a 2020  = 'tab:green'.  
+00013db0: 2020 2020 2020 7864 6174 6520 3d20 5b78        xdate = [x
+00013dc0: 2e64 6174 6528 2920 666f 7220 7820 696e  .date() for x in
+00013dd0: 2064 6174 612e 696e 6465 785d 0a20 2020   data.index].   
+00013de0: 2020 2020 2061 7831 2e73 6574 5f78 6c61       ax1.set_xla
+00013df0: 6265 6c28 2744 6174 6527 2c20 636f 6c6f  bel('Date', colo
+00013e00: 723d 636f 6c6f 7229 0a20 2020 2020 2020  r=color).       
+00013e10: 2061 7831 2e70 6c6f 7428 7864 6174 652c   ax1.plot(xdate,
+00013e20: 2064 6174 612e 436c 6f73 652c 206c 6162   data.Close, lab
+00013e30: 656c 3d22 636c 6f73 6522 2c20 636f 6c6f  el="close", colo
+00013e40: 723d 636f 6c6f 7229 0a20 2020 2020 2020  r=color).       
+00013e50: 2061 7831 2e74 6963 6b5f 7061 7261 6d73   ax1.tick_params
+00013e60: 2861 7869 733d 2778 272c 206c 6162 656c  (axis='x', label
+00013e70: 636f 6c6f 723d 636f 6c6f 7229 0a0a 2020  color=color)..  
+00013e80: 2020 2020 2020 6178 3220 3d20 6178 312e        ax2 = ax1.
+00013e90: 7477 696e 7928 2920 2320 6178 3220 616e  twiny() # ax2 an
+00013ea0: 6420 6178 3120 7769 6c6c 2068 6176 6520  d ax1 will have 
+00013eb0: 636f 6d6d 6f6e 2079 2061 7869 7320 616e  common y axis an
+00013ec0: 6420 6469 6666 6572 656e 7420 7820 6178  d different x ax
+00013ed0: 6973 2c20 7477 696e 790a 2020 2020 2020  is, twiny.      
+00013ee0: 2020 6178 322e 706c 6f74 2864 6174 612e    ax2.plot(data.
+00013ef0: 4e75 6d62 6572 2c20 6461 7461 2e52 6573  Number, data.Res
+00013f00: 6973 7461 6e63 652c 206c 6162 656c 3d22  istance, label="
+00013f10: 5265 7322 290a 2020 2020 2020 2020 6178  Res").        ax
+00013f20: 322e 706c 6f74 2864 6174 612e 4e75 6d62  2.plot(data.Numb
+00013f30: 6572 2c20 6461 7461 2e53 7570 706f 7274  er, data.Support
+00013f40: 2c20 6c61 6265 6c3d 2253 7570 2229 0a0a  , label="Sup")..
+00013f50: 2020 2020 2020 2020 706c 742e 6c65 6765          plt.lege
+00013f60: 6e64 2829 0a20 2020 2020 2020 2070 6c74  nd().        plt
+00013f70: 2e67 7269 6428 290a 2020 2020 2020 2020  .grid().        
+00013f80: 706c 742e 7368 6f77 2829 0a20 2020 2020  plt.show().     
+00013f90: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00013fa0: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00013fb0: 2023 2040 6d65 6173 7572 655f 7469 6d65   # @measure_time
+00013fc0: 0a20 2020 2064 6566 2066 696e 6455 7074  .    def findUpt
+00013fd0: 7265 6e64 2873 656c 662c 2064 662c 2073  rend(self, df, s
+00013fe0: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+00013ff0: 6963 742c 2074 6573 7469 6e67 2c20 7374  ict, testing, st
+00014000: 6f63 6b2c 6f6e 6c79 4d46 3d46 616c 7365  ock,onlyMF=False
+00014010: 2c68 6f73 7444 6174 613d 4e6f 6e65 2c65  ,hostData=None,e
+00014020: 7863 6861 6e67 654e 616d 653d 2249 4e44  xchangeName="IND
+00014030: 4941 222c 7265 6672 6573 684d 4641 6e64  IA",refreshMFAnd
+00014040: 4656 3d54 7275 6529 3a0a 2020 2020 2020  FV=True):.      
+00014050: 2020 2320 7368 6f75 6c64 5072 6f63 6565    # shouldProcee
+00014060: 6420 3d20 5472 7565 0a20 2020 2020 2020  d = True.       
+00014070: 2069 7355 7074 7265 6e64 203d 2046 616c   isUptrend = Fal
+00014080: 7365 0a20 2020 2020 2020 2069 7344 6f77  se.        isDow
+00014090: 6e74 7265 6e64 203d 2046 616c 7365 0a20  ntrend = False. 
+000140a0: 2020 2020 2020 2069 7335 3044 4d41 5570         is50DMAUp
+000140b0: 7472 656e 6420 3d20 4661 6c73 650a 2020  trend = False.  
+000140c0: 2020 2020 2020 6973 3530 444d 4144 6f77        is50DMADow
+000140d0: 6e74 7265 6e64 203d 2046 616c 7365 0a20  ntrend = False. 
+000140e0: 2020 2020 2020 2064 6563 6973 696f 6e20         decision 
+000140f0: 3d20 2222 0a20 2020 2020 2020 2064 6d61  = "".        dma
+00014100: 3530 6465 6369 7369 6f6e 203d 2022 220a  50decision = "".
+00014110: 2020 2020 2020 2020 6661 6972 5661 6c75          fairValu
+00014120: 6520 3d20 300a 2020 2020 2020 2020 6661  e = 0.        fa
+00014130: 6972 5661 6c75 6544 6966 6620 3d20 300a  irValueDiff = 0.
+00014140: 2020 2020 2020 2020 2320 6966 2064 6620          # if df 
+00014150: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+00014160: 6629 203c 2032 3230 206f 7220 7465 7374  f) < 220 or test
+00014170: 696e 673a 0a20 2020 2020 2020 2023 2020  ing:.        #  
+00014180: 2020 2073 686f 756c 6450 726f 6365 6564     shouldProceed
+00014190: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+000141a0: 2069 6620 6466 2069 7320 6e6f 7420 4e6f   if df is not No
+000141b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000141c0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+000141d0: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
+000141e0: 6f70 7928 290a 2020 2020 2020 2020 2020  opy().          
+000141f0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00014200: 615b 3a3a 2d31 5d0a 2020 2020 2020 2020  a[::-1].        
+00014210: 2020 2020 2020 2020 746f 6461 795f 736d          today_sm
+00014220: 6120 3d20 706b 7461 6c69 622e 534d 4128  a = pktalib.SMA(
+00014230: 6461 7461 5b22 436c 6f73 6522 5d2c 2074  data["Close"], t
+00014240: 696d 6570 6572 696f 643d 3530 290a 2020  imeperiod=50).  
+00014250: 2020 2020 2020 2020 2020 2020 2020 736d                sm
+00014260: 615f 6d69 6e75 7339 203d 2070 6b74 616c  a_minus9 = pktal
+00014270: 6962 2e53 4d41 2864 6174 612e 6865 6164  ib.SMA(data.head
+00014280: 286c 656e 2864 6174 6129 2d39 295b 2243  (len(data)-9)["C
+00014290: 6c6f 7365 225d 2c20 7469 6d65 7065 7269  lose"], timeperi
+000142a0: 6f64 3d35 3029 0a20 2020 2020 2020 2020  od=50).         
+000142b0: 2020 2020 2020 2073 6d61 5f6d 696e 7573         sma_minus
+000142c0: 3134 203d 2070 6b74 616c 6962 2e53 4d41  14 = pktalib.SMA
+000142d0: 2864 6174 612e 6865 6164 286c 656e 2864  (data.head(len(d
+000142e0: 6174 6129 2d31 3429 5b22 436c 6f73 6522  ata)-14)["Close"
+000142f0: 5d2c 2074 696d 6570 6572 696f 643d 3530  ], timeperiod=50
+00014300: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014310: 2020 736d 615f 6d69 6e75 7332 3020 3d20    sma_minus20 = 
+00014320: 706b 7461 6c69 622e 534d 4128 6461 7461  pktalib.SMA(data
+00014330: 2e68 6561 6428 6c65 6e28 6461 7461 292d  .head(len(data)-
+00014340: 3230 295b 2243 6c6f 7365 225d 2c20 7469  20)["Close"], ti
+00014350: 6d65 7065 7269 6f64 3d35 3029 0a20 2020  meperiod=50).   
+00014360: 2020 2020 2020 2020 2020 2020 2074 6f64               tod
+00014370: 6179 5f6c 6d61 203d 2070 6b74 616c 6962  ay_lma = pktalib
+00014380: 2e53 4d41 2864 6174 615b 2243 6c6f 7365  .SMA(data["Close
+00014390: 225d 2c20 7469 6d65 7065 7269 6f64 3d32  "], timeperiod=2
+000143a0: 3030 290a 2020 2020 2020 2020 2020 2020  00).            
+000143b0: 2020 2020 6c6d 615f 6d69 6e75 7332 3020      lma_minus20 
+000143c0: 3d20 706b 7461 6c69 622e 534d 4128 6461  = pktalib.SMA(da
+000143d0: 7461 2e68 6561 6428 6c65 6e28 6461 7461  ta.head(len(data
+000143e0: 292d 3230 295b 2243 6c6f 7365 225d 2c20  )-20)["Close"], 
+000143f0: 7469 6d65 7065 7269 6f64 3d32 3030 290a  timeperiod=200).
+00014400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014410: 6c6d 615f 6d69 6e75 7338 3020 3d20 706b  lma_minus80 = pk
+00014420: 7461 6c69 622e 534d 4128 6461 7461 2e68  talib.SMA(data.h
+00014430: 6561 6428 6c65 6e28 6461 7461 292d 3830  ead(len(data)-80
+00014440: 295b 2243 6c6f 7365 225d 2c20 7469 6d65  )["Close"], time
+00014450: 7065 7269 6f64 3d32 3030 290a 2020 2020  period=200).    
+00014460: 2020 2020 2020 2020 2020 2020 6c6d 615f              lma_
+00014470: 6d69 6e75 7331 3030 203d 2070 6b74 616c  minus100 = pktal
+00014480: 6962 2e53 4d41 2864 6174 612e 6865 6164  ib.SMA(data.head
+00014490: 286c 656e 2864 6174 6129 2d31 3030 295b  (len(data)-100)[
+000144a0: 2243 6c6f 7365 225d 2c20 7469 6d65 7065  "Close"], timepe
+000144b0: 7269 6f64 3d32 3030 290a 2020 2020 2020  riod=200).      
+000144c0: 2020 2020 2020 2020 2020 746f 6461 795f            today_
+000144d0: 6c6d 6120 3d20 746f 6461 795f 6c6d 612e  lma = today_lma.
+000144e0: 696c 6f63 5b6c 656e 2874 6f64 6179 5f6c  iloc[len(today_l
+000144f0: 6d61 292d 315d 2069 6620 746f 6461 795f  ma)-1] if today_
+00014500: 6c6d 6120 6973 206e 6f74 204e 6f6e 6520  lma is not None 
+00014510: 656c 7365 2030 0a20 2020 2020 2020 2020  else 0.         
+00014520: 2020 2020 2020 206c 6d61 5f6d 696e 7573         lma_minus
+00014530: 3230 203d 206c 6d61 5f6d 696e 7573 3230  20 = lma_minus20
+00014540: 2e69 6c6f 635b 6c65 6e28 6c6d 615f 6d69  .iloc[len(lma_mi
+00014550: 6e75 7332 3029 2d31 5d20 6966 206c 6d61  nus20)-1] if lma
+00014560: 5f6d 696e 7573 3230 2069 7320 6e6f 7420  _minus20 is not 
+00014570: 4e6f 6e65 2065 6c73 6520 300a 2020 2020  None else 0.    
+00014580: 2020 2020 2020 2020 2020 2020 6c6d 615f              lma_
+00014590: 6d69 6e75 7338 3020 3d20 6c6d 615f 6d69  minus80 = lma_mi
+000145a0: 6e75 7338 302e 696c 6f63 5b6c 656e 286c  nus80.iloc[len(l
+000145b0: 6d61 5f6d 696e 7573 3830 292d 315d 2069  ma_minus80)-1] i
+000145c0: 6620 6c6d 615f 6d69 6e75 7338 3020 6973  f lma_minus80 is
+000145d0: 206e 6f74 204e 6f6e 6520 656c 7365 2030   not None else 0
+000145e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000145f0: 206c 6d61 5f6d 696e 7573 3130 3020 3d20   lma_minus100 = 
+00014600: 6c6d 615f 6d69 6e75 7331 3030 2e69 6c6f  lma_minus100.ilo
+00014610: 635b 6c65 6e28 6c6d 615f 6d69 6e75 7331  c[len(lma_minus1
+00014620: 3030 292d 315d 2069 6620 6c6d 615f 6d69  00)-1] if lma_mi
+00014630: 6e75 7331 3030 2069 7320 6e6f 7420 4e6f  nus100 is not No
+00014640: 6e65 2065 6c73 6520 300a 2020 2020 2020  ne else 0.      
+00014650: 2020 2020 2020 2020 2020 746f 6461 795f            today_
+00014660: 736d 6120 3d20 746f 6461 795f 736d 612e  sma = today_sma.
+00014670: 696c 6f63 5b6c 656e 2874 6f64 6179 5f73  iloc[len(today_s
+00014680: 6d61 292d 315d 2069 6620 746f 6461 795f  ma)-1] if today_
+00014690: 736d 6120 6973 206e 6f74 204e 6f6e 6520  sma is not None 
+000146a0: 656c 7365 2030 0a20 2020 2020 2020 2020  else 0.         
+000146b0: 2020 2020 2020 2073 6d61 5f6d 696e 7573         sma_minus
+000146c0: 3920 3d20 736d 615f 6d69 6e75 7339 2e69  9 = sma_minus9.i
+000146d0: 6c6f 635b 6c65 6e28 736d 615f 6d69 6e75  loc[len(sma_minu
+000146e0: 7339 292d 315d 2069 6620 736d 615f 6d69  s9)-1] if sma_mi
+000146f0: 6e75 7339 2069 7320 6e6f 7420 4e6f 6e65  nus9 is not None
+00014700: 2065 6c73 6520 300a 2020 2020 2020 2020   else 0.        
+00014710: 2020 2020 2020 2020 736d 615f 6d69 6e75          sma_minu
+00014720: 7331 3420 3d20 736d 615f 6d69 6e75 7331  s14 = sma_minus1
+00014730: 342e 696c 6f63 5b6c 656e 2873 6d61 5f6d  4.iloc[len(sma_m
+00014740: 696e 7573 3134 292d 315d 2069 6620 736d  inus14)-1] if sm
+00014750: 615f 6d69 6e75 7331 3420 6973 206e 6f74  a_minus14 is not
+00014760: 204e 6f6e 6520 656c 7365 2030 0a20 2020   None else 0.   
+00014770: 2020 2020 2020 2020 2020 2020 2073 6d61               sma
+00014780: 5f6d 696e 7573 3230 203d 2073 6d61 5f6d  _minus20 = sma_m
+00014790: 696e 7573 3230 2e69 6c6f 635b 6c65 6e28  inus20.iloc[len(
+000147a0: 736d 615f 6d69 6e75 7332 3029 2d31 5d20  sma_minus20)-1] 
+000147b0: 6966 2073 6d61 5f6d 696e 7573 3230 2069  if sma_minus20 i
+000147c0: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+000147d0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+000147e0: 2020 6973 5570 7472 656e 6420 3d20 2874    isUptrend = (t
+000147f0: 6f64 6179 5f6c 6d61 203e 206c 6d61 5f6d  oday_lma > lma_m
+00014800: 696e 7573 3230 2920 6f72 2028 746f 6461  inus20) or (toda
+00014810: 795f 6c6d 6120 3e20 6c6d 615f 6d69 6e75  y_lma > lma_minu
+00014820: 7338 3029 206f 7220 2874 6f64 6179 5f6c  s80) or (today_l
+00014830: 6d61 203e 206c 6d61 5f6d 696e 7573 3130  ma > lma_minus10
+00014840: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+00014850: 2020 2069 7344 6f77 6e74 7265 6e64 203d     isDowntrend =
+00014860: 2028 746f 6461 795f 6c6d 6120 3c20 6c6d   (today_lma < lm
+00014870: 615f 6d69 6e75 7332 3029 2061 6e64 2028  a_minus20) and (
+00014880: 746f 6461 795f 6c6d 6120 3c20 6c6d 615f  today_lma < lma_
+00014890: 6d69 6e75 7338 3029 2061 6e64 2028 746f  minus80) and (to
+000148a0: 6461 795f 6c6d 6120 3c20 6c6d 615f 6d69  day_lma < lma_mi
+000148b0: 6e75 7331 3030 290a 2020 2020 2020 2020  nus100).        
+000148c0: 2020 2020 2020 2020 6973 3530 444d 4155          is50DMAU
+000148d0: 7074 7265 6e64 203d 2028 746f 6461 795f  ptrend = (today_
+000148e0: 736d 6120 3e20 736d 615f 6d69 6e75 7339  sma > sma_minus9
+000148f0: 2920 6f72 2028 746f 6461 795f 736d 6120  ) or (today_sma 
+00014900: 3e20 736d 615f 6d69 6e75 7331 3429 206f  > sma_minus14) o
+00014910: 7220 2874 6f64 6179 5f73 6d61 203e 2073  r (today_sma > s
+00014920: 6d61 5f6d 696e 7573 3230 290a 2020 2020  ma_minus20).    
+00014930: 2020 2020 2020 2020 2020 2020 6973 3530              is50
+00014940: 444d 4144 6f77 6e74 7265 6e64 203d 2028  DMADowntrend = (
+00014950: 746f 6461 795f 736d 6120 3c20 736d 615f  today_sma < sma_
+00014960: 6d69 6e75 7339 2920 616e 6420 2874 6f64  minus9) and (tod
+00014970: 6179 5f73 6d61 203c 2073 6d61 5f6d 696e  ay_sma < sma_min
+00014980: 7573 3134 2920 616e 6420 2874 6f64 6179  us14) and (today
+00014990: 5f73 6d61 203c 2073 6d61 5f6d 696e 7573  _sma < sma_minus
+000149a0: 3230 290a 2020 2020 2020 2020 2020 2020  20).            
+000149b0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+000149c0: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+000149d0: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
+000149e0: 2020 2020 2020 2320 7365 6c66 2e64 6566        # self.def
+000149f0: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
+00014a00: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
+00014a10: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00014a20: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
+00014a30: 2064 6563 6973 696f 6e20 3d20 2754 3ae2   decision = 'T:.
+00014a40: 96b2 2720 6966 2069 7355 7074 7265 6e64  ..' if isUptrend
+00014a50: 2065 6c73 6520 2827 543a e296 bc27 2069   else ('T:...' i
+00014a60: 6620 6973 446f 776e 7472 656e 6420 656c  f isDowntrend el
+00014a70: 7365 2027 2729 0a20 2020 2020 2020 2064  se '').        d
+00014a80: 6d61 3530 6465 6369 7369 6f6e 203d 2027  ma50decision = '
+00014a90: 743a e296 b227 2069 6620 6973 3530 444d  t:...' if is50DM
+00014aa0: 4155 7074 7265 6e64 2065 6c73 6520 2827  AUptrend else ('
+00014ab0: 743a e296 bc27 2069 6620 6973 3530 444d  t:...' if is50DM
+00014ac0: 4144 6f77 6e74 7265 6e64 2065 6c73 6520  ADowntrend else 
+00014ad0: 2727 290a 2020 2020 2020 2020 6d66 5f69  '').        mf_i
+00014ae0: 6e73 745f 6f77 6e65 7273 6869 7043 6861  nst_ownershipCha
+00014af0: 6e67 6520 3d20 300a 2020 2020 2020 2020  nge = 0.        
+00014b00: 6368 616e 6765 5f6d 696c 6c69 6f6e 7320  change_millions 
+00014b10: 3d22 220a 2020 2020 2020 2020 6d66 203d  ="".        mf =
+00014b20: 2022 220a 2020 2020 2020 2020 6d66 7320   "".        mfs 
+00014b30: 3d20 2222 0a20 2020 2020 2020 2069 6620  = "".        if 
+00014b40: 7265 6672 6573 684d 4641 6e64 4656 3a0a  refreshMFAndFV:.
+00014b50: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00014b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014b70: 206d 665f 696e 7374 5f6f 776e 6572 7368   mf_inst_ownersh
+00014b80: 6970 4368 616e 6765 203d 2073 656c 662e  ipChange = self.
+00014b90: 6765 744d 7574 7561 6c46 756e 6453 7461  getMutualFundSta
+00014ba0: 7475 7328 7374 6f63 6b2c 6f6e 6c79 4d46  tus(stock,onlyMF
+00014bb0: 3d6f 6e6c 794d 462c 686f 7374 4461 7461  =onlyMF,hostData
+00014bc0: 3d68 6f73 7444 6174 612c 666f 7263 653d  =hostData,force=
+00014bd0: 2868 6f73 7444 6174 6120 6973 204e 6f6e  (hostData is Non
+00014be0: 6520 6f72 2068 6f73 7444 6174 612e 656d  e or hostData.em
+00014bf0: 7074 7920 6f72 206e 6f74 2028 224d 4622  pty or not ("MF"
+00014c00: 2069 6e20 686f 7374 4461 7461 2e63 6f6c   in hostData.col
+00014c10: 756d 6e73 206f 7220 2246 4949 2220 696e  umns or "FII" in
+00014c20: 2068 6f73 7444 6174 612e 636f 6c75 6d6e   hostData.column
+00014c30: 7329 292c 6578 6368 616e 6765 4e61 6d65  s)),exchangeName
+00014c40: 3d65 7863 6861 6e67 654e 616d 6529 0a20  =exchangeName). 
+00014c50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014c60: 6620 6973 696e 7374 616e 6365 286d 665f  f isinstance(mf_
+00014c70: 696e 7374 5f6f 776e 6572 7368 6970 4368  inst_ownershipCh
+00014c80: 616e 6765 2c20 7064 2e53 6572 6965 7329  ange, pd.Series)
+00014c90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014ca0: 2020 2020 2020 6d66 5f69 6e73 745f 6f77        mf_inst_ow
+00014cb0: 6e65 7273 6869 7043 6861 6e67 6520 3d20  nershipChange = 
+00014cc0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+00014cd0: 2020 726f 756e 644f 6666 203d 2032 0a20    roundOff = 2. 
+00014ce0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00014cf0: 696c 6c69 6f6e 7320 3d20 726f 756e 6428  illions = round(
+00014d00: 6d66 5f69 6e73 745f 6f77 6e65 7273 6869  mf_inst_ownershi
+00014d10: 7043 6861 6e67 652f 3130 3030 3030 302c  pChange/1000000,
+00014d20: 726f 756e 644f 6666 290a 2020 2020 2020  roundOff).      
+00014d30: 2020 2020 2020 2020 2020 7768 696c 6520            while 
+00014d40: 666c 6f61 7428 6d69 6c6c 696f 6e73 2920  float(millions) 
+00014d50: 3d3d 2030 2061 6e64 2072 6f75 6e64 4f66  == 0 and roundOf
+00014d60: 6620 3c3d 353a 0a20 2020 2020 2020 2020  f <=5:.         
+00014d70: 2020 2020 2020 2020 2020 2072 6f75 6e64             round
+00014d80: 4f66 6620 2b3d 310a 2020 2020 2020 2020  Off +=1.        
+00014d90: 2020 2020 2020 2020 2020 2020 6d69 6c6c              mill
+00014da0: 696f 6e73 203d 2072 6f75 6e64 286d 665f  ions = round(mf_
+00014db0: 696e 7374 5f6f 776e 6572 7368 6970 4368  inst_ownershipCh
+00014dc0: 616e 6765 2f31 3030 3030 3030 2c72 6f75  ange/1000000,rou
+00014dd0: 6e64 4f66 6629 0a20 2020 2020 2020 2020  ndOff).         
+00014de0: 2020 2020 2020 2063 6861 6e67 655f 6d69         change_mi
+00014df0: 6c6c 696f 6e73 203d 2066 2228 7b6d 696c  llions = f"({mil
+00014e00: 6c69 6f6e 737d 4d29 220a 2020 2020 2020  lions}M)".      
+00014e10: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00014e20: 6570 7469 6f6e 2061 7320 653a 2020 2320  eption as e:  # 
+00014e30: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+00014e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014e50: 2073 656c 662e 6465 6661 756c 745f 6c6f   self.default_lo
+00014e60: 6767 6572 2e64 6562 7567 2865 2c20 6578  gger.debug(e, ex
+00014e70: 635f 696e 666f 3d54 7275 6529 0a20 2020  c_info=True).   
+00014e80: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+00014e90: 730a 2020 2020 2020 2020 2020 2020 7472  s.            tr
+00014ea0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00014eb0: 2020 2023 4c65 7427 7320 6765 7420 7468     #Let's get th
+00014ec0: 6520 6661 6972 2076 616c 7565 2c20 6569  e fair value, ei
+00014ed0: 7468 6572 2073 6176 6564 206f 7220 6672  ther saved or fr
+00014ee0: 6573 6820 6672 6f6d 2073 6572 7669 6365  esh from service
+00014ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014f00: 2066 6169 7256 616c 7565 203d 2073 656c   fairValue = sel
+00014f10: 662e 6765 7446 6169 7256 616c 7565 2873  f.getFairValue(s
+00014f20: 746f 636b 2c68 6f73 7444 6174 612c 666f  tock,hostData,fo
+00014f30: 7263 653d 2868 6f73 7444 6174 6120 6973  rce=(hostData is
+00014f40: 204e 6f6e 6520 6f72 2068 6f73 7444 6174   None or hostDat
+00014f50: 612e 656d 7074 7920 6f72 2022 4661 6972  a.empty or "Fair
+00014f60: 5661 6c75 6522 206e 6f74 2069 6e20 686f  Value" not in ho
+00014f70: 7374 4461 7461 2e63 6f6c 756d 6e73 292c  stData.columns),
+00014f80: 6578 6368 616e 6765 4e61 6d65 3d65 7863  exchangeName=exc
+00014f90: 6861 6e67 654e 616d 6529 0a20 2020 2020  hangeName).     
+00014fa0: 2020 2020 2020 2020 2020 2069 6620 6661             if fa
+00014fb0: 6972 5661 6c75 6520 6973 206e 6f74 204e  irValue is not N
+00014fc0: 6f6e 6520 616e 6420 6661 6972 5661 6c75  one and fairValu
+00014fd0: 6520 213d 2030 3a0a 2020 2020 2020 2020  e != 0:.        
+00014fe0: 2020 2020 2020 2020 2020 2020 6c74 7020              ltp 
+00014ff0: 3d20 7361 7665 4469 6374 5b22 4c54 5022  = saveDict["LTP"
+00015000: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00015010: 2020 2020 2020 6661 6972 5661 6c75 6544        fairValueD
+00015020: 6966 6620 3d20 726f 756e 6428 6661 6972  iff = round(fair
+00015030: 5661 6c75 6520 2d20 6c74 702c 3029 0a20  Value - ltp,0). 
+00015040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015050: 2020 2073 6176 6544 6963 745b 2246 6169     saveDict["Fai
+00015060: 7256 616c 7565 225d 203d 2073 7472 2866  rValue"] = str(f
+00015070: 6169 7256 616c 7565 290a 2020 2020 2020  airValue).      
+00015080: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00015090: 7665 4469 6374 5b22 4656 4469 6666 225d  veDict["FVDiff"]
+000150a0: 203d 2066 6169 7256 616c 7565 4469 6666   = fairValueDiff
+000150b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000150c0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+000150d0: 2246 5644 6966 6622 5d20 3d20 6661 6972  "FVDiff"] = fair
+000150e0: 5661 6c75 6544 6966 660a 2020 2020 2020  ValueDiff.      
+000150f0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00015100: 7265 656e 4469 6374 5b22 4661 6972 5661  reenDict["FairVa
+00015110: 6c75 6522 5d20 3d20 2863 6f6c 6f72 5465  lue"] = (colorTe
+00015120: 7874 2e47 5245 454e 2069 6620 6661 6972  xt.GREEN if fair
+00015130: 5661 6c75 6520 3e3d 206c 7470 2065 6c73  Value >= ltp els
+00015140: 6520 636f 6c6f 7254 6578 742e 4641 494c  e colorText.FAIL
+00015150: 2920 2b20 7361 7665 4469 6374 5b22 4661  ) + saveDict["Fa
+00015160: 6972 5661 6c75 6522 5d20 2b20 636f 6c6f  irValue"] + colo
+00015170: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+00015180: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00015190: 6570 7469 6f6e 2061 7320 653a 2020 2320  eption as e:  # 
+000151a0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+000151b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000151c0: 2073 656c 662e 6465 6661 756c 745f 6c6f   self.default_lo
+000151d0: 6767 6572 2e64 6562 7567 2865 2c20 6578  gger.debug(e, ex
+000151e0: 635f 696e 666f 3d54 7275 6529 0a20 2020  c_info=True).   
+000151f0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+00015200: 730a 2020 2020 2020 2020 2020 2020 0a20  s.            . 
+00015210: 2020 2020 2020 2020 2020 2069 6620 6d66             if mf
+00015220: 5f69 6e73 745f 6f77 6e65 7273 6869 7043  _inst_ownershipC
+00015230: 6861 6e67 6520 3e20 303a 0a20 2020 2020  hange > 0:.     
+00015240: 2020 2020 2020 2020 2020 206d 6620 3d20             mf = 
+00015250: 6622 4d46 493a e296 b220 7b63 6861 6e67  f"MFI:... {chang
+00015260: 655f 6d69 6c6c 696f 6e73 7d22 0a20 2020  e_millions}".   
+00015270: 2020 2020 2020 2020 2020 2020 206d 6673               mfs
+00015280: 203d 2063 6f6c 6f72 5465 7874 2e47 5245   = colorText.GRE
+00015290: 454e 202b 206d 6620 2b20 636f 6c6f 7254  EN + mf + colorT
+000152a0: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+000152b0: 2020 2020 656c 6966 206d 665f 696e 7374      elif mf_inst
+000152c0: 5f6f 776e 6572 7368 6970 4368 616e 6765  _ownershipChange
+000152d0: 203c 2030 3a0a 2020 2020 2020 2020 2020   < 0:.          
+000152e0: 2020 2020 2020 6d66 203d 2066 224d 4649        mf = f"MFI
+000152f0: 3ae2 96bc 207b 6368 616e 6765 5f6d 696c  :... {change_mil
+00015300: 6c69 6f6e 737d 220a 2020 2020 2020 2020  lions}".        
+00015310: 2020 2020 2020 2020 6d66 7320 3d20 636f          mfs = co
+00015320: 6c6f 7254 6578 742e 4641 494c 202b 206d  lorText.FAIL + m
+00015330: 6620 2b20 636f 6c6f 7254 6578 742e 454e  f + colorText.EN
+00015340: 440a 0a20 2020 2020 2020 2073 6176 6564  D..        saved
+00015350: 203d 2073 656c 662e 6669 6e64 4375 7272   = self.findCurr
+00015360: 656e 7453 6176 6564 5661 6c75 6528 7363  entSavedValue(sc
+00015370: 7265 656e 4469 6374 2c73 6176 6544 6963  reenDict,saveDic
+00015380: 742c 2254 7265 6e64 2229 0a20 2020 2020  t,"Trend").     
+00015390: 2020 2064 6563 6973 696f 6e5f 7363 7220     decision_scr 
+000153a0: 3d20 2863 6f6c 6f72 5465 7874 2e47 5245  = (colorText.GRE
+000153b0: 454e 2069 6620 6973 5570 7472 656e 6420  EN if isUptrend 
+000153c0: 656c 7365 2028 636f 6c6f 7254 6578 742e  else (colorText.
+000153d0: 4641 494c 2069 6620 6973 446f 776e 7472  FAIL if isDowntr
+000153e0: 656e 6420 656c 7365 2063 6f6c 6f72 5465  end else colorTe
+000153f0: 7874 2e57 4152 4e29 2920 2b20 6622 7b64  xt.WARN)) + f"{d
+00015400: 6563 6973 696f 6e7d 2220 2b20 636f 6c6f  ecision}" + colo
+00015410: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+00015420: 2020 646d 6135 3064 6563 6973 696f 6e5f    dma50decision_
+00015430: 7363 7220 3d20 2863 6f6c 6f72 5465 7874  scr = (colorText
+00015440: 2e47 5245 454e 2069 6620 6973 3530 444d  .GREEN if is50DM
+00015450: 4155 7074 7265 6e64 2065 6c73 6520 2863  AUptrend else (c
+00015460: 6f6c 6f72 5465 7874 2e46 4149 4c20 6966  olorText.FAIL if
+00015470: 2069 7335 3044 4d41 446f 776e 7472 656e   is50DMADowntren
+00015480: 6420 656c 7365 2063 6f6c 6f72 5465 7874  d else colorText
+00015490: 2e57 4152 4e29 2920 2b20 6622 7b64 6d61  .WARN)) + f"{dma
+000154a0: 3530 6465 6369 7369 6f6e 7d22 202b 2063  50decision}" + c
+000154b0: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
+000154c0: 2020 2020 2073 6176 6544 6963 745b 2254       saveDict["T
+000154d0: 7265 6e64 225d 203d 2066 227b 7361 7665  rend"] = f"{save
+000154e0: 645b 315d 7d20 7b64 6563 6973 696f 6e7d  d[1]} {decision}
+000154f0: 207b 646d 6135 3064 6563 6973 696f 6e7d   {dma50decision}
+00015500: 207b 6d66 7d22 0a20 2020 2020 2020 2073   {mf}".        s
+00015510: 6372 6565 6e44 6963 745b 2254 7265 6e64  creenDict["Trend
+00015520: 225d 203d 2066 227b 7361 7665 645b 305d  "] = f"{saved[0]
+00015530: 7d20 7b64 6563 6973 696f 6e5f 7363 727d  } {decision_scr}
+00015540: 207b 646d 6135 3064 6563 6973 696f 6e5f   {dma50decision_
+00015550: 7363 727d 207b 6d66 737d 220a 2020 2020  scr} {mfs}".    
+00015560: 2020 2020 7361 7665 4469 6374 5b22 4d46      saveDict["MF
+00015570: 4922 5d20 3d20 6d66 5f69 6e73 745f 6f77  I"] = mf_inst_ow
+00015580: 6e65 7273 6869 7043 6861 6e67 650a 2020  nershipChange.  
+00015590: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+000155a0: 5b22 4d46 4922 5d20 3d20 6d66 5f69 6e73  ["MFI"] = mf_ins
+000155b0: 745f 6f77 6e65 7273 6869 7043 6861 6e67  t_ownershipChang
+000155c0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+000155d0: 2069 7355 7074 7265 6e64 2c20 6d66 5f69   isUptrend, mf_i
+000155e0: 6e73 745f 6f77 6e65 7273 6869 7043 6861  nst_ownershipCha
+000155f0: 6e67 652c 2066 6169 7256 616c 7565 4469  nge, fairValueDi
+00015600: 6666 0a20 2020 200a 2020 2020 2320 5072  ff.    .    # Pr
+00015610: 6976 6174 6520 6d65 7468 6f64 2074 6f20  ivate method to 
+00015620: 6669 6e64 2063 616e 646c 6520 7479 7065  find candle type
+00015630: 0a20 2020 2023 2054 7275 6520 3d20 4275  .    # True = Bu
+00015640: 6c6c 6973 682c 2046 616c 7365 203d 2042  llish, False = B
+00015650: 6561 7269 7368 0a20 2020 2064 6566 2067  earish.    def g
+00015660: 6574 4361 6e64 6c65 5479 7065 2873 656c  etCandleType(sel
+00015670: 662c 2064 6169 6c79 4461 7461 293a 0a20  f, dailyData):. 
+00015680: 2020 2020 2020 2072 6574 7572 6e20 626f         return bo
+00015690: 6f6c 2864 6169 6c79 4461 7461 5b22 436c  ol(dailyData["Cl
+000156a0: 6f73 6522 5d2e 696c 6f63 5b30 5d20 3e3d  ose"].iloc[0] >=
+000156b0: 2064 6169 6c79 4461 7461 5b22 4f70 656e   dailyData["Open
+000156c0: 225d 2e69 6c6f 635b 305d 290a 0a20 2020  "].iloc[0])..   
+000156d0: 2064 6566 2067 6574 4361 6e64 6c65 426f   def getCandleBo
+000156e0: 6479 4865 6967 6874 2873 656c 662c 2064  dyHeight(self, d
+000156f0: 6169 6c79 4461 7461 293a 0a20 2020 2020  ailyData):.     
+00015700: 2020 2062 6f64 7948 6569 6768 7420 3d20     bodyHeight = 
+00015710: 6461 696c 7944 6174 615b 2243 6c6f 7365  dailyData["Close
+00015720: 225d 2e69 6c6f 635b 305d 202d 2064 6169  "].iloc[0] - dai
+00015730: 6c79 4461 7461 5b22 4f70 656e 225d 2e69  lyData["Open"].i
+00015740: 6c6f 635b 305d 0a20 2020 2020 2020 2072  loc[0].        r
+00015750: 6574 7572 6e20 626f 6479 4865 6967 6874  eturn bodyHeight
+00015760: 0a0a 2020 2020 6465 6620 6765 7446 6169  ..    def getFai
+00015770: 7256 616c 7565 2873 656c 662c 2073 746f  rValue(self, sto
+00015780: 636b 2c20 686f 7374 4461 7461 3d4e 6f6e  ck, hostData=Non
+00015790: 652c 2066 6f72 6365 3d46 616c 7365 2c65  e, force=False,e
+000157a0: 7863 6861 6e67 654e 616d 653d 2249 4e44  xchangeName="IND
+000157b0: 4941 2229 3a0a 2020 2020 2020 2020 6966  IA"):.        if
+000157c0: 2068 6f73 7444 6174 6120 6973 204e 6f6e   hostData is Non
+000157d0: 6520 6f72 206c 656e 2868 6f73 7444 6174  e or len(hostDat
+000157e0: 6129 203c 2031 3a0a 2020 2020 2020 2020  a) < 1:.        
+000157f0: 2020 2020 686f 7374 4461 7461 203d 2070      hostData = p
+00015800: 642e 4461 7461 4672 616d 6528 290a 2020  d.DataFrame().  
+00015810: 2020 2020 2020 2320 4c65 7427 7320 6c6f        # Let's lo
+00015820: 6f6b 2066 6f72 2066 6169 7220 7661 6c75  ok for fair valu
+00015830: 6573 0a20 2020 2020 2020 2066 6169 7256  es.        fairV
+00015840: 616c 7565 203d 2030 0a20 2020 2020 2020  alue = 0.       
+00015850: 2069 6620 2246 6169 7256 616c 7565 2220   if "FairValue" 
+00015860: 696e 2068 6f73 7444 6174 612e 636f 6c75  in hostData.colu
+00015870: 6d6e 7320 616e 6420 504b 4461 7465 5574  mns and PKDateUt
+00015880: 696c 6974 6965 732e 6375 7272 656e 7444  ilities.currentD
+00015890: 6174 6554 696d 6528 292e 7765 656b 6461  ateTime().weekda
+000158a0: 7928 2920 3c3d 2034 3a0a 2020 2020 2020  y() <= 4:.      
+000158b0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+000158c0: 2020 2020 2020 2020 2020 2066 6169 7256             fairV
+000158d0: 616c 7565 203d 2068 6f73 7444 6174 612e  alue = hostData.
+000158e0: 6c6f 635b 686f 7374 4461 7461 2e69 6e64  loc[hostData.ind
+000158f0: 6578 5b2d 315d 2c22 4661 6972 5661 6c75  ex[-1],"FairValu
+00015900: 6522 5d0a 2020 2020 2020 2020 2020 2020  e"].            
+00015910: 6578 6365 7074 2028 4b65 7945 7272 6f72  except (KeyError
+00015920: 2c49 6e64 6578 4572 726f 7229 3a0a 2020  ,IndexError):.  
+00015930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015940: 2020 7061 7373 0a20 2020 2020 2020 2065    pass.        e
+00015950: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00015960: 2069 6620 504b 4461 7465 5574 696c 6974   if PKDateUtilit
+00015970: 6965 732e 6375 7272 656e 7444 6174 6554  ies.currentDateT
+00015980: 696d 6528 292e 7765 656b 6461 7928 2920  ime().weekday() 
+00015990: 3e3d 2035 206f 7220 666f 7263 653a 0a20  >= 5 or force:. 
+000159a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000159b0: 6563 7572 6974 7920 3d20 4e6f 6e65 0a20  ecurity = None. 
+000159c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000159d0: 2052 6566 7265 7368 2065 6163 6820 7361   Refresh each sa
+000159e0: 7475 7264 6179 206f 7220 7375 6e64 6179  turday or sunday
+000159f0: 206f 7220 7768 656e 206e 6f74 2066 6f75   or when not fou
+00015a00: 6e64 2069 6e20 7361 7665 6420 6461 7461  nd in saved data
+00015a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015a20: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00015a30: 2020 2020 2020 2020 2020 7769 7468 2053            with S
+00015a40: 7570 7072 6573 734f 7574 7075 7428 7375  uppressOutput(su
+00015a50: 7070 7265 7373 5f73 7464 6572 723d 5472  ppress_stderr=Tr
+00015a60: 7565 2c20 7375 7070 7265 7373 5f73 7464  ue, suppress_std
+00015a70: 6f75 743d 5472 7565 293a 0a20 2020 2020  out=True):.     
+00015a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a90: 2020 2073 6563 7572 6974 7920 3d20 5374     security = St
+00015aa0: 6f63 6b28 7374 6f63 6b2c 6578 6368 616e  ock(stock,exchan
+00015ab0: 6765 3d65 7863 6861 6e67 654e 616d 6529  ge=exchangeName)
+00015ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015ad0: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
+00015ae0: 6f72 3a20 2320 7072 6167 6d61 3a20 6e6f  or: # pragma: no
+00015af0: 2063 6f76 6572 0a20 2020 2020 2020 2020   cover.         
+00015b00: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
+00015b10: 6469 6420 6e6f 7420 6669 6e64 2074 6865  did not find the
+00015b20: 2073 746f 636b 3f20 4974 2773 206f 6b61   stock? It's oka
+00015b30: 792e 204d 6f76 6520 6f6e 2074 6f20 7468  y. Move on to th
+00015b40: 6520 6e65 7874 206f 6e65 2e0a 2020 2020  e next one..    
+00015b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b60: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+00015b70: 2020 2020 2065 7863 6570 7420 2854 696d       except (Tim
+00015b80: 656f 7574 4572 726f 722c 2043 6f6e 6e65  eoutError, Conne
+00015b90: 6374 696f 6e45 7272 6f72 2920 6173 2065  ctionError) as e
+00015ba0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015bb0: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
+00015bc0: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
+00015bd0: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
+00015be0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015bf0: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+00015c00: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00015c10: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00015c20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015c30: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
+00015c40: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
+00015c50: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
+00015c60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015c70: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+00015c80: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00015c90: 6375 7269 7479 2069 7320 6e6f 7420 4e6f  curity is not No
+00015ca0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00015cb0: 2020 2020 2020 2020 7769 7468 2053 7570          with Sup
+00015cc0: 7072 6573 734f 7574 7075 7428 7375 7070  pressOutput(supp
+00015cd0: 7265 7373 5f73 7464 6572 723d 5472 7565  ress_stderr=True
+00015ce0: 2c20 7375 7070 7265 7373 5f73 7464 6f75  , suppress_stdou
+00015cf0: 743d 5472 7565 293a 0a20 2020 2020 2020  t=True):.       
+00015d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d10: 2066 7620 3d20 7365 6375 7269 7479 2e66   fv = security.f
+00015d20: 6169 7256 616c 7565 2829 0a20 2020 2020  airValue().     
+00015d30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00015d40: 6620 6676 2069 7320 6e6f 7420 4e6f 6e65  f fv is not None
+00015d50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015d60: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00015d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d80: 2020 2020 2020 2020 2020 2066 7652 6573             fvRes
+00015d90: 706f 6e73 6556 616c 7565 203d 2066 765b  ponseValue = fv[
+00015da0: 226c 6174 6573 7446 6169 7256 616c 7565  "latestFairValue
+00015db0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00015dc0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00015dd0: 6620 6676 5265 7370 6f6e 7365 5661 6c75  f fvResponseValu
+00015de0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00015df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00015e10: 6169 7256 616c 7565 203d 2066 6c6f 6174  airValue = float
+00015e20: 2866 7652 6573 706f 6e73 6556 616c 7565  (fvResponseValue
+00015e30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015e40: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00015e50: 3a20 2320 7072 6167 6d61 3a20 6e6f 2063  : # pragma: no c
+00015e60: 6f76 6572 0a20 2020 2020 2020 2020 2020  over.           
 00015e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e80: 2020 2020 2020 2020 2320 7365 6c66 2e64          # self.d
-00015e90: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
-00015ea0: 6275 6728 6622 7b65 7d5c 6e52 6573 706f  bug(f"{e}\nRespo
-00015eb0: 6e73 653a 6676 3a5c 6e7b 6676 7d22 2c20  nse:fv:\n{fv}", 
-00015ec0: 6578 635f 696e 666f 3d54 7275 6529 0a20  exc_info=True). 
-00015ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ee0: 2020 2066 6169 7256 616c 7565 203d 2072     fairValue = r
-00015ef0: 6f75 6e64 2866 6c6f 6174 2866 6169 7256  ound(float(fairV
-00015f00: 616c 7565 292c 3129 0a20 2020 2020 2020  alue),1).       
-00015f10: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00015f20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015f30: 2020 2020 2020 2020 2020 686f 7374 4461            hostDa
-00015f40: 7461 2e6c 6f63 5b68 6f73 7444 6174 612e  ta.loc[hostData.
-00015f50: 696e 6465 785b 2d31 5d2c 2246 6169 7256  index[-1],"FairV
-00015f60: 616c 7565 225d 203d 2066 6169 7256 616c  alue"] = fairVal
-00015f70: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-00015f80: 2020 2020 2020 2065 7863 6570 7420 284b         except (K
-00015f90: 6579 4572 726f 722c 496e 6465 7845 7272  eyError,IndexErr
-00015fa0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-00015fb0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00015fc0: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-00015fd0: 2066 6169 7256 616c 7565 0a0a 2020 2020   fairValue..    
-00015fe0: 6465 6620 6765 744d 7574 7561 6c46 756e  def getMutualFun
-00015ff0: 6453 7461 7475 7328 7365 6c66 2c20 7374  dStatus(self, st
-00016000: 6f63 6b2c 6f6e 6c79 4d46 3d46 616c 7365  ock,onlyMF=False
-00016010: 2c20 686f 7374 4461 7461 3d4e 6f6e 652c  , hostData=None,
-00016020: 2066 6f72 6365 3d46 616c 7365 2c65 7863   force=False,exc
-00016030: 6861 6e67 654e 616d 653d 2249 4e44 4941  hangeName="INDIA
-00016040: 2229 3a0a 2020 2020 2020 2020 6966 2068  "):.        if h
-00016050: 6f73 7444 6174 6120 6973 204e 6f6e 6520  ostData is None 
-00016060: 6f72 206c 656e 2868 6f73 7444 6174 6129  or len(hostData)
-00016070: 203c 2031 3a0a 2020 2020 2020 2020 2020   < 1:.          
-00016080: 2020 686f 7374 4461 7461 203d 2070 642e    hostData = pd.
-00016090: 4461 7461 4672 616d 6528 290a 2020 2020  DataFrame().    
-000160a0: 2020 2020 0a20 2020 2020 2020 206e 6574      .        net
-000160b0: 4368 616e 6765 4d46 203d 2030 0a20 2020  ChangeMF = 0.   
-000160c0: 2020 2020 206e 6574 4368 616e 6765 496e       netChangeIn
-000160d0: 7374 203d 2030 0a20 2020 2020 2020 206c  st = 0.        l
-000160e0: 6174 6573 745f 6d66 6461 7465 203d 204e  atest_mfdate = N
-000160f0: 6f6e 650a 2020 2020 2020 2020 6c61 7465  one.        late
-00016100: 7374 5f69 6e73 7464 6174 6520 3d20 4e6f  st_instdate = No
-00016110: 6e65 0a20 2020 2020 2020 206e 6565 6473  ne.        needs
-00016120: 4672 6573 6855 7064 6174 6520 3d20 5472  FreshUpdate = Tr
-00016130: 7565 0a20 2020 2020 2020 206c 6173 7444  ue.        lastD
-00016140: 6179 4c61 7374 4d6f 6e74 6820 3d20 504b  ayLastMonth = PK
-00016150: 4461 7465 5574 696c 6974 6965 732e 6c61  DateUtilities.la
-00016160: 7374 5f64 6179 5f6f 665f 7072 6576 696f  st_day_of_previo
-00016170: 7573 5f6d 6f6e 7468 2850 4b44 6174 6555  us_month(PKDateU
-00016180: 7469 6c69 7469 6573 2e63 7572 7265 6e74  tilities.current
-00016190: 4461 7465 5469 6d65 2829 290a 2020 2020  DateTime()).    
-000161a0: 2020 2020 6966 2068 6f73 7444 6174 6120      if hostData 
-000161b0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-000161c0: 6c65 6e28 686f 7374 4461 7461 2920 3e20  len(hostData) > 
-000161d0: 303a 0a20 2020 2020 2020 2020 2020 2069  0:.            i
-000161e0: 6620 224d 4622 2069 6e20 686f 7374 4461  f "MF" in hostDa
-000161f0: 7461 2e63 6f6c 756d 6e73 206f 7220 2246  ta.columns or "F
-00016200: 4949 2220 696e 2068 6f73 7444 6174 612e  II" in hostData.
-00016210: 636f 6c75 6d6e 733a 0a20 2020 2020 2020  columns:.       
-00016220: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00016230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016240: 2020 6e65 7443 6861 6e67 654d 4620 3d20    netChangeMF = 
-00016250: 686f 7374 4461 7461 2e6c 6f63 5b68 6f73  hostData.loc[hos
-00016260: 7444 6174 612e 696e 6465 785b 2d31 5d2c  tData.index[-1],
-00016270: 224d 4622 5d0a 2020 2020 2020 2020 2020  "MF"].          
-00016280: 2020 2020 2020 6578 6365 7074 2028 4b65        except (Ke
-00016290: 7945 7272 6f72 2c49 6e64 6578 4572 726f  yError,IndexErro
-000162a0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-000162b0: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-000162c0: 2020 2020 2020 2020 2020 2020 2074 7279               try
-000162d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000162e0: 2020 2020 2020 6e65 7443 6861 6e67 6549        netChangeI
-000162f0: 6e73 7420 3d20 686f 7374 4461 7461 2e6c  nst = hostData.l
-00016300: 6f63 5b68 6f73 7444 6174 612e 696e 6465  oc[hostData.inde
-00016310: 785b 2d31 5d2c 2246 4949 225d 0a20 2020  x[-1],"FII"].   
-00016320: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00016330: 6570 7420 284b 6579 4572 726f 722c 496e  ept (KeyError,In
-00016340: 6465 7845 7272 6f72 293a 0a20 2020 2020  dexError):.     
-00016350: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00016360: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-00016370: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00016380: 2020 2020 2020 2020 2020 2020 206c 6174               lat
-00016390: 6573 745f 6d66 6461 7465 203d 2068 6f73  est_mfdate = hos
-000163a0: 7444 6174 612e 6c6f 635b 686f 7374 4461  tData.loc[hostDa
-000163b0: 7461 2e69 6e64 6578 5b2d 315d 2c22 4d46  ta.index[-1],"MF
-000163c0: 5f44 6174 6522 5d0a 2020 2020 2020 2020  _Date"].        
-000163d0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000163e0: 7369 6e73 7461 6e63 6528 6c61 7465 7374  sinstance(latest
-000163f0: 5f6d 6664 6174 652c 2066 6c6f 6174 293a  _mfdate, float):
-00016400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016410: 2020 2020 2020 2020 206c 6174 6573 745f           latest_
-00016420: 6d66 6461 7465 203d 2064 6174 6574 696d  mfdate = datetim
-00016430: 652e 6461 7465 7469 6d65 2e66 726f 6d74  e.datetime.fromt
-00016440: 696d 6573 7461 6d70 286c 6174 6573 745f  imestamp(latest_
-00016450: 6d66 6461 7465 292e 7374 7266 7469 6d65  mfdate).strftime
-00016460: 2827 2559 2d25 6d2d 2564 2729 0a20 2020  ('%Y-%m-%d').   
-00016470: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00016480: 6570 7420 284b 6579 4572 726f 722c 496e  ept (KeyError,In
-00016490: 6465 7845 7272 6f72 293a 0a20 2020 2020  dexError):.     
-000164a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000164b0: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-000164c0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000164d0: 2020 2020 2020 2020 2020 2020 206c 6174               lat
-000164e0: 6573 745f 696e 7374 6461 7465 203d 2068  est_instdate = h
-000164f0: 6f73 7444 6174 612e 6c6f 635b 686f 7374  ostData.loc[host
-00016500: 4461 7461 2e69 6e64 6578 5b2d 315d 2c22  Data.index[-1],"
-00016510: 4649 495f 4461 7465 225d 0a20 2020 2020  FII_Date"].     
-00016520: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016530: 6620 6973 696e 7374 616e 6365 286c 6174  f isinstance(lat
-00016540: 6573 745f 696e 7374 6461 7465 2c20 666c  est_instdate, fl
-00016550: 6f61 7429 3a0a 2020 2020 2020 2020 2020  oat):.          
-00016560: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00016570: 7465 7374 5f69 6e73 7464 6174 6520 3d20  test_instdate = 
-00016580: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
-00016590: 652e 6672 6f6d 7469 6d65 7374 616d 7028  e.fromtimestamp(
-000165a0: 6c61 7465 7374 5f69 6e73 7464 6174 6529  latest_instdate)
-000165b0: 2e73 7472 6674 696d 6528 2725 592d 256d  .strftime('%Y-%m
-000165c0: 2d25 6427 290a 2020 2020 2020 2020 2020  -%d').          
-000165d0: 2020 2020 2020 6578 6365 7074 2028 4b65        except (Ke
-000165e0: 7945 7272 6f72 2c49 6e64 6578 4572 726f  yError,IndexErro
-000165f0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00016600: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-00016610: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00016620: 6c61 7465 7374 5f6d 6664 6174 6520 6973  latest_mfdate is
-00016630: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00016640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016650: 6176 6564 5f6d 6664 6174 6520 3d20 504b  aved_mfdate = PK
-00016660: 4461 7465 5574 696c 6974 6965 732e 6461  DateUtilities.da
-00016670: 7465 4672 6f6d 596d 6453 7472 696e 6728  teFromYmdString(
-00016680: 6c61 7465 7374 5f6d 6664 6174 652e 7370  latest_mfdate.sp
-00016690: 6c69 7428 2254 2229 5b30 5d29 0a20 2020  lit("T")[0]).   
-000166a0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000166b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000166c0: 2020 2020 2020 2073 6176 6564 5f6d 6664         saved_mfd
-000166d0: 6174 6520 3d20 6c61 7374 4461 794c 6173  ate = lastDayLas
-000166e0: 744d 6f6e 7468 202d 2064 6174 6574 696d  tMonth - datetim
-000166f0: 652e 7469 6d65 6465 6c74 6128 3129 0a20  e.timedelta(1). 
-00016700: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016710: 6620 6c61 7465 7374 5f69 6e73 7464 6174  f latest_instdat
-00016720: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00016730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016740: 2020 2073 6176 6564 5f69 6e73 7464 6174     saved_instdat
-00016750: 6520 3d20 504b 4461 7465 5574 696c 6974  e = PKDateUtilit
-00016760: 6965 732e 6461 7465 4672 6f6d 596d 6453  ies.dateFromYmdS
-00016770: 7472 696e 6728 6c61 7465 7374 5f69 6e73  tring(latest_ins
-00016780: 7464 6174 652e 7370 6c69 7428 2254 2229  tdate.split("T")
-00016790: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-000167a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000167b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000167c0: 6176 6564 5f69 6e73 7464 6174 6520 3d20  aved_instdate = 
-000167d0: 6c61 7374 4461 794c 6173 744d 6f6e 7468  lastDayLastMonth
-000167e0: 202d 2064 6174 6574 696d 652e 7469 6d65   - datetime.time
-000167f0: 6465 6c74 6128 3129 0a20 2020 2020 2020  delta(1).       
-00016800: 2020 2020 2020 2020 2074 6f64 6179 203d           today =
-00016810: 2050 4b44 6174 6555 7469 6c69 7469 6573   PKDateUtilities
-00016820: 2e63 7572 7265 6e74 4461 7465 5469 6d65  .currentDateTime
-00016830: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00016840: 2020 206e 6565 6473 4672 6573 6855 7064     needsFreshUpd
-00016850: 6174 6520 3d20 2873 6176 6564 5f6d 6664  ate = (saved_mfd
-00016860: 6174 652e 6461 7465 2829 203c 206c 6173  ate.date() < las
-00016870: 7444 6179 4c61 7374 4d6f 6e74 682e 6461  tDayLastMonth.da
-00016880: 7465 2829 2920 616e 6420 2873 6176 6564  te()) and (saved
-00016890: 5f69 6e73 7464 6174 652e 6461 7465 2829  _instdate.date()
-000168a0: 203c 206c 6173 7444 6179 4c61 7374 4d6f   < lastDayLastMo
-000168b0: 6e74 682e 6461 7465 2829 290a 2020 2020  nth.date()).    
-000168c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000168d0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-000168e0: 6564 7346 7265 7368 5570 6461 7465 203d  edsFreshUpdate =
-000168f0: 2054 7275 650a 0a20 2020 2020 2020 2069   True..        i
-00016900: 6620 6e65 6564 7346 7265 7368 5570 6461  f needsFreshUpda
-00016910: 7465 2061 6e64 2066 6f72 6365 3a0a 2020  te and force:.  
-00016920: 2020 2020 2020 2020 2020 6e65 7443 6861            netCha
-00016930: 6e67 654d 462c 206e 6574 4368 616e 6765  ngeMF, netChange
-00016940: 496e 7374 2c20 6c61 7465 7374 5f6d 6664  Inst, latest_mfd
-00016950: 6174 652c 206c 6174 6573 745f 696e 7374  ate, latest_inst
-00016960: 6461 7465 203d 2073 656c 662e 6765 7446  date = self.getF
-00016970: 7265 7368 4d46 4953 7461 7475 7328 7374  reshMFIStatus(st
-00016980: 6f63 6b2c 6578 6368 616e 6765 4e61 6d65  ock,exchangeName
-00016990: 3d65 7863 6861 6e67 654e 616d 6529 0a20  =exchangeName). 
-000169a0: 2020 2020 2020 2020 2020 2069 6620 6e65             if ne
-000169b0: 7443 6861 6e67 654d 4620 6973 206e 6f74  tChangeMF is not
-000169c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000169d0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-000169e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169f0: 686f 7374 4461 7461 2e6c 6f63 5b68 6f73  hostData.loc[hos
-00016a00: 7444 6174 612e 696e 6465 785b 2d31 5d2c  tData.index[-1],
-00016a10: 224d 4622 5d20 3d20 6e65 7443 6861 6e67  "MF"] = netChang
-00016a20: 654d 460a 2020 2020 2020 2020 2020 2020  eMF.            
-00016a30: 2020 2020 6578 6365 7074 2028 4b65 7945      except (KeyE
-00016a40: 7272 6f72 2c49 6e64 6578 4572 726f 7229  rror,IndexError)
-00016a50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016a60: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-00016a70: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00016a80: 2020 2020 2020 2020 2020 2020 206e 6574               net
-00016a90: 4368 616e 6765 4d46 203d 2030 0a20 2020  ChangeMF = 0.   
-00016aa0: 2020 2020 2020 2020 2069 6620 6c61 7465           if late
-00016ab0: 7374 5f6d 6664 6174 6520 6973 206e 6f74  st_mfdate is not
-00016ac0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00016ad0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00016ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016af0: 686f 7374 4461 7461 2e6c 6f63 5b68 6f73  hostData.loc[hos
-00016b00: 7444 6174 612e 696e 6465 785b 2d31 5d2c  tData.index[-1],
-00016b10: 224d 465f 4461 7465 225d 203d 206c 6174  "MF_Date"] = lat
-00016b20: 6573 745f 6d66 6461 7465 0a20 2020 2020  est_mfdate.     
-00016b30: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00016b40: 7420 284b 6579 4572 726f 722c 496e 6465  t (KeyError,Inde
-00016b50: 7845 7272 6f72 293a 0a20 2020 2020 2020  xError):.       
-00016b60: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00016b70: 730a 2020 2020 2020 2020 2020 2020 6966  s.            if
-00016b80: 206e 6574 4368 616e 6765 496e 7374 2069   netChangeInst i
-00016b90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00016ba0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00016bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016bc0: 2020 2020 2068 6f73 7444 6174 612e 6c6f       hostData.lo
-00016bd0: 635b 686f 7374 4461 7461 2e69 6e64 6578  c[hostData.index
-00016be0: 5b2d 315d 2c22 4649 4922 5d20 3d20 6e65  [-1],"FII"] = ne
-00016bf0: 7443 6861 6e67 6549 6e73 740a 2020 2020  tChangeInst.    
-00016c00: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00016c10: 7074 2028 4b65 7945 7272 6f72 2c49 6e64  pt (KeyError,Ind
-00016c20: 6578 4572 726f 7229 3a0a 2020 2020 2020  exError):.      
-00016c30: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00016c40: 7373 0a20 2020 2020 2020 2020 2020 2065  ss.            e
-00016c50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00016c60: 2020 2020 206e 6574 4368 616e 6765 496e       netChangeIn
-00016c70: 7374 203d 2030 0a20 2020 2020 2020 2020  st = 0.         
-00016c80: 2020 2069 6620 6c61 7465 7374 5f69 6e73     if latest_ins
-00016c90: 7464 6174 6520 6973 206e 6f74 204e 6f6e  tdate is not Non
-00016ca0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00016cb0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00016cc0: 2020 2020 2020 2020 2020 2020 686f 7374              host
-00016cd0: 4461 7461 2e6c 6f63 5b68 6f73 7444 6174  Data.loc[hostDat
-00016ce0: 612e 696e 6465 785b 2d31 5d2c 2246 4949  a.index[-1],"FII
-00016cf0: 5f44 6174 6522 5d20 3d20 6c61 7465 7374  _Date"] = latest
-00016d00: 5f69 6e73 7464 6174 650a 2020 2020 2020  _instdate.      
-00016d10: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00016d20: 2028 4b65 7945 7272 6f72 2c49 6e64 6578   (KeyError,Index
-00016d30: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-00016d40: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00016d50: 0a20 2020 2020 2020 206c 6173 7444 6179  .        lastDay
-00016d60: 4c61 7374 4d6f 6e74 6820 3d20 6c61 7374  LastMonth = last
-00016d70: 4461 794c 6173 744d 6f6e 7468 2e73 7472  DayLastMonth.str
-00016d80: 6674 696d 6528 2225 592d 256d 2d25 6454  ftime("%Y-%m-%dT
-00016d90: 3030 3a30 303a 3030 2e30 3030 2229 0a20  00:00:00.000"). 
-00016da0: 2020 2020 2020 2069 6620 6f6e 6c79 4d46         if onlyMF
-00016db0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00016dc0: 7475 726e 206e 6574 4368 616e 6765 4d46  turn netChangeMF
-00016dd0: 0a20 2020 2020 2020 2069 6620 6c61 7465  .        if late
-00016de0: 7374 5f69 6e73 7464 6174 6520 3d3d 206c  st_instdate == l
-00016df0: 6174 6573 745f 6d66 6461 7465 3a0a 2020  atest_mfdate:.  
-00016e00: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00016e10: 2028 6e65 7443 6861 6e67 654d 4620 2b20   (netChangeMF + 
-00016e20: 6e65 7443 6861 6e67 6549 6e73 7429 0a20  netChangeInst). 
-00016e30: 2020 2020 2020 2065 6c69 6620 6c61 7465         elif late
-00016e40: 7374 5f6d 6664 6174 6520 3d3d 206c 6173  st_mfdate == las
-00016e50: 7444 6179 4c61 7374 4d6f 6e74 683a 0a20  tDayLastMonth:. 
-00016e60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00016e70: 6e20 6e65 7443 6861 6e67 654d 460a 2020  n netChangeMF.  
-00016e80: 2020 2020 2020 656c 6966 206c 6174 6573        elif lates
-00016e90: 745f 696e 7374 6461 7465 203d 3d20 6c61  t_instdate == la
-00016ea0: 7374 4461 794c 6173 744d 6f6e 7468 3a0a  stDayLastMonth:.
-00016eb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00016ec0: 726e 206e 6574 4368 616e 6765 496e 7374  rn netChangeInst
-00016ed0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00016ee0: 2020 2020 2020 2020 2020 2023 2066 696e             # fin
-00016ef0: 6420 7468 6520 6c61 7465 7374 2064 6174  d the latest dat
-00016f00: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
-00016f10: 206c 6174 6573 745f 6d66 6461 7465 2069   latest_mfdate i
-00016f20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00016f30: 2020 2020 2020 2020 2020 2020 6c61 7465              late
-00016f40: 7374 5f6d 6664 6174 6520 3d20 504b 4461  st_mfdate = PKDa
-00016f50: 7465 5574 696c 6974 6965 732e 6461 7465  teUtilities.date
-00016f60: 4672 6f6d 596d 6453 7472 696e 6728 6c61  FromYmdString(la
-00016f70: 7465 7374 5f6d 6664 6174 652e 7370 6c69  test_mfdate.spli
-00016f80: 7428 2254 2229 5b30 5d29 0a20 2020 2020  t("T")[0]).     
-00016f90: 2020 2020 2020 2069 6620 6c61 7465 7374         if latest
-00016fa0: 5f69 6e73 7464 6174 6520 6973 206e 6f74  _instdate is not
-00016fb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00016fc0: 2020 2020 2020 206c 6174 6573 745f 696e         latest_in
-00016fd0: 7374 6461 7465 203d 2050 4b44 6174 6555  stdate = PKDateU
-00016fe0: 7469 6c69 7469 6573 2e64 6174 6546 726f  tilities.dateFro
-00016ff0: 6d59 6d64 5374 7269 6e67 286c 6174 6573  mYmdString(lates
-00017000: 745f 696e 7374 6461 7465 2e73 706c 6974  t_instdate.split
-00017010: 2822 5422 295b 305d 290a 2020 2020 2020  ("T")[0]).      
-00017020: 2020 2020 2020 7265 7475 726e 206e 6574        return net
-00017030: 4368 616e 6765 4d46 2069 6620 2828 6c61  ChangeMF if ((la
-00017040: 7465 7374 5f6d 6664 6174 6520 6973 206e  test_mfdate is n
-00017050: 6f74 204e 6f6e 6529 2061 6e64 206c 6174  ot None) and lat
-00017060: 6573 745f 6d66 6461 7465 203e 2028 6c61  est_mfdate > (la
-00017070: 7465 7374 5f69 6e73 7464 6174 6520 6966  test_instdate if
-00017080: 206c 6174 6573 745f 696e 7374 6461 7465   latest_instdate
-00017090: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
-000170a0: 6520 286c 6174 6573 745f 6d66 6461 7465  e (latest_mfdate
-000170b0: 202d 2064 6174 6574 696d 652e 7469 6d65   - datetime.time
-000170c0: 6465 6c74 6128 3129 2929 2920 656c 7365  delta(1)))) else
-000170d0: 206e 6574 4368 616e 6765 496e 7374 0a0a   netChangeInst..
-000170e0: 2020 2020 6465 6620 6765 7446 7265 7368      def getFresh
-000170f0: 4d46 4953 7461 7475 7328 7365 6c66 2c20  MFIStatus(self, 
-00017100: 7374 6f63 6b2c 6578 6368 616e 6765 4e61  stock,exchangeNa
-00017110: 6d65 3d22 494e 4449 4122 293a 0a20 2020  me="INDIA"):.   
-00017120: 2020 2020 2063 6861 6e67 6553 7461 7475       changeStatu
-00017130: 7344 6174 614d 4620 3d20 4e6f 6e65 0a20  sDataMF = None. 
-00017140: 2020 2020 2020 2063 6861 6e67 6553 7461         changeSta
-00017150: 7475 7344 6174 6149 6e73 7420 3d20 4e6f  tusDataInst = No
-00017160: 6e65 0a20 2020 2020 2020 206e 6574 4368  ne.        netCh
-00017170: 616e 6765 4d46 203d 2030 0a20 2020 2020  angeMF = 0.     
-00017180: 2020 206e 6574 4368 616e 6765 496e 7374     netChangeInst
-00017190: 203d 2030 0a20 2020 2020 2020 206c 6174   = 0.        lat
-000171a0: 6573 745f 6d66 6461 7465 203d 204e 6f6e  est_mfdate = Non
-000171b0: 650a 2020 2020 2020 2020 6c61 7465 7374  e.        latest
-000171c0: 5f69 6e73 7464 6174 6520 3d20 4e6f 6e65  _instdate = None
-000171d0: 0a20 2020 2020 2020 2073 6563 7572 6974  .        securit
-000171e0: 7920 3d20 4e6f 6e65 0a20 2020 2020 2020  y = None.       
-000171f0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00017200: 2020 7769 7468 2053 7570 7072 6573 734f    with SuppressO
-00017210: 7574 7075 7428 7375 7070 7265 7373 5f73  utput(suppress_s
-00017220: 7464 6572 723d 5472 7565 2c20 7375 7070  tderr=True, supp
-00017230: 7265 7373 5f73 7464 6f75 743d 5472 7565  ress_stdout=True
-00017240: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00017250: 2020 2073 6563 7572 6974 7920 3d20 5374     security = St
-00017260: 6f63 6b28 7374 6f63 6b2c 6578 6368 616e  ock(stock,exchan
-00017270: 6765 3d65 7863 6861 6e67 654e 616d 6529  ge=exchangeName)
-00017280: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00017290: 5661 6c75 6545 7272 6f72 3a0a 2020 2020  ValueError:.    
-000172a0: 2020 2020 2020 2020 2320 5765 2064 6964          # We did
-000172b0: 206e 6f74 2066 696e 6420 7468 6520 7374   not find the st
-000172c0: 6f63 6b3f 2049 7427 7320 6f6b 6179 2e20  ock? It's okay. 
-000172d0: 4d6f 7665 206f 6e20 746f 2074 6865 206e  Move on to the n
-000172e0: 6578 7420 6f6e 652e 0a20 2020 2020 2020  ext one..       
-000172f0: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-00017300: 2020 6578 6365 7074 2028 5469 6d65 6f75    except (Timeou
-00017310: 7445 7272 6f72 2c20 436f 6e6e 6563 7469  tError, Connecti
-00017320: 6f6e 4572 726f 7229 2061 7320 653a 0a20  onError) as e:. 
-00017330: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017340: 6465 6661 756c 745f 6c6f 6767 6572 2e64  default_logger.d
-00017350: 6562 7567 2865 2c20 6578 635f 696e 666f  ebug(e, exc_info
-00017360: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00017370: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-00017380: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00017390: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-000173a0: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
-000173b0: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
-000173c0: 6578 635f 696e 666f 3d54 7275 6529 0a20  exc_info=True). 
-000173d0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-000173e0: 2020 2020 2020 2020 6966 2073 6563 7572          if secur
-000173f0: 6974 7920 6973 206e 6f74 204e 6f6e 653a  ity is not None:
-00017400: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-00017410: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017420: 2020 7769 7468 2053 7570 7072 6573 734f    with SuppressO
-00017430: 7574 7075 7428 7375 7070 7265 7373 5f73  utput(suppress_s
-00017440: 7464 6572 723d 5472 7565 2c20 7375 7070  tderr=True, supp
-00017450: 7265 7373 5f73 7464 6f75 743d 5472 7565  ress_stdout=True
-00017460: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00017470: 2020 2020 2020 2063 6861 6e67 6553 7461         changeSta
-00017480: 7475 7352 6f77 734d 4620 3d20 7365 6375  tusRowsMF = secu
-00017490: 7269 7479 2e6d 7574 7561 6c46 756e 644f  rity.mutualFundO
-000174a0: 776e 6572 7368 6970 2874 6f70 3d35 290a  wnership(top=5).
-000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174c0: 2020 2020 6368 616e 6765 5374 6174 7573      changeStatus
-000174d0: 526f 7773 496e 7374 203d 2073 6563 7572  RowsInst = secur
-000174e0: 6974 792e 696e 7374 6974 7574 696f 6e4f  ity.institutionO
-000174f0: 776e 6572 7368 6970 2874 6f70 3d35 290a  wnership(top=5).
-00017500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017510: 2020 2020 6368 616e 6765 5374 6174 7573      changeStatus
-00017520: 4461 7461 4d46 203d 2073 6563 7572 6974  DataMF = securit
-00017530: 792e 6d75 7475 616c 4675 6e64 4649 4943  y.mutualFundFIIC
-00017540: 6861 6e67 6544 6174 6128 6368 616e 6765  hangeData(change
-00017550: 5374 6174 7573 526f 7773 4d46 290a 2020  StatusRowsMF).  
-00017560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017570: 2020 6368 616e 6765 5374 6174 7573 4461    changeStatusDa
-00017580: 7461 496e 7374 203d 2073 6563 7572 6974  taInst = securit
-00017590: 792e 6d75 7475 616c 4675 6e64 4649 4943  y.mutualFundFIIC
-000175a0: 6861 6e67 6544 6174 6128 6368 616e 6765  hangeData(change
-000175b0: 5374 6174 7573 526f 7773 496e 7374 290a  StatusRowsInst).
-000175c0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-000175d0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-000175e0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000175f0: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
-00017600: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
-00017610: 6578 635f 696e 666f 3d54 7275 6529 0a20  exc_info=True). 
-00017620: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00017630: 2054 7970 6545 7272 6f72 206f 7220 436f   TypeError or Co
-00017640: 6e6e 6563 7469 6f6e 4572 726f 7220 6265  nnectionError be
-00017650: 6361 7573 6520 7765 2063 6f75 6c64 206e  cause we could n
-00017660: 6f74 2066 696e 6420 7468 6520 7374 6f63  ot find the stoc
-00017670: 6b20 6f72 204d 4649 2064 6174 6120 6973  k or MFI data is
-00017680: 6e27 7420 6176 6169 6c61 626c 653f 0a20  n't available?. 
-00017690: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000176a0: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-000176b0: 6c61 7374 4461 794c 6173 744d 6f6e 7468  lastDayLastMonth
-000176c0: 203d 2050 4b44 6174 6555 7469 6c69 7469   = PKDateUtiliti
-000176d0: 6573 2e6c 6173 745f 6461 795f 6f66 5f70  es.last_day_of_p
-000176e0: 7265 7669 6f75 735f 6d6f 6e74 6828 504b  revious_month(PK
-000176f0: 4461 7465 5574 696c 6974 6965 732e 6375  DateUtilities.cu
-00017700: 7272 656e 7444 6174 6554 696d 6528 2929  rrentDateTime())
-00017710: 0a20 2020 2020 2020 2020 2020 206c 6173  .            las
-00017720: 7444 6179 4c61 7374 4d6f 6e74 6820 3d20  tDayLastMonth = 
-00017730: 6c61 7374 4461 794c 6173 744d 6f6e 7468  lastDayLastMonth
-00017740: 2e73 7472 6674 696d 6528 2225 592d 256d  .strftime("%Y-%m
-00017750: 2d25 6454 3030 3a30 303a 3030 2e30 3030  -%dT00:00:00.000
-00017760: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
-00017770: 6620 6368 616e 6765 5374 6174 7573 4461  f changeStatusDa
-00017780: 7461 4d46 2069 7320 6e6f 7420 4e6f 6e65  taMF is not None
-00017790: 2061 6e64 206c 656e 2863 6861 6e67 6553   and len(changeS
-000177a0: 7461 7475 7344 6174 614d 4629 203e 2030  tatusDataMF) > 0
-000177b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000177c0: 2020 6466 5f67 726f 7570 6564 4d46 203d    df_groupedMF =
-000177d0: 2063 6861 6e67 6553 7461 7475 7344 6174   changeStatusDat
-000177e0: 614d 462e 6772 6f75 7062 7928 2264 6174  aMF.groupby("dat
-000177f0: 6522 2c20 736f 7274 3d46 616c 7365 290a  e", sort=False).
-00017800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017810: 666f 7220 6d66 6461 7465 2c20 6466 5f67  for mfdate, df_g
-00017820: 726f 7570 4d46 2069 6e20 6466 5f67 726f  roupMF in df_gro
-00017830: 7570 6564 4d46 3a0a 2020 2020 2020 2020  upedMF:.        
-00017840: 2020 2020 2020 2020 2020 2020 6e65 7443              netC
-00017850: 6861 6e67 654d 4620 3d20 6466 5f67 726f  hangeMF = df_gro
-00017860: 7570 4d46 5b22 6368 616e 6765 416d 6f75  upMF["changeAmou
-00017870: 6e74 225d 2e73 756d 2829 0a20 2020 2020  nt"].sum().     
-00017880: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00017890: 6174 6573 745f 6d66 6461 7465 203d 206d  atest_mfdate = m
-000178a0: 6664 6174 650a 2020 2020 2020 2020 2020  fdate.          
-000178b0: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-000178c0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-000178d0: 6861 6e67 6553 7461 7475 7344 6174 6149  hangeStatusDataI
-000178e0: 6e73 7420 6973 206e 6f74 204e 6f6e 6520  nst is not None 
-000178f0: 616e 6420 6c65 6e28 6368 616e 6765 5374  and len(changeSt
-00017900: 6174 7573 4461 7461 496e 7374 2920 3e20  atusDataInst) > 
-00017910: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-00017920: 2020 2064 665f 6772 6f75 7065 6449 6e73     df_groupedIns
-00017930: 7420 3d20 6368 616e 6765 5374 6174 7573  t = changeStatus
-00017940: 4461 7461 496e 7374 2e67 726f 7570 6279  DataInst.groupby
-00017950: 2822 6461 7465 222c 2073 6f72 743d 4661  ("date", sort=Fa
-00017960: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-00017970: 2020 2020 2066 6f72 2069 6e73 7464 6174       for instdat
-00017980: 652c 2064 665f 6772 6f75 7049 6e73 7420  e, df_groupInst 
-00017990: 696e 2064 665f 6772 6f75 7065 6449 6e73  in df_groupedIns
-000179a0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-000179b0: 2020 2020 2020 2069 6620 286c 6174 6573         if (lates
-000179c0: 745f 6d66 6461 7465 2069 7320 6e6f 7420  t_mfdate is not 
-000179d0: 4e6f 6e65 2061 6e64 206c 6174 6573 745f  None and latest_
-000179e0: 6d66 6461 7465 203d 3d20 696e 7374 6461  mfdate == instda
-000179f0: 7465 2920 6f72 2028 6c61 7465 7374 5f6d  te) or (latest_m
-00017a00: 6664 6174 6520 6973 204e 6f6e 6529 206f  fdate is None) o
-00017a10: 7220 2869 6e73 7464 6174 6520 3d3d 206c  r (instdate == l
-00017a20: 6173 7444 6179 4c61 7374 4d6f 6e74 6829  astDayLastMonth)
-00017a30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017a40: 2020 2020 2020 2020 2020 6e65 7443 6861            netCha
-00017a50: 6e67 6549 6e73 7420 3d20 6466 5f67 726f  ngeInst = df_gro
-00017a60: 7570 496e 7374 5b22 6368 616e 6765 416d  upInst["changeAm
-00017a70: 6f75 6e74 225d 2e73 756d 2829 0a20 2020  ount"].sum().   
-00017a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a90: 2020 2020 206c 6174 6573 745f 696e 7374       latest_inst
-00017aa0: 6461 7465 203d 2069 6e73 7464 6174 650a  date = instdate.
-00017ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ac0: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-00017ad0: 2020 7265 7475 726e 206e 6574 4368 616e    return netChan
-00017ae0: 6765 4d46 2c6e 6574 4368 616e 6765 496e  geMF,netChangeIn
-00017af0: 7374 2c6c 6174 6573 745f 6d66 6461 7465  st,latest_mfdate
-00017b00: 2c6c 6174 6573 745f 696e 7374 6461 7465  ,latest_instdate
-00017b10: 0a0a 0a20 2020 2064 6566 2067 6574 4e69  ...    def getNi
-00017b20: 6674 7950 7265 6469 6374 696f 6e28 7365  ftyPrediction(se
-00017b30: 6c66 2c20 6466 293a 0a20 2020 2020 2020  lf, df):.       
-00017b40: 2069 6d70 6f72 7420 7761 726e 696e 6773   import warnings
-00017b50: 0a0a 2020 2020 2020 2020 7761 726e 696e  ..        warnin
-00017b60: 6773 2e66 696c 7465 7277 6172 6e69 6e67  gs.filterwarning
-00017b70: 7328 2269 676e 6f72 6522 290a 2020 2020  s("ignore").    
-00017b80: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
-00017b90: 7079 2829 0a20 2020 2020 2020 206d 6f64  py().        mod
-00017ba0: 656c 2c20 706b 6c20 3d20 5574 696c 6974  el, pkl = Utilit
-00017bb0: 792e 746f 6f6c 732e 6765 744e 6966 7479  y.tools.getNifty
-00017bc0: 4d6f 6465 6c28 290a 2020 2020 2020 2020  Model().        
-00017bd0: 6966 206d 6f64 656c 2069 7320 4e6f 6e65  if model is None
-00017be0: 206f 7220 706b 6c20 6973 204e 6f6e 653a   or pkl is None:
-00017bf0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00017c00: 7572 6e20 302c 2022 556e 6b6e 6f77 6e22  urn 0, "Unknown"
-00017c10: 2c20 2255 6e6b 6e6f 776e 220a 2020 2020  , "Unknown".    
-00017c20: 2020 2020 7769 7468 2053 7570 7072 6573      with Suppres
-00017c30: 734f 7574 7075 7428 7375 7070 7265 7373  sOutput(suppress
-00017c40: 5f73 7464 6572 723d 5472 7565 2c20 7375  _stderr=True, su
-00017c50: 7070 7265 7373 5f73 7464 6f75 743d 5472  ppress_stdout=Tr
-00017c60: 7565 293a 0a20 2020 2020 2020 2020 2020  ue):.           
-00017c70: 2064 6174 6120 3d20 6461 7461 5b70 6b6c   data = data[pkl
-00017c80: 5b22 636f 6c75 6d6e 7322 5d5d 0a20 2020  ["columns"]].   
-00017c90: 2020 2020 2020 2020 2023 2323 2076 3220           ### v2 
-00017ca0: 5072 6570 726f 6365 7373 696e 670a 2020  Preprocessing.  
-00017cb0: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
-00017cc0: 4869 6768 225d 203d 2064 6174 615b 2248  High"] = data["H
-00017cd0: 6967 6822 5d2e 7063 745f 6368 616e 6765  igh"].pct_change
-00017ce0: 2829 202a 2031 3030 0a20 2020 2020 2020  () * 100.       
-00017cf0: 2020 2020 2064 6174 615b 224c 6f77 225d       data["Low"]
-00017d00: 203d 2064 6174 615b 224c 6f77 225d 2e70   = data["Low"].p
-00017d10: 6374 5f63 6861 6e67 6528 2920 2a20 3130  ct_change() * 10
-00017d20: 300a 2020 2020 2020 2020 2020 2020 6461  0.            da
-00017d30: 7461 5b22 4f70 656e 225d 203d 2064 6174  ta["Open"] = dat
-00017d40: 615b 224f 7065 6e22 5d2e 7063 745f 6368  a["Open"].pct_ch
-00017d50: 616e 6765 2829 202a 2031 3030 0a20 2020  ange() * 100.   
-00017d60: 2020 2020 2020 2020 2064 6174 615b 2243           data["C
-00017d70: 6c6f 7365 225d 203d 2064 6174 615b 2243  lose"] = data["C
-00017d80: 6c6f 7365 225d 2e70 6374 5f63 6861 6e67  lose"].pct_chang
-00017d90: 6528 2920 2a20 3130 300a 2020 2020 2020  e() * 100.      
-00017da0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00017db0: 612e 696c 6f63 5b2d 315d 0a20 2020 2020  a.iloc[-1].     
-00017dc0: 2020 2020 2020 2023 2323 0a20 2020 2020         ###.     
-00017dd0: 2020 2020 2020 2064 6174 6120 3d20 706b         data = pk
-00017de0: 6c5b 2273 6361 6c65 7222 5d2e 7472 616e  l["scaler"].tran
-00017df0: 7366 6f72 6d28 5b64 6174 615d 290a 2020  sform([data]).  
-00017e00: 2020 2020 2020 2020 2020 7769 7468 2053            with S
-00017e10: 7570 7072 6573 734f 7574 7075 7428 7375  uppressOutput(su
-00017e20: 7070 7265 7373 5f73 7464 6f75 743d 5472  ppress_stdout=Tr
-00017e30: 7565 2c20 7375 7070 7265 7373 5f73 7464  ue, suppress_std
-00017e40: 6572 723d 5472 7565 293a 0a20 2020 2020  err=True):.     
-00017e50: 2020 2020 2020 2020 2020 2070 7265 6420             pred 
-00017e60: 3d20 6d6f 6465 6c2e 7072 6564 6963 7428  = model.predict(
-00017e70: 6461 7461 295b 305d 0a20 2020 2020 2020  data)[0].       
-00017e80: 2069 6620 7072 6564 203e 2030 2e35 3a0a   if pred > 0.5:.
-00017e90: 2020 2020 2020 2020 2020 2020 6f75 7454              outT
-00017ea0: 6578 7420 3d20 2242 4541 5249 5348 220a  ext = "BEARISH".
-00017eb0: 2020 2020 2020 2020 2020 2020 6f75 7420              out 
-00017ec0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00017ed0: 2020 2020 636f 6c6f 7254 6578 742e 424f      colorText.BO
-00017ee0: 4c44 0a20 2020 2020 2020 2020 2020 2020  LD.             
-00017ef0: 2020 202b 2063 6f6c 6f72 5465 7874 2e46     + colorText.F
-00017f00: 4149 4c0a 2020 2020 2020 2020 2020 2020  AIL.            
-00017f10: 2020 2020 2b20 6f75 7454 6578 740a 2020      + outText.  
+00015e80: 2070 6173 730a 2020 2020 2020 2020 2020   pass.          
+00015e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ea0: 2020 2320 7365 6c66 2e64 6566 6175 6c74    # self.default
+00015eb0: 5f6c 6f67 6765 722e 6465 6275 6728 6622  _logger.debug(f"
+00015ec0: 7b65 7d5c 6e52 6573 706f 6e73 653a 6676  {e}\nResponse:fv
+00015ed0: 3a5c 6e7b 6676 7d22 2c20 6578 635f 696e  :\n{fv}", exc_in
+00015ee0: 666f 3d54 7275 6529 0a20 2020 2020 2020  fo=True).       
+00015ef0: 2020 2020 2020 2020 2020 2020 2066 6169               fai
+00015f00: 7256 616c 7565 203d 2072 6f75 6e64 2866  rValue = round(f
+00015f10: 6c6f 6174 2866 6169 7256 616c 7565 292c  loat(fairValue),
+00015f20: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
+00015f30: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00015f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f50: 2020 2020 686f 7374 4461 7461 2e6c 6f63      hostData.loc
+00015f60: 5b68 6f73 7444 6174 612e 696e 6465 785b  [hostData.index[
+00015f70: 2d31 5d2c 2246 6169 7256 616c 7565 225d  -1],"FairValue"]
+00015f80: 203d 2066 6169 7256 616c 7565 0a20 2020   = fairValue.   
+00015f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015fa0: 2065 7863 6570 7420 284b 6579 4572 726f   except (KeyErro
+00015fb0: 722c 496e 6465 7845 7272 6f72 293a 0a20  r,IndexError):. 
+00015fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015fd0: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+00015fe0: 2020 2020 7265 7475 726e 2066 6169 7256      return fairV
+00015ff0: 616c 7565 0a0a 2020 2020 6465 6620 6765  alue..    def ge
+00016000: 744d 7574 7561 6c46 756e 6453 7461 7475  tMutualFundStatu
+00016010: 7328 7365 6c66 2c20 7374 6f63 6b2c 6f6e  s(self, stock,on
+00016020: 6c79 4d46 3d46 616c 7365 2c20 686f 7374  lyMF=False, host
+00016030: 4461 7461 3d4e 6f6e 652c 2066 6f72 6365  Data=None, force
+00016040: 3d46 616c 7365 2c65 7863 6861 6e67 654e  =False,exchangeN
+00016050: 616d 653d 2249 4e44 4941 2229 3a0a 2020  ame="INDIA"):.  
+00016060: 2020 2020 2020 6966 2068 6f73 7444 6174        if hostDat
+00016070: 6120 6973 204e 6f6e 6520 6f72 206c 656e  a is None or len
+00016080: 2868 6f73 7444 6174 6129 203c 2031 3a0a  (hostData) < 1:.
+00016090: 2020 2020 2020 2020 2020 2020 686f 7374              host
+000160a0: 4461 7461 203d 2070 642e 4461 7461 4672  Data = pd.DataFr
+000160b0: 616d 6528 290a 2020 2020 2020 2020 0a20  ame().        . 
+000160c0: 2020 2020 2020 206e 6574 4368 616e 6765         netChange
+000160d0: 4d46 203d 2030 0a20 2020 2020 2020 206e  MF = 0.        n
+000160e0: 6574 4368 616e 6765 496e 7374 203d 2030  etChangeInst = 0
+000160f0: 0a20 2020 2020 2020 206c 6174 6573 745f  .        latest_
+00016100: 6d66 6461 7465 203d 204e 6f6e 650a 2020  mfdate = None.  
+00016110: 2020 2020 2020 6c61 7465 7374 5f69 6e73        latest_ins
+00016120: 7464 6174 6520 3d20 4e6f 6e65 0a20 2020  tdate = None.   
+00016130: 2020 2020 206e 6565 6473 4672 6573 6855       needsFreshU
+00016140: 7064 6174 6520 3d20 5472 7565 0a20 2020  pdate = True.   
+00016150: 2020 2020 206c 6173 7444 6179 4c61 7374       lastDayLast
+00016160: 4d6f 6e74 6820 3d20 504b 4461 7465 5574  Month = PKDateUt
+00016170: 696c 6974 6965 732e 6c61 7374 5f64 6179  ilities.last_day
+00016180: 5f6f 665f 7072 6576 696f 7573 5f6d 6f6e  _of_previous_mon
+00016190: 7468 2850 4b44 6174 6555 7469 6c69 7469  th(PKDateUtiliti
+000161a0: 6573 2e63 7572 7265 6e74 4461 7465 5469  es.currentDateTi
+000161b0: 6d65 2829 290a 2020 2020 2020 2020 6966  me()).        if
+000161c0: 2068 6f73 7444 6174 6120 6973 206e 6f74   hostData is not
+000161d0: 204e 6f6e 6520 616e 6420 6c65 6e28 686f   None and len(ho
+000161e0: 7374 4461 7461 2920 3e20 303a 0a20 2020  stData) > 0:.   
+000161f0: 2020 2020 2020 2020 2069 6620 224d 4622           if "MF"
+00016200: 2069 6e20 686f 7374 4461 7461 2e63 6f6c   in hostData.col
+00016210: 756d 6e73 206f 7220 2246 4949 2220 696e  umns or "FII" in
+00016220: 2068 6f73 7444 6174 612e 636f 6c75 6d6e   hostData.column
+00016230: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00016240: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00016250: 2020 2020 2020 2020 2020 2020 6e65 7443              netC
+00016260: 6861 6e67 654d 4620 3d20 686f 7374 4461  hangeMF = hostDa
+00016270: 7461 2e6c 6f63 5b68 6f73 7444 6174 612e  ta.loc[hostData.
+00016280: 696e 6465 785b 2d31 5d2c 224d 4622 5d0a  index[-1],"MF"].
+00016290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162a0: 6578 6365 7074 2028 4b65 7945 7272 6f72  except (KeyError
+000162b0: 2c49 6e64 6578 4572 726f 7229 3a0a 2020  ,IndexError):.  
+000162c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162d0: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
+000162e0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+000162f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016300: 6e65 7443 6861 6e67 6549 6e73 7420 3d20  netChangeInst = 
+00016310: 686f 7374 4461 7461 2e6c 6f63 5b68 6f73  hostData.loc[hos
+00016320: 7444 6174 612e 696e 6465 785b 2d31 5d2c  tData.index[-1],
+00016330: 2246 4949 225d 0a20 2020 2020 2020 2020  "FII"].         
+00016340: 2020 2020 2020 2065 7863 6570 7420 284b         except (K
+00016350: 6579 4572 726f 722c 496e 6465 7845 7272  eyError,IndexErr
+00016360: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+00016370: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+00016380: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00016390: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+000163a0: 2020 2020 2020 206c 6174 6573 745f 6d66         latest_mf
+000163b0: 6461 7465 203d 2068 6f73 7444 6174 612e  date = hostData.
+000163c0: 6c6f 635b 686f 7374 4461 7461 2e69 6e64  loc[hostData.ind
+000163d0: 6578 5b2d 315d 2c22 4d46 5f44 6174 6522  ex[-1],"MF_Date"
+000163e0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000163f0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00016400: 6e63 6528 6c61 7465 7374 5f6d 6664 6174  nce(latest_mfdat
+00016410: 652c 2066 6c6f 6174 293a 0a20 2020 2020  e, float):.     
+00016420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016430: 2020 206c 6174 6573 745f 6d66 6461 7465     latest_mfdate
+00016440: 203d 2064 6174 6574 696d 652e 6461 7465   = datetime.date
+00016450: 7469 6d65 2e66 726f 6d74 696d 6573 7461  time.fromtimesta
+00016460: 6d70 286c 6174 6573 745f 6d66 6461 7465  mp(latest_mfdate
+00016470: 292e 7374 7266 7469 6d65 2827 2559 2d25  ).strftime('%Y-%
+00016480: 6d2d 2564 2729 0a20 2020 2020 2020 2020  m-%d').         
+00016490: 2020 2020 2020 2065 7863 6570 7420 284b         except (K
+000164a0: 6579 4572 726f 722c 496e 6465 7845 7272  eyError,IndexErr
+000164b0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+000164c0: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+000164d0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000164e0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+000164f0: 2020 2020 2020 206c 6174 6573 745f 696e         latest_in
+00016500: 7374 6461 7465 203d 2068 6f73 7444 6174  stdate = hostDat
+00016510: 612e 6c6f 635b 686f 7374 4461 7461 2e69  a.loc[hostData.i
+00016520: 6e64 6578 5b2d 315d 2c22 4649 495f 4461  ndex[-1],"FII_Da
+00016530: 7465 225d 0a20 2020 2020 2020 2020 2020  te"].           
+00016540: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+00016550: 7374 616e 6365 286c 6174 6573 745f 696e  stance(latest_in
+00016560: 7374 6461 7465 2c20 666c 6f61 7429 3a0a  stdate, float):.
+00016570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016580: 2020 2020 2020 2020 6c61 7465 7374 5f69          latest_i
+00016590: 6e73 7464 6174 6520 3d20 6461 7465 7469  nstdate = dateti
+000165a0: 6d65 2e64 6174 6574 696d 652e 6672 6f6d  me.datetime.from
+000165b0: 7469 6d65 7374 616d 7028 6c61 7465 7374  timestamp(latest
+000165c0: 5f69 6e73 7464 6174 6529 2e73 7472 6674  _instdate).strft
+000165d0: 696d 6528 2725 592d 256d 2d25 6427 290a  ime('%Y-%m-%d').
+000165e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000165f0: 6578 6365 7074 2028 4b65 7945 7272 6f72  except (KeyError
+00016600: 2c49 6e64 6578 4572 726f 7229 3a0a 2020  ,IndexError):.  
+00016610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016620: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
+00016630: 2020 2020 2020 2069 6620 6c61 7465 7374         if latest
+00016640: 5f6d 6664 6174 6520 6973 206e 6f74 204e  _mfdate is not N
+00016650: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00016660: 2020 2020 2020 2020 2073 6176 6564 5f6d           saved_m
+00016670: 6664 6174 6520 3d20 504b 4461 7465 5574  fdate = PKDateUt
+00016680: 696c 6974 6965 732e 6461 7465 4672 6f6d  ilities.dateFrom
+00016690: 596d 6453 7472 696e 6728 6c61 7465 7374  YmdString(latest
+000166a0: 5f6d 6664 6174 652e 7370 6c69 7428 2254  _mfdate.split("T
+000166b0: 2229 5b30 5d29 0a20 2020 2020 2020 2020  ")[0]).         
+000166c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000166d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166e0: 2073 6176 6564 5f6d 6664 6174 6520 3d20   saved_mfdate = 
+000166f0: 6c61 7374 4461 794c 6173 744d 6f6e 7468  lastDayLastMonth
+00016700: 202d 2064 6174 6574 696d 652e 7469 6d65   - datetime.time
+00016710: 6465 6c74 6128 3129 0a20 2020 2020 2020  delta(1).       
+00016720: 2020 2020 2020 2020 2069 6620 6c61 7465           if late
+00016730: 7374 5f69 6e73 7464 6174 6520 6973 206e  st_instdate is n
+00016740: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00016750: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00016760: 6564 5f69 6e73 7464 6174 6520 3d20 504b  ed_instdate = PK
+00016770: 4461 7465 5574 696c 6974 6965 732e 6461  DateUtilities.da
+00016780: 7465 4672 6f6d 596d 6453 7472 696e 6728  teFromYmdString(
+00016790: 6c61 7465 7374 5f69 6e73 7464 6174 652e  latest_instdate.
+000167a0: 7370 6c69 7428 2254 2229 5b30 5d29 0a20  split("T")[0]). 
+000167b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000167c0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000167d0: 2020 2020 2020 2020 2073 6176 6564 5f69           saved_i
+000167e0: 6e73 7464 6174 6520 3d20 6c61 7374 4461  nstdate = lastDa
+000167f0: 794c 6173 744d 6f6e 7468 202d 2064 6174  yLastMonth - dat
+00016800: 6574 696d 652e 7469 6d65 6465 6c74 6128  etime.timedelta(
+00016810: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
+00016820: 2020 2074 6f64 6179 203d 2050 4b44 6174     today = PKDat
+00016830: 6555 7469 6c69 7469 6573 2e63 7572 7265  eUtilities.curre
+00016840: 6e74 4461 7465 5469 6d65 2829 0a20 2020  ntDateTime().   
+00016850: 2020 2020 2020 2020 2020 2020 206e 6565               nee
+00016860: 6473 4672 6573 6855 7064 6174 6520 3d20  dsFreshUpdate = 
+00016870: 2873 6176 6564 5f6d 6664 6174 652e 6461  (saved_mfdate.da
+00016880: 7465 2829 203c 206c 6173 7444 6179 4c61  te() < lastDayLa
+00016890: 7374 4d6f 6e74 682e 6461 7465 2829 2920  stMonth.date()) 
+000168a0: 616e 6420 2873 6176 6564 5f69 6e73 7464  and (saved_instd
+000168b0: 6174 652e 6461 7465 2829 203c 206c 6173  ate.date() < las
+000168c0: 7444 6179 4c61 7374 4d6f 6e74 682e 6461  tDayLastMonth.da
+000168d0: 7465 2829 290a 2020 2020 2020 2020 2020  te()).          
+000168e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000168f0: 2020 2020 2020 2020 6e65 6564 7346 7265          needsFre
+00016900: 7368 5570 6461 7465 203d 2054 7275 650a  shUpdate = True.
+00016910: 0a20 2020 2020 2020 2069 6620 6e65 6564  .        if need
+00016920: 7346 7265 7368 5570 6461 7465 2061 6e64  sFreshUpdate and
+00016930: 2066 6f72 6365 3a0a 2020 2020 2020 2020   force:.        
+00016940: 2020 2020 6e65 7443 6861 6e67 654d 462c      netChangeMF,
+00016950: 206e 6574 4368 616e 6765 496e 7374 2c20   netChangeInst, 
+00016960: 6c61 7465 7374 5f6d 6664 6174 652c 206c  latest_mfdate, l
+00016970: 6174 6573 745f 696e 7374 6461 7465 203d  atest_instdate =
+00016980: 2073 656c 662e 6765 7446 7265 7368 4d46   self.getFreshMF
+00016990: 4953 7461 7475 7328 7374 6f63 6b2c 6578  IStatus(stock,ex
+000169a0: 6368 616e 6765 4e61 6d65 3d65 7863 6861  changeName=excha
+000169b0: 6e67 654e 616d 6529 0a20 2020 2020 2020  ngeName).       
+000169c0: 2020 2020 2069 6620 6e65 7443 6861 6e67       if netChang
+000169d0: 654d 4620 6973 206e 6f74 204e 6f6e 653a  eMF is not None:
+000169e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000169f0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00016a00: 2020 2020 2020 2020 2020 686f 7374 4461            hostDa
+00016a10: 7461 2e6c 6f63 5b68 6f73 7444 6174 612e  ta.loc[hostData.
+00016a20: 696e 6465 785b 2d31 5d2c 224d 4622 5d20  index[-1],"MF"] 
+00016a30: 3d20 6e65 7443 6861 6e67 654d 460a 2020  = netChangeMF.  
+00016a40: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00016a50: 6365 7074 2028 4b65 7945 7272 6f72 2c49  cept (KeyError,I
+00016a60: 6e64 6578 4572 726f 7229 3a0a 2020 2020  ndexError):.    
+00016a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a80: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+00016a90: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00016aa0: 2020 2020 2020 206e 6574 4368 616e 6765         netChange
+00016ab0: 4d46 203d 2030 0a20 2020 2020 2020 2020  MF = 0.         
+00016ac0: 2020 2069 6620 6c61 7465 7374 5f6d 6664     if latest_mfd
+00016ad0: 6174 6520 6973 206e 6f74 204e 6f6e 653a  ate is not None:
+00016ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016af0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00016b00: 2020 2020 2020 2020 2020 686f 7374 4461            hostDa
+00016b10: 7461 2e6c 6f63 5b68 6f73 7444 6174 612e  ta.loc[hostData.
+00016b20: 696e 6465 785b 2d31 5d2c 224d 465f 4461  index[-1],"MF_Da
+00016b30: 7465 225d 203d 206c 6174 6573 745f 6d66  te"] = latest_mf
+00016b40: 6461 7465 0a20 2020 2020 2020 2020 2020  date.           
+00016b50: 2020 2020 2065 7863 6570 7420 284b 6579       except (Key
+00016b60: 4572 726f 722c 496e 6465 7845 7272 6f72  Error,IndexError
+00016b70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00016b80: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+00016b90: 2020 2020 2020 2020 6966 206e 6574 4368          if netCh
+00016ba0: 616e 6765 496e 7374 2069 7320 6e6f 7420  angeInst is not 
+00016bb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00016bc0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00016bd0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00016be0: 6f73 7444 6174 612e 6c6f 635b 686f 7374  ostData.loc[host
+00016bf0: 4461 7461 2e69 6e64 6578 5b2d 315d 2c22  Data.index[-1],"
+00016c00: 4649 4922 5d20 3d20 6e65 7443 6861 6e67  FII"] = netChang
+00016c10: 6549 6e73 740a 2020 2020 2020 2020 2020  eInst.          
+00016c20: 2020 2020 2020 6578 6365 7074 2028 4b65        except (Ke
+00016c30: 7945 7272 6f72 2c49 6e64 6578 4572 726f  yError,IndexErro
+00016c40: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00016c50: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+00016c60: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00016c70: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00016c80: 6574 4368 616e 6765 496e 7374 203d 2030  etChangeInst = 0
+00016c90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00016ca0: 6c61 7465 7374 5f69 6e73 7464 6174 6520  latest_instdate 
+00016cb0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00016cc0: 2020 2020 2020 2020 2020 2020 2074 7279               try
+00016cd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016ce0: 2020 2020 2020 686f 7374 4461 7461 2e6c        hostData.l
+00016cf0: 6f63 5b68 6f73 7444 6174 612e 696e 6465  oc[hostData.inde
+00016d00: 785b 2d31 5d2c 2246 4949 5f44 6174 6522  x[-1],"FII_Date"
+00016d10: 5d20 3d20 6c61 7465 7374 5f69 6e73 7464  ] = latest_instd
+00016d20: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
+00016d30: 2020 2020 6578 6365 7074 2028 4b65 7945      except (KeyE
+00016d40: 7272 6f72 2c49 6e64 6578 4572 726f 7229  rror,IndexError)
+00016d50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016d60: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+00016d70: 2020 206c 6173 7444 6179 4c61 7374 4d6f     lastDayLastMo
+00016d80: 6e74 6820 3d20 6c61 7374 4461 794c 6173  nth = lastDayLas
+00016d90: 744d 6f6e 7468 2e73 7472 6674 696d 6528  tMonth.strftime(
+00016da0: 2225 592d 256d 2d25 6454 3030 3a30 303a  "%Y-%m-%dT00:00:
+00016db0: 3030 2e30 3030 2229 0a20 2020 2020 2020  00.000").       
+00016dc0: 2069 6620 6f6e 6c79 4d46 3a0a 2020 2020   if onlyMF:.    
+00016dd0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00016de0: 6574 4368 616e 6765 4d46 0a20 2020 2020  etChangeMF.     
+00016df0: 2020 2069 6620 6c61 7465 7374 5f69 6e73     if latest_ins
+00016e00: 7464 6174 6520 3d3d 206c 6174 6573 745f  tdate == latest_
+00016e10: 6d66 6461 7465 3a0a 2020 2020 2020 2020  mfdate:.        
+00016e20: 2020 2020 7265 7475 726e 2028 6e65 7443      return (netC
+00016e30: 6861 6e67 654d 4620 2b20 6e65 7443 6861  hangeMF + netCha
+00016e40: 6e67 6549 6e73 7429 0a20 2020 2020 2020  ngeInst).       
+00016e50: 2065 6c69 6620 6c61 7465 7374 5f6d 6664   elif latest_mfd
+00016e60: 6174 6520 3d3d 206c 6173 7444 6179 4c61  ate == lastDayLa
+00016e70: 7374 4d6f 6e74 683a 0a20 2020 2020 2020  stMonth:.       
+00016e80: 2020 2020 2072 6574 7572 6e20 6e65 7443       return netC
+00016e90: 6861 6e67 654d 460a 2020 2020 2020 2020  hangeMF.        
+00016ea0: 656c 6966 206c 6174 6573 745f 696e 7374  elif latest_inst
+00016eb0: 6461 7465 203d 3d20 6c61 7374 4461 794c  date == lastDayL
+00016ec0: 6173 744d 6f6e 7468 3a0a 2020 2020 2020  astMonth:.      
+00016ed0: 2020 2020 2020 7265 7475 726e 206e 6574        return net
+00016ee0: 4368 616e 6765 496e 7374 0a20 2020 2020  ChangeInst.     
+00016ef0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00016f00: 2020 2020 2023 2066 696e 6420 7468 6520       # find the 
+00016f10: 6c61 7465 7374 2064 6174 650a 2020 2020  latest date.    
+00016f20: 2020 2020 2020 2020 6966 206c 6174 6573          if lates
+00016f30: 745f 6d66 6461 7465 2069 7320 6e6f 7420  t_mfdate is not 
+00016f40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00016f50: 2020 2020 2020 6c61 7465 7374 5f6d 6664        latest_mfd
+00016f60: 6174 6520 3d20 504b 4461 7465 5574 696c  ate = PKDateUtil
+00016f70: 6974 6965 732e 6461 7465 4672 6f6d 596d  ities.dateFromYm
+00016f80: 6453 7472 696e 6728 6c61 7465 7374 5f6d  dString(latest_m
+00016f90: 6664 6174 652e 7370 6c69 7428 2254 2229  fdate.split("T")
+00016fa0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+00016fb0: 2069 6620 6c61 7465 7374 5f69 6e73 7464   if latest_instd
+00016fc0: 6174 6520 6973 206e 6f74 204e 6f6e 653a  ate is not None:
+00016fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016fe0: 206c 6174 6573 745f 696e 7374 6461 7465   latest_instdate
+00016ff0: 203d 2050 4b44 6174 6555 7469 6c69 7469   = PKDateUtiliti
+00017000: 6573 2e64 6174 6546 726f 6d59 6d64 5374  es.dateFromYmdSt
+00017010: 7269 6e67 286c 6174 6573 745f 696e 7374  ring(latest_inst
+00017020: 6461 7465 2e73 706c 6974 2822 5422 295b  date.split("T")[
+00017030: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
+00017040: 7265 7475 726e 206e 6574 4368 616e 6765  return netChange
+00017050: 4d46 2069 6620 2828 6c61 7465 7374 5f6d  MF if ((latest_m
+00017060: 6664 6174 6520 6973 206e 6f74 204e 6f6e  fdate is not Non
+00017070: 6529 2061 6e64 206c 6174 6573 745f 6d66  e) and latest_mf
+00017080: 6461 7465 203e 2028 6c61 7465 7374 5f69  date > (latest_i
+00017090: 6e73 7464 6174 6520 6966 206c 6174 6573  nstdate if lates
+000170a0: 745f 696e 7374 6461 7465 2069 7320 6e6f  t_instdate is no
+000170b0: 7420 4e6f 6e65 2065 6c73 6520 286c 6174  t None else (lat
+000170c0: 6573 745f 6d66 6461 7465 202d 2064 6174  est_mfdate - dat
+000170d0: 6574 696d 652e 7469 6d65 6465 6c74 6128  etime.timedelta(
+000170e0: 3129 2929 2920 656c 7365 206e 6574 4368  1)))) else netCh
+000170f0: 616e 6765 496e 7374 0a0a 2020 2020 6465  angeInst..    de
+00017100: 6620 6765 7446 7265 7368 4d46 4953 7461  f getFreshMFISta
+00017110: 7475 7328 7365 6c66 2c20 7374 6f63 6b2c  tus(self, stock,
+00017120: 6578 6368 616e 6765 4e61 6d65 3d22 494e  exchangeName="IN
+00017130: 4449 4122 293a 0a20 2020 2020 2020 2063  DIA"):.        c
+00017140: 6861 6e67 6553 7461 7475 7344 6174 614d  hangeStatusDataM
+00017150: 4620 3d20 4e6f 6e65 0a20 2020 2020 2020  F = None.       
+00017160: 2063 6861 6e67 6553 7461 7475 7344 6174   changeStatusDat
+00017170: 6149 6e73 7420 3d20 4e6f 6e65 0a20 2020  aInst = None.   
+00017180: 2020 2020 206e 6574 4368 616e 6765 4d46       netChangeMF
+00017190: 203d 2030 0a20 2020 2020 2020 206e 6574   = 0.        net
+000171a0: 4368 616e 6765 496e 7374 203d 2030 0a20  ChangeInst = 0. 
+000171b0: 2020 2020 2020 206c 6174 6573 745f 6d66         latest_mf
+000171c0: 6461 7465 203d 204e 6f6e 650a 2020 2020  date = None.    
+000171d0: 2020 2020 6c61 7465 7374 5f69 6e73 7464      latest_instd
+000171e0: 6174 6520 3d20 4e6f 6e65 0a20 2020 2020  ate = None.     
+000171f0: 2020 2073 6563 7572 6974 7920 3d20 4e6f     security = No
+00017200: 6e65 0a20 2020 2020 2020 2074 7279 3a0a  ne.        try:.
+00017210: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00017220: 2053 7570 7072 6573 734f 7574 7075 7428   SuppressOutput(
+00017230: 7375 7070 7265 7373 5f73 7464 6572 723d  suppress_stderr=
+00017240: 5472 7565 2c20 7375 7070 7265 7373 5f73  True, suppress_s
+00017250: 7464 6f75 743d 5472 7565 293a 0a20 2020  tdout=True):.   
+00017260: 2020 2020 2020 2020 2020 2020 2073 6563               sec
+00017270: 7572 6974 7920 3d20 5374 6f63 6b28 7374  urity = Stock(st
+00017280: 6f63 6b2c 6578 6368 616e 6765 3d65 7863  ock,exchange=exc
+00017290: 6861 6e67 654e 616d 6529 0a20 2020 2020  hangeName).     
+000172a0: 2020 2065 7863 6570 7420 5661 6c75 6545     except ValueE
+000172b0: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+000172c0: 2020 2320 5765 2064 6964 206e 6f74 2066    # We did not f
+000172d0: 696e 6420 7468 6520 7374 6f63 6b3f 2049  ind the stock? I
+000172e0: 7427 7320 6f6b 6179 2e20 4d6f 7665 206f  t's okay. Move o
+000172f0: 6e20 746f 2074 6865 206e 6578 7420 6f6e  n to the next on
+00017300: 652e 0a20 2020 2020 2020 2020 2020 2070  e..            p
+00017310: 6173 730a 2020 2020 2020 2020 6578 6365  ass.        exce
+00017320: 7074 2028 5469 6d65 6f75 7445 7272 6f72  pt (TimeoutError
+00017330: 2c20 436f 6e6e 6563 7469 6f6e 4572 726f  , ConnectionErro
+00017340: 7229 2061 7320 653a 0a20 2020 2020 2020  r) as e:.       
+00017350: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
+00017360: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
+00017370: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
+00017380: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
+00017390: 730a 2020 2020 2020 2020 6578 6365 7074  s.        except
+000173a0: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+000173b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000173c0: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
+000173d0: 2e64 6562 7567 2865 2c20 6578 635f 696e  .debug(e, exc_in
+000173e0: 666f 3d54 7275 6529 0a20 2020 2020 2020  fo=True).       
+000173f0: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
+00017400: 2020 6966 2073 6563 7572 6974 7920 6973    if security is
+00017410: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00017420: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00017430: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00017440: 2053 7570 7072 6573 734f 7574 7075 7428   SuppressOutput(
+00017450: 7375 7070 7265 7373 5f73 7464 6572 723d  suppress_stderr=
+00017460: 5472 7565 2c20 7375 7070 7265 7373 5f73  True, suppress_s
+00017470: 7464 6f75 743d 5472 7565 293a 0a20 2020  tdout=True):.   
+00017480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017490: 2063 6861 6e67 6553 7461 7475 7352 6f77   changeStatusRow
+000174a0: 734d 4620 3d20 7365 6375 7269 7479 2e6d  sMF = security.m
+000174b0: 7574 7561 6c46 756e 644f 776e 6572 7368  utualFundOwnersh
+000174c0: 6970 2874 6f70 3d35 290a 2020 2020 2020  ip(top=5).      
+000174d0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+000174e0: 616e 6765 5374 6174 7573 526f 7773 496e  angeStatusRowsIn
+000174f0: 7374 203d 2073 6563 7572 6974 792e 696e  st = security.in
+00017500: 7374 6974 7574 696f 6e4f 776e 6572 7368  stitutionOwnersh
+00017510: 6970 2874 6f70 3d35 290a 2020 2020 2020  ip(top=5).      
+00017520: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+00017530: 616e 6765 5374 6174 7573 4461 7461 4d46  angeStatusDataMF
+00017540: 203d 2073 6563 7572 6974 792e 6d75 7475   = security.mutu
+00017550: 616c 4675 6e64 4649 4943 6861 6e67 6544  alFundFIIChangeD
+00017560: 6174 6128 6368 616e 6765 5374 6174 7573  ata(changeStatus
+00017570: 526f 7773 4d46 290a 2020 2020 2020 2020  RowsMF).        
+00017580: 2020 2020 2020 2020 2020 2020 6368 616e              chan
+00017590: 6765 5374 6174 7573 4461 7461 496e 7374  geStatusDataInst
+000175a0: 203d 2073 6563 7572 6974 792e 6d75 7475   = security.mutu
+000175b0: 616c 4675 6e64 4649 4943 6861 6e67 6544  alFundFIIChangeD
+000175c0: 6174 6128 6368 616e 6765 5374 6174 7573  ata(changeStatus
+000175d0: 526f 7773 496e 7374 290a 2020 2020 2020  RowsInst).      
+000175e0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+000175f0: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
+00017600: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017610: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
+00017620: 2e64 6562 7567 2865 2c20 6578 635f 696e  .debug(e, exc_in
+00017630: 666f 3d54 7275 6529 0a20 2020 2020 2020  fo=True).       
+00017640: 2020 2020 2020 2020 2023 2054 7970 6545           # TypeE
+00017650: 7272 6f72 206f 7220 436f 6e6e 6563 7469  rror or Connecti
+00017660: 6f6e 4572 726f 7220 6265 6361 7573 6520  onError because 
+00017670: 7765 2063 6f75 6c64 206e 6f74 2066 696e  we could not fin
+00017680: 6420 7468 6520 7374 6f63 6b20 6f72 204d  d the stock or M
+00017690: 4649 2064 6174 6120 6973 6e27 7420 6176  FI data isn't av
+000176a0: 6169 6c61 626c 653f 0a20 2020 2020 2020  ailable?.       
+000176b0: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+000176c0: 2020 2020 2020 2020 2020 6c61 7374 4461            lastDa
+000176d0: 794c 6173 744d 6f6e 7468 203d 2050 4b44  yLastMonth = PKD
+000176e0: 6174 6555 7469 6c69 7469 6573 2e6c 6173  ateUtilities.las
+000176f0: 745f 6461 795f 6f66 5f70 7265 7669 6f75  t_day_of_previou
+00017700: 735f 6d6f 6e74 6828 504b 4461 7465 5574  s_month(PKDateUt
+00017710: 696c 6974 6965 732e 6375 7272 656e 7444  ilities.currentD
+00017720: 6174 6554 696d 6528 2929 0a20 2020 2020  ateTime()).     
+00017730: 2020 2020 2020 206c 6173 7444 6179 4c61         lastDayLa
+00017740: 7374 4d6f 6e74 6820 3d20 6c61 7374 4461  stMonth = lastDa
+00017750: 794c 6173 744d 6f6e 7468 2e73 7472 6674  yLastMonth.strft
+00017760: 696d 6528 2225 592d 256d 2d25 6454 3030  ime("%Y-%m-%dT00
+00017770: 3a30 303a 3030 2e30 3030 2229 0a20 2020  :00:00.000").   
+00017780: 2020 2020 2020 2020 2069 6620 6368 616e           if chan
+00017790: 6765 5374 6174 7573 4461 7461 4d46 2069  geStatusDataMF i
+000177a0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206c  s not None and l
+000177b0: 656e 2863 6861 6e67 6553 7461 7475 7344  en(changeStatusD
+000177c0: 6174 614d 4629 203e 2030 3a0a 2020 2020  ataMF) > 0:.    
+000177d0: 2020 2020 2020 2020 2020 2020 6466 5f67              df_g
+000177e0: 726f 7570 6564 4d46 203d 2063 6861 6e67  roupedMF = chang
+000177f0: 6553 7461 7475 7344 6174 614d 462e 6772  eStatusDataMF.gr
+00017800: 6f75 7062 7928 2264 6174 6522 2c20 736f  oupby("date", so
+00017810: 7274 3d46 616c 7365 290a 2020 2020 2020  rt=False).      
+00017820: 2020 2020 2020 2020 2020 666f 7220 6d66            for mf
+00017830: 6461 7465 2c20 6466 5f67 726f 7570 4d46  date, df_groupMF
+00017840: 2069 6e20 6466 5f67 726f 7570 6564 4d46   in df_groupedMF
+00017850: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017860: 2020 2020 2020 6e65 7443 6861 6e67 654d        netChangeM
+00017870: 4620 3d20 6466 5f67 726f 7570 4d46 5b22  F = df_groupMF["
+00017880: 6368 616e 6765 416d 6f75 6e74 225d 2e73  changeAmount"].s
+00017890: 756d 2829 0a20 2020 2020 2020 2020 2020  um().           
+000178a0: 2020 2020 2020 2020 206c 6174 6573 745f           latest_
+000178b0: 6d66 6461 7465 203d 206d 6664 6174 650a  mfdate = mfdate.
+000178c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178d0: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+000178e0: 2020 2020 2020 6966 2063 6861 6e67 6553        if changeS
+000178f0: 7461 7475 7344 6174 6149 6e73 7420 6973  tatusDataInst is
+00017900: 206e 6f74 204e 6f6e 6520 616e 6420 6c65   not None and le
+00017910: 6e28 6368 616e 6765 5374 6174 7573 4461  n(changeStatusDa
+00017920: 7461 496e 7374 2920 3e20 303a 0a20 2020  taInst) > 0:.   
+00017930: 2020 2020 2020 2020 2020 2020 2064 665f               df_
+00017940: 6772 6f75 7065 6449 6e73 7420 3d20 6368  groupedInst = ch
+00017950: 616e 6765 5374 6174 7573 4461 7461 496e  angeStatusDataIn
+00017960: 7374 2e67 726f 7570 6279 2822 6461 7465  st.groupby("date
+00017970: 222c 2073 6f72 743d 4661 6c73 6529 0a20  ", sort=False). 
+00017980: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00017990: 6f72 2069 6e73 7464 6174 652c 2064 665f  or instdate, df_
+000179a0: 6772 6f75 7049 6e73 7420 696e 2064 665f  groupInst in df_
+000179b0: 6772 6f75 7065 6449 6e73 743a 0a20 2020  groupedInst:.   
+000179c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179d0: 2069 6620 286c 6174 6573 745f 6d66 6461   if (latest_mfda
+000179e0: 7465 2069 7320 6e6f 7420 4e6f 6e65 2061  te is not None a
+000179f0: 6e64 206c 6174 6573 745f 6d66 6461 7465  nd latest_mfdate
+00017a00: 203d 3d20 696e 7374 6461 7465 2920 6f72   == instdate) or
+00017a10: 2028 6c61 7465 7374 5f6d 6664 6174 6520   (latest_mfdate 
+00017a20: 6973 204e 6f6e 6529 206f 7220 2869 6e73  is None) or (ins
+00017a30: 7464 6174 6520 3d3d 206c 6173 7444 6179  tdate == lastDay
+00017a40: 4c61 7374 4d6f 6e74 6829 3a0a 2020 2020  LastMonth):.    
+00017a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a60: 2020 2020 6e65 7443 6861 6e67 6549 6e73      netChangeIns
+00017a70: 7420 3d20 6466 5f67 726f 7570 496e 7374  t = df_groupInst
+00017a80: 5b22 6368 616e 6765 416d 6f75 6e74 225d  ["changeAmount"]
+00017a90: 2e73 756d 2829 0a20 2020 2020 2020 2020  .sum().         
+00017aa0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00017ab0: 6174 6573 745f 696e 7374 6461 7465 203d  atest_instdate =
+00017ac0: 2069 6e73 7464 6174 650a 2020 2020 2020   instdate.      
+00017ad0: 2020 2020 2020 2020 2020 2020 2020 6272                br
+00017ae0: 6561 6b0a 2020 2020 2020 2020 7265 7475  eak.        retu
+00017af0: 726e 206e 6574 4368 616e 6765 4d46 2c6e  rn netChangeMF,n
+00017b00: 6574 4368 616e 6765 496e 7374 2c6c 6174  etChangeInst,lat
+00017b10: 6573 745f 6d66 6461 7465 2c6c 6174 6573  est_mfdate,lates
+00017b20: 745f 696e 7374 6461 7465 0a0a 0a20 2020  t_instdate...   
+00017b30: 2064 6566 2067 6574 4e69 6674 7950 7265   def getNiftyPre
+00017b40: 6469 6374 696f 6e28 7365 6c66 2c20 6466  diction(self, df
+00017b50: 293a 0a20 2020 2020 2020 2069 6d70 6f72  ):.        impor
+00017b60: 7420 7761 726e 696e 6773 0a0a 2020 2020  t warnings..    
+00017b70: 2020 2020 7761 726e 696e 6773 2e66 696c      warnings.fil
+00017b80: 7465 7277 6172 6e69 6e67 7328 2269 676e  terwarnings("ign
+00017b90: 6f72 6522 290a 2020 2020 2020 2020 6461  ore").        da
+00017ba0: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
+00017bb0: 2020 2020 2020 206d 6f64 656c 2c20 706b         model, pk
+00017bc0: 6c20 3d20 5574 696c 6974 792e 746f 6f6c  l = Utility.tool
+00017bd0: 732e 6765 744e 6966 7479 4d6f 6465 6c28  s.getNiftyModel(
+00017be0: 290a 2020 2020 2020 2020 6966 206d 6f64  ).        if mod
+00017bf0: 656c 2069 7320 4e6f 6e65 206f 7220 706b  el is None or pk
+00017c00: 6c20 6973 204e 6f6e 653a 0a20 2020 2020  l is None:.     
+00017c10: 2020 2020 2020 2072 6574 7572 6e20 302c         return 0,
+00017c20: 2022 556e 6b6e 6f77 6e22 2c20 2255 6e6b   "Unknown", "Unk
+00017c30: 6e6f 776e 220a 2020 2020 2020 2020 7769  nown".        wi
+00017c40: 7468 2053 7570 7072 6573 734f 7574 7075  th SuppressOutpu
+00017c50: 7428 7375 7070 7265 7373 5f73 7464 6572  t(suppress_stder
+00017c60: 723d 5472 7565 2c20 7375 7070 7265 7373  r=True, suppress
+00017c70: 5f73 7464 6f75 743d 5472 7565 293a 0a20  _stdout=True):. 
+00017c80: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00017c90: 3d20 6461 7461 5b70 6b6c 5b22 636f 6c75  = data[pkl["colu
+00017ca0: 6d6e 7322 5d5d 0a20 2020 2020 2020 2020  mns"]].         
+00017cb0: 2020 2023 2323 2076 3220 5072 6570 726f     ### v2 Prepro
+00017cc0: 6365 7373 696e 670a 2020 2020 2020 2020  cessing.        
+00017cd0: 2020 2020 6461 7461 5b22 4869 6768 225d      data["High"]
+00017ce0: 203d 2064 6174 615b 2248 6967 6822 5d2e   = data["High"].
+00017cf0: 7063 745f 6368 616e 6765 2829 202a 2031  pct_change() * 1
+00017d00: 3030 0a20 2020 2020 2020 2020 2020 2064  00.            d
+00017d10: 6174 615b 224c 6f77 225d 203d 2064 6174  ata["Low"] = dat
+00017d20: 615b 224c 6f77 225d 2e70 6374 5f63 6861  a["Low"].pct_cha
+00017d30: 6e67 6528 2920 2a20 3130 300a 2020 2020  nge() * 100.    
+00017d40: 2020 2020 2020 2020 6461 7461 5b22 4f70          data["Op
+00017d50: 656e 225d 203d 2064 6174 615b 224f 7065  en"] = data["Ope
+00017d60: 6e22 5d2e 7063 745f 6368 616e 6765 2829  n"].pct_change()
+00017d70: 202a 2031 3030 0a20 2020 2020 2020 2020   * 100.         
+00017d80: 2020 2064 6174 615b 2243 6c6f 7365 225d     data["Close"]
+00017d90: 203d 2064 6174 615b 2243 6c6f 7365 225d   = data["Close"]
+00017da0: 2e70 6374 5f63 6861 6e67 6528 2920 2a20  .pct_change() * 
+00017db0: 3130 300a 2020 2020 2020 2020 2020 2020  100.            
+00017dc0: 6461 7461 203d 2064 6174 612e 696c 6f63  data = data.iloc
+00017dd0: 5b2d 315d 0a20 2020 2020 2020 2020 2020  [-1].           
+00017de0: 2023 2323 0a20 2020 2020 2020 2020 2020   ###.           
+00017df0: 2064 6174 6120 3d20 706b 6c5b 2273 6361   data = pkl["sca
+00017e00: 6c65 7222 5d2e 7472 616e 7366 6f72 6d28  ler"].transform(
+00017e10: 5b64 6174 615d 290a 2020 2020 2020 2020  [data]).        
+00017e20: 2020 2020 7769 7468 2053 7570 7072 6573      with Suppres
+00017e30: 734f 7574 7075 7428 7375 7070 7265 7373  sOutput(suppress
+00017e40: 5f73 7464 6f75 743d 5472 7565 2c20 7375  _stdout=True, su
+00017e50: 7070 7265 7373 5f73 7464 6572 723d 5472  ppress_stderr=Tr
+00017e60: 7565 293a 0a20 2020 2020 2020 2020 2020  ue):.           
+00017e70: 2020 2020 2070 7265 6420 3d20 6d6f 6465       pred = mode
+00017e80: 6c2e 7072 6564 6963 7428 6461 7461 295b  l.predict(data)[
+00017e90: 305d 0a20 2020 2020 2020 2069 6620 7072  0].        if pr
+00017ea0: 6564 203e 2030 2e35 3a0a 2020 2020 2020  ed > 0.5:.      
+00017eb0: 2020 2020 2020 6f75 7454 6578 7420 3d20        outText = 
+00017ec0: 2242 4541 5249 5348 220a 2020 2020 2020  "BEARISH".      
+00017ed0: 2020 2020 2020 6f75 7420 3d20 280a 2020        out = (.  
+00017ee0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00017ef0: 6c6f 7254 6578 742e 424f 4c44 0a20 2020  lorText.BOLD.   
+00017f00: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+00017f10: 6f6c 6f72 5465 7874 2e46 4149 4c0a 2020  olorText.FAIL.  
 00017f20: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00017f30: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-00017f40: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00017f50: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
-00017f60: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00017f70: 2020 2020 2020 2020 2073 7567 203d 2022           sug = "
-00017f80: 486f 6c64 2079 6f75 7220 5368 6f72 7420  Hold your Short 
-00017f90: 706f 7369 7469 6f6e 2122 0a20 2020 2020  position!".     
-00017fa0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00017fb0: 2020 2020 206f 7574 5465 7874 203d 2022       outText = "
-00017fc0: 4255 4c4c 4953 4822 0a20 2020 2020 2020  BULLISH".       
-00017fd0: 2020 2020 206f 7574 203d 2028 0a20 2020       out = (.   
-00017fe0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00017ff0: 6f72 5465 7874 2e42 4f4c 440a 2020 2020  orText.BOLD.    
-00018000: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-00018010: 6c6f 7254 6578 742e 4752 4545 4e0a 2020  lorText.GREEN.  
-00018020: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00018030: 6f75 7454 6578 740a 2020 2020 2020 2020  outText.        
-00018040: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-00018050: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
-00018060: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-00018070: 6578 742e 424f 4c44 0a20 2020 2020 2020  ext.BOLD.       
-00018080: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00018090: 2020 2073 7567 203d 2022 5374 6179 2042     sug = "Stay B
-000180a0: 756c 6c69 7368 2122 0a20 2020 2020 2020  ullish!".       
-000180b0: 2069 6620 504b 4461 7465 5574 696c 6974   if PKDateUtilit
-000180c0: 6965 732e 6973 436c 6f73 696e 6748 6f75  ies.isClosingHou
-000180d0: 7228 293a 0a20 2020 2020 2020 2020 2020  r():.           
-000180e0: 204f 7574 7075 7443 6f6e 7472 6f6c 7328   OutputControls(
-000180f0: 292e 7072 696e 744f 7574 7075 7428 0a20  ).printOutput(. 
-00018100: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00018110: 6f6c 6f72 5465 7874 2e42 4f4c 440a 2020  olorText.BOLD.  
-00018120: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00018130: 636f 6c6f 7254 6578 742e 5741 524e 0a20  colorText.WARN. 
-00018140: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00018150: 2022 4e6f 7465 3a20 5468 6520 4149 2070   "Note: The AI p
-00018160: 7265 6469 6374 696f 6e20 7368 6f75 6c64  rediction should
-00018170: 2062 6520 6578 6563 7574 6564 2041 6674   be executed Aft
-00018180: 6572 2033 2050 4d20 6f72 204e 6561 7220  er 3 PM or Near 
-00018190: 746f 2043 6c6f 7369 6e67 2074 696d 6520  to Closing time 
-000181a0: 6173 2074 6865 2050 7265 6469 6374 696f  as the Predictio
-000181b0: 6e20 4163 6375 7261 6379 2069 7320 6261  n Accuracy is ba
-000181c0: 7365 6420 6f6e 2074 6865 2043 6c6f 7369  sed on the Closi
-000181d0: 6e67 2070 7269 6365 2122 0a20 2020 2020  ng price!".     
-000181e0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-000181f0: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
-00018200: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00018210: 2070 7265 6469 6374 696f 6e54 6578 7420   predictionText 
-00018220: 3d20 224d 6172 6b65 7420 6d61 7920 4f70  = "Market may Op
-00018230: 656e 207b 7d20 6e65 7874 2064 6179 2120  en {} next day! 
-00018240: 7b7d 222e 666f 726d 6174 286f 7574 2c20  {}".format(out, 
-00018250: 7375 6729 0a20 2020 2020 2020 2073 7472  sug).        str
-00018260: 656e 6774 6854 6578 7420 3d20 2250 726f  engthText = "Pro
-00018270: 6261 6269 6c69 7479 2f53 7472 656e 6774  bability/Strengt
-00018280: 6820 6f66 2050 7265 6469 6374 696f 6e20  h of Prediction 
-00018290: 3d20 7b7d 2522 2e66 6f72 6d61 7428 0a20  = {}%".format(. 
-000182a0: 2020 2020 2020 2020 2020 2055 7469 6c69             Utili
-000182b0: 7479 2e74 6f6f 6c73 2e67 6574 5369 676d  ty.tools.getSigm
-000182c0: 6f69 6443 6f6e 6669 6465 6e63 6528 7072  oidConfidence(pr
-000182d0: 6564 5b30 5d29 0a20 2020 2020 2020 2029  ed[0]).        )
-000182e0: 0a20 2020 2020 2020 204f 7574 7075 7443  .        OutputC
-000182f0: 6f6e 7472 6f6c 7328 292e 7072 696e 744f  ontrols().printO
-00018300: 7574 7075 7428 0a20 2020 2020 2020 2020  utput(.         
-00018310: 2020 2063 6f6c 6f72 5465 7874 2e42 4f4c     colorText.BOL
-00018320: 440a 2020 2020 2020 2020 2020 2020 2b20  D.            + 
-00018330: 636f 6c6f 7254 6578 742e 424c 5545 0a20  colorText.BLUE. 
-00018340: 2020 2020 2020 2020 2020 202b 2022 5c6e             + "\n
-00018350: 220a 2020 2020 2020 2020 2020 2020 2b20  ".            + 
-00018360: 225b 2b5d 204e 6966 7479 2041 4920 5072  "[+] Nifty AI Pr
-00018370: 6564 6963 7469 6f6e 202d 3e20 220a 2020  ediction -> ".  
-00018380: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-00018390: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
-000183a0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-000183b0: 742e 424f 4c44 0a20 2020 2020 2020 2020  t.BOLD.         
-000183c0: 2020 202b 2070 7265 6469 6374 696f 6e54     + predictionT
-000183d0: 6578 740a 2020 2020 2020 2020 2020 2020  ext.            
-000183e0: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-000183f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00018400: 2020 4f75 7470 7574 436f 6e74 726f 6c73    OutputControls
-00018410: 2829 2e70 7269 6e74 4f75 7470 7574 280a  ().printOutput(.
-00018420: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-00018430: 7254 6578 742e 424f 4c44 0a20 2020 2020  rText.BOLD.     
-00018440: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-00018450: 7874 2e42 4c55 450a 2020 2020 2020 2020  xt.BLUE.        
-00018460: 2020 2020 2b20 225c 6e22 0a20 2020 2020      + "\n".     
-00018470: 2020 2020 2020 202b 2022 5b2b 5d20 4e69         + "[+] Ni
-00018480: 6674 7920 4149 2050 7265 6469 6374 696f  fty AI Predictio
-00018490: 6e20 2d3e 2022 0a20 2020 2020 2020 2020  n -> ".         
-000184a0: 2020 202b 2063 6f6c 6f72 5465 7874 2e45     + colorText.E
-000184b0: 4e44 0a20 2020 2020 2020 2020 2020 202b  ND.            +
-000184c0: 2073 7472 656e 6774 6854 6578 740a 2020   strengthText.  
-000184d0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000184e0: 2072 6574 7572 6e20 7072 6564 2c20 7072   return pred, pr
-000184f0: 6564 6963 7469 6f6e 5465 7874 2e72 6570  edictionText.rep
-00018500: 6c61 6365 286f 7574 2c20 6f75 7454 6578  lace(out, outTex
-00018510: 7429 2c20 7374 7265 6e67 7468 5465 7874  t), strengthText
-00018520: 0a0a 2020 2020 6465 6620 6d6f 6e69 746f  ..    def monito
-00018530: 7246 6976 6545 6d61 2873 656c 662c 2066  rFiveEma(self, f
-00018540: 6574 6368 6572 2c20 7265 7375 6c74 5f64  etcher, result_d
-00018550: 662c 206c 6173 745f 7369 676e 616c 2c20  f, last_signal, 
-00018560: 7269 736b 5f72 6577 6172 643d 3329 3a0a  risk_reward=3):.
-00018570: 2020 2020 2020 2020 636f 6c5f 6e61 6d65          col_name
-00018580: 7320 3d20 5b22 4869 6768 222c 2022 4c6f  s = ["High", "Lo
-00018590: 7722 2c20 2243 6c6f 7365 222c 2022 3545  w", "Close", "5E
-000185a0: 4d41 225d 0a20 2020 2020 2020 2064 6174  MA"].        dat
-000185b0: 615f 6c69 7374 203d 205b 226e 6966 7479  a_list = ["nifty
-000185c0: 5f62 7579 222c 2022 6261 6e6b 6e69 6674  _buy", "banknift
-000185d0: 795f 6275 7922 2c20 226e 6966 7479 5f73  y_buy", "nifty_s
-000185e0: 656c 6c22 2c20 2262 616e 6b6e 6966 7479  ell", "banknifty
-000185f0: 5f73 656c 6c22 5d0a 0a20 2020 2020 2020  _sell"]..       
-00018600: 2064 6174 615f 7475 706c 6520 3d20 6665   data_tuple = fe
-00018610: 7463 6865 722e 6665 7463 6846 6976 6545  tcher.fetchFiveE
-00018620: 6d61 4461 7461 2829 0a20 2020 2020 2020  maData().       
-00018630: 2066 6f72 2063 6e74 2069 6e20 7261 6e67   for cnt in rang
-00018640: 6528 6c65 6e28 6461 7461 5f74 7570 6c65  e(len(data_tuple
-00018650: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00018660: 6420 3d20 6461 7461 5f74 7570 6c65 5b63  d = data_tuple[c
-00018670: 6e74 5d0a 2020 2020 2020 2020 2020 2020  nt].            
-00018680: 645b 2235 454d 4122 5d20 3d20 706b 7461  d["5EMA"] = pkta
-00018690: 6c69 622e 454d 4128 645b 2243 6c6f 7365  lib.EMA(d["Close
-000186a0: 225d 2c20 7469 6d65 7065 7269 6f64 3d35  "], timeperiod=5
-000186b0: 290a 2020 2020 2020 2020 2020 2020 6420  ).            d 
-000186c0: 3d20 645b 636f 6c5f 6e61 6d65 735d 0a20  = d[col_names]. 
-000186d0: 2020 2020 2020 2020 2020 2064 203d 2064             d = d
-000186e0: 2e64 726f 706e 6128 292e 726f 756e 6428  .dropna().round(
-000186f0: 3229 0a0a 2020 2020 2020 2020 2020 2020  2)..            
-00018700: 7769 7468 2053 7570 7072 6573 734f 7574  with SuppressOut
-00018710: 7075 7428 7375 7070 7265 7373 5f73 7464  put(suppress_std
-00018720: 6572 723d 5472 7565 2c20 7375 7070 7265  err=True, suppre
-00018730: 7373 5f73 7464 6f75 743d 5472 7565 293a  ss_stdout=True):
-00018740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018750: 2069 6620 2273 656c 6c22 2069 6e20 6461   if "sell" in da
-00018760: 7461 5f6c 6973 745b 636e 745d 3a0a 2020  ta_list[cnt]:.  
-00018770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018780: 2020 7374 7265 6368 6564 203d 2064 5b28    streched = d[(
-00018790: 642e 4c6f 7720 3e20 645b 2235 454d 4122  d.Low > d["5EMA"
-000187a0: 5d29 2026 2028 642e 4c6f 7720 2d20 645b  ]) & (d.Low - d[
-000187b0: 2235 454d 4122 5d20 3e20 302e 3529 5d0a  "5EMA"] > 0.5)].
-000187c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187d0: 2020 2020 7374 7265 6368 6564 5b22 534c      streched["SL
-000187e0: 225d 203d 2073 7472 6563 6865 642e 4869  "] = streched.Hi
-000187f0: 6768 0a20 2020 2020 2020 2020 2020 2020  gh.             
-00018800: 2020 2020 2020 2076 616c 6964 6174 6520         validate 
-00018810: 3d20 645b 0a20 2020 2020 2020 2020 2020  = d[.           
-00018820: 2020 2020 2020 2020 2020 2020 2028 642e               (d.
-00018830: 4c6f 772e 7368 6966 7428 3129 203e 2064  Low.shift(1) > d
-00018840: 5b22 3545 4d41 225d 2e73 6869 6674 2831  ["5EMA"].shift(1
-00018850: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00018860: 2020 2020 2020 2020 2020 2026 2028 642e             & (d.
-00018870: 4c6f 772e 7368 6966 7428 3129 202d 2064  Low.shift(1) - d
-00018880: 5b22 3545 4d41 225d 2e73 6869 6674 2831  ["5EMA"].shift(1
-00018890: 2920 3e20 302e 3529 0a20 2020 2020 2020  ) > 0.5).       
-000188a0: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
-000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188c0: 2020 206f 6c64 5f69 6e64 6578 203d 2076     old_index = v
-000188d0: 616c 6964 6174 652e 696e 6465 780a 2020  alidate.index.  
-000188e0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000188f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00018900: 2020 2020 2020 2020 6d61 736b 203d 2028          mask = (
-00018910: 642e 4869 6768 203c 2064 5b22 3545 4d41  d.High < d["5EMA
-00018920: 225d 2920 2620 2864 5b22 3545 4d41 225d  "]) & (d["5EMA"]
-00018930: 202d 2064 2e48 6967 6820 3e20 302e 3529   - d.High > 0.5)
-00018940: 2020 2320 4275 790a 2020 2020 2020 2020    # Buy.        
-00018950: 2020 2020 2020 2020 2020 2020 7374 7265              stre
-00018960: 6368 6564 203d 2064 5b6d 6173 6b5d 0a20  ched = d[mask]. 
-00018970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018980: 2020 2073 7472 6563 6865 645b 2253 4c22     streched["SL"
-00018990: 5d20 3d20 7374 7265 6368 6564 2e4c 6f77  ] = streched.Low
-000189a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000189b0: 2020 2020 2076 616c 6964 6174 6520 3d20       validate = 
-000189c0: 642e 6c6f 635b 6d61 736b 2e73 6869 6674  d.loc[mask.shift
-000189d0: 2831 292e 6669 6c6c 6e61 2846 616c 7365  (1).fillna(False
-000189e0: 295d 0a20 2020 2020 2020 2020 2020 2020  )].             
-000189f0: 2020 2020 2020 206f 6c64 5f69 6e64 6578         old_index
-00018a00: 203d 2076 616c 6964 6174 652e 696e 6465   = validate.inde
-00018a10: 780a 2020 2020 2020 2020 2020 2020 7467  x.            tg
-00018a20: 7420 3d20 7064 2e44 6174 6146 7261 6d65  t = pd.DataFrame
-00018a30: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00018a40: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-00018a50: 2020 2020 2020 2020 7661 6c69 6461 7465          validate
-00018a60: 2e43 6c6f 7365 2e72 6573 6574 5f69 6e64  .Close.reset_ind
-00018a70: 6578 2864 726f 703d 5472 7565 290a 2020  ex(drop=True).  
-00018a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a90: 2020 2d20 280a 2020 2020 2020 2020 2020    - (.          
-00018aa0: 2020 2020 2020 2020 2020 2020 2020 280a                (.
+00017f30: 6f75 7454 6578 740a 2020 2020 2020 2020  outText.        
+00017f40: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00017f50: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+00017f60: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00017f70: 6578 742e 424f 4c44 0a20 2020 2020 2020  ext.BOLD.       
+00017f80: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00017f90: 2020 2073 7567 203d 2022 486f 6c64 2079     sug = "Hold y
+00017fa0: 6f75 7220 5368 6f72 7420 706f 7369 7469  our Short positi
+00017fb0: 6f6e 2122 0a20 2020 2020 2020 2065 6c73  on!".        els
+00017fc0: 653a 0a20 2020 2020 2020 2020 2020 206f  e:.            o
+00017fd0: 7574 5465 7874 203d 2022 4255 4c4c 4953  utText = "BULLIS
+00017fe0: 4822 0a20 2020 2020 2020 2020 2020 206f  H".            o
+00017ff0: 7574 203d 2028 0a20 2020 2020 2020 2020  ut = (.         
+00018000: 2020 2020 2020 2063 6f6c 6f72 5465 7874         colorText
+00018010: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
+00018020: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+00018030: 742e 4752 4545 4e0a 2020 2020 2020 2020  t.GREEN.        
+00018040: 2020 2020 2020 2020 2b20 6f75 7454 6578          + outTex
+00018050: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00018060: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+00018070: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+00018080: 2020 2b20 636f 6c6f 7254 6578 742e 424f    + colorText.BO
+00018090: 4c44 0a20 2020 2020 2020 2020 2020 2029  LD.            )
+000180a0: 0a20 2020 2020 2020 2020 2020 2073 7567  .            sug
+000180b0: 203d 2022 5374 6179 2042 756c 6c69 7368   = "Stay Bullish
+000180c0: 2122 0a20 2020 2020 2020 2069 6620 504b  !".        if PK
+000180d0: 4461 7465 5574 696c 6974 6965 732e 6973  DateUtilities.is
+000180e0: 436c 6f73 696e 6748 6f75 7228 293a 0a20  ClosingHour():. 
+000180f0: 2020 2020 2020 2020 2020 204f 7574 7075             Outpu
+00018100: 7443 6f6e 7472 6f6c 7328 292e 7072 696e  tControls().prin
+00018110: 744f 7574 7075 7428 0a20 2020 2020 2020  tOutput(.       
+00018120: 2020 2020 2020 2020 2063 6f6c 6f72 5465           colorTe
+00018130: 7874 2e42 4f4c 440a 2020 2020 2020 2020  xt.BOLD.        
+00018140: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00018150: 6578 742e 5741 524e 0a20 2020 2020 2020  ext.WARN.       
+00018160: 2020 2020 2020 2020 202b 2022 4e6f 7465           + "Note
+00018170: 3a20 5468 6520 4149 2070 7265 6469 6374  : The AI predict
+00018180: 696f 6e20 7368 6f75 6c64 2062 6520 6578  ion should be ex
+00018190: 6563 7574 6564 2041 6674 6572 2033 2050  ecuted After 3 P
+000181a0: 4d20 6f72 204e 6561 7220 746f 2043 6c6f  M or Near to Clo
+000181b0: 7369 6e67 2074 696d 6520 6173 2074 6865  sing time as the
+000181c0: 2050 7265 6469 6374 696f 6e20 4163 6375   Prediction Accu
+000181d0: 7261 6379 2069 7320 6261 7365 6420 6f6e  racy is based on
+000181e0: 2074 6865 2043 6c6f 7369 6e67 2070 7269   the Closing pri
+000181f0: 6365 2122 0a20 2020 2020 2020 2020 2020  ce!".           
+00018200: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+00018210: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
+00018220: 2029 0a20 2020 2020 2020 2070 7265 6469   ).        predi
+00018230: 6374 696f 6e54 6578 7420 3d20 224d 6172  ctionText = "Mar
+00018240: 6b65 7420 6d61 7920 4f70 656e 207b 7d20  ket may Open {} 
+00018250: 6e65 7874 2064 6179 2120 7b7d 222e 666f  next day! {}".fo
+00018260: 726d 6174 286f 7574 2c20 7375 6729 0a20  rmat(out, sug). 
+00018270: 2020 2020 2020 2073 7472 656e 6774 6854         strengthT
+00018280: 6578 7420 3d20 2250 726f 6261 6269 6c69  ext = "Probabili
+00018290: 7479 2f53 7472 656e 6774 6820 6f66 2050  ty/Strength of P
+000182a0: 7265 6469 6374 696f 6e20 3d20 7b7d 2522  rediction = {}%"
+000182b0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
+000182c0: 2020 2020 2055 7469 6c69 7479 2e74 6f6f       Utility.too
+000182d0: 6c73 2e67 6574 5369 676d 6f69 6443 6f6e  ls.getSigmoidCon
+000182e0: 6669 6465 6e63 6528 7072 6564 5b30 5d29  fidence(pred[0])
+000182f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00018300: 2020 204f 7574 7075 7443 6f6e 7472 6f6c     OutputControl
+00018310: 7328 292e 7072 696e 744f 7574 7075 7428  s().printOutput(
+00018320: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+00018330: 6f72 5465 7874 2e42 4f4c 440a 2020 2020  orText.BOLD.    
+00018340: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00018350: 6578 742e 424c 5545 0a20 2020 2020 2020  ext.BLUE.       
+00018360: 2020 2020 202b 2022 5c6e 220a 2020 2020       + "\n".    
+00018370: 2020 2020 2020 2020 2b20 225b 2b5d 204e          + "[+] N
+00018380: 6966 7479 2041 4920 5072 6564 6963 7469  ifty AI Predicti
+00018390: 6f6e 202d 3e20 220a 2020 2020 2020 2020  on -> ".        
+000183a0: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+000183b0: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
+000183c0: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
+000183d0: 0a20 2020 2020 2020 2020 2020 202b 2070  .            + p
+000183e0: 7265 6469 6374 696f 6e54 6578 740a 2020  redictionText.  
+000183f0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+00018400: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+00018410: 2020 290a 2020 2020 2020 2020 4f75 7470    ).        Outp
+00018420: 7574 436f 6e74 726f 6c73 2829 2e70 7269  utControls().pri
+00018430: 6e74 4f75 7470 7574 280a 2020 2020 2020  ntOutput(.      
+00018440: 2020 2020 2020 636f 6c6f 7254 6578 742e        colorText.
+00018450: 424f 4c44 0a20 2020 2020 2020 2020 2020  BOLD.           
+00018460: 202b 2063 6f6c 6f72 5465 7874 2e42 4c55   + colorText.BLU
+00018470: 450a 2020 2020 2020 2020 2020 2020 2b20  E.            + 
+00018480: 225c 6e22 0a20 2020 2020 2020 2020 2020  "\n".           
+00018490: 202b 2022 5b2b 5d20 4e69 6674 7920 4149   + "[+] Nifty AI
+000184a0: 2050 7265 6469 6374 696f 6e20 2d3e 2022   Prediction -> "
+000184b0: 0a20 2020 2020 2020 2020 2020 202b 2063  .            + c
+000184c0: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
+000184d0: 2020 2020 2020 2020 202b 2073 7472 656e           + stren
+000184e0: 6774 6854 6578 740a 2020 2020 2020 2020  gthText.        
+000184f0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00018500: 6e20 7072 6564 2c20 7072 6564 6963 7469  n pred, predicti
+00018510: 6f6e 5465 7874 2e72 6570 6c61 6365 286f  onText.replace(o
+00018520: 7574 2c20 6f75 7454 6578 7429 2c20 7374  ut, outText), st
+00018530: 7265 6e67 7468 5465 7874 0a0a 2020 2020  rengthText..    
+00018540: 6465 6620 6d6f 6e69 746f 7246 6976 6545  def monitorFiveE
+00018550: 6d61 2873 656c 662c 2066 6574 6368 6572  ma(self, fetcher
+00018560: 2c20 7265 7375 6c74 5f64 662c 206c 6173  , result_df, las
+00018570: 745f 7369 676e 616c 2c20 7269 736b 5f72  t_signal, risk_r
+00018580: 6577 6172 643d 3329 3a0a 2020 2020 2020  eward=3):.      
+00018590: 2020 636f 6c5f 6e61 6d65 7320 3d20 5b22    col_names = ["
+000185a0: 4869 6768 222c 2022 4c6f 7722 2c20 2243  High", "Low", "C
+000185b0: 6c6f 7365 222c 2022 3545 4d41 225d 0a20  lose", "5EMA"]. 
+000185c0: 2020 2020 2020 2064 6174 615f 6c69 7374         data_list
+000185d0: 203d 205b 226e 6966 7479 5f62 7579 222c   = ["nifty_buy",
+000185e0: 2022 6261 6e6b 6e69 6674 795f 6275 7922   "banknifty_buy"
+000185f0: 2c20 226e 6966 7479 5f73 656c 6c22 2c20  , "nifty_sell", 
+00018600: 2262 616e 6b6e 6966 7479 5f73 656c 6c22  "banknifty_sell"
+00018610: 5d0a 0a20 2020 2020 2020 2064 6174 615f  ]..        data_
+00018620: 7475 706c 6520 3d20 6665 7463 6865 722e  tuple = fetcher.
+00018630: 6665 7463 6846 6976 6545 6d61 4461 7461  fetchFiveEmaData
+00018640: 2829 0a20 2020 2020 2020 2066 6f72 2063  ().        for c
+00018650: 6e74 2069 6e20 7261 6e67 6528 6c65 6e28  nt in range(len(
+00018660: 6461 7461 5f74 7570 6c65 2929 3a0a 2020  data_tuple)):.  
+00018670: 2020 2020 2020 2020 2020 6420 3d20 6461            d = da
+00018680: 7461 5f74 7570 6c65 5b63 6e74 5d0a 2020  ta_tuple[cnt].  
+00018690: 2020 2020 2020 2020 2020 645b 2235 454d            d["5EM
+000186a0: 4122 5d20 3d20 706b 7461 6c69 622e 454d  A"] = pktalib.EM
+000186b0: 4128 645b 2243 6c6f 7365 225d 2c20 7469  A(d["Close"], ti
+000186c0: 6d65 7065 7269 6f64 3d35 290a 2020 2020  meperiod=5).    
+000186d0: 2020 2020 2020 2020 6420 3d20 645b 636f          d = d[co
+000186e0: 6c5f 6e61 6d65 735d 0a20 2020 2020 2020  l_names].       
+000186f0: 2020 2020 2064 203d 2064 2e64 726f 706e       d = d.dropn
+00018700: 6128 292e 726f 756e 6428 3229 0a0a 2020  a().round(2)..  
+00018710: 2020 2020 2020 2020 2020 7769 7468 2053            with S
+00018720: 7570 7072 6573 734f 7574 7075 7428 7375  uppressOutput(su
+00018730: 7070 7265 7373 5f73 7464 6572 723d 5472  ppress_stderr=Tr
+00018740: 7565 2c20 7375 7070 7265 7373 5f73 7464  ue, suppress_std
+00018750: 6f75 743d 5472 7565 293a 0a20 2020 2020  out=True):.     
+00018760: 2020 2020 2020 2020 2020 2069 6620 2273             if "s
+00018770: 656c 6c22 2069 6e20 6461 7461 5f6c 6973  ell" in data_lis
+00018780: 745b 636e 745d 3a0a 2020 2020 2020 2020  t[cnt]:.        
+00018790: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+000187a0: 6368 6564 203d 2064 5b28 642e 4c6f 7720  ched = d[(d.Low 
+000187b0: 3e20 645b 2235 454d 4122 5d29 2026 2028  > d["5EMA"]) & (
+000187c0: 642e 4c6f 7720 2d20 645b 2235 454d 4122  d.Low - d["5EMA"
+000187d0: 5d20 3e20 302e 3529 5d0a 2020 2020 2020  ] > 0.5)].      
+000187e0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+000187f0: 7265 6368 6564 5b22 534c 225d 203d 2073  reched["SL"] = s
+00018800: 7472 6563 6865 642e 4869 6768 0a20 2020  treched.High.   
+00018810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018820: 2076 616c 6964 6174 6520 3d20 645b 0a20   validate = d[. 
+00018830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018840: 2020 2020 2020 2028 642e 4c6f 772e 7368         (d.Low.sh
+00018850: 6966 7428 3129 203e 2064 5b22 3545 4d41  ift(1) > d["5EMA
+00018860: 225d 2e73 6869 6674 2831 2929 0a20 2020  "].shift(1)).   
+00018870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018880: 2020 2020 2026 2028 642e 4c6f 772e 7368       & (d.Low.sh
+00018890: 6966 7428 3129 202d 2064 5b22 3545 4d41  ift(1) - d["5EMA
+000188a0: 225d 2e73 6869 6674 2831 2920 3e20 302e  "].shift(1) > 0.
+000188b0: 3529 0a20 2020 2020 2020 2020 2020 2020  5).             
+000188c0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+000188d0: 2020 2020 2020 2020 2020 2020 206f 6c64               old
+000188e0: 5f69 6e64 6578 203d 2076 616c 6964 6174  _index = validat
+000188f0: 652e 696e 6465 780a 2020 2020 2020 2020  e.index.        
+00018900: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00018910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018920: 2020 6d61 736b 203d 2028 642e 4869 6768    mask = (d.High
+00018930: 203c 2064 5b22 3545 4d41 225d 2920 2620   < d["5EMA"]) & 
+00018940: 2864 5b22 3545 4d41 225d 202d 2064 2e48  (d["5EMA"] - d.H
+00018950: 6967 6820 3e20 302e 3529 2020 2320 4275  igh > 0.5)  # Bu
+00018960: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+00018970: 2020 2020 2020 7374 7265 6368 6564 203d        streched =
+00018980: 2064 5b6d 6173 6b5d 0a20 2020 2020 2020   d[mask].       
+00018990: 2020 2020 2020 2020 2020 2020 2073 7472               str
+000189a0: 6563 6865 645b 2253 4c22 5d20 3d20 7374  eched["SL"] = st
+000189b0: 7265 6368 6564 2e4c 6f77 0a20 2020 2020  reched.Low.     
+000189c0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+000189d0: 616c 6964 6174 6520 3d20 642e 6c6f 635b  alidate = d.loc[
+000189e0: 6d61 736b 2e73 6869 6674 2831 292e 6669  mask.shift(1).fi
+000189f0: 6c6c 6e61 2846 616c 7365 295d 0a20 2020  llna(False)].   
+00018a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a10: 206f 6c64 5f69 6e64 6578 203d 2076 616c   old_index = val
+00018a20: 6964 6174 652e 696e 6465 780a 2020 2020  idate.index.    
+00018a30: 2020 2020 2020 2020 7467 7420 3d20 7064          tgt = pd
+00018a40: 2e44 6174 6146 7261 6d65 280a 2020 2020  .DataFrame(.    
+00018a50: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
+00018a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a70: 2020 7661 6c69 6461 7465 2e43 6c6f 7365    validate.Close
+00018a80: 2e72 6573 6574 5f69 6e64 6578 2864 726f  .reset_index(dro
+00018a90: 703d 5472 7565 290a 2020 2020 2020 2020  p=True).        
+00018aa0: 2020 2020 2020 2020 2020 2020 2d20 280a              - (.
 00018ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ac0: 2020 2020 2020 2020 2020 2020 7374 7265              stre
-00018ad0: 6368 6564 2e53 4c2e 7265 7365 745f 696e  ched.SL.reset_in
-00018ae0: 6465 7828 6472 6f70 3d54 7275 6529 0a20  dex(drop=True). 
-00018af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b00: 2020 2020 2020 2020 2020 202d 2076 616c             - val
-00018b10: 6964 6174 652e 436c 6f73 652e 7265 7365  idate.Close.rese
-00018b20: 745f 696e 6465 7828 6472 6f70 3d54 7275  t_index(drop=Tru
-00018b30: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00018b40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00018ac0: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
+00018ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ae0: 2020 2020 2020 7374 7265 6368 6564 2e53        streched.S
+00018af0: 4c2e 7265 7365 745f 696e 6465 7828 6472  L.reset_index(dr
+00018b00: 6f70 3d54 7275 6529 0a20 2020 2020 2020  op=True).       
+00018b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b20: 2020 2020 202d 2076 616c 6964 6174 652e       - validate.
+00018b30: 436c 6f73 652e 7265 7365 745f 696e 6465  Close.reset_inde
+00018b40: 7828 6472 6f70 3d54 7275 6529 0a20 2020  x(drop=True).   
 00018b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b60: 2020 2020 202a 2072 6973 6b5f 7265 7761       * risk_rewa
-00018b70: 7264 0a20 2020 2020 2020 2020 2020 2020  rd.             
-00018b80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00018b90: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00018ba0: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-00018bb0: 6d6e 733d 5b22 5461 7267 6574 225d 2c0a  mns=["Target"],.
-00018bc0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00018bd0: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
-00018be0: 7465 203d 2070 642e 636f 6e63 6174 280a  te = pd.concat(.
-00018bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c00: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00018c10: 2020 2020 2020 7661 6c69 6461 7465 2e72        validate.r
-00018c20: 6573 6574 5f69 6e64 6578 2864 726f 703d  eset_index(drop=
-00018c30: 5472 7565 292c 0a20 2020 2020 2020 2020  True),.         
-00018c40: 2020 2020 2020 2020 2020 2073 7472 6563             strec
-00018c50: 6865 645b 2253 4c22 5d2e 7265 7365 745f  hed["SL"].reset_
-00018c60: 696e 6465 7828 6472 6f70 3d54 7275 6529  index(drop=True)
-00018c70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018c80: 2020 2020 2020 7467 742c 0a20 2020 2020        tgt,.     
-00018c90: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
-00018ca0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-00018cb0: 6973 3d31 2c0a 2020 2020 2020 2020 2020  is=1,.          
-00018cc0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00018cd0: 7661 6c69 6461 7465 203d 2076 616c 6964  validate = valid
-00018ce0: 6174 652e 7461 696c 286c 656e 286f 6c64  ate.tail(len(old
-00018cf0: 5f69 6e64 6578 2929 0a20 2020 2020 2020  _index)).       
-00018d00: 2020 2020 2076 616c 6964 6174 6520 3d20       validate = 
-00018d10: 7661 6c69 6461 7465 2e73 6574 5f69 6e64  validate.set_ind
-00018d20: 6578 286f 6c64 5f69 6e64 6578 290a 2020  ex(old_index).  
-00018d30: 2020 2020 2020 2020 2020 6966 2022 7365            if "se
-00018d40: 6c6c 2220 696e 2064 6174 615f 6c69 7374  ll" in data_list
-00018d50: 5b63 6e74 5d3a 0a20 2020 2020 2020 2020  [cnt]:.         
-00018d60: 2020 2020 2020 2066 696e 616c 203d 2076         final = v
-00018d70: 616c 6964 6174 655b 7661 6c69 6461 7465  alidate[validate
-00018d80: 2e43 6c6f 7365 203c 2076 616c 6964 6174  .Close < validat
-00018d90: 655b 2235 454d 4122 5d5d 2e74 6169 6c28  e["5EMA"]].tail(
-00018da0: 3129 0a20 2020 2020 2020 2020 2020 2065  1).            e
-00018db0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00018dc0: 2020 2020 2066 696e 616c 203d 2076 616c       final = val
-00018dd0: 6964 6174 655b 7661 6c69 6461 7465 2e43  idate[validate.C
-00018de0: 6c6f 7365 203e 2076 616c 6964 6174 655b  lose > validate[
-00018df0: 2235 454d 4122 5d5d 2e74 6169 6c28 3129  "5EMA"]].tail(1)
-00018e00: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00018e10: 2064 6174 615f 6c69 7374 5b63 6e74 5d20   data_list[cnt] 
-00018e20: 6e6f 7420 696e 206c 6173 745f 7369 676e  not in last_sign
-00018e30: 616c 3a0a 2020 2020 2020 2020 2020 2020  al:.            
-00018e40: 2020 2020 6c61 7374 5f73 6967 6e61 6c5b      last_signal[
-00018e50: 6461 7461 5f6c 6973 745b 636e 745d 5d20  data_list[cnt]] 
-00018e60: 3d20 6669 6e61 6c0a 2020 2020 2020 2020  = final.        
-00018e70: 2020 2020 656c 6966 2064 6174 615f 6c69      elif data_li
-00018e80: 7374 5b63 6e74 5d20 696e 206c 6173 745f  st[cnt] in last_
-00018e90: 7369 676e 616c 3a0a 2020 2020 2020 2020  signal:.        
-00018ea0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00018eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ec0: 2063 6f6e 6469 7469 6f6e 203d 206c 6173   condition = las
-00018ed0: 745f 7369 676e 616c 5b64 6174 615f 6c69  t_signal[data_li
-00018ee0: 7374 5b63 6e74 5d5d 5b30 5d5b 2253 4c22  st[cnt]][0]["SL"
-00018ef0: 5d5b 305d 0a20 2020 2020 2020 2020 2020  ][0].           
-00018f00: 2020 2020 2065 7863 6570 7420 4b65 7945       except KeyE
-00018f10: 7272 6f72 2061 7320 653a 2023 2070 7261  rror as e: # pra
-00018f20: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-00018f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f40: 2020 7365 6c66 2e64 6566 6175 6c74 5f6c    self.default_l
-00018f50: 6f67 6765 722e 6465 6275 6728 652c 2065  ogger.debug(e, e
-00018f60: 7863 5f69 6e66 6f3d 5472 7565 290a 2020  xc_info=True).  
-00018f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f80: 2020 636f 6e64 6974 696f 6e20 3d20 6c61    condition = la
-00018f90: 7374 5f73 6967 6e61 6c5b 6461 7461 5f6c  st_signal[data_l
-00018fa0: 6973 745b 636e 745d 5d5b 2253 4c22 5d5b  ist[cnt]]["SL"][
-00018fb0: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
-00018fc0: 2020 2023 2069 6620 6c61 7374 5f73 6967     # if last_sig
-00018fd0: 6e61 6c5b 6461 7461 5f6c 6973 745b 636e  nal[data_list[cn
-00018fe0: 745d 5d20 6973 206e 6f74 2066 696e 616c  t]] is not final
-00018ff0: 3a20 2020 2020 2020 2020 2023 2044 6562  :          # Deb
-00019000: 7567 202d 2053 686f 7773 2061 6c6c 2063  ug - Shows all c
-00019010: 6f6e 6469 7469 6f6e 730a 2020 2020 2020  onditions.      
-00019020: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-00019030: 2866 696e 616c 5b22 534c 225d 2920 3e20  (final["SL"]) > 
-00019040: 3020 616e 6420 636f 6e64 6974 696f 6e20  0 and condition 
-00019050: 213d 2066 696e 616c 5b22 534c 225d 2e69  != final["SL"].i
-00019060: 6c6f 635b 305d 3a0a 2020 2020 2020 2020  loc[0]:.        
-00019070: 2020 2020 2020 2020 2020 2020 2320 446f              # Do
-00019080: 2073 6f6d 6574 6869 6e67 2077 6974 6820   something with 
-00019090: 7265 7375 6c74 730a 2020 2020 2020 2020  results.        
-000190a0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000190b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000190c0: 2020 2020 2020 2020 2072 6573 756c 745f           result_
-000190d0: 6466 203d 2070 642e 636f 6e63 6174 280a  df = pd.concat(.
-000190e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190f0: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+00018b60: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00018b70: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+00018b80: 2072 6973 6b5f 7265 7761 7264 0a20 2020   risk_reward.   
+00018b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ba0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00018bb0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+00018bc0: 2020 2020 2020 636f 6c75 6d6e 733d 5b22        columns=["
+00018bd0: 5461 7267 6574 225d 2c0a 2020 2020 2020  Target"],.      
+00018be0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00018bf0: 2020 2020 7661 6c69 6461 7465 203d 2070      validate = p
+00018c00: 642e 636f 6e63 6174 280a 2020 2020 2020  d.concat(.      
+00018c10: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
+00018c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c30: 7661 6c69 6461 7465 2e72 6573 6574 5f69  validate.reset_i
+00018c40: 6e64 6578 2864 726f 703d 5472 7565 292c  ndex(drop=True),
+00018c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018c60: 2020 2020 2073 7472 6563 6865 645b 2253       streched["S
+00018c70: 4c22 5d2e 7265 7365 745f 696e 6465 7828  L"].reset_index(
+00018c80: 6472 6f70 3d54 7275 6529 2c0a 2020 2020  drop=True),.    
+00018c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ca0: 7467 742c 0a20 2020 2020 2020 2020 2020  tgt,.           
+00018cb0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00018cc0: 2020 2020 2020 2020 6178 6973 3d31 2c0a          axis=1,.
+00018cd0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00018ce0: 2020 2020 2020 2020 2020 7661 6c69 6461            valida
+00018cf0: 7465 203d 2076 616c 6964 6174 652e 7461  te = validate.ta
+00018d00: 696c 286c 656e 286f 6c64 5f69 6e64 6578  il(len(old_index
+00018d10: 2929 0a20 2020 2020 2020 2020 2020 2076  )).            v
+00018d20: 616c 6964 6174 6520 3d20 7661 6c69 6461  alidate = valida
+00018d30: 7465 2e73 6574 5f69 6e64 6578 286f 6c64  te.set_index(old
+00018d40: 5f69 6e64 6578 290a 2020 2020 2020 2020  _index).        
+00018d50: 2020 2020 6966 2022 7365 6c6c 2220 696e      if "sell" in
+00018d60: 2064 6174 615f 6c69 7374 5b63 6e74 5d3a   data_list[cnt]:
+00018d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018d80: 2066 696e 616c 203d 2076 616c 6964 6174   final = validat
+00018d90: 655b 7661 6c69 6461 7465 2e43 6c6f 7365  e[validate.Close
+00018da0: 203c 2076 616c 6964 6174 655b 2235 454d   < validate["5EM
+00018db0: 4122 5d5d 2e74 6169 6c28 3129 0a20 2020  A"]].tail(1).   
+00018dc0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00018dd0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00018de0: 696e 616c 203d 2076 616c 6964 6174 655b  inal = validate[
+00018df0: 7661 6c69 6461 7465 2e43 6c6f 7365 203e  validate.Close >
+00018e00: 2076 616c 6964 6174 655b 2235 454d 4122   validate["5EMA"
+00018e10: 5d5d 2e74 6169 6c28 3129 0a0a 2020 2020  ]].tail(1)..    
+00018e20: 2020 2020 2020 2020 6966 2064 6174 615f          if data_
+00018e30: 6c69 7374 5b63 6e74 5d20 6e6f 7420 696e  list[cnt] not in
+00018e40: 206c 6173 745f 7369 676e 616c 3a0a 2020   last_signal:.  
+00018e50: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+00018e60: 7374 5f73 6967 6e61 6c5b 6461 7461 5f6c  st_signal[data_l
+00018e70: 6973 745b 636e 745d 5d20 3d20 6669 6e61  ist[cnt]] = fina
+00018e80: 6c0a 2020 2020 2020 2020 2020 2020 656c  l.            el
+00018e90: 6966 2064 6174 615f 6c69 7374 5b63 6e74  if data_list[cnt
+00018ea0: 5d20 696e 206c 6173 745f 7369 676e 616c  ] in last_signal
+00018eb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018ec0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00018ed0: 2020 2020 2020 2020 2020 2063 6f6e 6469             condi
+00018ee0: 7469 6f6e 203d 206c 6173 745f 7369 676e  tion = last_sign
+00018ef0: 616c 5b64 6174 615f 6c69 7374 5b63 6e74  al[data_list[cnt
+00018f00: 5d5d 5b30 5d5b 2253 4c22 5d5b 305d 0a20  ]][0]["SL"][0]. 
+00018f10: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00018f20: 7863 6570 7420 4b65 7945 7272 6f72 2061  xcept KeyError a
+00018f30: 7320 653a 2023 2070 7261 676d 613a 206e  s e: # pragma: n
+00018f40: 6f20 636f 7665 720a 2020 2020 2020 2020  o cover.        
+00018f50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018f60: 2e64 6566 6175 6c74 5f6c 6f67 6765 722e  .default_logger.
+00018f70: 6465 6275 6728 652c 2065 7863 5f69 6e66  debug(e, exc_inf
+00018f80: 6f3d 5472 7565 290a 2020 2020 2020 2020  o=True).        
+00018f90: 2020 2020 2020 2020 2020 2020 636f 6e64              cond
+00018fa0: 6974 696f 6e20 3d20 6c61 7374 5f73 6967  ition = last_sig
+00018fb0: 6e61 6c5b 6461 7461 5f6c 6973 745b 636e  nal[data_list[cn
+00018fc0: 745d 5d5b 2253 4c22 5d5b 305d 0a20 2020  t]]["SL"][0].   
+00018fd0: 2020 2020 2020 2020 2020 2020 2023 2069               # i
+00018fe0: 6620 6c61 7374 5f73 6967 6e61 6c5b 6461  f last_signal[da
+00018ff0: 7461 5f6c 6973 745b 636e 745d 5d20 6973  ta_list[cnt]] is
+00019000: 206e 6f74 2066 696e 616c 3a20 2020 2020   not final:     
+00019010: 2020 2020 2023 2044 6562 7567 202d 2053       # Debug - S
+00019020: 686f 7773 2061 6c6c 2063 6f6e 6469 7469  hows all conditi
+00019030: 6f6e 730a 2020 2020 2020 2020 2020 2020  ons.            
+00019040: 2020 2020 6966 206c 656e 2866 696e 616c      if len(final
+00019050: 5b22 534c 225d 2920 3e20 3020 616e 6420  ["SL"]) > 0 and 
+00019060: 636f 6e64 6974 696f 6e20 213d 2066 696e  condition != fin
+00019070: 616c 5b22 534c 225d 2e69 6c6f 635b 305d  al["SL"].iloc[0]
+00019080: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00019090: 2020 2020 2020 2320 446f 2073 6f6d 6574        # Do somet
+000190a0: 6869 6e67 2077 6974 6820 7265 7375 6c74  hing with result
+000190b0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+000190c0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+000190d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190e0: 2020 2072 6573 756c 745f 6466 203d 2070     result_df = p
+000190f0: 642e 636f 6e63 6174 280a 2020 2020 2020  d.concat(.      
 00019100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019110: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00019120: 7375 6c74 5f64 662c 0a20 2020 2020 2020  sult_df,.       
-00019130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019140: 2020 2020 2020 2020 2070 642e 4461 7461           pd.Data
-00019150: 4672 616d 6528 0a20 2020 2020 2020 2020  Frame(.         
-00019160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019170: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+00019110: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00019120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019130: 2020 2020 2020 2020 7265 7375 6c74 5f64          result_d
+00019140: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+00019150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019160: 2020 2070 642e 4461 7461 4672 616d 6528     pd.DataFrame(
+00019170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00019180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191a0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
-000191b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191d0: 2020 2063 6f6c 6f72 5465 7874 2e42 4c55     colorText.BLU
-000191e0: 450a 2020 2020 2020 2020 2020 2020 2020  E.              
-000191f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019200: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00019210: 7374 7228 6669 6e61 6c2e 696e 6465 785b  str(final.index[
-00019220: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-00019230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019190: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+000191a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191b0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+000191c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000191d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191e0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+000191f0: 6f72 5465 7874 2e42 4c55 450a 2020 2020  orText.BLUE.    
+00019200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019220: 2020 2020 2020 2020 2b20 7374 7228 6669          + str(fi
+00019230: 6e61 6c2e 696e 6465 785b 305d 290a 2020  nal.index[0]).  
 00019240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019250: 2b20 636f 6c6f 7254 6578 742e 454e 442c  + colorText.END,
-00019260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019280: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-00019290: 6f72 5465 7874 2e42 4f4c 440a 2020 2020  orText.BOLD.    
-000192a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192c0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-000192d0: 6578 742e 5741 524e 0a20 2020 2020 2020  ext.WARN.       
-000192e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019300: 2020 2020 202b 2064 6174 615f 6c69 7374       + data_list
-00019310: 5b63 6e74 5d2e 7370 6c69 7428 225f 2229  [cnt].split("_")
-00019320: 5b30 5d2e 7570 7065 7228 290a 2020 2020  [0].upper().    
-00019330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019350: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-00019360: 6578 742e 454e 442c 0a20 2020 2020 2020  ext.END,.       
-00019370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019390: 2020 2020 2028 0a20 2020 2020 2020 2020       (.         
-000193a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193c0: 2020 2020 2020 2063 6f6c 6f72 5465 7874         colorText
-000193d0: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
-000193e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019260: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+00019270: 7254 6578 742e 454e 442c 0a20 2020 2020  rText.END,.     
+00019280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192a0: 2020 2020 2020 2063 6f6c 6f72 5465 7874         colorText
+000192b0: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
+000192c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192e0: 2020 2b20 636f 6c6f 7254 6578 742e 5741    + colorText.WA
+000192f0: 524e 0a20 2020 2020 2020 2020 2020 2020  RN.             
+00019300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019310: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00019320: 2064 6174 615f 6c69 7374 5b63 6e74 5d2e   data_list[cnt].
+00019330: 7370 6c69 7428 225f 2229 5b30 5d2e 7570  split("_")[0].up
+00019340: 7065 7228 290a 2020 2020 2020 2020 2020  per().          
+00019350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019370: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+00019380: 442c 0a20 2020 2020 2020 2020 2020 2020  D,.             
+00019390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193a0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+000193b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000193c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193e0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440a   colorText.BOLD.
 000193f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019400: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-00019410: 742e 4641 494c 0a20 2020 2020 2020 2020  t.FAIL.         
-00019420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019440: 2020 2020 2020 202b 2064 6174 615f 6c69         + data_li
-00019450: 7374 5b63 6e74 5d2e 7370 6c69 7428 225f  st[cnt].split("_
-00019460: 2229 5b31 5d2e 7570 7065 7228 290a 2020  ")[1].upper().  
-00019470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019490: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000194a0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-000194b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194d0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00019400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019420: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
+00019430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019460: 202b 2064 6174 615f 6c69 7374 5b63 6e74   + data_list[cnt
+00019470: 5d2e 7370 6c69 7428 225f 2229 5b31 5d2e  ].split("_")[1].
+00019480: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
+00019490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194b0: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+000194c0: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+000194d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000194e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019500: 2020 2020 2020 2020 6966 2022 7365 6c6c          if "sell
-00019510: 2220 696e 2064 6174 615f 6c69 7374 5b63  " in data_list[c
-00019520: 6e74 5d0a 2020 2020 2020 2020 2020 2020  nt].            
-00019530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194f0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00019500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019520: 2020 6966 2022 7365 6c6c 2220 696e 2064    if "sell" in d
+00019530: 6174 615f 6c69 7374 5b63 6e74 5d0a 2020  ata_list[cnt].  
 00019540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019550: 656c 7365 2028 0a20 2020 2020 2020 2020  else (.         
-00019560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019580: 2020 2020 2020 2063 6f6c 6f72 5465 7874         colorText
-00019590: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
-000195a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019560: 2020 2020 2020 2020 2020 656c 7365 2028            else (
+00019570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195a0: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440a   colorText.BOLD.
 000195b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195c0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-000195d0: 742e 4752 4545 4e0a 2020 2020 2020 2020  t.GREEN.        
-000195e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019600: 2020 2020 2020 2020 2b20 6461 7461 5f6c          + data_l
-00019610: 6973 745b 636e 745d 2e73 706c 6974 2822  ist[cnt].split("
-00019620: 5f22 295b 315d 2e75 7070 6572 2829 0a20  _")[1].upper(). 
-00019630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019650: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-00019660: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
-00019670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019690: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+000195c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195e0: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+000195f0: 4e0a 2020 2020 2020 2020 2020 2020 2020  N.              
+00019600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019620: 2020 2b20 6461 7461 5f6c 6973 745b 636e    + data_list[cn
+00019630: 745d 2e73 706c 6974 2822 5f22 295b 315d  t].split("_")[1]
+00019640: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
+00019650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019670: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+00019680: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+00019690: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000196a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196c0: 2020 2020 2020 2020 2020 636f 6c6f 7254            colorT
-000196d0: 6578 742e 4641 494c 0a20 2020 2020 2020  ext.FAIL.       
-000196e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019700: 2020 2020 202b 2073 7472 2866 696e 616c       + str(final
-00019710: 2e53 4c5b 305d 290a 2020 2020 2020 2020  .SL[0]).        
-00019720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019740: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-00019750: 454e 442c 0a20 2020 2020 2020 2020 2020  END,.           
-00019760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196b0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+000196c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196e0: 2020 2020 636f 6c6f 7254 6578 742e 4641      colorText.FA
+000196f0: 494c 0a20 2020 2020 2020 2020 2020 2020  IL.             
+00019700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019710: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00019720: 2073 7472 2866 696e 616c 2e53 4c5b 305d   str(final.SL[0]
+00019730: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019750: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00019760: 636f 6c6f 7254 6578 742e 454e 442c 0a20  colorText.END,. 
 00019770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019780: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
-00019790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000197a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197b0: 2020 2020 2020 2020 2020 2020 202b 2073               + s
-000197c0: 7472 2866 696e 616c 2e54 6172 6765 745b  tr(final.Target[
-000197d0: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-000197e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019790: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+000197a0: 5465 7874 2e47 5245 454e 0a20 2020 2020  Text.GREEN.     
+000197b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197d0: 2020 2020 2020 202b 2073 7472 2866 696e         + str(fin
+000197e0: 616c 2e54 6172 6765 745b 305d 290a 2020  al.Target[0]).  
 000197f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019800: 2b20 636f 6c6f 7254 6578 742e 454e 442c  + colorText.END,
-00019810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019830: 2020 2020 2020 2020 2020 2020 2066 2231               f"1
-00019840: 3a7b 7269 736b 5f72 6577 6172 647d 222c  :{risk_reward}",
-00019850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019870: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00019800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019810: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+00019820: 7254 6578 742e 454e 442c 0a20 2020 2020  rText.END,.     
+00019830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019850: 2020 2020 2020 2066 2231 3a7b 7269 736b         f"1:{risk
+00019860: 5f72 6577 6172 647d 222c 0a20 2020 2020  _reward}",.     
+00019870: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019890: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-000198a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000198b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198c0: 2020 2020 2020 636f 6c75 6d6e 733d 7265        columns=re
-000198d0: 7375 6c74 5f64 662e 636f 6c75 6d6e 732c  sult_df.columns,
-000198e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000198f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019900: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00019910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019920: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00019930: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00019940: 7869 733d 302c 0a20 2020 2020 2020 2020  xis=0,.         
-00019950: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00019890: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+000198a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198b0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+000198c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198e0: 636f 6c75 6d6e 733d 7265 7375 6c74 5f64  columns=result_d
+000198f0: 662e 636f 6c75 6d6e 732c 0a20 2020 2020  f.columns,.     
+00019900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019910: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+00019920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019930: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00019940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019950: 2020 2020 2020 2020 2061 7869 733d 302c           axis=0,
 00019960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019970: 2020 2020 2020 2020 2072 6573 756c 745f           result_
-00019980: 6466 2e72 6573 6574 5f69 6e64 6578 2864  df.reset_index(d
-00019990: 726f 703d 5472 7565 2c20 696e 706c 6163  rop=True, inplac
-000199a0: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
-000199b0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-000199c0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-000199d0: 653a 2020 2320 7072 6167 6d61 3a20 6e6f  e:  # pragma: no
-000199e0: 2063 6f76 6572 0a20 2020 2020 2020 2020   cover.         
-000199f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019a00: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
-00019a10: 6572 2e64 6562 7567 2865 2c20 6578 635f  er.debug(e, exc_
-00019a20: 696e 666f 3d54 7275 6529 0a20 2020 2020  info=True).     
-00019a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a40: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-00019a50: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-00019a60: 656e 2075 7064 6174 650a 2020 2020 2020  en update.      
-00019a70: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00019a80: 7374 5f73 6967 6e61 6c5b 6461 7461 5f6c  st_signal[data_l
-00019a90: 6973 745b 636e 745d 5d20 3d20 5b66 696e  ist[cnt]] = [fin
-00019aa0: 616c 5d0a 2020 2020 2020 2020 6966 2072  al].        if r
-00019ab0: 6573 756c 745f 6466 2069 7320 6e6f 7420  esult_df is not 
-00019ac0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00019ad0: 2020 7265 7375 6c74 5f64 662e 6472 6f70    result_df.drop
-00019ae0: 5f64 7570 6c69 6361 7465 7328 6b65 6570  _duplicates(keep
-00019af0: 3d22 6c61 7374 222c 2069 6e70 6c61 6365  ="last", inplace
-00019b00: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00019b10: 2020 2072 6573 756c 745f 6466 2e73 6f72     result_df.sor
-00019b20: 745f 7661 6c75 6573 2862 793d 2254 696d  t_values(by="Tim
-00019b30: 6522 2c20 696e 706c 6163 653d 5472 7565  e", inplace=True
-00019b40: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00019b50: 2072 6573 756c 745f 6466 5b3a 3a2d 315d   result_df[::-1]
-00019b60: 0a0a 2020 2020 2320 5072 6570 726f 6365  ..    # Preproce
-00019b70: 7373 2074 6865 2061 6371 7569 7265 6420  ss the acquired 
-00019b80: 6461 7461 0a20 2020 2064 6566 2070 7265  data.    def pre
-00019b90: 7072 6f63 6573 7344 6174 6128 7365 6c66  processData(self
-00019ba0: 2c20 6466 2c20 6461 7973 546f 4c6f 6f6b  , df, daysToLook
-00019bb0: 6261 636b 3d4e 6f6e 6529 3a0a 2020 2020  back=None):.    
-00019bc0: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
-00019bd0: 7461 6e63 6528 6466 2c20 7064 2e44 6174  tance(df, pd.Dat
-00019be0: 6146 7261 6d65 290a 2020 2020 2020 2020  aFrame).        
-00019bf0: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
-00019c00: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00019c10: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00019c20: 2064 6174 612e 7265 706c 6163 6528 6e70   data.replace(np
-00019c30: 2e69 6e66 2c20 6e70 2e6e 616e 292e 7265  .inf, np.nan).re
-00019c40: 706c 6163 6528 2d6e 702e 696e 662c 206e  place(-np.inf, n
-00019c50: 702e 6e61 6e29 2e64 726f 706e 6128 686f  p.nan).dropna(ho
-00019c60: 773d 2261 6c6c 2229 0a20 2020 2020 2020  w="all").       
-00019c70: 2020 2020 2023 2073 656c 662e 6465 6661       # self.defa
-00019c80: 756c 745f 6c6f 6767 6572 2e69 6e66 6f28  ult_logger.info(
-00019c90: 6622 5072 6570 726f 6365 7373 696e 6720  f"Preprocessing 
-00019ca0: 6461 7461 3a5c 6e7b 6461 7461 2e68 6561  data:\n{data.hea
-00019cb0: 6428 3129 7d5c 6e22 290a 2020 2020 2020  d(1)}\n").      
-00019cc0: 2020 2020 2020 6966 2064 6179 7354 6f4c        if daysToL
-00019cd0: 6f6f 6b62 6163 6b20 6973 204e 6f6e 653a  ookback is None:
-00019ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019cf0: 2064 6179 7354 6f4c 6f6f 6b62 6163 6b20   daysToLookback 
-00019d00: 3d20 7365 6c66 2e63 6f6e 6669 674d 616e  = self.configMan
-00019d10: 6167 6572 2e64 6179 7354 6f4c 6f6f 6b62  ager.daysToLookb
-00019d20: 6163 6b0a 2020 2020 2020 2020 2020 2020  ack.            
-00019d30: 6966 2073 656c 662e 636f 6e66 6967 4d61  if self.configMa
-00019d40: 6e61 6765 722e 7573 6545 4d41 3a0a 2020  nager.useEMA:.  
-00019d50: 2020 2020 2020 2020 2020 2020 2020 736d                sm
-00019d60: 6120 3d20 706b 7461 6c69 622e 454d 4128  a = pktalib.EMA(
-00019d70: 6461 7461 5b22 436c 6f73 6522 5d2c 2074  data["Close"], t
-00019d80: 696d 6570 6572 696f 643d 3530 290a 2020  imeperiod=50).  
-00019d90: 2020 2020 2020 2020 2020 2020 2020 6c6d                lm
-00019da0: 6120 3d20 706b 7461 6c69 622e 454d 4128  a = pktalib.EMA(
-00019db0: 6461 7461 5b22 436c 6f73 6522 5d2c 2074  data["Close"], t
-00019dc0: 696d 6570 6572 696f 643d 3230 3029 0a20  imeperiod=200). 
-00019dd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019de0: 736d 6120 3d20 706b 7461 6c69 622e 454d  sma = pktalib.EM
-00019df0: 4128 6461 7461 5b22 436c 6f73 6522 5d2c  A(data["Close"],
-00019e00: 2074 696d 6570 6572 696f 643d 3929 0a20   timeperiod=9). 
-00019e10: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00019e20: 6174 612e 696e 7365 7274 286c 656e 2864  ata.insert(len(d
-00019e30: 6174 612e 636f 6c75 6d6e 7329 2c20 2253  ata.columns), "S
-00019e40: 4d41 222c 2073 6d61 290a 2020 2020 2020  MA", sma).      
-00019e50: 2020 2020 2020 2020 2020 6461 7461 2e69            data.i
-00019e60: 6e73 6572 7428 6c65 6e28 6461 7461 2e63  nsert(len(data.c
-00019e70: 6f6c 756d 6e73 292c 2022 4c4d 4122 2c20  olumns), "LMA", 
-00019e80: 6c6d 6129 0a20 2020 2020 2020 2020 2020  lma).           
-00019e90: 2020 2020 2064 6174 612e 696e 7365 7274       data.insert
-00019ea0: 286c 656e 2864 6174 612e 636f 6c75 6d6e  (len(data.column
-00019eb0: 7329 2c20 2253 534d 4122 2c20 7373 6d61  s), "SSMA", ssma
-00019ec0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00019ed0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00019ee0: 2020 2020 736d 6120 3d20 706b 7461 6c69      sma = pktali
-00019ef0: 622e 534d 4128 6461 7461 5b22 436c 6f73  b.SMA(data["Clos
-00019f00: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
-00019f10: 3530 290a 2020 2020 2020 2020 2020 2020  50).            
-00019f20: 2020 2020 6c6d 6120 3d20 706b 7461 6c69      lma = pktali
-00019f30: 622e 534d 4128 6461 7461 5b22 436c 6f73  b.SMA(data["Clos
-00019f40: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
-00019f50: 3230 3029 0a20 2020 2020 2020 2020 2020  200).           
-00019f60: 2020 2020 2073 736d 6120 3d20 706b 7461       ssma = pkta
-00019f70: 6c69 622e 534d 4128 6461 7461 5b22 436c  lib.SMA(data["Cl
-00019f80: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
-00019f90: 643d 3929 0a20 2020 2020 2020 2020 2020  d=9).           
-00019fa0: 2020 2020 2064 6174 612e 696e 7365 7274       data.insert
-00019fb0: 286c 656e 2864 6174 612e 636f 6c75 6d6e  (len(data.column
-00019fc0: 7329 2c20 2253 4d41 222c 2073 6d61 290a  s), "SMA", sma).
-00019fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019fe0: 6461 7461 2e69 6e73 6572 7428 6c65 6e28  data.insert(len(
-00019ff0: 6461 7461 2e63 6f6c 756d 6e73 292c 2022  data.columns), "
-0001a000: 4c4d 4122 2c20 6c6d 6129 0a20 2020 2020  LMA", lma).     
-0001a010: 2020 2020 2020 2020 2020 2064 6174 612e             data.
-0001a020: 696e 7365 7274 286c 656e 2864 6174 612e  insert(len(data.
-0001a030: 636f 6c75 6d6e 7329 2c20 2253 534d 4122  columns), "SSMA"
-0001a040: 2c20 7373 6d61 290a 2020 2020 2020 2020  , ssma).        
-0001a050: 2020 2020 766f 6c20 3d20 706b 7461 6c69      vol = pktali
-0001a060: 622e 534d 4128 6461 7461 5b22 566f 6c75  b.SMA(data["Volu
-0001a070: 6d65 225d 2c20 7469 6d65 7065 7269 6f64  me"], timeperiod
-0001a080: 3d32 3029 0a20 2020 2020 2020 2020 2020  =20).           
-0001a090: 2072 7369 203d 2070 6b74 616c 6962 2e52   rsi = pktalib.R
-0001a0a0: 5349 2864 6174 615b 2243 6c6f 7365 225d  SI(data["Close"]
-0001a0b0: 2c20 7469 6d65 7065 7269 6f64 3d31 3429  , timeperiod=14)
-0001a0c0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0001a0d0: 612e 696e 7365 7274 286c 656e 2864 6174  a.insert(len(dat
-0001a0e0: 612e 636f 6c75 6d6e 7329 2c20 2256 6f6c  a.columns), "Vol
-0001a0f0: 4d41 222c 2076 6f6c 290a 2020 2020 2020  MA", vol).      
-0001a100: 2020 2020 2020 6461 7461 2e69 6e73 6572        data.inser
-0001a110: 7428 6c65 6e28 6461 7461 2e63 6f6c 756d  t(len(data.colum
-0001a120: 6e73 292c 2022 5253 4922 2c20 7273 6929  ns), "RSI", rsi)
-0001a130: 0a20 2020 2020 2020 2020 2020 2063 6369  .            cci
-0001a140: 203d 2070 6b74 616c 6962 2e43 4349 2864   = pktalib.CCI(d
-0001a150: 6174 615b 2248 6967 6822 5d2c 2064 6174  ata["High"], dat
-0001a160: 615b 224c 6f77 225d 2c20 6461 7461 5b22  a["Low"], data["
-0001a170: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
-0001a180: 696f 643d 3134 290a 2020 2020 2020 2020  iod=14).        
-0001a190: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
-0001a1a0: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
-0001a1b0: 292c 2022 4343 4922 2c20 6363 6929 0a20  ), "CCI", cci). 
-0001a1c0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0001a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1e0: 6661 7374 6b2c 2066 6173 7464 203d 2070  fastk, fastd = p
-0001a1f0: 6b74 616c 6962 2e53 544f 4348 5253 4928  ktalib.STOCHRSI(
-0001a200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a210: 2020 2020 2064 6174 615b 2243 6c6f 7365       data["Close
-0001a220: 225d 2c20 7469 6d65 7065 7269 6f64 3d31  "], timeperiod=1
-0001a230: 342c 2066 6173 746b 5f70 6572 696f 643d  4, fastk_period=
-0001a240: 352c 2066 6173 7464 5f70 6572 696f 643d  5, fastd_period=
-0001a250: 332c 2066 6173 7464 5f6d 6174 7970 653d  3, fastd_matype=
-0001a260: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-0001a270: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0001a280: 2020 2020 6461 7461 2e69 6e73 6572 7428      data.insert(
-0001a290: 6c65 6e28 6461 7461 2e63 6f6c 756d 6e73  len(data.columns
-0001a2a0: 292c 2022 4641 5354 4b22 2c20 6661 7374  ), "FASTK", fast
-0001a2b0: 6b29 0a20 2020 2020 2020 2020 2020 2020  k).             
-0001a2c0: 2020 2064 6174 612e 696e 7365 7274 286c     data.insert(l
-0001a2d0: 656e 2864 6174 612e 636f 6c75 6d6e 7329  en(data.columns)
-0001a2e0: 2c20 2246 4153 5444 222c 2066 6173 7464  , "FASTD", fastd
-0001a2f0: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
-0001a300: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-0001a310: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-0001a320: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
-0001a330: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
-0001a340: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
-0001a350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a360: 2070 6173 730a 2020 2020 2020 2020 6578   pass.        ex
-0001a370: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-0001a380: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-0001a390: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
-0001a3a0: 745f 6c6f 6767 6572 2e64 6562 7567 2865  t_logger.debug(e
-0001a3b0: 2c20 6578 635f 696e 666f 3d54 7275 6529  , exc_info=True)
-0001a3c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a3d0: 2070 6173 730a 2020 2020 2020 2020 6461   pass.        da
-0001a3e0: 7461 203d 2064 6174 615b 3a3a 2d31 5d20  ta = data[::-1] 
-0001a3f0: 2023 2052 6576 6572 7365 2074 6865 2064   # Reverse the d
-0001a400: 6174 6166 7261 6d65 0a20 2020 2020 2020  ataframe.       
-0001a410: 2023 2064 6174 6120 3d20 6461 7461 2e66   # data = data.f
-0001a420: 696c 6c6e 6128 3029 0a20 2020 2020 2020  illna(0).       
-0001a430: 2023 2064 6174 6120 3d20 6461 7461 2e72   # data = data.r
-0001a440: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
-0001a450: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
-0001a460: 2020 2020 2066 756c 6c44 6174 6120 3d20       fullData = 
-0001a470: 6461 7461 0a20 2020 2020 2020 2074 7269  data.        tri
-0001a480: 6d6d 6564 4461 7461 203d 2064 6174 612e  mmedData = data.
-0001a490: 6865 6164 2864 6179 7354 6f4c 6f6f 6b62  head(daysToLookb
-0001a4a0: 6163 6b29 0a20 2020 2020 2020 2072 6574  ack).        ret
-0001a4b0: 7572 6e20 2866 756c 6c44 6174 612c 2074  urn (fullData, t
-0001a4c0: 7269 6d6d 6564 4461 7461 290a 0a20 2020  rimmedData)..   
-0001a4d0: 2023 2056 616c 6964 6174 6520 6966 2074   # Validate if t
-0001a4e0: 6865 2073 746f 636b 2069 7320 6275 6c6c  he stock is bull
-0001a4f0: 6973 6820 696e 2074 6865 2073 686f 7274  ish in the short
-0001a500: 2074 6572 6d0a 2020 2020 6465 6620 7661   term.    def va
-0001a510: 6c69 6461 7465 3135 4d69 6e75 7465 5072  lidate15MinutePr
-0001a520: 6963 6556 6f6c 756d 6542 7265 616b 6f75  iceVolumeBreakou
-0001a530: 7428 7365 6c66 2c20 6466 293a 0a20 2020  t(self, df):.   
-0001a540: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
-0001a550: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
-0001a560: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-0001a570: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-0001a580: 2020 2020 2023 2068 7474 7073 3a2f 2f63       # https://c
-0001a590: 6861 7274 696e 6b2e 636f 6d2f 7363 7265  hartink.com/scre
-0001a5a0: 656e 6572 2f31 352d 6d69 6e2d 7072 6963  ener/15-min-pric
-0001a5b0: 652d 766f 6c75 6d65 2d62 7265 616b 6f75  e-volume-breakou
-0001a5c0: 740a 2020 2020 2020 2020 6461 7461 203d  t.        data =
-0001a5d0: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
-0001a5e0: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
-0001a5f0: 696c 6c6e 6128 3029 0a20 2020 2020 2020  illna(0).       
-0001a600: 2064 6174 6120 3d20 6461 7461 2e72 6570   data = data.rep
-0001a610: 6c61 6365 285b 6e70 2e69 6e66 2c20 2d6e  lace([np.inf, -n
-0001a620: 702e 696e 665d 2c20 3029 0a20 2020 2020  p.inf], 0).     
-0001a630: 2020 2064 6174 6120 3d20 6461 7461 5b3a     data = data[:
-0001a640: 3a2d 315d 2020 2320 5265 7665 7273 6520  :-1]  # Reverse 
-0001a650: 7468 6520 6461 7461 6672 616d 6520 736f  the dataframe so
-0001a660: 2074 6861 7420 6974 7320 7468 6520 6f6c   that its the ol
-0001a670: 6465 7374 2064 6174 6520 6669 7273 740a  dest date first.
-0001a680: 2020 2020 2020 2020 6461 7461 5b22 534d          data["SM
-0001a690: 4132 3022 5d20 3d20 706b 7461 6c69 622e  A20"] = pktalib.
-0001a6a0: 534d 4128 6461 7461 5b22 436c 6f73 6522  SMA(data["Close"
-0001a6b0: 5d2c 2032 3029 0a20 2020 2020 2020 2064  ], 20).        d
-0001a6c0: 6174 615b 2253 4d41 3230 5622 5d20 3d20  ata["SMA20V"] = 
-0001a6d0: 706b 7461 6c69 622e 534d 4128 6461 7461  pktalib.SMA(data
-0001a6e0: 5b22 566f 6c75 6d65 225d 2c20 3230 290a  ["Volume"], 20).
-0001a6f0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001a700: 6174 615b 0a20 2020 2020 2020 2020 2020  ata[.           
-0001a710: 203a 3a2d 310a 2020 2020 2020 2020 5d20   ::-1.        ] 
-0001a720: 2023 2052 6576 6572 7365 2074 6865 2064   # Reverse the d
-0001a730: 6174 6166 7261 6d65 2073 6f20 7468 6174  ataframe so that
-0001a740: 2069 7427 7320 7468 6520 6d6f 7374 2072   it's the most r
-0001a750: 6563 656e 7420 6461 7465 2066 6972 7374  ecent date first
-0001a760: 0a20 2020 2020 2020 2072 6563 656e 7420  .        recent 
-0001a770: 3d20 6461 7461 2e68 6561 6428 3329 0a20  = data.head(3). 
-0001a780: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
-0001a790: 6365 6e74 2920 3c20 333a 0a20 2020 2020  cent) < 3:.     
-0001a7a0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-0001a7b0: 6c73 650a 2020 2020 2020 2020 636f 6e64  lse.        cond
-0001a7c0: 3120 3d20 7265 6365 6e74 5b22 436c 6f73  1 = recent["Clos
-0001a7d0: 6522 5d2e 696c 6f63 5b30 5d20 3e20 7265  e"].iloc[0] > re
-0001a7e0: 6365 6e74 5b22 436c 6f73 6522 5d2e 696c  cent["Close"].il
-0001a7f0: 6f63 5b31 5d0a 2020 2020 2020 2020 636f  oc[1].        co
-0001a800: 6e64 3220 3d20 636f 6e64 3120 616e 6420  nd2 = cond1 and 
-0001a810: 2872 6563 656e 745b 2243 6c6f 7365 225d  (recent["Close"]
-0001a820: 2e69 6c6f 635b 305d 203e 2072 6563 656e  .iloc[0] > recen
-0001a830: 745b 2253 4d41 3230 225d 2e69 6c6f 635b  t["SMA20"].iloc[
-0001a840: 305d 290a 2020 2020 2020 2020 636f 6e64  0]).        cond
-0001a850: 3320 3d20 636f 6e64 3220 616e 6420 2872  3 = cond2 and (r
-0001a860: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
-0001a870: 6c6f 635b 315d 203e 2072 6563 656e 745b  loc[1] > recent[
-0001a880: 2248 6967 6822 5d2e 696c 6f63 5b32 5d29  "High"].iloc[2])
-0001a890: 0a20 2020 2020 2020 2063 6f6e 6434 203d  .        cond4 =
-0001a8a0: 2063 6f6e 6433 2061 6e64 2028 7265 6365   cond3 and (rece
-0001a8b0: 6e74 5b22 566f 6c75 6d65 225d 2e69 6c6f  nt["Volume"].ilo
-0001a8c0: 635b 305d 203e 2072 6563 656e 745b 2253  c[0] > recent["S
-0001a8d0: 4d41 3230 5622 5d2e 696c 6f63 5b30 5d29  MA20V"].iloc[0])
-0001a8e0: 0a20 2020 2020 2020 2063 6f6e 6435 203d  .        cond5 =
-0001a8f0: 2063 6f6e 6434 2061 6e64 2028 7265 6365   cond4 and (rece
-0001a900: 6e74 5b22 566f 6c75 6d65 225d 2e69 6c6f  nt["Volume"].ilo
-0001a910: 635b 315d 203e 2072 6563 656e 745b 2253  c[1] > recent["S
-0001a920: 4d41 3230 5622 5d2e 696c 6f63 5b30 5d29  MA20V"].iloc[0])
-0001a930: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001a940: 636f 6e64 350a 0a20 2020 2064 6566 2076  cond5..    def v
-0001a950: 616c 6964 6174 6542 756c 6c69 7368 466f  alidateBullishFo
-0001a960: 7254 6f6d 6f72 726f 7728 7365 6c66 2c20  rTomorrow(self, 
-0001a970: 6466 293a 0a20 2020 2020 2020 2069 6620  df):.        if 
-0001a980: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
-0001a990: 6e28 6466 2920 3d3d 2030 3a0a 2020 2020  n(df) == 0:.    
-0001a9a0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001a9b0: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
-0001a9c0: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
-0001a9d0: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
-0001a9e0: 6368 6172 7469 6e6b 2e63 6f6d 2f73 6372  chartink.com/scr
-0001a9f0: 6565 6e65 722f 6275 6c6c 6973 682d 666f  eener/bullish-fo
-0001aa00: 722d 746f 6d6f 7272 6f77 0a20 2020 2020  r-tomorrow.     
-0001aa10: 2020 2064 6174 6120 3d20 6461 7461 2e66     data = data.f
-0001aa20: 696c 6c6e 6128 3029 0a20 2020 2020 2020  illna(0).       
-0001aa30: 2064 6174 6120 3d20 6461 7461 2e72 6570   data = data.rep
-0001aa40: 6c61 6365 285b 6e70 2e69 6e66 2c20 2d6e  lace([np.inf, -n
-0001aa50: 702e 696e 665d 2c20 3029 0a20 2020 2020  p.inf], 0).     
-0001aa60: 2020 2064 6174 6120 3d20 6461 7461 5b3a     data = data[:
-0001aa70: 3a2d 315d 2020 2320 5265 7665 7273 6520  :-1]  # Reverse 
-0001aa80: 7468 6520 6461 7461 6672 616d 6520 736f  the dataframe so
-0001aa90: 2074 6861 7420 6974 7320 7468 6520 6f6c   that its the ol
-0001aaa0: 6465 7374 2064 6174 6520 6669 7273 740a  dest date first.
-0001aab0: 2020 2020 2020 2020 6d61 6364 4c69 6e65          macdLine
-0001aac0: 203d 2070 6b74 616c 6962 2e4d 4143 4428   = pktalib.MACD(
-0001aad0: 6461 7461 5b22 436c 6f73 6522 5d2c 2031  data["Close"], 1
-0001aae0: 322c 2032 362c 2039 295b 305d 2e74 6169  2, 26, 9)[0].tai
-0001aaf0: 6c28 3329 0a20 2020 2020 2020 206d 6163  l(3).        mac
-0001ab00: 6453 6967 6e61 6c20 3d20 706b 7461 6c69  dSignal = pktali
-0001ab10: 622e 4d41 4344 2864 6174 615b 2243 6c6f  b.MACD(data["Clo
-0001ab20: 7365 225d 2c20 3132 2c20 3236 2c20 3929  se"], 12, 26, 9)
-0001ab30: 5b31 5d2e 7461 696c 2833 290a 2020 2020  [1].tail(3).    
-0001ab40: 2020 2020 6d61 6364 4869 7374 203d 2070      macdHist = p
-0001ab50: 6b74 616c 6962 2e4d 4143 4428 6461 7461  ktalib.MACD(data
-0001ab60: 5b22 436c 6f73 6522 5d2c 2031 322c 2032  ["Close"], 12, 2
-0001ab70: 362c 2039 295b 325d 2e74 6169 6c28 3329  6, 9)[2].tail(3)
-0001ab80: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001ab90: 2028 0a20 2020 2020 2020 2020 2020 2028   (.            (
-0001aba0: 6d61 6364 4869 7374 2e69 6c6f 635b 3a31  macdHist.iloc[:1
-0001abb0: 5d2e 696c 6f63 5b30 5d20 3c20 6d61 6364  ].iloc[0] < macd
-0001abc0: 4869 7374 2e69 6c6f 635b 3a32 5d2e 696c  Hist.iloc[:2].il
-0001abd0: 6f63 5b31 5d29 0a20 2020 2020 2020 2020  oc[1]).         
-0001abe0: 2020 2061 6e64 2028 6d61 6364 4869 7374     and (macdHist
-0001abf0: 2e69 6c6f 635b 3a33 5d2e 696c 6f63 5b32  .iloc[:3].iloc[2
-0001ac00: 5d20 3e20 6d61 6364 4869 7374 2e69 6c6f  ] > macdHist.ilo
-0001ac10: 635b 3a32 5d2e 696c 6f63 5b31 5d29 0a20  c[:2].iloc[1]). 
-0001ac20: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
-0001ac30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ac40: 2028 6d61 6364 4c69 6e65 2e69 6c6f 635b   (macdLine.iloc[
-0001ac50: 3a33 5d2e 696c 6f63 5b32 5d20 2d20 6d61  :3].iloc[2] - ma
-0001ac60: 6364 5369 676e 616c 2e69 6c6f 635b 3a33  cdSignal.iloc[:3
-0001ac70: 5d2e 696c 6f63 5b32 5d29 0a20 2020 2020  ].iloc[2]).     
-0001ac80: 2020 2020 2020 2020 2020 202d 2028 6d61             - (ma
-0001ac90: 6364 4c69 6e65 2e69 6c6f 635b 3a32 5d2e  cdLine.iloc[:2].
-0001aca0: 696c 6f63 5b31 5d20 2d20 6d61 6364 5369  iloc[1] - macdSi
-0001acb0: 676e 616c 2e69 6c6f 635b 3a32 5d2e 696c  gnal.iloc[:2].il
-0001acc0: 6f63 5b31 5d29 0a20 2020 2020 2020 2020  oc[1]).         
-0001acd0: 2020 2020 2020 203e 3d20 302e 340a 2020         >= 0.4.  
-0001ace0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0001acf0: 2020 2020 2020 2020 616e 6420 280a 2020          and (.  
-0001ad00: 2020 2020 2020 2020 2020 2020 2020 286d                (m
-0001ad10: 6163 644c 696e 652e 696c 6f63 5b3a 325d  acdLine.iloc[:2]
-0001ad20: 2e69 6c6f 635b 315d 202d 206d 6163 6453  .iloc[1] - macdS
-0001ad30: 6967 6e61 6c2e 696c 6f63 5b3a 325d 2e69  ignal.iloc[:2].i
-0001ad40: 6c6f 635b 315d 290a 2020 2020 2020 2020  loc[1]).        
-0001ad50: 2020 2020 2020 2020 2d20 286d 6163 644c          - (macdL
-0001ad60: 696e 652e 696c 6f63 5b3a 315d 2e69 6c6f  ine.iloc[:1].ilo
-0001ad70: 635b 305d 202d 206d 6163 6453 6967 6e61  c[0] - macdSigna
-0001ad80: 6c2e 696c 6f63 5b3a 315d 2e69 6c6f 635b  l.iloc[:1].iloc[
-0001ad90: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-0001ada0: 2020 2020 3c3d 2030 2e32 0a20 2020 2020      <= 0.2.     
-0001adb0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001adc0: 2020 2020 2061 6e64 2028 6d61 6364 4c69       and (macdLi
-0001add0: 6e65 2e69 6c6f 635b 3a33 5d2e 696c 6f63  ne.iloc[:3].iloc
-0001ade0: 5b32 5d20 3e20 6d61 6364 5369 676e 616c  [2] > macdSignal
-0001adf0: 2e69 6c6f 635b 3a33 5d2e 696c 6f63 5b32  .iloc[:3].iloc[2
-0001ae00: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
-0001ae10: 6e64 2028 0a20 2020 2020 2020 2020 2020  nd (.           
-0001ae20: 2020 2020 2028 6d61 6364 4c69 6e65 2e69       (macdLine.i
-0001ae30: 6c6f 635b 3a33 5d2e 696c 6f63 5b32 5d20  loc[:3].iloc[2] 
-0001ae40: 2d20 6d61 6364 5369 676e 616c 2e69 6c6f  - macdSignal.ilo
-0001ae50: 635b 3a33 5d2e 696c 6f63 5b32 5d29 0a20  c[:3].iloc[2]). 
-0001ae60: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-0001ae70: 2028 6d61 6364 4c69 6e65 2e69 6c6f 635b   (macdLine.iloc[
-0001ae80: 3a32 5d2e 696c 6f63 5b31 5d20 2d20 6d61  :2].iloc[1] - ma
-0001ae90: 6364 5369 676e 616c 2e69 6c6f 635b 3a32  cdSignal.iloc[:2
-0001aea0: 5d2e 696c 6f63 5b31 5d29 0a20 2020 2020  ].iloc[1]).     
-0001aeb0: 2020 2020 2020 2020 2020 203c 2031 0a20             < 1. 
-0001aec0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0001aed0: 2020 2020 2029 0a0a 2020 2020 2340 6d65       )..    #@me
-0001aee0: 6173 7572 655f 7469 6d65 0a20 2020 2023  asure_time.    #
-0001aef0: 2076 616c 6964 6174 6520 6966 2043 4349   validate if CCI
-0001af00: 2069 7320 7769 7468 696e 2067 6976 656e   is within given
-0001af10: 2072 616e 6765 0a20 2020 2064 6566 2076   range.    def v
-0001af20: 616c 6964 6174 6543 4349 2873 656c 662c  alidateCCI(self,
-0001af30: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
-0001af40: 2073 6176 6544 6963 742c 206d 696e 4343   saveDict, minCC
-0001af50: 492c 206d 6178 4343 4929 3a0a 2020 2020  I, maxCCI):.    
-0001af60: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
-0001af70: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
-0001af80: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-0001af90: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-0001afa0: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
-0001afb0: 7079 2829 0a20 2020 2020 2020 2064 6174  py().        dat
-0001afc0: 6120 3d20 6461 7461 2e66 696c 6c6e 6128  a = data.fillna(
-0001afd0: 3029 0a20 2020 2020 2020 2064 6174 6120  0).        data 
-0001afe0: 3d20 6461 7461 2e72 6570 6c61 6365 285b  = data.replace([
-0001aff0: 6e70 2e69 6e66 2c20 2d6e 702e 696e 665d  np.inf, -np.inf]
-0001b000: 2c20 3029 0a20 2020 2020 2020 2063 6369  , 0).        cci
-0001b010: 203d 2069 6e74 2864 6174 612e 6865 6164   = int(data.head
-0001b020: 2831 295b 2243 4349 225d 2e69 6c6f 635b  (1)["CCI"].iloc[
-0001b030: 305d 290a 2020 2020 2020 2020 7361 7665  0]).        save
-0001b040: 4469 6374 5b22 4343 4922 5d20 3d20 6363  Dict["CCI"] = cc
-0001b050: 690a 2020 2020 2020 2020 6966 2028 6363  i.        if (cc
-0001b060: 6920 3e3d 206d 696e 4343 4920 616e 6420  i >= minCCI and 
-0001b070: 6363 6920 3c3d 206d 6178 4343 4929 3a0a  cci <= maxCCI):.
-0001b080: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-0001b090: 2255 7022 2069 6e20 7361 7665 4469 6374  "Up" in saveDict
-0001b0a0: 5b22 5472 656e 6422 5d29 3a0a 2020 2020  ["Trend"]):.    
-0001b0b0: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-0001b0c0: 656e 4469 6374 5b22 4343 4922 5d20 3d20  enDict["CCI"] = 
-0001b0d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001b0e0: 2020 2020 2020 2863 6f6c 6f72 5465 7874        (colorText
-0001b0f0: 2e42 4f4c 4420 6966 2028 2253 7472 6f6e  .BOLD if ("Stron
-0001b100: 6722 2069 6e20 7361 7665 4469 6374 5b22  g" in saveDict["
-0001b110: 5472 656e 6422 5d29 2065 6c73 6520 2222  Trend"]) else ""
-0001b120: 2920 2b20 636f 6c6f 7254 6578 742e 4752  ) + colorText.GR
-0001b130: 4545 4e20 2b20 7374 7228 6363 6929 202b  EEN + str(cci) +
-0001b140: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
-0001b150: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001b160: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0001b170: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001b180: 2020 2073 6372 6565 6e44 6963 745b 2243     screenDict["C
-0001b190: 4349 225d 203d 2028 0a20 2020 2020 2020  CI"] = (.       
-0001b1a0: 2020 2020 2020 2020 2020 2020 2028 636f               (co
-0001b1b0: 6c6f 7254 6578 742e 424f 4c44 2069 6620  lorText.BOLD if 
-0001b1c0: 2822 5374 726f 6e67 2220 696e 2073 6176  ("Strong" in sav
-0001b1d0: 6544 6963 745b 2254 7265 6e64 225d 2920  eDict["Trend"]) 
-0001b1e0: 656c 7365 2022 2229 202b 2063 6f6c 6f72  else "") + color
-0001b1f0: 5465 7874 2e46 4149 4c20 2b20 7374 7228  Text.FAIL + str(
-0001b200: 6363 6929 202b 2063 6f6c 6f72 5465 7874  cci) + colorText
-0001b210: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
-0001b220: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0001b230: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-0001b240: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-0001b250: 745b 2243 4349 225d 203d 2063 6f6c 6f72  t["CCI"] = color
-0001b260: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
-0001b270: 7254 6578 742e 4641 494c 202b 2073 7472  rText.FAIL + str
-0001b280: 2863 6369 2920 2b20 636f 6c6f 7254 6578  (cci) + colorTex
-0001b290: 742e 454e 440a 2020 2020 2020 2020 7265  t.END.        re
-0001b2a0: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
-0001b2b0: 2320 4669 6e64 2043 6f6e 666c 7563 656e  # Find Conflucen
-0001b2c0: 6365 0a20 2020 2064 6566 2076 616c 6964  ce.    def valid
-0001b2d0: 6174 6543 6f6e 666c 7565 6e63 6528 7365  ateConfluence(se
-0001b2e0: 6c66 2c20 7374 6f63 6b2c 2064 662c 2073  lf, stock, df, s
-0001b2f0: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-0001b300: 6963 742c 2070 6572 6365 6e74 6167 653d  ict, percentage=
-0001b310: 302e 312c 636f 6e66 4669 6c74 6572 3d33  0.1,confFilter=3
-0001b320: 293a 0a20 2020 2020 2020 2069 6620 6466  ):.        if df
-0001b330: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
-0001b340: 6466 2920 3d3d 2030 3a0a 2020 2020 2020  df) == 0:.      
-0001b350: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0001b360: 7365 0a20 2020 2020 2020 2064 6174 6120  se.        data 
-0001b370: 3d20 6466 2e63 6f70 7928 290a 2020 2020  = df.copy().    
-0001b380: 2020 2020 7265 6365 6e74 203d 2064 6174      recent = dat
-0001b390: 612e 6865 6164 2832 290a 2020 2020 2020  a.head(2).      
-0001b3a0: 2020 6966 206c 656e 2872 6563 656e 7429    if len(recent)
-0001b3b0: 203c 2032 3a0a 2020 2020 2020 2020 2020   < 2:.          
-0001b3c0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-0001b3d0: 2020 2020 2020 2069 7335 3044 4d41 5570         is50DMAUp
-0001b3e0: 5472 656e 6420 3d20 2872 6563 656e 745b  Trend = (recent[
-0001b3f0: 2253 4d41 225d 2e69 6c6f 635b 305d 203e  "SMA"].iloc[0] >
-0001b400: 2072 6563 656e 745b 2253 4d41 225d 2e69   recent["SMA"].i
-0001b410: 6c6f 635b 315d 290a 2020 2020 2020 2020  loc[1]).        
-0001b420: 6973 3530 444d 4144 6f77 6e54 7265 6e64  is50DMADownTrend
-0001b430: 203d 2028 7265 6365 6e74 5b22 534d 4122   = (recent["SMA"
-0001b440: 5d2e 696c 6f63 5b30 5d20 3c20 7265 6365  ].iloc[0] < rece
-0001b450: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b31  nt["SMA"].iloc[1
-0001b460: 5d29 0a20 2020 2020 2020 2069 7347 6f6c  ]).        isGol
-0001b470: 6465 6e43 726f 7373 4f76 6572 203d 2028  denCrossOver = (
-0001b480: 7265 6365 6e74 5b22 534d 4122 5d2e 696c  recent["SMA"].il
-0001b490: 6f63 5b30 5d20 3e3d 2072 6563 656e 745b  oc[0] >= recent[
-0001b4a0: 224c 4d41 225d 2e69 6c6f 635b 305d 2920  "LMA"].iloc[0]) 
-0001b4b0: 616e 6420 5c0a 2020 2020 2020 2020 2020  and \.          
-0001b4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b4d0: 2020 2872 6563 656e 745b 2253 4d41 225d    (recent["SMA"]
-0001b4e0: 2e69 6c6f 635b 315d 203c 3d20 7265 6365  .iloc[1] <= rece
-0001b4f0: 6e74 5b22 4c4d 4122 5d2e 696c 6f63 5b31  nt["LMA"].iloc[1
-0001b500: 5d29 0a20 2020 2020 2020 2069 7344 6561  ]).        isDea
-0001b510: 6443 726f 7373 4f76 6572 203d 2028 7265  dCrossOver = (re
-0001b520: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
-0001b530: 5b30 5d20 3c3d 2072 6563 656e 745b 224c  [0] <= recent["L
-0001b540: 4d41 225d 2e69 6c6f 635b 305d 2920 616e  MA"].iloc[0]) an
-0001b550: 6420 5c0a 2020 2020 2020 2020 2020 2020  d \.            
-0001b560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b570: 2872 6563 656e 745b 2253 4d41 225d 2e69  (recent["SMA"].i
-0001b580: 6c6f 635b 315d 203e 3d20 7265 6365 6e74  loc[1] >= recent
-0001b590: 5b22 4c4d 4122 5d2e 696c 6f63 5b31 5d29  ["LMA"].iloc[1])
-0001b5a0: 0a20 2020 2020 2020 2069 7335 3044 4d41  .        is50DMA
-0001b5b0: 203d 2028 7265 6365 6e74 5b22 534d 4122   = (recent["SMA"
-0001b5c0: 5d2e 696c 6f63 5b30 5d20 3c3d 2072 6563  ].iloc[0] <= rec
-0001b5d0: 656e 745b 2243 6c6f 7365 225d 2e69 6c6f  ent["Close"].ilo
-0001b5e0: 635b 305d 290a 2020 2020 2020 2020 6973  c[0]).        is
-0001b5f0: 3230 3044 4d41 203d 2028 7265 6365 6e74  200DMA = (recent
-0001b600: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d20  ["LMA"].iloc[0] 
-0001b610: 3c3d 2072 6563 656e 745b 2243 6c6f 7365  <= recent["Close
-0001b620: 225d 2e69 6c6f 635b 305d 290a 2020 2020  "].iloc[0]).    
-0001b630: 2020 2020 6469 6666 6572 656e 6365 203d      difference =
-0001b640: 2072 6f75 6e64 2828 7265 6365 6e74 5b22   round((recent["
-0001b650: 534d 4122 5d2e 696c 6f63 5b30 5d20 2d20  SMA"].iloc[0] - 
-0001b660: 7265 6365 6e74 5b22 4c4d 4122 5d2e 696c  recent["LMA"].il
-0001b670: 6f63 5b30 5d29 0a20 2020 2020 2020 2020  oc[0]).         
-0001b680: 2020 2020 2020 202f 2072 6563 656e 745b         / recent[
-0001b690: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
-0001b6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b6b0: 202a 2031 3030 2c0a 2020 2020 2020 2020   * 100,.        
-0001b6c0: 2020 2020 2020 2020 322c 0a20 2020 2020          2,.     
-0001b6d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001b6e0: 2073 6176 6544 6963 745b 2243 6f6e 6644   saveDict["ConfD
-0001b6f0: 4d41 4469 6666 6572 656e 6365 225d 203d  MADifference"] =
-0001b700: 2064 6966 6665 7265 6e63 650a 2020 2020   difference.    
-0001b710: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-0001b720: 436f 6e66 444d 4144 6966 6665 7265 6e63  ConfDMADifferenc
-0001b730: 6522 5d20 3d20 6469 6666 6572 656e 6365  e"] = difference
-0001b740: 0a20 2020 2020 2020 2073 6176 6564 203d  .        saved =
-0001b750: 2073 656c 662e 6669 6e64 4375 7272 656e   self.findCurren
-0001b760: 7453 6176 6564 5661 6c75 6528 7363 7265  tSavedValue(scre
-0001b770: 656e 4469 6374 2c73 6176 6544 6963 742c  enDict,saveDict,
-0001b780: 224d 412d 5369 676e 616c 2229 0a20 2020  "MA-Signal").   
-0001b790: 2020 2020 2023 2064 6966 6665 7265 6e63       # differenc
-0001b7a0: 6520 3d20 6162 7328 6469 6666 6572 656e  e = abs(differen
-0001b7b0: 6365 290a 2020 2020 2020 2020 636f 6e66  ce).        conf
-0001b7c0: 5465 7874 203d 2066 227b 2747 6f6c 6465  Text = f"{'Golde
-0001b7d0: 6e43 726f 7373 6f76 6572 2720 6966 2069  nCrossover' if i
-0001b7e0: 7347 6f6c 6465 6e43 726f 7373 4f76 6572  sGoldenCrossOver
-0001b7f0: 2065 6c73 6520 2827 4465 6164 4372 6f73   else ('DeadCros
-0001b800: 736f 7665 7227 2069 6620 6973 4465 6164  sover' if isDead
-0001b810: 4372 6f73 734f 7665 7220 656c 7365 2028  CrossOver else (
-0001b820: 2743 6f6e 662e 5570 2720 6966 2069 7335  'Conf.Up' if is5
-0001b830: 3044 4d41 5570 5472 656e 6420 656c 7365  0DMAUpTrend else
-0001b840: 2028 2743 6f6e 662e 446f 776e 2720 6966   ('Conf.Down' if
-0001b850: 2069 7335 3044 4d41 446f 776e 5472 656e   is50DMADownTren
-0001b860: 6420 656c 7365 2028 2735 3044 4d41 2720  d else ('50DMA' 
-0001b870: 6966 2069 7335 3044 4d41 2065 6c73 6520  if is50DMA else 
-0001b880: 2827 3230 3044 4d41 2720 6966 2069 7332  ('200DMA' if is2
-0001b890: 3030 444d 4120 656c 7365 2027 556e 6b6e  00DMA else 'Unkn
-0001b8a0: 6f77 6e27 2929 2929 297d 220a 2020 2020  own')))))}".    
-0001b8b0: 2020 2020 6966 2061 6273 2872 6563 656e      if abs(recen
-0001b8c0: 745b 2253 4d41 225d 2e69 6c6f 635b 305d  t["SMA"].iloc[0]
-0001b8d0: 202d 2072 6563 656e 745b 224c 4d41 225d   - recent["LMA"]
-0001b8e0: 2e69 6c6f 635b 305d 2920 3c3d 2028 0a20  .iloc[0]) <= (. 
-0001b8f0: 2020 2020 2020 2020 2020 2072 6563 656e             recen
-0001b900: 745b 2253 4d41 225d 2e69 6c6f 635b 305d  t["SMA"].iloc[0]
-0001b910: 202a 2070 6572 6365 6e74 6167 650a 2020   * percentage.  
-0001b920: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-0001b930: 2020 2020 2069 6620 7265 6365 6e74 5b22       if recent["
-0001b940: 534d 4122 5d2e 696c 6f63 5b30 5d20 3e3d  SMA"].iloc[0] >=
-0001b950: 2072 6563 656e 745b 224c 4d41 225d 2e69   recent["LMA"].i
-0001b960: 6c6f 635b 305d 3a0a 2020 2020 2020 2020  loc[0]:.        
-0001b970: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-0001b980: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-0001b990: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0001b9a0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-0001b9b0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0001b9c0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001b9d0: 742e 424f 4c44 0a20 2020 2020 2020 2020  t.BOLD.         
-0001b9e0: 2020 2020 2020 2020 2020 202b 2028 636f             + (co
-0001b9f0: 6c6f 7254 6578 742e 4752 4545 4e20 6966  lorText.GREEN if
-0001ba00: 2069 7335 3044 4d41 5570 5472 656e 6420   is50DMAUpTrend 
-0001ba10: 656c 7365 2028 636f 6c6f 7254 6578 742e  else (colorText.
-0001ba20: 4641 494c 2069 6620 6973 3530 444d 4144  FAIL if is50DMAD
-0001ba30: 6f77 6e54 7265 6e64 2065 6c73 6520 636f  ownTrend else co
-0001ba40: 6c6f 7254 6578 742e 5741 524e 2929 0a20  lorText.WARN)). 
-0001ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ba60: 2020 202b 2066 227b 636f 6e66 5465 7874     + f"{confText
-0001ba70: 7d20 287b 6469 6666 6572 656e 6365 7d25  } ({difference}%
-0001ba80: 2922 0a20 2020 2020 2020 2020 2020 2020  )".             
-0001ba90: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-0001baa0: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
-0001bab0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001bac0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-0001bad0: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-0001bae0: 2073 6176 6564 5b31 5d20 2b20 6622 7b63   saved[1] + f"{c
-0001baf0: 6f6e 6654 6578 747d 2028 7b64 6966 6665  onfText} ({diffe
-0001bb00: 7265 6e63 657d 2529 220a 2020 2020 2020  rence}%)".      
-0001bb10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001bb20: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-0001bb30: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
-0001bb40: 6c22 5d20 3d20 280a 2020 2020 2020 2020  l"] = (.        
-0001bb50: 2020 2020 2020 2020 2020 2020 7361 7665              save
-0001bb60: 645b 305d 200a 2020 2020 2020 2020 2020  d[0] .          
-0001bb70: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001bb80: 7254 6578 742e 424f 4c44 0a20 2020 2020  rText.BOLD.     
-0001bb90: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001bba0: 2028 636f 6c6f 7254 6578 742e 4752 4545   (colorText.GREE
-0001bbb0: 4e20 6966 2069 7335 3044 4d41 5570 5472  N if is50DMAUpTr
-0001bbc0: 656e 6420 656c 7365 2028 636f 6c6f 7254  end else (colorT
-0001bbd0: 6578 742e 4641 494c 2069 6620 6973 3530  ext.FAIL if is50
-0001bbe0: 444d 4144 6f77 6e54 7265 6e64 2065 6c73  DMADownTrend els
-0001bbf0: 6520 636f 6c6f 7254 6578 742e 5741 524e  e colorText.WARN
-0001bc00: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0001bc10: 2020 2020 2020 202b 2066 227b 636f 6e66         + f"{conf
-0001bc20: 5465 7874 7d20 287b 6469 6666 6572 656e  Text} ({differen
-0001bc30: 6365 7d25 2922 0a20 2020 2020 2020 2020  ce}%)".         
-0001bc40: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-0001bc50: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
-0001bc60: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0001bc70: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-0001bc80: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
-0001bc90: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-0001bca0: 6622 7b63 6f6e 6654 6578 747d 2028 7b64  f"{confText} ({d
-0001bcb0: 6966 6665 7265 6e63 657d 2529 220a 2020  ifference}%)".  
-0001bcc0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001bcd0: 2063 6f6e 6646 696c 7465 7220 3d3d 2033   confFilter == 3
-0001bce0: 206f 7220 5c0a 2020 2020 2020 2020 2020   or \.          
-0001bcf0: 2020 2020 2020 2863 6f6e 6646 696c 7465        (confFilte
-0001bd00: 7220 3d3d 2031 2061 6e64 2028 6973 3530  r == 1 and (is50
-0001bd10: 444d 4155 7054 7265 6e64 206f 7220 2869  DMAUpTrend or (i
-0001bd20: 7347 6f6c 6465 6e43 726f 7373 4f76 6572  sGoldenCrossOver
-0001bd30: 206f 7220 2755 7027 2069 6e20 636f 6e66   or 'Up' in conf
-0001bd40: 5465 7874 2929 2920 6f72 205c 0a20 2020  Text))) or \.   
-0001bd50: 2020 2020 2020 2020 2020 2020 2028 636f               (co
-0001bd60: 6e66 4669 6c74 6572 203d 3d20 3220 616e  nfFilter == 2 an
-0001bd70: 6420 2869 7335 3044 4d41 446f 776e 5472  d (is50DMADownTr
-0001bd80: 656e 6420 6f72 2069 7344 6561 6443 726f  end or isDeadCro
-0001bd90: 7373 4f76 6572 206f 7220 2744 6f77 6e27  ssOver or 'Down'
-0001bda0: 2069 6e20 636f 6e66 5465 7874 2929 0a20   in confText)). 
-0001bdb0: 2020 2020 2020 2023 204d 6179 6265 2074         # Maybe t
-0001bdc0: 6865 2064 6966 6665 7265 6e63 6520 6973  he difference is
-0001bdd0: 206e 6f74 2077 6974 6869 6e20 7468 6520   not within the 
-0001bde0: 7261 6e67 652c 2062 7574 2077 6527 6420  range, but we'd 
-0001bdf0: 7374 696c 6c20 6c69 6b65 2074 6f20 6b65  still like to ke
-0001be00: 6570 2074 6865 2073 746f 636b 2069 6e0a  ep the stock in.
-0001be10: 2020 2020 2020 2020 2320 7468 6520 6c69          # the li
-0001be20: 7374 2069 6620 6974 2773 2061 2067 6f6c  st if it's a gol
-0001be30: 6465 6e20 6372 6f73 736f 7665 7220 6f72  den crossover or
-0001be40: 2064 6561 6420 6372 6f73 736f 7665 720a   dead crossover.
-0001be50: 2020 2020 2020 2020 6966 2069 7347 6f6c          if isGol
-0001be60: 6465 6e43 726f 7373 4f76 6572 206f 7220  denCrossOver or 
-0001be70: 6973 4465 6164 4372 6f73 734f 7665 723a  isDeadCrossOver:
-0001be80: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-0001be90: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
-0001bea0: 616c 225d 203d 2028 0a20 2020 2020 2020  al"] = (.       
-0001beb0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-0001bec0: 6564 5b30 5d20 0a20 2020 2020 2020 2020  ed[0] .         
-0001bed0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-0001bee0: 6f72 5465 7874 2e42 4f4c 440a 2020 2020  orText.BOLD.    
-0001bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf00: 2b20 2863 6f6c 6f72 5465 7874 2e47 5245  + (colorText.GRE
-0001bf10: 454e 2069 6620 6973 3530 444d 4155 7054  EN if is50DMAUpT
-0001bf20: 7265 6e64 2065 6c73 6520 2863 6f6c 6f72  rend else (color
-0001bf30: 5465 7874 2e46 4149 4c20 6966 2069 7335  Text.FAIL if is5
-0001bf40: 3044 4d41 446f 776e 5472 656e 6420 656c  0DMADownTrend el
-0001bf50: 7365 2063 6f6c 6f72 5465 7874 2e57 4152  se colorText.WAR
-0001bf60: 4e29 290a 2020 2020 2020 2020 2020 2020  N)).            
-0001bf70: 2020 2020 2020 2020 2b20 6622 7b63 6f6e          + f"{con
-0001bf80: 6654 6578 747d 2028 7b64 6966 6665 7265  fText} ({differe
-0001bf90: 6e63 657d 2529 220a 2020 2020 2020 2020  nce}%)".        
-0001bfa0: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-0001bfb0: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
-0001bfc0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001bfd0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-0001bfe0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-0001bff0: 3d20 7361 7665 645b 315d 202b 2066 227b  = saved[1] + f"{
-0001c000: 636f 6e66 5465 7874 7d20 287b 6469 6666  confText} ({diff
-0001c010: 6572 656e 6365 7d25 2922 0a20 2020 2020  erence}%)".     
-0001c020: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
-0001c030: 6e66 4669 6c74 6572 203d 3d20 3320 6f72  nfFilter == 3 or
-0001c040: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-0001c050: 2020 2028 636f 6e66 4669 6c74 6572 203d     (confFilter =
-0001c060: 3d20 3120 616e 6420 6973 476f 6c64 656e  = 1 and isGolden
-0001c070: 4372 6f73 734f 7665 7229 206f 7220 5c0a  CrossOver) or \.
-0001c080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c090: 2863 6f6e 6646 696c 7465 7220 3d3d 2032  (confFilter == 2
-0001c0a0: 2061 6e64 2069 7344 6561 6443 726f 7373   and isDeadCross
-0001c0b0: 4f76 6572 290a 2020 2020 2020 2020 7265  Over).        re
-0001c0c0: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
-0001c0d0: 2340 6d65 6173 7572 655f 7469 6d65 0a20  #@measure_time. 
-0001c0e0: 2020 2023 2056 616c 6964 6174 6520 6966     # Validate if
-0001c0f0: 2073 6861 7265 2070 7269 6365 7320 6172   share prices ar
-0001c100: 6520 636f 6e73 6f6c 6964 6174 696e 670a  e consolidating.
-0001c110: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0001c120: 436f 6e73 6f6c 6964 6174 696f 6e28 7365  Consolidation(se
-0001c130: 6c66 2c20 6466 2c20 7363 7265 656e 4469  lf, df, screenDi
-0001c140: 6374 2c20 7361 7665 4469 6374 2c20 7065  ct, saveDict, pe
-0001c150: 7263 656e 7461 6765 3d31 3029 3a0a 2020  rcentage=10):.  
-0001c160: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
-0001c170: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
-0001c180: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-0001c190: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-0001c1a0: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
-0001c1b0: 636f 7079 2829 0a20 2020 2020 2020 2064  copy().        d
-0001c1c0: 6174 6120 3d20 6461 7461 2e66 696c 6c6e  ata = data.filln
-0001c1d0: 6128 3029 0a20 2020 2020 2020 2064 6174  a(0).        dat
-0001c1e0: 6120 3d20 6461 7461 2e72 6570 6c61 6365  a = data.replace
-0001c1f0: 285b 6e70 2e69 6e66 2c20 2d6e 702e 696e  ([np.inf, -np.in
-0001c200: 665d 2c20 3029 0a20 2020 2020 2020 2068  f], 0).        h
-0001c210: 6320 3d20 6461 7461 2e64 6573 6372 6962  c = data.describ
-0001c220: 6528 295b 2243 6c6f 7365 225d 5b22 6d61  e()["Close"]["ma
-0001c230: 7822 5d0a 2020 2020 2020 2020 6c63 203d  x"].        lc =
-0001c240: 2064 6174 612e 6465 7363 7269 6265 2829   data.describe()
-0001c250: 5b22 436c 6f73 6522 5d5b 226d 696e 225d  ["Close"]["min"]
-0001c260: 0a20 2020 2020 2020 2069 6620 2868 6320  .        if (hc 
-0001c270: 2d20 6c63 2920 3c3d 2028 6863 202a 2070  - lc) <= (hc * p
-0001c280: 6572 6365 6e74 6167 6520 2f20 3130 3029  ercentage / 100)
-0001c290: 2061 6e64 2028 6863 202d 206c 6320 213d   and (hc - lc !=
-0001c2a0: 2030 293a 0a20 2020 2020 2020 2020 2020   0):.           
-0001c2b0: 2073 6372 6565 6e44 6963 745b 2243 6f6e   screenDict["Con
-0001c2c0: 736f 6c2e 225d 203d 2028 0a20 2020 2020  sol."] = (.     
-0001c2d0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
-0001c2e0: 5465 7874 2e42 4f4c 440a 2020 2020 2020  Text.BOLD.      
-0001c2f0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001c300: 7254 6578 742e 4752 4545 4e0a 2020 2020  rText.GREEN.    
-0001c310: 2020 2020 2020 2020 2020 2020 2b20 2252              + "R
-0001c320: 616e 6765 3a22 0a20 2020 2020 2020 2020  ange:".         
-0001c330: 2020 2020 2020 202b 2073 7472 2872 6f75         + str(rou
-0001c340: 6e64 2828 6162 7328 2868 6320 2d20 6c63  nd((abs((hc - lc
-0001c350: 2920 2f20 6863 2920 2a20 3130 3029 2c20  ) / hc) * 100), 
-0001c360: 3129 290a 2020 2020 2020 2020 2020 2020  1)).            
-0001c370: 2020 2020 2b20 2225 220a 2020 2020 2020      + "%".      
-0001c380: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001c390: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
-0001c3a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001c3b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001c3c0: 2020 7363 7265 656e 4469 6374 5b22 436f    screenDict["Co
-0001c3d0: 6e73 6f6c 2e22 5d20 3d20 280a 2020 2020  nsol."] = (.    
-0001c3e0: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-0001c3f0: 7254 6578 742e 424f 4c44 0a20 2020 2020  rText.BOLD.     
-0001c400: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-0001c410: 6f72 5465 7874 2e46 4149 4c0a 2020 2020  orText.FAIL.    
-0001c420: 2020 2020 2020 2020 2020 2020 2b20 2252              + "R
-0001c430: 616e 6765 3a22 0a20 2020 2020 2020 2020  ange:".         
-0001c440: 2020 2020 2020 202b 2073 7472 2872 6f75         + str(rou
-0001c450: 6e64 2828 6162 7328 2868 6320 2d20 6c63  nd((abs((hc - lc
-0001c460: 2920 2f20 6863 2920 2a20 3130 3029 2c20  ) / hc) * 100), 
-0001c470: 3129 290a 2020 2020 2020 2020 2020 2020  1)).            
-0001c480: 2020 2020 2b20 2225 220a 2020 2020 2020      + "%".      
-0001c490: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001c4a0: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
-0001c4b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001c4c0: 7361 7665 4469 6374 5b22 436f 6e73 6f6c  saveDict["Consol
-0001c4d0: 2e22 5d20 3d20 6627 5261 6e67 653a 7b73  ."] = f'Range:{s
-0001c4e0: 7472 2872 6f75 6e64 2828 6162 7328 2868  tr(round((abs((h
-0001c4f0: 632d 6c63 292f 6863 292a 3130 3029 2c31  c-lc)/hc)*100),1
-0001c500: 2929 2b22 2522 7d27 0a20 2020 2020 2020  ))+"%"}'.       
-0001c510: 2072 6574 7572 6e20 726f 756e 6428 2861   return round((a
-0001c520: 6273 2828 6863 202d 206c 6329 202f 2068  bs((hc - lc) / h
-0001c530: 6329 202a 2031 3030 292c 2031 290a 0a20  c) * 100), 1).. 
-0001c540: 2020 2023 2076 616c 6964 6174 6520 6966     # validate if
-0001c550: 2074 6865 2073 746f 636b 2068 6173 2062   the stock has b
-0001c560: 6565 6e20 6861 7669 6e67 2068 6967 6865  een having highe
-0001c570: 7220 6869 6768 732c 2068 6967 6865 7220  r highs, higher 
-0001c580: 6c6f 7773 0a20 2020 2023 2061 6e64 2068  lows.    # and h
-0001c590: 6967 6865 7220 636c 6f73 6520 7769 7468  igher close with
-0001c5a0: 206c 6174 6573 7420 636c 6f73 6520 3e20   latest close > 
-0001c5b0: 7375 7065 7274 7265 6e64 2061 6e64 2038  supertrend and 8
-0001c5c0: 2d45 4d41 2e0a 2020 2020 6465 6620 7661  -EMA..    def va
-0001c5d0: 6c69 6461 7465 4869 6768 6572 4869 6768  lidateHigherHigh
-0001c5e0: 7348 6967 6865 724c 6f77 7348 6967 6865  sHigherLowsHighe
-0001c5f0: 7243 6c6f 7365 2873 656c 662c 2064 6629  rClose(self, df)
-0001c600: 3a0a 2020 2020 2020 2020 6966 2064 6620  :.        if df 
-0001c610: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-0001c620: 6629 203d 3d20 303a 0a20 2020 2020 2020  f) == 0:.       
-0001c630: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-0001c640: 650a 2020 2020 2020 2020 6461 7461 203d  e.        data =
-0001c650: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
-0001c660: 2020 2064 6179 3020 3d20 6461 7461 0a20     day0 = data. 
-0001c670: 2020 2020 2020 2064 6179 3120 3d20 6461         day1 = da
-0001c680: 7461 5b31 3a5d 0a20 2020 2020 2020 2064  ta[1:].        d
-0001c690: 6179 3220 3d20 6461 7461 5b32 3a5d 0a20  ay2 = data[2:]. 
-0001c6a0: 2020 2020 2020 2064 6179 3320 3d20 6461         day3 = da
-0001c6b0: 7461 5b33 3a5d 0a20 2020 2020 2020 2069  ta[3:].        i
-0001c6c0: 6620 6c65 6e28 6461 7931 2920 3c20 3120  f len(day1) < 1 
-0001c6d0: 6f72 206c 656e 2864 6179 3229 203c 2031  or len(day2) < 1
-0001c6e0: 206f 7220 6c65 6e28 6461 7933 2920 3c20   or len(day3) < 
-0001c6f0: 313a 0a20 2020 2020 2020 2020 2020 2072  1:.            r
-0001c700: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-0001c710: 2020 2020 6869 6768 6572 4869 6768 7320      higherHighs 
-0001c720: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0001c730: 2864 6179 305b 2248 6967 6822 5d2e 696c  (day0["High"].il
-0001c740: 6f63 5b30 5d20 3e20 6461 7931 5b22 4869  oc[0] > day1["Hi
-0001c750: 6768 225d 2e69 6c6f 635b 305d 290a 2020  gh"].iloc[0]).  
-0001c760: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
-0001c770: 6179 315b 2248 6967 6822 5d2e 696c 6f63  ay1["High"].iloc
-0001c780: 5b30 5d20 3e20 6461 7932 5b22 4869 6768  [0] > day2["High
-0001c790: 225d 2e69 6c6f 635b 305d 290a 2020 2020  "].iloc[0]).    
-0001c7a0: 2020 2020 2020 2020 616e 6420 2864 6179          and (day
-0001c7b0: 325b 2248 6967 6822 5d2e 696c 6f63 5b30  2["High"].iloc[0
-0001c7c0: 5d20 3e20 6461 7933 5b22 4869 6768 225d  ] > day3["High"]
-0001c7d0: 2e69 6c6f 635b 305d 290a 2020 2020 2020  .iloc[0]).      
-0001c7e0: 2020 290a 2020 2020 2020 2020 6869 6768    ).        high
-0001c7f0: 6572 4c6f 7773 203d 2028 0a20 2020 2020  erLows = (.     
-0001c800: 2020 2020 2020 2028 6461 7930 5b22 4c6f         (day0["Lo
-0001c810: 7722 5d2e 696c 6f63 5b30 5d20 3e20 6461  w"].iloc[0] > da
-0001c820: 7931 5b22 4c6f 7722 5d2e 696c 6f63 5b30  y1["Low"].iloc[0
-0001c830: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
-0001c840: 6e64 2028 6461 7931 5b22 4c6f 7722 5d2e  nd (day1["Low"].
-0001c850: 696c 6f63 5b30 5d20 3e20 6461 7932 5b22  iloc[0] > day2["
-0001c860: 4c6f 7722 5d2e 696c 6f63 5b30 5d29 0a20  Low"].iloc[0]). 
-0001c870: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
-0001c880: 6461 7932 5b22 4c6f 7722 5d2e 696c 6f63  day2["Low"].iloc
-0001c890: 5b30 5d20 3e20 6461 7933 5b22 4c6f 7722  [0] > day3["Low"
-0001c8a0: 5d2e 696c 6f63 5b30 5d29 0a20 2020 2020  ].iloc[0]).     
-0001c8b0: 2020 2029 0a20 2020 2020 2020 2068 6967     ).        hig
-0001c8c0: 6865 7243 6c6f 7365 203d 2028 0a20 2020  herClose = (.   
-0001c8d0: 2020 2020 2020 2020 2028 6461 7930 5b22           (day0["
-0001c8e0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-0001c8f0: 3e20 6461 7931 5b22 436c 6f73 6522 5d2e  > day1["Close"].
-0001c900: 696c 6f63 5b30 5d29 0a20 2020 2020 2020  iloc[0]).       
-0001c910: 2020 2020 2061 6e64 2028 6461 7931 5b22       and (day1["
-0001c920: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-0001c930: 3e20 6461 7932 5b22 436c 6f73 6522 5d2e  > day2["Close"].
-0001c940: 696c 6f63 5b30 5d29 0a20 2020 2020 2020  iloc[0]).       
-0001c950: 2020 2020 2061 6e64 2028 6461 7932 5b22       and (day2["
-0001c960: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
-0001c970: 3e20 6461 7933 5b22 436c 6f73 6522 5d2e  > day3["Close"].
-0001c980: 696c 6f63 5b30 5d29 0a20 2020 2020 2020  iloc[0]).       
-0001c990: 2029 0a20 2020 2020 2020 2023 2068 6967   ).        # hig
-0001c9a0: 6865 7252 5349 203d 2028 6461 7930 5b22  herRSI = (day0["
-0001c9b0: 5253 4922 5d2e 696c 6f63 5b30 5d20 3e20  RSI"].iloc[0] > 
-0001c9c0: 6461 7931 5b22 5253 4922 5d2e 696c 6f63  day1["RSI"].iloc
-0001c9d0: 5b30 5d29 2061 6e64 205c 0a20 2020 2020  [0]) and \.     
-0001c9e0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0001c9f0: 2020 2020 2028 6461 7931 5b22 5253 4922       (day1["RSI"
-0001ca00: 5d2e 696c 6f63 5b30 5d20 3e20 6461 7932  ].iloc[0] > day2
-0001ca10: 5b22 5253 4922 5d2e 696c 6f63 5b30 5d29  ["RSI"].iloc[0])
-0001ca20: 2061 6e64 205c 0a20 2020 2020 2020 2023   and \.        #
-0001ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca40: 2028 6461 7932 5b22 5253 4922 5d2e 696c   (day2["RSI"].il
-0001ca50: 6f63 5b30 5d20 3e20 6461 7933 5b22 5253  oc[0] > day3["RS
-0001ca60: 4922 5d2e 696c 6f63 5b30 5d29 2061 6e64  I"].iloc[0]) and
-0001ca70: 205c 0a20 2020 2020 2020 2023 2020 2020   \.        #    
-0001ca80: 2020 2020 2020 2020 2020 2020 2064 6179               day
-0001ca90: 335b 2252 5349 225d 2e69 6c6f 635b 305d  3["RSI"].iloc[0]
-0001caa0: 203e 3d20 3530 2061 6e64 2064 6179 305b   >= 50 and day0[
-0001cab0: 2252 5349 225d 2e69 6c6f 635b 305d 203e  "RSI"].iloc[0] >
-0001cac0: 3d20 3635 0a20 2020 2020 2020 2072 6576  = 65.        rev
-0001cad0: 6572 7365 6444 6174 6120 3d20 6461 7461  ersedData = data
-0001cae0: 5b3a 3a2d 315d 2e63 6f70 7928 290a 2020  [::-1].copy().  
-0001caf0: 2020 2020 2020 7265 7665 7273 6564 4461        reversedDa
-0001cb00: 7461 5b22 5355 5045 5254 225d 203d 2070  ta["SUPERT"] = p
-0001cb10: 6b74 616c 6962 2e73 7570 6572 7472 656e  ktalib.supertren
-0001cb20: 6428 7265 7665 7273 6564 4461 7461 2c20  d(reversedData, 
-0001cb30: 372c 2033 295b 2253 5550 4552 545f 375f  7, 3)["SUPERT_7_
-0001cb40: 332e 3022 5d0a 2020 2020 2020 2020 7265  3.0"].        re
-0001cb50: 7665 7273 6564 4461 7461 5b22 454d 4138  versedData["EMA8
-0001cb60: 225d 203d 2070 6b74 616c 6962 2e45 4d41  "] = pktalib.EMA
-0001cb70: 2872 6576 6572 7365 6444 6174 615b 2243  (reversedData["C
-0001cb80: 6c6f 7365 225d 2c20 7469 6d65 7065 7269  lose"], timeperi
-0001cb90: 6f64 3d39 290a 2020 2020 2020 2020 6869  od=9).        hi
-0001cba0: 6768 6572 436c 6f73 6520 3d20 280a 2020  gherClose = (.  
-0001cbb0: 2020 2020 2020 2020 2020 6869 6768 6572            higher
-0001cbc0: 436c 6f73 650a 2020 2020 2020 2020 2020  Close.          
-0001cbd0: 2020 616e 6420 6461 7930 5b22 436c 6f73    and day0["Clos
-0001cbe0: 6522 5d2e 696c 6f63 5b30 5d20 3e20 7265  e"].iloc[0] > re
-0001cbf0: 7665 7273 6564 4461 7461 2e74 6169 6c28  versedData.tail(
-0001cc00: 3129 5b22 5355 5045 5254 225d 2e69 6c6f  1)["SUPERT"].ilo
-0001cc10: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
-0001cc20: 2061 6e64 2064 6179 305b 2243 6c6f 7365   and day0["Close
-0001cc30: 225d 2e69 6c6f 635b 305d 203e 2072 6576  "].iloc[0] > rev
-0001cc40: 6572 7365 6444 6174 612e 7461 696c 2831  ersedData.tail(1
-0001cc50: 295b 2245 4d41 3822 5d2e 696c 6f63 5b30  )["EMA8"].iloc[0
-0001cc60: 5d0a 2020 2020 2020 2020 290a 2020 2020  ].        ).    
-0001cc70: 2020 2020 7265 7475 726e 2068 6967 6865      return highe
-0001cc80: 7248 6967 6873 2061 6e64 2068 6967 6865  rHighs and highe
-0001cc90: 724c 6f77 7320 616e 6420 6869 6768 6572  rLows and higher
-0001cca0: 436c 6f73 650a 0a20 2020 2023 406d 6561  Close..    #@mea
-0001ccb0: 7375 7265 5f74 696d 650a 2020 2020 2320  sure_time.    # 
-0001ccc0: 5661 6c69 6461 7465 2027 496e 7369 6465  Validate 'Inside
-0001ccd0: 2042 6172 2720 7374 7275 6374 7572 6520   Bar' structure 
-0001cce0: 666f 7220 7265 6365 6e74 2064 6179 730a  for recent days.
-0001ccf0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0001cd00: 496e 7369 6465 4261 7228 0a20 2020 2020  InsideBar(.     
-0001cd10: 2020 2073 656c 662c 2064 662c 2073 6372     self, df, scr
-0001cd20: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-0001cd30: 742c 2063 6861 7274 5061 7474 6572 6e3d  t, chartPattern=
-0001cd40: 312c 2064 6179 7354 6f4c 6f6f 6b62 6163  1, daysToLookbac
-0001cd50: 6b3d 350a 2020 2020 293a 0a20 2020 2020  k=5.    ):.     
-0001cd60: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
-0001cd70: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
-0001cd80: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0001cd90: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-0001cda0: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-0001cdb0: 7928 290a 2020 2020 2020 2020 6f72 6744  y().        orgD
-0001cdc0: 6174 6120 3d20 6461 7461 0a20 2020 2020  ata = data.     
-0001cdd0: 2020 2073 6176 6564 203d 2073 656c 662e     saved = self.
-0001cde0: 6669 6e64 4375 7272 656e 7453 6176 6564  findCurrentSaved
-0001cdf0: 5661 6c75 6528 7363 7265 656e 4469 6374  Value(screenDict
-0001ce00: 2c20 7361 7665 4469 6374 2c20 2250 6174  , saveDict, "Pat
-0001ce10: 7465 726e 2229 0a20 2020 2020 2020 2066  tern").        f
-0001ce20: 6f72 2069 2069 6e20 7261 6e67 6528 696e  or i in range(in
-0001ce30: 7428 6461 7973 546f 4c6f 6f6b 6261 636b  t(daysToLookback
-0001ce40: 292c 2069 6e74 2872 6f75 6e64 2864 6179  ), int(round(day
-0001ce50: 7354 6f4c 6f6f 6b62 6163 6b20 2a20 302e  sToLookback * 0.
-0001ce60: 3529 2920 2d20 312c 202d 3129 3a0a 2020  5)) - 1, -1):.  
-0001ce70: 2020 2020 2020 2020 2020 6966 2069 203d            if i =
-0001ce80: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
-0001ce90: 2020 2020 2072 6574 7572 6e20 3020 2023       return 0  #
-0001cea0: 2045 7869 7420 6966 206f 6e6c 7920 6c61   Exit if only la
-0001ceb0: 7374 2032 2063 616e 646c 6573 2061 7265  st 2 candles are
-0001cec0: 206c 6566 740a 2020 2020 2020 2020 2020   left.          
-0001ced0: 2020 6966 2063 6861 7274 5061 7474 6572    if chartPatter
-0001cee0: 6e20 3d3d 2031 3a0a 2020 2020 2020 2020  n == 1:.        
-0001cef0: 2020 2020 2020 2020 6966 2022 5570 2220          if "Up" 
-0001cf00: 696e 2073 6176 6544 6963 745b 2254 7265  in saveDict["Tre
-0001cf10: 6e64 225d 2061 6e64 2028 0a20 2020 2020  nd"] and (.     
-0001cf20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001cf30: 4275 6c6c 2220 696e 2073 6176 6544 6963  Bull" in saveDic
-0001cf40: 745b 224d 412d 5369 676e 616c 225d 0a20  t["MA-Signal"]. 
-0001cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cf60: 2020 206f 7220 2253 7570 706f 7274 2220     or "Support" 
-0001cf70: 696e 2073 6176 6544 6963 745b 224d 412d  in saveDict["MA-
-0001cf80: 5369 676e 616c 225d 0a20 2020 2020 2020  Signal"].       
-0001cf90: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
-0001cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cfb0: 6461 7461 203d 206f 7267 4461 7461 2e68  data = orgData.h
-0001cfc0: 6561 6428 6929 0a20 2020 2020 2020 2020  ead(i).         
-0001cfd0: 2020 2020 2020 2020 2020 2072 6566 4361             refCa
-0001cfe0: 6e64 6c65 203d 2064 6174 612e 7461 696c  ndle = data.tail
-0001cff0: 2831 290a 2020 2020 2020 2020 2020 2020  (1).            
-0001d000: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-0001d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d020: 2020 2020 2028 6c65 6e28 6461 7461 2e48       (len(data.H
-0001d030: 6967 685b 6461 7461 2e48 6967 6820 3e20  igh[data.High > 
-0001d040: 7265 6643 616e 646c 652e 4869 6768 2e69  refCandle.High.i
-0001d050: 7465 6d28 295d 2920 3d3d 2030 290a 2020  tem()]) == 0).  
-0001d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d070: 2020 2020 2020 616e 6420 286c 656e 2864        and (len(d
-0001d080: 6174 612e 4c6f 775b 6461 7461 2e4c 6f77  ata.Low[data.Low
-0001d090: 203c 2072 6566 4361 6e64 6c65 2e4c 6f77   < refCandle.Low
-0001d0a0: 2e69 7465 6d28 295d 2920 3d3d 2030 290a  .item()]) == 0).
-0001d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d0c0: 2020 2020 2020 2020 616e 6420 286c 656e          and (len
-0001d0d0: 2864 6174 612e 4f70 656e 5b64 6174 612e  (data.Open[data.
-0001d0e0: 4f70 656e 203e 2072 6566 4361 6e64 6c65  Open > refCandle
-0001d0f0: 2e48 6967 682e 6974 656d 2829 5d29 203d  .High.item()]) =
-0001d100: 3d20 3029 0a20 2020 2020 2020 2020 2020  = 0).           
-0001d110: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-0001d120: 2028 6c65 6e28 6461 7461 2e43 6c6f 7365   (len(data.Close
-0001d130: 5b64 6174 612e 436c 6f73 6520 3c20 7265  [data.Close < re
-0001d140: 6643 616e 646c 652e 4c6f 772e 6974 656d  fCandle.Low.item
-0001d150: 2829 5d29 203d 3d20 3029 0a20 2020 2020  ()]) == 0).     
-0001d160: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001d170: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001d180: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-0001d190: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-0001d1a0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0001d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1c0: 7361 7665 645b 305d 0a20 2020 2020 2020  saved[0].       
-0001d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1e0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001d1f0: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
-0001d200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d210: 2020 2b20 636f 6c6f 7254 6578 742e 5741    + colorText.WA
-0001d220: 524e 0a20 2020 2020 2020 2020 2020 2020  RN.             
-0001d230: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001d240: 2028 2249 6e73 6964 6520 4261 7220 2825   ("Inside Bar (%
-0001d250: 6429 2220 2520 6929 0a20 2020 2020 2020  d)" % i).       
-0001d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d270: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001d280: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
-0001d290: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0001d2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d2b0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-0001d2c0: 2250 6174 7465 726e 225d 203d 2073 6176  "Pattern"] = sav
-0001d2d0: 6564 5b31 5d20 2b20 2249 6e73 6964 6520  ed[1] + "Inside 
-0001d2e0: 4261 7220 2825 6429 2220 2520 690a 2020  Bar (%d)" % i.  
-0001d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d300: 2020 2020 2020 7265 7475 726e 2069 0a20        return i. 
-0001d310: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0001d320: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0001d330: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0001d340: 300a 2020 2020 2020 2020 2020 2020 656c  0.            el
-0001d350: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001d360: 2020 2020 6966 2022 446f 776e 2220 696e      if "Down" in
-0001d370: 2073 6176 6544 6963 745b 2254 7265 6e64   saveDict["Trend
-0001d380: 225d 2061 6e64 2028 0a20 2020 2020 2020  "] and (.       
-0001d390: 2020 2020 2020 2020 2020 2020 2022 4265               "Be
-0001d3a0: 6172 2220 696e 2073 6176 6544 6963 745b  ar" in saveDict[
-0001d3b0: 224d 412d 5369 676e 616c 225d 206f 7220  "MA-Signal"] or 
-0001d3c0: 2252 6573 6973 7422 2069 6e20 7361 7665  "Resist" in save
-0001d3d0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
-0001d3e0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0001d3f0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-0001d400: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-0001d410: 6f72 6744 6174 612e 6865 6164 2869 290a  orgData.head(i).
-0001d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d430: 2020 2020 7265 6643 616e 646c 6520 3d20      refCandle = 
-0001d440: 6461 7461 2e74 6169 6c28 3129 0a20 2020  data.tail(1).   
-0001d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d460: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-0001d470: 2020 2020 2020 2020 2020 2020 2020 286c                (l
-0001d480: 656e 2864 6174 612e 4869 6768 5b64 6174  en(data.High[dat
-0001d490: 612e 4869 6768 203e 2072 6566 4361 6e64  a.High > refCand
-0001d4a0: 6c65 2e48 6967 682e 6974 656d 2829 5d29  le.High.item()])
-0001d4b0: 203d 3d20 3029 0a20 2020 2020 2020 2020   == 0).         
-0001d4c0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001d4d0: 6e64 2028 6c65 6e28 6461 7461 2e4c 6f77  nd (len(data.Low
-0001d4e0: 5b64 6174 612e 4c6f 7720 3c20 7265 6643  [data.Low < refC
-0001d4f0: 616e 646c 652e 4c6f 772e 6974 656d 2829  andle.Low.item()
-0001d500: 5d29 203d 3d20 3029 0a20 2020 2020 2020  ]) == 0).       
-0001d510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d520: 2061 6e64 2028 6c65 6e28 6461 7461 2e4f   and (len(data.O
-0001d530: 7065 6e5b 6461 7461 2e4f 7065 6e20 3e20  pen[data.Open > 
-0001d540: 7265 6643 616e 646c 652e 4869 6768 2e69  refCandle.High.i
-0001d550: 7465 6d28 295d 2920 3d3d 2030 290a 2020  tem()]) == 0).  
-0001d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d570: 2020 2020 2020 616e 6420 286c 656e 2864        and (len(d
-0001d580: 6174 612e 436c 6f73 655b 6461 7461 2e43  ata.Close[data.C
-0001d590: 6c6f 7365 203c 2072 6566 4361 6e64 6c65  lose < refCandle
-0001d5a0: 2e4c 6f77 2e69 7465 6d28 295d 2920 3d3d  .Low.item()]) ==
-0001d5b0: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
-0001d5c0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-0001d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5e0: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
-0001d5f0: 6174 7465 726e 225d 203d 2028 0a20 2020  attern"] = (.   
-0001d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d610: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-0001d620: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0001d630: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001d640: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
-0001d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d660: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-0001d670: 6f72 5465 7874 2e57 4152 4e0a 2020 2020  orText.WARN.    
-0001d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d690: 2020 2020 2020 2020 2b20 2822 496e 7369          + ("Insi
-0001d6a0: 6465 2042 6172 2028 2564 2922 2025 2069  de Bar (%d)" % i
-0001d6b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001d6c0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001d6d0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
+00019970: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00019980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019990: 2020 2072 6573 756c 745f 6466 2e72 6573     result_df.res
+000199a0: 6574 5f69 6e64 6578 2864 726f 703d 5472  et_index(drop=Tr
+000199b0: 7565 2c20 696e 706c 6163 653d 5472 7565  ue, inplace=True
+000199c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000199d0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+000199e0: 6570 7469 6f6e 2061 7320 653a 2020 2320  eption as e:  # 
+000199f0: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+00019a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019a10: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00019a20: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
+00019a30: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
+00019a40: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00019a50: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+00019a60: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00019a70: 2020 2020 2020 2320 5468 656e 2075 7064        # Then upd
+00019a80: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
+00019a90: 2020 2020 2020 2020 6c61 7374 5f73 6967          last_sig
+00019aa0: 6e61 6c5b 6461 7461 5f6c 6973 745b 636e  nal[data_list[cn
+00019ab0: 745d 5d20 3d20 5b66 696e 616c 5d0a 2020  t]] = [final].  
+00019ac0: 2020 2020 2020 6966 2072 6573 756c 745f        if result_
+00019ad0: 6466 2069 7320 6e6f 7420 4e6f 6e65 3a0a  df is not None:.
+00019ae0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00019af0: 6c74 5f64 662e 6472 6f70 5f64 7570 6c69  lt_df.drop_dupli
+00019b00: 6361 7465 7328 6b65 6570 3d22 6c61 7374  cates(keep="last
+00019b10: 222c 2069 6e70 6c61 6365 3d54 7275 6529  ", inplace=True)
+00019b20: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00019b30: 756c 745f 6466 2e73 6f72 745f 7661 6c75  ult_df.sort_valu
+00019b40: 6573 2862 793d 2254 696d 6522 2c20 696e  es(by="Time", in
+00019b50: 706c 6163 653d 5472 7565 290a 2020 2020  place=True).    
+00019b60: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00019b70: 745f 6466 5b3a 3a2d 315d 0a0a 2020 2020  t_df[::-1]..    
+00019b80: 2320 5072 6570 726f 6365 7373 2074 6865  # Preprocess the
+00019b90: 2061 6371 7569 7265 6420 6461 7461 0a20   acquired data. 
+00019ba0: 2020 2064 6566 2070 7265 7072 6f63 6573     def preproces
+00019bb0: 7344 6174 6128 7365 6c66 2c20 6466 2c20  sData(self, df, 
+00019bc0: 6461 7973 546f 4c6f 6f6b 6261 636b 3d4e  daysToLookback=N
+00019bd0: 6f6e 6529 3a0a 2020 2020 2020 2020 6173  one):.        as
+00019be0: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
+00019bf0: 6466 2c20 7064 2e44 6174 6146 7261 6d65  df, pd.DataFrame
+00019c00: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
+00019c10: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
+00019c20: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00019c30: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+00019c40: 7265 706c 6163 6528 6e70 2e69 6e66 2c20  replace(np.inf, 
+00019c50: 6e70 2e6e 616e 292e 7265 706c 6163 6528  np.nan).replace(
+00019c60: 2d6e 702e 696e 662c 206e 702e 6e61 6e29  -np.inf, np.nan)
+00019c70: 2e64 726f 706e 6128 686f 773d 2261 6c6c  .dropna(how="all
+00019c80: 2229 0a20 2020 2020 2020 2020 2020 2023  ").            #
+00019c90: 2073 656c 662e 6465 6661 756c 745f 6c6f   self.default_lo
+00019ca0: 6767 6572 2e69 6e66 6f28 6622 5072 6570  gger.info(f"Prep
+00019cb0: 726f 6365 7373 696e 6720 6461 7461 3a5c  rocessing data:\
+00019cc0: 6e7b 6461 7461 2e68 6561 6428 3129 7d5c  n{data.head(1)}\
+00019cd0: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+00019ce0: 6966 2064 6179 7354 6f4c 6f6f 6b62 6163  if daysToLookbac
+00019cf0: 6b20 6973 204e 6f6e 653a 0a20 2020 2020  k is None:.     
+00019d00: 2020 2020 2020 2020 2020 2064 6179 7354             daysT
+00019d10: 6f4c 6f6f 6b62 6163 6b20 3d20 7365 6c66  oLookback = self
+00019d20: 2e63 6f6e 6669 674d 616e 6167 6572 2e64  .configManager.d
+00019d30: 6179 7354 6f4c 6f6f 6b62 6163 6b0a 2020  aysToLookback.  
+00019d40: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00019d50: 662e 636f 6e66 6967 4d61 6e61 6765 722e  f.configManager.
+00019d60: 7573 6545 4d41 3a0a 2020 2020 2020 2020  useEMA:.        
+00019d70: 2020 2020 2020 2020 736d 6120 3d20 706b          sma = pk
+00019d80: 7461 6c69 622e 454d 4128 6461 7461 5b22  talib.EMA(data["
+00019d90: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
+00019da0: 696f 643d 3530 290a 2020 2020 2020 2020  iod=50).        
+00019db0: 2020 2020 2020 2020 6c6d 6120 3d20 706b          lma = pk
+00019dc0: 7461 6c69 622e 454d 4128 6461 7461 5b22  talib.EMA(data["
+00019dd0: 436c 6f73 6522 5d2c 2074 696d 6570 6572  Close"], timeper
+00019de0: 696f 643d 3230 3029 0a20 2020 2020 2020  iod=200).       
+00019df0: 2020 2020 2020 2020 2073 736d 6120 3d20           ssma = 
+00019e00: 706b 7461 6c69 622e 454d 4128 6461 7461  pktalib.EMA(data
+00019e10: 5b22 436c 6f73 6522 5d2c 2074 696d 6570  ["Close"], timep
+00019e20: 6572 696f 643d 3929 0a20 2020 2020 2020  eriod=9).       
+00019e30: 2020 2020 2020 2020 2073 736d 6132 3020           ssma20 
+00019e40: 3d20 706b 7461 6c69 622e 454d 4128 6461  = pktalib.EMA(da
+00019e50: 7461 5b22 436c 6f73 6522 5d2c 2074 696d  ta["Close"], tim
+00019e60: 6570 6572 696f 643d 3230 290a 2020 2020  eperiod=20).    
+00019e70: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00019e80: 2e69 6e73 6572 7428 6c65 6e28 6461 7461  .insert(len(data
+00019e90: 2e63 6f6c 756d 6e73 292c 2022 534d 4122  .columns), "SMA"
+00019ea0: 2c20 736d 6129 0a20 2020 2020 2020 2020  , sma).         
+00019eb0: 2020 2020 2020 2064 6174 612e 696e 7365         data.inse
+00019ec0: 7274 286c 656e 2864 6174 612e 636f 6c75  rt(len(data.colu
+00019ed0: 6d6e 7329 2c20 224c 4d41 222c 206c 6d61  mns), "LMA", lma
+00019ee0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00019ef0: 2020 6461 7461 2e69 6e73 6572 7428 6c65    data.insert(le
+00019f00: 6e28 6461 7461 2e63 6f6c 756d 6e73 292c  n(data.columns),
+00019f10: 2022 5353 4d41 222c 2073 736d 6129 0a20   "SSMA", ssma). 
+00019f20: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00019f30: 6174 612e 696e 7365 7274 286c 656e 2864  ata.insert(len(d
+00019f40: 6174 612e 636f 6c75 6d6e 7329 2c20 2253  ata.columns), "S
+00019f50: 534d 4132 3022 2c20 7373 6d61 3230 290a  SMA20", ssma20).
+00019f60: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00019f70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00019f80: 2020 736d 6120 3d20 706b 7461 6c69 622e    sma = pktalib.
+00019f90: 534d 4128 6461 7461 5b22 436c 6f73 6522  SMA(data["Close"
+00019fa0: 5d2c 2074 696d 6570 6572 696f 643d 3530  ], timeperiod=50
+00019fb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00019fc0: 2020 6c6d 6120 3d20 706b 7461 6c69 622e    lma = pktalib.
+00019fd0: 534d 4128 6461 7461 5b22 436c 6f73 6522  SMA(data["Close"
+00019fe0: 5d2c 2074 696d 6570 6572 696f 643d 3230  ], timeperiod=20
+00019ff0: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+0001a000: 2020 2073 736d 6120 3d20 706b 7461 6c69     ssma = pktali
+0001a010: 622e 534d 4128 6461 7461 5b22 436c 6f73  b.SMA(data["Clos
+0001a020: 6522 5d2c 2074 696d 6570 6572 696f 643d  e"], timeperiod=
+0001a030: 3929 0a20 2020 2020 2020 2020 2020 2020  9).             
+0001a040: 2020 2073 736d 6132 3020 3d20 706b 7461     ssma20 = pkta
+0001a050: 6c69 622e 534d 4128 6461 7461 5b22 436c  lib.SMA(data["Cl
+0001a060: 6f73 6522 5d2c 2074 696d 6570 6572 696f  ose"], timeperio
+0001a070: 643d 3230 290a 2020 2020 2020 2020 2020  d=20).          
+0001a080: 2020 2020 2020 6461 7461 2e69 6e73 6572        data.inser
+0001a090: 7428 6c65 6e28 6461 7461 2e63 6f6c 756d  t(len(data.colum
+0001a0a0: 6e73 292c 2022 534d 4122 2c20 736d 6129  ns), "SMA", sma)
+0001a0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a0c0: 2064 6174 612e 696e 7365 7274 286c 656e   data.insert(len
+0001a0d0: 2864 6174 612e 636f 6c75 6d6e 7329 2c20  (data.columns), 
+0001a0e0: 224c 4d41 222c 206c 6d61 290a 2020 2020  "LMA", lma).    
+0001a0f0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0001a100: 2e69 6e73 6572 7428 6c65 6e28 6461 7461  .insert(len(data
+0001a110: 2e63 6f6c 756d 6e73 292c 2022 5353 4d41  .columns), "SSMA
+0001a120: 222c 2073 736d 6129 0a20 2020 2020 2020  ", ssma).       
+0001a130: 2020 2020 2020 2020 2064 6174 612e 696e           data.in
+0001a140: 7365 7274 286c 656e 2864 6174 612e 636f  sert(len(data.co
+0001a150: 6c75 6d6e 7329 2c20 2253 534d 4132 3022  lumns), "SSMA20"
+0001a160: 2c20 7373 6d61 3230 290a 2020 2020 2020  , ssma20).      
+0001a170: 2020 2020 2020 766f 6c20 3d20 706b 7461        vol = pkta
+0001a180: 6c69 622e 534d 4128 6461 7461 5b22 566f  lib.SMA(data["Vo
+0001a190: 6c75 6d65 225d 2c20 7469 6d65 7065 7269  lume"], timeperi
+0001a1a0: 6f64 3d32 3029 0a20 2020 2020 2020 2020  od=20).         
+0001a1b0: 2020 2072 7369 203d 2070 6b74 616c 6962     rsi = pktalib
+0001a1c0: 2e52 5349 2864 6174 615b 2243 6c6f 7365  .RSI(data["Close
+0001a1d0: 225d 2c20 7469 6d65 7065 7269 6f64 3d31  "], timeperiod=1
+0001a1e0: 3429 0a20 2020 2020 2020 2020 2020 2064  4).            d
+0001a1f0: 6174 612e 696e 7365 7274 286c 656e 2864  ata.insert(len(d
+0001a200: 6174 612e 636f 6c75 6d6e 7329 2c20 2256  ata.columns), "V
+0001a210: 6f6c 4d41 222c 2076 6f6c 290a 2020 2020  olMA", vol).    
+0001a220: 2020 2020 2020 2020 6461 7461 2e69 6e73          data.ins
+0001a230: 6572 7428 6c65 6e28 6461 7461 2e63 6f6c  ert(len(data.col
+0001a240: 756d 6e73 292c 2022 5253 4922 2c20 7273  umns), "RSI", rs
+0001a250: 6929 0a20 2020 2020 2020 2020 2020 2063  i).            c
+0001a260: 6369 203d 2070 6b74 616c 6962 2e43 4349  ci = pktalib.CCI
+0001a270: 2864 6174 615b 2248 6967 6822 5d2c 2064  (data["High"], d
+0001a280: 6174 615b 224c 6f77 225d 2c20 6461 7461  ata["Low"], data
+0001a290: 5b22 436c 6f73 6522 5d2c 2074 696d 6570  ["Close"], timep
+0001a2a0: 6572 696f 643d 3134 290a 2020 2020 2020  eriod=14).      
+0001a2b0: 2020 2020 2020 6461 7461 2e69 6e73 6572        data.inser
+0001a2c0: 7428 6c65 6e28 6461 7461 2e63 6f6c 756d  t(len(data.colum
+0001a2d0: 6e73 292c 2022 4343 4922 2c20 6363 6929  ns), "CCI", cci)
+0001a2e0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+0001a2f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001a300: 2020 6661 7374 6b2c 2066 6173 7464 203d    fastk, fastd =
+0001a310: 2070 6b74 616c 6962 2e53 544f 4348 5253   pktalib.STOCHRS
+0001a320: 4928 0a20 2020 2020 2020 2020 2020 2020  I(.             
+0001a330: 2020 2020 2020 2064 6174 615b 2243 6c6f         data["Clo
+0001a340: 7365 225d 2c20 7469 6d65 7065 7269 6f64  se"], timeperiod
+0001a350: 3d31 342c 2066 6173 746b 5f70 6572 696f  =14, fastk_perio
+0001a360: 643d 352c 2066 6173 7464 5f70 6572 696f  d=5, fastd_perio
+0001a370: 643d 332c 2066 6173 7464 5f6d 6174 7970  d=3, fastd_matyp
+0001a380: 653d 300a 2020 2020 2020 2020 2020 2020  e=0.            
+0001a390: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0001a3a0: 2020 2020 2020 6461 7461 2e69 6e73 6572        data.inser
+0001a3b0: 7428 6c65 6e28 6461 7461 2e63 6f6c 756d  t(len(data.colum
+0001a3c0: 6e73 292c 2022 4641 5354 4b22 2c20 6661  ns), "FASTK", fa
+0001a3d0: 7374 6b29 0a20 2020 2020 2020 2020 2020  stk).           
+0001a3e0: 2020 2020 2064 6174 612e 696e 7365 7274       data.insert
+0001a3f0: 286c 656e 2864 6174 612e 636f 6c75 6d6e  (len(data.column
+0001a400: 7329 2c20 2246 4153 5444 222c 2066 6173  s), "FASTD", fas
+0001a410: 7464 290a 2020 2020 2020 2020 2020 2020  td).            
+0001a420: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+0001a430: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+0001a440: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
+0001a450: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
+0001a460: 2865 2c20 6578 635f 696e 666f 3d54 7275  (e, exc_info=Tru
+0001a470: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0001a480: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
+0001a490: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+0001a4a0: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+0001a4b0: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
+0001a4c0: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
+0001a4d0: 2865 2c20 6578 635f 696e 666f 3d54 7275  (e, exc_info=Tru
+0001a4e0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0001a4f0: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
+0001a500: 6461 7461 203d 2064 6174 615b 3a3a 2d31  data = data[::-1
+0001a510: 5d20 2023 2052 6576 6572 7365 2074 6865  ]  # Reverse the
+0001a520: 2064 6174 6166 7261 6d65 0a20 2020 2020   dataframe.     
+0001a530: 2020 2023 2064 6174 6120 3d20 6461 7461     # data = data
+0001a540: 2e66 696c 6c6e 6128 3029 0a20 2020 2020  .fillna(0).     
+0001a550: 2020 2023 2064 6174 6120 3d20 6461 7461     # data = data
+0001a560: 2e72 6570 6c61 6365 285b 6e70 2e69 6e66  .replace([np.inf
+0001a570: 2c20 2d6e 702e 696e 665d 2c20 3029 0a20  , -np.inf], 0). 
+0001a580: 2020 2020 2020 2066 756c 6c44 6174 6120         fullData 
+0001a590: 3d20 6461 7461 0a20 2020 2020 2020 2074  = data.        t
+0001a5a0: 7269 6d6d 6564 4461 7461 203d 2064 6174  rimmedData = dat
+0001a5b0: 612e 6865 6164 2864 6179 7354 6f4c 6f6f  a.head(daysToLoo
+0001a5c0: 6b62 6163 6b29 0a20 2020 2020 2020 2072  kback).        r
+0001a5d0: 6574 7572 6e20 2866 756c 6c44 6174 612c  eturn (fullData,
+0001a5e0: 2074 7269 6d6d 6564 4461 7461 290a 0a20   trimmedData).. 
+0001a5f0: 2020 2023 2056 616c 6964 6174 6520 6966     # Validate if
+0001a600: 2074 6865 2073 746f 636b 2069 7320 6275   the stock is bu
+0001a610: 6c6c 6973 6820 696e 2074 6865 2073 686f  llish in the sho
+0001a620: 7274 2074 6572 6d0a 2020 2020 6465 6620  rt term.    def 
+0001a630: 7661 6c69 6461 7465 3135 4d69 6e75 7465  validate15Minute
+0001a640: 5072 6963 6556 6f6c 756d 6542 7265 616b  PriceVolumeBreak
+0001a650: 6f75 7428 7365 6c66 2c20 6466 293a 0a20  out(self, df):. 
+0001a660: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
+0001a670: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
+0001a680: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+0001a690: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+0001a6a0: 2020 2020 2020 2023 2068 7474 7073 3a2f         # https:/
+0001a6b0: 2f63 6861 7274 696e 6b2e 636f 6d2f 7363  /chartink.com/sc
+0001a6c0: 7265 656e 6572 2f31 352d 6d69 6e2d 7072  reener/15-min-pr
+0001a6d0: 6963 652d 766f 6c75 6d65 2d62 7265 616b  ice-volume-break
+0001a6e0: 6f75 740a 2020 2020 2020 2020 6461 7461  out.        data
+0001a6f0: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
+0001a700: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+0001a710: 2e66 696c 6c6e 6128 3029 0a20 2020 2020  .fillna(0).     
+0001a720: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+0001a730: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
+0001a740: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
+0001a750: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+0001a760: 5b3a 3a2d 315d 2020 2320 5265 7665 7273  [::-1]  # Revers
+0001a770: 6520 7468 6520 6461 7461 6672 616d 6520  e the dataframe 
+0001a780: 736f 2074 6861 7420 6974 7320 7468 6520  so that its the 
+0001a790: 6f6c 6465 7374 2064 6174 6520 6669 7273  oldest date firs
+0001a7a0: 740a 2020 2020 2020 2020 6461 7461 5b22  t.        data["
+0001a7b0: 534d 4132 3022 5d20 3d20 706b 7461 6c69  SMA20"] = pktali
+0001a7c0: 622e 534d 4128 6461 7461 5b22 436c 6f73  b.SMA(data["Clos
+0001a7d0: 6522 5d2c 2032 3029 0a20 2020 2020 2020  e"], 20).       
+0001a7e0: 2064 6174 615b 2253 4d41 3230 5622 5d20   data["SMA20V"] 
+0001a7f0: 3d20 706b 7461 6c69 622e 534d 4128 6461  = pktalib.SMA(da
+0001a800: 7461 5b22 566f 6c75 6d65 225d 2c20 3230  ta["Volume"], 20
+0001a810: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
+0001a820: 2064 6174 615b 0a20 2020 2020 2020 2020   data[.         
+0001a830: 2020 203a 3a2d 310a 2020 2020 2020 2020     ::-1.        
+0001a840: 5d20 2023 2052 6576 6572 7365 2074 6865  ]  # Reverse the
+0001a850: 2064 6174 6166 7261 6d65 2073 6f20 7468   dataframe so th
+0001a860: 6174 2069 7427 7320 7468 6520 6d6f 7374  at it's the most
+0001a870: 2072 6563 656e 7420 6461 7465 2066 6972   recent date fir
+0001a880: 7374 0a20 2020 2020 2020 2072 6563 656e  st.        recen
+0001a890: 7420 3d20 6461 7461 2e68 6561 6428 3329  t = data.head(3)
+0001a8a0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+0001a8b0: 7265 6365 6e74 2920 3c20 333a 0a20 2020  recent) < 3:.   
+0001a8c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001a8d0: 4661 6c73 650a 2020 2020 2020 2020 636f  False.        co
+0001a8e0: 6e64 3120 3d20 7265 6365 6e74 5b22 436c  nd1 = recent["Cl
+0001a8f0: 6f73 6522 5d2e 696c 6f63 5b30 5d20 3e20  ose"].iloc[0] > 
+0001a900: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
+0001a910: 696c 6f63 5b31 5d0a 2020 2020 2020 2020  iloc[1].        
+0001a920: 636f 6e64 3220 3d20 636f 6e64 3120 616e  cond2 = cond1 an
+0001a930: 6420 2872 6563 656e 745b 2243 6c6f 7365  d (recent["Close
+0001a940: 225d 2e69 6c6f 635b 305d 203e 2072 6563  "].iloc[0] > rec
+0001a950: 656e 745b 2253 4d41 3230 225d 2e69 6c6f  ent["SMA20"].ilo
+0001a960: 635b 305d 290a 2020 2020 2020 2020 636f  c[0]).        co
+0001a970: 6e64 3320 3d20 636f 6e64 3220 616e 6420  nd3 = cond2 and 
+0001a980: 2872 6563 656e 745b 2243 6c6f 7365 225d  (recent["Close"]
+0001a990: 2e69 6c6f 635b 315d 203e 2072 6563 656e  .iloc[1] > recen
+0001a9a0: 745b 2248 6967 6822 5d2e 696c 6f63 5b32  t["High"].iloc[2
+0001a9b0: 5d29 0a20 2020 2020 2020 2063 6f6e 6434  ]).        cond4
+0001a9c0: 203d 2063 6f6e 6433 2061 6e64 2028 7265   = cond3 and (re
+0001a9d0: 6365 6e74 5b22 566f 6c75 6d65 225d 2e69  cent["Volume"].i
+0001a9e0: 6c6f 635b 305d 203e 2072 6563 656e 745b  loc[0] > recent[
+0001a9f0: 2253 4d41 3230 5622 5d2e 696c 6f63 5b30  "SMA20V"].iloc[0
+0001aa00: 5d29 0a20 2020 2020 2020 2063 6f6e 6435  ]).        cond5
+0001aa10: 203d 2063 6f6e 6434 2061 6e64 2028 7265   = cond4 and (re
+0001aa20: 6365 6e74 5b22 566f 6c75 6d65 225d 2e69  cent["Volume"].i
+0001aa30: 6c6f 635b 315d 203e 2072 6563 656e 745b  loc[1] > recent[
+0001aa40: 2253 4d41 3230 5622 5d2e 696c 6f63 5b30  "SMA20V"].iloc[0
+0001aa50: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+0001aa60: 6e20 636f 6e64 350a 0a20 2020 2064 6566  n cond5..    def
+0001aa70: 2076 616c 6964 6174 6542 756c 6c69 7368   validateBullish
+0001aa80: 466f 7254 6f6d 6f72 726f 7728 7365 6c66  ForTomorrow(self
+0001aa90: 2c20 6466 293a 0a20 2020 2020 2020 2069  , df):.        i
+0001aaa0: 6620 6466 2069 7320 4e6f 6e65 206f 7220  f df is None or 
+0001aab0: 6c65 6e28 6466 2920 3d3d 2030 3a0a 2020  len(df) == 0:.  
+0001aac0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001aad0: 2046 616c 7365 0a20 2020 2020 2020 2064   False.        d
+0001aae0: 6174 6120 3d20 6466 2e63 6f70 7928 290a  ata = df.copy().
+0001aaf0: 2020 2020 2020 2020 2320 6874 7470 733a          # https:
+0001ab00: 2f2f 6368 6172 7469 6e6b 2e63 6f6d 2f73  //chartink.com/s
+0001ab10: 6372 6565 6e65 722f 6275 6c6c 6973 682d  creener/bullish-
+0001ab20: 666f 722d 746f 6d6f 7272 6f77 0a20 2020  for-tomorrow.   
+0001ab30: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+0001ab40: 2e66 696c 6c6e 6128 3029 0a20 2020 2020  .fillna(0).     
+0001ab50: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+0001ab60: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
+0001ab70: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
+0001ab80: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+0001ab90: 5b3a 3a2d 315d 2020 2320 5265 7665 7273  [::-1]  # Revers
+0001aba0: 6520 7468 6520 6461 7461 6672 616d 6520  e the dataframe 
+0001abb0: 736f 2074 6861 7420 6974 7320 7468 6520  so that its the 
+0001abc0: 6f6c 6465 7374 2064 6174 6520 6669 7273  oldest date firs
+0001abd0: 740a 2020 2020 2020 2020 6d61 6364 4c69  t.        macdLi
+0001abe0: 6e65 203d 2070 6b74 616c 6962 2e4d 4143  ne = pktalib.MAC
+0001abf0: 4428 6461 7461 5b22 436c 6f73 6522 5d2c  D(data["Close"],
+0001ac00: 2031 322c 2032 362c 2039 295b 305d 2e74   12, 26, 9)[0].t
+0001ac10: 6169 6c28 3329 0a20 2020 2020 2020 206d  ail(3).        m
+0001ac20: 6163 6453 6967 6e61 6c20 3d20 706b 7461  acdSignal = pkta
+0001ac30: 6c69 622e 4d41 4344 2864 6174 615b 2243  lib.MACD(data["C
+0001ac40: 6c6f 7365 225d 2c20 3132 2c20 3236 2c20  lose"], 12, 26, 
+0001ac50: 3929 5b31 5d2e 7461 696c 2833 290a 2020  9)[1].tail(3).  
+0001ac60: 2020 2020 2020 6d61 6364 4869 7374 203d        macdHist =
+0001ac70: 2070 6b74 616c 6962 2e4d 4143 4428 6461   pktalib.MACD(da
+0001ac80: 7461 5b22 436c 6f73 6522 5d2c 2031 322c  ta["Close"], 12,
+0001ac90: 2032 362c 2039 295b 325d 2e74 6169 6c28   26, 9)[2].tail(
+0001aca0: 3329 0a0a 2020 2020 2020 2020 7265 7475  3)..        retu
+0001acb0: 726e 2028 0a20 2020 2020 2020 2020 2020  rn (.           
+0001acc0: 2028 6d61 6364 4869 7374 2e69 6c6f 635b   (macdHist.iloc[
+0001acd0: 3a31 5d2e 696c 6f63 5b30 5d20 3c20 6d61  :1].iloc[0] < ma
+0001ace0: 6364 4869 7374 2e69 6c6f 635b 3a32 5d2e  cdHist.iloc[:2].
+0001acf0: 696c 6f63 5b31 5d29 0a20 2020 2020 2020  iloc[1]).       
+0001ad00: 2020 2020 2061 6e64 2028 6d61 6364 4869       and (macdHi
+0001ad10: 7374 2e69 6c6f 635b 3a33 5d2e 696c 6f63  st.iloc[:3].iloc
+0001ad20: 5b32 5d20 3e20 6d61 6364 4869 7374 2e69  [2] > macdHist.i
+0001ad30: 6c6f 635b 3a32 5d2e 696c 6f63 5b31 5d29  loc[:2].iloc[1])
+0001ad40: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001ad50: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0001ad60: 2020 2028 6d61 6364 4c69 6e65 2e69 6c6f     (macdLine.ilo
+0001ad70: 635b 3a33 5d2e 696c 6f63 5b32 5d20 2d20  c[:3].iloc[2] - 
+0001ad80: 6d61 6364 5369 676e 616c 2e69 6c6f 635b  macdSignal.iloc[
+0001ad90: 3a33 5d2e 696c 6f63 5b32 5d29 0a20 2020  :3].iloc[2]).   
+0001ada0: 2020 2020 2020 2020 2020 2020 202d 2028               - (
+0001adb0: 6d61 6364 4c69 6e65 2e69 6c6f 635b 3a32  macdLine.iloc[:2
+0001adc0: 5d2e 696c 6f63 5b31 5d20 2d20 6d61 6364  ].iloc[1] - macd
+0001add0: 5369 676e 616c 2e69 6c6f 635b 3a32 5d2e  Signal.iloc[:2].
+0001ade0: 696c 6f63 5b31 5d29 0a20 2020 2020 2020  iloc[1]).       
+0001adf0: 2020 2020 2020 2020 203e 3d20 302e 340a           >= 0.4.
+0001ae00: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0001ae10: 2020 2020 2020 2020 2020 616e 6420 280a            and (.
+0001ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae30: 286d 6163 644c 696e 652e 696c 6f63 5b3a  (macdLine.iloc[:
+0001ae40: 325d 2e69 6c6f 635b 315d 202d 206d 6163  2].iloc[1] - mac
+0001ae50: 6453 6967 6e61 6c2e 696c 6f63 5b3a 325d  dSignal.iloc[:2]
+0001ae60: 2e69 6c6f 635b 315d 290a 2020 2020 2020  .iloc[1]).      
+0001ae70: 2020 2020 2020 2020 2020 2d20 286d 6163            - (mac
+0001ae80: 644c 696e 652e 696c 6f63 5b3a 315d 2e69  dLine.iloc[:1].i
+0001ae90: 6c6f 635b 305d 202d 206d 6163 6453 6967  loc[0] - macdSig
+0001aea0: 6e61 6c2e 696c 6f63 5b3a 315d 2e69 6c6f  nal.iloc[:1].ilo
+0001aeb0: 635b 305d 290a 2020 2020 2020 2020 2020  c[0]).          
+0001aec0: 2020 2020 2020 3c3d 2030 2e32 0a20 2020        <= 0.2.   
+0001aed0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0001aee0: 2020 2020 2020 2061 6e64 2028 6d61 6364         and (macd
+0001aef0: 4c69 6e65 2e69 6c6f 635b 3a33 5d2e 696c  Line.iloc[:3].il
+0001af00: 6f63 5b32 5d20 3e20 6d61 6364 5369 676e  oc[2] > macdSign
+0001af10: 616c 2e69 6c6f 635b 3a33 5d2e 696c 6f63  al.iloc[:3].iloc
+0001af20: 5b32 5d29 0a20 2020 2020 2020 2020 2020  [2]).           
+0001af30: 2061 6e64 2028 0a20 2020 2020 2020 2020   and (.         
+0001af40: 2020 2020 2020 2028 6d61 6364 4c69 6e65         (macdLine
+0001af50: 2e69 6c6f 635b 3a33 5d2e 696c 6f63 5b32  .iloc[:3].iloc[2
+0001af60: 5d20 2d20 6d61 6364 5369 676e 616c 2e69  ] - macdSignal.i
+0001af70: 6c6f 635b 3a33 5d2e 696c 6f63 5b32 5d29  loc[:3].iloc[2])
+0001af80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001af90: 202d 2028 6d61 6364 4c69 6e65 2e69 6c6f   - (macdLine.ilo
+0001afa0: 635b 3a32 5d2e 696c 6f63 5b31 5d20 2d20  c[:2].iloc[1] - 
+0001afb0: 6d61 6364 5369 676e 616c 2e69 6c6f 635b  macdSignal.iloc[
+0001afc0: 3a32 5d2e 696c 6f63 5b31 5d29 0a20 2020  :2].iloc[1]).   
+0001afd0: 2020 2020 2020 2020 2020 2020 203c 2031               < 1
+0001afe0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0001aff0: 2020 2020 2020 2029 0a0a 2020 2020 2340         )..    #@
+0001b000: 6d65 6173 7572 655f 7469 6d65 0a20 2020  measure_time.   
+0001b010: 2023 2076 616c 6964 6174 6520 6966 2043   # validate if C
+0001b020: 4349 2069 7320 7769 7468 696e 2067 6976  CI is within giv
+0001b030: 656e 2072 616e 6765 0a20 2020 2064 6566  en range.    def
+0001b040: 2076 616c 6964 6174 6543 4349 2873 656c   validateCCI(sel
+0001b050: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+0001b060: 742c 2073 6176 6544 6963 742c 206d 696e  t, saveDict, min
+0001b070: 4343 492c 206d 6178 4343 4929 3a0a 2020  CCI, maxCCI):.  
+0001b080: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
+0001b090: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
+0001b0a0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+0001b0b0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+0001b0c0: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+0001b0d0: 636f 7079 2829 0a20 2020 2020 2020 2064  copy().        d
+0001b0e0: 6174 6120 3d20 6461 7461 2e66 696c 6c6e  ata = data.filln
+0001b0f0: 6128 3029 0a20 2020 2020 2020 2064 6174  a(0).        dat
+0001b100: 6120 3d20 6461 7461 2e72 6570 6c61 6365  a = data.replace
+0001b110: 285b 6e70 2e69 6e66 2c20 2d6e 702e 696e  ([np.inf, -np.in
+0001b120: 665d 2c20 3029 0a20 2020 2020 2020 2063  f], 0).        c
+0001b130: 6369 203d 2069 6e74 2864 6174 612e 6865  ci = int(data.he
+0001b140: 6164 2831 295b 2243 4349 225d 2e69 6c6f  ad(1)["CCI"].ilo
+0001b150: 635b 305d 290a 2020 2020 2020 2020 7361  c[0]).        sa
+0001b160: 7665 4469 6374 5b22 4343 4922 5d20 3d20  veDict["CCI"] = 
+0001b170: 6363 690a 2020 2020 2020 2020 6966 2028  cci.        if (
+0001b180: 6363 6920 3e3d 206d 696e 4343 4920 616e  cci >= minCCI an
+0001b190: 6420 6363 6920 3c3d 206d 6178 4343 4929  d cci <= maxCCI)
+0001b1a0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0001b1b0: 2028 2255 7022 2069 6e20 7361 7665 4469   ("Up" in saveDi
+0001b1c0: 6374 5b22 5472 656e 6422 5d29 3a0a 2020  ct["Trend"]):.  
+0001b1d0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+0001b1e0: 7265 656e 4469 6374 5b22 4343 4922 5d20  reenDict["CCI"] 
+0001b1f0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0001b200: 2020 2020 2020 2020 2863 6f6c 6f72 5465          (colorTe
+0001b210: 7874 2e42 4f4c 4420 6966 2028 2253 7472  xt.BOLD if ("Str
+0001b220: 6f6e 6722 2069 6e20 7361 7665 4469 6374  ong" in saveDict
+0001b230: 5b22 5472 656e 6422 5d29 2065 6c73 6520  ["Trend"]) else 
+0001b240: 2222 2920 2b20 636f 6c6f 7254 6578 742e  "") + colorText.
+0001b250: 4752 4545 4e20 2b20 7374 7228 6363 6929  GREEN + str(cci)
+0001b260: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+0001b270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b280: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
+0001b290: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0001b2a0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001b2b0: 2243 4349 225d 203d 2028 0a20 2020 2020  "CCI"] = (.     
+0001b2c0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+0001b2d0: 636f 6c6f 7254 6578 742e 424f 4c44 2069  colorText.BOLD i
+0001b2e0: 6620 2822 5374 726f 6e67 2220 696e 2073  f ("Strong" in s
+0001b2f0: 6176 6544 6963 745b 2254 7265 6e64 225d  aveDict["Trend"]
+0001b300: 2920 656c 7365 2022 2229 202b 2063 6f6c  ) else "") + col
+0001b310: 6f72 5465 7874 2e46 4149 4c20 2b20 7374  orText.FAIL + st
+0001b320: 7228 6363 6929 202b 2063 6f6c 6f72 5465  r(cci) + colorTe
+0001b330: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
+0001b340: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0001b350: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+0001b360: 0a20 2020 2020 2020 2073 6372 6565 6e44  .        screenD
+0001b370: 6963 745b 2243 4349 225d 203d 2063 6f6c  ict["CCI"] = col
+0001b380: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
+0001b390: 6c6f 7254 6578 742e 4641 494c 202b 2073  lorText.FAIL + s
+0001b3a0: 7472 2863 6369 2920 2b20 636f 6c6f 7254  tr(cci) + colorT
+0001b3b0: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+0001b3c0: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
+0001b3d0: 2020 2320 4669 6e64 2043 6f6e 666c 7563    # Find Confluc
+0001b3e0: 656e 6365 0a20 2020 2064 6566 2076 616c  ence.    def val
+0001b3f0: 6964 6174 6543 6f6e 666c 7565 6e63 6528  idateConfluence(
+0001b400: 7365 6c66 2c20 7374 6f63 6b2c 2064 662c  self, stock, df,
+0001b410: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
+0001b420: 6544 6963 742c 2070 6572 6365 6e74 6167  eDict, percentag
+0001b430: 653d 302e 312c 636f 6e66 4669 6c74 6572  e=0.1,confFilter
+0001b440: 3d33 293a 0a20 2020 2020 2020 2069 6620  =3):.        if 
+0001b450: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
+0001b460: 6e28 6466 2920 3d3d 2030 3a0a 2020 2020  n(df) == 0:.    
+0001b470: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0001b480: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
+0001b490: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
+0001b4a0: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
+0001b4b0: 6174 612e 6865 6164 2832 290a 2020 2020  ata.head(2).    
+0001b4c0: 2020 2020 6966 206c 656e 2872 6563 656e      if len(recen
+0001b4d0: 7429 203c 2032 3a0a 2020 2020 2020 2020  t) < 2:.        
+0001b4e0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+0001b4f0: 0a20 2020 2020 2020 2069 7335 3044 4d41  .        is50DMA
+0001b500: 5570 5472 656e 6420 3d20 2872 6563 656e  UpTrend = (recen
+0001b510: 745b 2253 4d41 225d 2e69 6c6f 635b 305d  t["SMA"].iloc[0]
+0001b520: 203e 2072 6563 656e 745b 2253 4d41 225d   > recent["SMA"]
+0001b530: 2e69 6c6f 635b 315d 290a 2020 2020 2020  .iloc[1]).      
+0001b540: 2020 6973 3530 444d 4144 6f77 6e54 7265    is50DMADownTre
+0001b550: 6e64 203d 2028 7265 6365 6e74 5b22 534d  nd = (recent["SM
+0001b560: 4122 5d2e 696c 6f63 5b30 5d20 3c20 7265  A"].iloc[0] < re
+0001b570: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
+0001b580: 5b31 5d29 0a20 2020 2020 2020 2069 7332  [1]).        is2
+0001b590: 3044 4d41 4372 6f73 736f 7665 7235 3044  0DMACrossover50D
+0001b5a0: 4d41 203d 2028 7265 6365 6e74 5b22 5353  MA = (recent["SS
+0001b5b0: 4d41 3230 225d 2e69 6c6f 635b 305d 203e  MA20"].iloc[0] >
+0001b5c0: 3d20 7265 6365 6e74 5b22 534d 4122 5d2e  = recent["SMA"].
+0001b5d0: 696c 6f63 5b30 5d29 2061 6e64 205c 0a20  iloc[0]) and \. 
+0001b5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b5f0: 2020 2020 2020 2020 2020 2028 7265 6365             (rece
+0001b600: 6e74 5b22 5353 4d41 3230 225d 2e69 6c6f  nt["SSMA20"].ilo
+0001b610: 635b 315d 203c 3d20 7265 6365 6e74 5b22  c[1] <= recent["
+0001b620: 534d 4122 5d2e 696c 6f63 5b31 5d29 0a20  SMA"].iloc[1]). 
+0001b630: 2020 2020 2020 2069 7335 3044 4d41 4372         is50DMACr
+0001b640: 6f73 736f 7665 7232 3030 444d 4120 3d20  ossover200DMA = 
+0001b650: 2872 6563 656e 745b 2253 4d41 225d 2e69  (recent["SMA"].i
+0001b660: 6c6f 635b 305d 203e 3d20 7265 6365 6e74  loc[0] >= recent
+0001b670: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d29  ["LMA"].iloc[0])
+0001b680: 2061 6e64 205c 0a20 2020 2020 2020 2020   and \.         
+0001b690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b6a0: 2020 2028 7265 6365 6e74 5b22 534d 4122     (recent["SMA"
+0001b6b0: 5d2e 696c 6f63 5b31 5d20 3c3d 2072 6563  ].iloc[1] <= rec
+0001b6c0: 656e 745b 224c 4d41 225d 2e69 6c6f 635b  ent["LMA"].iloc[
+0001b6d0: 315d 290a 2020 2020 2020 2020 6973 476f  1]).        isGo
+0001b6e0: 6c64 656e 4372 6f73 734f 7665 7220 3d20  ldenCrossOver = 
+0001b6f0: 6973 3230 444d 4143 726f 7373 6f76 6572  is20DMACrossover
+0001b700: 3530 444d 4120 6f72 2069 7335 3044 4d41  50DMA or is50DMA
+0001b710: 4372 6f73 736f 7665 7232 3030 444d 410a  Crossover200DMA.
+0001b720: 2020 2020 2020 2020 6973 3530 444d 4143          is50DMAC
+0001b730: 726f 7373 6f76 6572 3230 3044 4d41 446f  rossover200DMADo
+0001b740: 776e 203d 2028 7265 6365 6e74 5b22 534d  wn = (recent["SM
+0001b750: 4122 5d2e 696c 6f63 5b30 5d20 3c3d 2072  A"].iloc[0] <= r
+0001b760: 6563 656e 745b 224c 4d41 225d 2e69 6c6f  ecent["LMA"].ilo
+0001b770: 635b 305d 2920 616e 6420 5c0a 2020 2020  c[0]) and \.    
+0001b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b790: 2020 2020 2020 2020 2872 6563 656e 745b          (recent[
+0001b7a0: 2253 4d41 225d 2e69 6c6f 635b 315d 203e  "SMA"].iloc[1] >
+0001b7b0: 3d20 7265 6365 6e74 5b22 4c4d 4122 5d2e  = recent["LMA"].
+0001b7c0: 696c 6f63 5b31 5d29 0a20 2020 2020 2020  iloc[1]).       
+0001b7d0: 2069 7332 3044 4d41 4372 6f73 736f 7665   is20DMACrossove
+0001b7e0: 7235 3044 4d41 446f 776e 203d 2028 7265  r50DMADown = (re
+0001b7f0: 6365 6e74 5b22 5353 4d41 3230 225d 2e69  cent["SSMA20"].i
+0001b800: 6c6f 635b 305d 203c 3d20 7265 6365 6e74  loc[0] <= recent
+0001b810: 5b22 534d 4122 5d2e 696c 6f63 5b30 5d29  ["SMA"].iloc[0])
+0001b820: 2061 6e64 205c 0a20 2020 2020 2020 2020   and \.         
+0001b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b840: 2020 2028 7265 6365 6e74 5b22 5353 4d41     (recent["SSMA
+0001b850: 3230 225d 2e69 6c6f 635b 315d 203e 3d20  20"].iloc[1] >= 
+0001b860: 7265 6365 6e74 5b22 534d 4122 5d2e 696c  recent["SMA"].il
+0001b870: 6f63 5b31 5d29 0a20 2020 2020 2020 2069  oc[1]).        i
+0001b880: 7344 6561 6443 726f 7373 4f76 6572 203d  sDeadCrossOver =
+0001b890: 2069 7332 3044 4d41 4372 6f73 736f 7665   is20DMACrossove
+0001b8a0: 7235 3044 4d41 446f 776e 206f 7220 6973  r50DMADown or is
+0001b8b0: 3530 444d 4143 726f 7373 6f76 6572 3230  50DMACrossover20
+0001b8c0: 3044 4d41 446f 776e 0a20 2020 2020 2020  0DMADown.       
+0001b8d0: 2064 6561 6478 4f76 6572 5465 7874 203d   deadxOverText =
+0001b8e0: 2066 2744 6561 6443 726f 7373 6f76 6572   f'DeadCrossover
+0001b8f0: 7b22 2832 3029 2220 6966 2069 7332 3044  {"(20)" if is20D
+0001b900: 4d41 4372 6f73 736f 7665 7235 3044 4d41  MACrossover50DMA
+0001b910: 446f 776e 2065 6c73 6520 2822 2835 3029  Down else ("(50)
+0001b920: 2220 6966 2069 7335 3044 4d41 4372 6f73  " if is50DMACros
+0001b930: 736f 7665 7232 3030 444d 4144 6f77 6e20  sover200DMADown 
+0001b940: 656c 7365 2022 2229 7d27 0a20 2020 2020  else "")}'.     
+0001b950: 2020 2067 6f6c 6465 6e78 4f76 6572 5465     goldenxOverTe
+0001b960: 7874 203d 2066 2747 6f6c 6465 6e43 726f  xt = f'GoldenCro
+0001b970: 7373 6f76 6572 7b22 2832 3029 2220 6966  ssover{"(20)" if
+0001b980: 2069 7332 3044 4d41 4372 6f73 736f 7665   is20DMACrossove
+0001b990: 7235 3044 4d41 2065 6c73 6520 2822 2835  r50DMA else ("(5
+0001b9a0: 3029 2220 6966 2069 7335 3044 4d41 4372  0)" if is50DMACr
+0001b9b0: 6f73 736f 7665 7232 3030 444d 4120 656c  ossover200DMA el
+0001b9c0: 7365 2022 2229 7d27 0a20 2020 2020 2020  se "")}'.       
+0001b9d0: 2069 7335 3044 4d41 203d 2028 7265 6365   is50DMA = (rece
+0001b9e0: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b30  nt["SMA"].iloc[0
+0001b9f0: 5d20 3c3d 2072 6563 656e 745b 2243 6c6f  ] <= recent["Clo
+0001ba00: 7365 225d 2e69 6c6f 635b 305d 290a 2020  se"].iloc[0]).  
+0001ba10: 2020 2020 2020 6973 3230 3044 4d41 203d        is200DMA =
+0001ba20: 2028 7265 6365 6e74 5b22 4c4d 4122 5d2e   (recent["LMA"].
+0001ba30: 696c 6f63 5b30 5d20 3c3d 2072 6563 656e  iloc[0] <= recen
+0001ba40: 745b 2243 6c6f 7365 225d 2e69 6c6f 635b  t["Close"].iloc[
+0001ba50: 305d 290a 2020 2020 2020 2020 6b65 7931  0]).        key1
+0001ba60: 203d 2022 534d 4122 0a20 2020 2020 2020   = "SMA".       
+0001ba70: 206b 6579 3220 3d20 224c 4d41 220a 2020   key2 = "LMA".  
+0001ba80: 2020 2020 2020 6966 2069 7332 3044 4d41        if is20DMA
+0001ba90: 4372 6f73 736f 7665 7235 3044 4d41 206f  Crossover50DMA o
+0001baa0: 7220 6973 3230 444d 4143 726f 7373 6f76  r is20DMACrossov
+0001bab0: 6572 3530 444d 4144 6f77 6e3a 0a20 2020  er50DMADown:.   
+0001bac0: 2020 2020 2020 2020 206b 6579 3120 3d20           key1 = 
+0001bad0: 2253 534d 4132 3022 0a20 2020 2020 2020  "SSMA20".       
+0001bae0: 2020 2020 206b 6579 3220 3d20 2253 4d41       key2 = "SMA
+0001baf0: 220a 2020 2020 2020 2020 6469 6666 6572  ".        differ
+0001bb00: 656e 6365 203d 2072 6f75 6e64 2828 7265  ence = round((re
+0001bb10: 6365 6e74 5b6b 6579 315d 2e69 6c6f 635b  cent[key1].iloc[
+0001bb20: 305d 202d 2072 6563 656e 745b 6b65 7932  0] - recent[key2
+0001bb30: 5d2e 696c 6f63 5b30 5d29 0a20 2020 2020  ].iloc[0]).     
+0001bb40: 2020 2020 2020 2020 2020 202f 2072 6563             / rec
+0001bb50: 656e 745b 2243 6c6f 7365 225d 2e69 6c6f  ent["Close"].ilo
+0001bb60: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
+0001bb70: 2020 2020 202a 2031 3030 2c0a 2020 2020       * 100,.    
+0001bb80: 2020 2020 2020 2020 2020 2020 322c 0a20              2,. 
+0001bb90: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001bba0: 2020 2020 2073 6176 6544 6963 745b 2243       saveDict["C
+0001bbb0: 6f6e 6644 4d41 4469 6666 6572 656e 6365  onfDMADifference
+0001bbc0: 225d 203d 2064 6966 6665 7265 6e63 650a  "] = difference.
+0001bbd0: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+0001bbe0: 6374 5b22 436f 6e66 444d 4144 6966 6665  ct["ConfDMADiffe
+0001bbf0: 7265 6e63 6522 5d20 3d20 6469 6666 6572  rence"] = differ
+0001bc00: 656e 6365 0a20 2020 2020 2020 2073 6176  ence.        sav
+0001bc10: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
+0001bc20: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
+0001bc30: 7363 7265 656e 4469 6374 2c73 6176 6544  screenDict,saveD
+0001bc40: 6963 742c 224d 412d 5369 676e 616c 2229  ict,"MA-Signal")
+0001bc50: 0a20 2020 2020 2020 2023 2064 6966 6665  .        # diffe
+0001bc60: 7265 6e63 6520 3d20 6162 7328 6469 6666  rence = abs(diff
+0001bc70: 6572 656e 6365 290a 2020 2020 2020 2020  erence).        
+0001bc80: 636f 6e66 5465 7874 203d 2066 227b 676f  confText = f"{go
+0001bc90: 6c64 656e 784f 7665 7254 6578 7420 6966  ldenxOverText if
+0001bca0: 2069 7347 6f6c 6465 6e43 726f 7373 4f76   isGoldenCrossOv
+0001bcb0: 6572 2065 6c73 6520 2864 6561 6478 4f76  er else (deadxOv
+0001bcc0: 6572 5465 7874 2069 6620 6973 4465 6164  erText if isDead
+0001bcd0: 4372 6f73 734f 7665 7220 656c 7365 2028  CrossOver else (
+0001bce0: 2743 6f6e 662e 5570 2720 6966 2069 7335  'Conf.Up' if is5
+0001bcf0: 3044 4d41 5570 5472 656e 6420 656c 7365  0DMAUpTrend else
+0001bd00: 2028 2743 6f6e 662e 446f 776e 2720 6966   ('Conf.Down' if
+0001bd10: 2069 7335 3044 4d41 446f 776e 5472 656e   is50DMADownTren
+0001bd20: 6420 656c 7365 2028 2735 3044 4d41 2720  d else ('50DMA' 
+0001bd30: 6966 2069 7335 3044 4d41 2065 6c73 6520  if is50DMA else 
+0001bd40: 2827 3230 3044 4d41 2720 6966 2069 7332  ('200DMA' if is2
+0001bd50: 3030 444d 4120 656c 7365 2027 556e 6b6e  00DMA else 'Unkn
+0001bd60: 6f77 6e27 2929 2929 297d 220a 2020 2020  own')))))}".    
+0001bd70: 2020 2020 6966 2061 6273 2872 6563 656e      if abs(recen
+0001bd80: 745b 6b65 7931 5d2e 696c 6f63 5b30 5d20  t[key1].iloc[0] 
+0001bd90: 2d20 7265 6365 6e74 5b6b 6579 325d 2e69  - recent[key2].i
+0001bda0: 6c6f 635b 305d 2920 3c3d 2028 0a20 2020  loc[0]) <= (.   
+0001bdb0: 2020 2020 2020 2020 2072 6563 656e 745b           recent[
+0001bdc0: 6b65 7931 5d2e 696c 6f63 5b30 5d20 2a20  key1].iloc[0] * 
+0001bdd0: 7065 7263 656e 7461 6765 0a20 2020 2020  percentage.     
+0001bde0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+0001bdf0: 2020 6966 2072 6563 656e 745b 6b65 7931    if recent[key1
+0001be00: 5d2e 696c 6f63 5b30 5d20 3e3d 2072 6563  ].iloc[0] >= rec
+0001be10: 656e 745b 6b65 7932 5d2e 696c 6f63 5b30  ent[key2].iloc[0
+0001be20: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0001be30: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
+0001be40: 412d 5369 676e 616c 225d 203d 2028 0a20  A-Signal"] = (. 
+0001be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be60: 2020 2073 6176 6564 5b30 5d20 0a20 2020     saved[0] .   
+0001be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be80: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+0001be90: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+0001bea0: 2020 2020 2020 2b20 2863 6f6c 6f72 5465        + (colorTe
+0001beb0: 7874 2e47 5245 454e 2069 6620 6973 3530  xt.GREEN if is50
+0001bec0: 444d 4155 7054 7265 6e64 2065 6c73 6520  DMAUpTrend else 
+0001bed0: 2863 6f6c 6f72 5465 7874 2e46 4149 4c20  (colorText.FAIL 
+0001bee0: 6966 2069 7335 3044 4d41 446f 776e 5472  if is50DMADownTr
+0001bef0: 656e 6420 656c 7365 2063 6f6c 6f72 5465  end else colorTe
+0001bf00: 7874 2e57 4152 4e29 290a 2020 2020 2020  xt.WARN)).      
+0001bf10: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001bf20: 6622 7b63 6f6e 6654 6578 747d 2028 7b64  f"{confText} ({d
+0001bf30: 6966 6665 7265 6e63 657d 2529 220a 2020  ifference}%)".  
+0001bf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf50: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+0001bf60: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+0001bf70: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001bf80: 2020 2020 7361 7665 4469 6374 5b22 4d41      saveDict["MA
+0001bf90: 2d53 6967 6e61 6c22 5d20 3d20 7361 7665  -Signal"] = save
+0001bfa0: 645b 315d 202b 2066 227b 636f 6e66 5465  d[1] + f"{confTe
+0001bfb0: 7874 7d20 287b 6469 6666 6572 656e 6365  xt} ({difference
+0001bfc0: 7d25 2922 0a20 2020 2020 2020 2020 2020  }%)".           
+0001bfd0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001bfe0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+0001bff0: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
+0001c000: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0001c010: 2020 2020 2020 2073 6176 6564 5b30 5d20         saved[0] 
+0001c020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c030: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+0001c040: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
+0001c050: 2020 2020 2020 2020 2020 2b20 2863 6f6c            + (col
+0001c060: 6f72 5465 7874 2e47 5245 454e 2069 6620  orText.GREEN if 
+0001c070: 6973 3530 444d 4155 7054 7265 6e64 2065  is50DMAUpTrend e
+0001c080: 6c73 6520 2863 6f6c 6f72 5465 7874 2e46  lse (colorText.F
+0001c090: 4149 4c20 6966 2069 7335 3044 4d41 446f  AIL if is50DMADo
+0001c0a0: 776e 5472 656e 6420 656c 7365 2063 6f6c  wnTrend else col
+0001c0b0: 6f72 5465 7874 2e57 4152 4e29 290a 2020  orText.WARN)).  
+0001c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c0d0: 2020 2b20 6622 7b63 6f6e 6654 6578 747d    + f"{confText}
+0001c0e0: 2028 7b64 6966 6665 7265 6e63 657d 2529   ({difference}%)
+0001c0f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0001c100: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+0001c110: 742e 454e 440a 2020 2020 2020 2020 2020  t.END.          
+0001c120: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001c130: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+0001c140: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
+0001c150: 7361 7665 645b 315d 202b 2066 227b 636f  saved[1] + f"{co
+0001c160: 6e66 5465 7874 7d20 287b 6469 6666 6572  nfText} ({differ
+0001c170: 656e 6365 7d25 2922 0a20 2020 2020 2020  ence}%)".       
+0001c180: 2020 2020 2072 6574 7572 6e20 636f 6e66       return conf
+0001c190: 4669 6c74 6572 203d 3d20 3320 6f72 205c  Filter == 3 or \
+0001c1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c1b0: 2028 636f 6e66 4669 6c74 6572 203d 3d20   (confFilter == 
+0001c1c0: 3120 616e 6420 2869 7335 3044 4d41 5570  1 and (is50DMAUp
+0001c1d0: 5472 656e 6420 6f72 2028 6973 476f 6c64  Trend or (isGold
+0001c1e0: 656e 4372 6f73 734f 7665 7220 6f72 2027  enCrossOver or '
+0001c1f0: 5570 2720 696e 2063 6f6e 6654 6578 7429  Up' in confText)
+0001c200: 2929 206f 7220 5c0a 2020 2020 2020 2020  )) or \.        
+0001c210: 2020 2020 2020 2020 2863 6f6e 6646 696c          (confFil
+0001c220: 7465 7220 3d3d 2032 2061 6e64 2028 6973  ter == 2 and (is
+0001c230: 3530 444d 4144 6f77 6e54 7265 6e64 206f  50DMADownTrend o
+0001c240: 7220 6973 4465 6164 4372 6f73 734f 7665  r isDeadCrossOve
+0001c250: 7220 6f72 2027 446f 776e 2720 696e 2063  r or 'Down' in c
+0001c260: 6f6e 6654 6578 7429 290a 2020 2020 2020  onfText)).      
+0001c270: 2020 2320 4d61 7962 6520 7468 6520 6469    # Maybe the di
+0001c280: 6666 6572 656e 6365 2069 7320 6e6f 7420  fference is not 
+0001c290: 7769 7468 696e 2074 6865 2072 616e 6765  within the range
+0001c2a0: 2c20 6275 7420 7765 2764 2073 7469 6c6c  , but we'd still
+0001c2b0: 206c 696b 6520 746f 206b 6565 7020 7468   like to keep th
+0001c2c0: 6520 7374 6f63 6b20 696e 0a20 2020 2020  e stock in.     
+0001c2d0: 2020 2023 2074 6865 206c 6973 7420 6966     # the list if
+0001c2e0: 2069 7427 7320 6120 676f 6c64 656e 2063   it's a golden c
+0001c2f0: 726f 7373 6f76 6572 206f 7220 6465 6164  rossover or dead
+0001c300: 2063 726f 7373 6f76 6572 0a20 2020 2020   crossover.     
+0001c310: 2020 2069 6620 6973 476f 6c64 656e 4372     if isGoldenCr
+0001c320: 6f73 734f 7665 7220 6f72 2069 7344 6561  ossOver or isDea
+0001c330: 6443 726f 7373 4f76 6572 3a0a 2020 2020  dCrossOver:.    
+0001c340: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+0001c350: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+0001c360: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0001c370: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+0001c380: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0001c390: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+0001c3a0: 742e 424f 4c44 0a20 2020 2020 2020 2020  t.BOLD.         
+0001c3b0: 2020 2020 2020 2020 2020 202b 2028 636f             + (co
+0001c3c0: 6c6f 7254 6578 742e 4752 4545 4e20 6966  lorText.GREEN if
+0001c3d0: 2069 7335 3044 4d41 5570 5472 656e 6420   is50DMAUpTrend 
+0001c3e0: 656c 7365 2028 636f 6c6f 7254 6578 742e  else (colorText.
+0001c3f0: 4641 494c 2069 6620 6973 3530 444d 4144  FAIL if is50DMAD
+0001c400: 6f77 6e54 7265 6e64 2065 6c73 6520 636f  ownTrend else co
+0001c410: 6c6f 7254 6578 742e 5741 524e 2929 0a20  lorText.WARN)). 
+0001c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c430: 2020 202b 2066 227b 636f 6e66 5465 7874     + f"{confText
+0001c440: 7d20 287b 6469 6666 6572 656e 6365 7d25  } ({difference}%
+0001c450: 2922 0a20 2020 2020 2020 2020 2020 2020  )".             
+0001c460: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+0001c470: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
+0001c480: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0001c490: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
+0001c4a0: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
+0001c4b0: 6564 5b31 5d20 2b20 6622 7b63 6f6e 6654  ed[1] + f"{confT
+0001c4c0: 6578 747d 2028 7b64 6966 6665 7265 6e63  ext} ({differenc
+0001c4d0: 657d 2529 220a 2020 2020 2020 2020 2020  e}%)".          
+0001c4e0: 2020 7265 7475 726e 2063 6f6e 6646 696c    return confFil
+0001c4f0: 7465 7220 3d3d 2033 206f 7220 5c0a 2020  ter == 3 or \.  
+0001c500: 2020 2020 2020 2020 2020 2020 2020 2863                (c
+0001c510: 6f6e 6646 696c 7465 7220 3d3d 2031 2061  onfFilter == 1 a
+0001c520: 6e64 2069 7347 6f6c 6465 6e43 726f 7373  nd isGoldenCross
+0001c530: 4f76 6572 2920 6f72 205c 0a20 2020 2020  Over) or \.     
+0001c540: 2020 2020 2020 2020 2020 2028 636f 6e66             (conf
+0001c550: 4669 6c74 6572 203d 3d20 3220 616e 6420  Filter == 2 and 
+0001c560: 6973 4465 6164 4372 6f73 734f 7665 7229  isDeadCrossOver)
+0001c570: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001c580: 4661 6c73 650a 0a20 2020 2023 406d 6561  False..    #@mea
+0001c590: 7375 7265 5f74 696d 650a 2020 2020 2320  sure_time.    # 
+0001c5a0: 5661 6c69 6461 7465 2069 6620 7368 6172  Validate if shar
+0001c5b0: 6520 7072 6963 6573 2061 7265 2063 6f6e  e prices are con
+0001c5c0: 736f 6c69 6461 7469 6e67 0a20 2020 2064  solidating.    d
+0001c5d0: 6566 2076 616c 6964 6174 6543 6f6e 736f  ef validateConso
+0001c5e0: 6c69 6461 7469 6f6e 2873 656c 662c 2064  lidation(self, d
+0001c5f0: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
+0001c600: 6176 6544 6963 742c 2070 6572 6365 6e74  aveDict, percent
+0001c610: 6167 653d 3130 293a 0a20 2020 2020 2020  age=10):.       
+0001c620: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
+0001c630: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
+0001c640: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001c650: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0001c660: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
+0001c670: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
+0001c680: 2064 6174 612e 6669 6c6c 6e61 2830 290a   data.fillna(0).
+0001c690: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0001c6a0: 6174 612e 7265 706c 6163 6528 5b6e 702e  ata.replace([np.
+0001c6b0: 696e 662c 202d 6e70 2e69 6e66 5d2c 2030  inf, -np.inf], 0
+0001c6c0: 290a 2020 2020 2020 2020 6863 203d 2064  ).        hc = d
+0001c6d0: 6174 612e 6465 7363 7269 6265 2829 5b22  ata.describe()["
+0001c6e0: 436c 6f73 6522 5d5b 226d 6178 225d 0a20  Close"]["max"]. 
+0001c6f0: 2020 2020 2020 206c 6320 3d20 6461 7461         lc = data
+0001c700: 2e64 6573 6372 6962 6528 295b 2243 6c6f  .describe()["Clo
+0001c710: 7365 225d 5b22 6d69 6e22 5d0a 2020 2020  se"]["min"].    
+0001c720: 2020 2020 6966 2028 6863 202d 206c 6329      if (hc - lc)
+0001c730: 203c 3d20 2868 6320 2a20 7065 7263 656e   <= (hc * percen
+0001c740: 7461 6765 202f 2031 3030 2920 616e 6420  tage / 100) and 
+0001c750: 2868 6320 2d20 6c63 2021 3d20 3029 3a0a  (hc - lc != 0):.
+0001c760: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+0001c770: 656e 4469 6374 5b22 436f 6e73 6f6c 2e22  enDict["Consol."
+0001c780: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
+0001c790: 2020 2020 2020 636f 6c6f 7254 6578 742e        colorText.
+0001c7a0: 424f 4c44 0a20 2020 2020 2020 2020 2020  BOLD.           
+0001c7b0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+0001c7c0: 2e47 5245 454e 0a20 2020 2020 2020 2020  .GREEN.         
+0001c7d0: 2020 2020 2020 202b 2022 5261 6e67 653a         + "Range:
+0001c7e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0001c7f0: 2020 2b20 7374 7228 726f 756e 6428 2861    + str(round((a
+0001c800: 6273 2828 6863 202d 206c 6329 202f 2068  bs((hc - lc) / h
+0001c810: 6329 202a 2031 3030 292c 2031 2929 0a20  c) * 100), 1)). 
+0001c820: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001c830: 2022 2522 0a20 2020 2020 2020 2020 2020   "%".           
+0001c840: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+0001c850: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
+0001c860: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
+0001c870: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
+0001c880: 6565 6e44 6963 745b 2243 6f6e 736f 6c2e  eenDict["Consol.
+0001c890: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
+0001c8a0: 2020 2020 2020 2063 6f6c 6f72 5465 7874         colorText
+0001c8b0: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
+0001c8c0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+0001c8d0: 742e 4641 494c 0a20 2020 2020 2020 2020  t.FAIL.         
+0001c8e0: 2020 2020 2020 202b 2022 5261 6e67 653a         + "Range:
+0001c8f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0001c900: 2020 2b20 7374 7228 726f 756e 6428 2861    + str(round((a
+0001c910: 6273 2828 6863 202d 206c 6329 202f 2068  bs((hc - lc) / h
+0001c920: 6329 202a 2031 3030 292c 2031 2929 0a20  c) * 100), 1)). 
+0001c930: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001c940: 2022 2522 0a20 2020 2020 2020 2020 2020   "%".           
+0001c950: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+0001c960: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
+0001c970: 2029 0a20 2020 2020 2020 2073 6176 6544   ).        saveD
+0001c980: 6963 745b 2243 6f6e 736f 6c2e 225d 203d  ict["Consol."] =
+0001c990: 2066 2752 616e 6765 3a7b 7374 7228 726f   f'Range:{str(ro
+0001c9a0: 756e 6428 2861 6273 2828 6863 2d6c 6329  und((abs((hc-lc)
+0001c9b0: 2f68 6329 2a31 3030 292c 3129 292b 2225  /hc)*100),1))+"%
+0001c9c0: 227d 270a 2020 2020 2020 2020 7265 7475  "}'.        retu
+0001c9d0: 726e 2072 6f75 6e64 2828 6162 7328 2868  rn round((abs((h
+0001c9e0: 6320 2d20 6c63 2920 2f20 6863 2920 2a20  c - lc) / hc) * 
+0001c9f0: 3130 3029 2c20 3129 0a0a 2020 2020 2320  100), 1)..    # 
+0001ca00: 7661 6c69 6461 7465 2069 6620 7468 6520  validate if the 
+0001ca10: 7374 6f63 6b20 6861 7320 6265 656e 2068  stock has been h
+0001ca20: 6176 696e 6720 6869 6768 6572 2068 6967  aving higher hig
+0001ca30: 6873 2c20 6869 6768 6572 206c 6f77 730a  hs, higher lows.
+0001ca40: 2020 2020 2320 616e 6420 6869 6768 6572      # and higher
+0001ca50: 2063 6c6f 7365 2077 6974 6820 6c61 7465   close with late
+0001ca60: 7374 2063 6c6f 7365 203e 2073 7570 6572  st close > super
+0001ca70: 7472 656e 6420 616e 6420 382d 454d 412e  trend and 8-EMA.
+0001ca80: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0001ca90: 6548 6967 6865 7248 6967 6873 4869 6768  eHigherHighsHigh
+0001caa0: 6572 4c6f 7773 4869 6768 6572 436c 6f73  erLowsHigherClos
+0001cab0: 6528 7365 6c66 2c20 6466 293a 0a20 2020  e(self, df):.   
+0001cac0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
+0001cad0: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
+0001cae0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0001caf0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+0001cb00: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
+0001cb10: 6f70 7928 290a 2020 2020 2020 2020 6461  opy().        da
+0001cb20: 7930 203d 2064 6174 610a 2020 2020 2020  y0 = data.      
+0001cb30: 2020 6461 7931 203d 2064 6174 615b 313a    day1 = data[1:
+0001cb40: 5d0a 2020 2020 2020 2020 6461 7932 203d  ].        day2 =
+0001cb50: 2064 6174 615b 323a 5d0a 2020 2020 2020   data[2:].      
+0001cb60: 2020 6461 7933 203d 2064 6174 615b 333a    day3 = data[3:
+0001cb70: 5d0a 2020 2020 2020 2020 6966 206c 656e  ].        if len
+0001cb80: 2864 6179 3129 203c 2031 206f 7220 6c65  (day1) < 1 or le
+0001cb90: 6e28 6461 7932 2920 3c20 3120 6f72 206c  n(day2) < 1 or l
+0001cba0: 656e 2864 6179 3329 203c 2031 3a0a 2020  en(day3) < 1:.  
+0001cbb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001cbc0: 2046 616c 7365 0a20 2020 2020 2020 2068   False.        h
+0001cbd0: 6967 6865 7248 6967 6873 203d 2028 0a20  igherHighs = (. 
+0001cbe0: 2020 2020 2020 2020 2020 2028 6461 7930             (day0
+0001cbf0: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
+0001cc00: 203e 2064 6179 315b 2248 6967 6822 5d2e   > day1["High"].
+0001cc10: 696c 6f63 5b30 5d29 0a20 2020 2020 2020  iloc[0]).       
+0001cc20: 2020 2020 2061 6e64 2028 6461 7931 5b22       and (day1["
+0001cc30: 4869 6768 225d 2e69 6c6f 635b 305d 203e  High"].iloc[0] >
+0001cc40: 2064 6179 325b 2248 6967 6822 5d2e 696c   day2["High"].il
+0001cc50: 6f63 5b30 5d29 0a20 2020 2020 2020 2020  oc[0]).         
+0001cc60: 2020 2061 6e64 2028 6461 7932 5b22 4869     and (day2["Hi
+0001cc70: 6768 225d 2e69 6c6f 635b 305d 203e 2064  gh"].iloc[0] > d
+0001cc80: 6179 335b 2248 6967 6822 5d2e 696c 6f63  ay3["High"].iloc
+0001cc90: 5b30 5d29 0a20 2020 2020 2020 2029 0a20  [0]).        ). 
+0001cca0: 2020 2020 2020 2068 6967 6865 724c 6f77         higherLow
+0001ccb0: 7320 3d20 280a 2020 2020 2020 2020 2020  s = (.          
+0001ccc0: 2020 2864 6179 305b 224c 6f77 225d 2e69    (day0["Low"].i
+0001ccd0: 6c6f 635b 305d 203e 2064 6179 315b 224c  loc[0] > day1["L
+0001cce0: 6f77 225d 2e69 6c6f 635b 305d 290a 2020  ow"].iloc[0]).  
+0001ccf0: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
+0001cd00: 6179 315b 224c 6f77 225d 2e69 6c6f 635b  ay1["Low"].iloc[
+0001cd10: 305d 203e 2064 6179 325b 224c 6f77 225d  0] > day2["Low"]
+0001cd20: 2e69 6c6f 635b 305d 290a 2020 2020 2020  .iloc[0]).      
+0001cd30: 2020 2020 2020 616e 6420 2864 6179 325b        and (day2[
+0001cd40: 224c 6f77 225d 2e69 6c6f 635b 305d 203e  "Low"].iloc[0] >
+0001cd50: 2064 6179 335b 224c 6f77 225d 2e69 6c6f   day3["Low"].ilo
+0001cd60: 635b 305d 290a 2020 2020 2020 2020 290a  c[0]).        ).
+0001cd70: 2020 2020 2020 2020 6869 6768 6572 436c          higherCl
+0001cd80: 6f73 6520 3d20 280a 2020 2020 2020 2020  ose = (.        
+0001cd90: 2020 2020 2864 6179 305b 2243 6c6f 7365      (day0["Close
+0001cda0: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
+0001cdb0: 315b 2243 6c6f 7365 225d 2e69 6c6f 635b  1["Close"].iloc[
+0001cdc0: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
+0001cdd0: 616e 6420 2864 6179 315b 2243 6c6f 7365  and (day1["Close
+0001cde0: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
+0001cdf0: 325b 2243 6c6f 7365 225d 2e69 6c6f 635b  2["Close"].iloc[
+0001ce00: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
+0001ce10: 616e 6420 2864 6179 325b 2243 6c6f 7365  and (day2["Close
+0001ce20: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
+0001ce30: 335b 2243 6c6f 7365 225d 2e69 6c6f 635b  3["Close"].iloc[
+0001ce40: 305d 290a 2020 2020 2020 2020 290a 2020  0]).        ).  
+0001ce50: 2020 2020 2020 2320 6869 6768 6572 5253        # higherRS
+0001ce60: 4920 3d20 2864 6179 305b 2252 5349 225d  I = (day0["RSI"]
+0001ce70: 2e69 6c6f 635b 305d 203e 2064 6179 315b  .iloc[0] > day1[
+0001ce80: 2252 5349 225d 2e69 6c6f 635b 305d 2920  "RSI"].iloc[0]) 
+0001ce90: 616e 6420 5c0a 2020 2020 2020 2020 2320  and \.        # 
+0001cea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ceb0: 2864 6179 315b 2252 5349 225d 2e69 6c6f  (day1["RSI"].ilo
+0001cec0: 635b 305d 203e 2064 6179 325b 2252 5349  c[0] > day2["RSI
+0001ced0: 225d 2e69 6c6f 635b 305d 2920 616e 6420  "].iloc[0]) and 
+0001cee0: 5c0a 2020 2020 2020 2020 2320 2020 2020  \.        #     
+0001cef0: 2020 2020 2020 2020 2020 2020 2864 6179              (day
+0001cf00: 325b 2252 5349 225d 2e69 6c6f 635b 305d  2["RSI"].iloc[0]
+0001cf10: 203e 2064 6179 335b 2252 5349 225d 2e69   > day3["RSI"].i
+0001cf20: 6c6f 635b 305d 2920 616e 6420 5c0a 2020  loc[0]) and \.  
+0001cf30: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0001cf40: 2020 2020 2020 2020 6461 7933 5b22 5253          day3["RS
+0001cf50: 4922 5d2e 696c 6f63 5b30 5d20 3e3d 2035  I"].iloc[0] >= 5
+0001cf60: 3020 616e 6420 6461 7930 5b22 5253 4922  0 and day0["RSI"
+0001cf70: 5d2e 696c 6f63 5b30 5d20 3e3d 2036 350a  ].iloc[0] >= 65.
+0001cf80: 2020 2020 2020 2020 7265 7665 7273 6564          reversed
+0001cf90: 4461 7461 203d 2064 6174 615b 3a3a 2d31  Data = data[::-1
+0001cfa0: 5d2e 636f 7079 2829 0a20 2020 2020 2020  ].copy().       
+0001cfb0: 2072 6576 6572 7365 6444 6174 615b 2253   reversedData["S
+0001cfc0: 5550 4552 5422 5d20 3d20 706b 7461 6c69  UPERT"] = pktali
+0001cfd0: 622e 7375 7065 7274 7265 6e64 2872 6576  b.supertrend(rev
+0001cfe0: 6572 7365 6444 6174 612c 2037 2c20 3329  ersedData, 7, 3)
+0001cff0: 5b22 5355 5045 5254 5f37 5f33 2e30 225d  ["SUPERT_7_3.0"]
+0001d000: 0a20 2020 2020 2020 2072 6576 6572 7365  .        reverse
+0001d010: 6444 6174 615b 2245 4d41 3822 5d20 3d20  dData["EMA8"] = 
+0001d020: 706b 7461 6c69 622e 454d 4128 7265 7665  pktalib.EMA(reve
+0001d030: 7273 6564 4461 7461 5b22 436c 6f73 6522  rsedData["Close"
+0001d040: 5d2c 2074 696d 6570 6572 696f 643d 3929  ], timeperiod=9)
+0001d050: 0a20 2020 2020 2020 2068 6967 6865 7243  .        higherC
+0001d060: 6c6f 7365 203d 2028 0a20 2020 2020 2020  lose = (.       
+0001d070: 2020 2020 2068 6967 6865 7243 6c6f 7365       higherClose
+0001d080: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001d090: 2064 6179 305b 2243 6c6f 7365 225d 2e69   day0["Close"].i
+0001d0a0: 6c6f 635b 305d 203e 2072 6576 6572 7365  loc[0] > reverse
+0001d0b0: 6444 6174 612e 7461 696c 2831 295b 2253  dData.tail(1)["S
+0001d0c0: 5550 4552 5422 5d2e 696c 6f63 5b30 5d0a  UPERT"].iloc[0].
+0001d0d0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0001d0e0: 6461 7930 5b22 436c 6f73 6522 5d2e 696c  day0["Close"].il
+0001d0f0: 6f63 5b30 5d20 3e20 7265 7665 7273 6564  oc[0] > reversed
+0001d100: 4461 7461 2e74 6169 6c28 3129 5b22 454d  Data.tail(1)["EM
+0001d110: 4138 225d 2e69 6c6f 635b 305d 0a20 2020  A8"].iloc[0].   
+0001d120: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+0001d130: 6574 7572 6e20 6869 6768 6572 4869 6768  eturn higherHigh
+0001d140: 7320 616e 6420 6869 6768 6572 4c6f 7773  s and higherLows
+0001d150: 2061 6e64 2068 6967 6865 7243 6c6f 7365   and higherClose
+0001d160: 0a0a 2020 2020 2340 6d65 6173 7572 655f  ..    #@measure_
+0001d170: 7469 6d65 0a20 2020 2023 2056 616c 6964  time.    # Valid
+0001d180: 6174 6520 2749 6e73 6964 6520 4261 7227  ate 'Inside Bar'
+0001d190: 2073 7472 7563 7475 7265 2066 6f72 2072   structure for r
+0001d1a0: 6563 656e 7420 6461 7973 0a20 2020 2064  ecent days.    d
+0001d1b0: 6566 2076 616c 6964 6174 6549 6e73 6964  ef validateInsid
+0001d1c0: 6542 6172 280a 2020 2020 2020 2020 7365  eBar(.        se
+0001d1d0: 6c66 2c20 6466 2c20 7363 7265 656e 4469  lf, df, screenDi
+0001d1e0: 6374 2c20 7361 7665 4469 6374 2c20 6368  ct, saveDict, ch
+0001d1f0: 6172 7450 6174 7465 726e 3d31 2c20 6461  artPattern=1, da
+0001d200: 7973 546f 4c6f 6f6b 6261 636b 3d35 0a20  ysToLookback=5. 
+0001d210: 2020 2029 3a0a 2020 2020 2020 2020 6966     ):.        if
+0001d220: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
+0001d230: 656e 2864 6629 203d 3d20 303a 0a20 2020  en(df) == 0:.   
+0001d240: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001d250: 4661 6c73 650a 2020 2020 2020 2020 6461  False.        da
+0001d260: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
+0001d270: 2020 2020 2020 206f 7267 4461 7461 203d         orgData =
+0001d280: 2064 6174 610a 2020 2020 2020 2020 7361   data.        sa
+0001d290: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
+0001d2a0: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
+0001d2b0: 2873 6372 6565 6e44 6963 742c 2073 6176  (screenDict, sav
+0001d2c0: 6544 6963 742c 2022 5061 7474 6572 6e22  eDict, "Pattern"
+0001d2d0: 290a 2020 2020 2020 2020 666f 7220 6920  ).        for i 
+0001d2e0: 696e 2072 616e 6765 2869 6e74 2864 6179  in range(int(day
+0001d2f0: 7354 6f4c 6f6f 6b62 6163 6b29 2c20 696e  sToLookback), in
+0001d300: 7428 726f 756e 6428 6461 7973 546f 4c6f  t(round(daysToLo
+0001d310: 6f6b 6261 636b 202a 2030 2e35 2929 202d  okback * 0.5)) -
+0001d320: 2031 2c20 2d31 293a 0a20 2020 2020 2020   1, -1):.       
+0001d330: 2020 2020 2069 6620 6920 3d3d 2032 3a0a       if i == 2:.
+0001d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d350: 7265 7475 726e 2030 2020 2320 4578 6974  return 0  # Exit
+0001d360: 2069 6620 6f6e 6c79 206c 6173 7420 3220   if only last 2 
+0001d370: 6361 6e64 6c65 7320 6172 6520 6c65 6674  candles are left
+0001d380: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001d390: 6368 6172 7450 6174 7465 726e 203d 3d20  chartPattern == 
+0001d3a0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+0001d3b0: 2020 2069 6620 2255 7022 2069 6e20 7361     if "Up" in sa
+0001d3c0: 7665 4469 6374 5b22 5472 656e 6422 5d20  veDict["Trend"] 
+0001d3d0: 616e 6420 280a 2020 2020 2020 2020 2020  and (.          
+0001d3e0: 2020 2020 2020 2020 2020 2242 756c 6c22            "Bull"
+0001d3f0: 2069 6e20 7361 7665 4469 6374 5b22 4d41   in saveDict["MA
+0001d400: 2d53 6967 6e61 6c22 5d0a 2020 2020 2020  -Signal"].      
+0001d410: 2020 2020 2020 2020 2020 2020 2020 6f72                or
+0001d420: 2022 5375 7070 6f72 7422 2069 6e20 7361   "Support" in sa
+0001d430: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
+0001d440: 6c22 5d0a 2020 2020 2020 2020 2020 2020  l"].            
+0001d450: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+0001d460: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+0001d470: 3d20 6f72 6744 6174 612e 6865 6164 2869  = orgData.head(i
+0001d480: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001d490: 2020 2020 2020 7265 6643 616e 646c 6520        refCandle 
+0001d4a0: 3d20 6461 7461 2e74 6169 6c28 3129 0a20  = data.tail(1). 
+0001d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4c0: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+0001d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4e0: 286c 656e 2864 6174 612e 4869 6768 5b64  (len(data.High[d
+0001d4f0: 6174 612e 4869 6768 203e 2072 6566 4361  ata.High > refCa
+0001d500: 6e64 6c65 2e48 6967 682e 6974 656d 2829  ndle.High.item()
+0001d510: 5d29 203d 3d20 3029 0a20 2020 2020 2020  ]) == 0).       
+0001d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d530: 2061 6e64 2028 6c65 6e28 6461 7461 2e4c   and (len(data.L
+0001d540: 6f77 5b64 6174 612e 4c6f 7720 3c20 7265  ow[data.Low < re
+0001d550: 6643 616e 646c 652e 4c6f 772e 6974 656d  fCandle.Low.item
+0001d560: 2829 5d29 203d 3d20 3029 0a20 2020 2020  ()]) == 0).     
+0001d570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d580: 2020 2061 6e64 2028 6c65 6e28 6461 7461     and (len(data
+0001d590: 2e4f 7065 6e5b 6461 7461 2e4f 7065 6e20  .Open[data.Open 
+0001d5a0: 3e20 7265 6643 616e 646c 652e 4869 6768  > refCandle.High
+0001d5b0: 2e69 7465 6d28 295d 2920 3d3d 2030 290a  .item()]) == 0).
+0001d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5d0: 2020 2020 2020 2020 616e 6420 286c 656e          and (len
+0001d5e0: 2864 6174 612e 436c 6f73 655b 6461 7461  (data.Close[data
+0001d5f0: 2e43 6c6f 7365 203c 2072 6566 4361 6e64  .Close < refCand
+0001d600: 6c65 2e4c 6f77 2e69 7465 6d28 295d 2920  le.Low.item()]) 
+0001d610: 3d3d 2030 290a 2020 2020 2020 2020 2020  == 0).          
+0001d620: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+0001d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d640: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001d650: 2250 6174 7465 726e 225d 203d 2028 0a20  "Pattern"] = (. 
+0001d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d670: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+0001d680: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+0001d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d6a0: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
+0001d6b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d6c0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001d6d0: 6f6c 6f72 5465 7874 2e57 4152 4e0a 2020  olorText.WARN.  
 0001d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d710: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
-0001d720: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
-0001d730: 2022 496e 7369 6465 2042 6172 2028 2564   "Inside Bar (%d
-0001d740: 2922 2025 2069 0a20 2020 2020 2020 2020  )" % i.         
-0001d750: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001d760: 6574 7572 6e20 690a 2020 2020 2020 2020  eturn i.        
-0001d770: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d790: 2020 7265 7475 726e 2030 0a20 2020 2020    return 0.     
-0001d7a0: 2020 2072 6574 7572 6e20 300a 0a20 2020     return 0..   
-0001d7b0: 2023 2046 696e 6420 4950 4f20 6261 7365   # Find IPO base
-0001d7c0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0001d7d0: 6549 706f 4261 7365 2873 656c 662c 2073  eIpoBase(self, s
-0001d7e0: 746f 636b 2c20 6466 2c20 7363 7265 656e  tock, df, screen
-0001d7f0: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
-0001d800: 7065 7263 656e 7461 6765 3d30 2e33 293a  percentage=0.3):
-0001d810: 0a20 2020 2020 2020 2069 6620 6466 2069  .        if df i
-0001d820: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
-0001d830: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
-0001d840: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0001d850: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-0001d860: 6466 2e63 6f70 7928 290a 2020 2020 2020  df.copy().      
-0001d870: 2020 6c69 7374 696e 6750 7269 6365 203d    listingPrice =
-0001d880: 2064 6174 615b 3a3a 2d31 5d2e 6865 6164   data[::-1].head
-0001d890: 2831 295b 224f 7065 6e22 5d2e 696c 6f63  (1)["Open"].iloc
-0001d8a0: 5b30 5d0a 2020 2020 2020 2020 6375 7272  [0].        curr
-0001d8b0: 656e 7450 7269 6365 203d 2064 6174 612e  entPrice = data.
-0001d8c0: 6865 6164 2831 295b 2243 6c6f 7365 225d  head(1)["Close"]
-0001d8d0: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
-0001d8e0: 2041 5448 203d 2064 6174 612e 6465 7363   ATH = data.desc
-0001d8f0: 7269 6265 2829 5b22 4869 6768 225d 5b22  ribe()["High"]["
-0001d900: 6d61 7822 5d0a 2020 2020 2020 2020 6966  max"].        if
-0001d910: 2041 5448 203e 2028 6c69 7374 696e 6750   ATH > (listingP
-0001d920: 7269 6365 202b 2028 6c69 7374 696e 6750  rice + (listingP
-0001d930: 7269 6365 202a 2070 6572 6365 6e74 6167  rice * percentag
-0001d940: 6529 293a 0a20 2020 2020 2020 2020 2020  e)):.           
-0001d950: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-0001d960: 2020 2020 2020 6177 6179 203d 2072 6f75        away = rou
-0001d970: 6e64 2828 2863 7572 7265 6e74 5072 6963  nd(((currentPric
-0001d980: 6520 2d20 6c69 7374 696e 6750 7269 6365  e - listingPrice
-0001d990: 2920 2f20 6c69 7374 696e 6750 7269 6365  ) / listingPrice
-0001d9a0: 2920 2a20 3130 302c 2031 290a 2020 2020  ) * 100, 1).    
-0001d9b0: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-0001d9c0: 2020 2020 2028 6c69 7374 696e 6750 7269       (listingPri
-0001d9d0: 6365 202d 2028 6c69 7374 696e 6750 7269  ce - (listingPri
-0001d9e0: 6365 202a 2070 6572 6365 6e74 6167 6529  ce * percentage)
-0001d9f0: 290a 2020 2020 2020 2020 2020 2020 3c3d  ).            <=
-0001da00: 2063 7572 7265 6e74 5072 6963 650a 2020   currentPrice.  
-0001da10: 2020 2020 2020 2020 2020 3c3d 2028 6c69            <= (li
-0001da20: 7374 696e 6750 7269 6365 202b 2028 6c69  stingPrice + (li
-0001da30: 7374 696e 6750 7269 6365 202a 2070 6572  stingPrice * per
-0001da40: 6365 6e74 6167 6529 290a 2020 2020 2020  centage)).      
-0001da50: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-0001da60: 2073 6176 6564 203d 2073 656c 662e 6669   saved = self.fi
-0001da70: 6e64 4375 7272 656e 7453 6176 6564 5661  ndCurrentSavedVa
-0001da80: 6c75 6528 7363 7265 656e 4469 6374 2c20  lue(screenDict, 
-0001da90: 7361 7665 4469 6374 2c20 2250 6174 7465  saveDict, "Patte
-0001daa0: 726e 2229 0a20 2020 2020 2020 2020 2020  rn").           
-0001dab0: 2069 6620 6177 6179 203e 2030 3a0a 2020   if away > 0:.  
-0001dac0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-0001dad0: 7265 656e 4469 6374 5b22 5061 7474 6572  reenDict["Patter
-0001dae0: 6e22 5d20 3d20 280a 2020 2020 2020 2020  n"] = (.        
-0001daf0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-0001db00: 645b 305d 200a 2020 2020 2020 2020 2020  d[0] .          
-0001db10: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001db20: 7254 6578 742e 424f 4c44 0a20 2020 2020  rText.BOLD.     
-0001db30: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001db40: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
-0001db50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001db60: 2020 2020 202b 2066 2249 504f 2042 6173       + f"IPO Bas
-0001db70: 6520 287b 6177 6179 7d20 2529 220a 2020  e ({away} %)".  
-0001db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db90: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
-0001dba0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-0001dbb0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0001dbc0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001dbd0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-0001dbe0: 5b22 5061 7474 6572 6e22 5d20 3d20 280a  ["Pattern"] = (.
-0001dbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dc00: 2020 2020 7361 7665 645b 305d 0a20 2020      saved[0].   
-0001dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dc20: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-0001dc30: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-0001dc40: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001dc50: 742e 4752 4545 4e0a 2020 2020 2020 2020  t.GREEN.        
-0001dc60: 2020 2020 2020 2020 2020 2020 2b20 2249              + "I
-0001dc70: 504f 2042 6173 6520 220a 2020 2020 2020  PO Base ".      
-0001dc80: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001dc90: 636f 6c6f 7254 6578 742e 4641 494c 0a20  colorText.FAIL. 
-0001dca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dcb0: 2020 202b 2066 2228 7b61 7761 797d 2025     + f"({away} %
-0001dcc0: 2922 0a20 2020 2020 2020 2020 2020 2020  )".             
-0001dcd0: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-0001dce0: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
-0001dcf0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001dd00: 2020 2020 2073 6176 6544 6963 745b 2250       saveDict["P
-0001dd10: 6174 7465 726e 225d 203d 2073 6176 6564  attern"] = saved
-0001dd20: 5b31 5d20 2b20 6622 4950 4f20 4261 7365  [1] + f"IPO Base
-0001dd30: 2028 7b61 7761 797d 2025 2922 0a20 2020   ({away} %)".   
-0001dd40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0001dd50: 5472 7565 0a20 2020 2020 2020 2072 6574  True.        ret
-0001dd60: 7572 6e20 4661 6c73 650a 0a20 2020 2023  urn False..    #
-0001dd70: 406d 6561 7375 7265 5f74 696d 650a 2020  @measure_time.  
-0001dd80: 2020 2320 5661 6c69 6461 7465 204c 6f72    # Validate Lor
-0001dd90: 656e 747a 6961 6e20 436c 6173 7369 6669  entzian Classifi
-0001dda0: 6361 7469 6f6e 2073 6967 6e61 6c0a 2020  cation signal.  
-0001ddb0: 2020 6465 6620 7661 6c69 6461 7465 4c6f    def validateLo
-0001ddc0: 7265 6e74 7a69 616e 2873 656c 662c 2064  rentzian(self, d
-0001ddd0: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
-0001dde0: 6176 6544 6963 742c 206c 6f6f 6b46 6f72  aveDict, lookFor
-0001ddf0: 3d33 293a 0a20 2020 2020 2020 2069 6620  =3):.        if 
-0001de00: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
-0001de10: 6e28 6466 2920 3d3d 2030 3a0a 2020 2020  n(df) == 0:.    
-0001de20: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001de30: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
-0001de40: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
-0001de50: 2020 2020 2020 2320 6c6f 6f6b 466f 723a        # lookFor:
-0001de60: 2031 2d42 7579 2c20 322d 5365 6c6c 2c20   1-Buy, 2-Sell, 
-0001de70: 332d 416e 790a 2020 2020 2020 2020 6461  3-Any.        da
-0001de80: 7461 203d 2064 6174 615b 3a3a 2d31 5d20  ta = data[::-1] 
-0001de90: 2023 2052 6576 6572 7365 2074 6865 2064   # Reverse the d
-0001dea0: 6174 6166 7261 6d65 0a20 2020 2020 2020  ataframe.       
-0001deb0: 2064 6174 6120 3d20 6461 7461 2e72 656e   data = data.ren
-0001dec0: 616d 6528 0a20 2020 2020 2020 2020 2020  ame(.           
-0001ded0: 2063 6f6c 756d 6e73 3d7b 0a20 2020 2020   columns={.     
-0001dee0: 2020 2020 2020 2020 2020 2022 4f70 656e             "Open
-0001def0: 223a 2022 6f70 656e 222c 0a20 2020 2020  ": "open",.     
-0001df00: 2020 2020 2020 2020 2020 2022 436c 6f73             "Clos
-0001df10: 6522 3a20 2263 6c6f 7365 222c 0a20 2020  e": "close",.   
-0001df20: 2020 2020 2020 2020 2020 2020 2022 4869               "Hi
-0001df30: 6768 223a 2022 6869 6768 222c 0a20 2020  gh": "high",.   
-0001df40: 2020 2020 2020 2020 2020 2020 2022 4c6f               "Lo
-0001df50: 7722 3a20 226c 6f77 222c 0a20 2020 2020  w": "low",.     
-0001df60: 2020 2020 2020 2020 2020 2022 566f 6c75             "Volu
-0001df70: 6d65 223a 2022 766f 6c75 6d65 222c 0a20  me": "volume",. 
-0001df80: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-0001df90: 2020 2020 2029 0a20 2020 2020 2020 2074       ).        t
-0001dfa0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0001dfb0: 7769 7468 2053 7570 7072 6573 734f 7574  with SuppressOut
-0001dfc0: 7075 7428 7375 7070 7265 7373 5f73 7464  put(suppress_std
-0001dfd0: 6f75 743d 5472 7565 2c20 7375 7070 7265  out=True, suppre
-0001dfe0: 7373 5f73 7464 6572 723d 5472 7565 293a  ss_stderr=True):
-0001dff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e000: 206c 6320 3d20 6174 612e 4c6f 7265 6e74   lc = ata.Lorent
-0001e010: 7a69 616e 436c 6173 7369 6669 6361 7469  zianClassificati
-0001e020: 6f6e 2864 6174 613d 6461 7461 290a 2020  on(data=data).  
-0001e030: 2020 2020 2020 2020 2020 7361 7665 6420            saved 
-0001e040: 3d20 7365 6c66 2e66 696e 6443 7572 7265  = self.findCurre
-0001e050: 6e74 5361 7665 6456 616c 7565 2873 6372  ntSavedValue(scr
-0001e060: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-0001e070: 742c 2022 5061 7474 6572 6e22 290a 2020  t, "Pattern").  
-0001e080: 2020 2020 2020 2020 2020 6966 206c 632e            if lc.
-0001e090: 6466 2e69 6c6f 635b 2d31 5d5b 2269 734e  df.iloc[-1]["isN
-0001e0a0: 6577 4275 7953 6967 6e61 6c22 5d3a 0a20  ewBuySignal"]:. 
+0001d6f0: 2020 2020 2020 2020 2020 2b20 2822 496e            + ("In
+0001d700: 7369 6465 2042 6172 2028 2564 2922 2025  side Bar (%d)" %
+0001d710: 2069 290a 2020 2020 2020 2020 2020 2020   i).            
+0001d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d730: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+0001d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d750: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0001d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d770: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
+0001d780: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
+0001d790: 202b 2022 496e 7369 6465 2042 6172 2028   + "Inside Bar (
+0001d7a0: 2564 2922 2025 2069 0a20 2020 2020 2020  %d)" % i.       
+0001d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d7c0: 2072 6574 7572 6e20 690a 2020 2020 2020   return i.      
+0001d7d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0001d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d7f0: 2020 2020 7265 7475 726e 2030 0a20 2020      return 0.   
+0001d800: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0001d810: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001d820: 6620 2244 6f77 6e22 2069 6e20 7361 7665  f "Down" in save
+0001d830: 4469 6374 5b22 5472 656e 6422 5d20 616e  Dict["Trend"] an
+0001d840: 6420 280a 2020 2020 2020 2020 2020 2020  d (.            
+0001d850: 2020 2020 2020 2020 2242 6561 7222 2069          "Bear" i
+0001d860: 6e20 7361 7665 4469 6374 5b22 4d41 2d53  n saveDict["MA-S
+0001d870: 6967 6e61 6c22 5d20 6f72 2022 5265 7369  ignal"] or "Resi
+0001d880: 7374 2220 696e 2073 6176 6544 6963 745b  st" in saveDict[
+0001d890: 224d 412d 5369 676e 616c 225d 0a20 2020  "MA-Signal"].   
+0001d8a0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
+0001d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8c0: 2020 2020 6461 7461 203d 206f 7267 4461      data = orgDa
+0001d8d0: 7461 2e68 6561 6428 6929 0a20 2020 2020  ta.head(i).     
+0001d8e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001d8f0: 6566 4361 6e64 6c65 203d 2064 6174 612e  efCandle = data.
+0001d900: 7461 696c 2831 290a 2020 2020 2020 2020  tail(1).        
+0001d910: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+0001d920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d930: 2020 2020 2020 2020 2028 6c65 6e28 6461           (len(da
+0001d940: 7461 2e48 6967 685b 6461 7461 2e48 6967  ta.High[data.Hig
+0001d950: 6820 3e20 7265 6643 616e 646c 652e 4869  h > refCandle.Hi
+0001d960: 6768 2e69 7465 6d28 295d 2920 3d3d 2030  gh.item()]) == 0
+0001d970: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001d980: 2020 2020 2020 2020 2020 616e 6420 286c            and (l
+0001d990: 656e 2864 6174 612e 4c6f 775b 6461 7461  en(data.Low[data
+0001d9a0: 2e4c 6f77 203c 2072 6566 4361 6e64 6c65  .Low < refCandle
+0001d9b0: 2e4c 6f77 2e69 7465 6d28 295d 2920 3d3d  .Low.item()]) ==
+0001d9c0: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
+0001d9d0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0001d9e0: 286c 656e 2864 6174 612e 4f70 656e 5b64  (len(data.Open[d
+0001d9f0: 6174 612e 4f70 656e 203e 2072 6566 4361  ata.Open > refCa
+0001da00: 6e64 6c65 2e48 6967 682e 6974 656d 2829  ndle.High.item()
+0001da10: 5d29 203d 3d20 3029 0a20 2020 2020 2020  ]) == 0).       
+0001da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da30: 2061 6e64 2028 6c65 6e28 6461 7461 2e43   and (len(data.C
+0001da40: 6c6f 7365 5b64 6174 612e 436c 6f73 6520  lose[data.Close 
+0001da50: 3c20 7265 6643 616e 646c 652e 4c6f 772e  < refCandle.Low.
+0001da60: 6974 656d 2829 5d29 203d 3d20 3029 0a20  item()]) == 0). 
+0001da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da80: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+0001da90: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+0001daa0: 7265 656e 4469 6374 5b22 5061 7474 6572  reenDict["Patter
+0001dab0: 6e22 5d20 3d20 280a 2020 2020 2020 2020  n"] = (.        
+0001dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dad0: 2020 2020 7361 7665 645b 305d 0a20 2020      saved[0].   
+0001dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001daf0: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+0001db00: 5465 7874 2e42 4f4c 440a 2020 2020 2020  Text.BOLD.      
+0001db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db20: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+0001db30: 742e 5741 524e 0a20 2020 2020 2020 2020  t.WARN.         
+0001db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db50: 2020 202b 2028 2249 6e73 6964 6520 4261     + ("Inside Ba
+0001db60: 7220 2825 6429 2220 2520 6929 0a20 2020  r (%d)" % i).   
+0001db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db80: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+0001db90: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+0001dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dbb0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0001dbc0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+0001dbd0: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+0001dbe0: 2073 6176 6564 5b31 5d20 2b20 2249 6e73   saved[1] + "Ins
+0001dbf0: 6964 6520 4261 7220 2825 6429 2220 2520  ide Bar (%d)" % 
+0001dc00: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
+0001dc10: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001dc20: 2069 0a20 2020 2020 2020 2020 2020 2020   i.             
+0001dc30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001dc40: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0001dc50: 7572 6e20 300a 2020 2020 2020 2020 7265  urn 0.        re
+0001dc60: 7475 726e 2030 0a0a 2020 2020 2320 4669  turn 0..    # Fi
+0001dc70: 6e64 2049 504f 2062 6173 650a 2020 2020  nd IPO base.    
+0001dc80: 6465 6620 7661 6c69 6461 7465 4970 6f42  def validateIpoB
+0001dc90: 6173 6528 7365 6c66 2c20 7374 6f63 6b2c  ase(self, stock,
+0001dca0: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
+0001dcb0: 2073 6176 6544 6963 742c 2070 6572 6365   saveDict, perce
+0001dcc0: 6e74 6167 653d 302e 3329 3a0a 2020 2020  ntage=0.3):.    
+0001dcd0: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
+0001dce0: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
+0001dcf0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+0001dd00: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+0001dd10: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
+0001dd20: 7079 2829 0a20 2020 2020 2020 206c 6973  py().        lis
+0001dd30: 7469 6e67 5072 6963 6520 3d20 6461 7461  tingPrice = data
+0001dd40: 5b3a 3a2d 315d 2e68 6561 6428 3129 5b22  [::-1].head(1)["
+0001dd50: 4f70 656e 225d 2e69 6c6f 635b 305d 0a20  Open"].iloc[0]. 
+0001dd60: 2020 2020 2020 2063 7572 7265 6e74 5072         currentPr
+0001dd70: 6963 6520 3d20 6461 7461 2e68 6561 6428  ice = data.head(
+0001dd80: 3129 5b22 436c 6f73 6522 5d2e 696c 6f63  1)["Close"].iloc
+0001dd90: 5b30 5d0a 2020 2020 2020 2020 4154 4820  [0].        ATH 
+0001dda0: 3d20 6461 7461 2e64 6573 6372 6962 6528  = data.describe(
+0001ddb0: 295b 2248 6967 6822 5d5b 226d 6178 225d  )["High"]["max"]
+0001ddc0: 0a20 2020 2020 2020 2069 6620 4154 4820  .        if ATH 
+0001ddd0: 3e20 286c 6973 7469 6e67 5072 6963 6520  > (listingPrice 
+0001dde0: 2b20 286c 6973 7469 6e67 5072 6963 6520  + (listingPrice 
+0001ddf0: 2a20 7065 7263 656e 7461 6765 2929 3a0a  * percentage)):.
+0001de00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001de10: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0001de20: 2061 7761 7920 3d20 726f 756e 6428 2828   away = round(((
+0001de30: 6375 7272 656e 7450 7269 6365 202d 206c  currentPrice - l
+0001de40: 6973 7469 6e67 5072 6963 6529 202f 206c  istingPrice) / l
+0001de50: 6973 7469 6e67 5072 6963 6529 202a 2031  istingPrice) * 1
+0001de60: 3030 2c20 3129 0a20 2020 2020 2020 2069  00, 1).        i
+0001de70: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+0001de80: 286c 6973 7469 6e67 5072 6963 6520 2d20  (listingPrice - 
+0001de90: 286c 6973 7469 6e67 5072 6963 6520 2a20  (listingPrice * 
+0001dea0: 7065 7263 656e 7461 6765 2929 0a20 2020  percentage)).   
+0001deb0: 2020 2020 2020 2020 203c 3d20 6375 7272           <= curr
+0001dec0: 656e 7450 7269 6365 0a20 2020 2020 2020  entPrice.       
+0001ded0: 2020 2020 203c 3d20 286c 6973 7469 6e67       <= (listing
+0001dee0: 5072 6963 6520 2b20 286c 6973 7469 6e67  Price + (listing
+0001def0: 5072 6963 6520 2a20 7065 7263 656e 7461  Price * percenta
+0001df00: 6765 2929 0a20 2020 2020 2020 2029 3a0a  ge)).        ):.
+0001df10: 2020 2020 2020 2020 2020 2020 7361 7665              save
+0001df20: 6420 3d20 7365 6c66 2e66 696e 6443 7572  d = self.findCur
+0001df30: 7265 6e74 5361 7665 6456 616c 7565 2873  rentSavedValue(s
+0001df40: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+0001df50: 6963 742c 2022 5061 7474 6572 6e22 290a  ict, "Pattern").
+0001df60: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+0001df70: 7761 7920 3e20 303a 0a20 2020 2020 2020  way > 0:.       
+0001df80: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+0001df90: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+0001dfa0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0001dfb0: 2020 2020 2020 2073 6176 6564 5b30 5d20         saved[0] 
+0001dfc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001dfd0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
+0001dfe0: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
+0001dff0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+0001e000: 7254 6578 742e 4752 4545 4e0a 2020 2020  rText.GREEN.    
+0001e010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e020: 2b20 6622 4950 4f20 4261 7365 2028 7b61  + f"IPO Base ({a
+0001e030: 7761 797d 2025 2922 0a20 2020 2020 2020  way} %)".       
+0001e040: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001e050: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
+0001e060: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0001e070: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001e080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e090: 2073 6372 6565 6e44 6963 745b 2250 6174   screenDict["Pat
+0001e0a0: 7465 726e 225d 203d 2028 0a20 2020 2020  tern"] = (.     
 0001e0b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001e0c0: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
-0001e0d0: 726e 225d 203d 2028 0a20 2020 2020 2020  rn"] = (.       
-0001e0e0: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-0001e0f0: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
-0001e100: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
-0001e110: 7874 2e47 5245 454e 202b 2022 4c6f 7265  xt.GREEN + "Lore
-0001e120: 6e74 7a69 616e 2d42 7579 2220 2b20 636f  ntzian-Buy" + co
-0001e130: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
-0001e140: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001e150: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-0001e160: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
-0001e170: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
-0001e180: 4c6f 7265 6e74 7a69 616e 2d42 7579 220a  Lorentzian-Buy".
-0001e190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1a0: 6966 206c 6f6f 6b46 6f72 2021 3d20 323a  if lookFor != 2:
-0001e1b0: 2023 204e 6f74 2053 656c 6c0a 2020 2020   # Not Sell.    
-0001e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1d0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0001e1e0: 2020 2020 2020 2020 656c 6966 206c 632e          elif lc.
-0001e1f0: 6466 2e69 6c6f 635b 2d31 5d5b 2269 734e  df.iloc[-1]["isN
-0001e200: 6577 5365 6c6c 5369 676e 616c 225d 3a0a  ewSellSignal"]:.
-0001e210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e220: 7363 7265 656e 4469 6374 5b22 5061 7474  screenDict["Patt
-0001e230: 6572 6e22 5d20 3d20 280a 2020 2020 2020  ern"] = (.      
-0001e240: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-0001e250: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
-0001e260: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
-0001e270: 6578 742e 4641 494c 202b 2022 4c6f 7265  ext.FAIL + "Lore
-0001e280: 6e74 7a69 616e 2d53 656c 6c22 202b 2063  ntzian-Sell" + c
-0001e290: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
-0001e2a0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0001e2b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001e2c0: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
-0001e2d0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-0001e2e0: 224c 6f72 656e 747a 6961 6e2d 5365 6c6c  "Lorentzian-Sell
-0001e2f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0001e300: 2020 6966 206c 6f6f 6b46 6f72 2021 3d20    if lookFor != 
-0001e310: 313a 2023 204e 6f74 2042 7579 0a20 2020  1: # Not Buy.   
-0001e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e330: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-0001e340: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-0001e350: 7074 696f 6e3a 2020 2320 7072 6167 6d61  ption:  # pragma
-0001e360: 3a20 6e6f 2063 6f76 6572 0a20 2020 2020  : no cover.     
-0001e370: 2020 2020 2020 2023 2056 616c 7565 4572         # ValueEr
-0001e380: 726f 723a 206f 7065 7261 6e64 7320 636f  ror: operands co
-0001e390: 756c 6420 6e6f 7420 6265 2062 726f 6164  uld not be broad
-0001e3a0: 6361 7374 2074 6f67 6574 6865 7220 7769  cast together wi
-0001e3b0: 7468 2073 6861 7065 7320 2832 302c 2920  th shapes (20,) 
-0001e3c0: 2832 362c 290a 2020 2020 2020 2020 2020  (26,).          
-0001e3d0: 2020 2320 4669 6c65 2022 2f6f 7074 2f68    # File "/opt/h
-0001e3e0: 6f6d 6562 7265 772f 6c69 622f 7079 7468  omebrew/lib/pyth
-0001e3f0: 6f6e 332e 3131 2f73 6974 652d 7061 636b  on3.11/site-pack
-0001e400: 6167 6573 2f61 6476 616e 6365 645f 7461  ages/advanced_ta
-0001e410: 2f4c 6f72 656e 747a 6961 6e43 6c61 7373  /LorentzianClass
-0001e420: 6966 6963 6174 696f 6e2f 436c 6173 7369  ification/Classi
-0001e430: 6669 6572 2e70 7922 2c20 6c69 6e65 2031  fier.py", line 1
-0001e440: 3836 2c20 696e 205f 5f69 6e69 745f 5f0a  86, in __init__.
-0001e450: 2020 2020 2020 2020 2020 2020 2320 4669              # Fi
-0001e460: 6c65 2022 2f6f 7074 2f68 6f6d 6562 7265  le "/opt/homebre
-0001e470: 772f 6c69 622f 7079 7468 6f6e 332e 3131  w/lib/python3.11
-0001e480: 2f73 6974 652d 7061 636b 6167 6573 2f61  /site-packages/a
-0001e490: 6476 616e 6365 645f 7461 2f4c 6f72 656e  dvanced_ta/Loren
-0001e4a0: 747a 6961 6e43 6c61 7373 6966 6963 6174  tzianClassificat
-0001e4b0: 696f 6e2f 436c 6173 7369 6669 6572 2e70  ion/Classifier.p
-0001e4c0: 7922 2c20 6c69 6e65 2033 3935 2c20 696e  y", line 395, in
-0001e4d0: 205f 5f63 6c61 7373 6966 790a 2020 2020   __classify.    
-0001e4e0: 2020 2020 2020 2020 2320 4669 6c65 2022          # File "
-0001e4f0: 2f6f 7074 2f68 6f6d 6562 7265 772f 6c69  /opt/homebrew/li
-0001e500: 622f 7079 7468 6f6e 332e 3131 2f73 6974  b/python3.11/sit
-0001e510: 652d 7061 636b 6167 6573 2f70 616e 6461  e-packages/panda
-0001e520: 732f 636f 7265 2f6f 7073 2f63 6f6d 6d6f  s/core/ops/commo
-0001e530: 6e2e 7079 222c 206c 696e 6520 3736 2c20  n.py", line 76, 
-0001e540: 696e 206e 6577 5f6d 6574 686f 640a 2020  in new_method.  
-0001e550: 2020 2020 2020 2020 2020 2320 4669 6c65            # File
-0001e560: 2022 2f6f 7074 2f68 6f6d 6562 7265 772f   "/opt/homebrew/
-0001e570: 6c69 622f 7079 7468 6f6e 332e 3131 2f73  lib/python3.11/s
-0001e580: 6974 652d 7061 636b 6167 6573 2f70 616e  ite-packages/pan
-0001e590: 6461 732f 636f 7265 2f61 7272 6179 6c69  das/core/arrayli
-0001e5a0: 6b65 2e70 7922 2c20 6c69 6e65 2037 302c  ke.py", line 70,
-0001e5b0: 2069 6e20 5f5f 616e 645f 5f0a 2020 2020   in __and__.    
-0001e5c0: 2020 2020 2020 2020 2320 4669 6c65 2022          # File "
-0001e5d0: 2f6f 7074 2f68 6f6d 6562 7265 772f 6c69  /opt/homebrew/li
-0001e5e0: 622f 7079 7468 6f6e 332e 3131 2f73 6974  b/python3.11/sit
-0001e5f0: 652d 7061 636b 6167 6573 2f70 616e 6461  e-packages/panda
-0001e600: 732f 636f 7265 2f73 6572 6965 732e 7079  s/core/series.py
-0001e610: 222c 206c 696e 6520 3538 3130 2c20 696e  ", line 5810, in
-0001e620: 205f 6c6f 6769 6361 6c5f 6d65 7468 6f64   _logical_method
-0001e630: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
-0001e640: 696c 6520 222f 6f70 742f 686f 6d65 6272  ile "/opt/homebr
-0001e650: 6577 2f6c 6962 2f70 7974 686f 6e33 2e31  ew/lib/python3.1
-0001e660: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
-0001e670: 7061 6e64 6173 2f63 6f72 652f 6f70 732f  pandas/core/ops/
-0001e680: 6172 7261 795f 6f70 732e 7079 222c 206c  array_ops.py", l
-0001e690: 696e 6520 3435 362c 2069 6e20 6c6f 6769  ine 456, in logi
-0001e6a0: 6361 6c5f 6f70 0a20 2020 2020 2020 2020  cal_op.         
-0001e6b0: 2020 2023 2046 696c 6520 222f 6f70 742f     # File "/opt/
-0001e6c0: 686f 6d65 6272 6577 2f6c 6962 2f70 7974  homebrew/lib/pyt
-0001e6d0: 686f 6e33 2e31 312f 7369 7465 2d70 6163  hon3.11/site-pac
-0001e6e0: 6b61 6765 732f 7061 6e64 6173 2f63 6f72  kages/pandas/cor
-0001e6f0: 652f 6f70 732f 6172 7261 795f 6f70 732e  e/ops/array_ops.
-0001e700: 7079 222c 206c 696e 6520 3336 342c 2069  py", line 364, i
-0001e710: 6e20 6e61 5f6c 6f67 6963 616c 5f6f 700a  n na_logical_op.
-0001e720: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-0001e730: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
-0001e740: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
-0001e750: 6e66 6f3d 5472 7565 290a 2020 2020 2020  nfo=True).      
-0001e760: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-0001e770: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-0001e780: 0a20 2020 2023 2076 616c 6964 6174 6520  .    # validate 
-0001e790: 6966 2074 6865 2073 746f 636b 2068 6173  if the stock has
-0001e7a0: 2062 6565 6e20 6861 7669 6e67 206c 6f77   been having low
-0001e7b0: 6572 206c 6f77 732c 206c 6f77 6572 2068  er lows, lower h
-0001e7c0: 6967 6873 0a20 2020 2064 6566 2076 616c  ighs.    def val
-0001e7d0: 6964 6174 654c 6f77 6572 4869 6768 734c  idateLowerHighsL
-0001e7e0: 6f77 6572 4c6f 7773 2873 656c 662c 2064  owerLows(self, d
-0001e7f0: 6629 3a0a 2020 2020 2020 2020 6966 2064  f):.        if d
-0001e800: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-0001e810: 2864 6629 203d 3d20 303a 0a20 2020 2020  (df) == 0:.     
-0001e820: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-0001e830: 6c73 650a 2020 2020 2020 2020 6461 7461  lse.        data
-0001e840: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
-0001e850: 2020 2020 2064 6179 3020 3d20 6461 7461       day0 = data
-0001e860: 0a20 2020 2020 2020 2064 6179 3120 3d20  .        day1 = 
-0001e870: 6461 7461 5b31 3a5d 0a20 2020 2020 2020  data[1:].       
-0001e880: 2064 6179 3220 3d20 6461 7461 5b32 3a5d   day2 = data[2:]
-0001e890: 0a20 2020 2020 2020 2064 6179 3320 3d20  .        day3 = 
-0001e8a0: 6461 7461 5b33 3a5d 0a20 2020 2020 2020  data[3:].       
-0001e8b0: 206c 6f77 6572 4869 6768 7320 3d20 280a   lowerHighs = (.
-0001e8c0: 2020 2020 2020 2020 2020 2020 2864 6179              (day
-0001e8d0: 305b 2248 6967 6822 5d2e 696c 6f63 5b30  0["High"].iloc[0
-0001e8e0: 5d20 3c20 6461 7931 5b22 4869 6768 225d  ] < day1["High"]
-0001e8f0: 2e69 6c6f 635b 305d 290a 2020 2020 2020  .iloc[0]).      
-0001e900: 2020 2020 2020 616e 6420 2864 6179 315b        and (day1[
-0001e910: 2248 6967 6822 5d2e 696c 6f63 5b30 5d20  "High"].iloc[0] 
-0001e920: 3c20 6461 7932 5b22 4869 6768 225d 2e69  < day2["High"].i
-0001e930: 6c6f 635b 305d 290a 2020 2020 2020 2020  loc[0]).        
-0001e940: 2020 2020 616e 6420 2864 6179 325b 2248      and (day2["H
-0001e950: 6967 6822 5d2e 696c 6f63 5b30 5d20 3c20  igh"].iloc[0] < 
-0001e960: 6461 7933 5b22 4869 6768 225d 2e69 6c6f  day3["High"].ilo
-0001e970: 635b 305d 290a 2020 2020 2020 2020 290a  c[0]).        ).
-0001e980: 2020 2020 2020 2020 6c6f 7765 724c 6f77          lowerLow
-0001e990: 7320 3d20 280a 2020 2020 2020 2020 2020  s = (.          
-0001e9a0: 2020 2864 6179 305b 224c 6f77 225d 2e69    (day0["Low"].i
-0001e9b0: 6c6f 635b 305d 203c 2064 6179 315b 224c  loc[0] < day1["L
-0001e9c0: 6f77 225d 2e69 6c6f 635b 305d 290a 2020  ow"].iloc[0]).  
-0001e9d0: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
-0001e9e0: 6179 315b 224c 6f77 225d 2e69 6c6f 635b  ay1["Low"].iloc[
-0001e9f0: 305d 203c 2064 6179 325b 224c 6f77 225d  0] < day2["Low"]
-0001ea00: 2e69 6c6f 635b 305d 290a 2020 2020 2020  .iloc[0]).      
-0001ea10: 2020 2020 2020 616e 6420 2864 6179 325b        and (day2[
-0001ea20: 224c 6f77 225d 2e69 6c6f 635b 305d 203c  "Low"].iloc[0] <
-0001ea30: 2064 6179 335b 224c 6f77 225d 2e69 6c6f   day3["Low"].ilo
-0001ea40: 635b 305d 290a 2020 2020 2020 2020 290a  c[0]).        ).
-0001ea50: 2020 2020 2020 2020 6869 6768 6572 5253          higherRS
-0001ea60: 4920 3d20 280a 2020 2020 2020 2020 2020  I = (.          
-0001ea70: 2020 2864 6179 305b 2252 5349 225d 2e69    (day0["RSI"].i
-0001ea80: 6c6f 635b 305d 203c 2064 6179 315b 2252  loc[0] < day1["R
-0001ea90: 5349 225d 2e69 6c6f 635b 305d 290a 2020  SI"].iloc[0]).  
-0001eaa0: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
-0001eab0: 6179 315b 2252 5349 225d 2e69 6c6f 635b  ay1["RSI"].iloc[
-0001eac0: 305d 203c 2064 6179 325b 2252 5349 225d  0] < day2["RSI"]
-0001ead0: 2e69 6c6f 635b 305d 290a 2020 2020 2020  .iloc[0]).      
-0001eae0: 2020 2020 2020 616e 6420 2864 6179 325b        and (day2[
-0001eaf0: 2252 5349 225d 2e69 6c6f 635b 305d 203c  "RSI"].iloc[0] <
-0001eb00: 2064 6179 335b 2252 5349 225d 2e69 6c6f   day3["RSI"].ilo
-0001eb10: 635b 305d 290a 2020 2020 2020 2020 2020  c[0]).          
-0001eb20: 2020 616e 6420 6461 7930 5b22 5253 4922    and day0["RSI"
-0001eb30: 5d2e 696c 6f63 5b30 5d20 3e3d 2035 300a  ].iloc[0] >= 50.
-0001eb40: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0001eb50: 2020 7265 7475 726e 206c 6f77 6572 4869    return lowerHi
-0001eb60: 6768 7320 616e 6420 6c6f 7765 724c 6f77  ghs and lowerLow
-0001eb70: 7320 616e 6420 6869 6768 6572 5253 490a  s and higherRSI.
-0001eb80: 0a20 2020 2023 2056 616c 6964 6174 6520  .    # Validate 
-0001eb90: 6966 2072 6563 656e 7420 766f 6c75 6d65  if recent volume
-0001eba0: 2069 7320 6c6f 7765 7374 206f 6620 6c61   is lowest of la
-0001ebb0: 7374 2027 4e27 2044 6179 730a 2020 2020  st 'N' Days.    
-0001ebc0: 6465 6620 7661 6c69 6461 7465 4c6f 7765  def validateLowe
-0001ebd0: 7374 566f 6c75 6d65 2873 656c 662c 2064  stVolume(self, d
-0001ebe0: 662c 2064 6179 7346 6f72 4c6f 7765 7374  f, daysForLowest
-0001ebf0: 566f 6c75 6d65 293a 0a20 2020 2020 2020  Volume):.       
-0001ec00: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-0001ec10: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
-0001ec20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001ec30: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-0001ec40: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-0001ec50: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
-0001ec60: 2064 6174 612e 6669 6c6c 6e61 2830 290a   data.fillna(0).
-0001ec70: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001ec80: 6174 612e 7265 706c 6163 6528 5b6e 702e  ata.replace([np.
-0001ec90: 696e 662c 202d 6e70 2e69 6e66 5d2c 2030  inf, -np.inf], 0
-0001eca0: 290a 2020 2020 2020 2020 6966 2064 6179  ).        if day
-0001ecb0: 7346 6f72 4c6f 7765 7374 566f 6c75 6d65  sForLowestVolume
-0001ecc0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0001ecd0: 2020 2020 2020 6461 7973 466f 724c 6f77        daysForLow
-0001ece0: 6573 7456 6f6c 756d 6520 3d20 3330 0a20  estVolume = 30. 
-0001ecf0: 2020 2020 2020 2069 6620 6c65 6e28 6461         if len(da
-0001ed00: 7461 2920 3c20 6461 7973 466f 724c 6f77  ta) < daysForLow
-0001ed10: 6573 7456 6f6c 756d 653a 0a20 2020 2020  estVolume:.     
-0001ed20: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-0001ed30: 6c73 650a 2020 2020 2020 2020 6461 7461  lse.        data
-0001ed40: 203d 2064 6174 612e 6865 6164 2864 6179   = data.head(day
-0001ed50: 7346 6f72 4c6f 7765 7374 566f 6c75 6d65  sForLowestVolume
-0001ed60: 290a 2020 2020 2020 2020 7265 6365 6e74  ).        recent
-0001ed70: 203d 2064 6174 612e 6865 6164 2831 290a   = data.head(1).
-0001ed80: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
-0001ed90: 6563 656e 7429 203c 2031 3a0a 2020 2020  ecent) < 1:.    
-0001eda0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001edb0: 616c 7365 0a20 2020 2020 2020 2069 6620  alse.        if 
-0001edc0: 2872 6563 656e 745b 2256 6f6c 756d 6522  (recent["Volume"
-0001edd0: 5d2e 696c 6f63 5b30 5d20 3c3d 2064 6174  ].iloc[0] <= dat
-0001ede0: 612e 6465 7363 7269 6265 2829 5b22 566f  a.describe()["Vo
-0001edf0: 6c75 6d65 225d 5b22 6d69 6e22 5d29 2061  lume"]["min"]) a
-0001ee00: 6e64 2072 6563 656e 745b 0a20 2020 2020  nd recent[.     
-0001ee10: 2020 2020 2020 2022 566f 6c75 6d65 220a         "Volume".
-0001ee20: 2020 2020 2020 2020 5d5b 305d 2021 3d20          ][0] != 
-0001ee30: 6e70 2e6e 616e 3a0a 2020 2020 2020 2020  np.nan:.        
-0001ee40: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-0001ee50: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001ee60: 616c 7365 0a0a 2020 2020 2320 5661 6c69  alse..    # Vali
-0001ee70: 6461 7465 204c 5450 2077 6974 6869 6e20  date LTP within 
-0001ee80: 6c69 6d69 7473 0a20 2020 2064 6566 2076  limits.    def v
-0001ee90: 616c 6964 6174 654c 5450 2873 656c 662c  alidateLTP(self,
-0001eea0: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
-0001eeb0: 2073 6176 6544 6963 742c 206d 696e 4c54   saveDict, minLT
-0001eec0: 503d 4e6f 6e65 2c20 6d61 784c 5450 3d4e  P=None, maxLTP=N
-0001eed0: 6f6e 652c 6d69 6e43 6861 6e67 653d 3029  one,minChange=0)
-0001eee0: 3a0a 2020 2020 2020 2020 6461 7461 203d  :.        data =
-0001eef0: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
-0001ef00: 2020 206c 7470 5661 6c69 6420 3d20 4661     ltpValid = Fa
-0001ef10: 6c73 650a 2020 2020 2020 2020 6966 206d  lse.        if m
-0001ef20: 696e 4c54 5020 6973 204e 6f6e 653a 0a20  inLTP is None:. 
-0001ef30: 2020 2020 2020 2020 2020 206d 696e 4c54             minLT
-0001ef40: 5020 3d20 7365 6c66 2e63 6f6e 6669 674d  P = self.configM
-0001ef50: 616e 6167 6572 2e6d 696e 4c54 500a 2020  anager.minLTP.  
-0001ef60: 2020 2020 2020 6966 206d 6178 4c54 5020        if maxLTP 
-0001ef70: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0001ef80: 2020 2020 206d 6178 4c54 5020 3d20 7365       maxLTP = se
-0001ef90: 6c66 2e63 6f6e 6669 674d 616e 6167 6572  lf.configManager
-0001efa0: 2e6d 6178 4c54 500a 2020 2020 2020 2020  .maxLTP.        
-0001efb0: 6461 7461 203d 2064 6174 612e 6669 6c6c  data = data.fill
-0001efc0: 6e61 2830 290a 2020 2020 2020 2020 6461  na(0).        da
-0001efd0: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
-0001efe0: 6528 5b6e 702e 696e 662c 202d 6e70 2e69  e([np.inf, -np.i
-0001eff0: 6e66 5d2c 2030 290a 2020 2020 2020 2020  nf], 0).        
-0001f000: 7265 6365 6e74 203d 2064 6174 612e 6865  recent = data.he
-0001f010: 6164 2831 290a 0a20 2020 2020 2020 2070  ad(1)..        p
-0001f020: 6374 5f63 6861 6e67 6520 3d20 2864 6174  ct_change = (dat
-0001f030: 615b 3a3a 2d31 5d5b 2243 6c6f 7365 225d  a[::-1]["Close"]
-0001f040: 2e70 6374 5f63 6861 6e67 6528 2920 2a20  .pct_change() * 
-0001f050: 3130 3029 2e69 6c6f 635b 2d31 5d0a 2020  100).iloc[-1].  
-0001f060: 2020 2020 2020 6966 2070 6374 5f63 6861        if pct_cha
-0001f070: 6e67 6520 3d3d 206e 702e 696e 6620 6f72  nge == np.inf or
-0001f080: 2070 6374 5f63 6861 6e67 6520 3d3d 202d   pct_change == -
-0001f090: 6e70 2e69 6e66 3a0a 2020 2020 2020 2020  np.inf:.        
-0001f0a0: 2020 2020 7063 745f 6368 616e 6765 203d      pct_change =
-0001f0b0: 2030 0a20 2020 2020 2020 2070 6374 5f73   0.        pct_s
-0001f0c0: 6176 6520 3d20 2225 2e31 6625 2522 2025  ave = "%.1f%%" %
-0001f0d0: 2070 6374 5f63 6861 6e67 650a 2020 2020   pct_change.    
-0001f0e0: 2020 2020 6966 2070 6374 5f63 6861 6e67      if pct_chang
-0001f0f0: 6520 3e20 302e 323a 0a20 2020 2020 2020  e > 0.2:.       
-0001f100: 2020 2020 2070 6374 5f63 6861 6e67 6520       pct_change 
-0001f110: 3d20 636f 6c6f 7254 6578 742e 4752 4545  = colorText.GREE
-0001f120: 4e20 2b20 2822 252e 3166 2525 2220 2520  N + ("%.1f%%" % 
-0001f130: 7063 745f 6368 616e 6765 2920 2b20 636f  pct_change) + co
-0001f140: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
-0001f150: 2020 2020 656c 6966 2070 6374 5f63 6861      elif pct_cha
-0001f160: 6e67 6520 3c20 2d30 2e32 3a0a 2020 2020  nge < -0.2:.    
-0001f170: 2020 2020 2020 2020 7063 745f 6368 616e          pct_chan
-0001f180: 6765 203d 2063 6f6c 6f72 5465 7874 2e46  ge = colorText.F
-0001f190: 4149 4c20 2b20 2822 252e 3166 2525 2220  AIL + ("%.1f%%" 
-0001f1a0: 2520 7063 745f 6368 616e 6765 2920 2b20  % pct_change) + 
-0001f1b0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-0001f1c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001f1d0: 2020 2020 2020 2020 7063 745f 6368 616e          pct_chan
-0001f1e0: 6765 203d 2063 6f6c 6f72 5465 7874 2e57  ge = colorText.W
-0001f1f0: 4152 4e20 2b20 2822 252e 3166 2525 2220  ARN + ("%.1f%%" 
-0001f200: 2520 7063 745f 6368 616e 6765 2920 2b20  % pct_change) + 
-0001f210: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-0001f220: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-0001f230: 2543 686e 6722 5d20 3d20 7063 745f 7361  %Chng"] = pct_sa
-0001f240: 7665 0a20 2020 2020 2020 2073 6372 6565  ve.        scree
-0001f250: 6e44 6963 745b 2225 4368 6e67 225d 203d  nDict["%Chng"] =
-0001f260: 2070 6374 5f63 6861 6e67 650a 2020 2020   pct_change.    
-0001f270: 2020 2020 6c74 7020 3d20 726f 756e 6428      ltp = round(
-0001f280: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
-0001f290: 696c 6f63 5b30 5d2c 2032 290a 2020 2020  iloc[0], 2).    
-0001f2a0: 2020 2020 7665 7269 6679 5374 6167 6554      verifyStageT
-0001f2b0: 776f 203d 2054 7275 650a 2020 2020 2020  wo = True.      
-0001f2c0: 2020 6966 206c 656e 2864 6174 6129 203e    if len(data) >
-0001f2d0: 2032 3530 3a0a 2020 2020 2020 2020 2020   250:.          
-0001f2e0: 2020 7965 6172 6c79 4c6f 7720 3d20 6461    yearlyLow = da
-0001f2f0: 7461 2e68 6561 6428 3235 3029 5b22 436c  ta.head(250)["Cl
-0001f300: 6f73 6522 5d2e 6d69 6e28 290a 2020 2020  ose"].min().    
-0001f310: 2020 2020 2020 2020 7965 6172 6c79 4869          yearlyHi
-0001f320: 6768 203d 2064 6174 612e 6865 6164 2832  gh = data.head(2
-0001f330: 3530 295b 2243 6c6f 7365 225d 2e6d 6178  50)["Close"].max
-0001f340: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
-0001f350: 6620 6c74 7020 3c20 2832 202a 2079 6561  f ltp < (2 * yea
-0001f360: 726c 794c 6f77 2920 616e 6420 6c74 7020  rlyLow) and ltp 
-0001f370: 3c20 2830 2e37 3520 2a20 7965 6172 6c79  < (0.75 * yearly
-0001f380: 4869 6768 293a 0a20 2020 2020 2020 2020  High):.         
-0001f390: 2020 2020 2020 2076 6572 6966 7953 7461         verifySta
-0001f3a0: 6765 5477 6f20 3d20 4661 6c73 650a 2020  geTwo = False.  
-0001f3b0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-0001f3c0: 7265 656e 4469 6374 5b22 5374 6f63 6b22  reenDict["Stock"
-0001f3d0: 5d20 3d20 636f 6c6f 7254 6578 742e 4641  ] = colorText.FA
-0001f3e0: 494c 202b 2073 6176 6544 6963 745b 2253  IL + saveDict["S
-0001f3f0: 746f 636b 225d 202b 2063 6f6c 6f72 5465  tock"] + colorTe
-0001f400: 7874 2e45 4e44 0a20 2020 2020 2020 2069  xt.END.        i
-0001f410: 6620 6c74 7020 3e3d 206d 696e 4c54 5020  f ltp >= minLTP 
-0001f420: 616e 6420 6c74 7020 3c3d 206d 6178 4c54  and ltp <= maxLT
-0001f430: 503a 0a20 2020 2020 2020 2020 2020 206c  P:.            l
-0001f440: 7470 5661 6c69 6420 3d20 5472 7565 0a20  tpValid = True. 
-0001f450: 2020 2020 2020 2020 2020 2069 6620 6d69             if mi
-0001f460: 6e43 6861 6e67 6520 213d 2030 3a0a 2020  nChange != 0:.  
-0001f470: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001f480: 5573 6572 2068 6173 2073 7570 706c 6965  User has supplie
-0001f490: 6420 736f 6d65 2066 696c 7465 7220 666f  d some filter fo
-0001f4a0: 7220 7065 7263 656e 7461 6765 2063 6861  r percentage cha
-0001f4b0: 6e67 650a 2020 2020 2020 2020 2020 2020  nge.            
-0001f4c0: 2020 2020 6c74 7056 616c 6964 203d 2066      ltpValid = f
-0001f4d0: 6c6f 6174 2873 7472 2870 6374 5f73 6176  loat(str(pct_sav
-0001f4e0: 6529 2e72 6570 6c61 6365 2822 2522 2c22  e).replace("%","
-0001f4f0: 2229 2920 3e3d 206d 696e 4368 616e 6765  ")) >= minChange
-0001f500: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-0001f510: 6544 6963 745b 224c 5450 225d 203d 2072  eDict["LTP"] = r
-0001f520: 6f75 6e64 286c 7470 2c20 3229 0a20 2020  ound(ltp, 2).   
-0001f530: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-0001f540: 6963 745b 224c 5450 225d 203d 2028 636f  ict["LTP"] = (co
-0001f550: 6c6f 7254 6578 742e 4752 4545 4e20 6966  lorText.GREEN if
-0001f560: 206c 7470 5661 6c69 6420 656c 7365 2063   ltpValid else c
-0001f570: 6f6c 6f72 5465 7874 2e46 4149 4c29 202b  olorText.FAIL) +
-0001f580: 2028 2225 2e32 6622 2025 206c 7470 2920   ("%.2f" % ltp) 
-0001f590: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-0001f5a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001f5b0: 726e 206c 7470 5661 6c69 642c 2076 6572  rn ltpValid, ver
-0001f5c0: 6966 7953 7461 6765 5477 6f0a 2020 2020  ifyStageTwo.    
-0001f5d0: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-0001f5e0: 4c54 5022 5d20 3d20 636f 6c6f 7254 6578  LTP"] = colorTex
-0001f5f0: 742e 4641 494c 202b 2028 2225 2e32 6622  t.FAIL + ("%.2f"
-0001f600: 2025 206c 7470 2920 2b20 636f 6c6f 7254   % ltp) + colorT
-0001f610: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
-0001f620: 7361 7665 4469 6374 5b22 4c54 5022 5d20  saveDict["LTP"] 
-0001f630: 3d20 726f 756e 6428 6c74 702c 2032 290a  = round(ltp, 2).
-0001f640: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-0001f650: 7470 5661 6c69 642c 2076 6572 6966 7953  tpValid, verifyS
-0001f660: 7461 6765 5477 6f0a 0a20 2020 2064 6566  tageTwo..    def
-0001f670: 2076 616c 6964 6174 654c 5450 466f 7250   validateLTPForP
-0001f680: 6f72 7466 6f6c 696f 4361 6c63 2873 656c  ortfolioCalc(sel
-0001f690: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
-0001f6a0: 742c 2073 6176 6544 6963 742c 7265 7175  t, saveDict,requ
-0001f6b0: 6573 7465 6450 6572 696f 643d 3029 3a0a  estedPeriod=0):.
-0001f6c0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001f6d0: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-0001f6e0: 2070 6572 696f 6473 203d 2073 656c 662e   periods = self.
-0001f6f0: 636f 6e66 6967 4d61 6e61 6765 722e 7065  configManager.pe
-0001f700: 7269 6f64 7352 616e 6765 0a20 2020 2020  riodsRange.     
-0001f710: 2020 2069 6620 7265 7175 6573 7465 6450     if requestedP
-0001f720: 6572 696f 6420 3e20 3020 616e 6420 7265  eriod > 0 and re
-0001f730: 7175 6573 7465 6450 6572 696f 6420 6e6f  questedPeriod no
-0001f740: 7420 696e 2070 6572 696f 6473 3a0a 2020  t in periods:.  
-0001f750: 2020 2020 2020 2020 2020 7065 7269 6f64            period
-0001f760: 732e 6170 7065 6e64 2872 6571 7565 7374  s.append(request
-0001f770: 6564 5065 7269 6f64 290a 2020 2020 2020  edPeriod).      
-0001f780: 2020 7072 6576 696f 7573 5f72 6563 656e    previous_recen
-0001f790: 7420 3d20 6461 7461 2e68 6561 6428 3129  t = data.head(1)
-0001f7a0: 0a20 2020 2020 2020 2070 7265 7669 6f75  .        previou
-0001f7b0: 735f 7265 6365 6e74 2e72 6573 6574 5f69  s_recent.reset_i
-0001f7c0: 6e64 6578 2869 6e70 6c61 6365 3d54 7275  ndex(inplace=Tru
-0001f7d0: 6529 0a20 2020 2020 2020 2063 616c 635f  e).        calc_
-0001f7e0: 6461 7465 203d 2073 7472 2870 7265 7669  date = str(previ
-0001f7f0: 6f75 735f 7265 6365 6e74 2e69 6c6f 635b  ous_recent.iloc[
-0001f800: 3a2c 2030 5d5b 305d 292e 7370 6c69 7428  :, 0][0]).split(
-0001f810: 2220 2229 5b30 5d0a 2020 2020 2020 2020  " ")[0].        
-0001f820: 666f 7220 7072 6420 696e 2070 6572 696f  for prd in perio
-0001f830: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
-0001f840: 6966 206c 656e 2864 6174 6129 203e 3d20  if len(data) >= 
-0001f850: 7072 6420 2b20 313a 0a20 2020 2020 2020  prd + 1:.       
-0001f860: 2020 2020 2020 2020 2070 7265 764c 7470           prevLtp
-0001f870: 203d 2064 6174 615b 2243 6c6f 7365 225d   = data["Close"]
-0001f880: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
-0001f890: 2020 2020 2020 2020 206c 7470 5464 7920           ltpTdy 
-0001f8a0: 3d20 6461 7461 5b22 436c 6f73 6522 5d2e  = data["Close"].
-0001f8b0: 696c 6f63 5b70 7264 5d0a 2020 2020 2020  iloc[prd].      
-0001f8c0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-0001f8d0: 6e73 7461 6e63 6528 7072 6576 4c74 702c  nstance(prevLtp,
-0001f8e0: 7064 2e53 6572 6965 7329 3a0a 2020 2020  pd.Series):.    
-0001f8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f900: 7072 6576 4c74 7020 3d20 7072 6576 4c74  prevLtp = prevLt
-0001f910: 705b 305d 0a20 2020 2020 2020 2020 2020  p[0].           
-0001f920: 2020 2020 2020 2020 206c 7470 5464 7920           ltpTdy 
-0001f930: 3d20 6c74 7054 6479 5b30 5d0a 2020 2020  = ltpTdy[0].    
-0001f940: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-0001f950: 656e 4469 6374 5b66 224c 5450 7b70 7264  enDict[f"LTP{prd
-0001f960: 7d22 5d20 3d20 280a 2020 2020 2020 2020  }"] = (.        
-0001f970: 2020 2020 2020 2020 2020 2020 2863 6f6c              (col
-0001f980: 6f72 5465 7874 2e47 5245 454e 2069 6620  orText.GREEN if 
-0001f990: 286c 7470 5464 7920 3e3d 2070 7265 764c  (ltpTdy >= prevL
-0001f9a0: 7470 2920 656c 7365 2028 636f 6c6f 7254  tp) else (colorT
-0001f9b0: 6578 742e 4641 494c 2929 0a20 2020 2020  ext.FAIL)).     
-0001f9c0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001f9d0: 2073 7472 2822 7b3a 2e32 667d 222e 666f   str("{:.2f}".fo
-0001f9e0: 726d 6174 286c 7470 5464 7929 290a 2020  rmat(ltpTdy)).  
-0001f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fa00: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
-0001fa10: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-0001fa20: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0001fa30: 2020 2020 7363 7265 656e 4469 6374 5b66      screenDict[f
-0001fa40: 2247 726f 7774 687b 7072 647d 225d 203d  "Growth{prd}"] =
-0001fa50: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0001fa60: 2020 2020 2020 2028 636f 6c6f 7254 6578         (colorTex
-0001fa70: 742e 4752 4545 4e20 6966 2028 6c74 7054  t.GREEN if (ltpT
-0001fa80: 6479 203e 3d20 7072 6576 4c74 7029 2065  dy >= prevLtp) e
-0001fa90: 6c73 6520 2863 6f6c 6f72 5465 7874 2e46  lse (colorText.F
-0001faa0: 4149 4c29 290a 2020 2020 2020 2020 2020  AIL)).          
-0001fab0: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
-0001fac0: 227b 3a2e 3266 7d22 2e66 6f72 6d61 7428  "{:.2f}".format(
-0001fad0: 6c74 7054 6479 202d 2070 7265 764c 7470  ltpTdy - prevLtp
-0001fae0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0001faf0: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-0001fb00: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
-0001fb10: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001fb20: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-0001fb30: 745b 6622 4c54 507b 7072 647d 225d 203d  t[f"LTP{prd}"] =
-0001fb40: 2072 6f75 6e64 286c 7470 5464 792c 2032   round(ltpTdy, 2
-0001fb50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001fb60: 2020 7361 7665 4469 6374 5b66 2247 726f    saveDict[f"Gro
-0001fb70: 7774 687b 7072 647d 225d 203d 2072 6f75  wth{prd}"] = rou
-0001fb80: 6e64 286c 7470 5464 7920 2d20 7072 6576  nd(ltpTdy - prev
-0001fb90: 4c74 702c 2032 290a 2020 2020 2020 2020  Ltp, 2).        
-0001fba0: 2020 2020 2020 2020 6966 2070 7264 203d          if prd =
-0001fbb0: 3d20 3232 206f 7220 2870 7264 203d 3d20  = 22 or (prd == 
-0001fbc0: 7265 7175 6573 7465 6450 6572 696f 6429  requestedPeriod)
-0001fbd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001fbe0: 2020 2020 2020 6368 616e 6765 5065 7263        changePerc
-0001fbf0: 656e 7420 3d20 726f 756e 6428 2828 7072  ent = round(((pr
-0001fc00: 6576 4c74 702d 6c74 7054 6479 2920 6966  evLtp-ltpTdy) if
-0001fc10: 2072 6571 7565 7374 6564 5065 7269 6f64   requestedPeriod
-0001fc20: 203d 3d30 2065 6c73 6520 286c 7470 5464   ==0 else (ltpTd
-0001fc30: 7920 2d20 7072 6576 4c74 7029 292a 3130  y - prevLtp))*10
-0001fc40: 302f 6c74 7054 6479 2c20 3229 0a20 2020  0/ltpTdy, 2).   
-0001fc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fc60: 2073 6176 6544 6963 745b 6622 7b70 7264   saveDict[f"{prd
-0001fc70: 7d2d 5064 2025 225d 203d 2066 227b 6368  }-Pd %"] = f"{ch
-0001fc80: 616e 6765 5065 7263 656e 747d 2522 2069  angePercent}%" i
-0001fc90: 6620 6e6f 7420 7064 2e69 736e 6128 6368  f not pd.isna(ch
-0001fca0: 616e 6765 5065 7263 656e 7429 2065 6c73  angePercent) els
-0001fcb0: 6520 272d 270a 2020 2020 2020 2020 2020  e '-'.          
-0001fcc0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-0001fcd0: 4469 6374 5b66 227b 7072 647d 2d50 6420  Dict[f"{prd}-Pd 
-0001fce0: 2522 5d20 3d20 2828 636f 6c6f 7254 6578  %"] = ((colorTex
-0001fcf0: 742e 4752 4545 4e20 6966 2063 6861 6e67  t.GREEN if chang
-0001fd00: 6550 6572 6365 6e74 203e 3d30 2065 6c73  ePercent >=0 els
-0001fd10: 6520 636f 6c6f 7254 6578 742e 4641 494c  e colorText.FAIL
-0001fd20: 2920 2b20 6622 7b63 6861 6e67 6550 6572  ) + f"{changePer
-0001fd30: 6365 6e74 7d25 2220 2b20 636f 6c6f 7254  cent}%" + colorT
-0001fd40: 6578 742e 454e 4429 2069 6620 6e6f 7420  ext.END) if not 
-0001fd50: 7064 2e69 736e 6128 6368 616e 6765 5065  pd.isna(changePe
-0001fd60: 7263 656e 7429 2065 6c73 6520 272d 270a  rcent) else '-'.
-0001fd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fd80: 7363 7265 656e 4469 6374 5b22 4461 7465  screenDict["Date
-0001fd90: 225d 203d 2063 616c 635f 6461 7465 0a20  "] = calc_date. 
-0001fda0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001fdb0: 6176 6544 6963 745b 2244 6174 6522 5d20  aveDict["Date"] 
-0001fdc0: 3d20 6361 6c63 5f64 6174 650a 2020 2020  = calc_date.    
-0001fdd0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001fde0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-0001fdf0: 7665 4469 6374 5b66 224c 5450 7b70 7264  veDict[f"LTP{prd
-0001fe00: 7d22 5d20 3d20 6e70 2e6e 616e 0a20 2020  }"] = np.nan.   
-0001fe10: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-0001fe20: 6544 6963 745b 6622 4772 6f77 7468 7b70  eDict[f"Growth{p
-0001fe30: 7264 7d22 5d20 3d20 6e70 2e6e 616e 0a20  rd}"] = np.nan. 
-0001fe40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001fe50: 6372 6565 6e44 6963 745b 2244 6174 6522  creenDict["Date"
-0001fe60: 5d20 3d20 6361 6c63 5f64 6174 650a 2020  ] = calc_date.  
-0001fe70: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-0001fe80: 7665 4469 6374 5b22 4461 7465 225d 203d  veDict["Date"] =
-0001fe90: 2063 616c 635f 6461 7465 0a0a 2020 2020   calc_date..    
-0001fea0: 2320 4669 6e64 2073 746f 636b 7320 7468  # Find stocks th
-0001feb0: 6174 2061 7265 2062 6561 7269 7368 2069  at are bearish i
-0001fec0: 6e74 7261 6461 793a 204d 6163 6420 4869  ntraday: Macd Hi
-0001fed0: 7374 6f67 7261 6d20 6e65 6761 7469 7665  stogram negative
-0001fee0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0001fef0: 654d 4143 4448 6973 746f 6772 616d 4265  eMACDHistogramBe
-0001ff00: 6c6f 7730 2873 656c 662c 2064 6629 3a0a  low0(self, df):.
-0001ff10: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
-0001ff20: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
-0001ff30: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0001ff40: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-0001ff50: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001ff60: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-0001ff70: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
-0001ff80: 6c6e 6128 3029 0a20 2020 2020 2020 2064  lna(0).        d
-0001ff90: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
-0001ffa0: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
-0001ffb0: 696e 665d 2c20 3029 0a20 2020 2020 2020  inf], 0).       
-0001ffc0: 2064 6174 6120 3d20 6461 7461 5b3a 3a2d   data = data[::-
-0001ffd0: 315d 2020 2320 5265 7665 7273 6520 7468  1]  # Reverse th
-0001ffe0: 6520 6461 7461 6672 616d 6520 736f 2074  e dataframe so t
-0001fff0: 6861 7420 6974 7320 7468 6520 6f6c 6465  hat its the olde
-00020000: 7374 2064 6174 6520 6669 7273 740a 2020  st date first.  
-00020010: 2020 2020 2020 6d61 6364 203d 2070 6b74        macd = pkt
-00020020: 616c 6962 2e4d 4143 4428 6461 7461 5b22  alib.MACD(data["
-00020030: 436c 6f73 6522 5d2c 2031 322c 2032 362c  Close"], 12, 26,
-00020040: 2039 295b 325d 2e74 6169 6c28 3129 0a20   9)[2].tail(1). 
-00020050: 2020 2020 2020 2072 6574 7572 6e20 6d61         return ma
-00020060: 6364 2e69 6c6f 635b 3a31 5d5b 305d 203c  cd.iloc[:1][0] <
-00020070: 2030 0a0a 2020 2020 2340 6d65 6173 7572   0..    #@measur
-00020080: 655f 7469 6d65 0a20 2020 2023 2046 696e  e_time.    # Fin
-00020090: 6420 6966 2073 746f 636b 2067 6169 6e69  d if stock gaini
-000200a0: 6e67 2062 756c 6c69 7368 206d 6f6d 656e  ng bullish momen
-000200b0: 7475 6d0a 2020 2020 6465 6620 7661 6c69  tum.    def vali
-000200c0: 6461 7465 4d6f 6d65 6e74 756d 2873 656c  dateMomentum(sel
-000200d0: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
-000200e0: 742c 2073 6176 6544 6963 7429 3a0a 2020  t, saveDict):.  
-000200f0: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
-00020100: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
-00020110: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00020120: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-00020130: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
-00020140: 636f 7079 2829 0a20 2020 2020 2020 2074  copy().        t
-00020150: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00020160: 6461 7461 203d 2064 6174 612e 6865 6164  data = data.head
-00020170: 2833 290a 2020 2020 2020 2020 2020 2020  (3).            
-00020180: 6966 206c 656e 2864 6174 6129 203c 2033  if len(data) < 3
-00020190: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000201a0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-000201b0: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
-000201c0: 6f77 2069 6e20 6461 7461 2e69 7465 7272  ow in data.iterr
-000201d0: 6f77 7328 293a 0a20 2020 2020 2020 2020  ows():.         
-000201e0: 2020 2020 2020 2023 2041 6c6c 2033 2063         # All 3 c
-000201f0: 616e 646c 6573 2073 686f 756c 6420 6265  andles should be
-00020200: 2047 7265 656e 2061 6e64 204e 4f54 2043   Green and NOT C
-00020210: 6972 6375 6974 730a 2020 2020 2020 2020  ircuits.        
-00020220: 2020 2020 2020 2020 7963 203d 2072 6f77          yc = row
-00020230: 5b31 5d5b 2243 6c6f 7365 225d 0a20 2020  [1]["Close"].   
-00020240: 2020 2020 2020 2020 2020 2020 2079 6f20               yo 
-00020250: 3d20 726f 775b 315d 5b22 4f70 656e 225d  = row[1]["Open"]
-00020260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020270: 2069 6620 7963 203c 3d20 796f 3a0a 2020   if yc <= yo:.  
-00020280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020290: 2020 2320 7365 6c66 2e64 6566 6175 6c74    # self.default
-000202a0: 5f6c 6f67 6765 722e 696e 666f 280a 2020  _logger.info(.  
-000202b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000202c0: 2020 2320 2020 2020 6627 5374 6f63 6b3a    #     f'Stock:
-000202d0: 7b73 6176 6544 6963 745b 2253 746f 636b  {saveDict["Stock
-000202e0: 225d 7d2c 2069 7320 6e6f 7420 6120 6d6f  "]}, is not a mo
-000202f0: 6d65 6e74 756d 2d67 6169 6e65 7220 6265  mentum-gainer be
-00020300: 6361 7573 6520 7965 7374 6572 6461 792d  cause yesterday-
-00020310: 636c 6f73 6520 287b 7963 7d29 203c 3d20  close ({yc}) <= 
-00020320: 7965 7374 6572 6461 792d 6f70 656e 2028  yesterday-open (
-00020330: 7b79 6f7d 2927 0a20 2020 2020 2020 2020  {yo})'.         
-00020340: 2020 2020 2020 2020 2020 2023 2029 0a20             # ). 
-00020350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020360: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00020370: 2020 2020 2020 2020 2020 2020 6f70 656e              open
-00020380: 4465 7363 203d 2064 6174 612e 736f 7274  Desc = data.sort
-00020390: 5f76 616c 7565 7328 6279 3d5b 224f 7065  _values(by=["Ope
-000203a0: 6e22 5d2c 2061 7363 656e 6469 6e67 3d46  n"], ascending=F
-000203b0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-000203c0: 2020 636c 6f73 6544 6573 6320 3d20 6461    closeDesc = da
-000203d0: 7461 2e73 6f72 745f 7661 6c75 6573 2862  ta.sort_values(b
-000203e0: 793d 5b22 436c 6f73 6522 5d2c 2061 7363  y=["Close"], asc
-000203f0: 656e 6469 6e67 3d46 616c 7365 290a 2020  ending=False).  
-00020400: 2020 2020 2020 2020 2020 766f 6c44 6573            volDes
-00020410: 6320 3d20 6461 7461 2e73 6f72 745f 7661  c = data.sort_va
-00020420: 6c75 6573 2862 793d 5b22 566f 6c75 6d65  lues(by=["Volume
-00020430: 225d 2c20 6173 6365 6e64 696e 673d 4661  "], ascending=Fa
-00020440: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-00020450: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00020460: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-00020470: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00020480: 6174 612e 6571 7561 6c73 286f 7065 6e44  ata.equals(openD
-00020490: 6573 6329 0a20 2020 2020 2020 2020 2020  esc).           
-000204a0: 2020 2020 2020 2020 2061 6e64 2064 6174           and dat
-000204b0: 612e 6571 7561 6c73 2863 6c6f 7365 4465  a.equals(closeDe
-000204c0: 7363 290a 2020 2020 2020 2020 2020 2020  sc).            
-000204d0: 2020 2020 2020 2020 616e 6420 6461 7461          and data
-000204e0: 2e65 7175 616c 7328 766f 6c44 6573 6329  .equals(volDesc)
-000204f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020500: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-00020510: 2020 2020 2020 2020 2320 7365 6c66 2e64          # self.d
-00020520: 6566 6175 6c74 5f6c 6f67 6765 722e 696e  efault_logger.in
-00020530: 666f 280a 2020 2020 2020 2020 2020 2020  fo(.            
-00020540: 2020 2020 2020 2020 2320 2020 2020 6627          #     f'
-00020550: 5374 6f63 6b3a 7b73 6176 6544 6963 745b  Stock:{saveDict[
-00020560: 2253 746f 636b 225d 7d2c 206f 7065 6e2c  "Stock"]}, open,
-00020570: 636c 6f73 6520 616e 6420 766f 6c75 6d65  close and volume
-00020580: 2065 7175 616c 2066 726f 6d20 6461 7920   equal from day 
-00020590: 6265 666f 7265 2079 6573 7465 7264 6179  before yesterday
-000205a0: 2e20 4120 706f 7465 6e74 6961 6c20 6d6f  . A potential mo
-000205b0: 6d65 6e74 756d 2d67 6169 6e65 7221 270a  mentum-gainer!'.
-000205c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000205d0: 2020 2020 2320 290a 2020 2020 2020 2020      # ).        
-000205e0: 2020 2020 2020 2020 2020 2020 746f 203d              to =
-000205f0: 2064 6174 615b 224f 7065 6e22 5d2e 696c   data["Open"].il
-00020600: 6f63 5b30 5d0a 2020 2020 2020 2020 2020  oc[0].          
-00020610: 2020 2020 2020 2020 2020 7963 203d 2064            yc = d
-00020620: 6174 615b 2243 6c6f 7365 225d 2e69 6c6f  ata["Close"].ilo
-00020630: 635b 315d 0a20 2020 2020 2020 2020 2020  c[1].           
-00020640: 2020 2020 2020 2020 2079 6f20 3d20 6461           yo = da
-00020650: 7461 5b22 4f70 656e 225d 2e69 6c6f 635b  ta["Open"].iloc[
-00020660: 315d 0a20 2020 2020 2020 2020 2020 2020  1].             
-00020670: 2020 2020 2020 2064 7963 203d 2064 6174         dyc = dat
-00020680: 615b 2243 6c6f 7365 225d 2e69 6c6f 635b  a["Close"].iloc[
-00020690: 325d 0a20 2020 2020 2020 2020 2020 2020  2].             
-000206a0: 2020 2020 2020 2069 6620 2874 6f20 3e3d         if (to >=
-000206b0: 2079 6329 2061 6e64 2028 796f 203e 3d20   yc) and (yo >= 
-000206c0: 6479 6329 3a0a 2020 2020 2020 2020 2020  dyc):.          
-000206d0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000206e0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
-000206f0: 6765 722e 696e 666f 280a 2020 2020 2020  ger.info(.      
-00020700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020710: 2020 2320 2020 2020 6627 5374 6f63 6b3a    #     f'Stock:
-00020720: 7b73 6176 6544 6963 745b 2253 746f 636b  {saveDict["Stock
-00020730: 225d 7d2c 2069 7320 6120 6d6f 6d65 6e74  "]}, is a moment
-00020740: 756d 2d67 6169 6e65 7220 6265 6361 7573  um-gainer becaus
-00020750: 6520 746f 6461 792d 6f70 656e 2028 7b74  e today-open ({t
-00020760: 6f7d 2920 3e3d 2079 6573 7465 7264 6179  o}) >= yesterday
-00020770: 2d63 6c6f 7365 2028 7b79 637d 2920 616e  -close ({yc}) an
-00020780: 6420 7965 7374 6572 6461 792d 6f70 656e  d yesterday-open
-00020790: 287b 796f 7d29 203e 3d20 6461 792d 6265  ({yo}) >= day-be
-000207a0: 666f 7265 2d63 6c6f 7365 287b 6479 637d  fore-close({dyc}
-000207b0: 2927 0a20 2020 2020 2020 2020 2020 2020  )'.             
-000207c0: 2020 2020 2020 2020 2020 2023 2029 0a20             # ). 
-000207d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000207e0: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
-000207f0: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
-00020800: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
-00020810: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
-00020820: 2250 6174 7465 726e 2229 0a20 2020 2020  "Pattern").     
-00020830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020840: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
-00020850: 6174 7465 726e 225d 203d 2028 0a20 2020  attern"] = (.   
-00020860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020870: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-00020880: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00020890: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000208a0: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
-000208b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000208c0: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
-000208d0: 6f72 5465 7874 2e47 5245 454e 0a20 2020  orText.GREEN.   
-000208e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000208f0: 2020 2020 2020 2020 202b 2022 4d6f 6d65           + "Mome
-00020900: 6e74 756d 2047 6169 6e65 7222 0a20 2020  ntum Gainer".   
-00020910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020920: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-00020930: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-00020940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020950: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00020960: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-00020970: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
-00020980: 2073 6176 6564 5b31 5d20 2b20 224d 6f6d   saved[1] + "Mom
-00020990: 656e 7475 6d20 4761 696e 6572 220a 2020  entum Gainer".  
-000209a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000209b0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-000209c0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-000209d0: 2020 2020 2020 2320 7365 6c66 2e64 6566        # self.def
-000209e0: 6175 6c74 5f6c 6f67 6765 722e 696e 666f  ault_logger.info
-000209f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00020a00: 2020 2020 2020 2320 2020 2020 6627 5374        #     f'St
-00020a10: 6f63 6b3a 7b73 6176 6544 6963 745b 2253  ock:{saveDict["S
-00020a20: 746f 636b 225d 7d2c 2069 7320 6e6f 7420  tock"]}, is not 
-00020a30: 6120 6d6f 6d65 6e74 756d 2d67 6169 6e65  a momentum-gaine
-00020a40: 7220 6265 6361 7573 6520 6569 7468 6572  r because either
-00020a50: 2074 6f64 6179 2d6f 7065 6e20 287b 746f   today-open ({to
-00020a60: 7d29 203c 2079 6573 7465 7264 6179 2d63  }) < yesterday-c
-00020a70: 6c6f 7365 2028 7b79 637d 2920 6f72 2079  lose ({yc}) or y
-00020a80: 6573 7465 7264 6179 2d6f 7065 6e28 7b79  esterday-open({y
-00020a90: 6f7d 2920 3c20 6461 792d 6265 666f 7265  o}) < day-before
-00020aa0: 2d63 6c6f 7365 287b 6479 637d 2927 0a20  -close({dyc})'. 
-00020ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ac0: 2020 2023 2029 0a20 2020 2020 2020 2020     # ).         
-00020ad0: 2020 2065 7863 6570 7420 496e 6465 7845     except IndexE
-00020ae0: 7272 6f72 2061 7320 653a 2023 2070 7261  rror as e: # pra
-00020af0: 676d 613a 206e 6f20 636f 7665 720a 2020  gma: no cover.  
-00020b00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00020b10: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
-00020b20: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
-00020b30: 6e66 6f3d 5472 7565 290a 2020 2020 2020  nfo=True).      
-00020b40: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00020b50: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
-00020b60: 6275 6728 6461 7461 290a 2020 2020 2020  bug(data).      
-00020b70: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
-00020b80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00020b90: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-00020ba0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00020bb0: 2061 7320 653a 2020 2320 7072 6167 6d61   as e:  # pragma
-00020bc0: 3a20 6e6f 2063 6f76 6572 0a20 2020 2020  : no cover.     
-00020bd0: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
-00020be0: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
-00020bf0: 2865 2c20 6578 635f 696e 666f 3d54 7275  (e, exc_info=Tru
-00020c00: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
-00020c10: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
-00020c20: 2023 406d 6561 7375 7265 5f74 696d 650a   #@measure_time.
-00020c30: 2020 2020 2320 5661 6c69 6461 7465 204d      # Validate M
-00020c40: 6f76 696e 6720 6176 6572 6167 6573 2061  oving averages a
-00020c50: 6e64 206c 6f6f 6b20 666f 7220 6275 792f  nd look for buy/
-00020c60: 7365 6c6c 2073 6967 6e61 6c73 0a20 2020  sell signals.   
-00020c70: 2064 6566 2076 616c 6964 6174 654d 6f76   def validateMov
-00020c80: 696e 6741 7665 7261 6765 7328 7365 6c66  ingAverages(self
-00020c90: 2c20 6466 2c20 7363 7265 656e 4469 6374  , df, screenDict
-00020ca0: 2c20 7361 7665 4469 6374 2c20 6d61 5261  , saveDict, maRa
-00020cb0: 6e67 653d 322e 3529 3a0a 2020 2020 2020  nge=2.5):.      
-00020cc0: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
-00020cd0: 2829 0a20 2020 2020 2020 2064 6174 6120  ().        data 
-00020ce0: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
-00020cf0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00020d00: 6461 7461 2e72 6570 6c61 6365 285b 6e70  data.replace([np
-00020d10: 2e69 6e66 2c20 2d6e 702e 696e 665d 2c20  .inf, -np.inf], 
-00020d20: 3029 0a20 2020 2020 2020 2072 6563 656e  0).        recen
-00020d30: 7420 3d20 6461 7461 2e68 6561 6428 3129  t = data.head(1)
-00020d40: 0a20 2020 2020 2020 2073 6176 6564 203d  .        saved =
-00020d50: 2073 656c 662e 6669 6e64 4375 7272 656e   self.findCurren
-00020d60: 7453 6176 6564 5661 6c75 6528 7363 7265  tSavedValue(scre
-00020d70: 656e 4469 6374 2c73 6176 6544 6963 742c  enDict,saveDict,
-00020d80: 224d 412d 5369 676e 616c 2229 0a20 2020  "MA-Signal").   
-00020d90: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-00020da0: 2020 2020 2020 7265 6365 6e74 5b22 534d        recent["SM
-00020db0: 4122 5d2e 696c 6f63 5b30 5d20 3e20 7265  A"].iloc[0] > re
-00020dc0: 6365 6e74 5b22 4c4d 4122 5d2e 696c 6f63  cent["LMA"].iloc
-00020dd0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00020de0: 616e 6420 7265 6365 6e74 5b22 436c 6f73  and recent["Clos
-00020df0: 6522 5d2e 696c 6f63 5b30 5d20 3e20 7265  e"].iloc[0] > re
-00020e00: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
-00020e10: 5b30 5d0a 2020 2020 2020 2020 293a 0a20  [0].        ):. 
-00020e20: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00020e30: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
-00020e40: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
-00020e50: 2020 2020 2020 2073 6176 6564 5b30 5d20         saved[0] 
-00020e60: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
-00020e70: 202b 2063 6f6c 6f72 5465 7874 2e47 5245   + colorText.GRE
-00020e80: 454e 202b 2022 4275 6c6c 6973 6822 202b  EN + "Bullish" +
-00020e90: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
-00020ea0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00020eb0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00020ec0: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-00020ed0: 2073 6176 6564 5b31 5d20 2b20 2242 756c   saved[1] + "Bul
-00020ee0: 6c69 7368 220a 2020 2020 2020 2020 656c  lish".        el
-00020ef0: 6966 2072 6563 656e 745b 2253 4d41 225d  if recent["SMA"]
-00020f00: 2e69 6c6f 635b 305d 203c 2072 6563 656e  .iloc[0] < recen
-00020f10: 745b 224c 4d41 225d 2e69 6c6f 635b 305d  t["LMA"].iloc[0]
-00020f20: 3a0a 2020 2020 2020 2020 2020 2020 7363  :.            sc
-00020f30: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
-00020f40: 6e61 6c22 5d20 3d20 280a 2020 2020 2020  nal"] = (.      
-00020f50: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
-00020f60: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
-00020f70: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
-00020f80: 4641 494c 202b 2022 4265 6172 6973 6822  FAIL + "Bearish"
-00020f90: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-00020fa0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00020fb0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-00020fc0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-00020fd0: 203d 2073 6176 6564 5b31 5d20 2b20 2242   = saved[1] + "B
-00020fe0: 6561 7269 7368 220a 2020 2020 2020 2020  earish".        
-00020ff0: 656c 6966 2072 6563 656e 745b 2253 4d41  elif recent["SMA
-00021000: 225d 2e69 6c6f 635b 305d 203d 3d20 303a  "].iloc[0] == 0:
-00021010: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-00021020: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
-00021030: 616c 225d 203d 2028 0a20 2020 2020 2020  al"] = (.       
-00021040: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-00021050: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
-00021060: 4c44 202b 2063 6f6c 6f72 5465 7874 2e57  LD + colorText.W
-00021070: 4152 4e20 2b20 2255 6e6b 6e6f 776e 2220  ARN + "Unknown" 
-00021080: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-00021090: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000210a0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-000210b0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-000210c0: 3d20 7361 7665 645b 315d 202b 2022 556e  = saved[1] + "Un
-000210d0: 6b6e 6f77 6e22 0a20 2020 2020 2020 2065  known".        e
-000210e0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000210f0: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
-00021100: 5369 676e 616c 225d 203d 2028 0a20 2020  Signal"] = (.   
-00021110: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00021120: 6564 5b30 5d20 2b20 636f 6c6f 7254 6578  ed[0] + colorTex
-00021130: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
-00021140: 7874 2e57 4152 4e20 2b20 224e 6575 7472  xt.WARN + "Neutr
-00021150: 616c 2220 2b20 636f 6c6f 7254 6578 742e  al" + colorText.
-00021160: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
-00021170: 290a 2020 2020 2020 2020 2020 2020 7361  ).            sa
-00021180: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
-00021190: 6c22 5d20 3d20 7361 7665 645b 315d 202b  l"] = saved[1] +
-000211a0: 2022 4e65 7574 7261 6c22 0a0a 2020 2020   "Neutral"..    
-000211b0: 2020 2020 736d 6144 6576 203d 2064 6174      smaDev = dat
-000211c0: 615b 2253 4d41 225d 2e69 6c6f 635b 305d  a["SMA"].iloc[0]
-000211d0: 202a 206d 6152 616e 6765 202f 2031 3030   * maRange / 100
-000211e0: 0a20 2020 2020 2020 206c 6d61 4465 7620  .        lmaDev 
-000211f0: 3d20 6461 7461 5b22 4c4d 4122 5d2e 696c  = data["LMA"].il
-00021200: 6f63 5b30 5d20 2a20 6d61 5261 6e67 6520  oc[0] * maRange 
-00021210: 2f20 3130 300a 2020 2020 2020 2020 6f70  / 100.        op
-00021220: 656e 2c20 6869 6768 2c20 6c6f 772c 2063  en, high, low, c
-00021230: 6c6f 7365 2c20 736d 612c 206c 6d61 203d  lose, sma, lma =
-00021240: 2028 0a20 2020 2020 2020 2020 2020 2064   (.            d
-00021250: 6174 615b 224f 7065 6e22 5d2e 696c 6f63  ata["Open"].iloc
-00021260: 5b30 5d2c 0a20 2020 2020 2020 2020 2020  [0],.           
-00021270: 2064 6174 615b 2248 6967 6822 5d2e 696c   data["High"].il
-00021280: 6f63 5b30 5d2c 0a20 2020 2020 2020 2020  oc[0],.         
-00021290: 2020 2064 6174 615b 224c 6f77 225d 2e69     data["Low"].i
-000212a0: 6c6f 635b 305d 2c0a 2020 2020 2020 2020  loc[0],.        
-000212b0: 2020 2020 6461 7461 5b22 436c 6f73 6522      data["Close"
-000212c0: 5d2e 696c 6f63 5b30 5d2c 0a20 2020 2020  ].iloc[0],.     
-000212d0: 2020 2020 2020 2064 6174 615b 2253 4d41         data["SMA
-000212e0: 225d 2e69 6c6f 635b 305d 2c0a 2020 2020  "].iloc[0],.    
-000212f0: 2020 2020 2020 2020 6461 7461 5b22 4c4d          data["LM
-00021300: 4122 5d2e 696c 6f63 5b30 5d2c 0a20 2020  A"].iloc[0],.   
-00021310: 2020 2020 2029 0a20 2020 2020 2020 206d       ).        m
-00021320: 6152 6576 6572 7361 6c20 3d20 300a 2020  aReversal = 0.  
-00021330: 2020 2020 2020 2320 5461 6b69 6e67 2053        # Taking S
-00021340: 7570 706f 7274 2035 300a 2020 2020 2020  upport 50.      
-00021350: 2020 6966 2063 6c6f 7365 203e 2073 6d61    if close > sma
-00021360: 2061 6e64 206c 6f77 203c 3d20 2873 6d61   and low <= (sma
-00021370: 202b 2073 6d61 4465 7629 3a0a 2020 2020   + smaDev):.    
-00021380: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-00021390: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-000213a0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-000213b0: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
-000213c0: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
-000213d0: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
-000213e0: 2b20 2235 304d 412d 5375 7070 6f72 7422  + "50MA-Support"
-000213f0: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-00021400: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00021410: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-00021420: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-00021430: 203d 2073 6176 6564 5b31 5d20 2b20 2235   = saved[1] + "5
-00021440: 304d 412d 5375 7070 6f72 7422 0a20 2020  0MA-Support".   
-00021450: 2020 2020 2020 2020 206d 6152 6576 6572           maRever
-00021460: 7361 6c20 3d20 310a 2020 2020 2020 2020  sal = 1.        
-00021470: 2320 5661 6c69 6461 7469 6e67 2052 6573  # Validating Res
-00021480: 6973 7461 6e63 6520 3530 0a20 2020 2020  istance 50.     
-00021490: 2020 2065 6c69 6620 636c 6f73 6520 3c20     elif close < 
-000214a0: 736d 6120 616e 6420 6869 6768 203e 3d20  sma and high >= 
-000214b0: 2873 6d61 202d 2073 6d61 4465 7629 3a0a  (sma - smaDev):.
-000214c0: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-000214d0: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
-000214e0: 6c22 5d20 3d20 280a 2020 2020 2020 2020  l"] = (.        
-000214f0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-00021500: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-00021510: 4420 2b20 636f 6c6f 7254 6578 742e 4641  D + colorText.FA
-00021520: 494c 202b 2022 3530 4d41 2d52 6573 6973  IL + "50MA-Resis
-00021530: 7422 202b 2063 6f6c 6f72 5465 7874 2e45  t" + colorText.E
-00021540: 4e44 0a20 2020 2020 2020 2020 2020 2029  ND.            )
-00021550: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
-00021560: 6544 6963 745b 224d 412d 5369 676e 616c  eDict["MA-Signal
-00021570: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-00021580: 2235 304d 412d 5265 7369 7374 220a 2020  "50MA-Resist".  
-00021590: 2020 2020 2020 2020 2020 6d61 5265 7665            maReve
-000215a0: 7273 616c 203d 202d 310a 2020 2020 2020  rsal = -1.      
-000215b0: 2020 2320 5461 6b69 6e67 2053 7570 706f    # Taking Suppo
-000215c0: 7274 2032 3030 0a20 2020 2020 2020 2065  rt 200.        e
-000215d0: 6c69 6620 636c 6f73 6520 3e20 6c6d 6120  lif close > lma 
-000215e0: 616e 6420 6c6f 7720 3c3d 2028 6c6d 6120  and low <= (lma 
-000215f0: 2b20 6c6d 6144 6576 293a 0a20 2020 2020  + lmaDev):.     
-00021600: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-00021610: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-00021620: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00021630: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
-00021640: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
-00021650: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
-00021660: 2022 3230 304d 412d 5375 7070 6f72 7422   "200MA-Support"
-00021670: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-00021680: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00021690: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+0001e0c0: 6176 6564 5b30 5d0a 2020 2020 2020 2020  aved[0].        
+0001e0d0: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+0001e0e0: 6c6f 7254 6578 742e 424f 4c44 0a20 2020  lorText.BOLD.   
+0001e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e100: 202b 2063 6f6c 6f72 5465 7874 2e47 5245   + colorText.GRE
+0001e110: 454e 0a20 2020 2020 2020 2020 2020 2020  EN.             
+0001e120: 2020 2020 2020 202b 2022 4950 4f20 4261         + "IPO Ba
+0001e130: 7365 2022 0a20 2020 2020 2020 2020 2020  se ".           
+0001e140: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+0001e150: 5465 7874 2e46 4149 4c0a 2020 2020 2020  Text.FAIL.      
+0001e160: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001e170: 6622 287b 6177 6179 7d20 2529 220a 2020  f"({away} %)".  
+0001e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e190: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+0001e1a0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+0001e1b0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001e1c0: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
+0001e1d0: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
+0001e1e0: 2066 2249 504f 2042 6173 6520 287b 6177   f"IPO Base ({aw
+0001e1f0: 6179 7d20 2529 220a 2020 2020 2020 2020  ay} %)".        
+0001e200: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0001e210: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0001e220: 616c 7365 0a0a 2020 2020 2340 6d65 6173  alse..    #@meas
+0001e230: 7572 655f 7469 6d65 0a20 2020 2023 2056  ure_time.    # V
+0001e240: 616c 6964 6174 6520 4c6f 7265 6e74 7a69  alidate Lorentzi
+0001e250: 616e 2043 6c61 7373 6966 6963 6174 696f  an Classificatio
+0001e260: 6e20 7369 676e 616c 0a20 2020 2064 6566  n signal.    def
+0001e270: 2076 616c 6964 6174 654c 6f72 656e 747a   validateLorentz
+0001e280: 6961 6e28 7365 6c66 2c20 6466 2c20 7363  ian(self, df, sc
+0001e290: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
+0001e2a0: 6374 2c20 6c6f 6f6b 466f 723d 3329 3a0a  ct, lookFor=3):.
+0001e2b0: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
+0001e2c0: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
+0001e2d0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+0001e2e0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0001e2f0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0001e300: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
+0001e310: 2023 206c 6f6f 6b46 6f72 3a20 312d 4275   # lookFor: 1-Bu
+0001e320: 792c 2032 2d53 656c 6c2c 2033 2d41 6e79  y, 2-Sell, 3-Any
+0001e330: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+0001e340: 6461 7461 5b3a 3a2d 315d 2020 2320 5265  data[::-1]  # Re
+0001e350: 7665 7273 6520 7468 6520 6461 7461 6672  verse the datafr
+0001e360: 616d 650a 2020 2020 2020 2020 6461 7461  ame.        data
+0001e370: 203d 2064 6174 612e 7265 6e61 6d65 280a   = data.rename(.
+0001e380: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+0001e390: 6d6e 733d 7b0a 2020 2020 2020 2020 2020  mns={.          
+0001e3a0: 2020 2020 2020 224f 7065 6e22 3a20 226f        "Open": "o
+0001e3b0: 7065 6e22 2c0a 2020 2020 2020 2020 2020  pen",.          
+0001e3c0: 2020 2020 2020 2243 6c6f 7365 223a 2022        "Close": "
+0001e3d0: 636c 6f73 6522 2c0a 2020 2020 2020 2020  close",.        
+0001e3e0: 2020 2020 2020 2020 2248 6967 6822 3a20          "High": 
+0001e3f0: 2268 6967 6822 2c0a 2020 2020 2020 2020  "high",.        
+0001e400: 2020 2020 2020 2020 224c 6f77 223a 2022          "Low": "
+0001e410: 6c6f 7722 2c0a 2020 2020 2020 2020 2020  low",.          
+0001e420: 2020 2020 2020 2256 6f6c 756d 6522 3a20        "Volume": 
+0001e430: 2276 6f6c 756d 6522 2c0a 2020 2020 2020  "volume",.      
+0001e440: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0001e450: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
+0001e460: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+0001e470: 5375 7070 7265 7373 4f75 7470 7574 2873  SuppressOutput(s
+0001e480: 7570 7072 6573 735f 7374 646f 7574 3d54  uppress_stdout=T
+0001e490: 7275 652c 2073 7570 7072 6573 735f 7374  rue, suppress_st
+0001e4a0: 6465 7272 3d54 7275 6529 3a0a 2020 2020  derr=True):.    
+0001e4b0: 2020 2020 2020 2020 2020 2020 6c63 203d              lc =
+0001e4c0: 2061 7461 2e4c 6f72 656e 747a 6961 6e43   ata.LorentzianC
+0001e4d0: 6c61 7373 6966 6963 6174 696f 6e28 6461  lassification(da
+0001e4e0: 7461 3d64 6174 6129 0a20 2020 2020 2020  ta=data).       
+0001e4f0: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
+0001e500: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
+0001e510: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
+0001e520: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
+0001e530: 6174 7465 726e 2229 0a20 2020 2020 2020  attern").       
+0001e540: 2020 2020 2069 6620 6c63 2e64 662e 696c       if lc.df.il
+0001e550: 6f63 5b2d 315d 5b22 6973 4e65 7742 7579  oc[-1]["isNewBuy
+0001e560: 5369 676e 616c 225d 3a0a 2020 2020 2020  Signal"]:.      
+0001e570: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+0001e580: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
+0001e590: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0001e5a0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+0001e5b0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+0001e5c0: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
+0001e5d0: 4545 4e20 2b20 224c 6f72 656e 747a 6961  EEN + "Lorentzia
+0001e5e0: 6e2d 4275 7922 202b 2063 6f6c 6f72 5465  n-Buy" + colorTe
+0001e5f0: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
+0001e600: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0001e610: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+0001e620: 745b 2250 6174 7465 726e 225d 203d 2073  t["Pattern"] = s
+0001e630: 6176 6564 5b31 5d20 2b20 224c 6f72 656e  aved[1] + "Loren
+0001e640: 747a 6961 6e2d 4275 7922 0a20 2020 2020  tzian-Buy".     
+0001e650: 2020 2020 2020 2020 2020 2069 6620 6c6f             if lo
+0001e660: 6f6b 466f 7220 213d 2032 3a20 2320 4e6f  okFor != 2: # No
+0001e670: 7420 5365 6c6c 0a20 2020 2020 2020 2020  t Sell.         
+0001e680: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001e690: 6e20 5472 7565 0a20 2020 2020 2020 2020  n True.         
+0001e6a0: 2020 2065 6c69 6620 6c63 2e64 662e 696c     elif lc.df.il
+0001e6b0: 6f63 5b2d 315d 5b22 6973 4e65 7753 656c  oc[-1]["isNewSel
+0001e6c0: 6c53 6967 6e61 6c22 5d3a 0a20 2020 2020  lSignal"]:.     
+0001e6d0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+0001e6e0: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
+0001e6f0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+0001e700: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
+0001e710: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
+0001e720: 4c44 202b 2063 6f6c 6f72 5465 7874 2e46  LD + colorText.F
+0001e730: 4149 4c20 2b20 224c 6f72 656e 747a 6961  AIL + "Lorentzia
+0001e740: 6e2d 5365 6c6c 2220 2b20 636f 6c6f 7254  n-Sell" + colorT
+0001e750: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+0001e760: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0001e770: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+0001e780: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
+0001e790: 7361 7665 645b 315d 202b 2022 4c6f 7265  saved[1] + "Lore
+0001e7a0: 6e74 7a69 616e 2d53 656c 6c22 0a20 2020  ntzian-Sell".   
+0001e7b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001e7c0: 6c6f 6f6b 466f 7220 213d 2031 3a20 2320  lookFor != 1: # 
+0001e7d0: 4e6f 7420 4275 790a 2020 2020 2020 2020  Not Buy.        
+0001e7e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001e7f0: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+0001e800: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+0001e810: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+0001e820: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
+0001e830: 2020 2320 5661 6c75 6545 7272 6f72 3a20    # ValueError: 
+0001e840: 6f70 6572 616e 6473 2063 6f75 6c64 206e  operands could n
+0001e850: 6f74 2062 6520 6272 6f61 6463 6173 7420  ot be broadcast 
+0001e860: 746f 6765 7468 6572 2077 6974 6820 7368  together with sh
+0001e870: 6170 6573 2028 3230 2c29 2028 3236 2c29  apes (20,) (26,)
+0001e880: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+0001e890: 696c 6520 222f 6f70 742f 686f 6d65 6272  ile "/opt/homebr
+0001e8a0: 6577 2f6c 6962 2f70 7974 686f 6e33 2e31  ew/lib/python3.1
+0001e8b0: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
+0001e8c0: 6164 7661 6e63 6564 5f74 612f 4c6f 7265  advanced_ta/Lore
+0001e8d0: 6e74 7a69 616e 436c 6173 7369 6669 6361  ntzianClassifica
+0001e8e0: 7469 6f6e 2f43 6c61 7373 6966 6965 722e  tion/Classifier.
+0001e8f0: 7079 222c 206c 696e 6520 3138 362c 2069  py", line 186, i
+0001e900: 6e20 5f5f 696e 6974 5f5f 0a20 2020 2020  n __init__.     
+0001e910: 2020 2020 2020 2023 2046 696c 6520 222f         # File "/
+0001e920: 6f70 742f 686f 6d65 6272 6577 2f6c 6962  opt/homebrew/lib
+0001e930: 2f70 7974 686f 6e33 2e31 312f 7369 7465  /python3.11/site
+0001e940: 2d70 6163 6b61 6765 732f 6164 7661 6e63  -packages/advanc
+0001e950: 6564 5f74 612f 4c6f 7265 6e74 7a69 616e  ed_ta/Lorentzian
+0001e960: 436c 6173 7369 6669 6361 7469 6f6e 2f43  Classification/C
+0001e970: 6c61 7373 6966 6965 722e 7079 222c 206c  lassifier.py", l
+0001e980: 696e 6520 3339 352c 2069 6e20 5f5f 636c  ine 395, in __cl
+0001e990: 6173 7369 6679 0a20 2020 2020 2020 2020  assify.         
+0001e9a0: 2020 2023 2046 696c 6520 222f 6f70 742f     # File "/opt/
+0001e9b0: 686f 6d65 6272 6577 2f6c 6962 2f70 7974  homebrew/lib/pyt
+0001e9c0: 686f 6e33 2e31 312f 7369 7465 2d70 6163  hon3.11/site-pac
+0001e9d0: 6b61 6765 732f 7061 6e64 6173 2f63 6f72  kages/pandas/cor
+0001e9e0: 652f 6f70 732f 636f 6d6d 6f6e 2e70 7922  e/ops/common.py"
+0001e9f0: 2c20 6c69 6e65 2037 362c 2069 6e20 6e65  , line 76, in ne
+0001ea00: 775f 6d65 7468 6f64 0a20 2020 2020 2020  w_method.       
+0001ea10: 2020 2020 2023 2046 696c 6520 222f 6f70       # File "/op
+0001ea20: 742f 686f 6d65 6272 6577 2f6c 6962 2f70  t/homebrew/lib/p
+0001ea30: 7974 686f 6e33 2e31 312f 7369 7465 2d70  ython3.11/site-p
+0001ea40: 6163 6b61 6765 732f 7061 6e64 6173 2f63  ackages/pandas/c
+0001ea50: 6f72 652f 6172 7261 796c 696b 652e 7079  ore/arraylike.py
+0001ea60: 222c 206c 696e 6520 3730 2c20 696e 205f  ", line 70, in _
+0001ea70: 5f61 6e64 5f5f 0a20 2020 2020 2020 2020  _and__.         
+0001ea80: 2020 2023 2046 696c 6520 222f 6f70 742f     # File "/opt/
+0001ea90: 686f 6d65 6272 6577 2f6c 6962 2f70 7974  homebrew/lib/pyt
+0001eaa0: 686f 6e33 2e31 312f 7369 7465 2d70 6163  hon3.11/site-pac
+0001eab0: 6b61 6765 732f 7061 6e64 6173 2f63 6f72  kages/pandas/cor
+0001eac0: 652f 7365 7269 6573 2e70 7922 2c20 6c69  e/series.py", li
+0001ead0: 6e65 2035 3831 302c 2069 6e20 5f6c 6f67  ne 5810, in _log
+0001eae0: 6963 616c 5f6d 6574 686f 640a 2020 2020  ical_method.    
+0001eaf0: 2020 2020 2020 2020 2320 4669 6c65 2022          # File "
+0001eb00: 2f6f 7074 2f68 6f6d 6562 7265 772f 6c69  /opt/homebrew/li
+0001eb10: 622f 7079 7468 6f6e 332e 3131 2f73 6974  b/python3.11/sit
+0001eb20: 652d 7061 636b 6167 6573 2f70 616e 6461  e-packages/panda
+0001eb30: 732f 636f 7265 2f6f 7073 2f61 7272 6179  s/core/ops/array
+0001eb40: 5f6f 7073 2e70 7922 2c20 6c69 6e65 2034  _ops.py", line 4
+0001eb50: 3536 2c20 696e 206c 6f67 6963 616c 5f6f  56, in logical_o
+0001eb60: 700a 2020 2020 2020 2020 2020 2020 2320  p.            # 
+0001eb70: 4669 6c65 2022 2f6f 7074 2f68 6f6d 6562  File "/opt/homeb
+0001eb80: 7265 772f 6c69 622f 7079 7468 6f6e 332e  rew/lib/python3.
+0001eb90: 3131 2f73 6974 652d 7061 636b 6167 6573  11/site-packages
+0001eba0: 2f70 616e 6461 732f 636f 7265 2f6f 7073  /pandas/core/ops
+0001ebb0: 2f61 7272 6179 5f6f 7073 2e70 7922 2c20  /array_ops.py", 
+0001ebc0: 6c69 6e65 2033 3634 2c20 696e 206e 615f  line 364, in na_
+0001ebd0: 6c6f 6769 6361 6c5f 6f70 0a20 2020 2020  logical_op.     
+0001ebe0: 2020 2020 2020 2023 2073 656c 662e 6465         # self.de
+0001ebf0: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
+0001ec00: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
+0001ec10: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+0001ec20: 2070 6173 730a 2020 2020 2020 2020 7265   pass.        re
+0001ec30: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
+0001ec40: 2320 7661 6c69 6461 7465 2069 6620 7468  # validate if th
+0001ec50: 6520 7374 6f63 6b20 6861 7320 6265 656e  e stock has been
+0001ec60: 2068 6176 696e 6720 6c6f 7765 7220 6c6f   having lower lo
+0001ec70: 7773 2c20 6c6f 7765 7220 6869 6768 730a  ws, lower highs.
+0001ec80: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0001ec90: 4c6f 7765 7248 6967 6873 4c6f 7765 724c  LowerHighsLowerL
+0001eca0: 6f77 7328 7365 6c66 2c20 6466 293a 0a20  ows(self, df):. 
+0001ecb0: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
+0001ecc0: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
+0001ecd0: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+0001ece0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+0001ecf0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
+0001ed00: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
+0001ed10: 6461 7930 203d 2064 6174 610a 2020 2020  day0 = data.    
+0001ed20: 2020 2020 6461 7931 203d 2064 6174 615b      day1 = data[
+0001ed30: 313a 5d0a 2020 2020 2020 2020 6461 7932  1:].        day2
+0001ed40: 203d 2064 6174 615b 323a 5d0a 2020 2020   = data[2:].    
+0001ed50: 2020 2020 6461 7933 203d 2064 6174 615b      day3 = data[
+0001ed60: 333a 5d0a 2020 2020 2020 2020 6c6f 7765  3:].        lowe
+0001ed70: 7248 6967 6873 203d 2028 0a20 2020 2020  rHighs = (.     
+0001ed80: 2020 2020 2020 2028 6461 7930 5b22 4869         (day0["Hi
+0001ed90: 6768 225d 2e69 6c6f 635b 305d 203c 2064  gh"].iloc[0] < d
+0001eda0: 6179 315b 2248 6967 6822 5d2e 696c 6f63  ay1["High"].iloc
+0001edb0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+0001edc0: 2061 6e64 2028 6461 7931 5b22 4869 6768   and (day1["High
+0001edd0: 225d 2e69 6c6f 635b 305d 203c 2064 6179  "].iloc[0] < day
+0001ede0: 325b 2248 6967 6822 5d2e 696c 6f63 5b30  2["High"].iloc[0
+0001edf0: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
+0001ee00: 6e64 2028 6461 7932 5b22 4869 6768 225d  nd (day2["High"]
+0001ee10: 2e69 6c6f 635b 305d 203c 2064 6179 335b  .iloc[0] < day3[
+0001ee20: 2248 6967 6822 5d2e 696c 6f63 5b30 5d29  "High"].iloc[0])
+0001ee30: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0001ee40: 2020 206c 6f77 6572 4c6f 7773 203d 2028     lowerLows = (
+0001ee50: 0a20 2020 2020 2020 2020 2020 2028 6461  .            (da
+0001ee60: 7930 5b22 4c6f 7722 5d2e 696c 6f63 5b30  y0["Low"].iloc[0
+0001ee70: 5d20 3c20 6461 7931 5b22 4c6f 7722 5d2e  ] < day1["Low"].
+0001ee80: 696c 6f63 5b30 5d29 0a20 2020 2020 2020  iloc[0]).       
+0001ee90: 2020 2020 2061 6e64 2028 6461 7931 5b22       and (day1["
+0001eea0: 4c6f 7722 5d2e 696c 6f63 5b30 5d20 3c20  Low"].iloc[0] < 
+0001eeb0: 6461 7932 5b22 4c6f 7722 5d2e 696c 6f63  day2["Low"].iloc
+0001eec0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+0001eed0: 2061 6e64 2028 6461 7932 5b22 4c6f 7722   and (day2["Low"
+0001eee0: 5d2e 696c 6f63 5b30 5d20 3c20 6461 7933  ].iloc[0] < day3
+0001eef0: 5b22 4c6f 7722 5d2e 696c 6f63 5b30 5d29  ["Low"].iloc[0])
+0001ef00: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0001ef10: 2020 2068 6967 6865 7252 5349 203d 2028     higherRSI = (
+0001ef20: 0a20 2020 2020 2020 2020 2020 2028 6461  .            (da
+0001ef30: 7930 5b22 5253 4922 5d2e 696c 6f63 5b30  y0["RSI"].iloc[0
+0001ef40: 5d20 3c20 6461 7931 5b22 5253 4922 5d2e  ] < day1["RSI"].
+0001ef50: 696c 6f63 5b30 5d29 0a20 2020 2020 2020  iloc[0]).       
+0001ef60: 2020 2020 2061 6e64 2028 6461 7931 5b22       and (day1["
+0001ef70: 5253 4922 5d2e 696c 6f63 5b30 5d20 3c20  RSI"].iloc[0] < 
+0001ef80: 6461 7932 5b22 5253 4922 5d2e 696c 6f63  day2["RSI"].iloc
+0001ef90: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+0001efa0: 2061 6e64 2028 6461 7932 5b22 5253 4922   and (day2["RSI"
+0001efb0: 5d2e 696c 6f63 5b30 5d20 3c20 6461 7933  ].iloc[0] < day3
+0001efc0: 5b22 5253 4922 5d2e 696c 6f63 5b30 5d29  ["RSI"].iloc[0])
+0001efd0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001efe0: 2064 6179 305b 2252 5349 225d 2e69 6c6f   day0["RSI"].ilo
+0001eff0: 635b 305d 203e 3d20 3530 0a20 2020 2020  c[0] >= 50.     
+0001f000: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
+0001f010: 7572 6e20 6c6f 7765 7248 6967 6873 2061  urn lowerHighs a
+0001f020: 6e64 206c 6f77 6572 4c6f 7773 2061 6e64  nd lowerLows and
+0001f030: 2068 6967 6865 7252 5349 0a0a 2020 2020   higherRSI..    
+0001f040: 2320 5661 6c69 6461 7465 2069 6620 7265  # Validate if re
+0001f050: 6365 6e74 2076 6f6c 756d 6520 6973 206c  cent volume is l
+0001f060: 6f77 6573 7420 6f66 206c 6173 7420 274e  owest of last 'N
+0001f070: 2720 4461 7973 0a20 2020 2064 6566 2076  ' Days.    def v
+0001f080: 616c 6964 6174 654c 6f77 6573 7456 6f6c  alidateLowestVol
+0001f090: 756d 6528 7365 6c66 2c20 6466 2c20 6461  ume(self, df, da
+0001f0a0: 7973 466f 724c 6f77 6573 7456 6f6c 756d  ysForLowestVolum
+0001f0b0: 6529 3a0a 2020 2020 2020 2020 6966 2064  e):.        if d
+0001f0c0: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+0001f0d0: 2864 6629 203d 3d20 303a 0a20 2020 2020  (df) == 0:.     
+0001f0e0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0001f0f0: 6c73 650a 2020 2020 2020 2020 6461 7461  lse.        data
+0001f100: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
+0001f110: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+0001f120: 2e66 696c 6c6e 6128 3029 0a20 2020 2020  .fillna(0).     
+0001f130: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+0001f140: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
+0001f150: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
+0001f160: 2020 2020 2069 6620 6461 7973 466f 724c       if daysForL
+0001f170: 6f77 6573 7456 6f6c 756d 6520 6973 204e  owestVolume is N
+0001f180: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0001f190: 2064 6179 7346 6f72 4c6f 7765 7374 566f   daysForLowestVo
+0001f1a0: 6c75 6d65 203d 2033 300a 2020 2020 2020  lume = 30.      
+0001f1b0: 2020 6966 206c 656e 2864 6174 6129 203c    if len(data) <
+0001f1c0: 2064 6179 7346 6f72 4c6f 7765 7374 566f   daysForLowestVo
+0001f1d0: 6c75 6d65 3a0a 2020 2020 2020 2020 2020  lume:.          
+0001f1e0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+0001f1f0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
+0001f200: 7461 2e68 6561 6428 6461 7973 466f 724c  ta.head(daysForL
+0001f210: 6f77 6573 7456 6f6c 756d 6529 0a20 2020  owestVolume).   
+0001f220: 2020 2020 2072 6563 656e 7420 3d20 6461       recent = da
+0001f230: 7461 2e68 6561 6428 3129 0a20 2020 2020  ta.head(1).     
+0001f240: 2020 2069 6620 6c65 6e28 7265 6365 6e74     if len(recent
+0001f250: 2920 3c20 313a 0a20 2020 2020 2020 2020  ) < 1:.         
+0001f260: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0001f270: 2020 2020 2020 2020 6966 2028 7265 6365          if (rece
+0001f280: 6e74 5b22 566f 6c75 6d65 225d 2e69 6c6f  nt["Volume"].ilo
+0001f290: 635b 305d 203c 3d20 6461 7461 2e64 6573  c[0] <= data.des
+0001f2a0: 6372 6962 6528 295b 2256 6f6c 756d 6522  cribe()["Volume"
+0001f2b0: 5d5b 226d 696e 225d 2920 616e 6420 7265  ]["min"]) and re
+0001f2c0: 6365 6e74 5b0a 2020 2020 2020 2020 2020  cent[.          
+0001f2d0: 2020 2256 6f6c 756d 6522 0a20 2020 2020    "Volume".     
+0001f2e0: 2020 205d 5b30 5d20 213d 206e 702e 6e61     ][0] != np.na
+0001f2f0: 6e3a 0a20 2020 2020 2020 2020 2020 2072  n:.            r
+0001f300: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+0001f310: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0001f320: 0a20 2020 2023 2056 616c 6964 6174 6520  .    # Validate 
+0001f330: 4c54 5020 7769 7468 696e 206c 696d 6974  LTP within limit
+0001f340: 730a 2020 2020 6465 6620 7661 6c69 6461  s.    def valida
+0001f350: 7465 4c54 5028 7365 6c66 2c20 6466 2c20  teLTP(self, df, 
+0001f360: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
+0001f370: 4469 6374 2c20 6d69 6e4c 5450 3d4e 6f6e  Dict, minLTP=Non
+0001f380: 652c 206d 6178 4c54 503d 4e6f 6e65 2c6d  e, maxLTP=None,m
+0001f390: 696e 4368 616e 6765 3d30 293a 0a20 2020  inChange=0):.   
+0001f3a0: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
+0001f3b0: 6f70 7928 290a 2020 2020 2020 2020 6c74  opy().        lt
+0001f3c0: 7056 616c 6964 203d 2046 616c 7365 0a20  pValid = False. 
+0001f3d0: 2020 2020 2020 2069 6620 6d69 6e4c 5450         if minLTP
+0001f3e0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0001f3f0: 2020 2020 2020 6d69 6e4c 5450 203d 2073        minLTP = s
+0001f400: 656c 662e 636f 6e66 6967 4d61 6e61 6765  elf.configManage
+0001f410: 722e 6d69 6e4c 5450 0a20 2020 2020 2020  r.minLTP.       
+0001f420: 2069 6620 6d61 784c 5450 2069 7320 4e6f   if maxLTP is No
+0001f430: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001f440: 6d61 784c 5450 203d 2073 656c 662e 636f  maxLTP = self.co
+0001f450: 6e66 6967 4d61 6e61 6765 722e 6d61 784c  nfigManager.maxL
+0001f460: 5450 0a20 2020 2020 2020 2064 6174 6120  TP.        data 
+0001f470: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
+0001f480: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+0001f490: 6461 7461 2e72 6570 6c61 6365 285b 6e70  data.replace([np
+0001f4a0: 2e69 6e66 2c20 2d6e 702e 696e 665d 2c20  .inf, -np.inf], 
+0001f4b0: 3029 0a20 2020 2020 2020 2072 6563 656e  0).        recen
+0001f4c0: 7420 3d20 6461 7461 2e68 6561 6428 3129  t = data.head(1)
+0001f4d0: 0a0a 2020 2020 2020 2020 7063 745f 6368  ..        pct_ch
+0001f4e0: 616e 6765 203d 2028 6461 7461 5b3a 3a2d  ange = (data[::-
+0001f4f0: 315d 5b22 436c 6f73 6522 5d2e 7063 745f  1]["Close"].pct_
+0001f500: 6368 616e 6765 2829 202a 2031 3030 292e  change() * 100).
+0001f510: 696c 6f63 5b2d 315d 0a20 2020 2020 2020  iloc[-1].       
+0001f520: 2069 6620 7063 745f 6368 616e 6765 203d   if pct_change =
+0001f530: 3d20 6e70 2e69 6e66 206f 7220 7063 745f  = np.inf or pct_
+0001f540: 6368 616e 6765 203d 3d20 2d6e 702e 696e  change == -np.in
+0001f550: 663a 0a20 2020 2020 2020 2020 2020 2070  f:.            p
+0001f560: 6374 5f63 6861 6e67 6520 3d20 300a 2020  ct_change = 0.  
+0001f570: 2020 2020 2020 7063 745f 7361 7665 203d        pct_save =
+0001f580: 2022 252e 3166 2525 2220 2520 7063 745f   "%.1f%%" % pct_
+0001f590: 6368 616e 6765 0a20 2020 2020 2020 2069  change.        i
+0001f5a0: 6620 7063 745f 6368 616e 6765 203e 2030  f pct_change > 0
+0001f5b0: 2e32 3a0a 2020 2020 2020 2020 2020 2020  .2:.            
+0001f5c0: 7063 745f 6368 616e 6765 203d 2063 6f6c  pct_change = col
+0001f5d0: 6f72 5465 7874 2e47 5245 454e 202b 2028  orText.GREEN + (
+0001f5e0: 2225 2e31 6625 2522 2025 2070 6374 5f63  "%.1f%%" % pct_c
+0001f5f0: 6861 6e67 6529 202b 2063 6f6c 6f72 5465  hange) + colorTe
+0001f600: 7874 2e45 4e44 0a20 2020 2020 2020 2065  xt.END.        e
+0001f610: 6c69 6620 7063 745f 6368 616e 6765 203c  lif pct_change <
+0001f620: 202d 302e 323a 0a20 2020 2020 2020 2020   -0.2:.         
+0001f630: 2020 2070 6374 5f63 6861 6e67 6520 3d20     pct_change = 
+0001f640: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
+0001f650: 2028 2225 2e31 6625 2522 2025 2070 6374   ("%.1f%%" % pct
+0001f660: 5f63 6861 6e67 6529 202b 2063 6f6c 6f72  _change) + color
+0001f670: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+0001f680: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001f690: 2020 2070 6374 5f63 6861 6e67 6520 3d20     pct_change = 
+0001f6a0: 636f 6c6f 7254 6578 742e 5741 524e 202b  colorText.WARN +
+0001f6b0: 2028 2225 2e31 6625 2522 2025 2070 6374   ("%.1f%%" % pct
+0001f6c0: 5f63 6861 6e67 6529 202b 2063 6f6c 6f72  _change) + color
+0001f6d0: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+0001f6e0: 2073 6176 6544 6963 745b 2225 4368 6e67   saveDict["%Chng
+0001f6f0: 225d 203d 2070 6374 5f73 6176 650a 2020  "] = pct_save.  
+0001f700: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+0001f710: 5b22 2543 686e 6722 5d20 3d20 7063 745f  ["%Chng"] = pct_
+0001f720: 6368 616e 6765 0a20 2020 2020 2020 206c  change.        l
+0001f730: 7470 203d 2072 6f75 6e64 2872 6563 656e  tp = round(recen
+0001f740: 745b 2243 6c6f 7365 225d 2e69 6c6f 635b  t["Close"].iloc[
+0001f750: 305d 2c20 3229 0a20 2020 2020 2020 2076  0], 2).        v
+0001f760: 6572 6966 7953 7461 6765 5477 6f20 3d20  erifyStageTwo = 
+0001f770: 5472 7565 0a20 2020 2020 2020 2069 6620  True.        if 
+0001f780: 6c65 6e28 6461 7461 2920 3e20 3235 303a  len(data) > 250:
+0001f790: 0a20 2020 2020 2020 2020 2020 2079 6561  .            yea
+0001f7a0: 726c 794c 6f77 203d 2064 6174 612e 6865  rlyLow = data.he
+0001f7b0: 6164 2832 3530 295b 2243 6c6f 7365 225d  ad(250)["Close"]
+0001f7c0: 2e6d 696e 2829 0a20 2020 2020 2020 2020  .min().         
+0001f7d0: 2020 2079 6561 726c 7948 6967 6820 3d20     yearlyHigh = 
+0001f7e0: 6461 7461 2e68 6561 6428 3235 3029 5b22  data.head(250)["
+0001f7f0: 436c 6f73 6522 5d2e 6d61 7828 290a 2020  Close"].max().  
+0001f800: 2020 2020 2020 2020 2020 6966 206c 7470            if ltp
+0001f810: 203c 2028 3220 2a20 7965 6172 6c79 4c6f   < (2 * yearlyLo
+0001f820: 7729 2061 6e64 206c 7470 203c 2028 302e  w) and ltp < (0.
+0001f830: 3735 202a 2079 6561 726c 7948 6967 6829  75 * yearlyHigh)
+0001f840: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001f850: 2020 7665 7269 6679 5374 6167 6554 776f    verifyStageTwo
+0001f860: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+0001f870: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+0001f880: 6963 745b 2253 746f 636b 225d 203d 2063  ict["Stock"] = c
+0001f890: 6f6c 6f72 5465 7874 2e46 4149 4c20 2b20  olorText.FAIL + 
+0001f8a0: 7361 7665 4469 6374 5b22 5374 6f63 6b22  saveDict["Stock"
+0001f8b0: 5d20 2b20 636f 6c6f 7254 6578 742e 454e  ] + colorText.EN
+0001f8c0: 440a 2020 2020 2020 2020 6966 206c 7470  D.        if ltp
+0001f8d0: 203e 3d20 6d69 6e4c 5450 2061 6e64 206c   >= minLTP and l
+0001f8e0: 7470 203c 3d20 6d61 784c 5450 3a0a 2020  tp <= maxLTP:.  
+0001f8f0: 2020 2020 2020 2020 2020 6c74 7056 616c            ltpVal
+0001f900: 6964 203d 2054 7275 650a 2020 2020 2020  id = True.      
+0001f910: 2020 2020 2020 6966 206d 696e 4368 616e        if minChan
+0001f920: 6765 2021 3d20 303a 0a20 2020 2020 2020  ge != 0:.       
+0001f930: 2020 2020 2020 2020 2023 2055 7365 7220           # User 
+0001f940: 6861 7320 7375 7070 6c69 6564 2073 6f6d  has supplied som
+0001f950: 6520 6669 6c74 6572 2066 6f72 2070 6572  e filter for per
+0001f960: 6365 6e74 6167 6520 6368 616e 6765 0a20  centage change. 
+0001f970: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0001f980: 7470 5661 6c69 6420 3d20 666c 6f61 7428  tpValid = float(
+0001f990: 7374 7228 7063 745f 7361 7665 292e 7265  str(pct_save).re
+0001f9a0: 706c 6163 6528 2225 222c 2222 2929 203e  place("%","")) >
+0001f9b0: 3d20 6d69 6e43 6861 6e67 650a 2020 2020  = minChange.    
+0001f9c0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+0001f9d0: 5b22 4c54 5022 5d20 3d20 726f 756e 6428  ["LTP"] = round(
+0001f9e0: 6c74 702c 2032 290a 2020 2020 2020 2020  ltp, 2).        
+0001f9f0: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+0001fa00: 4c54 5022 5d20 3d20 2863 6f6c 6f72 5465  LTP"] = (colorTe
+0001fa10: 7874 2e47 5245 454e 2069 6620 6c74 7056  xt.GREEN if ltpV
+0001fa20: 616c 6964 2065 6c73 6520 636f 6c6f 7254  alid else colorT
+0001fa30: 6578 742e 4641 494c 2920 2b20 2822 252e  ext.FAIL) + ("%.
+0001fa40: 3266 2220 2520 6c74 7029 202b 2063 6f6c  2f" % ltp) + col
+0001fa50: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
+0001fa60: 2020 2020 2020 2072 6574 7572 6e20 6c74         return lt
+0001fa70: 7056 616c 6964 2c20 7665 7269 6679 5374  pValid, verifySt
+0001fa80: 6167 6554 776f 0a20 2020 2020 2020 2073  ageTwo.        s
+0001fa90: 6372 6565 6e44 6963 745b 224c 5450 225d  creenDict["LTP"]
+0001faa0: 203d 2063 6f6c 6f72 5465 7874 2e46 4149   = colorText.FAI
+0001fab0: 4c20 2b20 2822 252e 3266 2220 2520 6c74  L + ("%.2f" % lt
+0001fac0: 7029 202b 2063 6f6c 6f72 5465 7874 2e45  p) + colorText.E
+0001fad0: 4e44 0a20 2020 2020 2020 2073 6176 6544  ND.        saveD
+0001fae0: 6963 745b 224c 5450 225d 203d 2072 6f75  ict["LTP"] = rou
+0001faf0: 6e64 286c 7470 2c20 3229 0a20 2020 2020  nd(ltp, 2).     
+0001fb00: 2020 2072 6574 7572 6e20 6c74 7056 616c     return ltpVal
+0001fb10: 6964 2c20 7665 7269 6679 5374 6167 6554  id, verifyStageT
+0001fb20: 776f 0a0a 2020 2020 6465 6620 7661 6c69  wo..    def vali
+0001fb30: 6461 7465 4c54 5046 6f72 506f 7274 666f  dateLTPForPortfo
+0001fb40: 6c69 6f43 616c 6328 7365 6c66 2c20 6466  lioCalc(self, df
+0001fb50: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
+0001fb60: 7665 4469 6374 2c72 6571 7565 7374 6564  veDict,requested
+0001fb70: 5065 7269 6f64 3d30 293a 0a20 2020 2020  Period=0):.     
+0001fb80: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
+0001fb90: 7928 290a 2020 2020 2020 2020 7065 7269  y().        peri
+0001fba0: 6f64 7320 3d20 7365 6c66 2e63 6f6e 6669  ods = self.confi
+0001fbb0: 674d 616e 6167 6572 2e70 6572 696f 6473  gManager.periods
+0001fbc0: 5261 6e67 650a 2020 2020 2020 2020 6966  Range.        if
+0001fbd0: 2072 6571 7565 7374 6564 5065 7269 6f64   requestedPeriod
+0001fbe0: 203e 2030 2061 6e64 2072 6571 7565 7374   > 0 and request
+0001fbf0: 6564 5065 7269 6f64 206e 6f74 2069 6e20  edPeriod not in 
+0001fc00: 7065 7269 6f64 733a 0a20 2020 2020 2020  periods:.       
+0001fc10: 2020 2020 2070 6572 696f 6473 2e61 7070       periods.app
+0001fc20: 656e 6428 7265 7175 6573 7465 6450 6572  end(requestedPer
+0001fc30: 696f 6429 0a20 2020 2020 2020 2070 7265  iod).        pre
+0001fc40: 7669 6f75 735f 7265 6365 6e74 203d 2064  vious_recent = d
+0001fc50: 6174 612e 6865 6164 2831 290a 2020 2020  ata.head(1).    
+0001fc60: 2020 2020 7072 6576 696f 7573 5f72 6563      previous_rec
+0001fc70: 656e 742e 7265 7365 745f 696e 6465 7828  ent.reset_index(
+0001fc80: 696e 706c 6163 653d 5472 7565 290a 2020  inplace=True).  
+0001fc90: 2020 2020 2020 6361 6c63 5f64 6174 6520        calc_date 
+0001fca0: 3d20 7374 7228 7072 6576 696f 7573 5f72  = str(previous_r
+0001fcb0: 6563 656e 742e 696c 6f63 5b3a 2c20 305d  ecent.iloc[:, 0]
+0001fcc0: 5b30 5d29 2e73 706c 6974 2822 2022 295b  [0]).split(" ")[
+0001fcd0: 305d 0a20 2020 2020 2020 2066 6f72 2070  0].        for p
+0001fce0: 7264 2069 6e20 7065 7269 6f64 733a 0a20  rd in periods:. 
+0001fcf0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+0001fd00: 6e28 6461 7461 2920 3e3d 2070 7264 202b  n(data) >= prd +
+0001fd10: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0001fd20: 2020 2020 7072 6576 4c74 7020 3d20 6461      prevLtp = da
+0001fd30: 7461 5b22 436c 6f73 6522 5d2e 696c 6f63  ta["Close"].iloc
+0001fd40: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+0001fd50: 2020 2020 6c74 7054 6479 203d 2064 6174      ltpTdy = dat
+0001fd60: 615b 2243 6c6f 7365 225d 2e69 6c6f 635b  a["Close"].iloc[
+0001fd70: 7072 645d 0a20 2020 2020 2020 2020 2020  prd].           
+0001fd80: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+0001fd90: 6365 2870 7265 764c 7470 2c70 642e 5365  ce(prevLtp,pd.Se
+0001fda0: 7269 6573 293a 0a20 2020 2020 2020 2020  ries):.         
+0001fdb0: 2020 2020 2020 2020 2020 2070 7265 764c             prevL
+0001fdc0: 7470 203d 2070 7265 764c 7470 5b30 5d0a  tp = prevLtp[0].
+0001fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fde0: 2020 2020 6c74 7054 6479 203d 206c 7470      ltpTdy = ltp
+0001fdf0: 5464 795b 305d 0a20 2020 2020 2020 2020  Tdy[0].         
+0001fe00: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+0001fe10: 745b 6622 4c54 507b 7072 647d 225d 203d  t[f"LTP{prd}"] =
+0001fe20: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0001fe30: 2020 2020 2020 2028 636f 6c6f 7254 6578         (colorTex
+0001fe40: 742e 4752 4545 4e20 6966 2028 6c74 7054  t.GREEN if (ltpT
+0001fe50: 6479 203e 3d20 7072 6576 4c74 7029 2065  dy >= prevLtp) e
+0001fe60: 6c73 6520 2863 6f6c 6f72 5465 7874 2e46  lse (colorText.F
+0001fe70: 4149 4c29 290a 2020 2020 2020 2020 2020  AIL)).          
+0001fe80: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
+0001fe90: 227b 3a2e 3266 7d22 2e66 6f72 6d61 7428  "{:.2f}".format(
+0001fea0: 6c74 7054 6479 2929 0a20 2020 2020 2020  ltpTdy)).       
+0001feb0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001fec0: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
+0001fed0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0001fee0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001fef0: 6372 6565 6e44 6963 745b 6622 4772 6f77  creenDict[f"Grow
+0001ff00: 7468 7b70 7264 7d22 5d20 3d20 280a 2020  th{prd}"] = (.  
+0001ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ff20: 2020 2863 6f6c 6f72 5465 7874 2e47 5245    (colorText.GRE
+0001ff30: 454e 2069 6620 286c 7470 5464 7920 3e3d  EN if (ltpTdy >=
+0001ff40: 2070 7265 764c 7470 2920 656c 7365 2028   prevLtp) else (
+0001ff50: 636f 6c6f 7254 6578 742e 4641 494c 2929  colorText.FAIL))
+0001ff60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ff70: 2020 2020 202b 2073 7472 2822 7b3a 2e32       + str("{:.2
+0001ff80: 667d 222e 666f 726d 6174 286c 7470 5464  f}".format(ltpTd
+0001ff90: 7920 2d20 7072 6576 4c74 7029 290a 2020  y - prevLtp)).  
+0001ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ffb0: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
+0001ffc0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+0001ffd0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001ffe0: 2020 2020 7361 7665 4469 6374 5b66 224c      saveDict[f"L
+0001fff0: 5450 7b70 7264 7d22 5d20 3d20 726f 756e  TP{prd}"] = roun
+00020000: 6428 6c74 7054 6479 2c20 3229 0a20 2020  d(ltpTdy, 2).   
+00020010: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00020020: 6544 6963 745b 6622 4772 6f77 7468 7b70  eDict[f"Growth{p
+00020030: 7264 7d22 5d20 3d20 726f 756e 6428 6c74  rd}"] = round(lt
+00020040: 7054 6479 202d 2070 7265 764c 7470 2c20  pTdy - prevLtp, 
+00020050: 3229 0a20 2020 2020 2020 2020 2020 2020  2).             
+00020060: 2020 2069 6620 7072 6420 3d3d 2032 3220     if prd == 22 
+00020070: 6f72 2028 7072 6420 3d3d 2072 6571 7565  or (prd == reque
+00020080: 7374 6564 5065 7269 6f64 293a 0a20 2020  stedPeriod):.   
+00020090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000200a0: 2063 6861 6e67 6550 6572 6365 6e74 203d   changePercent =
+000200b0: 2072 6f75 6e64 2828 2870 7265 764c 7470   round(((prevLtp
+000200c0: 2d6c 7470 5464 7929 2069 6620 7265 7175  -ltpTdy) if requ
+000200d0: 6573 7465 6450 6572 696f 6420 3d3d 3020  estedPeriod ==0 
+000200e0: 656c 7365 2028 6c74 7054 6479 202d 2070  else (ltpTdy - p
+000200f0: 7265 764c 7470 2929 2a31 3030 2f6c 7470  revLtp))*100/ltp
+00020100: 5464 792c 2032 290a 2020 2020 2020 2020  Tdy, 2).        
+00020110: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00020120: 4469 6374 5b66 227b 7072 647d 2d50 6420  Dict[f"{prd}-Pd 
+00020130: 2522 5d20 3d20 6622 7b63 6861 6e67 6550  %"] = f"{changeP
+00020140: 6572 6365 6e74 7d25 2220 6966 206e 6f74  ercent}%" if not
+00020150: 2070 642e 6973 6e61 2863 6861 6e67 6550   pd.isna(changeP
+00020160: 6572 6365 6e74 2920 656c 7365 2027 2d27  ercent) else '-'
+00020170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020180: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00020190: 6622 7b70 7264 7d2d 5064 2025 225d 203d  f"{prd}-Pd %"] =
+000201a0: 2028 2863 6f6c 6f72 5465 7874 2e47 5245   ((colorText.GRE
+000201b0: 454e 2069 6620 6368 616e 6765 5065 7263  EN if changePerc
+000201c0: 656e 7420 3e3d 3020 656c 7365 2063 6f6c  ent >=0 else col
+000201d0: 6f72 5465 7874 2e46 4149 4c29 202b 2066  orText.FAIL) + f
+000201e0: 227b 6368 616e 6765 5065 7263 656e 747d  "{changePercent}
+000201f0: 2522 202b 2063 6f6c 6f72 5465 7874 2e45  %" + colorText.E
+00020200: 4e44 2920 6966 206e 6f74 2070 642e 6973  ND) if not pd.is
+00020210: 6e61 2863 6861 6e67 6550 6572 6365 6e74  na(changePercent
+00020220: 2920 656c 7365 2027 2d27 0a20 2020 2020  ) else '-'.     
+00020230: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+00020240: 6e44 6963 745b 2244 6174 6522 5d20 3d20  nDict["Date"] = 
+00020250: 6361 6c63 5f64 6174 650a 2020 2020 2020  calc_date.      
+00020260: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00020270: 6374 5b22 4461 7465 225d 203d 2063 616c  ct["Date"] = cal
+00020280: 635f 6461 7465 0a20 2020 2020 2020 2020  c_date.         
+00020290: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000202a0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+000202b0: 745b 6622 4c54 507b 7072 647d 225d 203d  t[f"LTP{prd}"] =
+000202c0: 206e 702e 6e61 6e0a 2020 2020 2020 2020   np.nan.        
+000202d0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+000202e0: 5b66 2247 726f 7774 687b 7072 647d 225d  [f"Growth{prd}"]
+000202f0: 203d 206e 702e 6e61 6e0a 2020 2020 2020   = np.nan.      
+00020300: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+00020310: 4469 6374 5b22 4461 7465 225d 203d 2063  Dict["Date"] = c
+00020320: 616c 635f 6461 7465 0a20 2020 2020 2020  alc_date.       
+00020330: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00020340: 745b 2244 6174 6522 5d20 3d20 6361 6c63  t["Date"] = calc
+00020350: 5f64 6174 650a 0a20 2020 2023 2046 696e  _date..    # Fin
+00020360: 6420 7374 6f63 6b73 2074 6861 7420 6172  d stocks that ar
+00020370: 6520 6265 6172 6973 6820 696e 7472 6164  e bearish intrad
+00020380: 6179 3a20 4d61 6364 2048 6973 746f 6772  ay: Macd Histogr
+00020390: 616d 206e 6567 6174 6976 650a 2020 2020  am negative.    
+000203a0: 6465 6620 7661 6c69 6461 7465 4d41 4344  def validateMACD
+000203b0: 4869 7374 6f67 7261 6d42 656c 6f77 3028  HistogramBelow0(
+000203c0: 7365 6c66 2c20 6466 293a 0a20 2020 2020  self, df):.     
+000203d0: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
+000203e0: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
+000203f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00020400: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+00020410: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
+00020420: 7928 290a 2020 2020 2020 2020 6461 7461  y().        data
+00020430: 203d 2064 6174 612e 6669 6c6c 6e61 2830   = data.fillna(0
+00020440: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
+00020450: 2064 6174 612e 7265 706c 6163 6528 5b6e   data.replace([n
+00020460: 702e 696e 662c 202d 6e70 2e69 6e66 5d2c  p.inf, -np.inf],
+00020470: 2030 290a 2020 2020 2020 2020 6461 7461   0).        data
+00020480: 203d 2064 6174 615b 3a3a 2d31 5d20 2023   = data[::-1]  #
+00020490: 2052 6576 6572 7365 2074 6865 2064 6174   Reverse the dat
+000204a0: 6166 7261 6d65 2073 6f20 7468 6174 2069  aframe so that i
+000204b0: 7473 2074 6865 206f 6c64 6573 7420 6461  ts the oldest da
+000204c0: 7465 2066 6972 7374 0a20 2020 2020 2020  te first.       
+000204d0: 206d 6163 6420 3d20 706b 7461 6c69 622e   macd = pktalib.
+000204e0: 4d41 4344 2864 6174 615b 2243 6c6f 7365  MACD(data["Close
+000204f0: 225d 2c20 3132 2c20 3236 2c20 3929 5b32  "], 12, 26, 9)[2
+00020500: 5d2e 7461 696c 2831 290a 2020 2020 2020  ].tail(1).      
+00020510: 2020 7265 7475 726e 206d 6163 642e 696c    return macd.il
+00020520: 6f63 5b3a 315d 5b30 5d20 3c20 300a 0a20  oc[:1][0] < 0.. 
+00020530: 2020 2023 406d 6561 7375 7265 5f74 696d     #@measure_tim
+00020540: 650a 2020 2020 2320 4669 6e64 2069 6620  e.    # Find if 
+00020550: 7374 6f63 6b20 6761 696e 696e 6720 6275  stock gaining bu
+00020560: 6c6c 6973 6820 6d6f 6d65 6e74 756d 0a20  llish momentum. 
+00020570: 2020 2064 6566 2076 616c 6964 6174 654d     def validateM
+00020580: 6f6d 656e 7475 6d28 7365 6c66 2c20 6466  omentum(self, df
+00020590: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
+000205a0: 7665 4469 6374 293a 0a20 2020 2020 2020  veDict):.       
+000205b0: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
+000205c0: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
+000205d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000205e0: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+000205f0: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
+00020600: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
+00020610: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+00020620: 3d20 6461 7461 2e68 6561 6428 3329 0a20  = data.head(3). 
+00020630: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00020640: 6e28 6461 7461 2920 3c20 333a 0a20 2020  n(data) < 3:.   
+00020650: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00020660: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00020670: 2020 2020 2020 666f 7220 726f 7720 696e        for row in
+00020680: 2064 6174 612e 6974 6572 726f 7773 2829   data.iterrows()
+00020690: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000206a0: 2020 2320 416c 6c20 3320 6361 6e64 6c65    # All 3 candle
+000206b0: 7320 7368 6f75 6c64 2062 6520 4772 6565  s should be Gree
+000206c0: 6e20 616e 6420 4e4f 5420 4369 7263 7569  n and NOT Circui
+000206d0: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
+000206e0: 2020 2079 6320 3d20 726f 775b 315d 5b22     yc = row[1]["
+000206f0: 436c 6f73 6522 5d0a 2020 2020 2020 2020  Close"].        
+00020700: 2020 2020 2020 2020 796f 203d 2072 6f77          yo = row
+00020710: 5b31 5d5b 224f 7065 6e22 5d0a 2020 2020  [1]["Open"].    
+00020720: 2020 2020 2020 2020 2020 2020 6966 2079              if y
+00020730: 6320 3c3d 2079 6f3a 0a20 2020 2020 2020  c <= yo:.       
+00020740: 2020 2020 2020 2020 2020 2020 2023 2073               # s
+00020750: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
+00020760: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
+00020770: 2020 2020 2020 2020 2020 2020 2023 2020               #  
+00020780: 2020 2066 2753 746f 636b 3a7b 7361 7665     f'Stock:{save
+00020790: 4469 6374 5b22 5374 6f63 6b22 5d7d 2c20  Dict["Stock"]}, 
+000207a0: 6973 206e 6f74 2061 206d 6f6d 656e 7475  is not a momentu
+000207b0: 6d2d 6761 696e 6572 2062 6563 6175 7365  m-gainer because
+000207c0: 2079 6573 7465 7264 6179 2d63 6c6f 7365   yesterday-close
+000207d0: 2028 7b79 637d 2920 3c3d 2079 6573 7465   ({yc}) <= yeste
+000207e0: 7264 6179 2d6f 7065 6e20 287b 796f 7d29  rday-open ({yo})
+000207f0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+00020800: 2020 2020 2020 2320 290a 2020 2020 2020        # ).      
+00020810: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00020820: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+00020830: 2020 2020 2020 206f 7065 6e44 6573 6320         openDesc 
+00020840: 3d20 6461 7461 2e73 6f72 745f 7661 6c75  = data.sort_valu
+00020850: 6573 2862 793d 5b22 4f70 656e 225d 2c20  es(by=["Open"], 
+00020860: 6173 6365 6e64 696e 673d 4661 6c73 6529  ascending=False)
+00020870: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
+00020880: 7365 4465 7363 203d 2064 6174 612e 736f  seDesc = data.so
+00020890: 7274 5f76 616c 7565 7328 6279 3d5b 2243  rt_values(by=["C
+000208a0: 6c6f 7365 225d 2c20 6173 6365 6e64 696e  lose"], ascendin
+000208b0: 673d 4661 6c73 6529 0a20 2020 2020 2020  g=False).       
+000208c0: 2020 2020 2076 6f6c 4465 7363 203d 2064       volDesc = d
+000208d0: 6174 612e 736f 7274 5f76 616c 7565 7328  ata.sort_values(
+000208e0: 6279 3d5b 2256 6f6c 756d 6522 5d2c 2061  by=["Volume"], a
+000208f0: 7363 656e 6469 6e67 3d46 616c 7365 290a  scending=False).
+00020900: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+00020910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020920: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
+00020930: 2020 2020 2020 2020 2020 6461 7461 2e65            data.e
+00020940: 7175 616c 7328 6f70 656e 4465 7363 290a  quals(openDesc).
+00020950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020960: 2020 2020 616e 6420 6461 7461 2e65 7175      and data.equ
+00020970: 616c 7328 636c 6f73 6544 6573 6329 0a20  als(closeDesc). 
+00020980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020990: 2020 2061 6e64 2064 6174 612e 6571 7561     and data.equa
+000209a0: 6c73 2876 6f6c 4465 7363 290a 2020 2020  ls(volDesc).    
+000209b0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
+000209c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000209d0: 2020 2023 2073 656c 662e 6465 6661 756c     # self.defaul
+000209e0: 745f 6c6f 6767 6572 2e69 6e66 6f28 0a20  t_logger.info(. 
+000209f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020a00: 2020 2023 2020 2020 2066 2753 746f 636b     #     f'Stock
+00020a10: 3a7b 7361 7665 4469 6374 5b22 5374 6f63  :{saveDict["Stoc
+00020a20: 6b22 5d7d 2c20 6f70 656e 2c63 6c6f 7365  k"]}, open,close
+00020a30: 2061 6e64 2076 6f6c 756d 6520 6571 7561   and volume equa
+00020a40: 6c20 6672 6f6d 2064 6179 2062 6566 6f72  l from day befor
+00020a50: 6520 7965 7374 6572 6461 792e 2041 2070  e yesterday. A p
+00020a60: 6f74 656e 7469 616c 206d 6f6d 656e 7475  otential momentu
+00020a70: 6d2d 6761 696e 6572 2127 0a20 2020 2020  m-gainer!'.     
+00020a80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00020a90: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00020aa0: 2020 2020 2020 2074 6f20 3d20 6461 7461         to = data
+00020ab0: 5b22 4f70 656e 225d 2e69 6c6f 635b 305d  ["Open"].iloc[0]
+00020ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020ad0: 2020 2020 2079 6320 3d20 6461 7461 5b22       yc = data["
+00020ae0: 436c 6f73 6522 5d2e 696c 6f63 5b31 5d0a  Close"].iloc[1].
+00020af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b00: 2020 2020 796f 203d 2064 6174 615b 224f      yo = data["O
+00020b10: 7065 6e22 5d2e 696c 6f63 5b31 5d0a 2020  pen"].iloc[1].  
+00020b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b30: 2020 6479 6320 3d20 6461 7461 5b22 436c    dyc = data["Cl
+00020b40: 6f73 6522 5d2e 696c 6f63 5b32 5d0a 2020  ose"].iloc[2].  
+00020b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020b60: 2020 6966 2028 746f 203e 3d20 7963 2920    if (to >= yc) 
+00020b70: 616e 6420 2879 6f20 3e3d 2064 7963 293a  and (yo >= dyc):
+00020b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00020b90: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+00020ba0: 6465 6661 756c 745f 6c6f 6767 6572 2e69  default_logger.i
+00020bb0: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
+00020bc0: 2020 2020 2020 2020 2020 2020 2023 2020               #  
+00020bd0: 2020 2066 2753 746f 636b 3a7b 7361 7665     f'Stock:{save
+00020be0: 4469 6374 5b22 5374 6f63 6b22 5d7d 2c20  Dict["Stock"]}, 
+00020bf0: 6973 2061 206d 6f6d 656e 7475 6d2d 6761  is a momentum-ga
+00020c00: 696e 6572 2062 6563 6175 7365 2074 6f64  iner because tod
+00020c10: 6179 2d6f 7065 6e20 287b 746f 7d29 203e  ay-open ({to}) >
+00020c20: 3d20 7965 7374 6572 6461 792d 636c 6f73  = yesterday-clos
+00020c30: 6520 287b 7963 7d29 2061 6e64 2079 6573  e ({yc}) and yes
+00020c40: 7465 7264 6179 2d6f 7065 6e28 7b79 6f7d  terday-open({yo}
+00020c50: 2920 3e3d 2064 6179 2d62 6566 6f72 652d  ) >= day-before-
+00020c60: 636c 6f73 6528 7b64 7963 7d29 270a 2020  close({dyc})'.  
+00020c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c80: 2020 2020 2020 2320 290a 2020 2020 2020        # ).      
+00020c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020ca0: 2020 7361 7665 6420 3d20 7365 6c66 2e66    saved = self.f
+00020cb0: 696e 6443 7572 7265 6e74 5361 7665 6456  indCurrentSavedV
+00020cc0: 616c 7565 2873 6372 6565 6e44 6963 742c  alue(screenDict,
+00020cd0: 2073 6176 6544 6963 742c 2022 5061 7474   saveDict, "Patt
+00020ce0: 6572 6e22 290a 2020 2020 2020 2020 2020  ern").          
+00020cf0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00020d00: 7265 656e 4469 6374 5b22 5061 7474 6572  reenDict["Patter
+00020d10: 6e22 5d20 3d20 280a 2020 2020 2020 2020  n"] = (.        
+00020d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d30: 2020 2020 7361 7665 645b 305d 0a20 2020      saved[0].   
+00020d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d50: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+00020d60: 5465 7874 2e42 4f4c 440a 2020 2020 2020  Text.BOLD.      
+00020d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d80: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+00020d90: 742e 4752 4545 4e0a 2020 2020 2020 2020  t.GREEN.        
+00020da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020db0: 2020 2020 2b20 224d 6f6d 656e 7475 6d20      + "Momentum 
+00020dc0: 4761 696e 6572 220a 2020 2020 2020 2020  Gainer".        
+00020dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020de0: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+00020df0: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
+00020e00: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00020e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020e20: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
+00020e30: 5061 7474 6572 6e22 5d20 3d20 7361 7665  Pattern"] = save
+00020e40: 645b 315d 202b 2022 4d6f 6d65 6e74 756d  d[1] + "Momentum
+00020e50: 2047 6169 6e65 7222 0a20 2020 2020 2020   Gainer".       
+00020e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020e70: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00020e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020e90: 2023 2073 656c 662e 6465 6661 756c 745f   # self.default_
+00020ea0: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+00020eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020ec0: 2023 2020 2020 2066 2753 746f 636b 3a7b   #     f'Stock:{
+00020ed0: 7361 7665 4469 6374 5b22 5374 6f63 6b22  saveDict["Stock"
+00020ee0: 5d7d 2c20 6973 206e 6f74 2061 206d 6f6d  ]}, is not a mom
+00020ef0: 656e 7475 6d2d 6761 696e 6572 2062 6563  entum-gainer bec
+00020f00: 6175 7365 2065 6974 6865 7220 746f 6461  ause either toda
+00020f10: 792d 6f70 656e 2028 7b74 6f7d 2920 3c20  y-open ({to}) < 
+00020f20: 7965 7374 6572 6461 792d 636c 6f73 6520  yesterday-close 
+00020f30: 287b 7963 7d29 206f 7220 7965 7374 6572  ({yc}) or yester
+00020f40: 6461 792d 6f70 656e 287b 796f 7d29 203c  day-open({yo}) <
+00020f50: 2064 6179 2d62 6566 6f72 652d 636c 6f73   day-before-clos
+00020f60: 6528 7b64 7963 7d29 270a 2020 2020 2020  e({dyc})'.      
+00020f70: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00020f80: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+00020f90: 6365 7074 2049 6e64 6578 4572 726f 7220  cept IndexError 
+00020fa0: 6173 2065 3a20 2320 7072 6167 6d61 3a20  as e: # pragma: 
+00020fb0: 6e6f 2063 6f76 6572 0a20 2020 2020 2020  no cover.       
+00020fc0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00020fd0: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
+00020fe0: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
+00020ff0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00021000: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
+00021010: 745f 6c6f 6767 6572 2e64 6562 7567 2864  t_logger.debug(d
+00021020: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
+00021030: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
+00021040: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00021050: 7365 0a20 2020 2020 2020 2065 7863 6570  se.        excep
+00021060: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00021070: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
+00021080: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
+00021090: 2020 7365 6c66 2e64 6566 6175 6c74 5f6c    self.default_l
+000210a0: 6f67 6765 722e 6465 6275 6728 652c 2065  ogger.debug(e, e
+000210b0: 7863 5f69 6e66 6f3d 5472 7565 290a 2020  xc_info=True).  
+000210c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000210d0: 2046 616c 7365 0a0a 2020 2020 2340 6d65   False..    #@me
+000210e0: 6173 7572 655f 7469 6d65 0a20 2020 2023  asure_time.    #
+000210f0: 2056 616c 6964 6174 6520 4d6f 7669 6e67   Validate Moving
+00021100: 2061 7665 7261 6765 7320 616e 6420 6c6f   averages and lo
+00021110: 6f6b 2066 6f72 2062 7579 2f73 656c 6c20  ok for buy/sell 
+00021120: 7369 676e 616c 730a 2020 2020 6465 6620  signals.    def 
+00021130: 7661 6c69 6461 7465 4d6f 7669 6e67 4176  validateMovingAv
+00021140: 6572 6167 6573 2873 656c 662c 2064 662c  erages(self, df,
+00021150: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
+00021160: 6544 6963 742c 206d 6152 616e 6765 3d32  eDict, maRange=2
+00021170: 2e35 2c6d 614c 656e 6774 683d 3029 3a0a  .5,maLength=0):.
+00021180: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00021190: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
+000211a0: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
+000211b0: 6c6e 6128 3029 0a20 2020 2020 2020 2064  lna(0).        d
+000211c0: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
+000211d0: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
+000211e0: 696e 665d 2c20 3029 0a20 2020 2020 2020  inf], 0).       
+000211f0: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
+00021200: 6561 6428 3129 0a20 2020 2020 2020 206d  ead(1).        m
+00021210: 6153 6967 6e61 6c73 203d 205b 5d0a 2020  aSignals = [].  
+00021220: 2020 2020 2020 6966 2073 7472 286d 614c        if str(maL
+00021230: 656e 6774 6829 2069 6e20 5b22 3022 2c22  ength) in ["0","
+00021240: 3222 2c22 3322 5d3a 0a20 2020 2020 2020  2","3"]:.       
+00021250: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
+00021260: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
+00021270: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
+00021280: 6374 2c73 6176 6544 6963 742c 224d 412d  ct,saveDict,"MA-
+00021290: 5369 676e 616c 2229 0a20 2020 2020 2020  Signal").       
+000212a0: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+000212b0: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
+000212c0: 5b22 534d 4122 5d2e 696c 6f63 5b30 5d20  ["SMA"].iloc[0] 
+000212d0: 3e20 7265 6365 6e74 5b22 4c4d 4122 5d2e  > recent["LMA"].
+000212e0: 696c 6f63 5b30 5d0a 2020 2020 2020 2020  iloc[0].        
+000212f0: 2020 2020 2020 2020 616e 6420 7265 6365          and rece
+00021300: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
+00021310: 5b30 5d20 3e20 7265 6365 6e74 5b22 534d  [0] > recent["SM
+00021320: 4122 5d2e 696c 6f63 5b30 5d0a 2020 2020  A"].iloc[0].    
+00021330: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+00021340: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+00021350: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
+00021360: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
+00021370: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+00021380: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
+00021390: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
+000213a0: 2e47 5245 454e 202b 2022 4275 6c6c 6973  .GREEN + "Bullis
+000213b0: 6822 202b 2063 6f6c 6f72 5465 7874 2e45  h" + colorText.E
+000213c0: 4e44 0a20 2020 2020 2020 2020 2020 2020  ND.             
+000213d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000213e0: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
+000213f0: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
+00021400: 6564 5b31 5d20 2b20 2242 756c 6c69 7368  ed[1] + "Bullish
+00021410: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00021420: 2020 6d61 5369 676e 616c 732e 6170 7065    maSignals.appe
+00021430: 6e64 2822 3322 290a 2020 2020 2020 2020  nd("3").        
+00021440: 2020 2020 656c 6966 2072 6563 656e 745b      elif recent[
+00021450: 2253 4d41 225d 2e69 6c6f 635b 305d 203c  "SMA"].iloc[0] <
+00021460: 2072 6563 656e 745b 224c 4d41 225d 2e69   recent["LMA"].i
+00021470: 6c6f 635b 305d 3a0a 2020 2020 2020 2020  loc[0]:.        
+00021480: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+00021490: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+000214a0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+000214b0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+000214c0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+000214d0: 4420 2b20 636f 6c6f 7254 6578 742e 4641  D + colorText.FA
+000214e0: 494c 202b 2022 4265 6172 6973 6822 202b  IL + "Bearish" +
+000214f0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
+00021500: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00021510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021520: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
+00021530: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
+00021540: 5d20 2b20 2242 6561 7269 7368 220a 2020  ] + "Bearish".  
+00021550: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00021560: 5369 676e 616c 732e 6170 7065 6e64 2822  Signals.append("
+00021570: 3222 290a 2020 2020 2020 2020 2020 2020  2").            
+00021580: 656c 6966 2072 6563 656e 745b 2253 4d41  elif recent["SMA
+00021590: 225d 2e69 6c6f 635b 305d 203d 3d20 303a  "].iloc[0] == 0:
+000215a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000215b0: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
+000215c0: 5369 676e 616c 225d 203d 2028 0a20 2020  Signal"] = (.   
+000215d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000215e0: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
+000215f0: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
+00021600: 6f72 5465 7874 2e57 4152 4e20 2b20 2255  orText.WARN + "U
+00021610: 6e6b 6e6f 776e 2220 2b20 636f 6c6f 7254  nknown" + colorT
+00021620: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+00021630: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00021640: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00021650: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+00021660: 3d20 7361 7665 645b 315d 202b 2022 556e  = saved[1] + "Un
+00021670: 6b6e 6f77 6e22 0a20 2020 2020 2020 2020  known".         
+00021680: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00021690: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
 000216a0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-000216b0: 203d 2073 6176 6564 5b31 5d20 2b20 2232   = saved[1] + "2
-000216c0: 3030 4d41 2d53 7570 706f 7274 220a 2020  00MA-Support".  
-000216d0: 2020 2020 2020 2020 2020 6d61 5265 7665            maReve
-000216e0: 7273 616c 203d 2031 0a20 2020 2020 2020  rsal = 1.       
-000216f0: 2023 2056 616c 6964 6174 696e 6720 5265   # Validating Re
-00021700: 7369 7374 616e 6365 2032 3030 0a20 2020  sistance 200.   
-00021710: 2020 2020 2065 6c69 6620 636c 6f73 6520       elif close 
-00021720: 3c20 6c6d 6120 616e 6420 6869 6768 203e  < lma and high >
-00021730: 3d20 286c 6d61 202d 206c 6d61 4465 7629  = (lma - lmaDev)
-00021740: 3a0a 2020 2020 2020 2020 2020 2020 7363  :.            sc
-00021750: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
-00021760: 6e61 6c22 5d20 3d20 280a 2020 2020 2020  nal"] = (.      
-00021770: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
-00021780: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
-00021790: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
-000217a0: 4641 494c 202b 2022 3230 304d 412d 5265  FAIL + "200MA-Re
-000217b0: 7369 7374 2220 2b20 636f 6c6f 7254 6578  sist" + colorTex
-000217c0: 742e 454e 440a 2020 2020 2020 2020 2020  t.END.          
-000217d0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000217e0: 7361 7665 4469 6374 5b22 4d41 2d53 6967  saveDict["MA-Sig
-000217f0: 6e61 6c22 5d20 3d20 7361 7665 645b 315d  nal"] = saved[1]
-00021800: 202b 2022 3230 304d 412d 5265 7369 7374   + "200MA-Resist
-00021810: 220a 2020 2020 2020 2020 2020 2020 6d61  ".            ma
-00021820: 5265 7665 7273 616c 203d 202d 310a 2020  Reversal = -1.  
-00021830: 2020 2020 2020 2320 466f 7220 6120 4275        # For a Bu
-00021840: 6c6c 6973 6820 4361 6e64 6c65 0a20 2020  llish Candle.   
-00021850: 2020 2020 2069 6620 7365 6c66 2e67 6574       if self.get
-00021860: 4361 6e64 6c65 5479 7065 2864 6174 6129  CandleType(data)
-00021870: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00021880: 4372 6f73 7369 6e67 2075 7020 3530 0a20  Crossing up 50. 
-00021890: 2020 2020 2020 2020 2020 2069 6620 6f70             if op
-000218a0: 656e 203c 2073 6d61 2061 6e64 2063 6c6f  en < sma and clo
-000218b0: 7365 203e 2073 6d61 3a0a 2020 2020 2020  se > sma:.      
-000218c0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-000218d0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
-000218e0: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
-000218f0: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
-00021900: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
-00021910: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
-00021920: 4752 4545 4e20 2b20 2242 756c 6c43 726f  GREEN + "BullCro
-00021930: 7373 2d35 304d 4122 202b 2063 6f6c 6f72  ss-50MA" + color
-00021940: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-00021950: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00021960: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-00021970: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-00021980: 203d 2073 6176 6564 5b31 5d20 2b20 2242   = saved[1] + "B
-00021990: 756c 6c43 726f 7373 2d35 304d 4122 0a20  ullCross-50MA". 
-000219a0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000219b0: 6152 6576 6572 7361 6c20 3d20 310a 2020  aReversal = 1.  
-000219c0: 2020 2020 2020 2020 2020 2320 4372 6f73            # Cros
-000219d0: 7369 6e67 2075 7020 3230 300a 2020 2020  sing up 200.    
-000219e0: 2020 2020 2020 2020 656c 6966 206f 7065          elif ope
-000219f0: 6e20 3c20 6c6d 6120 616e 6420 636c 6f73  n < lma and clos
-00021a00: 6520 3e20 6c6d 613a 0a20 2020 2020 2020  e > lma:.       
-00021a10: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00021a20: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-00021a30: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00021a40: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-00021a50: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
-00021a60: 4c44 202b 2063 6f6c 6f72 5465 7874 2e47  LD + colorText.G
-00021a70: 5245 454e 202b 2022 4275 6c6c 4372 6f73  REEN + "BullCros
-00021a80: 732d 3230 304d 4122 202b 2063 6f6c 6f72  s-200MA" + color
-00021a90: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-00021aa0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00021ab0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-00021ac0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-00021ad0: 203d 2073 6176 6564 5b31 5d20 2b20 2242   = saved[1] + "B
-00021ae0: 756c 6c43 726f 7373 2d32 3030 4d41 220a  ullCross-200MA".
-00021af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021b00: 6d61 5265 7665 7273 616c 203d 2031 0a20  maReversal = 1. 
-00021b10: 2020 2020 2020 2023 2046 6f72 2061 2042         # For a B
-00021b20: 6561 7269 7368 2043 616e 646c 650a 2020  earish Candle.  
-00021b30: 2020 2020 2020 656c 6966 206e 6f74 2073        elif not s
-00021b40: 656c 662e 6765 7443 616e 646c 6554 7970  elf.getCandleTyp
-00021b50: 6528 6461 7461 293a 0a20 2020 2020 2020  e(data):.       
-00021b60: 2020 2020 2023 2043 726f 7373 696e 6720       # Crossing 
-00021b70: 646f 776e 2035 300a 2020 2020 2020 2020  down 50.        
-00021b80: 2020 2020 6966 206f 7065 6e20 3e20 736d      if open > sm
-00021b90: 6120 616e 6420 636c 6f73 6520 3c20 736d  a and close < sm
-00021ba0: 613a 0a20 2020 2020 2020 2020 2020 2020  a:.             
-00021bb0: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
-00021bc0: 412d 5369 676e 616c 225d 203d 2028 0a20  A-Signal"] = (. 
-00021bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021be0: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
-00021bf0: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
-00021c00: 6f6c 6f72 5465 7874 2e46 4149 4c20 2b20  olorText.FAIL + 
-00021c10: 2242 6561 7243 726f 7373 2d35 304d 4122  "BearCross-50MA"
-00021c20: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-00021c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021c40: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00021c50: 2020 2073 6176 6544 6963 745b 224d 412d     saveDict["MA-
-00021c60: 5369 676e 616c 225d 203d 2073 6176 6564  Signal"] = saved
-00021c70: 5b31 5d20 2b20 2242 6561 7243 726f 7373  [1] + "BearCross
-00021c80: 2d35 304d 4122 0a20 2020 2020 2020 2020  -50MA".         
-00021c90: 2020 2020 2020 206d 6152 6576 6572 7361         maReversa
-00021ca0: 6c20 3d20 2d31 0a20 2020 2020 2020 2020  l = -1.         
-00021cb0: 2020 2023 2043 726f 7373 696e 6720 7570     # Crossing up
-00021cc0: 2032 3030 0a20 2020 2020 2020 2020 2020   200.           
-00021cd0: 2065 6c69 6620 6f70 656e 203e 206c 6d61   elif open > lma
-00021ce0: 2061 6e64 2063 6c6f 7365 203c 206c 6d61   and close < lma
-00021cf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00021d00: 2020 7363 7265 656e 4469 6374 5b22 4d41    screenDict["MA
-00021d10: 2d53 6967 6e61 6c22 5d20 3d20 280a 2020  -Signal"] = (.  
-00021d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021d30: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
-00021d40: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-00021d50: 6c6f 7254 6578 742e 4641 494c 202b 2022  lorText.FAIL + "
-00021d60: 4265 6172 4372 6f73 732d 3230 304d 4122  BearCross-200MA"
-00021d70: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-00021d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021d90: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00021da0: 2020 2073 6176 6544 6963 745b 224d 412d     saveDict["MA-
-00021db0: 5369 676e 616c 225d 203d 2073 6176 6564  Signal"] = saved
-00021dc0: 5b31 5d20 2b20 2242 6561 7243 726f 7373  [1] + "BearCross
-00021dd0: 2d32 3030 4d41 220a 2020 2020 2020 2020  -200MA".        
-00021de0: 2020 2020 2020 2020 6d61 5265 7665 7273          maRevers
-00021df0: 616c 203d 202d 310a 2020 2020 2020 2020  al = -1.        
-00021e00: 7265 7475 726e 206d 6152 6576 6572 7361  return maReversa
-00021e10: 6c0a 0a20 2020 2023 2046 696e 6420 4e52  l..    # Find NR
-00021e20: 7820 7261 6e67 6520 666f 7220 5265 7665  x range for Reve
-00021e30: 7273 616c 0a20 2020 2064 6566 2076 616c  rsal.    def val
-00021e40: 6964 6174 654e 6172 726f 7752 616e 6765  idateNarrowRange
-00021e50: 2873 656c 662c 2064 662c 2073 6372 6565  (self, df, scree
-00021e60: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
-00021e70: 206e 723d 3429 3a0a 2020 2020 2020 2020   nr=4):.        
-00021e80: 6966 2064 6620 6973 204e 6f6e 6520 6f72  if df is None or
-00021e90: 206c 656e 2864 6629 203d 3d20 303a 0a20   len(df) == 0:. 
-00021ea0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00021eb0: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-00021ec0: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
-00021ed0: 0a20 2020 2020 2020 2073 6176 6564 203d  .        saved =
-00021ee0: 2073 656c 662e 6669 6e64 4375 7272 656e   self.findCurren
-00021ef0: 7453 6176 6564 5661 6c75 6528 7363 7265  tSavedValue(scre
-00021f00: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-00021f10: 2c20 2250 6174 7465 726e 2229 0a20 2020  , "Pattern").   
-00021f20: 2020 2020 2069 6620 504b 4461 7465 5574       if PKDateUt
-00021f30: 696c 6974 6965 732e 6973 5472 6164 696e  ilities.isTradin
-00021f40: 6754 696d 6528 293a 0a20 2020 2020 2020  gTime():.       
-00021f50: 2020 2020 2072 616e 6765 4461 7461 203d       rangeData =
-00021f60: 2064 6174 612e 6865 6164 286e 7220 2b20   data.head(nr + 
-00021f70: 3129 5b31 3a5d 0a20 2020 2020 2020 2020  1)[1:].         
-00021f80: 2020 206e 6f77 5f63 616e 646c 6520 3d20     now_candle = 
-00021f90: 6461 7461 2e68 6561 6428 3129 0a20 2020  data.head(1).   
-00021fa0: 2020 2020 2020 2020 2072 616e 6765 4461           rangeDa
-00021fb0: 7461 5b22 5261 6e67 6522 5d20 3d20 6162  ta["Range"] = ab
-00021fc0: 7328 7261 6e67 6544 6174 615b 2243 6c6f  s(rangeData["Clo
-00021fd0: 7365 225d 202d 2072 616e 6765 4461 7461  se"] - rangeData
-00021fe0: 5b22 4f70 656e 225d 290a 2020 2020 2020  ["Open"]).      
-00021ff0: 2020 2020 2020 7265 6365 6e74 203d 2072        recent = r
-00022000: 616e 6765 4461 7461 2e68 6561 6428 3129  angeData.head(1)
-00022010: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00022020: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00022030: 2020 6c65 6e28 7265 6365 6e74 2920 3d3d    len(recent) ==
-00022040: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
-00022050: 2020 2061 6e64 2072 6563 656e 745b 2252     and recent["R
-00022060: 616e 6765 225d 2e69 6c6f 635b 305d 203d  ange"].iloc[0] =
-00022070: 3d20 7261 6e67 6544 6174 612e 6465 7363  = rangeData.desc
-00022080: 7269 6265 2829 5b22 5261 6e67 6522 5d5b  ribe()["Range"][
-00022090: 226d 696e 225d 0a20 2020 2020 2020 2020  "min"].         
-000220a0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-000220b0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-000220c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000220d0: 656c 662e 6765 7443 616e 646c 6554 7970  elf.getCandleTyp
-000220e0: 6528 7265 6365 6e74 290a 2020 2020 2020  e(recent).      
-000220f0: 2020 2020 2020 2020 2020 2020 2020 616e                an
-00022100: 6420 6e6f 775f 6361 6e64 6c65 5b22 436c  d now_candle["Cl
-00022110: 6f73 6522 5d2e 696c 6f63 5b30 5d20 3e3d  ose"].iloc[0] >=
-00022120: 2072 6563 656e 745b 2243 6c6f 7365 225d   recent["Close"]
-00022130: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
-00022140: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
-00022150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022160: 7363 7265 656e 4469 6374 5b22 5061 7474  screenDict["Patt
-00022170: 6572 6e22 5d20 3d20 280a 2020 2020 2020  ern"] = (.      
-00022180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022190: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
-000221a0: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-000221b0: 6c6f 7254 6578 742e 4752 4545 4e20 2b20  lorText.GREEN + 
-000221c0: 6622 4275 792d 4e52 7b6e 727d 2220 2b20  f"Buy-NR{nr}" + 
-000221d0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-000221e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000221f0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00022200: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-00022210: 5b22 5061 7474 6572 6e22 5d20 3d20 7361  ["Pattern"] = sa
-00022220: 7665 645b 315d 202b 2066 2242 7579 2d4e  ved[1] + f"Buy-N
-00022230: 527b 6e72 7d22 0a20 2020 2020 2020 2020  R{nr}".         
-00022240: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00022250: 6e20 5472 7565 0a20 2020 2020 2020 2020  n True.         
-00022260: 2020 2020 2020 2065 6c69 6620 280a 2020         elif (.  
-00022270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022280: 2020 6e6f 7420 7365 6c66 2e67 6574 4361    not self.getCa
-00022290: 6e64 6c65 5479 7065 2872 6563 656e 7429  ndleType(recent)
-000222a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000222b0: 2020 2020 2061 6e64 206e 6f77 5f63 616e       and now_can
-000222c0: 646c 655b 2243 6c6f 7365 225d 2e69 6c6f  dle["Close"].ilo
-000222d0: 635b 305d 203c 3d20 7265 6365 6e74 5b22  c[0] <= recent["
-000222e0: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d0a  Close"].iloc[0].
-000222f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022300: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00022310: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-00022320: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
-00022330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022340: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-00022350: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
-00022360: 4c44 202b 2063 6f6c 6f72 5465 7874 2e46  LD + colorText.F
-00022370: 4149 4c20 2b20 6622 5365 6c6c 2d4e 527b  AIL + f"Sell-NR{
-00022380: 6e72 7d22 202b 2063 6f6c 6f72 5465 7874  nr}" + colorText
-00022390: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
-000223a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000223b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000223c0: 6176 6544 6963 745b 2250 6174 7465 726e  aveDict["Pattern
-000223d0: 225d 203d 2073 6176 6564 5b31 5d20 2b20  "] = saved[1] + 
-000223e0: 6622 5365 6c6c 2d4e 527b 6e72 7d22 0a20  f"Sell-NR{nr}". 
-000223f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022400: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00022410: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00022420: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-00022430: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00022440: 2020 7261 6e67 6544 6174 6120 3d20 6461    rangeData = da
-00022450: 7461 2e68 6561 6428 6e72 290a 2020 2020  ta.head(nr).    
-00022460: 2020 2020 2020 2020 7261 6e67 6544 6174          rangeDat
-00022470: 612e 6c6f 635b 3a2c 2752 616e 6765 275d  a.loc[:,'Range']
-00022480: 203d 2061 6273 2872 616e 6765 4461 7461   = abs(rangeData
-00022490: 5b22 436c 6f73 6522 5d20 2d20 7261 6e67  ["Close"] - rang
-000224a0: 6544 6174 615b 224f 7065 6e22 5d29 0a20  eData["Open"]). 
-000224b0: 2020 2020 2020 2020 2020 2072 6563 656e             recen
-000224c0: 7420 3d20 7261 6e67 6544 6174 612e 6865  t = rangeData.he
-000224d0: 6164 2831 290a 2020 2020 2020 2020 2020  ad(1).          
-000224e0: 2020 6966 2072 6563 656e 745b 2252 616e    if recent["Ran
-000224f0: 6765 225d 2e69 6c6f 635b 305d 203d 3d20  ge"].iloc[0] == 
-00022500: 7261 6e67 6544 6174 612e 6465 7363 7269  rangeData.descri
-00022510: 6265 2829 5b22 5261 6e67 6522 5d5b 226d  be()["Range"]["m
-00022520: 696e 225d 3a0a 2020 2020 2020 2020 2020  in"]:.          
-00022530: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-00022540: 5b22 5061 7474 6572 6e22 5d20 3d20 280a  ["Pattern"] = (.
-00022550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022560: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
-00022570: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
-00022580: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
-00022590: 2b20 6622 4e52 7b6e 727d 2220 2b20 636f  + f"NR{nr}" + co
-000225a0: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
-000225b0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000225c0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-000225d0: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
-000225e0: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
-000225f0: 224e 527b 6e72 7d22 0a20 2020 2020 2020  "NR{nr}".       
-00022600: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00022610: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-00022620: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-00022630: 2020 2023 2046 696e 6420 6966 2073 746f     # Find if sto
-00022640: 636b 2069 7320 6e65 776c 7920 6c69 7374  ck is newly list
-00022650: 6564 0a20 2020 2064 6566 2076 616c 6964  ed.    def valid
-00022660: 6174 654e 6577 6c79 4c69 7374 6564 2873  ateNewlyListed(s
-00022670: 656c 662c 2064 662c 2064 6179 7354 6f4c  elf, df, daysToL
-00022680: 6f6f 6b62 6163 6b29 3a0a 2020 2020 2020  ookback):.      
-00022690: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
-000226a0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
-000226b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000226c0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-000226d0: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
-000226e0: 2829 0a20 2020 2020 2020 2064 6179 7354  ().        daysT
-000226f0: 6f4c 6f6f 6b62 6163 6b20 3d20 696e 7428  oLookback = int(
-00022700: 6461 7973 546f 4c6f 6f6b 6261 636b 5b3a  daysToLookback[:
-00022710: 2d31 5d29 0a20 2020 2020 2020 2072 6563  -1]).        rec
-00022720: 656e 7420 3d20 6461 7461 2e68 6561 6428  ent = data.head(
-00022730: 3129 0a20 2020 2020 2020 2069 6620 6c65  1).        if le
-00022740: 6e28 7265 6365 6e74 2920 3c20 313a 0a20  n(recent) < 1:. 
-00022750: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00022760: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-00022770: 6966 206c 656e 2864 6174 6129 203c 2064  if len(data) < d
-00022780: 6179 7354 6f4c 6f6f 6b62 6163 6b20 616e  aysToLookback an
-00022790: 6420 280a 2020 2020 2020 2020 2020 2020  d (.            
-000227a0: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
-000227b0: 696c 6f63 5b30 5d20 213d 206e 702e 6e61  iloc[0] != np.na
-000227c0: 6e20 616e 6420 7265 6365 6e74 5b22 436c  n and recent["Cl
-000227d0: 6f73 6522 5d2e 696c 6f63 5b30 5d20 3e20  ose"].iloc[0] > 
-000227e0: 300a 2020 2020 2020 2020 293a 0a20 2020  0.        ):.   
-000227f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00022800: 5472 7565 0a20 2020 2020 2020 2072 6574  True.        ret
-00022810: 7572 6e20 4661 6c73 650a 0a20 2020 2023  urn False..    #
-00022820: 2056 616c 6964 6174 6520 6966 2074 6865   Validate if the
-00022830: 2073 746f 636b 2070 7269 6365 7320 6172   stock prices ar
-00022840: 6520 6174 206c 6561 7374 2072 6973 696e  e at least risin
-00022850: 6720 6279 2032 2520 666f 7220 7468 6520  g by 2% for the 
-00022860: 6c61 7374 2033 2073 6573 7369 6f6e 730a  last 3 sessions.
-00022870: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00022880: 5072 6963 6552 6973 696e 6742 7941 744c  PriceRisingByAtL
-00022890: 6561 7374 3250 6572 6365 6e74 2873 656c  east2Percent(sel
-000228a0: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
-000228b0: 742c 2073 6176 6544 6963 7429 3a0a 2020  t, saveDict):.  
-000228c0: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
-000228d0: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
-000228e0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-000228f0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-00022900: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
-00022910: 636f 7079 2829 0a20 2020 2020 2020 2064  copy().        d
-00022920: 6174 6120 3d20 6461 7461 2e66 696c 6c6e  ata = data.filln
-00022930: 6128 3029 0a20 2020 2020 2020 2064 6174  a(0).        dat
-00022940: 6120 3d20 6461 7461 2e72 6570 6c61 6365  a = data.replace
-00022950: 285b 6e70 2e69 6e66 2c20 2d6e 702e 696e  ([np.inf, -np.in
-00022960: 665d 2c20 3029 0a20 2020 2020 2020 2064  f], 0).        d
-00022970: 6174 6120 3d20 6461 7461 2e68 6561 6428  ata = data.head(
-00022980: 3429 0a20 2020 2020 2020 2069 6620 6c65  4).        if le
-00022990: 6e28 6461 7461 2920 3c20 343a 0a20 2020  n(data) < 4:.   
-000229a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000229b0: 4661 6c73 650a 2020 2020 2020 2020 6461  False.        da
-000229c0: 7930 203d 2064 6174 612e 696c 6f63 5b30  y0 = data.iloc[0
-000229d0: 5d5b 2243 6c6f 7365 225d 2e69 7465 6d28  ]["Close"].item(
-000229e0: 290a 2020 2020 2020 2020 6461 794d 696e  ).        dayMin
-000229f0: 7573 3120 3d20 6461 7461 2e69 6c6f 635b  us1 = data.iloc[
-00022a00: 315d 5b22 436c 6f73 6522 5d2e 6974 656d  1]["Close"].item
-00022a10: 2829 0a20 2020 2020 2020 2064 6179 4d69  ().        dayMi
-00022a20: 6e75 7332 203d 2064 6174 612e 696c 6f63  nus2 = data.iloc
-00022a30: 5b32 5d5b 2243 6c6f 7365 225d 2e69 7465  [2]["Close"].ite
-00022a40: 6d28 290a 2020 2020 2020 2020 6461 794d  m().        dayM
-00022a50: 696e 7573 3320 3d20 6461 7461 2e69 6c6f  inus3 = data.ilo
-00022a60: 635b 335d 5b22 436c 6f73 6522 5d2e 6974  c[3]["Close"].it
-00022a70: 656d 2829 0a20 2020 2020 2020 2070 6572  em().        per
-00022a80: 6365 6e74 3320 3d20 726f 756e 6428 2864  cent3 = round((d
-00022a90: 6179 4d69 6e75 7332 202d 2064 6179 4d69  ayMinus2 - dayMi
-00022aa0: 6e75 7333 2920 2a20 3130 3020 2f20 6461  nus3) * 100 / da
-00022ab0: 794d 696e 7573 332c 2032 290a 2020 2020  yMinus3, 2).    
-00022ac0: 2020 2020 7065 7263 656e 7432 203d 2072      percent2 = r
-00022ad0: 6f75 6e64 2828 6461 794d 696e 7573 3120  ound((dayMinus1 
-00022ae0: 2d20 6461 794d 696e 7573 3229 202a 2031  - dayMinus2) * 1
-00022af0: 3030 202f 2064 6179 4d69 6e75 7332 2c20  00 / dayMinus2, 
-00022b00: 3229 0a20 2020 2020 2020 2070 6572 6365  2).        perce
-00022b10: 6e74 3120 3d20 726f 756e 6428 2864 6179  nt1 = round((day
-00022b20: 3020 2d20 6461 794d 696e 7573 3129 202a  0 - dayMinus1) *
-00022b30: 2031 3030 202f 2064 6179 4d69 6e75 7331   100 / dayMinus1
-00022b40: 2c20 3229 0a0a 2020 2020 2020 2020 6966  , 2)..        if
-00022b50: 2070 6572 6365 6e74 3120 3e3d 2032 2061   percent1 >= 2 a
-00022b60: 6e64 2070 6572 6365 6e74 3220 3e3d 2032  nd percent2 >= 2
-00022b70: 2061 6e64 2070 6572 6365 6e74 3320 3e3d   and percent3 >=
-00022b80: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-00022b90: 7063 745f 6368 616e 6765 5f74 6578 7420  pct_change_text 
-00022ba0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00022bb0: 2020 2020 2822 252e 3166 2525 2220 2520      ("%.1f%%" % 
-00022bc0: 7065 7263 656e 7431 290a 2020 2020 2020  percent1).      
-00022bd0: 2020 2020 2020 2020 2020 2b20 2822 2028            + (" (
-00022be0: 252e 3166 2525 2c22 2025 2070 6572 6365  %.1f%%," % perce
-00022bf0: 6e74 3229 0a20 2020 2020 2020 2020 2020  nt2).           
-00022c00: 2020 2020 202b 2028 2220 252e 3166 2525       + (" %.1f%%
-00022c10: 2922 2025 2070 6572 6365 6e74 3329 0a20  )" % percent3). 
-00022c20: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00022c30: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00022c40: 745b 2225 4368 6e67 225d 203d 2070 6374  t["%Chng"] = pct
-00022c50: 5f63 6861 6e67 655f 7465 7874 0a20 2020  _change_text.   
-00022c60: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-00022c70: 6963 745b 2225 4368 6e67 225d 203d 2063  ict["%Chng"] = c
-00022c80: 6f6c 6f72 5465 7874 2e47 5245 454e 202b  olorText.GREEN +
-00022c90: 2070 6374 5f63 6861 6e67 655f 7465 7874   pct_change_text
-00022ca0: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-00022cb0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00022cc0: 7572 6e20 5472 7565 2061 6e64 2073 656c  urn True and sel
-00022cd0: 662e 6765 7443 616e 646c 6554 7970 6528  f.getCandleType(
-00022ce0: 6461 7461 2e68 6561 6428 3129 290a 2020  data.head(1)).  
-00022cf0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00022d00: 7365 0a0a 2020 2020 2340 6d65 6173 7572  se..    #@measur
-00022d10: 655f 7469 6d65 0a20 2020 2023 2076 616c  e_time.    # val
-00022d20: 6964 6174 6520 6966 2052 5349 2069 7320  idate if RSI is 
-00022d30: 7769 7468 696e 2067 6976 656e 2072 616e  within given ran
-00022d40: 6765 0a20 2020 2064 6566 2076 616c 6964  ge.    def valid
-00022d50: 6174 6552 5349 2873 656c 662c 2064 662c  ateRSI(self, df,
-00022d60: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
-00022d70: 6544 6963 742c 206d 696e 5253 492c 206d  eDict, minRSI, m
-00022d80: 6178 5253 492c 7273 694b 6579 3d22 5253  axRSI,rsiKey="RS
-00022d90: 4922 293a 0a20 2020 2020 2020 2069 6620  I"):.        if 
-00022da0: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
-00022db0: 6e28 6466 2920 3d3d 2030 3a0a 2020 2020  n(df) == 0:.    
-00022dc0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00022dd0: 616c 7365 0a20 2020 2020 2020 2069 6620  alse.        if 
-00022de0: 7273 694b 6579 206e 6f74 2069 6e20 6466  rsiKey not in df
-00022df0: 2e63 6f6c 756d 6e73 3a0a 2020 2020 2020  .columns:.      
-00022e00: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00022e10: 7365 0a20 2020 2020 2020 2064 6174 6120  se.        data 
-00022e20: 3d20 6466 2e63 6f70 7928 290a 2020 2020  = df.copy().    
-00022e30: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
-00022e40: 6669 6c6c 6e61 2830 290a 2020 2020 2020  fillna(0).      
-00022e50: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
-00022e60: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
-00022e70: 6e70 2e69 6e66 5d2c 2030 290a 2020 2020  np.inf], 0).    
-00022e80: 2020 2020 7273 6920 3d20 696e 7428 6461      rsi = int(da
-00022e90: 7461 2e68 6561 6428 3129 5b72 7369 4b65  ta.head(1)[rsiKe
-00022ea0: 795d 2e69 6c6f 635b 305d 290a 2020 2020  y].iloc[0]).    
-00022eb0: 2020 2020 7361 7665 4469 6374 5b72 7369      saveDict[rsi
-00022ec0: 4b65 795d 203d 2072 7369 0a20 2020 2020  Key] = rsi.     
-00022ed0: 2020 2023 2068 7474 7073 3a2f 2f63 6861     # https://cha
-00022ee0: 7274 696e 6b2e 636f 6d2f 7363 7265 656e  rtink.com/screen
-00022ef0: 6572 2f72 7369 2d73 6372 6565 6e69 6e67  er/rsi-screening
-00022f00: 0a20 2020 2020 2020 2069 6620 7273 693e  .        if rsi>
-00022f10: 2030 2061 6e64 2072 7369 203e 3d20 6d69   0 and rsi >= mi
-00022f20: 6e52 5349 2061 6e64 2072 7369 203c 3d20  nRSI and rsi <= 
-00022f30: 6d61 7852 5349 3a20 2023 206f 7220 2872  maxRSI:  # or (r
-00022f40: 7369 203c 3d20 3731 2061 6e64 2072 7369  si <= 71 and rsi
-00022f50: 203e 3d20 3637 293a 0a20 2020 2020 2020   >= 67):.       
-00022f60: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00022f70: 7273 694b 6579 5d20 3d20 280a 2020 2020  rsiKey] = (.    
-00022f80: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-00022f90: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
-00022fa0: 6f72 5465 7874 2e47 5245 454e 202b 2073  orText.GREEN + s
-00022fb0: 7472 2872 7369 2920 2b20 636f 6c6f 7254  tr(rsi) + colorT
-00022fc0: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
-00022fd0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00022fe0: 2020 7265 7475 726e 2054 7275 6520 6966    return True if
-00022ff0: 2028 7273 694b 6579 203d 3d20 2252 5349   (rsiKey == "RSI
-00023000: 6922 2920 656c 7365 2028 7365 6c66 2e76  i") else (self.v
-00023010: 616c 6964 6174 6552 5349 2864 662c 2073  alidateRSI(df, s
-00023020: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-00023030: 6963 742c 206d 696e 5253 492c 206d 6178  ict, minRSI, max
-00023040: 5253 492c 7273 694b 6579 3d22 5253 4969  RSI,rsiKey="RSIi
-00023050: 2229 206f 7220 5472 7565 290a 2020 2020  ") or True).    
-00023060: 2020 2020 7363 7265 656e 4469 6374 5b72      screenDict[r
-00023070: 7369 4b65 795d 203d 2063 6f6c 6f72 5465  siKey] = colorTe
-00023080: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
-00023090: 6578 742e 4641 494c 202b 2073 7472 2872  ext.FAIL + str(r
-000230a0: 7369 2920 2b20 636f 6c6f 7254 6578 742e  si) + colorText.
-000230b0: 454e 440a 2020 2020 2020 2020 2320 4966  END.        # If
-000230c0: 2065 6974 6865 7220 6461 696c 7920 6f72   either daily or
-000230d0: 2069 6e74 7261 6461 7920 5253 4920 636f   intraday RSI co
-000230e0: 6d65 7320 7769 7468 696e 2072 616e 6765  mes within range
-000230f0: 3f0a 2020 2020 2020 2020 7265 7475 726e  ?.        return
-00023100: 2046 616c 7365 2069 6620 2872 7369 4b65   False if (rsiKe
-00023110: 7920 3d3d 2022 5253 4969 2229 2065 6c73  y == "RSIi") els
-00023120: 6520 2873 656c 662e 7661 6c69 6461 7465  e (self.validate
-00023130: 5253 4928 6466 2c20 7363 7265 656e 4469  RSI(df, screenDi
-00023140: 6374 2c20 7361 7665 4469 6374 2c20 6d69  ct, saveDict, mi
-00023150: 6e52 5349 2c20 6d61 7852 5349 2c72 7369  nRSI, maxRSI,rsi
-00023160: 4b65 793d 2252 5349 6922 2929 0a0a 2020  Key="RSIi"))..  
-00023170: 2020 2320 5661 6c69 6461 7465 2069 6620    # Validate if 
-00023180: 7468 6520 7374 6f63 6b20 6973 2062 756c  the stock is bul
-00023190: 6c69 7368 2069 6e20 7468 6520 7368 6f72  lish in the shor
-000231a0: 7420 7465 726d 0a20 2020 2064 6566 2076  t term.    def v
-000231b0: 616c 6964 6174 6553 686f 7274 5465 726d  alidateShortTerm
-000231c0: 4275 6c6c 6973 6828 7365 6c66 2c20 6466  Bullish(self, df
-000231d0: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
-000231e0: 7665 4469 6374 293a 0a20 2020 2020 2020  veDict):.       
-000231f0: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-00023200: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
-00023210: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00023220: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-00023230: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-00023240: 290a 2020 2020 2020 2020 2320 6874 7470  ).        # http
-00023250: 733a 2f2f 6368 6172 7469 6e6b 2e63 6f6d  s://chartink.com
-00023260: 2f73 6372 6565 6e65 722f 7368 6f72 742d  /screener/short-
-00023270: 7465 726d 2d62 756c 6c69 7368 0a20 2020  term-bullish.   
-00023280: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-00023290: 2e66 696c 6c6e 6128 3029 0a20 2020 2020  .fillna(0).     
-000232a0: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
-000232b0: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
-000232c0: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
-000232d0: 2020 2020 2072 6563 656e 7420 3d20 6461       recent = da
-000232e0: 7461 2e68 6561 6428 3129 0a20 2020 2020  ta.head(1).     
-000232f0: 2020 2066 6b20 3d20 3020 6966 206c 656e     fk = 0 if len
-00023300: 2864 6174 6129 203c 2033 2065 6c73 6520  (data) < 3 else 
-00023310: 6e70 2e72 6f75 6e64 2864 6174 615b 2246  np.round(data["F
-00023320: 4153 544b 225d 2e69 6c6f 635b 325d 2c20  ASTK"].iloc[2], 
-00023330: 3529 0a20 2020 2020 2020 2023 2052 6576  5).        # Rev
-00023340: 6572 7365 2074 6865 2064 6174 6166 7261  erse the datafra
-00023350: 6d65 2066 6f72 2069 6368 696d 6f6b 7520  me for ichimoku 
-00023360: 6361 6c63 756c 6174 696f 6e73 2077 6974  calculations wit
-00023370: 6820 6461 7465 2069 6e20 6173 6365 6e64  h date in ascend
-00023380: 696e 6720 6f72 6465 720a 2020 2020 2020  ing order.      
-00023390: 2020 6466 5f6e 6577 203d 2064 6174 615b    df_new = data[
-000233a0: 3a3a 2d31 5d0a 2020 2020 2020 2020 7472  ::-1].        tr
-000233b0: 793a 0a20 2020 2020 2020 2020 2020 2064  y:.            d
-000233c0: 665f 6963 6869 203d 2064 665f 6e65 772e  f_ichi = df_new.
-000233d0: 7265 6e61 6d65 280a 2020 2020 2020 2020  rename(.        
-000233e0: 2020 2020 2020 2020 636f 6c75 6d6e 733d          columns=
-000233f0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00023400: 2020 2020 2020 224f 7065 6e22 3a20 226f        "Open": "o
-00023410: 7065 6e22 2c0a 2020 2020 2020 2020 2020  pen",.          
-00023420: 2020 2020 2020 2020 2020 2248 6967 6822            "High"
-00023430: 3a20 2268 6967 6822 2c0a 2020 2020 2020  : "high",.      
-00023440: 2020 2020 2020 2020 2020 2020 2020 224c                "L
-00023450: 6f77 223a 2022 6c6f 7722 2c0a 2020 2020  ow": "low",.    
-00023460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023470: 2243 6c6f 7365 223a 2022 636c 6f73 6522  "Close": "close"
-00023480: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00023490: 2020 2020 2020 2256 6f6c 756d 6522 3a20        "Volume": 
-000234a0: 2276 6f6c 756d 6522 2c0a 2020 2020 2020  "volume",.      
-000234b0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-000234c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000234d0: 2020 2020 2020 6963 6869 203d 2070 6b74        ichi = pkt
-000234e0: 616c 6962 2e69 6368 696d 6f6b 7528 6466  alib.ichimoku(df
-000234f0: 5f69 6368 692c 2039 2c20 3236 2c20 3532  _ichi, 9, 26, 52
-00023500: 2c20 3236 290a 2020 2020 2020 2020 2020  , 26).          
-00023510: 2020 6966 2069 6368 6920 6973 204e 6f6e    if ichi is Non
-00023520: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00023530: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00023540: 2020 2020 2020 2020 2020 2020 6466 5f6e              df_n
-00023550: 6577 203d 2070 642e 636f 6e63 6174 285b  ew = pd.concat([
-00023560: 6466 5f6e 6577 2c20 6963 6869 5d2c 2061  df_new, ichi], a
-00023570: 7869 733d 3129 0a20 2020 2020 2020 2020  xis=1).         
-00023580: 2020 2023 2052 6576 6572 7365 2061 6761     # Reverse aga
-00023590: 696e 2074 6f20 6765 7420 7468 6520 6d6f  in to get the mo
-000235a0: 7374 2072 6563 656e 7420 6461 7465 206f  st recent date o
-000235b0: 6e20 746f 700a 2020 2020 2020 2020 2020  n top.          
-000235c0: 2020 6466 5f6e 6577 203d 2064 665f 6e65    df_new = df_ne
-000235d0: 775b 3a3a 2d31 5d0a 2020 2020 2020 2020  w[::-1].        
-000235e0: 2020 2020 6466 5f6e 6577 203d 2064 665f      df_new = df_
-000235f0: 6e65 772e 6865 6164 2831 290a 2020 2020  new.head(1).    
-00023600: 2020 2020 2020 2020 6466 5f6e 6577 5b22          df_new["
-00023610: 636c 6f75 645f 6772 6565 6e22 5d20 3d20  cloud_green"] = 
-00023620: 6466 5f6e 6577 5b22 4953 415f 3922 5d2e  df_new["ISA_9"].
-00023630: 696c 6f63 5b30 5d20 3e20 6466 5f6e 6577  iloc[0] > df_new
-00023640: 5b22 4953 425f 3236 225d 2e69 6c6f 635b  ["ISB_26"].iloc[
-00023650: 305d 0a20 2020 2020 2020 2020 2020 2064  0].            d
-00023660: 665f 6e65 775b 2263 6c6f 7564 5f72 6564  f_new["cloud_red
-00023670: 225d 203d 2064 665f 6e65 775b 2249 5342  "] = df_new["ISB
-00023680: 5f32 3622 5d2e 696c 6f63 5b30 5d20 3e20  _26"].iloc[0] > 
-00023690: 6466 5f6e 6577 5b22 4953 415f 3922 5d2e  df_new["ISA_9"].
-000236a0: 696c 6f63 5b30 5d0a 2020 2020 2020 2020  iloc[0].        
-000236b0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-000236c0: 2061 7320 653a 2020 2320 7072 6167 6d61   as e:  # pragma
-000236d0: 3a20 6e6f 2063 6f76 6572 0a20 2020 2020  : no cover.     
-000236e0: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
-000236f0: 756c 745f 6c6f 6767 6572 2e64 6562 7567  ult_logger.debug
-00023700: 2865 2c20 6578 635f 696e 666f 3d54 7275  (e, exc_info=Tru
-00023710: 6529 0a20 2020 2020 2020 2020 2020 2070  e).            p
-00023720: 6173 730a 2020 2020 2020 2020 6162 6f76  ass.        abov
-00023730: 6543 6c6f 7564 546f 7020 3d20 4661 6c73  eCloudTop = Fals
-00023740: 650a 2020 2020 2020 2020 2320 6261 7365  e.        # base
-00023750: 6c69 6e65 203e 2063 6c6f 7564 2074 6f70  line > cloud top
-00023760: 2028 636c 6f75 6420 6973 2062 6f75 6e64   (cloud is bound
-00023770: 2062 7920 7370 616e 2061 2061 6e64 2073   by span a and s
-00023780: 7061 6e20 6229 2061 6e64 2063 6c6f 7365  pan b) and close
-00023790: 2069 7320 3e20 636c 6f75 6420 746f 700a   is > cloud top.
-000237a0: 2020 2020 2020 2020 6966 2064 665f 6e65          if df_ne
-000237b0: 775b 2263 6c6f 7564 5f67 7265 656e 225d  w["cloud_green"]
-000237c0: 2e69 6c6f 635b 305d 3a0a 2020 2020 2020  .iloc[0]:.      
-000237d0: 2020 2020 2020 6162 6f76 6543 6c6f 7564        aboveCloud
-000237e0: 546f 7020 3d20 280a 2020 2020 2020 2020  Top = (.        
-000237f0: 2020 2020 2020 2020 6466 5f6e 6577 5b22          df_new["
-00023800: 494b 535f 3236 225d 2e69 6c6f 635b 305d  IKS_26"].iloc[0]
-00023810: 203e 2064 665f 6e65 775b 2249 5341 5f39   > df_new["ISA_9
-00023820: 225d 2e69 6c6f 635b 305d 0a20 2020 2020  "].iloc[0].     
-00023830: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
-00023840: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
-00023850: 6c6f 635b 305d 203e 2064 665f 6e65 775b  loc[0] > df_new[
-00023860: 2249 5341 5f39 225d 2e69 6c6f 635b 305d  "ISA_9"].iloc[0]
-00023870: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00023880: 2020 2020 2020 2065 6c69 6620 6466 5f6e         elif df_n
-00023890: 6577 5b22 636c 6f75 645f 7265 6422 5d2e  ew["cloud_red"].
-000238a0: 696c 6f63 5b30 5d3a 0a20 2020 2020 2020  iloc[0]:.       
-000238b0: 2020 2020 2061 626f 7665 436c 6f75 6454       aboveCloudT
-000238c0: 6f70 203d 2028 0a20 2020 2020 2020 2020  op = (.         
-000238d0: 2020 2020 2020 2064 665f 6e65 775b 2249         df_new["I
-000238e0: 4b53 5f32 3622 5d2e 696c 6f63 5b30 5d20  KS_26"].iloc[0] 
-000238f0: 3e20 6466 5f6e 6577 5b22 4953 425f 3236  > df_new["ISB_26
-00023900: 225d 2e69 6c6f 635b 305d 0a20 2020 2020  "].iloc[0].     
-00023910: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
-00023920: 6563 656e 745b 2243 6c6f 7365 225d 2e69  ecent["Close"].i
-00023930: 6c6f 635b 305d 203e 2064 665f 6e65 775b  loc[0] > df_new[
-00023940: 2249 5342 5f32 3622 5d2e 696c 6f63 5b30  "ISB_26"].iloc[0
-00023950: 5d0a 2020 2020 2020 2020 2020 2020 290a  ].            ).
-00023960: 0a20 2020 2020 2020 2023 204c 6174 6573  .        # Lates
-00023970: 7420 4963 6869 6d6f 6b75 2062 6173 656c  t Ichimoku basel
-00023980: 696e 6520 6973 203c 206c 6174 6573 7420  ine is < latest 
-00023990: 4963 6869 6d6f 6b75 2063 6f6e 7665 7273  Ichimoku convers
-000239a0: 696f 6e20 6c69 6e65 0a20 2020 2020 2020  ion line.       
-000239b0: 2069 6620 6162 6f76 6543 6c6f 7564 546f   if aboveCloudTo
-000239c0: 7020 616e 6420 6466 5f6e 6577 5b22 494b  p and df_new["IK
-000239d0: 535f 3236 225d 2e69 6c6f 635b 305d 203c  S_26"].iloc[0] <
-000239e0: 2064 665f 6e65 775b 2249 5453 5f39 225d   df_new["ITS_9"]
-000239f0: 2e69 6c6f 635b 305d 3a0a 2020 2020 2020  .iloc[0]:.      
-00023a00: 2020 2020 2020 2320 5374 6f63 6852 5349        # StochRSI
-00023a10: 2063 726f 7373 6564 2032 3020 616e 6420   crossed 20 and 
-00023a20: 5253 4920 3e20 3530 0a20 2020 2020 2020  RSI > 50.       
-00023a30: 2020 2020 2069 6620 666b 203e 2032 3020       if fk > 20 
-00023a40: 616e 6420 7265 6365 6e74 5b22 5253 4922  and recent["RSI"
-00023a50: 5d2e 696c 6f63 5b30 5d20 3e20 3530 3a0a  ].iloc[0] > 50:.
-00023a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023a70: 2320 636f 6e64 6974 696f 6e20 6f66 2063  # condition of c
-00023a80: 726f 7373 696e 6720 7468 6520 5374 6f63  rossing the Stoc
-00023a90: 6852 5349 206d 6169 6e20 7369 676e 616c  hRSI main signal
-00023aa0: 206c 696e 6520 6672 6f6d 2062 6f74 746f   line from botto
-00023ab0: 6d20 746f 2074 6f70 0a20 2020 2020 2020  m to top.       
-00023ac0: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
-00023ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023ae0: 2020 6461 7461 5b22 4641 5354 4422 5d2e    data["FASTD"].
-00023af0: 696c 6f63 5b31 3030 5d20 3c20 6461 7461  iloc[100] < data
-00023b00: 5b22 4641 5354 4b22 5d2e 696c 6f63 5b31  ["FASTK"].iloc[1
-00023b10: 3030 5d0a 2020 2020 2020 2020 2020 2020  00].            
-00023b20: 2020 2020 2020 2020 616e 6420 6461 7461          and data
-00023b30: 5b22 4641 5354 4422 5d2e 696c 6f63 5b31  ["FASTD"].iloc[1
-00023b40: 3031 5d20 3e20 6461 7461 5b22 4641 5354  01] > data["FAST
-00023b50: 4b22 5d2e 696c 6f63 5b31 3031 5d0a 2020  K"].iloc[101].  
-00023b60: 2020 2020 2020 2020 2020 2020 2020 293a                ):
-00023b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023b80: 2020 2020 2023 2063 6c6f 7365 203e 2035       # close > 5
-00023b90: 3020 7065 7269 6f64 2053 4d41 2f45 4d41  0 period SMA/EMA
-00023ba0: 2061 6e64 2032 3030 2070 6572 696f 6420   and 200 period 
-00023bb0: 534d 412f 454d 410a 2020 2020 2020 2020  SMA/EMA.        
-00023bc0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00023bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023be0: 2020 2020 2020 2020 2072 6563 656e 745b           recent[
-00023bf0: 2253 534d 4122 5d2e 696c 6f63 5b30 5d20  "SSMA"].iloc[0] 
-00023c00: 3e20 7265 6365 6e74 5b22 534d 4122 5d2e  > recent["SMA"].
-00023c10: 696c 6f63 5b30 5d0a 2020 2020 2020 2020  iloc[0].        
-00023c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023c30: 616e 6420 7265 6365 6e74 5b22 436c 6f73  and recent["Clos
-00023c40: 6522 5d2e 696c 6f63 5b30 5d20 3e20 7265  e"].iloc[0] > re
-00023c50: 6365 6e74 5b22 5353 4d41 225d 2e69 6c6f  cent["SSMA"].ilo
-00023c60: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
-00023c70: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00023c80: 2072 6563 656e 745b 2243 6c6f 7365 225d   recent["Close"]
-00023c90: 2e69 6c6f 635b 305d 203e 2072 6563 656e  .iloc[0] > recen
-00023ca0: 745b 224c 4d41 225d 2e69 6c6f 635b 305d  t["LMA"].iloc[0]
-00023cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00023cc0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-00023cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023ce0: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
-00023cf0: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
-00023d00: 7565 2873 6372 6565 6e44 6963 742c 7361  ue(screenDict,sa
-00023d10: 7665 4469 6374 2c22 4d41 2d53 6967 6e61  veDict,"MA-Signa
-00023d20: 6c22 290a 2020 2020 2020 2020 2020 2020  l").            
-00023d30: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-00023d40: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
-00023d50: 6c22 5d20 3d20 280a 2020 2020 2020 2020  l"] = (.        
-00023d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023d70: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
-00023d80: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
-00023d90: 636f 6c6f 7254 6578 742e 4752 4545 4e20  colorText.GREEN 
-00023da0: 2b20 2242 756c 6c69 7368 2220 2b20 636f  + "Bullish" + co
-00023db0: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
-00023dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023dd0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00023de0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00023df0: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
-00023e00: 6c22 5d20 3d20 7361 7665 645b 315d 202b  l"] = saved[1] +
-00023e10: 2022 4275 6c6c 6973 6822 0a20 2020 2020   "Bullish".     
-00023e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023e30: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00023e40: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00023e50: 6c73 650a 0a20 2020 2023 2056 616c 6964  lse..    # Valid
-00023e60: 6174 6520 5650 430a 2020 2020 6465 6620  ate VPC.    def 
-00023e70: 7661 6c69 6461 7465 5643 5028 0a20 2020  validateVCP(.   
-00023e80: 2020 2020 2073 656c 662c 2064 662c 2073       self, df, s
-00023e90: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-00023ea0: 6963 742c 2073 746f 636b 4e61 6d65 3d4e  ict, stockName=N
-00023eb0: 6f6e 652c 2077 696e 646f 773d 332c 2070  one, window=3, p
-00023ec0: 6572 6365 6e74 6167 6546 726f 6d54 6f70  ercentageFromTop
-00023ed0: 3d33 0a20 2020 2029 3a0a 2020 2020 2020  =3.    ):.      
-00023ee0: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
-00023ef0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
-00023f00: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00023f10: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-00023f20: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
-00023f30: 2829 0a20 2020 2020 2020 2074 7279 3a0a  ().        try:.
-00023f40: 2020 2020 2020 2020 2020 2020 7065 7263              perc
-00023f50: 656e 7461 6765 4672 6f6d 546f 7020 2f3d  entageFromTop /=
-00023f60: 2031 3030 0a20 2020 2020 2020 2020 2020   100.           
-00023f70: 2064 6174 612e 7265 7365 745f 696e 6465   data.reset_inde
-00023f80: 7828 696e 706c 6163 653d 5472 7565 290a  x(inplace=True).
-00023f90: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00023fa0: 2e72 656e 616d 6528 636f 6c75 6d6e 733d  .rename(columns=
-00023fb0: 7b22 696e 6465 7822 3a20 2244 6174 6522  {"index": "Date"
-00023fc0: 7d2c 2069 6e70 6c61 6365 3d54 7275 6529  }, inplace=True)
-00023fd0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00023fe0: 615b 2274 6f70 7322 5d20 3d20 280a 2020  a["tops"] = (.  
-00023ff0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00024000: 7461 5b22 4869 6768 225d 0a20 2020 2020  ta["High"].     
-00024010: 2020 2020 2020 2020 2020 202e 696c 6f63             .iloc
-00024020: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00024030: 2020 2020 2020 6c69 7374 280a 2020 2020        list(.    
-00024040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024050: 2020 2020 706b 7461 6c69 622e 6172 6772      pktalib.argr
-00024060: 656c 6578 7472 656d 6128 0a20 2020 2020  elextrema(.     
-00024070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024080: 2020 2020 2020 206e 702e 6172 7261 7928         np.array(
-00024090: 6461 7461 5b22 4869 6768 225d 292c 206e  data["High"]), n
-000240a0: 702e 6772 6561 7465 725f 6571 7561 6c2c  p.greater_equal,
-000240b0: 206f 7264 6572 3d77 696e 646f 770a 2020   order=window.  
-000240c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000240d0: 2020 2020 2020 295b 305d 0a20 2020 2020        )[0].     
-000240e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000240f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024100: 205d 0a20 2020 2020 2020 2020 2020 2020   ].             
-00024110: 2020 202e 6865 6164 2834 290a 2020 2020     .head(4).    
-00024120: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00024130: 2020 2020 2020 6461 7461 5b22 626f 7473        data["bots
-00024140: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
-00024150: 2020 2020 2020 2064 6174 615b 224c 6f77         data["Low
-00024160: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-00024170: 2020 202e 696c 6f63 5b0a 2020 2020 2020     .iloc[.      
-00024180: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-00024190: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
-000241a0: 2020 2020 2020 2020 2020 2020 706b 7461              pkta
-000241b0: 6c69 622e 6172 6772 656c 6578 7472 656d  lib.argrelextrem
-000241c0: 6128 0a20 2020 2020 2020 2020 2020 2020  a(.             
-000241d0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000241e0: 702e 6172 7261 7928 6461 7461 5b22 4c6f  p.array(data["Lo
-000241f0: 7722 5d29 2c20 6e70 2e6c 6573 735f 6571  w"]), np.less_eq
-00024200: 7561 6c2c 206f 7264 6572 3d77 696e 646f  ual, order=windo
-00024210: 770a 2020 2020 2020 2020 2020 2020 2020  w.              
-00024220: 2020 2020 2020 2020 2020 295b 305d 0a20            )[0]. 
-00024230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024240: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00024250: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
-00024260: 2020 2020 2020 202e 6865 6164 2834 290a         .head(4).
-00024270: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00024280: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00024290: 2064 6174 612e 6669 6c6c 6e61 2830 290a   data.fillna(0).
-000242a0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000242b0: 203d 2064 6174 612e 7265 706c 6163 6528   = data.replace(
-000242c0: 5b6e 702e 696e 662c 202d 6e70 2e69 6e66  [np.inf, -np.inf
-000242d0: 5d2c 2030 290a 2020 2020 2020 2020 2020  ], 0).          
-000242e0: 2020 746f 7073 203d 2064 6174 615b 6461    tops = data[da
-000242f0: 7461 2e74 6f70 7320 3e20 305d 0a20 2020  ta.tops > 0].   
-00024300: 2020 2020 2020 2020 2023 2062 6f74 7320           # bots 
-00024310: 3d20 6461 7461 5b64 6174 612e 626f 7473  = data[data.bots
-00024320: 203e 2030 5d0a 2020 2020 2020 2020 2020   > 0].          
-00024330: 2020 6869 6768 6573 7454 6f70 203d 2072    highestTop = r
-00024340: 6f75 6e64 2874 6f70 732e 6465 7363 7269  ound(tops.descri
-00024350: 6265 2829 5b22 4869 6768 225d 5b22 6d61  be()["High"]["ma
-00024360: 7822 5d2c 2031 290a 2020 2020 2020 2020  x"], 1).        
-00024370: 2020 2020 6669 6c74 6572 6564 546f 7073      filteredTops
-00024380: 203d 2074 6f70 735b 0a20 2020 2020 2020   = tops[.       
-00024390: 2020 2020 2020 2020 2074 6f70 732e 746f           tops.to
-000243a0: 7073 203e 2028 6869 6768 6573 7454 6f70  ps > (highestTop
-000243b0: 202d 2028 6869 6768 6573 7454 6f70 202a   - (highestTop *
-000243c0: 2070 6572 6365 6e74 6167 6546 726f 6d54   percentageFromT
-000243d0: 6f70 2929 0a20 2020 2020 2020 2020 2020  op)).           
-000243e0: 205d 0a20 2020 2020 2020 2020 2020 2069   ].            i
-000243f0: 6620 6669 6c74 6572 6564 546f 7073 2e65  f filteredTops.e
-00024400: 7175 616c 7328 746f 7073 293a 2020 2320  quals(tops):  # 
-00024410: 546f 7073 2061 7265 2069 6e20 7468 6520  Tops are in the 
-00024420: 7261 6e67 650a 2020 2020 2020 2020 2020  range.          
-00024430: 2020 2020 2020 6c6f 7750 6f69 6e74 7320        lowPoints 
-00024440: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
-00024450: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00024460: 6e67 6528 6c65 6e28 746f 7073 2920 2d20  nge(len(tops) - 
-00024470: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-00024480: 2020 2020 2020 2020 656e 6444 6174 6520          endDate 
-00024490: 3d20 746f 7073 2e69 6c6f 635b 695d 5b22  = tops.iloc[i]["
-000244a0: 4461 7465 225d 0a20 2020 2020 2020 2020  Date"].         
-000244b0: 2020 2020 2020 2020 2020 2073 7461 7274             start
-000244c0: 4461 7465 203d 2074 6f70 732e 696c 6f63  Date = tops.iloc
-000244d0: 5b69 202b 2031 5d5b 2244 6174 6522 5d0a  [i + 1]["Date"].
-000244e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000244f0: 2020 2020 6c6f 7750 6f69 6e74 732e 6170      lowPoints.ap
-00024500: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
-00024510: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00024520: 7461 5b0a 2020 2020 2020 2020 2020 2020  ta[.            
-00024530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024540: 2864 6174 612e 4461 7465 203e 3d20 7374  (data.Date >= st
-00024550: 6172 7444 6174 6529 2026 2028 6461 7461  artDate) & (data
-00024560: 2e44 6174 6520 3c3d 2065 6e64 4461 7465  .Date <= endDate
-00024570: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00024580: 2020 2020 2020 2020 2020 5d2e 6465 7363            ].desc
-00024590: 7269 6265 2829 5b22 4c6f 7722 5d5b 226d  ribe()["Low"]["m
-000245a0: 696e 225d 0a20 2020 2020 2020 2020 2020  in"].           
-000245b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000245c0: 2020 2020 2020 2020 2020 206c 6f77 506f             lowPo
-000245d0: 696e 7473 4f72 6720 3d20 6c6f 7750 6f69  intsOrg = lowPoi
-000245e0: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-000245f0: 2020 2020 6c6f 7750 6f69 6e74 732e 736f      lowPoints.so
-00024600: 7274 2872 6576 6572 7365 3d54 7275 6529  rt(reverse=True)
-00024610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024620: 206c 6f77 506f 696e 7473 536f 7274 6564   lowPointsSorted
-00024630: 203d 206c 6f77 506f 696e 7473 0a20 2020   = lowPoints.   
-00024640: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00024650: 6461 7461 2e65 6d70 7479 206f 7220 6c65  data.empty or le
-00024660: 6e28 6c6f 7750 6f69 6e74 7329 203c 2031  n(lowPoints) < 1
-00024670: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00024680: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00024690: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-000246a0: 2020 206c 7470 203d 2064 6174 612e 6865     ltp = data.he
-000246b0: 6164 2831 295b 2243 6c6f 7365 225d 2e69  ad(1)["Close"].i
-000246c0: 6c6f 635b 305d 0a20 2020 2020 2020 2020  loc[0].         
-000246d0: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-000246e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000246f0: 6c6f 7750 6f69 6e74 734f 7267 203d 3d20  lowPointsOrg == 
-00024700: 6c6f 7750 6f69 6e74 7353 6f72 7465 640a  lowPointsSorted.
-00024710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024720: 2020 2020 616e 6420 6c74 7020 3c20 6869      and ltp < hi
-00024730: 6768 6573 7454 6f70 0a20 2020 2020 2020  ghestTop.       
-00024740: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00024750: 206c 7470 203e 206c 6f77 506f 696e 7473   ltp > lowPoints
-00024760: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00024770: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00024780: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-00024790: 203d 2073 656c 662e 6669 6e64 4375 7272   = self.findCurr
-000247a0: 656e 7453 6176 6564 5661 6c75 6528 7363  entSavedValue(sc
-000247b0: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
-000247c0: 6374 2c20 2250 6174 7465 726e 2229 0a20  ct, "Pattern"). 
-000247d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000247e0: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
-000247f0: 6174 7465 726e 225d 203d 2028 0a20 2020  attern"] = (.   
-00024800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024810: 2020 2020 2073 6176 6564 5b30 5d20 0a20       saved[0] . 
-00024820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024830: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-00024840: 7874 2e42 4f4c 440a 2020 2020 2020 2020  xt.BOLD.        
-00024850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024860: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
-00024870: 4e0a 2020 2020 2020 2020 2020 2020 2020  N.              
-00024880: 2020 2020 2020 2020 2020 2b20 6622 5643            + f"VC
-00024890: 5020 2842 4f3a 207b 6869 6768 6573 7454  P (BO: {highestT
-000248a0: 6f70 7d29 220a 2020 2020 2020 2020 2020  op})".          
-000248b0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000248c0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-000248d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000248e0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000248f0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-00024900: 5b22 5061 7474 6572 6e22 5d20 3d20 7361  ["Pattern"] = sa
-00024910: 7665 645b 315d 202b 2066 2256 4350 2028  ved[1] + f"VCP (
-00024920: 424f 3a20 7b68 6967 6865 7374 546f 707d  BO: {highestTop}
-00024930: 2922 0a20 2020 2020 2020 2020 2020 2020  )".             
-00024940: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00024950: 7565 0a20 2020 2020 2020 2065 7863 6570  ue.        excep
-00024960: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00024970: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
-00024980: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
-00024990: 2020 7365 6c66 2e64 6566 6175 6c74 5f6c    self.default_l
-000249a0: 6f67 6765 722e 6465 6275 6728 652c 2065  ogger.debug(e, e
-000249b0: 7863 5f69 6e66 6f3d 5472 7565 290a 2020  xc_info=True).  
-000249c0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-000249d0: 7365 0a0a 2020 2020 2320 5661 6c69 6461  se..    # Valida
-000249e0: 7465 2069 6620 766f 6c75 6d65 206f 6620  te if volume of 
-000249f0: 6c61 7374 2064 6179 2069 7320 6869 6768  last day is high
-00024a00: 6572 2074 6861 6e20 6176 670a 2020 2020  er than avg.    
-00024a10: 6465 6620 7661 6c69 6461 7465 566f 6c75  def validateVolu
-00024a20: 6d65 280a 2020 2020 2020 2020 7365 6c66  me(.        self
-00024a30: 2c20 6466 2c20 7363 7265 656e 4469 6374  , df, screenDict
-00024a40: 2c20 7361 7665 4469 6374 2c20 766f 6c75  , saveDict, volu
-00024a50: 6d65 5261 7469 6f3d 322e 352c 206d 696e  meRatio=2.5, min
-00024a60: 566f 6c75 6d65 3d31 3030 0a20 2020 2029  Volume=100.    )
-00024a70: 3a0a 2020 2020 2020 2020 6966 2064 6620  :.        if df 
-00024a80: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
-00024a90: 6629 203d 3d20 303a 0a20 2020 2020 2020  f) == 0:.       
-00024aa0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00024ab0: 652c 2046 616c 7365 0a20 2020 2020 2020  e, False.       
-00024ac0: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-00024ad0: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
-00024ae0: 2064 6174 612e 6669 6c6c 6e61 2830 290a   data.fillna(0).
-00024af0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00024b00: 6174 612e 7265 706c 6163 6528 5b6e 702e  ata.replace([np.
-00024b10: 696e 662c 202d 6e70 2e69 6e66 5d2c 2030  inf, -np.inf], 0
-00024b20: 290a 2020 2020 2020 2020 7265 6365 6e74  ).        recent
-00024b30: 203d 2064 6174 612e 6865 6164 2831 290a   = data.head(1).
-00024b40: 2020 2020 2020 2020 2320 4569 7468 6572          # Either
-00024b50: 2074 6865 2072 6f6c 6c69 6e67 2076 6f6c   the rolling vol
-00024b60: 756d 6520 6f66 2070 6173 7420 3230 2073  ume of past 20 s
-00024b70: 6573 7369 6f6e 7320 6f72 2074 6f64 6179  essions or today
-00024b80: 2773 2076 6f6c 756d 6520 7368 6f75 6c64  's volume should
-00024b90: 2062 6520 3e20 6d69 6e20 766f 6c75 6d65   be > min volume
-00024ba0: 0a20 2020 2020 2020 2068 6173 4d69 6e69  .        hasMini
-00024bb0: 6d75 6d56 6f6c 756d 6520 3d20 280a 2020  mumVolume = (.  
-00024bc0: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
-00024bd0: 5b22 566f 6c4d 4122 5d2e 696c 6f63 5b30  ["VolMA"].iloc[0
-00024be0: 5d20 3e3d 206d 696e 566f 6c75 6d65 0a20  ] >= minVolume. 
-00024bf0: 2020 2020 2020 2020 2020 206f 7220 7265             or re
-00024c00: 6365 6e74 5b22 566f 6c75 6d65 225d 2e69  cent["Volume"].i
-00024c10: 6c6f 635b 305d 203e 3d20 6d69 6e56 6f6c  loc[0] >= minVol
-00024c20: 756d 650a 2020 2020 2020 2020 290a 2020  ume.        ).  
-00024c30: 2020 2020 2020 6966 2072 6563 656e 745b        if recent[
-00024c40: 2256 6f6c 4d41 225d 2e69 6c6f 635b 305d  "VolMA"].iloc[0]
-00024c50: 203d 3d20 303a 2020 2320 4861 6e64 6c65   == 0:  # Handle
-00024c60: 7320 4469 7669 6465 2062 7920 3020 7761  s Divide by 0 wa
-00024c70: 726e 696e 670a 2020 2020 2020 2020 2020  rning.          
-00024c80: 2020 7361 7665 4469 6374 5b22 566f 6c75    saveDict["Volu
-00024c90: 6d65 225d 203d 2030 2020 2320 2255 6e6b  me"] = 0  # "Unk
-00024ca0: 6e6f 776e 220a 2020 2020 2020 2020 2020  nown".          
-00024cb0: 2020 7363 7265 656e 4469 6374 5b22 566f    screenDict["Vo
-00024cc0: 6c75 6d65 225d 203d 2030 0a20 2020 2020  lume"] = 0.     
-00024cd0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00024ce0: 6c73 652c 2068 6173 4d69 6e69 6d75 6d56  lse, hasMinimumV
-00024cf0: 6f6c 756d 650a 2020 2020 2020 2020 7261  olume.        ra
-00024d00: 7469 6f20 3d20 726f 756e 6428 7265 6365  tio = round(rece
-00024d10: 6e74 5b22 566f 6c75 6d65 225d 2e69 6c6f  nt["Volume"].ilo
-00024d20: 635b 305d 202f 2072 6563 656e 745b 2256  c[0] / recent["V
-00024d30: 6f6c 4d41 225d 2e69 6c6f 635b 305d 2c20  olMA"].iloc[0], 
-00024d40: 3229 0a20 2020 2020 2020 2073 6176 6544  2).        saveD
-00024d50: 6963 745b 2256 6f6c 756d 6522 5d20 3d20  ict["Volume"] = 
-00024d60: 7261 7469 6f0a 2020 2020 2020 2020 6966  ratio.        if
-00024d70: 2072 6174 696f 203e 3d20 766f 6c75 6d65   ratio >= volume
-00024d80: 5261 7469 6f20 616e 6420 7261 7469 6f20  Ratio and ratio 
-00024d90: 213d 206e 702e 6e61 6e20 616e 6420 286e  != np.nan and (n
-00024da0: 6f74 206d 6174 682e 6973 696e 6628 7261  ot math.isinf(ra
-00024db0: 7469 6f29 293a 0a20 2020 2020 2020 2020  tio)):.         
-00024dc0: 2020 2073 6372 6565 6e44 6963 745b 2256     screenDict["V
-00024dd0: 6f6c 756d 6522 5d20 3d20 7261 7469 6f0a  olume"] = ratio.
-00024de0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00024df0: 726e 2054 7275 652c 2068 6173 4d69 6e69  rn True, hasMini
-00024e00: 6d75 6d56 6f6c 756d 650a 2020 2020 2020  mumVolume.      
-00024e10: 2020 7363 7265 656e 4469 6374 5b22 566f    screenDict["Vo
-00024e20: 6c75 6d65 225d 203d 2072 6174 696f 0a20  lume"] = ratio. 
-00024e30: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00024e40: 6c73 652c 2068 6173 4d69 6e69 6d75 6d56  lse, hasMinimumV
-00024e50: 6f6c 756d 650a 0a20 2020 2023 2046 696e  olume..    # Fin
-00024e60: 6420 6966 2073 746f 636b 2069 7320 7661  d if stock is va
-00024e70: 6c69 6461 7469 6e67 2076 6f6c 756d 6520  lidating volume 
-00024e80: 7370 7265 6164 2061 6e61 6c79 7369 730a  spread analysis.
-00024e90: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00024ea0: 566f 6c75 6d65 5370 7265 6164 416e 616c  VolumeSpreadAnal
-00024eb0: 7973 6973 2873 656c 662c 2064 662c 2073  ysis(self, df, s
-00024ec0: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-00024ed0: 6963 7429 3a0a 2020 2020 2020 2020 7472  ict):.        tr
-00024ee0: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
-00024ef0: 6620 6466 2069 7320 4e6f 6e65 206f 7220  f df is None or 
-00024f00: 6c65 6e28 6466 2920 3d3d 2030 3a0a 2020  len(df) == 0:.  
-00024f10: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00024f20: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-00024f30: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
-00024f40: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
-00024f50: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
-00024f60: 6865 6164 2832 290a 2020 2020 2020 2020  head(2).        
-00024f70: 2020 2020 6966 206c 656e 2864 6174 6129      if len(data)
-00024f80: 203c 2032 3a0a 2020 2020 2020 2020 2020   < 2:.          
-00024f90: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00024fa0: 7365 0a20 2020 2020 2020 2020 2020 2074  se.            t
-00024fb0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00024fc0: 2020 2020 2320 4368 6563 6b20 666f 7220      # Check for 
-00024fd0: 7072 6576 696f 7573 2052 4544 2063 616e  previous RED can
-00024fe0: 646c 6573 0a20 2020 2020 2020 2020 2020  dles.           
-00024ff0: 2020 2020 2023 2043 7572 7265 6e74 2063       # Current c
-00025000: 616e 646c 6520 3d20 3074 682c 2050 7265  andle = 0th, Pre
-00025010: 7669 6f75 7320 4361 6e64 6c65 203d 2031  vious Candle = 1
-00025020: 7374 2066 6f72 2066 6f6c 6c6f 7769 6e67  st for following
-00025030: 206c 6f67 6963 0a20 2020 2020 2020 2020   logic.         
-00025040: 2020 2020 2020 2069 6620 6461 7461 2e69         if data.i
-00025050: 6c6f 635b 315d 5b22 4f70 656e 225d 203e  loc[1]["Open"] >
-00025060: 3d20 6461 7461 2e69 6c6f 635b 315d 5b22  = data.iloc[1]["
-00025070: 436c 6f73 6522 5d3a 0a20 2020 2020 2020  Close"]:.       
-00025080: 2020 2020 2020 2020 2020 2020 2073 7072               spr
-00025090: 6561 6431 203d 2061 6273 2864 6174 612e  ead1 = abs(data.
-000250a0: 696c 6f63 5b31 5d5b 224f 7065 6e22 5d20  iloc[1]["Open"] 
-000250b0: 2d20 6461 7461 2e69 6c6f 635b 315d 5b22  - data.iloc[1]["
-000250c0: 436c 6f73 6522 5d29 0a20 2020 2020 2020  Close"]).       
-000250d0: 2020 2020 2020 2020 2020 2020 2073 7072               spr
-000250e0: 6561 6430 203d 2061 6273 2864 6174 612e  ead0 = abs(data.
-000250f0: 696c 6f63 5b30 5d5b 224f 7065 6e22 5d20  iloc[0]["Open"] 
-00025100: 2d20 6461 7461 2e69 6c6f 635b 305d 5b22  - data.iloc[0]["
-00025110: 436c 6f73 6522 5d29 0a20 2020 2020 2020  Close"]).       
-00025120: 2020 2020 2020 2020 2020 2020 206c 6f77               low
-00025130: 6572 5f77 6963 6b5f 7370 7265 6164 3020  er_wick_spread0 
-00025140: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00025150: 2020 2020 2020 2020 2020 2020 6d61 7828              max(
-00025160: 6461 7461 2e69 6c6f 635b 305d 5b22 4f70  data.iloc[0]["Op
-00025170: 656e 225d 2c20 6461 7461 2e69 6c6f 635b  en"], data.iloc[
-00025180: 305d 5b22 436c 6f73 6522 5d29 0a20 2020  0]["Close"]).   
-00025190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000251a0: 2020 2020 202d 2064 6174 612e 696c 6f63       - data.iloc
-000251b0: 5b30 5d5b 224c 6f77 225d 0a20 2020 2020  [0]["Low"].     
-000251c0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000251d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000251e0: 2020 2020 2076 6f6c 3120 3d20 6461 7461       vol1 = data
-000251f0: 2e69 6c6f 635b 315d 5b22 566f 6c75 6d65  .iloc[1]["Volume
-00025200: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-00025210: 2020 2020 2020 2076 6f6c 3020 3d20 6461         vol0 = da
-00025220: 7461 2e69 6c6f 635b 305d 5b22 566f 6c75  ta.iloc[0]["Volu
-00025230: 6d65 225d 0a20 2020 2020 2020 2020 2020  me"].           
-00025240: 2020 2020 2020 2020 2073 6176 6564 203d           saved =
-00025250: 2073 656c 662e 6669 6e64 4375 7272 656e   self.findCurren
-00025260: 7453 6176 6564 5661 6c75 6528 7363 7265  tSavedValue(scre
-00025270: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
-00025280: 2c20 2250 6174 7465 726e 2229 0a20 2020  , "Pattern").   
-00025290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000252a0: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-000252b0: 2020 2020 2020 2020 2020 2020 2020 7370                sp
-000252c0: 7265 6164 3020 3e20 7370 7265 6164 310a  read0 > spread1.
-000252d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000252e0: 2020 2020 2020 2020 616e 6420 766f 6c30          and vol0
-000252f0: 203c 2076 6f6c 310a 2020 2020 2020 2020   < vol1.        
-00025300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025310: 616e 6420 6461 7461 2e69 6c6f 635b 305d  and data.iloc[0]
-00025320: 5b22 566f 6c75 6d65 225d 203c 2064 6174  ["Volume"] < dat
-00025330: 612e 696c 6f63 5b30 5d5b 2256 6f6c 4d41  a.iloc[0]["VolMA
-00025340: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-00025350: 2020 2020 2020 2020 2020 2061 6e64 2064             and d
-00025360: 6174 612e 696c 6f63 5b30 5d5b 2243 6c6f  ata.iloc[0]["Clo
-00025370: 7365 225d 203c 3d20 6461 7461 2e69 6c6f  se"] <= data.ilo
-00025380: 635b 315d 5b22 4f70 656e 225d 0a20 2020  c[1]["Open"].   
-00025390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000253a0: 2020 2020 2061 6e64 2073 7072 6561 6430       and spread0
-000253b0: 203c 206c 6f77 6572 5f77 6963 6b5f 7370   < lower_wick_sp
-000253c0: 7265 6164 300a 2020 2020 2020 2020 2020  read0.          
-000253d0: 2020 2020 2020 2020 2020 2020 2020 616e                an
-000253e0: 6420 6461 7461 2e69 6c6f 635b 305d 5b22  d data.iloc[0]["
-000253f0: 566f 6c75 6d65 225d 203c 3d20 696e 7428  Volume"] <= int(
-00025400: 6461 7461 2e69 6c6f 635b 315d 5b22 566f  data.iloc[1]["Vo
-00025410: 6c75 6d65 225d 202a 2030 2e37 3529 0a20  lume"] * 0.75). 
-00025420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025430: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-00025440: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00025450: 7265 656e 4469 6374 5b22 5061 7474 6572  reenDict["Patter
-00025460: 6e22 5d20 3d20 280a 2020 2020 2020 2020  n"] = (.        
-00025470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025480: 2020 2020 7361 7665 645b 305d 200a 2020      saved[0] .  
-00025490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000254a0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-000254b0: 7254 6578 742e 424f 4c44 0a20 2020 2020  rText.BOLD.     
-000254c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000254d0: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-000254e0: 7874 2e47 5245 454e 0a20 2020 2020 2020  xt.GREEN.       
-000254f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025500: 2020 2020 202b 2022 5375 7070 6c79 2044       + "Supply D
-00025510: 726f 7567 6874 220a 2020 2020 2020 2020  rought".        
-00025520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025530: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-00025540: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
-00025550: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00025560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025570: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-00025580: 5061 7474 6572 6e22 5d20 3d20 7361 7665  Pattern"] = save
-00025590: 645b 315d 202b 2022 5375 7070 6c79 2044  d[1] + "Supply D
-000255a0: 726f 7567 6874 220a 2020 2020 2020 2020  rought".        
-000255b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000255c0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
+000216b0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+000216c0: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
+000216d0: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
+000216e0: 4c44 202b 2063 6f6c 6f72 5465 7874 2e57  LD + colorText.W
+000216f0: 4152 4e20 2b20 224e 6575 7472 616c 2220  ARN + "Neutral" 
+00021700: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+00021710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021720: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00021730: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
+00021740: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
+00021750: 315d 202b 2022 4e65 7574 7261 6c22 0a20  1] + "Neutral". 
+00021760: 2020 2020 2020 2072 6576 6572 7365 6444         reversedD
+00021770: 6174 6120 3d20 6461 7461 5b3a 3a2d 315d  ata = data[::-1]
+00021780: 2020 2320 5265 7665 7273 6520 7468 6520    # Reverse the 
+00021790: 6461 7461 6672 616d 650a 2020 2020 2020  dataframe.      
+000217a0: 2020 656d 615f 3230 203d 2070 6b74 616c    ema_20 = pktal
+000217b0: 6962 2e45 4d41 2872 6576 6572 7365 6444  ib.EMA(reversedD
+000217c0: 6174 615b 2243 6c6f 7365 225d 2c32 3029  ata["Close"],20)
+000217d0: 2e74 6169 6c28 3129 2e69 6c6f 635b 305d  .tail(1).iloc[0]
+000217e0: 0a20 2020 2020 2020 2076 7761 7020 3d20  .        vwap = 
+000217f0: 706b 7461 6c69 622e 5657 4150 2872 6576  pktalib.VWAP(rev
+00021800: 6572 7365 6444 6174 615b 2248 6967 6822  ersedData["High"
+00021810: 5d2c 7265 7665 7273 6564 4461 7461 5b22  ],reversedData["
+00021820: 4c6f 7722 5d2c 7265 7665 7273 6564 4461  Low"],reversedDa
+00021830: 7461 5b22 436c 6f73 6522 5d2c 7265 7665  ta["Close"],reve
+00021840: 7273 6564 4461 7461 5b22 566f 6c75 6d65  rsedData["Volume
+00021850: 225d 292e 7461 696c 2831 292e 696c 6f63  "]).tail(1).iloc
+00021860: 5b30 5d0a 2020 2020 2020 2020 736d 6144  [0].        smaD
+00021870: 6576 203d 2064 6174 615b 2253 4d41 225d  ev = data["SMA"]
+00021880: 2e69 6c6f 635b 305d 202a 206d 6152 616e  .iloc[0] * maRan
+00021890: 6765 202f 2031 3030 0a20 2020 2020 2020  ge / 100.       
+000218a0: 206c 6d61 4465 7620 3d20 6461 7461 5b22   lmaDev = data["
+000218b0: 4c4d 4122 5d2e 696c 6f63 5b30 5d20 2a20  LMA"].iloc[0] * 
+000218c0: 6d61 5261 6e67 6520 2f20 3130 300a 2020  maRange / 100.  
+000218d0: 2020 2020 2020 656d 6144 6576 203d 2065        emaDev = e
+000218e0: 6d61 5f32 3020 2a20 6d61 5261 6e67 6520  ma_20 * maRange 
+000218f0: 2f20 3130 300a 2020 2020 2020 2020 7677  / 100.        vw
+00021900: 6170 4465 7620 3d20 7677 6170 202a 206d  apDev = vwap * m
+00021910: 6152 616e 6765 202f 2031 3030 0a20 2020  aRange / 100.   
+00021920: 2020 2020 206f 7065 6e2c 2068 6967 682c       open, high,
+00021930: 206c 6f77 2c20 636c 6f73 652c 2073 6d61   low, close, sma
+00021940: 2c20 6c6d 6120 3d20 280a 2020 2020 2020  , lma = (.      
+00021950: 2020 2020 2020 6461 7461 5b22 4f70 656e        data["Open
+00021960: 225d 2e69 6c6f 635b 305d 2c0a 2020 2020  "].iloc[0],.    
+00021970: 2020 2020 2020 2020 6461 7461 5b22 4869          data["Hi
+00021980: 6768 225d 2e69 6c6f 635b 305d 2c0a 2020  gh"].iloc[0],.  
+00021990: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
+000219a0: 4c6f 7722 5d2e 696c 6f63 5b30 5d2c 0a20  Low"].iloc[0],. 
+000219b0: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+000219c0: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+000219d0: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+000219e0: 7461 5b22 534d 4122 5d2e 696c 6f63 5b30  ta["SMA"].iloc[0
+000219f0: 5d2c 0a20 2020 2020 2020 2020 2020 2064  ],.            d
+00021a00: 6174 615b 224c 4d41 225d 2e69 6c6f 635b  ata["LMA"].iloc[
+00021a10: 305d 2c0a 2020 2020 2020 2020 290a 2020  0],.        ).  
+00021a20: 2020 2020 2020 6d61 7320 3d20 5b73 6d61        mas = [sma
+00021a30: 2c6c 6d61 2c65 6d61 5f32 302c 7677 6170  ,lma,ema_20,vwap
+00021a40: 5d20 6966 206d 614c 656e 6774 683d 3d30  ] if maLength==0
+00021a50: 2065 6c73 6520 5b73 6d61 2c6c 6d61 2c65   else [sma,lma,e
+00021a60: 6d61 5f32 305d 0a20 2020 2020 2020 206d  ma_20].        m
+00021a70: 6144 6576 7320 3d20 5b73 6d61 4465 762c  aDevs = [smaDev,
+00021a80: 206c 6d61 4465 762c 2065 6d61 4465 762c   lmaDev, emaDev,
+00021a90: 2076 7761 7044 6576 5d20 6966 206d 614c   vwapDev] if maL
+00021aa0: 656e 6774 683d 3d30 2065 6c73 6520 5b73  ength==0 else [s
+00021ab0: 6d61 4465 762c 206c 6d61 4465 762c 2065  maDev, lmaDev, e
+00021ac0: 6d61 4465 765d 0a20 2020 2020 2020 206d  maDev].        m
+00021ad0: 6154 6578 7473 203d 205b 2235 304d 4122  aTexts = ["50MA"
+00021ae0: 2c22 3230 304d 4122 2c22 3230 454d 4122  ,"200MA","20EMA"
+00021af0: 2c22 5657 4150 225d 2069 6620 6d61 4c65  ,"VWAP"] if maLe
+00021b00: 6e67 7468 3d3d 3020 656c 7365 205b 2235  ngth==0 else ["5
+00021b10: 304d 4122 2c22 3230 304d 4122 2c22 3230  0MA","200MA","20
+00021b20: 454d 4122 5d0a 2020 2020 2020 2020 6d61  EMA"].        ma
+00021b30: 5265 7665 7273 616c 203d 2030 0a20 2020  Reversal = 0.   
+00021b40: 2020 2020 2069 6e64 6578 203d 2030 0a20       index = 0. 
+00021b50: 2020 2020 2020 2062 756c 6c69 7368 4361         bullishCa
+00021b60: 6e64 6c65 203d 2073 656c 662e 6765 7443  ndle = self.getC
+00021b70: 616e 646c 6554 7970 6528 6461 7461 290a  andleType(data).
+00021b80: 2020 2020 2020 2020 6966 2073 7472 286d          if str(m
+00021b90: 614c 656e 6774 6829 206e 6f74 2069 6e20  aLength) not in 
+00021ba0: 5b22 3222 2c22 3322 5d3a 0a20 2020 2020  ["2","3"]:.     
+00021bb0: 2020 2020 2020 2066 6f72 206d 6120 696e         for ma in
+00021bc0: 206d 6173 3a0a 2020 2020 2020 2020 2020   mas:.          
+00021bd0: 2020 2020 2020 7361 7665 6420 3d20 7365        saved = se
+00021be0: 6c66 2e66 696e 6443 7572 7265 6e74 5361  lf.findCurrentSa
+00021bf0: 7665 6456 616c 7565 2873 6372 6565 6e44  vedValue(screenD
+00021c00: 6963 742c 7361 7665 4469 6374 2c22 4d41  ict,saveDict,"MA
+00021c10: 2d53 6967 6e61 6c22 290a 2020 2020 2020  -Signal").      
+00021c20: 2020 2020 2020 2020 2020 2320 5461 6b69            # Taki
+00021c30: 6e67 2053 7570 706f 7274 0a20 2020 2020  ng Support.     
+00021c40: 2020 2020 2020 2020 2020 2069 6620 636c             if cl
+00021c50: 6f73 6520 3e20 6d61 2061 6e64 206c 6f77  ose > ma and low
+00021c60: 203c 3d20 286d 6120 2b20 6d61 4465 7673   <= (ma + maDevs
+00021c70: 5b69 6e64 6578 5d29 2061 6e64 2073 7472  [index]) and str
+00021c80: 286d 614c 656e 6774 6829 2069 6e20 5b22  (maLength) in ["
+00021c90: 3022 2c22 3122 5d3a 0a20 2020 2020 2020  0","1"]:.       
+00021ca0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00021cb0: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
+00021cc0: 616c 225d 203d 2028 0a20 2020 2020 2020  al"] = (.       
+00021cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021ce0: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
+00021cf0: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
+00021d00: 6f72 5465 7874 2e47 5245 454e 202b 2066  orText.GREEN + f
+00021d10: 227b 6d61 5465 7874 735b 696e 6465 785d  "{maTexts[index]
+00021d20: 7d2d 5375 7070 6f72 7422 202b 2063 6f6c  }-Support" + col
+00021d30: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
+00021d40: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00021d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021d60: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
+00021d70: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
+00021d80: 6564 5b31 5d20 2b20 6622 7b6d 6154 6578  ed[1] + f"{maTex
+00021d90: 7473 5b69 6e64 6578 5d7d 2d53 7570 706f  ts[index]}-Suppo
+00021da0: 7274 220a 2020 2020 2020 2020 2020 2020  rt".            
+00021db0: 2020 2020 2020 2020 6d61 5265 7665 7273          maRevers
+00021dc0: 616c 203d 2031 0a20 2020 2020 2020 2020  al = 1.         
+00021dd0: 2020 2020 2020 2020 2020 206d 6153 6967             maSig
+00021de0: 6e61 6c73 2e61 7070 656e 6428 2231 2229  nals.append("1")
+00021df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021e00: 2023 2056 616c 6964 6174 696e 6720 5265   # Validating Re
+00021e10: 7369 7374 616e 6365 0a20 2020 2020 2020  sistance.       
+00021e20: 2020 2020 2020 2020 2065 6c69 6620 636c           elif cl
+00021e30: 6f73 6520 3c20 6d61 2061 6e64 2068 6967  ose < ma and hig
+00021e40: 6820 3e3d 2028 6d61 202d 206d 6144 6576  h >= (ma - maDev
+00021e50: 735b 696e 6465 785d 2920 616e 6420 7374  s[index]) and st
+00021e60: 7228 6d61 4c65 6e67 7468 2920 696e 205b  r(maLength) in [
+00021e70: 2230 222c 2236 225d 3a0a 2020 2020 2020  "0","6"]:.      
+00021e80: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00021e90: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
+00021ea0: 6e61 6c22 5d20 3d20 280a 2020 2020 2020  nal"] = (.      
+00021eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021ec0: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
+00021ed0: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
+00021ee0: 6c6f 7254 6578 742e 4641 494c 202b 2066  lorText.FAIL + f
+00021ef0: 227b 6d61 5465 7874 735b 696e 6465 785d  "{maTexts[index]
+00021f00: 7d2d 5265 7369 7374 2220 2b20 636f 6c6f  }-Resist" + colo
+00021f10: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+00021f20: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00021f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021f40: 2020 2020 7361 7665 4469 6374 5b22 4d41      saveDict["MA
+00021f50: 2d53 6967 6e61 6c22 5d20 3d20 7361 7665  -Signal"] = save
+00021f60: 645b 315d 202b 2066 227b 6d61 5465 7874  d[1] + f"{maText
+00021f70: 735b 696e 6465 785d 7d2d 5265 7369 7374  s[index]}-Resist
+00021f80: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00021f90: 2020 2020 2020 6d61 5265 7665 7273 616c        maReversal
+00021fa0: 203d 202d 310a 2020 2020 2020 2020 2020   = -1.          
+00021fb0: 2020 2020 2020 2020 2020 6d61 5369 676e            maSign
+00021fc0: 616c 732e 6170 7065 6e64 2822 3622 290a  als.append("6").
+00021fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021fe0: 2320 466f 7220 6120 4275 6c6c 6973 6820  # For a Bullish 
+00021ff0: 4361 6e64 6c65 0a20 2020 2020 2020 2020  Candle.         
+00022000: 2020 2020 2020 2069 6620 6275 6c6c 6973         if bullis
+00022010: 6843 616e 646c 653a 0a20 2020 2020 2020  hCandle:.       
+00022020: 2020 2020 2020 2020 2020 2020 2023 2043               # C
+00022030: 726f 7373 696e 6720 7570 0a20 2020 2020  rossing up.     
+00022040: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00022050: 6620 6f70 656e 203c 206d 6120 616e 6420  f open < ma and 
+00022060: 636c 6f73 6520 3e20 6d61 2061 6e64 2073  close > ma and s
+00022070: 7472 286d 614c 656e 6774 6829 2069 6e20  tr(maLength) in 
+00022080: 5b22 3022 2c22 3522 5d3a 0a20 2020 2020  ["0","5"]:.     
+00022090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000220a0: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
+000220b0: 412d 5369 676e 616c 225d 203d 2028 0a20  A-Signal"] = (. 
+000220c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000220d0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+000220e0: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
+000220f0: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
+00022100: 2e47 5245 454e 202b 2066 2242 756c 6c43  .GREEN + f"BullC
+00022110: 726f 7373 2d7b 6d61 5465 7874 735b 696e  ross-{maTexts[in
+00022120: 6465 785d 7d22 202b 2063 6f6c 6f72 5465  dex]}" + colorTe
+00022130: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
+00022140: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00022150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022160: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
+00022170: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
+00022180: 2073 6176 6564 5b31 5d20 2b20 6622 4275   saved[1] + f"Bu
+00022190: 6c6c 4372 6f73 732d 7b6d 6154 6578 7473  llCross-{maTexts
+000221a0: 5b69 6e64 6578 5d7d 220a 2020 2020 2020  [index]}".      
+000221b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000221c0: 2020 6d61 5265 7665 7273 616c 203d 2031    maReversal = 1
+000221d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000221e0: 2020 2020 2020 2020 206d 6153 6967 6e61           maSigna
+000221f0: 6c73 2e61 7070 656e 6428 2235 2229 0a20  ls.append("5"). 
+00022200: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00022210: 2046 6f72 2061 2042 6561 7269 7368 2043   For a Bearish C
+00022220: 616e 646c 650a 2020 2020 2020 2020 2020  andle.          
+00022230: 2020 2020 2020 656c 6966 206e 6f74 2062        elif not b
+00022240: 756c 6c69 7368 4361 6e64 6c65 3a0a 2020  ullishCandle:.  
+00022250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022260: 2020 2320 4372 6f73 7369 6e67 2064 6f77    # Crossing dow
+00022270: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00022280: 2020 2020 2020 6966 206f 7065 6e20 3e20        if open > 
+00022290: 736d 6120 616e 6420 636c 6f73 6520 3c20  sma and close < 
+000222a0: 736d 6120 616e 6420 7374 7228 6d61 4c65  sma and str(maLe
+000222b0: 6e67 7468 2920 696e 205b 2230 222c 2234  ngth) in ["0","4
+000222c0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+000222d0: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+000222e0: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
+000222f0: 6c22 5d20 3d20 280a 2020 2020 2020 2020  l"] = (.        
+00022300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022310: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
+00022320: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
+00022330: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
+00022340: 2066 2242 6561 7243 726f 7373 2d7b 6d61   f"BearCross-{ma
+00022350: 5465 7874 735b 696e 6465 785d 7d22 202b  Texts[index]}" +
+00022360: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
+00022370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022380: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00022390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000223a0: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
+000223b0: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
+000223c0: 5d20 2b20 6622 4265 6172 4372 6f73 732d  ] + f"BearCross-
+000223d0: 7b6d 6154 6578 7473 5b69 6e64 6578 5d7d  {maTexts[index]}
+000223e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000223f0: 2020 2020 2020 2020 2020 6d61 5265 7665            maReve
+00022400: 7273 616c 203d 202d 310a 2020 2020 2020  rsal = -1.      
+00022410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022420: 2020 6d61 5369 676e 616c 732e 6170 7065    maSignals.appe
+00022430: 6e64 2822 3422 290a 2020 2020 2020 2020  nd("4").        
+00022440: 2020 2020 2020 2020 696e 6465 7820 2b3d          index +=
+00022450: 2031 0a20 2020 2020 2020 2072 6574 7572   1.        retur
+00022460: 6e56 616c 7565 203d 206d 6152 6576 6572  nValue = maRever
+00022470: 7361 6c0a 2020 2020 2020 2020 6966 206d  sal.        if m
+00022480: 614c 656e 6774 6820 213d 2030 3a0a 2020  aLength != 0:.  
+00022490: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000224a0: 5661 6c75 6520 3d20 7374 7228 6d61 4c65  Value = str(maLe
+000224b0: 6e67 7468 2920 696e 206d 6153 6967 6e61  ngth) in maSigna
+000224c0: 6c73 0a20 2020 2020 2020 2072 6574 7572  ls.        retur
+000224d0: 6e20 7265 7475 726e 5661 6c75 650a 0a20  n returnValue.. 
+000224e0: 2020 2023 2046 696e 6420 4e52 7820 7261     # Find NRx ra
+000224f0: 6e67 6520 666f 7220 5265 7665 7273 616c  nge for Reversal
+00022500: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00022510: 654e 6172 726f 7752 616e 6765 2873 656c  eNarrowRange(sel
+00022520: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+00022530: 742c 2073 6176 6544 6963 742c 206e 723d  t, saveDict, nr=
+00022540: 3429 3a0a 2020 2020 2020 2020 6966 2064  4):.        if d
+00022550: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+00022560: 2864 6629 203d 3d20 303a 0a20 2020 2020  (df) == 0:.     
+00022570: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00022580: 6c73 650a 2020 2020 2020 2020 6461 7461  lse.        data
+00022590: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
+000225a0: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
+000225b0: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
+000225c0: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
+000225d0: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
+000225e0: 6174 7465 726e 2229 0a20 2020 2020 2020  attern").       
+000225f0: 2069 6620 504b 4461 7465 5574 696c 6974   if PKDateUtilit
+00022600: 6965 732e 6973 5472 6164 696e 6754 696d  ies.isTradingTim
+00022610: 6528 293a 0a20 2020 2020 2020 2020 2020  e():.           
+00022620: 2072 616e 6765 4461 7461 203d 2064 6174   rangeData = dat
+00022630: 612e 6865 6164 286e 7220 2b20 3129 5b31  a.head(nr + 1)[1
+00022640: 3a5d 0a20 2020 2020 2020 2020 2020 206e  :].            n
+00022650: 6f77 5f63 616e 646c 6520 3d20 6461 7461  ow_candle = data
+00022660: 2e68 6561 6428 3129 0a20 2020 2020 2020  .head(1).       
+00022670: 2020 2020 2072 616e 6765 4461 7461 5b22       rangeData["
+00022680: 5261 6e67 6522 5d20 3d20 6162 7328 7261  Range"] = abs(ra
+00022690: 6e67 6544 6174 615b 2243 6c6f 7365 225d  ngeData["Close"]
+000226a0: 202d 2072 616e 6765 4461 7461 5b22 4f70   - rangeData["Op
+000226b0: 656e 225d 290a 2020 2020 2020 2020 2020  en"]).          
+000226c0: 2020 7265 6365 6e74 203d 2072 616e 6765    recent = range
+000226d0: 4461 7461 2e68 6561 6428 3129 0a20 2020  Data.head(1).   
+000226e0: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
+000226f0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+00022700: 6e28 7265 6365 6e74 2920 3d3d 2031 0a20  n(recent) == 1. 
+00022710: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00022720: 6e64 2072 6563 656e 745b 2252 616e 6765  nd recent["Range
+00022730: 225d 2e69 6c6f 635b 305d 203d 3d20 7261  "].iloc[0] == ra
+00022740: 6e67 6544 6174 612e 6465 7363 7269 6265  ngeData.describe
+00022750: 2829 5b22 5261 6e67 6522 5d5b 226d 696e  ()["Range"]["min
+00022760: 225d 0a20 2020 2020 2020 2020 2020 2029  "].            )
+00022770: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00022780: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
+00022790: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000227a0: 6765 7443 616e 646c 6554 7970 6528 7265  getCandleType(re
+000227b0: 6365 6e74 290a 2020 2020 2020 2020 2020  cent).          
+000227c0: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
+000227d0: 775f 6361 6e64 6c65 5b22 436c 6f73 6522  w_candle["Close"
+000227e0: 5d2e 696c 6f63 5b30 5d20 3e3d 2072 6563  ].iloc[0] >= rec
+000227f0: 656e 745b 2243 6c6f 7365 225d 2e69 6c6f  ent["Close"].ilo
+00022800: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
+00022810: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+00022820: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+00022830: 656e 4469 6374 5b22 5061 7474 6572 6e22  enDict["Pattern"
+00022840: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
+00022850: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00022860: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
+00022870: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
+00022880: 6578 742e 4752 4545 4e20 2b20 6622 4275  ext.GREEN + f"Bu
+00022890: 792d 4e52 7b6e 727d 2220 2b20 636f 6c6f  y-NR{nr}" + colo
+000228a0: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+000228b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000228c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000228d0: 2020 2020 7361 7665 4469 6374 5b22 5061      saveDict["Pa
+000228e0: 7474 6572 6e22 5d20 3d20 7361 7665 645b  ttern"] = saved[
+000228f0: 315d 202b 2066 2242 7579 2d4e 527b 6e72  1] + f"Buy-NR{nr
+00022900: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+00022910: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00022920: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+00022930: 2020 2065 6c69 6620 280a 2020 2020 2020     elif (.      
+00022940: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00022950: 7420 7365 6c66 2e67 6574 4361 6e64 6c65  t self.getCandle
+00022960: 5479 7065 2872 6563 656e 7429 0a20 2020  Type(recent).   
+00022970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022980: 2061 6e64 206e 6f77 5f63 616e 646c 655b   and now_candle[
+00022990: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+000229a0: 203c 3d20 7265 6365 6e74 5b22 436c 6f73   <= recent["Clos
+000229b0: 6522 5d2e 696c 6f63 5b30 5d0a 2020 2020  e"].iloc[0].    
+000229c0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
+000229d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229e0: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
+000229f0: 6174 7465 726e 225d 203d 2028 0a20 2020  attern"] = (.   
+00022a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a10: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
+00022a20: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
+00022a30: 2063 6f6c 6f72 5465 7874 2e46 4149 4c20   colorText.FAIL 
+00022a40: 2b20 6622 5365 6c6c 2d4e 527b 6e72 7d22  + f"Sell-NR{nr}"
+00022a50: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+00022a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022a70: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00022a80: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+00022a90: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+00022aa0: 2073 6176 6564 5b31 5d20 2b20 6622 5365   saved[1] + f"Se
+00022ab0: 6c6c 2d4e 527b 6e72 7d22 0a20 2020 2020  ll-NR{nr}".     
+00022ac0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00022ad0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00022ae0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00022af0: 6c73 650a 2020 2020 2020 2020 656c 7365  lse.        else
+00022b00: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00022b10: 6e67 6544 6174 6120 3d20 6461 7461 2e68  ngeData = data.h
+00022b20: 6561 6428 6e72 290a 2020 2020 2020 2020  ead(nr).        
+00022b30: 2020 2020 7261 6e67 6544 6174 612e 6c6f      rangeData.lo
+00022b40: 635b 3a2c 2752 616e 6765 275d 203d 2061  c[:,'Range'] = a
+00022b50: 6273 2872 616e 6765 4461 7461 5b22 436c  bs(rangeData["Cl
+00022b60: 6f73 6522 5d20 2d20 7261 6e67 6544 6174  ose"] - rangeDat
+00022b70: 615b 224f 7065 6e22 5d29 0a20 2020 2020  a["Open"]).     
+00022b80: 2020 2020 2020 2072 6563 656e 7420 3d20         recent = 
+00022b90: 7261 6e67 6544 6174 612e 6865 6164 2831  rangeData.head(1
+00022ba0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00022bb0: 2072 6563 656e 745b 2252 616e 6765 225d   recent["Range"]
+00022bc0: 2e69 6c6f 635b 305d 203d 3d20 7261 6e67  .iloc[0] == rang
+00022bd0: 6544 6174 612e 6465 7363 7269 6265 2829  eData.describe()
+00022be0: 5b22 5261 6e67 6522 5d5b 226d 696e 225d  ["Range"]["min"]
+00022bf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00022c00: 2020 7363 7265 656e 4469 6374 5b22 5061    screenDict["Pa
+00022c10: 7474 6572 6e22 5d20 3d20 280a 2020 2020  ttern"] = (.    
+00022c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022c30: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
+00022c40: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
+00022c50: 7254 6578 742e 4752 4545 4e20 2b20 6622  rText.GREEN + f"
+00022c60: 4e52 7b6e 727d 2220 2b20 636f 6c6f 7254  NR{nr}" + colorT
+00022c70: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+00022c80: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00022c90: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+00022ca0: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
+00022cb0: 7361 7665 645b 315d 202b 2066 224e 527b  saved[1] + f"NR{
+00022cc0: 6e72 7d22 0a20 2020 2020 2020 2020 2020  nr}".           
+00022cd0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00022ce0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00022cf0: 7572 6e20 4661 6c73 650a 0a20 2020 2023  urn False..    #
+00022d00: 2046 696e 6420 6966 2073 746f 636b 2069   Find if stock i
+00022d10: 7320 6e65 776c 7920 6c69 7374 6564 0a20  s newly listed. 
+00022d20: 2020 2064 6566 2076 616c 6964 6174 654e     def validateN
+00022d30: 6577 6c79 4c69 7374 6564 2873 656c 662c  ewlyListed(self,
+00022d40: 2064 662c 2064 6179 7354 6f4c 6f6f 6b62   df, daysToLookb
+00022d50: 6163 6b29 3a0a 2020 2020 2020 2020 6966  ack):.        if
+00022d60: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
+00022d70: 656e 2864 6629 203d 3d20 303a 0a20 2020  en(df) == 0:.   
+00022d80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00022d90: 4661 6c73 650a 2020 2020 2020 2020 6461  False.        da
+00022da0: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
+00022db0: 2020 2020 2020 2064 6179 7354 6f4c 6f6f         daysToLoo
+00022dc0: 6b62 6163 6b20 3d20 696e 7428 6461 7973  kback = int(days
+00022dd0: 546f 4c6f 6f6b 6261 636b 5b3a 2d31 5d29  ToLookback[:-1])
+00022de0: 0a20 2020 2020 2020 2072 6563 656e 7420  .        recent 
+00022df0: 3d20 6461 7461 2e68 6561 6428 3129 0a20  = data.head(1). 
+00022e00: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
+00022e10: 6365 6e74 2920 3c20 313a 0a20 2020 2020  cent) < 1:.     
+00022e20: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00022e30: 6c73 650a 2020 2020 2020 2020 6966 206c  lse.        if l
+00022e40: 656e 2864 6174 6129 203c 2064 6179 7354  en(data) < daysT
+00022e50: 6f4c 6f6f 6b62 6163 6b20 616e 6420 280a  oLookback and (.
+00022e60: 2020 2020 2020 2020 2020 2020 7265 6365              rece
+00022e70: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
+00022e80: 5b30 5d20 213d 206e 702e 6e61 6e20 616e  [0] != np.nan an
+00022e90: 6420 7265 6365 6e74 5b22 436c 6f73 6522  d recent["Close"
+00022ea0: 5d2e 696c 6f63 5b30 5d20 3e20 300a 2020  ].iloc[0] > 0.  
+00022eb0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+00022ec0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00022ed0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00022ee0: 4661 6c73 650a 0a20 2020 2023 2056 616c  False..    # Val
+00022ef0: 6964 6174 6520 6966 2074 6865 2073 746f  idate if the sto
+00022f00: 636b 2070 7269 6365 7320 6172 6520 6174  ck prices are at
+00022f10: 206c 6561 7374 2072 6973 696e 6720 6279   least rising by
+00022f20: 2032 2520 666f 7220 7468 6520 6c61 7374   2% for the last
+00022f30: 2033 2073 6573 7369 6f6e 730a 2020 2020   3 sessions.    
+00022f40: 6465 6620 7661 6c69 6461 7465 5072 6963  def validatePric
+00022f50: 6552 6973 696e 6742 7941 744c 6561 7374  eRisingByAtLeast
+00022f60: 3250 6572 6365 6e74 2873 656c 662c 2064  2Percent(self, d
+00022f70: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
+00022f80: 6176 6544 6963 7429 3a0a 2020 2020 2020  aveDict):.      
+00022f90: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
+00022fa0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
+00022fb0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00022fc0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00022fd0: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
+00022fe0: 2829 0a20 2020 2020 2020 2064 6174 6120  ().        data 
+00022ff0: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
+00023000: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00023010: 6461 7461 2e72 6570 6c61 6365 285b 6e70  data.replace([np
+00023020: 2e69 6e66 2c20 2d6e 702e 696e 665d 2c20  .inf, -np.inf], 
+00023030: 3029 0a20 2020 2020 2020 2064 6174 6120  0).        data 
+00023040: 3d20 6461 7461 2e68 6561 6428 3429 0a20  = data.head(4). 
+00023050: 2020 2020 2020 2069 6620 6c65 6e28 6461         if len(da
+00023060: 7461 2920 3c20 343a 0a20 2020 2020 2020  ta) < 4:.       
+00023070: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00023080: 650a 2020 2020 2020 2020 6461 7930 203d  e.        day0 =
+00023090: 2064 6174 612e 696c 6f63 5b30 5d5b 2243   data.iloc[0]["C
+000230a0: 6c6f 7365 225d 2e69 7465 6d28 290a 2020  lose"].item().  
+000230b0: 2020 2020 2020 6461 794d 696e 7573 3120        dayMinus1 
+000230c0: 3d20 6461 7461 2e69 6c6f 635b 315d 5b22  = data.iloc[1]["
+000230d0: 436c 6f73 6522 5d2e 6974 656d 2829 0a20  Close"].item(). 
+000230e0: 2020 2020 2020 2064 6179 4d69 6e75 7332         dayMinus2
+000230f0: 203d 2064 6174 612e 696c 6f63 5b32 5d5b   = data.iloc[2][
+00023100: 2243 6c6f 7365 225d 2e69 7465 6d28 290a  "Close"].item().
+00023110: 2020 2020 2020 2020 6461 794d 696e 7573          dayMinus
+00023120: 3320 3d20 6461 7461 2e69 6c6f 635b 335d  3 = data.iloc[3]
+00023130: 5b22 436c 6f73 6522 5d2e 6974 656d 2829  ["Close"].item()
+00023140: 0a20 2020 2020 2020 2070 6572 6365 6e74  .        percent
+00023150: 3320 3d20 726f 756e 6428 2864 6179 4d69  3 = round((dayMi
+00023160: 6e75 7332 202d 2064 6179 4d69 6e75 7333  nus2 - dayMinus3
+00023170: 2920 2a20 3130 3020 2f20 6461 794d 696e  ) * 100 / dayMin
+00023180: 7573 332c 2032 290a 2020 2020 2020 2020  us3, 2).        
+00023190: 7065 7263 656e 7432 203d 2072 6f75 6e64  percent2 = round
+000231a0: 2828 6461 794d 696e 7573 3120 2d20 6461  ((dayMinus1 - da
+000231b0: 794d 696e 7573 3229 202a 2031 3030 202f  yMinus2) * 100 /
+000231c0: 2064 6179 4d69 6e75 7332 2c20 3229 0a20   dayMinus2, 2). 
+000231d0: 2020 2020 2020 2070 6572 6365 6e74 3120         percent1 
+000231e0: 3d20 726f 756e 6428 2864 6179 3020 2d20  = round((day0 - 
+000231f0: 6461 794d 696e 7573 3129 202a 2031 3030  dayMinus1) * 100
+00023200: 202f 2064 6179 4d69 6e75 7331 2c20 3229   / dayMinus1, 2)
+00023210: 0a0a 2020 2020 2020 2020 6966 2070 6572  ..        if per
+00023220: 6365 6e74 3120 3e3d 2032 2061 6e64 2070  cent1 >= 2 and p
+00023230: 6572 6365 6e74 3220 3e3d 2032 2061 6e64  ercent2 >= 2 and
+00023240: 2070 6572 6365 6e74 3320 3e3d 2032 3a0a   percent3 >= 2:.
+00023250: 2020 2020 2020 2020 2020 2020 7063 745f              pct_
+00023260: 6368 616e 6765 5f74 6578 7420 3d20 280a  change_text = (.
+00023270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023280: 2822 252e 3166 2525 2220 2520 7065 7263  ("%.1f%%" % perc
+00023290: 656e 7431 290a 2020 2020 2020 2020 2020  ent1).          
+000232a0: 2020 2020 2020 2b20 2822 2028 252e 3166        + (" (%.1f
+000232b0: 2525 2c22 2025 2070 6572 6365 6e74 3229  %%," % percent2)
+000232c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000232d0: 202b 2028 2220 252e 3166 2525 2922 2025   + (" %.1f%%)" %
+000232e0: 2070 6572 6365 6e74 3329 0a20 2020 2020   percent3).     
+000232f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00023300: 2020 2020 2073 6176 6544 6963 745b 2225       saveDict["%
+00023310: 4368 6e67 225d 203d 2070 6374 5f63 6861  Chng"] = pct_cha
+00023320: 6e67 655f 7465 7874 0a20 2020 2020 2020  nge_text.       
+00023330: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+00023340: 2225 4368 6e67 225d 203d 2063 6f6c 6f72  "%Chng"] = color
+00023350: 5465 7874 2e47 5245 454e 202b 2070 6374  Text.GREEN + pct
+00023360: 5f63 6861 6e67 655f 7465 7874 202b 2063  _change_text + c
+00023370: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
+00023380: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00023390: 5472 7565 2061 6e64 2073 656c 662e 6765  True and self.ge
+000233a0: 7443 616e 646c 6554 7970 6528 6461 7461  tCandleType(data
+000233b0: 2e68 6561 6428 3129 290a 2020 2020 2020  .head(1)).      
+000233c0: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+000233d0: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
+000233e0: 6d65 0a20 2020 2023 2076 616c 6964 6174  me.    # validat
+000233f0: 6520 6966 2052 5349 2069 7320 7769 7468  e if RSI is with
+00023400: 696e 2067 6976 656e 2072 616e 6765 0a20  in given range. 
+00023410: 2020 2064 6566 2076 616c 6964 6174 6552     def validateR
+00023420: 5349 2873 656c 662c 2064 662c 2073 6372  SI(self, df, scr
+00023430: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+00023440: 742c 206d 696e 5253 492c 206d 6178 5253  t, minRSI, maxRS
+00023450: 492c 7273 694b 6579 3d22 5253 4922 293a  I,rsiKey="RSI"):
+00023460: 0a20 2020 2020 2020 2069 6620 6466 2069  .        if df i
+00023470: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
+00023480: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
+00023490: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000234a0: 0a20 2020 2020 2020 2069 6620 7273 694b  .        if rsiK
+000234b0: 6579 206e 6f74 2069 6e20 6466 2e63 6f6c  ey not in df.col
+000234c0: 756d 6e73 3a0a 2020 2020 2020 2020 2020  umns:.          
+000234d0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+000234e0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
+000234f0: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
+00023500: 6461 7461 203d 2064 6174 612e 6669 6c6c  data = data.fill
+00023510: 6e61 2830 290a 2020 2020 2020 2020 6461  na(0).        da
+00023520: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
+00023530: 6528 5b6e 702e 696e 662c 202d 6e70 2e69  e([np.inf, -np.i
+00023540: 6e66 5d2c 2030 290a 2020 2020 2020 2020  nf], 0).        
+00023550: 7273 6920 3d20 696e 7428 6461 7461 2e68  rsi = int(data.h
+00023560: 6561 6428 3129 5b72 7369 4b65 795d 2e69  ead(1)[rsiKey].i
+00023570: 6c6f 635b 305d 290a 2020 2020 2020 2020  loc[0]).        
+00023580: 7361 7665 4469 6374 5b72 7369 4b65 795d  saveDict[rsiKey]
+00023590: 203d 2072 7369 0a20 2020 2020 2020 2023   = rsi.        #
+000235a0: 2068 7474 7073 3a2f 2f63 6861 7274 696e   https://chartin
+000235b0: 6b2e 636f 6d2f 7363 7265 656e 6572 2f72  k.com/screener/r
+000235c0: 7369 2d73 6372 6565 6e69 6e67 0a20 2020  si-screening.   
+000235d0: 2020 2020 2069 6620 7273 693e 2030 2061       if rsi> 0 a
+000235e0: 6e64 2072 7369 203e 3d20 6d69 6e52 5349  nd rsi >= minRSI
+000235f0: 2061 6e64 2072 7369 203c 3d20 6d61 7852   and rsi <= maxR
+00023600: 5349 3a20 2023 206f 7220 2872 7369 203c  SI:  # or (rsi <
+00023610: 3d20 3731 2061 6e64 2072 7369 203e 3d20  = 71 and rsi >= 
+00023620: 3637 293a 0a20 2020 2020 2020 2020 2020  67):.           
+00023630: 2073 6372 6565 6e44 6963 745b 7273 694b   screenDict[rsiK
+00023640: 6579 5d20 3d20 280a 2020 2020 2020 2020  ey] = (.        
+00023650: 2020 2020 2020 2020 636f 6c6f 7254 6578          colorTex
+00023660: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
+00023670: 7874 2e47 5245 454e 202b 2073 7472 2872  xt.GREEN + str(r
+00023680: 7369 2920 2b20 636f 6c6f 7254 6578 742e  si) + colorText.
+00023690: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
+000236a0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+000236b0: 7475 726e 2054 7275 6520 6966 2028 7273  turn True if (rs
+000236c0: 694b 6579 203d 3d20 2252 5349 6922 2920  iKey == "RSIi") 
+000236d0: 656c 7365 2028 7365 6c66 2e76 616c 6964  else (self.valid
+000236e0: 6174 6552 5349 2864 662c 2073 6372 6565  ateRSI(df, scree
+000236f0: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
+00023700: 206d 696e 5253 492c 206d 6178 5253 492c   minRSI, maxRSI,
+00023710: 7273 694b 6579 3d22 5253 4969 2229 206f  rsiKey="RSIi") o
+00023720: 7220 5472 7565 290a 2020 2020 2020 2020  r True).        
+00023730: 7363 7265 656e 4469 6374 5b72 7369 4b65  screenDict[rsiKe
+00023740: 795d 203d 2063 6f6c 6f72 5465 7874 2e42  y] = colorText.B
+00023750: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
+00023760: 4641 494c 202b 2073 7472 2872 7369 2920  FAIL + str(rsi) 
+00023770: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+00023780: 2020 2020 2020 2020 2320 4966 2065 6974          # If eit
+00023790: 6865 7220 6461 696c 7920 6f72 2069 6e74  her daily or int
+000237a0: 7261 6461 7920 5253 4920 636f 6d65 7320  raday RSI comes 
+000237b0: 7769 7468 696e 2072 616e 6765 3f0a 2020  within range?.  
+000237c0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+000237d0: 7365 2069 6620 2872 7369 4b65 7920 3d3d  se if (rsiKey ==
+000237e0: 2022 5253 4969 2229 2065 6c73 6520 2873   "RSIi") else (s
+000237f0: 656c 662e 7661 6c69 6461 7465 5253 4928  elf.validateRSI(
+00023800: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
+00023810: 7361 7665 4469 6374 2c20 6d69 6e52 5349  saveDict, minRSI
+00023820: 2c20 6d61 7852 5349 2c72 7369 4b65 793d  , maxRSI,rsiKey=
+00023830: 2252 5349 6922 2929 0a0a 2020 2020 2320  "RSIi"))..    # 
+00023840: 5661 6c69 6461 7465 2069 6620 7468 6520  Validate if the 
+00023850: 7374 6f63 6b20 6973 2062 756c 6c69 7368  stock is bullish
+00023860: 2069 6e20 7468 6520 7368 6f72 7420 7465   in the short te
+00023870: 726d 0a20 2020 2064 6566 2076 616c 6964  rm.    def valid
+00023880: 6174 6553 686f 7274 5465 726d 4275 6c6c  ateShortTermBull
+00023890: 6973 6828 7365 6c66 2c20 6466 2c20 7363  ish(self, df, sc
+000238a0: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
+000238b0: 6374 293a 0a20 2020 2020 2020 2069 6620  ct):.        if 
+000238c0: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
+000238d0: 6e28 6466 2920 3d3d 2030 3a0a 2020 2020  n(df) == 0:.    
+000238e0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+000238f0: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
+00023900: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
+00023910: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
+00023920: 6368 6172 7469 6e6b 2e63 6f6d 2f73 6372  chartink.com/scr
+00023930: 6565 6e65 722f 7368 6f72 742d 7465 726d  eener/short-term
+00023940: 2d62 756c 6c69 7368 0a20 2020 2020 2020  -bullish.       
+00023950: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
+00023960: 6c6e 6128 3029 0a20 2020 2020 2020 2064  lna(0).        d
+00023970: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
+00023980: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
+00023990: 696e 665d 2c20 3029 0a20 2020 2020 2020  inf], 0).       
+000239a0: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
+000239b0: 6561 6428 3129 0a20 2020 2020 2020 2066  ead(1).        f
+000239c0: 6b20 3d20 3020 6966 206c 656e 2864 6174  k = 0 if len(dat
+000239d0: 6129 203c 2033 2065 6c73 6520 6e70 2e72  a) < 3 else np.r
+000239e0: 6f75 6e64 2864 6174 615b 2246 4153 544b  ound(data["FASTK
+000239f0: 225d 2e69 6c6f 635b 325d 2c20 3529 0a20  "].iloc[2], 5). 
+00023a00: 2020 2020 2020 2023 2052 6576 6572 7365         # Reverse
+00023a10: 2074 6865 2064 6174 6166 7261 6d65 2066   the dataframe f
+00023a20: 6f72 2069 6368 696d 6f6b 7520 6361 6c63  or ichimoku calc
+00023a30: 756c 6174 696f 6e73 2077 6974 6820 6461  ulations with da
+00023a40: 7465 2069 6e20 6173 6365 6e64 696e 6720  te in ascending 
+00023a50: 6f72 6465 720a 2020 2020 2020 2020 6466  order.        df
+00023a60: 5f6e 6577 203d 2064 6174 615b 3a3a 2d31  _new = data[::-1
+00023a70: 5d0a 2020 2020 2020 2020 7472 793a 0a20  ].        try:. 
+00023a80: 2020 2020 2020 2020 2020 2064 665f 6963             df_ic
+00023a90: 6869 203d 2064 665f 6e65 772e 7265 6e61  hi = df_new.rena
+00023aa0: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
+00023ab0: 2020 2020 636f 6c75 6d6e 733d 7b0a 2020      columns={.  
+00023ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ad0: 2020 224f 7065 6e22 3a20 226f 7065 6e22    "Open": "open"
+00023ae0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00023af0: 2020 2020 2020 2248 6967 6822 3a20 2268        "High": "h
+00023b00: 6967 6822 2c0a 2020 2020 2020 2020 2020  igh",.          
+00023b10: 2020 2020 2020 2020 2020 224c 6f77 223a            "Low":
+00023b20: 2022 6c6f 7722 2c0a 2020 2020 2020 2020   "low",.        
+00023b30: 2020 2020 2020 2020 2020 2020 2243 6c6f              "Clo
+00023b40: 7365 223a 2022 636c 6f73 6522 2c0a 2020  se": "close",.  
+00023b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b60: 2020 2256 6f6c 756d 6522 3a20 2276 6f6c    "Volume": "vol
+00023b70: 756d 6522 2c0a 2020 2020 2020 2020 2020  ume",.          
+00023b80: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00023b90: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00023ba0: 2020 6963 6869 203d 2070 6b74 616c 6962    ichi = pktalib
+00023bb0: 2e69 6368 696d 6f6b 7528 6466 5f69 6368  .ichimoku(df_ich
+00023bc0: 692c 2039 2c20 3236 2c20 3532 2c20 3236  i, 9, 26, 52, 26
+00023bd0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00023be0: 2069 6368 6920 6973 204e 6f6e 653a 0a20   ichi is None:. 
+00023bf0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00023c00: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+00023c10: 2020 2020 2020 2020 6466 5f6e 6577 203d          df_new =
+00023c20: 2070 642e 636f 6e63 6174 285b 6466 5f6e   pd.concat([df_n
+00023c30: 6577 2c20 6963 6869 5d2c 2061 7869 733d  ew, ichi], axis=
+00023c40: 3129 0a20 2020 2020 2020 2020 2020 2023  1).            #
+00023c50: 2052 6576 6572 7365 2061 6761 696e 2074   Reverse again t
+00023c60: 6f20 6765 7420 7468 6520 6d6f 7374 2072  o get the most r
+00023c70: 6563 656e 7420 6461 7465 206f 6e20 746f  ecent date on to
+00023c80: 700a 2020 2020 2020 2020 2020 2020 6466  p.            df
+00023c90: 5f6e 6577 203d 2064 665f 6e65 775b 3a3a  _new = df_new[::
+00023ca0: 2d31 5d0a 2020 2020 2020 2020 2020 2020  -1].            
+00023cb0: 6466 5f6e 6577 203d 2064 665f 6e65 772e  df_new = df_new.
+00023cc0: 6865 6164 2831 290a 2020 2020 2020 2020  head(1).        
+00023cd0: 2020 2020 6466 5f6e 6577 5b22 636c 6f75      df_new["clou
+00023ce0: 645f 6772 6565 6e22 5d20 3d20 6466 5f6e  d_green"] = df_n
+00023cf0: 6577 5b22 4953 415f 3922 5d2e 696c 6f63  ew["ISA_9"].iloc
+00023d00: 5b30 5d20 3e20 6466 5f6e 6577 5b22 4953  [0] > df_new["IS
+00023d10: 425f 3236 225d 2e69 6c6f 635b 305d 0a20  B_26"].iloc[0]. 
+00023d20: 2020 2020 2020 2020 2020 2064 665f 6e65             df_ne
+00023d30: 775b 2263 6c6f 7564 5f72 6564 225d 203d  w["cloud_red"] =
+00023d40: 2064 665f 6e65 775b 2249 5342 5f32 3622   df_new["ISB_26"
+00023d50: 5d2e 696c 6f63 5b30 5d20 3e20 6466 5f6e  ].iloc[0] > df_n
+00023d60: 6577 5b22 4953 415f 3922 5d2e 696c 6f63  ew["ISA_9"].iloc
+00023d70: 5b30 5d0a 2020 2020 2020 2020 6578 6365  [0].        exce
+00023d80: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00023d90: 653a 2020 2320 7072 6167 6d61 3a20 6e6f  e:  # pragma: no
+00023da0: 2063 6f76 6572 0a20 2020 2020 2020 2020   cover.         
+00023db0: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
+00023dc0: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
+00023dd0: 6578 635f 696e 666f 3d54 7275 6529 0a20  exc_info=True). 
+00023de0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+00023df0: 2020 2020 2020 2020 6162 6f76 6543 6c6f          aboveClo
+00023e00: 7564 546f 7020 3d20 4661 6c73 650a 2020  udTop = False.  
+00023e10: 2020 2020 2020 2320 6261 7365 6c69 6e65        # baseline
+00023e20: 203e 2063 6c6f 7564 2074 6f70 2028 636c   > cloud top (cl
+00023e30: 6f75 6420 6973 2062 6f75 6e64 2062 7920  oud is bound by 
+00023e40: 7370 616e 2061 2061 6e64 2073 7061 6e20  span a and span 
+00023e50: 6229 2061 6e64 2063 6c6f 7365 2069 7320  b) and close is 
+00023e60: 3e20 636c 6f75 6420 746f 700a 2020 2020  > cloud top.    
+00023e70: 2020 2020 6966 2064 665f 6e65 775b 2263      if df_new["c
+00023e80: 6c6f 7564 5f67 7265 656e 225d 2e69 6c6f  loud_green"].ilo
+00023e90: 635b 305d 3a0a 2020 2020 2020 2020 2020  c[0]:.          
+00023ea0: 2020 6162 6f76 6543 6c6f 7564 546f 7020    aboveCloudTop 
+00023eb0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00023ec0: 2020 2020 6466 5f6e 6577 5b22 494b 535f      df_new["IKS_
+00023ed0: 3236 225d 2e69 6c6f 635b 305d 203e 2064  26"].iloc[0] > d
+00023ee0: 665f 6e65 775b 2249 5341 5f39 225d 2e69  f_new["ISA_9"].i
+00023ef0: 6c6f 635b 305d 0a20 2020 2020 2020 2020  loc[0].         
+00023f00: 2020 2020 2020 2061 6e64 2072 6563 656e         and recen
+00023f10: 745b 2243 6c6f 7365 225d 2e69 6c6f 635b  t["Close"].iloc[
+00023f20: 305d 203e 2064 665f 6e65 775b 2249 5341  0] > df_new["ISA
+00023f30: 5f39 225d 2e69 6c6f 635b 305d 0a20 2020  _9"].iloc[0].   
+00023f40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00023f50: 2020 2065 6c69 6620 6466 5f6e 6577 5b22     elif df_new["
+00023f60: 636c 6f75 645f 7265 6422 5d2e 696c 6f63  cloud_red"].iloc
+00023f70: 5b30 5d3a 0a20 2020 2020 2020 2020 2020  [0]:.           
+00023f80: 2061 626f 7665 436c 6f75 6454 6f70 203d   aboveCloudTop =
+00023f90: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00023fa0: 2020 2064 665f 6e65 775b 2249 4b53 5f32     df_new["IKS_2
+00023fb0: 3622 5d2e 696c 6f63 5b30 5d20 3e20 6466  6"].iloc[0] > df
+00023fc0: 5f6e 6577 5b22 4953 425f 3236 225d 2e69  _new["ISB_26"].i
+00023fd0: 6c6f 635b 305d 0a20 2020 2020 2020 2020  loc[0].         
+00023fe0: 2020 2020 2020 2061 6e64 2072 6563 656e         and recen
+00023ff0: 745b 2243 6c6f 7365 225d 2e69 6c6f 635b  t["Close"].iloc[
+00024000: 305d 203e 2064 665f 6e65 775b 2249 5342  0] > df_new["ISB
+00024010: 5f32 3622 5d2e 696c 6f63 5b30 5d0a 2020  _26"].iloc[0].  
+00024020: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00024030: 2020 2020 2023 204c 6174 6573 7420 4963       # Latest Ic
+00024040: 6869 6d6f 6b75 2062 6173 656c 696e 6520  himoku baseline 
+00024050: 6973 203c 206c 6174 6573 7420 4963 6869  is < latest Ichi
+00024060: 6d6f 6b75 2063 6f6e 7665 7273 696f 6e20  moku conversion 
+00024070: 6c69 6e65 0a20 2020 2020 2020 2069 6620  line.        if 
+00024080: 6162 6f76 6543 6c6f 7564 546f 7020 616e  aboveCloudTop an
+00024090: 6420 6466 5f6e 6577 5b22 494b 535f 3236  d df_new["IKS_26
+000240a0: 225d 2e69 6c6f 635b 305d 203c 2064 665f  "].iloc[0] < df_
+000240b0: 6e65 775b 2249 5453 5f39 225d 2e69 6c6f  new["ITS_9"].ilo
+000240c0: 635b 305d 3a0a 2020 2020 2020 2020 2020  c[0]:.          
+000240d0: 2020 2320 5374 6f63 6852 5349 2063 726f    # StochRSI cro
+000240e0: 7373 6564 2032 3020 616e 6420 5253 4920  ssed 20 and RSI 
+000240f0: 3e20 3530 0a20 2020 2020 2020 2020 2020  > 50.           
+00024100: 2069 6620 666b 203e 2032 3020 616e 6420   if fk > 20 and 
+00024110: 7265 6365 6e74 5b22 5253 4922 5d2e 696c  recent["RSI"].il
+00024120: 6f63 5b30 5d20 3e20 3530 3a0a 2020 2020  oc[0] > 50:.    
+00024130: 2020 2020 2020 2020 2020 2020 2320 636f              # co
+00024140: 6e64 6974 696f 6e20 6f66 2063 726f 7373  ndition of cross
+00024150: 696e 6720 7468 6520 5374 6f63 6852 5349  ing the StochRSI
+00024160: 206d 6169 6e20 7369 676e 616c 206c 696e   main signal lin
+00024170: 6520 6672 6f6d 2062 6f74 746f 6d20 746f  e from bottom to
+00024180: 2074 6f70 0a20 2020 2020 2020 2020 2020   top.           
+00024190: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+000241a0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+000241b0: 7461 5b22 4641 5354 4422 5d2e 696c 6f63  ta["FASTD"].iloc
+000241c0: 5b31 3030 5d20 3c20 6461 7461 5b22 4641  [100] < data["FA
+000241d0: 5354 4b22 5d2e 696c 6f63 5b31 3030 5d0a  STK"].iloc[100].
+000241e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000241f0: 2020 2020 616e 6420 6461 7461 5b22 4641      and data["FA
+00024200: 5354 4422 5d2e 696c 6f63 5b31 3031 5d20  STD"].iloc[101] 
+00024210: 3e20 6461 7461 5b22 4641 5354 4b22 5d2e  > data["FASTK"].
+00024220: 696c 6f63 5b31 3031 5d0a 2020 2020 2020  iloc[101].      
+00024230: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+00024240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024250: 2023 2063 6c6f 7365 203e 2035 3020 7065   # close > 50 pe
+00024260: 7269 6f64 2053 4d41 2f45 4d41 2061 6e64  riod SMA/EMA and
+00024270: 2032 3030 2070 6572 696f 6420 534d 412f   200 period SMA/
+00024280: 454d 410a 2020 2020 2020 2020 2020 2020  EMA.            
+00024290: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
+000242a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000242b0: 2020 2020 2072 6563 656e 745b 2253 534d       recent["SSM
+000242c0: 4122 5d2e 696c 6f63 5b30 5d20 3e20 7265  A"].iloc[0] > re
+000242d0: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
+000242e0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+000242f0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00024300: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
+00024310: 696c 6f63 5b30 5d20 3e20 7265 6365 6e74  iloc[0] > recent
+00024320: 5b22 5353 4d41 225d 2e69 6c6f 635b 305d  ["SSMA"].iloc[0]
+00024330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024340: 2020 2020 2020 2020 2061 6e64 2072 6563           and rec
+00024350: 656e 745b 2243 6c6f 7365 225d 2e69 6c6f  ent["Close"].ilo
+00024360: 635b 305d 203e 2072 6563 656e 745b 224c  c[0] > recent["L
+00024370: 4d41 225d 2e69 6c6f 635b 305d 0a20 2020  MA"].iloc[0].   
+00024380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024390: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000243a0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+000243b0: 6420 3d20 7365 6c66 2e66 696e 6443 7572  d = self.findCur
+000243c0: 7265 6e74 5361 7665 6456 616c 7565 2873  rentSavedValue(s
+000243d0: 6372 6565 6e44 6963 742c 7361 7665 4469  creenDict,saveDi
+000243e0: 6374 2c22 4d41 2d53 6967 6e61 6c22 290a  ct,"MA-Signal").
+000243f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024400: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+00024410: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+00024420: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00024430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024440: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
+00024450: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
+00024460: 7254 6578 742e 4752 4545 4e20 2b20 2242  rText.GREEN + "B
+00024470: 756c 6c69 7368 2220 2b20 636f 6c6f 7254  ullish" + colorT
+00024480: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+00024490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000244a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000244b0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+000244c0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+000244d0: 3d20 7361 7665 645b 315d 202b 2022 4275  = saved[1] + "Bu
+000244e0: 6c6c 6973 6822 0a20 2020 2020 2020 2020  llish".         
+000244f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00024500: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00024510: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00024520: 2020 2020 0a20 2020 2023 2056 616c 6964      .    # Valid
+00024530: 6174 6520 5643 5020 6173 2070 6572 204d  ate VCP as per M
+00024540: 6172 6b20 4d69 6e65 7276 696e 690a 2020  ark Minervini.  
+00024550: 2020 2320 6874 7470 733a 2f2f 6368 6172    # https://char
+00024560: 7469 6e6b 2e63 6f6d 2f73 6372 6565 6e65  tink.com/screene
+00024570: 722f 766f 6c61 7469 6c69 7479 2d63 6f6d  r/volatility-com
+00024580: 7072 6573 7369 6f6e 0a20 2020 2064 6566  pression.    def
+00024590: 2076 616c 6964 6174 6556 4350 4d61 726b   validateVCPMark
+000245a0: 4d69 6e65 7276 696e 6928 7365 6c66 2c20  Minervini(self, 
+000245b0: 6466 3a70 642e 4461 7461 4672 616d 652c  df:pd.DataFrame,
+000245c0: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
+000245d0: 6544 6963 7429 3a0a 2020 2020 2020 2020  eDict):.        
+000245e0: 6966 2064 6620 6973 204e 6f6e 6520 6f72  if df is None or
+000245f0: 206c 656e 2864 6629 203d 3d20 303a 0a20   len(df) == 0:. 
+00024600: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00024610: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+00024620: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
+00024630: 0a20 2020 2020 2020 206f 686c 635f 6469  .        ohlc_di
+00024640: 6374 203d 207b 0a20 2020 2020 2020 2020  ct = {.         
+00024650: 2020 2027 4f70 656e 273a 2766 6972 7374     'Open':'first
+00024660: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+00024670: 4869 6768 273a 276d 6178 272c 0a20 2020  High':'max',.   
+00024680: 2020 2020 2020 2020 2027 4c6f 7727 3a27           'Low':'
+00024690: 6d69 6e27 2c0a 2020 2020 2020 2020 2020  min',.          
+000246a0: 2020 2743 6c6f 7365 273a 276c 6173 7427    'Close':'last'
+000246b0: 2c0a 2020 2020 2020 2020 2020 2020 2756  ,.            'V
+000246c0: 6f6c 756d 6527 3a27 7375 6d27 0a20 2020  olume':'sum'.   
+000246d0: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
+000246e0: 2066 696e 616c 5f64 6620 3d20 6466 2e72   final_df = df.r
+000246f0: 6573 616d 706c 6528 2757 2d46 5249 272c  esample('W-FRI',
+00024700: 2063 6c6f 7365 643d 276c 6566 7427 292e   closed='left').
+00024710: 6167 6728 6f68 6c63 5f64 6963 7429 2e73  agg(ohlc_dict).s
+00024720: 6869 6674 2827 3164 2729 0a20 2020 2020  hift('1d').     
+00024730: 2020 2077 6565 6b6c 7944 6174 6120 3d20     weeklyData = 
+00024740: 6461 7461 2e72 6573 616d 706c 6528 2757  data.resample('W
+00024750: 2729 2e61 6767 286f 686c 635f 6469 6374  ').agg(ohlc_dict
+00024760: 290a 2020 2020 2020 2020 7265 7665 7273  ).        revers
+00024770: 6564 4461 7461 203d 2064 6174 615b 3a3a  edData = data[::
+00024780: 2d31 5d20 2023 2052 6576 6572 7365 2074  -1]  # Reverse t
+00024790: 6865 2064 6174 6166 7261 6d65 0a20 2020  he dataframe.   
+000247a0: 2020 2020 2072 6563 656e 745f 636c 6f73       recent_clos
+000247b0: 6520 3d20 6461 7461 5b22 436c 6f73 6522  e = data["Close"
+000247c0: 5d2e 6865 6164 2831 292e 696c 6f63 5b30  ].head(1).iloc[0
+000247d0: 5d0a 2020 2020 2020 2020 775f 656d 615f  ].        w_ema_
+000247e0: 3133 203d 2070 6b74 616c 6962 2e45 4d41  13 = pktalib.EMA
+000247f0: 2877 6565 6b6c 7944 6174 615b 2243 6c6f  (weeklyData["Clo
+00024800: 7365 225d 2c74 696d 6570 6572 696f 643d  se"],timeperiod=
+00024810: 3133 292e 7461 696c 2831 292e 696c 6f63  13).tail(1).iloc
+00024820: 5b30 5d0a 2020 2020 2020 2020 775f 656d  [0].        w_em
+00024830: 615f 3236 203d 2070 6b74 616c 6962 2e45  a_26 = pktalib.E
+00024840: 4d41 2877 6565 6b6c 7944 6174 615b 2243  MA(weeklyData["C
+00024850: 6c6f 7365 225d 2c74 696d 6570 6572 696f  lose"],timeperio
+00024860: 643d 3236 292e 7461 696c 2831 292e 696c  d=26).tail(1).il
+00024870: 6f63 5b30 5d0a 2020 2020 2020 2020 775f  oc[0].        w_
+00024880: 736d 615f 3530 203d 2070 6b74 616c 6962  sma_50 = pktalib
+00024890: 2e53 4d41 2877 6565 6b6c 7944 6174 615b  .SMA(weeklyData[
+000248a0: 2243 6c6f 7365 225d 2c74 696d 6570 6572  "Close"],timeper
+000248b0: 696f 643d 3530 292e 7461 696c 2831 292e  iod=50).tail(1).
+000248c0: 696c 6f63 5b30 5d0a 2020 2020 2020 2020  iloc[0].        
+000248d0: 775f 736d 615f 3430 203d 2070 6b74 616c  w_sma_40 = pktal
+000248e0: 6962 2e53 4d41 2877 6565 6b6c 7944 6174  ib.SMA(weeklyDat
+000248f0: 615b 2243 6c6f 7365 225d 2c74 696d 6570  a["Close"],timep
+00024900: 6572 696f 643d 3430 292e 7461 696c 2831  eriod=40).tail(1
+00024910: 292e 696c 6f63 5b30 5d0a 2020 2020 2020  ).iloc[0].      
+00024920: 2020 775f 736d 615f 3430 5f35 775f 6167    w_sma_40_5w_ag
+00024930: 6f20 3d20 706b 7461 6c69 622e 534d 4128  o = pktalib.SMA(
+00024940: 7765 656b 6c79 4461 7461 2e68 6561 6428  weeklyData.head(
+00024950: 6c65 6e28 7765 656b 6c79 4461 7461 292d  len(weeklyData)-
+00024960: 3529 5b22 436c 6f73 6522 5d2c 7469 6d65  5)["Close"],time
+00024970: 7065 7269 6f64 3d34 3029 2e74 6169 6c28  period=40).tail(
+00024980: 3129 2e69 6c6f 635b 305d 0a20 2020 2020  1).iloc[0].     
+00024990: 2020 2077 5f6d 696e 5f35 3020 3d20 6d69     w_min_50 = mi
+000249a0: 6e28 312e 332a 7765 656b 6c79 4461 7461  n(1.3*weeklyData
+000249b0: 2e74 6169 6c28 3530 295b 224c 6f77 225d  .tail(50)["Low"]
+000249c0: 290a 2020 2020 2020 2020 775f 6d61 785f  ).        w_max_
+000249d0: 3530 203d 206d 6178 2830 2e37 352a 7765  50 = max(0.75*we
+000249e0: 656b 6c79 4461 7461 2e74 6169 6c28 3530  eklyData.tail(50
+000249f0: 295b 2248 6967 6822 5d29 0a20 2020 2020  )["High"]).     
+00024a00: 2020 2077 5f65 6d61 5f32 365f 3230 775f     w_ema_26_20w_
+00024a10: 6167 6f20 3d20 706b 7461 6c69 622e 454d  ago = pktalib.EM
+00024a20: 4128 7765 656b 6c79 4461 7461 2e68 6561  A(weeklyData.hea
+00024a30: 6428 6c65 6e28 7765 656b 6c79 4461 7461  d(len(weeklyData
+00024a40: 292d 3230 295b 2243 6c6f 7365 225d 2c74  )-20)["Close"],t
+00024a50: 696d 6570 6572 696f 643d 3236 292e 7461  imeperiod=26).ta
+00024a60: 696c 2831 292e 696c 6f63 5b30 5d0a 2020  il(1).iloc[0].  
+00024a70: 2020 2020 2020 7265 6365 6e74 5f65 6d61        recent_ema
+00024a80: 5f31 335f 3230 645f 6167 6f20 3d20 706b  _13_20d_ago = pk
+00024a90: 7461 6c69 622e 454d 4128 7265 7665 7273  talib.EMA(revers
+00024aa0: 6564 4461 7461 2e68 6561 6428 6c65 6e28  edData.head(len(
+00024ab0: 7265 7665 7273 6564 4461 7461 292d 3230  reversedData)-20
+00024ac0: 295b 2243 6c6f 7365 225d 2c74 696d 6570  )["Close"],timep
+00024ad0: 6572 696f 643d 3133 292e 7461 696c 2831  eriod=13).tail(1
+00024ae0: 292e 696c 6f63 5b30 5d0a 2020 2020 2020  ).iloc[0].      
+00024af0: 2020 775f 736d 615f 3430 5f35 775f 6167    w_sma_40_5w_ag
+00024b00: 6f20 3d20 706b 7461 6c69 622e 534d 4128  o = pktalib.SMA(
+00024b10: 7765 656b 6c79 4461 7461 2e68 6561 6428  weeklyData.head(
+00024b20: 6c65 6e28 7765 656b 6c79 4461 7461 292d  len(weeklyData)-
+00024b30: 3529 5b22 436c 6f73 6522 5d2c 7469 6d65  5)["Close"],time
+00024b40: 7065 7269 6f64 3d34 3029 2e74 6169 6c28  period=40).tail(
+00024b50: 3129 2e69 6c6f 635b 305d 0a20 2020 2020  1).iloc[0].     
+00024b60: 2020 2077 5f73 6d61 5f34 305f 3130 775f     w_sma_40_10w_
+00024b70: 6167 6f20 3d20 706b 7461 6c69 622e 534d  ago = pktalib.SM
+00024b80: 4128 7765 656b 6c79 4461 7461 2e68 6561  A(weeklyData.hea
+00024b90: 6428 6c65 6e28 7765 656b 6c79 4461 7461  d(len(weeklyData
+00024ba0: 292d 3130 295b 2243 6c6f 7365 225d 2c74  )-10)["Close"],t
+00024bb0: 696d 6570 6572 696f 643d 3430 292e 7461  imeperiod=40).ta
+00024bc0: 696c 2831 292e 696c 6f63 5b30 5d0a 2020  il(1).iloc[0].  
+00024bd0: 2020 2020 2020 7265 6365 6e74 5f73 6d61        recent_sma
+00024be0: 5f35 3020 3d20 706b 7461 6c69 622e 534d  _50 = pktalib.SM
+00024bf0: 4128 7265 7665 7273 6564 4461 7461 5b22  A(reversedData["
+00024c00: 436c 6f73 6522 5d2c 7469 6d65 7065 7269  Close"],timeperi
+00024c10: 6f64 3d35 3029 2e74 6169 6c28 3129 2e69  od=50).tail(1).i
+00024c20: 6c6f 635b 305d 0a20 2020 2020 2020 2077  loc[0].        w
+00024c30: 5f77 6d61 5f38 203d 2070 6b74 616c 6962  _wma_8 = pktalib
+00024c40: 2e57 4d41 2877 6565 6b6c 7944 6174 615b  .WMA(weeklyData[
+00024c50: 2243 6c6f 7365 225d 2c74 696d 6570 6572  "Close"],timeper
+00024c60: 696f 643d 3829 2e74 6169 6c28 3129 2e69  iod=8).tail(1).i
+00024c70: 6c6f 635b 305d 0a20 2020 2020 2020 2077  loc[0].        w
+00024c80: 5f73 6d61 5f38 203d 2070 6b74 616c 6962  _sma_8 = pktalib
+00024c90: 2e53 4d41 2877 6565 6b6c 7944 6174 615b  .SMA(weeklyData[
+00024ca0: 2243 6c6f 7365 225d 2c74 696d 6570 6572  "Close"],timeper
+00024cb0: 696f 643d 3829 2e74 6169 6c28 3129 2e69  iod=8).tail(1).i
+00024cc0: 6c6f 635b 305d 0a20 2020 2020 2020 200a  loc[0].        .
+00024cd0: 2020 2020 2020 2020 6973 5643 5020 3d20          isVCP = 
+00024ce0: 775f 656d 615f 3133 203e 2077 5f65 6d61  w_ema_13 > w_ema
+00024cf0: 5f32 3620 616e 6420 5c0a 2020 2020 2020  _26 and \.      
+00024d00: 2020 2020 2020 2020 2020 775f 656d 615f            w_ema_
+00024d10: 3236 203e 2077 5f73 6d61 5f35 3020 616e  26 > w_sma_50 an
+00024d20: 6420 5c0a 2020 2020 2020 2020 2020 2020  d \.            
+00024d30: 2020 2020 775f 736d 615f 3430 203e 2077      w_sma_40 > w
+00024d40: 5f73 6d61 5f34 305f 3577 5f61 676f 2061  _sma_40_5w_ago a
+00024d50: 6e64 205c 0a20 2020 2020 2020 2020 2020  nd \.           
+00024d60: 2020 2020 2072 6563 656e 745f 636c 6f73       recent_clos
+00024d70: 6520 3e3d 2077 5f6d 696e 5f35 3020 616e  e >= w_min_50 an
+00024d80: 6420 5c0a 2020 2020 2020 2020 2020 2020  d \.            
+00024d90: 2020 2020 7265 6365 6e74 5f63 6c6f 7365      recent_close
+00024da0: 203e 3d20 775f 6d61 785f 3530 2061 6e64   >= w_max_50 and
+00024db0: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+00024dc0: 2020 2072 6563 656e 745f 656d 615f 3133     recent_ema_13
+00024dd0: 5f32 3064 5f61 676f 203e 2077 5f65 6d61  _20d_ago > w_ema
+00024de0: 5f32 365f 3230 775f 6167 6f20 616e 6420  _26_20w_ago and 
+00024df0: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
+00024e00: 2020 775f 736d 615f 3430 5f35 775f 6167    w_sma_40_5w_ag
+00024e10: 6f20 3e20 775f 736d 615f 3430 5f31 3077  o > w_sma_40_10w
+00024e20: 5f61 676f 2061 6e64 205c 0a20 2020 2020  _ago and \.     
+00024e30: 2020 2020 2020 2020 2020 2072 6563 656e             recen
+00024e40: 745f 636c 6f73 6520 3e20 7265 6365 6e74  t_close > recent
+00024e50: 5f73 6d61 5f35 3020 616e 6420 5c0a 2020  _sma_50 and \.  
+00024e60: 2020 2020 2020 2020 2020 2020 2020 2877                (w
+00024e70: 5f77 6d61 5f38 202d 2077 5f73 6d61 5f38  _wma_8 - w_sma_8
+00024e80: 292a 362f 3239 203c 2030 2e35 2061 6e64  )*6/29 < 0.5 and
+00024e90: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+00024ea0: 2020 2072 6563 656e 745f 636c 6f73 6520     recent_close 
+00024eb0: 3e20 3130 0a20 2020 2020 2020 2069 6620  > 10.        if 
+00024ec0: 6973 5643 503a 0a20 2020 2020 2020 2020  isVCP:.         
+00024ed0: 2020 2073 6176 6564 203d 2073 656c 662e     saved = self.
+00024ee0: 6669 6e64 4375 7272 656e 7453 6176 6564  findCurrentSaved
+00024ef0: 5661 6c75 6528 7363 7265 656e 4469 6374  Value(screenDict
+00024f00: 2c20 7361 7665 4469 6374 2c20 2250 6174  , saveDict, "Pat
+00024f10: 7465 726e 2229 0a20 2020 2020 2020 2020  tern").         
+00024f20: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
+00024f30: 6174 7465 726e 225d 203d 2028 0a20 2020  attern"] = (.   
+00024f40: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00024f50: 6564 5b30 5d20 0a20 2020 2020 2020 2020  ed[0] .         
+00024f60: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+00024f70: 7874 2e42 4f4c 440a 2020 2020 2020 2020  xt.BOLD.        
+00024f80: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00024f90: 6578 742e 4752 4545 4e0a 2020 2020 2020  ext.GREEN.      
+00024fa0: 2020 2020 2020 2020 2020 2b20 6622 5643            + f"VC
+00024fb0: 5028 4d69 6e65 7276 696e 6929 220a 2020  P(Minervini)".  
+00024fc0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00024fd0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
+00024fe0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00024ff0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+00025000: 5b22 5061 7474 6572 6e22 5d20 3d20 7361  ["Pattern"] = sa
+00025010: 7665 645b 315d 202b 2066 2256 4350 284d  ved[1] + f"VCP(M
+00025020: 696e 6572 7669 6e69 2922 0a20 2020 2020  inervini)".     
+00025030: 2020 2072 6574 7572 6e20 6973 5643 500a     return isVCP.
+00025040: 2020 2020 0a20 2020 2023 2056 616c 6964      .    # Valid
+00025050: 6174 6520 5643 500a 2020 2020 6465 6620  ate VCP.    def 
+00025060: 7661 6c69 6461 7465 5643 5028 0a20 2020  validateVCP(.   
+00025070: 2020 2020 2073 656c 662c 2064 662c 2073       self, df, s
+00025080: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+00025090: 6963 742c 2073 746f 636b 4e61 6d65 3d4e  ict, stockName=N
+000250a0: 6f6e 652c 2077 696e 646f 773d 332c 2070  one, window=3, p
+000250b0: 6572 6365 6e74 6167 6546 726f 6d54 6f70  ercentageFromTop
+000250c0: 3d33 0a20 2020 2029 3a0a 2020 2020 2020  =3.    ):.      
+000250d0: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
+000250e0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
+000250f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00025100: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00025110: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
+00025120: 2829 0a20 2020 2020 2020 2074 7279 3a0a  ().        try:.
+00025130: 2020 2020 2020 2020 2020 2020 7065 7263              perc
+00025140: 656e 7461 6765 4672 6f6d 546f 7020 2f3d  entageFromTop /=
+00025150: 2031 3030 0a20 2020 2020 2020 2020 2020   100.           
+00025160: 2064 6174 612e 7265 7365 745f 696e 6465   data.reset_inde
+00025170: 7828 696e 706c 6163 653d 5472 7565 290a  x(inplace=True).
+00025180: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00025190: 2e72 656e 616d 6528 636f 6c75 6d6e 733d  .rename(columns=
+000251a0: 7b22 696e 6465 7822 3a20 2244 6174 6522  {"index": "Date"
+000251b0: 7d2c 2069 6e70 6c61 6365 3d54 7275 6529  }, inplace=True)
+000251c0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000251d0: 615b 2274 6f70 7322 5d20 3d20 2864 6174  a["tops"] = (dat
+000251e0: 615b 2248 6967 6822 5d2e 696c 6f63 5b6c  a["High"].iloc[l
+000251f0: 6973 7428 706b 7461 6c69 622e 6172 6772  ist(pktalib.argr
+00025200: 656c 6578 7472 656d 6128 6e70 2e61 7272  elextrema(np.arr
+00025210: 6179 2864 6174 615b 2248 6967 6822 5d29  ay(data["High"])
+00025220: 2c20 6e70 2e67 7265 6174 6572 5f65 7175  , np.greater_equ
+00025230: 616c 2c20 6f72 6465 723d 7769 6e64 6f77  al, order=window
+00025240: 295b 305d 295d 2e68 6561 6428 3429 290a  )[0])].head(4)).
+00025250: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00025260: 5b22 626f 7473 225d 203d 2028 6461 7461  ["bots"] = (data
+00025270: 5b22 4c6f 7722 5d2e 696c 6f63 5b6c 6973  ["Low"].iloc[lis
+00025280: 7428 706b 7461 6c69 622e 6172 6772 656c  t(pktalib.argrel
+00025290: 6578 7472 656d 6128 6e70 2e61 7272 6179  extrema(np.array
+000252a0: 2864 6174 615b 224c 6f77 225d 292c 206e  (data["Low"]), n
+000252b0: 702e 6c65 7373 5f65 7175 616c 2c20 6f72  p.less_equal, or
+000252c0: 6465 723d 7769 6e64 6f77 295b 305d 295d  der=window)[0])]
+000252d0: 2e68 6561 6428 3429 290a 2020 2020 2020  .head(4)).      
+000252e0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+000252f0: 612e 6669 6c6c 6e61 2830 290a 2020 2020  a.fillna(0).    
+00025300: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00025310: 6174 612e 7265 706c 6163 6528 5b6e 702e  ata.replace([np.
+00025320: 696e 662c 202d 6e70 2e69 6e66 5d2c 2030  inf, -np.inf], 0
+00025330: 290a 2020 2020 2020 2020 2020 2020 746f  ).            to
+00025340: 7073 203d 2064 6174 615b 6461 7461 2e74  ps = data[data.t
+00025350: 6f70 7320 3e20 305d 0a20 2020 2020 2020  ops > 0].       
+00025360: 2020 2020 2023 2062 6f74 7320 3d20 6461       # bots = da
+00025370: 7461 5b64 6174 612e 626f 7473 203e 2030  ta[data.bots > 0
+00025380: 5d0a 2020 2020 2020 2020 2020 2020 6869  ].            hi
+00025390: 6768 6573 7454 6f70 203d 2072 6f75 6e64  ghestTop = round
+000253a0: 2874 6f70 732e 6465 7363 7269 6265 2829  (tops.describe()
+000253b0: 5b22 4869 6768 225d 5b22 6d61 7822 5d2c  ["High"]["max"],
+000253c0: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
+000253d0: 6669 6c74 6572 6564 546f 7073 203d 2074  filteredTops = t
+000253e0: 6f70 735b 0a20 2020 2020 2020 2020 2020  ops[.           
+000253f0: 2020 2020 2074 6f70 732e 746f 7073 203e       tops.tops >
+00025400: 2028 6869 6768 6573 7454 6f70 202d 2028   (highestTop - (
+00025410: 6869 6768 6573 7454 6f70 202a 2070 6572  highestTop * per
+00025420: 6365 6e74 6167 6546 726f 6d54 6f70 2929  centageFromTop))
+00025430: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
+00025440: 2020 2020 2020 2020 2020 2069 6620 6669             if fi
+00025450: 6c74 6572 6564 546f 7073 2e65 7175 616c  lteredTops.equal
+00025460: 7328 746f 7073 293a 2020 2320 546f 7073  s(tops):  # Tops
+00025470: 2061 7265 2069 6e20 7468 6520 7261 6e67   are in the rang
+00025480: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00025490: 2020 6c6f 7750 6f69 6e74 7320 3d20 5b5d    lowPoints = []
+000254a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000254b0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+000254c0: 6c65 6e28 746f 7073 2920 2d20 3129 3a0a  len(tops) - 1):.
+000254d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000254e0: 2020 2020 656e 6444 6174 6520 3d20 746f      endDate = to
+000254f0: 7073 2e69 6c6f 635b 695d 5b22 4461 7465  ps.iloc[i]["Date
+00025500: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00025510: 2020 2020 2020 2073 7461 7274 4461 7465         startDate
+00025520: 203d 2074 6f70 732e 696c 6f63 5b69 202b   = tops.iloc[i +
+00025530: 2031 5d5b 2244 6174 6522 5d0a 2020 2020   1]["Date"].    
+00025540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025550: 6c6f 7750 6f69 6e74 732e 6170 7065 6e64  lowPoints.append
+00025560: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00025570: 2020 2020 2020 2020 2020 6461 7461 5b0a            data[.
+00025580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025590: 2020 2020 2020 2020 2020 2020 2864 6174              (dat
+000255a0: 612e 4461 7465 203e 3d20 7374 6172 7444  a.Date >= startD
+000255b0: 6174 6529 2026 2028 6461 7461 2e44 6174  ate) & (data.Dat
+000255c0: 6520 3c3d 2065 6e64 4461 7465 290a 2020  e <= endDate).  
 000255d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000255e0: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-000255f0: 2020 2020 2020 2020 2020 2020 2073 7072               spr
-00025600: 6561 6430 203c 2073 7072 6561 6431 0a20  ead0 < spread1. 
-00025610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025620: 2020 2020 2020 2061 6e64 2076 6f6c 3020         and vol0 
-00025630: 3e20 766f 6c31 0a20 2020 2020 2020 2020  > vol1.         
-00025640: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00025650: 6e64 2064 6174 612e 696c 6f63 5b30 5d5b  nd data.iloc[0][
-00025660: 2256 6f6c 756d 6522 5d20 3e20 6461 7461  "Volume"] > data
-00025670: 2e69 6c6f 635b 305d 5b22 566f 6c4d 4122  .iloc[0]["VolMA"
-00025680: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00025690: 2020 2020 2020 2020 2020 616e 6420 6461            and da
-000256a0: 7461 2e69 6c6f 635b 305d 5b22 436c 6f73  ta.iloc[0]["Clos
-000256b0: 6522 5d20 3c3d 2064 6174 612e 696c 6f63  e"] <= data.iloc
-000256c0: 5b31 5d5b 224f 7065 6e22 5d0a 2020 2020  [1]["Open"].    
+000255e0: 2020 2020 2020 5d2e 6465 7363 7269 6265        ].describe
+000255f0: 2829 5b22 4c6f 7722 5d5b 226d 696e 225d  ()["Low"]["min"]
+00025600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025610: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00025620: 2020 2020 2020 206c 6f77 506f 696e 7473         lowPoints
+00025630: 4f72 6720 3d20 6c6f 7750 6f69 6e74 730a  Org = lowPoints.
+00025640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025650: 6c6f 7750 6f69 6e74 732e 736f 7274 2872  lowPoints.sort(r
+00025660: 6576 6572 7365 3d54 7275 6529 0a20 2020  everse=True).   
+00025670: 2020 2020 2020 2020 2020 2020 206c 6f77               low
+00025680: 506f 696e 7473 536f 7274 6564 203d 206c  PointsSorted = l
+00025690: 6f77 506f 696e 7473 0a20 2020 2020 2020  owPoints.       
+000256a0: 2020 2020 2020 2020 2069 6620 6461 7461           if data
+000256b0: 2e65 6d70 7479 206f 7220 6c65 6e28 6c6f  .empty or len(lo
+000256c0: 7750 6f69 6e74 7329 203c 2031 3a0a 2020  wPoints) < 1:.  
 000256d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000256e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000256f0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00025700: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
-00025710: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00025720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025730: 2073 6176 6564 5b30 5d20 0a20 2020 2020   saved[0] .     
-00025740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025750: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-00025760: 7874 2e42 4f4c 440a 2020 2020 2020 2020  xt.BOLD.        
+000256e0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+000256f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00025700: 7470 203d 2064 6174 612e 6865 6164 2831  tp = data.head(1
+00025710: 295b 2243 6c6f 7365 225d 2e69 6c6f 635b  )["Close"].iloc[
+00025720: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+00025730: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+00025740: 2020 2020 2020 2020 2020 2020 6c6f 7750              lowP
+00025750: 6f69 6e74 734f 7267 203d 3d20 6c6f 7750  ointsOrg == lowP
+00025760: 6f69 6e74 7353 6f72 7465 640a 2020 2020  ointsSorted.    
 00025770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025780: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-00025790: 4752 4545 4e0a 2020 2020 2020 2020 2020  GREEN.          
-000257a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257b0: 2020 2b20 2244 656d 616e 6420 5269 7365    + "Demand Rise
-000257c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000257d0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-000257e0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-000257f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025800: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00025810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025820: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
-00025830: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
-00025840: 2022 4465 6d61 6e64 2052 6973 6522 0a20   "Demand Rise". 
-00025850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025860: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00025870: 7565 0a20 2020 2020 2020 2020 2020 2065  ue.            e
-00025880: 7863 6570 7420 496e 6465 7845 7272 6f72  xcept IndexError
-00025890: 2061 7320 653a 2023 2070 7261 676d 613a   as e: # pragma:
-000258a0: 206e 6f20 636f 7665 720a 2020 2020 2020   no cover.      
-000258b0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-000258c0: 6566 6175 6c74 5f6c 6f67 6765 722e 6465  efault_logger.de
-000258d0: 6275 6728 652c 2065 7863 5f69 6e66 6f3d  bug(e, exc_info=
-000258e0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-000258f0: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-00025900: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00025910: 6c73 650a 2020 2020 2020 2020 6578 6365  lse.        exce
-00025920: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00025930: 653a 2020 2320 7072 6167 6d61 3a20 6e6f  e:  # pragma: no
-00025940: 2063 6f76 6572 0a20 2020 2020 2020 2020   cover.         
-00025950: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
-00025960: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
-00025970: 6578 635f 696e 666f 3d54 7275 6529 0a20  exc_info=True). 
-00025980: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00025990: 6e20 4661 6c73 650a                      n False.
+00025780: 616e 6420 6c74 7020 3c20 6869 6768 6573  and ltp < highes
+00025790: 7454 6f70 0a20 2020 2020 2020 2020 2020  tTop.           
+000257a0: 2020 2020 2020 2020 2061 6e64 206c 7470           and ltp
+000257b0: 203e 206c 6f77 506f 696e 7473 5b30 5d0a   > lowPoints[0].
+000257c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000257d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000257e0: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
+000257f0: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
+00025800: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
+00025810: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
+00025820: 2250 6174 7465 726e 2229 0a20 2020 2020  "Pattern").     
+00025830: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00025840: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
+00025850: 726e 225d 203d 2028 0a20 2020 2020 2020  rn"] = (.       
+00025860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025870: 2073 6176 6564 5b30 5d20 0a20 2020 2020   saved[0] .     
+00025880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025890: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
+000258a0: 4f4c 440a 2020 2020 2020 2020 2020 2020  OLD.            
+000258b0: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+000258c0: 6c6f 7254 6578 742e 4752 4545 4e0a 2020  lorText.GREEN.  
+000258d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000258e0: 2020 2020 2020 2b20 6622 5643 5020 2842        + f"VCP (B
+000258f0: 4f3a 207b 6869 6768 6573 7454 6f70 7d29  O: {highestTop})
+00025900: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00025910: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+00025920: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+00025930: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00025940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025950: 2020 2020 7361 7665 4469 6374 5b22 5061      saveDict["Pa
+00025960: 7474 6572 6e22 5d20 3d20 7361 7665 645b  ttern"] = saved[
+00025970: 315d 202b 2066 2256 4350 2028 424f 3a20  1] + f"VCP (BO: 
+00025980: 7b68 6967 6865 7374 546f 707d 2922 0a20  {highestTop})". 
+00025990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000259a0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+000259b0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+000259c0: 6365 7074 696f 6e20 6173 2065 3a20 2023  ception as e:  #
+000259d0: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
+000259e0: 720a 2020 2020 2020 2020 2020 2020 7365  r.            se
+000259f0: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
+00025a00: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
+00025a10: 6e66 6f3d 5472 7565 290a 2020 2020 2020  nfo=True).      
+00025a20: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+00025a30: 2020 2020 2320 5661 6c69 6461 7465 2069      # Validate i
+00025a40: 6620 766f 6c75 6d65 206f 6620 6c61 7374  f volume of last
+00025a50: 2064 6179 2069 7320 6869 6768 6572 2074   day is higher t
+00025a60: 6861 6e20 6176 670a 2020 2020 6465 6620  han avg.    def 
+00025a70: 7661 6c69 6461 7465 566f 6c75 6d65 280a  validateVolume(.
+00025a80: 2020 2020 2020 2020 7365 6c66 2c20 6466          self, df
+00025a90: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
+00025aa0: 7665 4469 6374 2c20 766f 6c75 6d65 5261  veDict, volumeRa
+00025ab0: 7469 6f3d 322e 352c 206d 696e 566f 6c75  tio=2.5, minVolu
+00025ac0: 6d65 3d31 3030 0a20 2020 2029 3a0a 2020  me=100.    ):.  
+00025ad0: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
+00025ae0: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
+00025af0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00025b00: 2072 6574 7572 6e20 4661 6c73 652c 2046   return False, F
+00025b10: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
+00025b20: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
+00025b30: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00025b40: 612e 6669 6c6c 6e61 2830 290a 2020 2020  a.fillna(0).    
+00025b50: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+00025b60: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
+00025b70: 202d 6e70 2e69 6e66 5d2c 2030 290a 2020   -np.inf], 0).  
+00025b80: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
+00025b90: 6174 612e 6865 6164 2831 290a 2020 2020  ata.head(1).    
+00025ba0: 2020 2020 2320 4569 7468 6572 2074 6865      # Either the
+00025bb0: 2072 6f6c 6c69 6e67 2076 6f6c 756d 6520   rolling volume 
+00025bc0: 6f66 2070 6173 7420 3230 2073 6573 7369  of past 20 sessi
+00025bd0: 6f6e 7320 6f72 2074 6f64 6179 2773 2076  ons or today's v
+00025be0: 6f6c 756d 6520 7368 6f75 6c64 2062 6520  olume should be 
+00025bf0: 3e20 6d69 6e20 766f 6c75 6d65 0a20 2020  > min volume.   
+00025c00: 2020 2020 2068 6173 4d69 6e69 6d75 6d56       hasMinimumV
+00025c10: 6f6c 756d 6520 3d20 280a 2020 2020 2020  olume = (.      
+00025c20: 2020 2020 2020 7265 6365 6e74 5b22 566f        recent["Vo
+00025c30: 6c4d 4122 5d2e 696c 6f63 5b30 5d20 3e3d  lMA"].iloc[0] >=
+00025c40: 206d 696e 566f 6c75 6d65 0a20 2020 2020   minVolume.     
+00025c50: 2020 2020 2020 206f 7220 7265 6365 6e74         or recent
+00025c60: 5b22 566f 6c75 6d65 225d 2e69 6c6f 635b  ["Volume"].iloc[
+00025c70: 305d 203e 3d20 6d69 6e56 6f6c 756d 650a  0] >= minVolume.
+00025c80: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00025c90: 2020 6966 2072 6563 656e 745b 2256 6f6c    if recent["Vol
+00025ca0: 4d41 225d 2e69 6c6f 635b 305d 203d 3d20  MA"].iloc[0] == 
+00025cb0: 303a 2020 2320 4861 6e64 6c65 7320 4469  0:  # Handles Di
+00025cc0: 7669 6465 2062 7920 3020 7761 726e 696e  vide by 0 warnin
+00025cd0: 670a 2020 2020 2020 2020 2020 2020 7361  g.            sa
+00025ce0: 7665 4469 6374 5b22 566f 6c75 6d65 225d  veDict["Volume"]
+00025cf0: 203d 2030 2020 2320 2255 6e6b 6e6f 776e   = 0  # "Unknown
+00025d00: 220a 2020 2020 2020 2020 2020 2020 7363  ".            sc
+00025d10: 7265 656e 4469 6374 5b22 566f 6c75 6d65  reenDict["Volume
+00025d20: 225d 203d 2030 0a20 2020 2020 2020 2020  "] = 0.         
+00025d30: 2020 2072 6574 7572 6e20 4661 6c73 652c     return False,
+00025d40: 2068 6173 4d69 6e69 6d75 6d56 6f6c 756d   hasMinimumVolum
+00025d50: 650a 2020 2020 2020 2020 7261 7469 6f20  e.        ratio 
+00025d60: 3d20 726f 756e 6428 7265 6365 6e74 5b22  = round(recent["
+00025d70: 566f 6c75 6d65 225d 2e69 6c6f 635b 305d  Volume"].iloc[0]
+00025d80: 202f 2072 6563 656e 745b 2256 6f6c 4d41   / recent["VolMA
+00025d90: 225d 2e69 6c6f 635b 305d 2c20 3229 0a20  "].iloc[0], 2). 
+00025da0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
+00025db0: 2256 6f6c 756d 6522 5d20 3d20 7261 7469  "Volume"] = rati
+00025dc0: 6f0a 2020 2020 2020 2020 6966 2072 6174  o.        if rat
+00025dd0: 696f 203e 3d20 766f 6c75 6d65 5261 7469  io >= volumeRati
+00025de0: 6f20 616e 6420 7261 7469 6f20 213d 206e  o and ratio != n
+00025df0: 702e 6e61 6e20 616e 6420 286e 6f74 206d  p.nan and (not m
+00025e00: 6174 682e 6973 696e 6628 7261 7469 6f29  ath.isinf(ratio)
+00025e10: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00025e20: 6372 6565 6e44 6963 745b 2256 6f6c 756d  creenDict["Volum
+00025e30: 6522 5d20 3d20 7261 7469 6f0a 2020 2020  e"] = ratio.    
+00025e40: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00025e50: 7275 652c 2068 6173 4d69 6e69 6d75 6d56  rue, hasMinimumV
+00025e60: 6f6c 756d 650a 2020 2020 2020 2020 7363  olume.        sc
+00025e70: 7265 656e 4469 6374 5b22 566f 6c75 6d65  reenDict["Volume
+00025e80: 225d 203d 2072 6174 696f 0a20 2020 2020  "] = ratio.     
+00025e90: 2020 2072 6574 7572 6e20 4661 6c73 652c     return False,
+00025ea0: 2068 6173 4d69 6e69 6d75 6d56 6f6c 756d   hasMinimumVolum
+00025eb0: 650a 0a20 2020 2023 2046 696e 6420 6966  e..    # Find if
+00025ec0: 2073 746f 636b 2069 7320 7661 6c69 6461   stock is valida
+00025ed0: 7469 6e67 2076 6f6c 756d 6520 7370 7265  ting volume spre
+00025ee0: 6164 2061 6e61 6c79 7369 730a 2020 2020  ad analysis.    
+00025ef0: 6465 6620 7661 6c69 6461 7465 566f 6c75  def validateVolu
+00025f00: 6d65 5370 7265 6164 416e 616c 7973 6973  meSpreadAnalysis
+00025f10: 2873 656c 662c 2064 662c 2073 6372 6565  (self, df, scree
+00025f20: 6e44 6963 742c 2073 6176 6544 6963 7429  nDict, saveDict)
+00025f30: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
+00025f40: 2020 2020 2020 2020 2020 2069 6620 6466             if df
+00025f50: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
+00025f60: 6466 2920 3d3d 2030 3a0a 2020 2020 2020  df) == 0:.      
+00025f70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00025f80: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
+00025f90: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
+00025fa0: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
+00025fb0: 6461 7461 203d 2064 6174 612e 6865 6164  data = data.head
+00025fc0: 2832 290a 2020 2020 2020 2020 2020 2020  (2).            
+00025fd0: 6966 206c 656e 2864 6174 6129 203c 2032  if len(data) < 2
+00025fe0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00025ff0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+00026000: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00026010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026020: 2320 4368 6563 6b20 666f 7220 7072 6576  # Check for prev
+00026030: 696f 7573 2052 4544 2063 616e 646c 6573  ious RED candles
+00026040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026050: 2023 2043 7572 7265 6e74 2063 616e 646c   # Current candl
+00026060: 6520 3d20 3074 682c 2050 7265 7669 6f75  e = 0th, Previou
+00026070: 7320 4361 6e64 6c65 203d 2031 7374 2066  s Candle = 1st f
+00026080: 6f72 2066 6f6c 6c6f 7769 6e67 206c 6f67  or following log
+00026090: 6963 0a20 2020 2020 2020 2020 2020 2020  ic.             
+000260a0: 2020 2069 6620 6461 7461 2e69 6c6f 635b     if data.iloc[
+000260b0: 315d 5b22 4f70 656e 225d 203e 3d20 6461  1]["Open"] >= da
+000260c0: 7461 2e69 6c6f 635b 315d 5b22 436c 6f73  ta.iloc[1]["Clos
+000260d0: 6522 5d3a 0a20 2020 2020 2020 2020 2020  e"]:.           
+000260e0: 2020 2020 2020 2020 2073 7072 6561 6431           spread1
+000260f0: 203d 2061 6273 2864 6174 612e 696c 6f63   = abs(data.iloc
+00026100: 5b31 5d5b 224f 7065 6e22 5d20 2d20 6461  [1]["Open"] - da
+00026110: 7461 2e69 6c6f 635b 315d 5b22 436c 6f73  ta.iloc[1]["Clos
+00026120: 6522 5d29 0a20 2020 2020 2020 2020 2020  e"]).           
+00026130: 2020 2020 2020 2020 2073 7072 6561 6430           spread0
+00026140: 203d 2061 6273 2864 6174 612e 696c 6f63   = abs(data.iloc
+00026150: 5b30 5d5b 224f 7065 6e22 5d20 2d20 6461  [0]["Open"] - da
+00026160: 7461 2e69 6c6f 635b 305d 5b22 436c 6f73  ta.iloc[0]["Clos
+00026170: 6522 5d29 0a20 2020 2020 2020 2020 2020  e"]).           
+00026180: 2020 2020 2020 2020 206c 6f77 6572 5f77           lower_w
+00026190: 6963 6b5f 7370 7265 6164 3020 3d20 280a  ick_spread0 = (.
+000261a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000261b0: 2020 2020 2020 2020 6d61 7828 6461 7461          max(data
+000261c0: 2e69 6c6f 635b 305d 5b22 4f70 656e 225d  .iloc[0]["Open"]
+000261d0: 2c20 6461 7461 2e69 6c6f 635b 305d 5b22  , data.iloc[0]["
+000261e0: 436c 6f73 6522 5d29 0a20 2020 2020 2020  Close"]).       
+000261f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026200: 202d 2064 6174 612e 696c 6f63 5b30 5d5b   - data.iloc[0][
+00026210: 224c 6f77 225d 0a20 2020 2020 2020 2020  "Low"].         
+00026220: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00026230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026240: 2076 6f6c 3120 3d20 6461 7461 2e69 6c6f   vol1 = data.ilo
+00026250: 635b 315d 5b22 566f 6c75 6d65 225d 0a20  c[1]["Volume"]. 
+00026260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026270: 2020 2076 6f6c 3020 3d20 6461 7461 2e69     vol0 = data.i
+00026280: 6c6f 635b 305d 5b22 566f 6c75 6d65 225d  loc[0]["Volume"]
+00026290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000262a0: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
+000262b0: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
+000262c0: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
+000262d0: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
+000262e0: 6174 7465 726e 2229 0a20 2020 2020 2020  attern").       
+000262f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00026300: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00026310: 2020 2020 2020 2020 2020 7370 7265 6164            spread
+00026320: 3020 3e20 7370 7265 6164 310a 2020 2020  0 > spread1.    
+00026330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026340: 2020 2020 616e 6420 766f 6c30 203c 2076      and vol0 < v
+00026350: 6f6c 310a 2020 2020 2020 2020 2020 2020  ol1.            
+00026360: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00026370: 6461 7461 2e69 6c6f 635b 305d 5b22 566f  data.iloc[0]["Vo
+00026380: 6c75 6d65 225d 203c 2064 6174 612e 696c  lume"] < data.il
+00026390: 6f63 5b30 5d5b 2256 6f6c 4d41 225d 0a20  oc[0]["VolMA"]. 
+000263a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000263b0: 2020 2020 2020 2061 6e64 2064 6174 612e         and data.
+000263c0: 696c 6f63 5b30 5d5b 2243 6c6f 7365 225d  iloc[0]["Close"]
+000263d0: 203c 3d20 6461 7461 2e69 6c6f 635b 315d   <= data.iloc[1]
+000263e0: 5b22 4f70 656e 225d 0a20 2020 2020 2020  ["Open"].       
+000263f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026400: 2061 6e64 2073 7072 6561 6430 203c 206c   and spread0 < l
+00026410: 6f77 6572 5f77 6963 6b5f 7370 7265 6164  ower_wick_spread
+00026420: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+00026430: 2020 2020 2020 2020 2020 616e 6420 6461            and da
+00026440: 7461 2e69 6c6f 635b 305d 5b22 566f 6c75  ta.iloc[0]["Volu
+00026450: 6d65 225d 203c 3d20 696e 7428 6461 7461  me"] <= int(data
+00026460: 2e69 6c6f 635b 315d 5b22 566f 6c75 6d65  .iloc[1]["Volume
+00026470: 225d 202a 2030 2e37 3529 0a20 2020 2020  "] * 0.75).     
+00026480: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00026490: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000264a0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
+000264b0: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
+000264c0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+000264d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000264e0: 7361 7665 645b 305d 200a 2020 2020 2020  saved[0] .      
+000264f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026500: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+00026510: 742e 424f 4c44 0a20 2020 2020 2020 2020  t.BOLD.         
+00026520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026530: 2020 202b 2063 6f6c 6f72 5465 7874 2e47     + colorText.G
+00026540: 5245 454e 0a20 2020 2020 2020 2020 2020  REEN.           
+00026550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026560: 202b 2022 5375 7070 6c79 2044 726f 7567   + "Supply Droug
+00026570: 6874 220a 2020 2020 2020 2020 2020 2020  ht".            
+00026580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026590: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+000265a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000265b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000265c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000265d0: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
+000265e0: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
+000265f0: 202b 2022 5375 7070 6c79 2044 726f 7567   + "Supply Droug
+00026600: 6874 220a 2020 2020 2020 2020 2020 2020  ht".            
+00026610: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00026620: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+00026630: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00026640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026650: 2020 2020 2020 2020 2073 7072 6561 6430           spread0
+00026660: 203c 2073 7072 6561 6431 0a20 2020 2020   < spread1.     
+00026670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026680: 2020 2061 6e64 2076 6f6c 3020 3e20 766f     and vol0 > vo
+00026690: 6c31 0a20 2020 2020 2020 2020 2020 2020  l1.             
+000266a0: 2020 2020 2020 2020 2020 2061 6e64 2064             and d
+000266b0: 6174 612e 696c 6f63 5b30 5d5b 2256 6f6c  ata.iloc[0]["Vol
+000266c0: 756d 6522 5d20 3e20 6461 7461 2e69 6c6f  ume"] > data.ilo
+000266d0: 635b 305d 5b22 566f 6c4d 4122 5d0a 2020  c[0]["VolMA"].  
+000266e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000266f0: 2020 2020 2020 616e 6420 6461 7461 2e69        and data.i
+00026700: 6c6f 635b 305d 5b22 436c 6f73 6522 5d20  loc[0]["Close"] 
+00026710: 3c3d 2064 6174 612e 696c 6f63 5b31 5d5b  <= data.iloc[1][
+00026720: 224f 7065 6e22 5d0a 2020 2020 2020 2020  "Open"].        
+00026730: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
+00026740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026750: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00026760: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
+00026770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026780: 2020 2020 2020 2020 2020 2020 2073 6176               sav
+00026790: 6564 5b30 5d20 0a20 2020 2020 2020 2020  ed[0] .         
+000267a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000267b0: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
+000267c0: 4f4c 440a 2020 2020 2020 2020 2020 2020  OLD.            
+000267d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000267e0: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+000267f0: 4e0a 2020 2020 2020 2020 2020 2020 2020  N.              
+00026800: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00026810: 2244 656d 616e 6420 5269 7365 220a 2020  "Demand Rise".  
+00026820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026830: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+00026840: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+00026850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026860: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00026870: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00026880: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
+00026890: 3d20 7361 7665 645b 315d 202b 2022 4465  = saved[1] + "De
+000268a0: 6d61 6e64 2052 6973 6522 0a20 2020 2020  mand Rise".     
+000268b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000268c0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
+000268d0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+000268e0: 7420 496e 6465 7845 7272 6f72 2061 7320  t IndexError as 
+000268f0: 653a 2023 2070 7261 676d 613a 206e 6f20  e: # pragma: no 
+00026900: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
+00026910: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
+00026920: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
+00026930: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
+00026940: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00026950: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
+00026960: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00026970: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00026980: 7863 6570 7469 6f6e 2061 7320 653a 2020  xception as e:  
+00026990: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+000269a0: 6572 0a20 2020 2020 2020 2020 2020 2073  er.            s
+000269b0: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
+000269c0: 6572 2e64 6562 7567 2865 2c20 6578 635f  er.debug(e, exc_
+000269d0: 696e 666f 3d54 7275 6529 0a20 2020 2020  info=True).     
+000269e0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+000269f0: 6c73 650a                                lse.
```

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/StockScreener.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,15 @@
                 isConfluence = False
                 isInsideBar = 0
                 isMaReversal = 0
                 isIpoBase = False
                 isMaSupport = False
                 isLorentzian = False
                 isVCP = False
+                isMinerviniVCP = False
                 isVSA = False
                 isNR = False
                 hasPsarRSIReversal = False
                 hasRisingRSIReversal = False
                 hasRSIMAReversal = False
                 isValidRsi = False
                 isBuyingTrendline = False
@@ -259,14 +260,15 @@
                 consolidationValue = 0
                 isBreaking = False
                 isValidCci = False
                 isVSA = False
                 isCandlePattern = False
                 isLowestVolume = False
                 hasBbandsSqz = False
+                hasMASignalFilter = False
 
                 isValidityCheckMet = self.performValidityCheckForExecuteOptions(executeOption,screener,fullData,screeningDictionary,saveDictionary,processedData,configManager,maLength)
                 if not isValidityCheckMet:
                     return returnLegibleData("Validity Check not met!")
                 isShortTermBullish = (executeOption == 11 and isValidityCheckMet)
                 if newlyListedOnly:
                     isIpoBase = screener.validateIpoBase(
@@ -395,15 +397,26 @@
                         if not hasBbandsSqz:
                             return returnLegibleData(f"hasBbandsSqz:{hasBbandsSqz}")
                     elif respChartPattern == 7:
                         isCandlePattern = candlePatterns.findPattern(
                         processedData, screeningDictionary, saveDictionary)
                         if not isCandlePattern:
                             return returnLegibleData(f"isCandlePattern:{isCandlePattern}")
-                        
+                    elif respChartPattern == 8:
+                        isMinerviniVCP = screener.validateVCPMarkMinervini(
+                            fullData, screeningDictionary, saveDictionary
+                        )
+                        if not isMinerviniVCP:
+                            return returnLegibleData(f"isMinerviniVCP:{isMinerviniVCP}")
+                    elif respChartPattern == 9:
+                        hasMASignalFilter = screener.validateMovingAverages(
+                            fullData, screeningDictionary, saveDictionary,maRange=1.25,maLength=maLength
+                        )
+                        if not hasMASignalFilter:
+                            return returnLegibleData(f"hasMASignalFilter:{hasMASignalFilter}")
                 elif executeOption == 10:
                     isPriceRisingByAtLeast2Percent = (
                         screener.validatePriceRisingByAtLeast2Percent(
                             processedData, screeningDictionary, saveDictionary
                         )
                     )
                     if not isPriceRisingByAtLeast2Percent:
@@ -456,15 +469,15 @@
                 if executeOption == 8:
                     isValidCci = screener.validateCCI(
                         processedData, screeningDictionary, saveDictionary, minRSI, maxRSI
                     )
                     if not isValidCci:
                         return returnLegibleData(f"isValidCci:{isValidCci}")
 
-                if not (isConfluence or isShortTermBullish or isMaSupport):
+                if not (isConfluence or isShortTermBullish or hasMASignalFilter):
                     isMaReversal = screener.validateMovingAverages(
                         processedData, screeningDictionary, saveDictionary, maRange=1.25
                     )
                 if executeOption == 6:
                     if reversalOption == 1 and not (str(saveDictionary["Pattern"]).split(",")[0]
                                                                     in CandlePatterns.reversalPatternsBullish
                                                                     or isMaReversal > 0):
@@ -482,15 +495,15 @@
                                 saveDictionary,
                                 chartPattern=respChartPattern,
                                 daysToLookback=insideBarToLookback,
                             )
                     if isInsideBar ==0:
                         return returnLegibleData(f"isInsideBar:{isInsideBar}")
 
-                if not (isLorentzian or (isInsideBar !=0) or isBuyingTrendline or isIpoBase or isNR or isVCP or isVSA):
+                if not (isLorentzian or (isInsideBar !=0) or isBuyingTrendline or isIpoBase or isNR or isVCP or isVSA or isMinerviniVCP):
                     isMomentum = screener.validateMomentum(
                         processedData, screeningDictionary, saveDictionary
                     )
                     if executeOption == 6 and reversalOption ==3 and not isMomentum:
                         return returnLegibleData(f"executeOption:{executeOption},reversalOption:{reversalOption},isMomentum:{isMomentum}")
 
                 with hostRef.processingResultsCounter.get_lock():
@@ -537,17 +550,19 @@
                                                                 or (reversalOption == 9 and hasRisingRSIReversal)
                                                                 or (reversalOption == 10 and hasRSIMAReversal)
                                                                 ))
                         or ((executeOption == 7) and ((respChartPattern < 3 and isInsideBar > 0) 
                                                                   or (isConfluence)
                                                                   or (isIpoBase and newlyListedOnly and not respChartPattern < 3)
                                                                   or (isVCP)
-                                                                  or (isBuyingTrendline))
+                                                                  or (isBuyingTrendline)
                                                                   or (respChartPattern == 6 and hasBbandsSqz)
                                                                   or (respChartPattern == 7 and isCandlePattern))
+                                                                  or (respChartPattern == 8 and isMinerviniVCP)
+                                                                  or (respChartPattern == 9 and hasMASignalFilter))
                         or (executeOption == 8 and isValidCci)
                         or (executeOption == 9 and hasMinVolumeRatio)
                         or (executeOption == 10 and isPriceRisingByAtLeast2Percent)
                         or (executeOption == 11 and isShortTermBullish)
                         or (executeOption in [12,13,14,15,16,17,18,19,20,23,24,25,27,28,30,31,32] and isValidityCheckMet)
                         or (executeOption == 21 and (mfiStake > 0 and reversalOption in [3,5]))
                         or (executeOption == 21 and (mfiStake < 0 and reversalOption in [6,7]))
```

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1479,15 +1479,15 @@
                         colorText.BOLD
                         + colorText.WARN
                         + "\n[+] Enter Percentage within which all MA/EMAs should be (Ideal: 1-2%)? (Default=2): "
                         + colorText.END
                     ) or "2"
                 )
                 return (resp, percent / 100.0)
-            if resp >= 0 and resp <= 7:
+            if resp >= 0 and resp <= 9:
                 return resp, 0
             raise ValueError
         except ValueError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
             input(
                 colorText.BOLD
                 + colorText.FAIL
@@ -1609,11 +1609,11 @@
     def alertSound(beeps=3, delay=0.2):
         for i in range(beeps):
             OutputControls().printOutput("\a")
             sleep(delay)
     
     def getMaxColumnWidths(df):
         columnWidths = [None]
-        addnlColumnWidths = [40 if (x in ["Trend(22Prds)"] or "-Pd" in x) else (20 if (x in ["Pattern"]) else None) for x in df.columns]
+        addnlColumnWidths = [40 if (x in ["Trend(22Prds)"] or "-Pd" in x) else (20 if (x in ["Pattern"]) else ((25 if (x in ["MA-Signal"]) else None))) for x in df.columns]
         columnWidths.extend(addnlColumnWidths)
         columnWidths = columnWidths[:-1]
         return columnWidths
```

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/classes/keys.py` & `pkscreener-0.45.20240527.418/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/courbd.ttf` & `pkscreener-0.45.20240527.418/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener/globals.py` & `pkscreener-0.45.20240527.418/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     level2_X_MenuDict,
     level3_X_ChartPattern_MenuDict,
     level3_X_PopularStocks_MenuDict,
     level3_X_Reversal_MenuDict,
     level4_X_Lorenzian_MenuDict,
     level4_X_ChartPattern_Confluence_MenuDict,
     level4_X_ChartPattern_BBands_SQZ_MenuDict,
+    level4_X_ChartPattern_MASignalMenuDict,
     menus,
     MAX_SUPPORTED_MENU_OPTION,
     MAX_MENU_OPTION,
     PIPED_SCANNERS,
     PREDEFINED_SCAN_MENU_KEYS
 )
 from pkscreener.classes.OtaUpdater import OTAUpdater
@@ -1053,46 +1054,47 @@
                 else:
                     (
                         respChartPattern,
                         insideBarToLookback,
                     ) = Utility.tools.promptChartPatterns(selectedMenu)
                 if maLength == 0:
                     maLength = Utility.tools.promptChartPatternSubMenu(selectedMenu, respChartPattern)
-            elif respChartPattern in [0, 4, 5, 6, 7]:
+            elif respChartPattern in [0, 4, 5, 6, 7, 8, 9]:
                 insideBarToLookback = 0
-                if respChartPattern == 6:
+                if respChartPattern == 6 or respChartPattern == 9:
                     if len(options) >= 5:
                         if str(options[4]).isnumeric():
                             maLength = int(options[4])
                         elif str(options[4]).upper() == "D":
-                            maLength = 1 # Bollinger Bands Squeeze-Buy
+                            maLength = 1 if respChartPattern == 6 else 6 # Bollinger Bands Squeeze-Buy or MA-Support
                     elif defaultAnswer == "Y" and user is not None:
                         # bot mode
-                        maLength = 4 # Bollinger Bands Squeeze- Any/All
+                        maLength = 4 if respChartPattern == 6 else 6 # Bollinger Bands Squeeze- Any/All or MA-Support
                     else:
                         maLength = Utility.tools.promptChartPatternSubMenu(selectedMenu,respChartPattern)
             else:
                 (
                     respChartPattern,
                     insideBarToLookback,
                 ) = Utility.tools.promptChartPatterns(selectedMenu)
         else:
             respChartPattern, insideBarToLookback = Utility.tools.promptChartPatterns(
                 selectedMenu
             )
-            if maLength == 0 and respChartPattern in [1, 2, 3, 6]:
+            if maLength == 0 and respChartPattern in [1, 2, 3, 6, 9]:
                 maLength = Utility.tools.promptChartPatternSubMenu(selectedMenu, respChartPattern)
         if (
             respChartPattern is None
             or insideBarToLookback is None
             or respChartPattern == 0
-            or (maLength == 0 and respChartPattern in [1, 2, 3, 6])
+            or (maLength == 0 and respChartPattern in [1, 2, 3, 6, 9])
         ):
             return None, None
         else:
+            userPassedArgs.maxdisplayresults = 2000 if respChartPattern in [3,4,5,8,9] else userPassedArgs.maxdisplayresults
             selectedChoice["3"] = str(respChartPattern)
             selectedChoice["4"] = str(insideBarToLookback) if (respChartPattern in [1, 2, 3] and (userPassedArgs is not None and userPassedArgs.pipedmenus is not None)) else str(maLength)
             selectedChoice["5"] = str(maLength) if (respChartPattern in [1, 2, 3] and (userPassedArgs is not None and userPassedArgs.pipedmenus is not None)) else ""
     if executeOption == 8:
         if len(options) >= 5:
             if "".join(str(options[3]).split(".")).isdecimal():
                 minRSI = int(options[3])
@@ -2001,14 +2003,19 @@
                 + f'>{level4_X_ChartPattern_Confluence_MenuDict[selectedChoice["4"]].strip()}'
             )
             elif len(selectedChoice) >= 5 and selectedChoice["3"] == "6":
                 menuChoiceHierarchy = (
                 menuChoiceHierarchy
                 + f'>{level4_X_ChartPattern_BBands_SQZ_MenuDict[selectedChoice["4"]].strip()}'
             )
+            elif len(selectedChoice) >= 5 and selectedChoice["3"] == "9":
+                menuChoiceHierarchy = (
+                menuChoiceHierarchy
+                + f'>{level4_X_ChartPattern_MASignalMenuDict[selectedChoice["4"]].strip()}'
+            )
         elif selectedChoice["2"] == "21":
             menuChoiceHierarchy = (
                 menuChoiceHierarchy
                 + f'>{level3_X_PopularStocks_MenuDict[selectedChoice["3"]].strip()}'
             )
         intraday = "(Intraday)" if (userPassedArgs is not None and userPassedArgs.intraday) or configManager.isIntradayConfig() else ""
         menuChoiceHierarchy = f"{menuChoiceHierarchy}{intraday}"
```

### Comparing `pkscreener-0.45.20240527.417/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240527.418/pkscreener/pkscreener.ini`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 atrtrailingstopsensitivity = 1.0
 backtestperiod = 120
 backtestperiodfactor = 1
 cachestockdata = y
 calculatersiintraday = n
 daystolookback = 22
 defaultindex = 12
-defaultmonitoroptions = X:12:9:2.5:~X:12:28:~X:12:23:~|{1}X:0:23:>|X:0:27:>|X:0:31:~|{2}X:0:31:~|{3}X:0:27:~X:12:7:3:.01:1:~|{5}X:0:5:0:40:~X:12:7:6:1:~X:12:11:~X:12:12:i 5m~X:12:17:~X:12:24:~X:12:6:7:1:~X:12:6:3:~X:12:6:8:~X:12:6:9:~X:12:6:10:1:~X:12:7:3:.02:1:~X:12:13:i 1m~X:12:2:~|{1}X:0:29:
+defaultmonitoroptions = X:12:9:2.5~X:12:23~X:12:28~X:12:31~|{1}X:0:23:>|X:0:27:>|X:0:31:~|{2}X:0:31:~|{3}X:0:27:~X:12:7:3:.01:1~|{5}X:0:5:0:35:~X:12:7:6:1~X:12:11:~X:12:12:i 5m~X:12:17~X:12:24~X:12:6:7:1~X:12:6:3~X:12:6:8~X:12:6:9~X:12:2:>|X:12:7:8:>|X:12:7:9:1:1:~X:12:6:10:1~X:12:7:3:.02:1~X:12:13:i 1m~X:12:2~|{1}X:0:29:
 duration = 1d
 enableportfoliocalculations = n
 generaltimeout = 2.0
 logsenabled = n
 longtimeout = 4.0
 maxbacktestwindow = 30
-maxdashboardwidgetsperrow = 5
+maxdashboardwidgetsperrow = 7
 maxnetworkretrycount = 10
 maxnumresultrowsinmonitor = 3
 morninganalysiscandlenumber = 25
 morninganalysiscandleduration = 1m
 onlystagetwostocks = y
 period = 1y
 showpaststrategydata = n
```

### Comparing `pkscreener-0.45.20240527.417/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240527.418/pkscreener/pkscreenerbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,18 +574,19 @@
     keyboard = [inlineMenus]
     reply_markup = InlineKeyboardMarkup(keyboard)
     return reply_markup
 
 
 async def sendUpdatedMenu(menuText, update: Update, context, reply_markup, replaceWhiteSpaces=True):
     try:
+        menuText.replace("     ", "").replace("    ", "").replace("\t", "").replace(colorText.FAIL,"").replace(colorText.END,"") if replaceWhiteSpaces else menuText
         if update.callback_query.message.text == menuText:
             menuText = f"{PKDateUtilities.currentDateTime()}:\n{menuText}"
         await update.callback_query.edit_message_text(
-            text=menuText.replace("     ", "").replace("    ", "").replace("\t", "").replace(colorText.FAIL,"").replace(colorText.END,"") if replaceWhiteSpaces else menuText,
+            text=menuText,
             parse_mode="HTML",
             reply_markup=reply_markup,
         )
     except Exception as e:# pragma: no cover
         logger.log(e)
         await start(update, context)
```

### Comparing `pkscreener-0.45.20240527.417/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240527.418/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240527.418/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240527.417
+Version: 0.45.20240527.418
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240527.417.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240527.418.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240526.416/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240527.417/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240527.418/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.417/setup.py` & `pkscreener-0.45.20240527.418/setup.py`

 * *Files identical despite different names*

