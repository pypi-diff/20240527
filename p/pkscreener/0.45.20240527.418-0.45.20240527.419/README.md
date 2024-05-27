# Comparing `tmp/pkscreener-0.45.20240527.418.tar.gz` & `tmp/pkscreener-0.45.20240527.419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240527.418.tar", last modified: Mon May 27 21:27:14 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240527.419.tar", last modified: Mon May 27 21:54:59 2024, max compression
```

## Comparing `pkscreener-0.45.20240527.418.tar` & `pkscreener-0.45.20240527.419.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:27:14.356891 pkscreener-0.45.20240527.418/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/LICENSE-Others
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-27 21:27:14.356891 pkscreener-0.45.20240527.418/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:27:14.348892 pkscreener-0.45.20240527.418/pkscreener/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:27:14.356891 pkscreener-0.45.20240527.418/pkscreener/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/ArtTexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Barometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/CandlePatterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)    33678 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/MarketMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/MarketStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    46722 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/MenuOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/OtaUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PKScanRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PKScheduledTaskProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PKScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PKSpreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PKTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Pktalib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/PortfolioXRay.py
--rw-r--r--   0 runner    (1001) docker     (127)   158196 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/ScreeningStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    56970 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/StockScreener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/UserMenuChoicesHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    85524 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/WorkflowManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 21:27:08.000000 pkscreener-0.45.20240527.418/pkscreener/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/classes/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/courbd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   145709 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/pkscreener.ini
--rw-r--r--   0 runner    (1001) docker     (127)    53279 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/pkscreenerbot.py
--rw-r--r--   0 runner    (1001) docker     (127)    33987 2024-05-27 21:25:45.000000 pkscreener-0.45.20240527.418/pkscreener/pkscreenercli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:27:14.352892 pkscreener-0.45.20240527.418/pkscreener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 21:27:14.000000 pkscreener-0.45.20240527.418/pkscreener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 21:27:14.356891 pkscreener-0.45.20240527.418/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-27 21:25:46.000000 pkscreener-0.45.20240527.418/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:54:59.131188 pkscreener-0.45.20240527.419/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/LICENSE-Others
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-27 21:54:59.131188 pkscreener-0.45.20240527.419/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:54:59.127188 pkscreener-0.45.20240527.419/pkscreener/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:54:59.131188 pkscreener-0.45.20240527.419/pkscreener/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/ArtTexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Barometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/CandlePatterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33678 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/MarketMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/MarketStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46722 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/MenuOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/OtaUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PKScanRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PKScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PKSpreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PKTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Pktalib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PortfolioXRay.py
+-rw-r--r--   0 runner    (1001) docker     (127)   158334 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/ScreeningStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56970 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/StockScreener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85524 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/WorkflowManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 21:54:52.000000 pkscreener-0.45.20240527.419/pkscreener/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/courbd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   145709 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/pkscreener.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    53279 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/pkscreenerbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33987 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/pkscreenercli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:54:59.127188 pkscreener-0.45.20240527.419/pkscreener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 21:54:59.131188 pkscreener-0.45.20240527.419/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/setup.py
```

### Comparing `pkscreener-0.45.20240527.418/LICENSE` & `pkscreener-0.45.20240527.419/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/LICENSE-Others` & `pkscreener-0.45.20240527.419/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/PKG-INFO` & `pkscreener-0.45.20240527.419/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240527.418
+Version: 0.45.20240527.419
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240527.418.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240527.419.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240527.418/README.md` & `pkscreener-0.45.20240527.419/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240527.418/pkscreener/__init__.py` & `pkscreener-0.45.20240527.419/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/ScreeningStatistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -6985,2904 +6985,2912 @@
 0001b480: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
 0001b490: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
 0001b4a0: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
 0001b4b0: 6174 612e 6865 6164 2832 290a 2020 2020  ata.head(2).    
 0001b4c0: 2020 2020 6966 206c 656e 2872 6563 656e      if len(recen
 0001b4d0: 7429 203c 2032 3a0a 2020 2020 2020 2020  t) < 2:.        
 0001b4e0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0001b4f0: 0a20 2020 2020 2020 2069 7335 3044 4d41  .        is50DMA
-0001b500: 5570 5472 656e 6420 3d20 2872 6563 656e  UpTrend = (recen
-0001b510: 745b 2253 4d41 225d 2e69 6c6f 635b 305d  t["SMA"].iloc[0]
-0001b520: 203e 2072 6563 656e 745b 2253 4d41 225d   > recent["SMA"]
-0001b530: 2e69 6c6f 635b 315d 290a 2020 2020 2020  .iloc[1]).      
-0001b540: 2020 6973 3530 444d 4144 6f77 6e54 7265    is50DMADownTre
-0001b550: 6e64 203d 2028 7265 6365 6e74 5b22 534d  nd = (recent["SM
-0001b560: 4122 5d2e 696c 6f63 5b30 5d20 3c20 7265  A"].iloc[0] < re
-0001b570: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
-0001b580: 5b31 5d29 0a20 2020 2020 2020 2069 7332  [1]).        is2
-0001b590: 3044 4d41 4372 6f73 736f 7665 7235 3044  0DMACrossover50D
-0001b5a0: 4d41 203d 2028 7265 6365 6e74 5b22 5353  MA = (recent["SS
-0001b5b0: 4d41 3230 225d 2e69 6c6f 635b 305d 203e  MA20"].iloc[0] >
-0001b5c0: 3d20 7265 6365 6e74 5b22 534d 4122 5d2e  = recent["SMA"].
-0001b5d0: 696c 6f63 5b30 5d29 2061 6e64 205c 0a20  iloc[0]) and \. 
-0001b5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b5f0: 2020 2020 2020 2020 2020 2028 7265 6365             (rece
-0001b600: 6e74 5b22 5353 4d41 3230 225d 2e69 6c6f  nt["SSMA20"].ilo
-0001b610: 635b 315d 203c 3d20 7265 6365 6e74 5b22  c[1] <= recent["
-0001b620: 534d 4122 5d2e 696c 6f63 5b31 5d29 0a20  SMA"].iloc[1]). 
-0001b630: 2020 2020 2020 2069 7335 3044 4d41 4372         is50DMACr
-0001b640: 6f73 736f 7665 7232 3030 444d 4120 3d20  ossover200DMA = 
-0001b650: 2872 6563 656e 745b 2253 4d41 225d 2e69  (recent["SMA"].i
-0001b660: 6c6f 635b 305d 203e 3d20 7265 6365 6e74  loc[0] >= recent
-0001b670: 5b22 4c4d 4122 5d2e 696c 6f63 5b30 5d29  ["LMA"].iloc[0])
-0001b680: 2061 6e64 205c 0a20 2020 2020 2020 2020   and \.         
-0001b690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b6a0: 2020 2028 7265 6365 6e74 5b22 534d 4122     (recent["SMA"
-0001b6b0: 5d2e 696c 6f63 5b31 5d20 3c3d 2072 6563  ].iloc[1] <= rec
-0001b6c0: 656e 745b 224c 4d41 225d 2e69 6c6f 635b  ent["LMA"].iloc[
-0001b6d0: 315d 290a 2020 2020 2020 2020 6973 476f  1]).        isGo
-0001b6e0: 6c64 656e 4372 6f73 734f 7665 7220 3d20  ldenCrossOver = 
-0001b6f0: 6973 3230 444d 4143 726f 7373 6f76 6572  is20DMACrossover
-0001b700: 3530 444d 4120 6f72 2069 7335 3044 4d41  50DMA or is50DMA
-0001b710: 4372 6f73 736f 7665 7232 3030 444d 410a  Crossover200DMA.
-0001b720: 2020 2020 2020 2020 6973 3530 444d 4143          is50DMAC
-0001b730: 726f 7373 6f76 6572 3230 3044 4d41 446f  rossover200DMADo
-0001b740: 776e 203d 2028 7265 6365 6e74 5b22 534d  wn = (recent["SM
-0001b750: 4122 5d2e 696c 6f63 5b30 5d20 3c3d 2072  A"].iloc[0] <= r
-0001b760: 6563 656e 745b 224c 4d41 225d 2e69 6c6f  ecent["LMA"].ilo
-0001b770: 635b 305d 2920 616e 6420 5c0a 2020 2020  c[0]) and \.    
-0001b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b790: 2020 2020 2020 2020 2872 6563 656e 745b          (recent[
-0001b7a0: 2253 4d41 225d 2e69 6c6f 635b 315d 203e  "SMA"].iloc[1] >
-0001b7b0: 3d20 7265 6365 6e74 5b22 4c4d 4122 5d2e  = recent["LMA"].
-0001b7c0: 696c 6f63 5b31 5d29 0a20 2020 2020 2020  iloc[1]).       
-0001b7d0: 2069 7332 3044 4d41 4372 6f73 736f 7665   is20DMACrossove
-0001b7e0: 7235 3044 4d41 446f 776e 203d 2028 7265  r50DMADown = (re
-0001b7f0: 6365 6e74 5b22 5353 4d41 3230 225d 2e69  cent["SSMA20"].i
-0001b800: 6c6f 635b 305d 203c 3d20 7265 6365 6e74  loc[0] <= recent
-0001b810: 5b22 534d 4122 5d2e 696c 6f63 5b30 5d29  ["SMA"].iloc[0])
-0001b820: 2061 6e64 205c 0a20 2020 2020 2020 2020   and \.         
-0001b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b840: 2020 2028 7265 6365 6e74 5b22 5353 4d41     (recent["SSMA
-0001b850: 3230 225d 2e69 6c6f 635b 315d 203e 3d20  20"].iloc[1] >= 
-0001b860: 7265 6365 6e74 5b22 534d 4122 5d2e 696c  recent["SMA"].il
-0001b870: 6f63 5b31 5d29 0a20 2020 2020 2020 2069  oc[1]).        i
-0001b880: 7344 6561 6443 726f 7373 4f76 6572 203d  sDeadCrossOver =
-0001b890: 2069 7332 3044 4d41 4372 6f73 736f 7665   is20DMACrossove
-0001b8a0: 7235 3044 4d41 446f 776e 206f 7220 6973  r50DMADown or is
-0001b8b0: 3530 444d 4143 726f 7373 6f76 6572 3230  50DMACrossover20
-0001b8c0: 3044 4d41 446f 776e 0a20 2020 2020 2020  0DMADown.       
-0001b8d0: 2064 6561 6478 4f76 6572 5465 7874 203d   deadxOverText =
-0001b8e0: 2066 2744 6561 6443 726f 7373 6f76 6572   f'DeadCrossover
-0001b8f0: 7b22 2832 3029 2220 6966 2069 7332 3044  {"(20)" if is20D
-0001b900: 4d41 4372 6f73 736f 7665 7235 3044 4d41  MACrossover50DMA
-0001b910: 446f 776e 2065 6c73 6520 2822 2835 3029  Down else ("(50)
-0001b920: 2220 6966 2069 7335 3044 4d41 4372 6f73  " if is50DMACros
-0001b930: 736f 7665 7232 3030 444d 4144 6f77 6e20  sover200DMADown 
-0001b940: 656c 7365 2022 2229 7d27 0a20 2020 2020  else "")}'.     
-0001b950: 2020 2067 6f6c 6465 6e78 4f76 6572 5465     goldenxOverTe
-0001b960: 7874 203d 2066 2747 6f6c 6465 6e43 726f  xt = f'GoldenCro
-0001b970: 7373 6f76 6572 7b22 2832 3029 2220 6966  ssover{"(20)" if
-0001b980: 2069 7332 3044 4d41 4372 6f73 736f 7665   is20DMACrossove
-0001b990: 7235 3044 4d41 2065 6c73 6520 2822 2835  r50DMA else ("(5
-0001b9a0: 3029 2220 6966 2069 7335 3044 4d41 4372  0)" if is50DMACr
-0001b9b0: 6f73 736f 7665 7232 3030 444d 4120 656c  ossover200DMA el
-0001b9c0: 7365 2022 2229 7d27 0a20 2020 2020 2020  se "")}'.       
-0001b9d0: 2069 7335 3044 4d41 203d 2028 7265 6365   is50DMA = (rece
-0001b9e0: 6e74 5b22 534d 4122 5d2e 696c 6f63 5b30  nt["SMA"].iloc[0
-0001b9f0: 5d20 3c3d 2072 6563 656e 745b 2243 6c6f  ] <= recent["Clo
-0001ba00: 7365 225d 2e69 6c6f 635b 305d 290a 2020  se"].iloc[0]).  
-0001ba10: 2020 2020 2020 6973 3230 3044 4d41 203d        is200DMA =
-0001ba20: 2028 7265 6365 6e74 5b22 4c4d 4122 5d2e   (recent["LMA"].
-0001ba30: 696c 6f63 5b30 5d20 3c3d 2072 6563 656e  iloc[0] <= recen
-0001ba40: 745b 2243 6c6f 7365 225d 2e69 6c6f 635b  t["Close"].iloc[
-0001ba50: 305d 290a 2020 2020 2020 2020 6b65 7931  0]).        key1
-0001ba60: 203d 2022 534d 4122 0a20 2020 2020 2020   = "SMA".       
-0001ba70: 206b 6579 3220 3d20 224c 4d41 220a 2020   key2 = "LMA".  
-0001ba80: 2020 2020 2020 6966 2069 7332 3044 4d41        if is20DMA
-0001ba90: 4372 6f73 736f 7665 7235 3044 4d41 206f  Crossover50DMA o
-0001baa0: 7220 6973 3230 444d 4143 726f 7373 6f76  r is20DMACrossov
-0001bab0: 6572 3530 444d 4144 6f77 6e3a 0a20 2020  er50DMADown:.   
-0001bac0: 2020 2020 2020 2020 206b 6579 3120 3d20           key1 = 
-0001bad0: 2253 534d 4132 3022 0a20 2020 2020 2020  "SSMA20".       
-0001bae0: 2020 2020 206b 6579 3220 3d20 2253 4d41       key2 = "SMA
-0001baf0: 220a 2020 2020 2020 2020 6469 6666 6572  ".        differ
-0001bb00: 656e 6365 203d 2072 6f75 6e64 2828 7265  ence = round((re
-0001bb10: 6365 6e74 5b6b 6579 315d 2e69 6c6f 635b  cent[key1].iloc[
-0001bb20: 305d 202d 2072 6563 656e 745b 6b65 7932  0] - recent[key2
-0001bb30: 5d2e 696c 6f63 5b30 5d29 0a20 2020 2020  ].iloc[0]).     
-0001bb40: 2020 2020 2020 2020 2020 202f 2072 6563             / rec
-0001bb50: 656e 745b 2243 6c6f 7365 225d 2e69 6c6f  ent["Close"].ilo
-0001bb60: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
-0001bb70: 2020 2020 202a 2031 3030 2c0a 2020 2020       * 100,.    
-0001bb80: 2020 2020 2020 2020 2020 2020 322c 0a20              2,. 
-0001bb90: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0001bba0: 2020 2020 2073 6176 6544 6963 745b 2243       saveDict["C
-0001bbb0: 6f6e 6644 4d41 4469 6666 6572 656e 6365  onfDMADifference
-0001bbc0: 225d 203d 2064 6966 6665 7265 6e63 650a  "] = difference.
-0001bbd0: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-0001bbe0: 6374 5b22 436f 6e66 444d 4144 6966 6665  ct["ConfDMADiffe
-0001bbf0: 7265 6e63 6522 5d20 3d20 6469 6666 6572  rence"] = differ
-0001bc00: 656e 6365 0a20 2020 2020 2020 2073 6176  ence.        sav
-0001bc10: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
-0001bc20: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
-0001bc30: 7363 7265 656e 4469 6374 2c73 6176 6544  screenDict,saveD
-0001bc40: 6963 742c 224d 412d 5369 676e 616c 2229  ict,"MA-Signal")
-0001bc50: 0a20 2020 2020 2020 2023 2064 6966 6665  .        # diffe
-0001bc60: 7265 6e63 6520 3d20 6162 7328 6469 6666  rence = abs(diff
-0001bc70: 6572 656e 6365 290a 2020 2020 2020 2020  erence).        
-0001bc80: 636f 6e66 5465 7874 203d 2066 227b 676f  confText = f"{go
-0001bc90: 6c64 656e 784f 7665 7254 6578 7420 6966  ldenxOverText if
-0001bca0: 2069 7347 6f6c 6465 6e43 726f 7373 4f76   isGoldenCrossOv
-0001bcb0: 6572 2065 6c73 6520 2864 6561 6478 4f76  er else (deadxOv
-0001bcc0: 6572 5465 7874 2069 6620 6973 4465 6164  erText if isDead
-0001bcd0: 4372 6f73 734f 7665 7220 656c 7365 2028  CrossOver else (
-0001bce0: 2743 6f6e 662e 5570 2720 6966 2069 7335  'Conf.Up' if is5
-0001bcf0: 3044 4d41 5570 5472 656e 6420 656c 7365  0DMAUpTrend else
-0001bd00: 2028 2743 6f6e 662e 446f 776e 2720 6966   ('Conf.Down' if
-0001bd10: 2069 7335 3044 4d41 446f 776e 5472 656e   is50DMADownTren
-0001bd20: 6420 656c 7365 2028 2735 3044 4d41 2720  d else ('50DMA' 
-0001bd30: 6966 2069 7335 3044 4d41 2065 6c73 6520  if is50DMA else 
-0001bd40: 2827 3230 3044 4d41 2720 6966 2069 7332  ('200DMA' if is2
-0001bd50: 3030 444d 4120 656c 7365 2027 556e 6b6e  00DMA else 'Unkn
-0001bd60: 6f77 6e27 2929 2929 297d 220a 2020 2020  own')))))}".    
-0001bd70: 2020 2020 6966 2061 6273 2872 6563 656e      if abs(recen
-0001bd80: 745b 6b65 7931 5d2e 696c 6f63 5b30 5d20  t[key1].iloc[0] 
-0001bd90: 2d20 7265 6365 6e74 5b6b 6579 325d 2e69  - recent[key2].i
-0001bda0: 6c6f 635b 305d 2920 3c3d 2028 0a20 2020  loc[0]) <= (.   
-0001bdb0: 2020 2020 2020 2020 2072 6563 656e 745b           recent[
-0001bdc0: 6b65 7931 5d2e 696c 6f63 5b30 5d20 2a20  key1].iloc[0] * 
-0001bdd0: 7065 7263 656e 7461 6765 0a20 2020 2020  percentage.     
-0001bde0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-0001bdf0: 2020 6966 2072 6563 656e 745b 6b65 7931    if recent[key1
-0001be00: 5d2e 696c 6f63 5b30 5d20 3e3d 2072 6563  ].iloc[0] >= rec
-0001be10: 656e 745b 6b65 7932 5d2e 696c 6f63 5b30  ent[key2].iloc[0
-0001be20: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-0001be30: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
-0001be40: 412d 5369 676e 616c 225d 203d 2028 0a20  A-Signal"] = (. 
-0001be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be60: 2020 2073 6176 6564 5b30 5d20 0a20 2020     saved[0] .   
-0001be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be80: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-0001be90: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-0001bea0: 2020 2020 2020 2b20 2863 6f6c 6f72 5465        + (colorTe
-0001beb0: 7874 2e47 5245 454e 2069 6620 6973 3530  xt.GREEN if is50
-0001bec0: 444d 4155 7054 7265 6e64 2065 6c73 6520  DMAUpTrend else 
-0001bed0: 2863 6f6c 6f72 5465 7874 2e46 4149 4c20  (colorText.FAIL 
-0001bee0: 6966 2069 7335 3044 4d41 446f 776e 5472  if is50DMADownTr
-0001bef0: 656e 6420 656c 7365 2063 6f6c 6f72 5465  end else colorTe
-0001bf00: 7874 2e57 4152 4e29 290a 2020 2020 2020  xt.WARN)).      
-0001bf10: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001bf20: 6622 7b63 6f6e 6654 6578 747d 2028 7b64  f"{confText} ({d
-0001bf30: 6966 6665 7265 6e63 657d 2529 220a 2020  ifference}%)".  
-0001bf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf50: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
-0001bf60: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-0001bf70: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0001bf80: 2020 2020 7361 7665 4469 6374 5b22 4d41      saveDict["MA
-0001bf90: 2d53 6967 6e61 6c22 5d20 3d20 7361 7665  -Signal"] = save
-0001bfa0: 645b 315d 202b 2066 227b 636f 6e66 5465  d[1] + f"{confTe
-0001bfb0: 7874 7d20 287b 6469 6666 6572 656e 6365  xt} ({difference
-0001bfc0: 7d25 2922 0a20 2020 2020 2020 2020 2020  }%)".           
-0001bfd0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001bfe0: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-0001bff0: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-0001c000: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0001c010: 2020 2020 2020 2073 6176 6564 5b30 5d20         saved[0] 
-0001c020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c030: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001c040: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
-0001c050: 2020 2020 2020 2020 2020 2b20 2863 6f6c            + (col
-0001c060: 6f72 5465 7874 2e47 5245 454e 2069 6620  orText.GREEN if 
-0001c070: 6973 3530 444d 4155 7054 7265 6e64 2065  is50DMAUpTrend e
-0001c080: 6c73 6520 2863 6f6c 6f72 5465 7874 2e46  lse (colorText.F
-0001c090: 4149 4c20 6966 2069 7335 3044 4d41 446f  AIL if is50DMADo
-0001c0a0: 776e 5472 656e 6420 656c 7365 2063 6f6c  wnTrend else col
-0001c0b0: 6f72 5465 7874 2e57 4152 4e29 290a 2020  orText.WARN)).  
-0001c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c0d0: 2020 2b20 6622 7b63 6f6e 6654 6578 747d    + f"{confText}
-0001c0e0: 2028 7b64 6966 6665 7265 6e63 657d 2529   ({difference}%)
-0001c0f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0001c100: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001c110: 742e 454e 440a 2020 2020 2020 2020 2020  t.END.          
-0001c120: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001c130: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-0001c140: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
-0001c150: 7361 7665 645b 315d 202b 2066 227b 636f  saved[1] + f"{co
-0001c160: 6e66 5465 7874 7d20 287b 6469 6666 6572  nfText} ({differ
-0001c170: 656e 6365 7d25 2922 0a20 2020 2020 2020  ence}%)".       
-0001c180: 2020 2020 2072 6574 7572 6e20 636f 6e66       return conf
-0001c190: 4669 6c74 6572 203d 3d20 3320 6f72 205c  Filter == 3 or \
-0001c1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c1b0: 2028 636f 6e66 4669 6c74 6572 203d 3d20   (confFilter == 
-0001c1c0: 3120 616e 6420 2869 7335 3044 4d41 5570  1 and (is50DMAUp
-0001c1d0: 5472 656e 6420 6f72 2028 6973 476f 6c64  Trend or (isGold
-0001c1e0: 656e 4372 6f73 734f 7665 7220 6f72 2027  enCrossOver or '
-0001c1f0: 5570 2720 696e 2063 6f6e 6654 6578 7429  Up' in confText)
-0001c200: 2929 206f 7220 5c0a 2020 2020 2020 2020  )) or \.        
-0001c210: 2020 2020 2020 2020 2863 6f6e 6646 696c          (confFil
-0001c220: 7465 7220 3d3d 2032 2061 6e64 2028 6973  ter == 2 and (is
-0001c230: 3530 444d 4144 6f77 6e54 7265 6e64 206f  50DMADownTrend o
-0001c240: 7220 6973 4465 6164 4372 6f73 734f 7665  r isDeadCrossOve
-0001c250: 7220 6f72 2027 446f 776e 2720 696e 2063  r or 'Down' in c
-0001c260: 6f6e 6654 6578 7429 290a 2020 2020 2020  onfText)).      
-0001c270: 2020 2320 4d61 7962 6520 7468 6520 6469    # Maybe the di
-0001c280: 6666 6572 656e 6365 2069 7320 6e6f 7420  fference is not 
-0001c290: 7769 7468 696e 2074 6865 2072 616e 6765  within the range
-0001c2a0: 2c20 6275 7420 7765 2764 2073 7469 6c6c  , but we'd still
-0001c2b0: 206c 696b 6520 746f 206b 6565 7020 7468   like to keep th
-0001c2c0: 6520 7374 6f63 6b20 696e 0a20 2020 2020  e stock in.     
-0001c2d0: 2020 2023 2074 6865 206c 6973 7420 6966     # the list if
-0001c2e0: 2069 7427 7320 6120 676f 6c64 656e 2063   it's a golden c
-0001c2f0: 726f 7373 6f76 6572 206f 7220 6465 6164  rossover or dead
-0001c300: 2063 726f 7373 6f76 6572 0a20 2020 2020   crossover.     
-0001c310: 2020 2069 6620 6973 476f 6c64 656e 4372     if isGoldenCr
-0001c320: 6f73 734f 7665 7220 6f72 2069 7344 6561  ossOver or isDea
-0001c330: 6443 726f 7373 4f76 6572 3a0a 2020 2020  dCrossOver:.    
-0001c340: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-0001c350: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-0001c360: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0001c370: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-0001c380: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0001c390: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001c3a0: 742e 424f 4c44 0a20 2020 2020 2020 2020  t.BOLD.         
-0001c3b0: 2020 2020 2020 2020 2020 202b 2028 636f             + (co
-0001c3c0: 6c6f 7254 6578 742e 4752 4545 4e20 6966  lorText.GREEN if
-0001c3d0: 2069 7335 3044 4d41 5570 5472 656e 6420   is50DMAUpTrend 
-0001c3e0: 656c 7365 2028 636f 6c6f 7254 6578 742e  else (colorText.
-0001c3f0: 4641 494c 2069 6620 6973 3530 444d 4144  FAIL if is50DMAD
-0001c400: 6f77 6e54 7265 6e64 2065 6c73 6520 636f  ownTrend else co
-0001c410: 6c6f 7254 6578 742e 5741 524e 2929 0a20  lorText.WARN)). 
-0001c420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c430: 2020 202b 2066 227b 636f 6e66 5465 7874     + f"{confText
-0001c440: 7d20 287b 6469 6666 6572 656e 6365 7d25  } ({difference}%
-0001c450: 2922 0a20 2020 2020 2020 2020 2020 2020  )".             
-0001c460: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-0001c470: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
-0001c480: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001c490: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
-0001c4a0: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
-0001c4b0: 6564 5b31 5d20 2b20 6622 7b63 6f6e 6654  ed[1] + f"{confT
-0001c4c0: 6578 747d 2028 7b64 6966 6665 7265 6e63  ext} ({differenc
-0001c4d0: 657d 2529 220a 2020 2020 2020 2020 2020  e}%)".          
-0001c4e0: 2020 7265 7475 726e 2063 6f6e 6646 696c    return confFil
-0001c4f0: 7465 7220 3d3d 2033 206f 7220 5c0a 2020  ter == 3 or \.  
-0001c500: 2020 2020 2020 2020 2020 2020 2020 2863                (c
-0001c510: 6f6e 6646 696c 7465 7220 3d3d 2031 2061  onfFilter == 1 a
-0001c520: 6e64 2069 7347 6f6c 6465 6e43 726f 7373  nd isGoldenCross
-0001c530: 4f76 6572 2920 6f72 205c 0a20 2020 2020  Over) or \.     
-0001c540: 2020 2020 2020 2020 2020 2028 636f 6e66             (conf
-0001c550: 4669 6c74 6572 203d 3d20 3220 616e 6420  Filter == 2 and 
-0001c560: 6973 4465 6164 4372 6f73 734f 7665 7229  isDeadCrossOver)
-0001c570: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001c580: 4661 6c73 650a 0a20 2020 2023 406d 6561  False..    #@mea
-0001c590: 7375 7265 5f74 696d 650a 2020 2020 2320  sure_time.    # 
-0001c5a0: 5661 6c69 6461 7465 2069 6620 7368 6172  Validate if shar
-0001c5b0: 6520 7072 6963 6573 2061 7265 2063 6f6e  e prices are con
-0001c5c0: 736f 6c69 6461 7469 6e67 0a20 2020 2064  solidating.    d
-0001c5d0: 6566 2076 616c 6964 6174 6543 6f6e 736f  ef validateConso
-0001c5e0: 6c69 6461 7469 6f6e 2873 656c 662c 2064  lidation(self, d
-0001c5f0: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
-0001c600: 6176 6544 6963 742c 2070 6572 6365 6e74  aveDict, percent
-0001c610: 6167 653d 3130 293a 0a20 2020 2020 2020  age=10):.       
-0001c620: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-0001c630: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
-0001c640: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001c650: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-0001c660: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-0001c670: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
-0001c680: 2064 6174 612e 6669 6c6c 6e61 2830 290a   data.fillna(0).
-0001c690: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001c6a0: 6174 612e 7265 706c 6163 6528 5b6e 702e  ata.replace([np.
-0001c6b0: 696e 662c 202d 6e70 2e69 6e66 5d2c 2030  inf, -np.inf], 0
-0001c6c0: 290a 2020 2020 2020 2020 6863 203d 2064  ).        hc = d
-0001c6d0: 6174 612e 6465 7363 7269 6265 2829 5b22  ata.describe()["
-0001c6e0: 436c 6f73 6522 5d5b 226d 6178 225d 0a20  Close"]["max"]. 
-0001c6f0: 2020 2020 2020 206c 6320 3d20 6461 7461         lc = data
-0001c700: 2e64 6573 6372 6962 6528 295b 2243 6c6f  .describe()["Clo
-0001c710: 7365 225d 5b22 6d69 6e22 5d0a 2020 2020  se"]["min"].    
-0001c720: 2020 2020 6966 2028 6863 202d 206c 6329      if (hc - lc)
-0001c730: 203c 3d20 2868 6320 2a20 7065 7263 656e   <= (hc * percen
-0001c740: 7461 6765 202f 2031 3030 2920 616e 6420  tage / 100) and 
-0001c750: 2868 6320 2d20 6c63 2021 3d20 3029 3a0a  (hc - lc != 0):.
-0001c760: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-0001c770: 656e 4469 6374 5b22 436f 6e73 6f6c 2e22  enDict["Consol."
-0001c780: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
-0001c790: 2020 2020 2020 636f 6c6f 7254 6578 742e        colorText.
-0001c7a0: 424f 4c44 0a20 2020 2020 2020 2020 2020  BOLD.           
-0001c7b0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001c7c0: 2e47 5245 454e 0a20 2020 2020 2020 2020  .GREEN.         
-0001c7d0: 2020 2020 2020 202b 2022 5261 6e67 653a         + "Range:
-0001c7e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0001c7f0: 2020 2b20 7374 7228 726f 756e 6428 2861    + str(round((a
-0001c800: 6273 2828 6863 202d 206c 6329 202f 2068  bs((hc - lc) / h
-0001c810: 6329 202a 2031 3030 292c 2031 2929 0a20  c) * 100), 1)). 
-0001c820: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001c830: 2022 2522 0a20 2020 2020 2020 2020 2020   "%".           
-0001c840: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001c850: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
-0001c860: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
-0001c870: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
-0001c880: 6565 6e44 6963 745b 2243 6f6e 736f 6c2e  eenDict["Consol.
-0001c890: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
-0001c8a0: 2020 2020 2020 2063 6f6c 6f72 5465 7874         colorText
-0001c8b0: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
-0001c8c0: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001c8d0: 742e 4641 494c 0a20 2020 2020 2020 2020  t.FAIL.         
-0001c8e0: 2020 2020 2020 202b 2022 5261 6e67 653a         + "Range:
-0001c8f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0001c900: 2020 2b20 7374 7228 726f 756e 6428 2861    + str(round((a
-0001c910: 6273 2828 6863 202d 206c 6329 202f 2068  bs((hc - lc) / h
-0001c920: 6329 202a 2031 3030 292c 2031 2929 0a20  c) * 100), 1)). 
-0001c930: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-0001c940: 2022 2522 0a20 2020 2020 2020 2020 2020   "%".           
-0001c950: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001c960: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
-0001c970: 2029 0a20 2020 2020 2020 2073 6176 6544   ).        saveD
-0001c980: 6963 745b 2243 6f6e 736f 6c2e 225d 203d  ict["Consol."] =
-0001c990: 2066 2752 616e 6765 3a7b 7374 7228 726f   f'Range:{str(ro
-0001c9a0: 756e 6428 2861 6273 2828 6863 2d6c 6329  und((abs((hc-lc)
-0001c9b0: 2f68 6329 2a31 3030 292c 3129 292b 2225  /hc)*100),1))+"%
-0001c9c0: 227d 270a 2020 2020 2020 2020 7265 7475  "}'.        retu
-0001c9d0: 726e 2072 6f75 6e64 2828 6162 7328 2868  rn round((abs((h
-0001c9e0: 6320 2d20 6c63 2920 2f20 6863 2920 2a20  c - lc) / hc) * 
-0001c9f0: 3130 3029 2c20 3129 0a0a 2020 2020 2320  100), 1)..    # 
-0001ca00: 7661 6c69 6461 7465 2069 6620 7468 6520  validate if the 
-0001ca10: 7374 6f63 6b20 6861 7320 6265 656e 2068  stock has been h
-0001ca20: 6176 696e 6720 6869 6768 6572 2068 6967  aving higher hig
-0001ca30: 6873 2c20 6869 6768 6572 206c 6f77 730a  hs, higher lows.
-0001ca40: 2020 2020 2320 616e 6420 6869 6768 6572      # and higher
-0001ca50: 2063 6c6f 7365 2077 6974 6820 6c61 7465   close with late
-0001ca60: 7374 2063 6c6f 7365 203e 2073 7570 6572  st close > super
-0001ca70: 7472 656e 6420 616e 6420 382d 454d 412e  trend and 8-EMA.
-0001ca80: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0001ca90: 6548 6967 6865 7248 6967 6873 4869 6768  eHigherHighsHigh
-0001caa0: 6572 4c6f 7773 4869 6768 6572 436c 6f73  erLowsHigherClos
-0001cab0: 6528 7365 6c66 2c20 6466 293a 0a20 2020  e(self, df):.   
-0001cac0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
-0001cad0: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
-0001cae0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-0001caf0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-0001cb00: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
-0001cb10: 6f70 7928 290a 2020 2020 2020 2020 6461  opy().        da
-0001cb20: 7930 203d 2064 6174 610a 2020 2020 2020  y0 = data.      
-0001cb30: 2020 6461 7931 203d 2064 6174 615b 313a    day1 = data[1:
-0001cb40: 5d0a 2020 2020 2020 2020 6461 7932 203d  ].        day2 =
-0001cb50: 2064 6174 615b 323a 5d0a 2020 2020 2020   data[2:].      
-0001cb60: 2020 6461 7933 203d 2064 6174 615b 333a    day3 = data[3:
-0001cb70: 5d0a 2020 2020 2020 2020 6966 206c 656e  ].        if len
-0001cb80: 2864 6179 3129 203c 2031 206f 7220 6c65  (day1) < 1 or le
-0001cb90: 6e28 6461 7932 2920 3c20 3120 6f72 206c  n(day2) < 1 or l
-0001cba0: 656e 2864 6179 3329 203c 2031 3a0a 2020  en(day3) < 1:.  
-0001cbb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001cbc0: 2046 616c 7365 0a20 2020 2020 2020 2068   False.        h
-0001cbd0: 6967 6865 7248 6967 6873 203d 2028 0a20  igherHighs = (. 
-0001cbe0: 2020 2020 2020 2020 2020 2028 6461 7930             (day0
-0001cbf0: 5b22 4869 6768 225d 2e69 6c6f 635b 305d  ["High"].iloc[0]
-0001cc00: 203e 2064 6179 315b 2248 6967 6822 5d2e   > day1["High"].
-0001cc10: 696c 6f63 5b30 5d29 0a20 2020 2020 2020  iloc[0]).       
-0001cc20: 2020 2020 2061 6e64 2028 6461 7931 5b22       and (day1["
-0001cc30: 4869 6768 225d 2e69 6c6f 635b 305d 203e  High"].iloc[0] >
-0001cc40: 2064 6179 325b 2248 6967 6822 5d2e 696c   day2["High"].il
-0001cc50: 6f63 5b30 5d29 0a20 2020 2020 2020 2020  oc[0]).         
-0001cc60: 2020 2061 6e64 2028 6461 7932 5b22 4869     and (day2["Hi
-0001cc70: 6768 225d 2e69 6c6f 635b 305d 203e 2064  gh"].iloc[0] > d
-0001cc80: 6179 335b 2248 6967 6822 5d2e 696c 6f63  ay3["High"].iloc
-0001cc90: 5b30 5d29 0a20 2020 2020 2020 2029 0a20  [0]).        ). 
-0001cca0: 2020 2020 2020 2068 6967 6865 724c 6f77         higherLow
-0001ccb0: 7320 3d20 280a 2020 2020 2020 2020 2020  s = (.          
-0001ccc0: 2020 2864 6179 305b 224c 6f77 225d 2e69    (day0["Low"].i
-0001ccd0: 6c6f 635b 305d 203e 2064 6179 315b 224c  loc[0] > day1["L
-0001cce0: 6f77 225d 2e69 6c6f 635b 305d 290a 2020  ow"].iloc[0]).  
-0001ccf0: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
-0001cd00: 6179 315b 224c 6f77 225d 2e69 6c6f 635b  ay1["Low"].iloc[
-0001cd10: 305d 203e 2064 6179 325b 224c 6f77 225d  0] > day2["Low"]
-0001cd20: 2e69 6c6f 635b 305d 290a 2020 2020 2020  .iloc[0]).      
-0001cd30: 2020 2020 2020 616e 6420 2864 6179 325b        and (day2[
-0001cd40: 224c 6f77 225d 2e69 6c6f 635b 305d 203e  "Low"].iloc[0] >
-0001cd50: 2064 6179 335b 224c 6f77 225d 2e69 6c6f   day3["Low"].ilo
-0001cd60: 635b 305d 290a 2020 2020 2020 2020 290a  c[0]).        ).
-0001cd70: 2020 2020 2020 2020 6869 6768 6572 436c          higherCl
-0001cd80: 6f73 6520 3d20 280a 2020 2020 2020 2020  ose = (.        
-0001cd90: 2020 2020 2864 6179 305b 2243 6c6f 7365      (day0["Close
-0001cda0: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
-0001cdb0: 315b 2243 6c6f 7365 225d 2e69 6c6f 635b  1["Close"].iloc[
-0001cdc0: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-0001cdd0: 616e 6420 2864 6179 315b 2243 6c6f 7365  and (day1["Close
-0001cde0: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
-0001cdf0: 325b 2243 6c6f 7365 225d 2e69 6c6f 635b  2["Close"].iloc[
-0001ce00: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-0001ce10: 616e 6420 2864 6179 325b 2243 6c6f 7365  and (day2["Close
-0001ce20: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
-0001ce30: 335b 2243 6c6f 7365 225d 2e69 6c6f 635b  3["Close"].iloc[
-0001ce40: 305d 290a 2020 2020 2020 2020 290a 2020  0]).        ).  
-0001ce50: 2020 2020 2020 2320 6869 6768 6572 5253        # higherRS
-0001ce60: 4920 3d20 2864 6179 305b 2252 5349 225d  I = (day0["RSI"]
-0001ce70: 2e69 6c6f 635b 305d 203e 2064 6179 315b  .iloc[0] > day1[
-0001ce80: 2252 5349 225d 2e69 6c6f 635b 305d 2920  "RSI"].iloc[0]) 
-0001ce90: 616e 6420 5c0a 2020 2020 2020 2020 2320  and \.        # 
-0001cea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ceb0: 2864 6179 315b 2252 5349 225d 2e69 6c6f  (day1["RSI"].ilo
-0001cec0: 635b 305d 203e 2064 6179 325b 2252 5349  c[0] > day2["RSI
-0001ced0: 225d 2e69 6c6f 635b 305d 2920 616e 6420  "].iloc[0]) and 
-0001cee0: 5c0a 2020 2020 2020 2020 2320 2020 2020  \.        #     
-0001cef0: 2020 2020 2020 2020 2020 2020 2864 6179              (day
-0001cf00: 325b 2252 5349 225d 2e69 6c6f 635b 305d  2["RSI"].iloc[0]
-0001cf10: 203e 2064 6179 335b 2252 5349 225d 2e69   > day3["RSI"].i
-0001cf20: 6c6f 635b 305d 2920 616e 6420 5c0a 2020  loc[0]) and \.  
-0001cf30: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0001cf40: 2020 2020 2020 2020 6461 7933 5b22 5253          day3["RS
-0001cf50: 4922 5d2e 696c 6f63 5b30 5d20 3e3d 2035  I"].iloc[0] >= 5
-0001cf60: 3020 616e 6420 6461 7930 5b22 5253 4922  0 and day0["RSI"
-0001cf70: 5d2e 696c 6f63 5b30 5d20 3e3d 2036 350a  ].iloc[0] >= 65.
-0001cf80: 2020 2020 2020 2020 7265 7665 7273 6564          reversed
-0001cf90: 4461 7461 203d 2064 6174 615b 3a3a 2d31  Data = data[::-1
-0001cfa0: 5d2e 636f 7079 2829 0a20 2020 2020 2020  ].copy().       
-0001cfb0: 2072 6576 6572 7365 6444 6174 615b 2253   reversedData["S
-0001cfc0: 5550 4552 5422 5d20 3d20 706b 7461 6c69  UPERT"] = pktali
-0001cfd0: 622e 7375 7065 7274 7265 6e64 2872 6576  b.supertrend(rev
-0001cfe0: 6572 7365 6444 6174 612c 2037 2c20 3329  ersedData, 7, 3)
-0001cff0: 5b22 5355 5045 5254 5f37 5f33 2e30 225d  ["SUPERT_7_3.0"]
-0001d000: 0a20 2020 2020 2020 2072 6576 6572 7365  .        reverse
-0001d010: 6444 6174 615b 2245 4d41 3822 5d20 3d20  dData["EMA8"] = 
-0001d020: 706b 7461 6c69 622e 454d 4128 7265 7665  pktalib.EMA(reve
-0001d030: 7273 6564 4461 7461 5b22 436c 6f73 6522  rsedData["Close"
-0001d040: 5d2c 2074 696d 6570 6572 696f 643d 3929  ], timeperiod=9)
-0001d050: 0a20 2020 2020 2020 2068 6967 6865 7243  .        higherC
-0001d060: 6c6f 7365 203d 2028 0a20 2020 2020 2020  lose = (.       
-0001d070: 2020 2020 2068 6967 6865 7243 6c6f 7365       higherClose
-0001d080: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-0001d090: 2064 6179 305b 2243 6c6f 7365 225d 2e69   day0["Close"].i
-0001d0a0: 6c6f 635b 305d 203e 2072 6576 6572 7365  loc[0] > reverse
-0001d0b0: 6444 6174 612e 7461 696c 2831 295b 2253  dData.tail(1)["S
-0001d0c0: 5550 4552 5422 5d2e 696c 6f63 5b30 5d0a  UPERT"].iloc[0].
-0001d0d0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0001d0e0: 6461 7930 5b22 436c 6f73 6522 5d2e 696c  day0["Close"].il
-0001d0f0: 6f63 5b30 5d20 3e20 7265 7665 7273 6564  oc[0] > reversed
-0001d100: 4461 7461 2e74 6169 6c28 3129 5b22 454d  Data.tail(1)["EM
-0001d110: 4138 225d 2e69 6c6f 635b 305d 0a20 2020  A8"].iloc[0].   
-0001d120: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
-0001d130: 6574 7572 6e20 6869 6768 6572 4869 6768  eturn higherHigh
-0001d140: 7320 616e 6420 6869 6768 6572 4c6f 7773  s and higherLows
-0001d150: 2061 6e64 2068 6967 6865 7243 6c6f 7365   and higherClose
-0001d160: 0a0a 2020 2020 2340 6d65 6173 7572 655f  ..    #@measure_
-0001d170: 7469 6d65 0a20 2020 2023 2056 616c 6964  time.    # Valid
-0001d180: 6174 6520 2749 6e73 6964 6520 4261 7227  ate 'Inside Bar'
-0001d190: 2073 7472 7563 7475 7265 2066 6f72 2072   structure for r
-0001d1a0: 6563 656e 7420 6461 7973 0a20 2020 2064  ecent days.    d
-0001d1b0: 6566 2076 616c 6964 6174 6549 6e73 6964  ef validateInsid
-0001d1c0: 6542 6172 280a 2020 2020 2020 2020 7365  eBar(.        se
-0001d1d0: 6c66 2c20 6466 2c20 7363 7265 656e 4469  lf, df, screenDi
-0001d1e0: 6374 2c20 7361 7665 4469 6374 2c20 6368  ct, saveDict, ch
-0001d1f0: 6172 7450 6174 7465 726e 3d31 2c20 6461  artPattern=1, da
-0001d200: 7973 546f 4c6f 6f6b 6261 636b 3d35 0a20  ysToLookback=5. 
-0001d210: 2020 2029 3a0a 2020 2020 2020 2020 6966     ):.        if
-0001d220: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
-0001d230: 656e 2864 6629 203d 3d20 303a 0a20 2020  en(df) == 0:.   
-0001d240: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0001d250: 4661 6c73 650a 2020 2020 2020 2020 6461  False.        da
-0001d260: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
-0001d270: 2020 2020 2020 206f 7267 4461 7461 203d         orgData =
-0001d280: 2064 6174 610a 2020 2020 2020 2020 7361   data.        sa
-0001d290: 7665 6420 3d20 7365 6c66 2e66 696e 6443  ved = self.findC
-0001d2a0: 7572 7265 6e74 5361 7665 6456 616c 7565  urrentSavedValue
-0001d2b0: 2873 6372 6565 6e44 6963 742c 2073 6176  (screenDict, sav
-0001d2c0: 6544 6963 742c 2022 5061 7474 6572 6e22  eDict, "Pattern"
-0001d2d0: 290a 2020 2020 2020 2020 666f 7220 6920  ).        for i 
-0001d2e0: 696e 2072 616e 6765 2869 6e74 2864 6179  in range(int(day
-0001d2f0: 7354 6f4c 6f6f 6b62 6163 6b29 2c20 696e  sToLookback), in
-0001d300: 7428 726f 756e 6428 6461 7973 546f 4c6f  t(round(daysToLo
-0001d310: 6f6b 6261 636b 202a 2030 2e35 2929 202d  okback * 0.5)) -
-0001d320: 2031 2c20 2d31 293a 0a20 2020 2020 2020   1, -1):.       
-0001d330: 2020 2020 2069 6620 6920 3d3d 2032 3a0a       if i == 2:.
-0001d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d350: 7265 7475 726e 2030 2020 2320 4578 6974  return 0  # Exit
-0001d360: 2069 6620 6f6e 6c79 206c 6173 7420 3220   if only last 2 
-0001d370: 6361 6e64 6c65 7320 6172 6520 6c65 6674  candles are left
-0001d380: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001d390: 6368 6172 7450 6174 7465 726e 203d 3d20  chartPattern == 
-0001d3a0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-0001d3b0: 2020 2069 6620 2255 7022 2069 6e20 7361     if "Up" in sa
-0001d3c0: 7665 4469 6374 5b22 5472 656e 6422 5d20  veDict["Trend"] 
-0001d3d0: 616e 6420 280a 2020 2020 2020 2020 2020  and (.          
-0001d3e0: 2020 2020 2020 2020 2020 2242 756c 6c22            "Bull"
-0001d3f0: 2069 6e20 7361 7665 4469 6374 5b22 4d41   in saveDict["MA
-0001d400: 2d53 6967 6e61 6c22 5d0a 2020 2020 2020  -Signal"].      
-0001d410: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-0001d420: 2022 5375 7070 6f72 7422 2069 6e20 7361   "Support" in sa
-0001d430: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
-0001d440: 6c22 5d0a 2020 2020 2020 2020 2020 2020  l"].            
-0001d450: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-0001d460: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-0001d470: 3d20 6f72 6744 6174 612e 6865 6164 2869  = orgData.head(i
-0001d480: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001d490: 2020 2020 2020 7265 6643 616e 646c 6520        refCandle 
-0001d4a0: 3d20 6461 7461 2e74 6169 6c28 3129 0a20  = data.tail(1). 
-0001d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4c0: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-0001d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4e0: 286c 656e 2864 6174 612e 4869 6768 5b64  (len(data.High[d
-0001d4f0: 6174 612e 4869 6768 203e 2072 6566 4361  ata.High > refCa
-0001d500: 6e64 6c65 2e48 6967 682e 6974 656d 2829  ndle.High.item()
-0001d510: 5d29 203d 3d20 3029 0a20 2020 2020 2020  ]) == 0).       
-0001d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d530: 2061 6e64 2028 6c65 6e28 6461 7461 2e4c   and (len(data.L
-0001d540: 6f77 5b64 6174 612e 4c6f 7720 3c20 7265  ow[data.Low < re
-0001d550: 6643 616e 646c 652e 4c6f 772e 6974 656d  fCandle.Low.item
-0001d560: 2829 5d29 203d 3d20 3029 0a20 2020 2020  ()]) == 0).     
-0001d570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d580: 2020 2061 6e64 2028 6c65 6e28 6461 7461     and (len(data
-0001d590: 2e4f 7065 6e5b 6461 7461 2e4f 7065 6e20  .Open[data.Open 
-0001d5a0: 3e20 7265 6643 616e 646c 652e 4869 6768  > refCandle.High
-0001d5b0: 2e69 7465 6d28 295d 2920 3d3d 2030 290a  .item()]) == 0).
-0001d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5d0: 2020 2020 2020 2020 616e 6420 286c 656e          and (len
-0001d5e0: 2864 6174 612e 436c 6f73 655b 6461 7461  (data.Close[data
-0001d5f0: 2e43 6c6f 7365 203c 2072 6566 4361 6e64  .Close < refCand
-0001d600: 6c65 2e4c 6f77 2e69 7465 6d28 295d 2920  le.Low.item()]) 
-0001d610: 3d3d 2030 290a 2020 2020 2020 2020 2020  == 0).          
-0001d620: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-0001d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d640: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-0001d650: 2250 6174 7465 726e 225d 203d 2028 0a20  "Pattern"] = (. 
-0001d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d670: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-0001d680: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-0001d690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6a0: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
-0001d6b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d6c0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-0001d6d0: 6f6c 6f72 5465 7874 2e57 4152 4e0a 2020  olorText.WARN.  
-0001d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6f0: 2020 2020 2020 2020 2020 2b20 2822 496e            + ("In
-0001d700: 7369 6465 2042 6172 2028 2564 2922 2025  side Bar (%d)" %
-0001d710: 2069 290a 2020 2020 2020 2020 2020 2020   i).            
-0001d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d730: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
+0001b4f0: 0a20 2020 2020 2020 206b 6579 3120 3d20  .        key1 = 
+0001b500: 2253 4d41 220a 2020 2020 2020 2020 6b65  "SMA".        ke
+0001b510: 7932 203d 2022 4c4d 4122 0a20 2020 2020  y2 = "LMA".     
+0001b520: 2020 206b 6579 3320 3d20 2235 3044 4d41     key3 = "50DMA
+0001b530: 220a 2020 2020 2020 2020 6b65 7934 203d  ".        key4 =
+0001b540: 2022 3230 3044 4d41 220a 2020 2020 2020   "200DMA".      
+0001b550: 2020 6973 3230 444d 4143 726f 7373 6f76    is20DMACrossov
+0001b560: 6572 3530 444d 4120 3d20 2872 6563 656e  er50DMA = (recen
+0001b570: 745b 2253 534d 4132 3022 5d2e 696c 6f63  t["SSMA20"].iloc
+0001b580: 5b30 5d20 3e3d 2072 6563 656e 745b 2253  [0] >= recent["S
+0001b590: 4d41 225d 2e69 6c6f 635b 305d 2920 616e  MA"].iloc[0]) an
+0001b5a0: 6420 5c0a 2020 2020 2020 2020 2020 2020  d \.            
+0001b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b5c0: 2872 6563 656e 745b 2253 534d 4132 3022  (recent["SSMA20"
+0001b5d0: 5d2e 696c 6f63 5b31 5d20 3c3d 2072 6563  ].iloc[1] <= rec
+0001b5e0: 656e 745b 2253 4d41 225d 2e69 6c6f 635b  ent["SMA"].iloc[
+0001b5f0: 315d 290a 2020 2020 2020 2020 6973 3530  1]).        is50
+0001b600: 444d 4143 726f 7373 6f76 6572 3230 3044  DMACrossover200D
+0001b610: 4d41 203d 2028 7265 6365 6e74 5b22 534d  MA = (recent["SM
+0001b620: 4122 5d2e 696c 6f63 5b30 5d20 3e3d 2072  A"].iloc[0] >= r
+0001b630: 6563 656e 745b 224c 4d41 225d 2e69 6c6f  ecent["LMA"].ilo
+0001b640: 635b 305d 2920 616e 6420 5c0a 2020 2020  c[0]) and \.    
+0001b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b660: 2020 2020 2020 2020 2872 6563 656e 745b          (recent[
+0001b670: 2253 4d41 225d 2e69 6c6f 635b 315d 203c  "SMA"].iloc[1] <
+0001b680: 3d20 7265 6365 6e74 5b22 4c4d 4122 5d2e  = recent["LMA"].
+0001b690: 696c 6f63 5b31 5d29 0a20 2020 2020 2020  iloc[1]).       
+0001b6a0: 2069 7347 6f6c 6465 6e43 726f 7373 4f76   isGoldenCrossOv
+0001b6b0: 6572 203d 2069 7332 3044 4d41 4372 6f73  er = is20DMACros
+0001b6c0: 736f 7665 7235 3044 4d41 206f 7220 6973  sover50DMA or is
+0001b6d0: 3530 444d 4143 726f 7373 6f76 6572 3230  50DMACrossover20
+0001b6e0: 3044 4d41 0a20 2020 2020 2020 2069 7335  0DMA.        is5
+0001b6f0: 3044 4d41 4372 6f73 736f 7665 7232 3030  0DMACrossover200
+0001b700: 444d 4144 6f77 6e20 3d20 2872 6563 656e  DMADown = (recen
+0001b710: 745b 2253 4d41 225d 2e69 6c6f 635b 305d  t["SMA"].iloc[0]
+0001b720: 203c 3d20 7265 6365 6e74 5b22 4c4d 4122   <= recent["LMA"
+0001b730: 5d2e 696c 6f63 5b30 5d29 2061 6e64 205c  ].iloc[0]) and \
+0001b740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b750: 2020 2020 2020 2020 2020 2020 2028 7265               (re
+0001b760: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
+0001b770: 5b31 5d20 3e3d 2072 6563 656e 745b 224c  [1] >= recent["L
+0001b780: 4d41 225d 2e69 6c6f 635b 315d 290a 2020  MA"].iloc[1]).  
+0001b790: 2020 2020 2020 6973 3230 444d 4143 726f        is20DMACro
+0001b7a0: 7373 6f76 6572 3530 444d 4144 6f77 6e20  ssover50DMADown 
+0001b7b0: 3d20 2872 6563 656e 745b 2253 534d 4132  = (recent["SSMA2
+0001b7c0: 3022 5d2e 696c 6f63 5b30 5d20 3c3d 2072  0"].iloc[0] <= r
+0001b7d0: 6563 656e 745b 2253 4d41 225d 2e69 6c6f  ecent["SMA"].ilo
+0001b7e0: 635b 305d 2920 616e 6420 5c0a 2020 2020  c[0]) and \.    
+0001b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b800: 2020 2020 2020 2020 2872 6563 656e 745b          (recent[
+0001b810: 2253 534d 4132 3022 5d2e 696c 6f63 5b31  "SSMA20"].iloc[1
+0001b820: 5d20 3e3d 2072 6563 656e 745b 2253 4d41  ] >= recent["SMA
+0001b830: 225d 2e69 6c6f 635b 315d 290a 2020 2020  "].iloc[1]).    
+0001b840: 2020 2020 6973 4465 6164 4372 6f73 734f      isDeadCrossO
+0001b850: 7665 7220 3d20 6973 3230 444d 4143 726f  ver = is20DMACro
+0001b860: 7373 6f76 6572 3530 444d 4144 6f77 6e20  ssover50DMADown 
+0001b870: 6f72 2069 7335 3044 4d41 4372 6f73 736f  or is50DMACrosso
+0001b880: 7665 7232 3030 444d 4144 6f77 6e0a 2020  ver200DMADown.  
+0001b890: 2020 2020 2020 6465 6164 784f 7665 7254        deadxOverT
+0001b8a0: 6578 7420 3d20 6627 4465 6164 4372 6f73  ext = f'DeadCros
+0001b8b0: 736f 7665 727b 2228 3230 2922 2069 6620  sover{"(20)" if 
+0001b8c0: 6973 3230 444d 4143 726f 7373 6f76 6572  is20DMACrossover
+0001b8d0: 3530 444d 4144 6f77 6e20 656c 7365 2028  50DMADown else (
+0001b8e0: 2228 3530 2922 2069 6620 6973 3530 444d  "(50)" if is50DM
+0001b8f0: 4143 726f 7373 6f76 6572 3230 3044 4d41  ACrossover200DMA
+0001b900: 446f 776e 2065 6c73 6520 2222 297d 270a  Down else "")}'.
+0001b910: 2020 2020 2020 2020 676f 6c64 656e 784f          goldenxO
+0001b920: 7665 7254 6578 7420 3d20 6627 476f 6c64  verText = f'Gold
+0001b930: 656e 4372 6f73 736f 7665 727b 2228 3230  enCrossover{"(20
+0001b940: 2922 2069 6620 6973 3230 444d 4143 726f  )" if is20DMACro
+0001b950: 7373 6f76 6572 3530 444d 4120 656c 7365  ssover50DMA else
+0001b960: 2028 2228 3530 2922 2069 6620 6973 3530   ("(50)" if is50
+0001b970: 444d 4143 726f 7373 6f76 6572 3230 3044  DMACrossover200D
+0001b980: 4d41 2065 6c73 6520 2222 297d 270a 2020  MA else "")}'.  
+0001b990: 2020 2020 2020 6966 2069 7332 3044 4d41        if is20DMA
+0001b9a0: 4372 6f73 736f 7665 7235 3044 4d41 206f  Crossover50DMA o
+0001b9b0: 7220 6973 3230 444d 4143 726f 7373 6f76  r is20DMACrossov
+0001b9c0: 6572 3530 444d 4144 6f77 6e3a 0a20 2020  er50DMADown:.   
+0001b9d0: 2020 2020 2020 2020 206b 6579 3120 3d20           key1 = 
+0001b9e0: 2253 534d 4132 3022 0a20 2020 2020 2020  "SSMA20".       
+0001b9f0: 2020 2020 206b 6579 3220 3d20 2253 4d41       key2 = "SMA
+0001ba00: 220a 2020 2020 2020 2020 2020 2020 6b65  ".            ke
+0001ba10: 7933 203d 2022 3230 444d 4122 0a20 2020  y3 = "20DMA".   
+0001ba20: 2020 2020 2020 2020 206b 6579 3420 3d20           key4 = 
+0001ba30: 2235 3044 4d41 220a 2020 2020 2020 2020  "50DMA".        
+0001ba40: 6973 3530 444d 4155 7054 7265 6e64 203d  is50DMAUpTrend =
+0001ba50: 2028 7265 6365 6e74 5b6b 6579 315d 2e69   (recent[key1].i
+0001ba60: 6c6f 635b 305d 203e 2072 6563 656e 745b  loc[0] > recent[
+0001ba70: 6b65 7932 5d2e 696c 6f63 5b31 5d29 0a20  key2].iloc[1]). 
+0001ba80: 2020 2020 2020 2069 7335 3044 4d41 446f         is50DMADo
+0001ba90: 776e 5472 656e 6420 3d20 2872 6563 656e  wnTrend = (recen
+0001baa0: 745b 6b65 7931 5d2e 696c 6f63 5b30 5d20  t[key1].iloc[0] 
+0001bab0: 3c20 7265 6365 6e74 5b6b 6579 315d 2e69  < recent[key1].i
+0001bac0: 6c6f 635b 315d 290a 2020 2020 2020 2020  loc[1]).        
+0001bad0: 6973 3530 444d 4120 3d20 2872 6563 656e  is50DMA = (recen
+0001bae0: 745b 6b65 7931 5d2e 696c 6f63 5b30 5d20  t[key1].iloc[0] 
+0001baf0: 3c3d 2072 6563 656e 745b 2243 6c6f 7365  <= recent["Close
+0001bb00: 225d 2e69 6c6f 635b 305d 290a 2020 2020  "].iloc[0]).    
+0001bb10: 2020 2020 6973 3230 3044 4d41 203d 2028      is200DMA = (
+0001bb20: 7265 6365 6e74 5b6b 6579 325d 2e69 6c6f  recent[key2].ilo
+0001bb30: 635b 305d 203c 3d20 7265 6365 6e74 5b22  c[0] <= recent["
+0001bb40: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d29  Close"].iloc[0])
+0001bb50: 0a20 2020 2020 2020 2064 6966 6665 7265  .        differe
+0001bb60: 6e63 6520 3d20 726f 756e 6428 2872 6563  nce = round((rec
+0001bb70: 656e 745b 6b65 7931 5d2e 696c 6f63 5b30  ent[key1].iloc[0
+0001bb80: 5d20 2d20 7265 6365 6e74 5b6b 6579 325d  ] - recent[key2]
+0001bb90: 2e69 6c6f 635b 305d 290a 2020 2020 2020  .iloc[0]).      
+0001bba0: 2020 2020 2020 2020 2020 2f20 7265 6365            / rece
+0001bbb0: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
+0001bbc0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+0001bbd0: 2020 2020 2a20 3130 302c 0a20 2020 2020      * 100,.     
+0001bbe0: 2020 2020 2020 2020 2020 2032 2c0a 2020             2,.  
+0001bbf0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001bc00: 2020 2020 7361 7665 4469 6374 5b22 436f      saveDict["Co
+0001bc10: 6e66 444d 4144 6966 6665 7265 6e63 6522  nfDMADifference"
+0001bc20: 5d20 3d20 6469 6666 6572 656e 6365 0a20  ] = difference. 
+0001bc30: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+0001bc40: 745b 2243 6f6e 6644 4d41 4469 6666 6572  t["ConfDMADiffer
+0001bc50: 656e 6365 225d 203d 2064 6966 6665 7265  ence"] = differe
+0001bc60: 6e63 650a 2020 2020 2020 2020 7361 7665  nce.        save
+0001bc70: 6420 3d20 7365 6c66 2e66 696e 6443 7572  d = self.findCur
+0001bc80: 7265 6e74 5361 7665 6456 616c 7565 2873  rentSavedValue(s
+0001bc90: 6372 6565 6e44 6963 742c 7361 7665 4469  creenDict,saveDi
+0001bca0: 6374 2c22 4d41 2d53 6967 6e61 6c22 290a  ct,"MA-Signal").
+0001bcb0: 2020 2020 2020 2020 2320 6469 6666 6572          # differ
+0001bcc0: 656e 6365 203d 2061 6273 2864 6966 6665  ence = abs(diffe
+0001bcd0: 7265 6e63 6529 0a20 2020 2020 2020 2063  rence).        c
+0001bce0: 6f6e 6654 6578 7420 3d20 6622 7b67 6f6c  onfText = f"{gol
+0001bcf0: 6465 6e78 4f76 6572 5465 7874 2069 6620  denxOverText if 
+0001bd00: 6973 476f 6c64 656e 4372 6f73 734f 7665  isGoldenCrossOve
+0001bd10: 7220 656c 7365 2028 6465 6164 784f 7665  r else (deadxOve
+0001bd20: 7254 6578 7420 6966 2069 7344 6561 6443  rText if isDeadC
+0001bd30: 726f 7373 4f76 6572 2065 6c73 6520 2827  rossOver else ('
+0001bd40: 436f 6e66 2e55 7027 2069 6620 6973 3530  Conf.Up' if is50
+0001bd50: 444d 4155 7054 7265 6e64 2065 6c73 6520  DMAUpTrend else 
+0001bd60: 2827 436f 6e66 2e44 6f77 6e27 2069 6620  ('Conf.Down' if 
+0001bd70: 6973 3530 444d 4144 6f77 6e54 7265 6e64  is50DMADownTrend
+0001bd80: 2065 6c73 6520 286b 6579 3320 6966 2069   else (key3 if i
+0001bd90: 7335 3044 4d41 2065 6c73 6520 286b 6579  s50DMA else (key
+0001bda0: 3420 6966 2069 7332 3030 444d 4120 656c  4 if is200DMA el
+0001bdb0: 7365 2027 556e 6b6e 6f77 6e27 2929 2929  se 'Unknown'))))
+0001bdc0: 297d 220a 2020 2020 2020 2020 6966 2061  )}".        if a
+0001bdd0: 6273 2872 6563 656e 745b 6b65 7931 5d2e  bs(recent[key1].
+0001bde0: 696c 6f63 5b30 5d20 2d20 7265 6365 6e74  iloc[0] - recent
+0001bdf0: 5b6b 6579 325d 2e69 6c6f 635b 305d 2920  [key2].iloc[0]) 
+0001be00: 3c3d 2028 0a20 2020 2020 2020 2020 2020  <= (.           
+0001be10: 2072 6563 656e 745b 6b65 7931 5d2e 696c   recent[key1].il
+0001be20: 6f63 5b30 5d20 2a20 7065 7263 656e 7461  oc[0] * percenta
+0001be30: 6765 0a20 2020 2020 2020 2029 3a0a 2020  ge.        ):.  
+0001be40: 2020 2020 2020 2020 2020 6966 2072 6563            if rec
+0001be50: 656e 745b 6b65 7931 5d2e 696c 6f63 5b30  ent[key1].iloc[0
+0001be60: 5d20 3e3d 2072 6563 656e 745b 6b65 7932  ] >= recent[key2
+0001be70: 5d2e 696c 6f63 5b30 5d3a 0a20 2020 2020  ].iloc[0]:.     
+0001be80: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+0001be90: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
+0001bea0: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
+0001beb0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+0001bec0: 5b30 5d20 0a20 2020 2020 2020 2020 2020  [0] .           
+0001bed0: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
+0001bee0: 5465 7874 2e42 4f4c 440a 2020 2020 2020  Text.BOLD.      
+0001bef0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001bf00: 2863 6f6c 6f72 5465 7874 2e47 5245 454e  (colorText.GREEN
+0001bf10: 2069 6620 6973 3530 444d 4155 7054 7265   if is50DMAUpTre
+0001bf20: 6e64 2065 6c73 6520 2863 6f6c 6f72 5465  nd else (colorTe
+0001bf30: 7874 2e46 4149 4c20 6966 2069 7335 3044  xt.FAIL if is50D
+0001bf40: 4d41 446f 776e 5472 656e 6420 656c 7365  MADownTrend else
+0001bf50: 2063 6f6c 6f72 5465 7874 2e57 4152 4e29   colorText.WARN)
+0001bf60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001bf70: 2020 2020 2020 2b20 6622 7b63 6f6e 6654        + f"{confT
+0001bf80: 6578 747d 2028 7b64 6966 6665 7265 6e63  ext} ({differenc
+0001bf90: 657d 2529 220a 2020 2020 2020 2020 2020  e}%)".          
+0001bfa0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+0001bfb0: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+0001bfc0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001bfd0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+0001bfe0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+0001bff0: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
+0001c000: 227b 636f 6e66 5465 7874 7d20 287b 6469  "{confText} ({di
+0001c010: 6666 6572 656e 6365 7d25 2922 0a20 2020  fference}%)".   
+0001c020: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0001c030: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001c040: 6372 6565 6e44 6963 745b 224d 412d 5369  creenDict["MA-Si
+0001c050: 676e 616c 225d 203d 2028 0a20 2020 2020  gnal"] = (.     
+0001c060: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001c070: 6176 6564 5b30 5d20 0a20 2020 2020 2020  aved[0] .       
+0001c080: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+0001c090: 6f6c 6f72 5465 7874 2e42 4f4c 440a 2020  olorText.BOLD.  
+0001c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c0b0: 2020 2b20 2863 6f6c 6f72 5465 7874 2e47    + (colorText.G
+0001c0c0: 5245 454e 2069 6620 6973 3530 444d 4155  REEN if is50DMAU
+0001c0d0: 7054 7265 6e64 2065 6c73 6520 2863 6f6c  pTrend else (col
+0001c0e0: 6f72 5465 7874 2e46 4149 4c20 6966 2069  orText.FAIL if i
+0001c0f0: 7335 3044 4d41 446f 776e 5472 656e 6420  s50DMADownTrend 
+0001c100: 656c 7365 2063 6f6c 6f72 5465 7874 2e57  else colorText.W
+0001c110: 4152 4e29 290a 2020 2020 2020 2020 2020  ARN)).          
+0001c120: 2020 2020 2020 2020 2020 2b20 6622 7b63            + f"{c
+0001c130: 6f6e 6654 6578 747d 2028 7b64 6966 6665  onfText} ({diffe
+0001c140: 7265 6e63 657d 2529 220a 2020 2020 2020  rence}%)".      
+0001c150: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+0001c160: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
+0001c170: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0001c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c190: 7361 7665 4469 6374 5b22 4d41 2d53 6967  saveDict["MA-Sig
+0001c1a0: 6e61 6c22 5d20 3d20 7361 7665 645b 315d  nal"] = saved[1]
+0001c1b0: 202b 2066 227b 636f 6e66 5465 7874 7d20   + f"{confText} 
+0001c1c0: 287b 6469 6666 6572 656e 6365 7d25 2922  ({difference}%)"
+0001c1d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0001c1e0: 7572 6e20 636f 6e66 4669 6c74 6572 203d  urn confFilter =
+0001c1f0: 3d20 3320 6f72 205c 0a20 2020 2020 2020  = 3 or \.       
+0001c200: 2020 2020 2020 2020 2028 636f 6e66 4669           (confFi
+0001c210: 6c74 6572 203d 3d20 3120 616e 6420 6e6f  lter == 1 and no
+0001c220: 7420 6973 4465 6164 4372 6f73 734f 7665  t isDeadCrossOve
+0001c230: 7220 616e 6420 2869 7335 3044 4d41 5570  r and (is50DMAUp
+0001c240: 5472 656e 6420 6f72 2028 6973 476f 6c64  Trend or (isGold
+0001c250: 656e 4372 6f73 734f 7665 7220 6f72 2027  enCrossOver or '
+0001c260: 5570 2720 696e 2063 6f6e 6654 6578 7429  Up' in confText)
+0001c270: 2929 206f 7220 5c0a 2020 2020 2020 2020  )) or \.        
+0001c280: 2020 2020 2020 2020 2863 6f6e 6646 696c          (confFil
+0001c290: 7465 7220 3d3d 2032 2061 6e64 206e 6f74  ter == 2 and not
+0001c2a0: 2069 7347 6f6c 6465 6e43 726f 7373 4f76   isGoldenCrossOv
+0001c2b0: 6572 2061 6e64 2028 6973 3530 444d 4144  er and (is50DMAD
+0001c2c0: 6f77 6e54 7265 6e64 206f 7220 6973 4465  ownTrend or isDe
+0001c2d0: 6164 4372 6f73 734f 7665 7220 6f72 2027  adCrossOver or '
+0001c2e0: 446f 776e 2720 696e 2063 6f6e 6654 6578  Down' in confTex
+0001c2f0: 7429 290a 2020 2020 2020 2020 2320 4d61  t)).        # Ma
+0001c300: 7962 6520 7468 6520 6469 6666 6572 656e  ybe the differen
+0001c310: 6365 2069 7320 6e6f 7420 7769 7468 696e  ce is not within
+0001c320: 2074 6865 2072 616e 6765 2c20 6275 7420   the range, but 
+0001c330: 7765 2764 2073 7469 6c6c 206c 696b 6520  we'd still like 
+0001c340: 746f 206b 6565 7020 7468 6520 7374 6f63  to keep the stoc
+0001c350: 6b20 696e 0a20 2020 2020 2020 2023 2074  k in.        # t
+0001c360: 6865 206c 6973 7420 6966 2069 7427 7320  he list if it's 
+0001c370: 6120 676f 6c64 656e 2063 726f 7373 6f76  a golden crossov
+0001c380: 6572 206f 7220 6465 6164 2063 726f 7373  er or dead cross
+0001c390: 6f76 6572 0a20 2020 2020 2020 2069 6620  over.        if 
+0001c3a0: 6973 476f 6c64 656e 4372 6f73 734f 7665  isGoldenCrossOve
+0001c3b0: 7220 6f72 2069 7344 6561 6443 726f 7373  r or isDeadCross
+0001c3c0: 4f76 6572 3a0a 2020 2020 2020 2020 2020  Over:.          
+0001c3d0: 2020 7363 7265 656e 4469 6374 5b22 4d41    screenDict["MA
+0001c3e0: 2d53 6967 6e61 6c22 5d20 3d20 280a 2020  -Signal"] = (.  
+0001c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c400: 2020 7361 7665 645b 305d 200a 2020 2020    saved[0] .    
+0001c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c420: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
+0001c430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c440: 2020 2020 202b 2028 636f 6c6f 7254 6578       + (colorTex
+0001c450: 742e 4752 4545 4e20 6966 2069 7335 3044  t.GREEN if is50D
+0001c460: 4d41 5570 5472 656e 6420 656c 7365 2028  MAUpTrend else (
+0001c470: 636f 6c6f 7254 6578 742e 4641 494c 2069  colorText.FAIL i
+0001c480: 6620 6973 3530 444d 4144 6f77 6e54 7265  f is50DMADownTre
+0001c490: 6e64 2065 6c73 6520 636f 6c6f 7254 6578  nd else colorTex
+0001c4a0: 742e 5741 524e 2929 0a20 2020 2020 2020  t.WARN)).       
+0001c4b0: 2020 2020 2020 2020 2020 2020 202b 2066               + f
+0001c4c0: 227b 636f 6e66 5465 7874 7d20 287b 6469  "{confText} ({di
+0001c4d0: 6666 6572 656e 6365 7d25 2922 0a20 2020  fference}%)".   
+0001c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c4f0: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+0001c500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c510: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
+0001c520: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
+0001c530: 616c 225d 203d 2073 6176 6564 5b31 5d20  al"] = saved[1] 
+0001c540: 2b20 6622 7b63 6f6e 6654 6578 747d 2028  + f"{confText} (
+0001c550: 7b64 6966 6665 7265 6e63 657d 2529 220a  {difference}%)".
+0001c560: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001c570: 726e 2063 6f6e 6646 696c 7465 7220 3d3d  rn confFilter ==
+0001c580: 2033 206f 7220 5c0a 2020 2020 2020 2020   3 or \.        
+0001c590: 2020 2020 2020 2020 2863 6f6e 6646 696c          (confFil
+0001c5a0: 7465 7220 3d3d 2031 2061 6e64 2069 7347  ter == 1 and isG
+0001c5b0: 6f6c 6465 6e43 726f 7373 4f76 6572 2920  oldenCrossOver) 
+0001c5c0: 6f72 205c 0a20 2020 2020 2020 2020 2020  or \.           
+0001c5d0: 2020 2020 2028 636f 6e66 4669 6c74 6572       (confFilter
+0001c5e0: 203d 3d20 3220 616e 6420 6973 4465 6164   == 2 and isDead
+0001c5f0: 4372 6f73 734f 7665 7229 0a20 2020 2020  CrossOver).     
+0001c600: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0001c610: 0a20 2020 2023 406d 6561 7375 7265 5f74  .    #@measure_t
+0001c620: 696d 650a 2020 2020 2320 5661 6c69 6461  ime.    # Valida
+0001c630: 7465 2069 6620 7368 6172 6520 7072 6963  te if share pric
+0001c640: 6573 2061 7265 2063 6f6e 736f 6c69 6461  es are consolida
+0001c650: 7469 6e67 0a20 2020 2064 6566 2076 616c  ting.    def val
+0001c660: 6964 6174 6543 6f6e 736f 6c69 6461 7469  idateConsolidati
+0001c670: 6f6e 2873 656c 662c 2064 662c 2073 6372  on(self, df, scr
+0001c680: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+0001c690: 742c 2070 6572 6365 6e74 6167 653d 3130  t, percentage=10
+0001c6a0: 293a 0a20 2020 2020 2020 2069 6620 6466  ):.        if df
+0001c6b0: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
+0001c6c0: 6466 2920 3d3d 2030 3a0a 2020 2020 2020  df) == 0:.      
+0001c6d0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0001c6e0: 7365 0a20 2020 2020 2020 2064 6174 6120  se.        data 
+0001c6f0: 3d20 6466 2e63 6f70 7928 290a 2020 2020  = df.copy().    
+0001c700: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+0001c710: 6669 6c6c 6e61 2830 290a 2020 2020 2020  fillna(0).      
+0001c720: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
+0001c730: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
+0001c740: 6e70 2e69 6e66 5d2c 2030 290a 2020 2020  np.inf], 0).    
+0001c750: 2020 2020 6863 203d 2064 6174 612e 6465      hc = data.de
+0001c760: 7363 7269 6265 2829 5b22 436c 6f73 6522  scribe()["Close"
+0001c770: 5d5b 226d 6178 225d 0a20 2020 2020 2020  ]["max"].       
+0001c780: 206c 6320 3d20 6461 7461 2e64 6573 6372   lc = data.descr
+0001c790: 6962 6528 295b 2243 6c6f 7365 225d 5b22  ibe()["Close"]["
+0001c7a0: 6d69 6e22 5d0a 2020 2020 2020 2020 6966  min"].        if
+0001c7b0: 2028 6863 202d 206c 6329 203c 3d20 2868   (hc - lc) <= (h
+0001c7c0: 6320 2a20 7065 7263 656e 7461 6765 202f  c * percentage /
+0001c7d0: 2031 3030 2920 616e 6420 2868 6320 2d20   100) and (hc - 
+0001c7e0: 6c63 2021 3d20 3029 3a0a 2020 2020 2020  lc != 0):.      
+0001c7f0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+0001c800: 5b22 436f 6e73 6f6c 2e22 5d20 3d20 280a  ["Consol."] = (.
+0001c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c820: 636f 6c6f 7254 6578 742e 424f 4c44 0a20  colorText.BOLD. 
+0001c830: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001c840: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+0001c850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c860: 202b 2022 5261 6e67 653a 220a 2020 2020   + "Range:".    
+0001c870: 2020 2020 2020 2020 2020 2020 2b20 7374              + st
+0001c880: 7228 726f 756e 6428 2861 6273 2828 6863  r(round((abs((hc
+0001c890: 202d 206c 6329 202f 2068 6329 202a 2031   - lc) / hc) * 1
+0001c8a0: 3030 292c 2031 2929 0a20 2020 2020 2020  00), 1)).       
+0001c8b0: 2020 2020 2020 2020 202b 2022 2522 0a20           + "%". 
+0001c8c0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001c8d0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
+0001c8e0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001c8f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001c900: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+0001c910: 745b 2243 6f6e 736f 6c2e 225d 203d 2028  t["Consol."] = (
+0001c920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c930: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440a   colorText.BOLD.
+0001c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c950: 2b20 636f 6c6f 7254 6578 742e 4641 494c  + colorText.FAIL
+0001c960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c970: 202b 2022 5261 6e67 653a 220a 2020 2020   + "Range:".    
+0001c980: 2020 2020 2020 2020 2020 2020 2b20 7374              + st
+0001c990: 7228 726f 756e 6428 2861 6273 2828 6863  r(round((abs((hc
+0001c9a0: 202d 206c 6329 202f 2068 6329 202a 2031   - lc) / hc) * 1
+0001c9b0: 3030 292c 2031 2929 0a20 2020 2020 2020  00), 1)).       
+0001c9c0: 2020 2020 2020 2020 202b 2022 2522 0a20           + "%". 
+0001c9d0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001c9e0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
+0001c9f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001ca00: 2020 2020 2073 6176 6544 6963 745b 2243       saveDict["C
+0001ca10: 6f6e 736f 6c2e 225d 203d 2066 2752 616e  onsol."] = f'Ran
+0001ca20: 6765 3a7b 7374 7228 726f 756e 6428 2861  ge:{str(round((a
+0001ca30: 6273 2828 6863 2d6c 6329 2f68 6329 2a31  bs((hc-lc)/hc)*1
+0001ca40: 3030 292c 3129 292b 2225 227d 270a 2020  00),1))+"%"}'.  
+0001ca50: 2020 2020 2020 7265 7475 726e 2072 6f75        return rou
+0001ca60: 6e64 2828 6162 7328 2868 6320 2d20 6c63  nd((abs((hc - lc
+0001ca70: 2920 2f20 6863 2920 2a20 3130 3029 2c20  ) / hc) * 100), 
+0001ca80: 3129 0a0a 2020 2020 2320 7661 6c69 6461  1)..    # valida
+0001ca90: 7465 2069 6620 7468 6520 7374 6f63 6b20  te if the stock 
+0001caa0: 6861 7320 6265 656e 2068 6176 696e 6720  has been having 
+0001cab0: 6869 6768 6572 2068 6967 6873 2c20 6869  higher highs, hi
+0001cac0: 6768 6572 206c 6f77 730a 2020 2020 2320  gher lows.    # 
+0001cad0: 616e 6420 6869 6768 6572 2063 6c6f 7365  and higher close
+0001cae0: 2077 6974 6820 6c61 7465 7374 2063 6c6f   with latest clo
+0001caf0: 7365 203e 2073 7570 6572 7472 656e 6420  se > supertrend 
+0001cb00: 616e 6420 382d 454d 412e 0a20 2020 2064  and 8-EMA..    d
+0001cb10: 6566 2076 616c 6964 6174 6548 6967 6865  ef validateHighe
+0001cb20: 7248 6967 6873 4869 6768 6572 4c6f 7773  rHighsHigherLows
+0001cb30: 4869 6768 6572 436c 6f73 6528 7365 6c66  HigherClose(self
+0001cb40: 2c20 6466 293a 0a20 2020 2020 2020 2069  , df):.        i
+0001cb50: 6620 6466 2069 7320 4e6f 6e65 206f 7220  f df is None or 
+0001cb60: 6c65 6e28 6466 2920 3d3d 2030 3a0a 2020  len(df) == 0:.  
+0001cb70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001cb80: 2046 616c 7365 0a20 2020 2020 2020 2064   False.        d
+0001cb90: 6174 6120 3d20 6466 2e63 6f70 7928 290a  ata = df.copy().
+0001cba0: 2020 2020 2020 2020 6461 7930 203d 2064          day0 = d
+0001cbb0: 6174 610a 2020 2020 2020 2020 6461 7931  ata.        day1
+0001cbc0: 203d 2064 6174 615b 313a 5d0a 2020 2020   = data[1:].    
+0001cbd0: 2020 2020 6461 7932 203d 2064 6174 615b      day2 = data[
+0001cbe0: 323a 5d0a 2020 2020 2020 2020 6461 7933  2:].        day3
+0001cbf0: 203d 2064 6174 615b 333a 5d0a 2020 2020   = data[3:].    
+0001cc00: 2020 2020 6966 206c 656e 2864 6179 3129      if len(day1)
+0001cc10: 203c 2031 206f 7220 6c65 6e28 6461 7932   < 1 or len(day2
+0001cc20: 2920 3c20 3120 6f72 206c 656e 2864 6179  ) < 1 or len(day
+0001cc30: 3329 203c 2031 3a0a 2020 2020 2020 2020  3) < 1:.        
+0001cc40: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+0001cc50: 0a20 2020 2020 2020 2068 6967 6865 7248  .        higherH
+0001cc60: 6967 6873 203d 2028 0a20 2020 2020 2020  ighs = (.       
+0001cc70: 2020 2020 2028 6461 7930 5b22 4869 6768       (day0["High
+0001cc80: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
+0001cc90: 315b 2248 6967 6822 5d2e 696c 6f63 5b30  1["High"].iloc[0
+0001cca0: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
+0001ccb0: 6e64 2028 6461 7931 5b22 4869 6768 225d  nd (day1["High"]
+0001ccc0: 2e69 6c6f 635b 305d 203e 2064 6179 325b  .iloc[0] > day2[
+0001ccd0: 2248 6967 6822 5d2e 696c 6f63 5b30 5d29  "High"].iloc[0])
+0001cce0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+0001ccf0: 2028 6461 7932 5b22 4869 6768 225d 2e69   (day2["High"].i
+0001cd00: 6c6f 635b 305d 203e 2064 6179 335b 2248  loc[0] > day3["H
+0001cd10: 6967 6822 5d2e 696c 6f63 5b30 5d29 0a20  igh"].iloc[0]). 
+0001cd20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0001cd30: 2068 6967 6865 724c 6f77 7320 3d20 280a   higherLows = (.
+0001cd40: 2020 2020 2020 2020 2020 2020 2864 6179              (day
+0001cd50: 305b 224c 6f77 225d 2e69 6c6f 635b 305d  0["Low"].iloc[0]
+0001cd60: 203e 2064 6179 315b 224c 6f77 225d 2e69   > day1["Low"].i
+0001cd70: 6c6f 635b 305d 290a 2020 2020 2020 2020  loc[0]).        
+0001cd80: 2020 2020 616e 6420 2864 6179 315b 224c      and (day1["L
+0001cd90: 6f77 225d 2e69 6c6f 635b 305d 203e 2064  ow"].iloc[0] > d
+0001cda0: 6179 325b 224c 6f77 225d 2e69 6c6f 635b  ay2["Low"].iloc[
+0001cdb0: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
+0001cdc0: 616e 6420 2864 6179 325b 224c 6f77 225d  and (day2["Low"]
+0001cdd0: 2e69 6c6f 635b 305d 203e 2064 6179 335b  .iloc[0] > day3[
+0001cde0: 224c 6f77 225d 2e69 6c6f 635b 305d 290a  "Low"].iloc[0]).
+0001cdf0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0001ce00: 2020 6869 6768 6572 436c 6f73 6520 3d20    higherClose = 
+0001ce10: 280a 2020 2020 2020 2020 2020 2020 2864  (.            (d
+0001ce20: 6179 305b 2243 6c6f 7365 225d 2e69 6c6f  ay0["Close"].ilo
+0001ce30: 635b 305d 203e 2064 6179 315b 2243 6c6f  c[0] > day1["Clo
+0001ce40: 7365 225d 2e69 6c6f 635b 305d 290a 2020  se"].iloc[0]).  
+0001ce50: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
+0001ce60: 6179 315b 2243 6c6f 7365 225d 2e69 6c6f  ay1["Close"].ilo
+0001ce70: 635b 305d 203e 2064 6179 325b 2243 6c6f  c[0] > day2["Clo
+0001ce80: 7365 225d 2e69 6c6f 635b 305d 290a 2020  se"].iloc[0]).  
+0001ce90: 2020 2020 2020 2020 2020 616e 6420 2864            and (d
+0001cea0: 6179 325b 2243 6c6f 7365 225d 2e69 6c6f  ay2["Close"].ilo
+0001ceb0: 635b 305d 203e 2064 6179 335b 2243 6c6f  c[0] > day3["Clo
+0001cec0: 7365 225d 2e69 6c6f 635b 305d 290a 2020  se"].iloc[0]).  
+0001ced0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001cee0: 2320 6869 6768 6572 5253 4920 3d20 2864  # higherRSI = (d
+0001cef0: 6179 305b 2252 5349 225d 2e69 6c6f 635b  ay0["RSI"].iloc[
+0001cf00: 305d 203e 2064 6179 315b 2252 5349 225d  0] > day1["RSI"]
+0001cf10: 2e69 6c6f 635b 305d 2920 616e 6420 5c0a  .iloc[0]) and \.
+0001cf20: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0001cf30: 2020 2020 2020 2020 2020 2864 6179 315b            (day1[
+0001cf40: 2252 5349 225d 2e69 6c6f 635b 305d 203e  "RSI"].iloc[0] >
+0001cf50: 2064 6179 325b 2252 5349 225d 2e69 6c6f   day2["RSI"].ilo
+0001cf60: 635b 305d 2920 616e 6420 5c0a 2020 2020  c[0]) and \.    
+0001cf70: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0001cf80: 2020 2020 2020 2864 6179 325b 2252 5349        (day2["RSI
+0001cf90: 225d 2e69 6c6f 635b 305d 203e 2064 6179  "].iloc[0] > day
+0001cfa0: 335b 2252 5349 225d 2e69 6c6f 635b 305d  3["RSI"].iloc[0]
+0001cfb0: 2920 616e 6420 5c0a 2020 2020 2020 2020  ) and \.        
+0001cfc0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0001cfd0: 2020 6461 7933 5b22 5253 4922 5d2e 696c    day3["RSI"].il
+0001cfe0: 6f63 5b30 5d20 3e3d 2035 3020 616e 6420  oc[0] >= 50 and 
+0001cff0: 6461 7930 5b22 5253 4922 5d2e 696c 6f63  day0["RSI"].iloc
+0001d000: 5b30 5d20 3e3d 2036 350a 2020 2020 2020  [0] >= 65.      
+0001d010: 2020 7265 7665 7273 6564 4461 7461 203d    reversedData =
+0001d020: 2064 6174 615b 3a3a 2d31 5d2e 636f 7079   data[::-1].copy
+0001d030: 2829 0a20 2020 2020 2020 2072 6576 6572  ().        rever
+0001d040: 7365 6444 6174 615b 2253 5550 4552 5422  sedData["SUPERT"
+0001d050: 5d20 3d20 706b 7461 6c69 622e 7375 7065  ] = pktalib.supe
+0001d060: 7274 7265 6e64 2872 6576 6572 7365 6444  rtrend(reversedD
+0001d070: 6174 612c 2037 2c20 3329 5b22 5355 5045  ata, 7, 3)["SUPE
+0001d080: 5254 5f37 5f33 2e30 225d 0a20 2020 2020  RT_7_3.0"].     
+0001d090: 2020 2072 6576 6572 7365 6444 6174 615b     reversedData[
+0001d0a0: 2245 4d41 3822 5d20 3d20 706b 7461 6c69  "EMA8"] = pktali
+0001d0b0: 622e 454d 4128 7265 7665 7273 6564 4461  b.EMA(reversedDa
+0001d0c0: 7461 5b22 436c 6f73 6522 5d2c 2074 696d  ta["Close"], tim
+0001d0d0: 6570 6572 696f 643d 3929 0a20 2020 2020  eperiod=9).     
+0001d0e0: 2020 2068 6967 6865 7243 6c6f 7365 203d     higherClose =
+0001d0f0: 2028 0a20 2020 2020 2020 2020 2020 2068   (.            h
+0001d100: 6967 6865 7243 6c6f 7365 0a20 2020 2020  igherClose.     
+0001d110: 2020 2020 2020 2061 6e64 2064 6179 305b         and day0[
+0001d120: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
+0001d130: 203e 2072 6576 6572 7365 6444 6174 612e   > reversedData.
+0001d140: 7461 696c 2831 295b 2253 5550 4552 5422  tail(1)["SUPERT"
+0001d150: 5d2e 696c 6f63 5b30 5d0a 2020 2020 2020  ].iloc[0].      
+0001d160: 2020 2020 2020 616e 6420 6461 7930 5b22        and day0["
+0001d170: 436c 6f73 6522 5d2e 696c 6f63 5b30 5d20  Close"].iloc[0] 
+0001d180: 3e20 7265 7665 7273 6564 4461 7461 2e74  > reversedData.t
+0001d190: 6169 6c28 3129 5b22 454d 4138 225d 2e69  ail(1)["EMA8"].i
+0001d1a0: 6c6f 635b 305d 0a20 2020 2020 2020 2029  loc[0].        )
+0001d1b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001d1c0: 6869 6768 6572 4869 6768 7320 616e 6420  higherHighs and 
+0001d1d0: 6869 6768 6572 4c6f 7773 2061 6e64 2068  higherLows and h
+0001d1e0: 6967 6865 7243 6c6f 7365 0a0a 2020 2020  igherClose..    
+0001d1f0: 2340 6d65 6173 7572 655f 7469 6d65 0a20  #@measure_time. 
+0001d200: 2020 2023 2056 616c 6964 6174 6520 2749     # Validate 'I
+0001d210: 6e73 6964 6520 4261 7227 2073 7472 7563  nside Bar' struc
+0001d220: 7475 7265 2066 6f72 2072 6563 656e 7420  ture for recent 
+0001d230: 6461 7973 0a20 2020 2064 6566 2076 616c  days.    def val
+0001d240: 6964 6174 6549 6e73 6964 6542 6172 280a  idateInsideBar(.
+0001d250: 2020 2020 2020 2020 7365 6c66 2c20 6466          self, df
+0001d260: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
+0001d270: 7665 4469 6374 2c20 6368 6172 7450 6174  veDict, chartPat
+0001d280: 7465 726e 3d31 2c20 6461 7973 546f 4c6f  tern=1, daysToLo
+0001d290: 6f6b 6261 636b 3d35 0a20 2020 2029 3a0a  okback=5.    ):.
+0001d2a0: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
+0001d2b0: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
+0001d2c0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+0001d2d0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+0001d2e0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0001d2f0: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
+0001d300: 206f 7267 4461 7461 203d 2064 6174 610a   orgData = data.
+0001d310: 2020 2020 2020 2020 7361 7665 6420 3d20          saved = 
+0001d320: 7365 6c66 2e66 696e 6443 7572 7265 6e74  self.findCurrent
+0001d330: 5361 7665 6456 616c 7565 2873 6372 6565  SavedValue(scree
+0001d340: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
+0001d350: 2022 5061 7474 6572 6e22 290a 2020 2020   "Pattern").    
+0001d360: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+0001d370: 6765 2869 6e74 2864 6179 7354 6f4c 6f6f  ge(int(daysToLoo
+0001d380: 6b62 6163 6b29 2c20 696e 7428 726f 756e  kback), int(roun
+0001d390: 6428 6461 7973 546f 4c6f 6f6b 6261 636b  d(daysToLookback
+0001d3a0: 202a 2030 2e35 2929 202d 2031 2c20 2d31   * 0.5)) - 1, -1
+0001d3b0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0001d3c0: 6620 6920 3d3d 2032 3a0a 2020 2020 2020  f i == 2:.      
+0001d3d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001d3e0: 2030 2020 2320 4578 6974 2069 6620 6f6e   0  # Exit if on
+0001d3f0: 6c79 206c 6173 7420 3220 6361 6e64 6c65  ly last 2 candle
+0001d400: 7320 6172 6520 6c65 6674 0a20 2020 2020  s are left.     
+0001d410: 2020 2020 2020 2069 6620 6368 6172 7450         if chartP
+0001d420: 6174 7465 726e 203d 3d20 313a 0a20 2020  attern == 1:.   
+0001d430: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001d440: 2255 7022 2069 6e20 7361 7665 4469 6374  "Up" in saveDict
+0001d450: 5b22 5472 656e 6422 5d20 616e 6420 280a  ["Trend"] and (.
+0001d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d470: 2020 2020 2242 756c 6c22 2069 6e20 7361      "Bull" in sa
+0001d480: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
+0001d490: 6c22 5d0a 2020 2020 2020 2020 2020 2020  l"].            
+0001d4a0: 2020 2020 2020 2020 6f72 2022 5375 7070          or "Supp
+0001d4b0: 6f72 7422 2069 6e20 7361 7665 4469 6374  ort" in saveDict
+0001d4c0: 5b22 4d41 2d53 6967 6e61 6c22 5d0a 2020  ["MA-Signal"].  
+0001d4d0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
+0001d4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d4f0: 2020 2020 2064 6174 6120 3d20 6f72 6744       data = orgD
+0001d500: 6174 612e 6865 6164 2869 290a 2020 2020  ata.head(i).    
+0001d510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d520: 7265 6643 616e 646c 6520 3d20 6461 7461  refCandle = data
+0001d530: 2e74 6169 6c28 3129 0a20 2020 2020 2020  .tail(1).       
+0001d540: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001d550: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001d560: 2020 2020 2020 2020 2020 286c 656e 2864            (len(d
+0001d570: 6174 612e 4869 6768 5b64 6174 612e 4869  ata.High[data.Hi
+0001d580: 6768 203e 2072 6566 4361 6e64 6c65 2e48  gh > refCandle.H
+0001d590: 6967 682e 6974 656d 2829 5d29 203d 3d20  igh.item()]) == 
+0001d5a0: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+0001d5b0: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
+0001d5c0: 6c65 6e28 6461 7461 2e4c 6f77 5b64 6174  len(data.Low[dat
+0001d5d0: 612e 4c6f 7720 3c20 7265 6643 616e 646c  a.Low < refCandl
+0001d5e0: 652e 4c6f 772e 6974 656d 2829 5d29 203d  e.Low.item()]) =
+0001d5f0: 3d20 3029 0a20 2020 2020 2020 2020 2020  = 0).           
+0001d600: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+0001d610: 2028 6c65 6e28 6461 7461 2e4f 7065 6e5b   (len(data.Open[
+0001d620: 6461 7461 2e4f 7065 6e20 3e20 7265 6643  data.Open > refC
+0001d630: 616e 646c 652e 4869 6768 2e69 7465 6d28  andle.High.item(
+0001d640: 295d 2920 3d3d 2030 290a 2020 2020 2020  )]) == 0).      
+0001d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d660: 2020 616e 6420 286c 656e 2864 6174 612e    and (len(data.
+0001d670: 436c 6f73 655b 6461 7461 2e43 6c6f 7365  Close[data.Close
+0001d680: 203c 2072 6566 4361 6e64 6c65 2e4c 6f77   < refCandle.Low
+0001d690: 2e69 7465 6d28 295d 2920 3d3d 2030 290a  .item()]) == 0).
+0001d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d6b0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+0001d6c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001d6d0: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
+0001d6e0: 726e 225d 203d 2028 0a20 2020 2020 2020  rn"] = (.       
+0001d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d700: 2020 2020 2073 6176 6564 5b30 5d0a 2020       saved[0].  
+0001d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d720: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+0001d730: 7254 6578 742e 424f 4c44 0a20 2020 2020  rText.BOLD.     
 0001d740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d750: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0001d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d770: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
-0001d780: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
-0001d790: 202b 2022 496e 7369 6465 2042 6172 2028   + "Inside Bar (
-0001d7a0: 2564 2922 2025 2069 0a20 2020 2020 2020  %d)" % i.       
-0001d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7c0: 2072 6574 7572 6e20 690a 2020 2020 2020   return i.      
-0001d7d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0001d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7f0: 2020 2020 7265 7475 726e 2030 0a20 2020      return 0.   
-0001d800: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0001d810: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001d820: 6620 2244 6f77 6e22 2069 6e20 7361 7665  f "Down" in save
-0001d830: 4469 6374 5b22 5472 656e 6422 5d20 616e  Dict["Trend"] an
-0001d840: 6420 280a 2020 2020 2020 2020 2020 2020  d (.            
-0001d850: 2020 2020 2020 2020 2242 6561 7222 2069          "Bear" i
-0001d860: 6e20 7361 7665 4469 6374 5b22 4d41 2d53  n saveDict["MA-S
-0001d870: 6967 6e61 6c22 5d20 6f72 2022 5265 7369  ignal"] or "Resi
-0001d880: 7374 2220 696e 2073 6176 6544 6963 745b  st" in saveDict[
-0001d890: 224d 412d 5369 676e 616c 225d 0a20 2020  "MA-Signal"].   
-0001d8a0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
-0001d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d8c0: 2020 2020 6461 7461 203d 206f 7267 4461      data = orgDa
-0001d8d0: 7461 2e68 6561 6428 6929 0a20 2020 2020  ta.head(i).     
-0001d8e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001d8f0: 6566 4361 6e64 6c65 203d 2064 6174 612e  efCandle = data.
-0001d900: 7461 696c 2831 290a 2020 2020 2020 2020  tail(1).        
-0001d910: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-0001d920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d930: 2020 2020 2020 2020 2028 6c65 6e28 6461           (len(da
-0001d940: 7461 2e48 6967 685b 6461 7461 2e48 6967  ta.High[data.Hig
-0001d950: 6820 3e20 7265 6643 616e 646c 652e 4869  h > refCandle.Hi
-0001d960: 6768 2e69 7465 6d28 295d 2920 3d3d 2030  gh.item()]) == 0
-0001d970: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001d980: 2020 2020 2020 2020 2020 616e 6420 286c            and (l
-0001d990: 656e 2864 6174 612e 4c6f 775b 6461 7461  en(data.Low[data
-0001d9a0: 2e4c 6f77 203c 2072 6566 4361 6e64 6c65  .Low < refCandle
-0001d9b0: 2e4c 6f77 2e69 7465 6d28 295d 2920 3d3d  .Low.item()]) ==
-0001d9c0: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
-0001d9d0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0001d9e0: 286c 656e 2864 6174 612e 4f70 656e 5b64  (len(data.Open[d
-0001d9f0: 6174 612e 4f70 656e 203e 2072 6566 4361  ata.Open > refCa
-0001da00: 6e64 6c65 2e48 6967 682e 6974 656d 2829  ndle.High.item()
-0001da10: 5d29 203d 3d20 3029 0a20 2020 2020 2020  ]) == 0).       
-0001da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da30: 2061 6e64 2028 6c65 6e28 6461 7461 2e43   and (len(data.C
-0001da40: 6c6f 7365 5b64 6174 612e 436c 6f73 6520  lose[data.Close 
-0001da50: 3c20 7265 6643 616e 646c 652e 4c6f 772e  < refCandle.Low.
-0001da60: 6974 656d 2829 5d29 203d 3d20 3029 0a20  item()]) == 0). 
-0001da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da80: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-0001da90: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-0001daa0: 7265 656e 4469 6374 5b22 5061 7474 6572  reenDict["Patter
-0001dab0: 6e22 5d20 3d20 280a 2020 2020 2020 2020  n"] = (.        
-0001dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dad0: 2020 2020 7361 7665 645b 305d 0a20 2020      saved[0].   
-0001dae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001daf0: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-0001db00: 5465 7874 2e42 4f4c 440a 2020 2020 2020  Text.BOLD.      
+0001d750: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+0001d760: 7874 2e57 4152 4e0a 2020 2020 2020 2020  xt.WARN.        
+0001d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d780: 2020 2020 2b20 2822 496e 7369 6465 2042      + ("Inside B
+0001d790: 6172 2028 2564 2922 2025 2069 290a 2020  ar (%d)" % i).  
+0001d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d7b0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+0001d7c0: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+0001d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d7e0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001d7f0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+0001d800: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
+0001d810: 3d20 7361 7665 645b 315d 202b 2022 496e  = saved[1] + "In
+0001d820: 7369 6465 2042 6172 2028 2564 2922 2025  side Bar (%d)" %
+0001d830: 2069 0a20 2020 2020 2020 2020 2020 2020   i.             
+0001d840: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001d850: 6e20 690a 2020 2020 2020 2020 2020 2020  n i.            
+0001d860: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001d870: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001d880: 7475 726e 2030 0a20 2020 2020 2020 2020  turn 0.         
+0001d890: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001d8a0: 2020 2020 2020 2020 2069 6620 2244 6f77           if "Dow
+0001d8b0: 6e22 2069 6e20 7361 7665 4469 6374 5b22  n" in saveDict["
+0001d8c0: 5472 656e 6422 5d20 616e 6420 280a 2020  Trend"] and (.  
+0001d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8e0: 2020 2242 6561 7222 2069 6e20 7361 7665    "Bear" in save
+0001d8f0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+0001d900: 5d20 6f72 2022 5265 7369 7374 2220 696e  ] or "Resist" in
+0001d910: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
+0001d920: 676e 616c 225d 0a20 2020 2020 2020 2020  gnal"].         
+0001d930: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+0001d940: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0001d950: 7461 203d 206f 7267 4461 7461 2e68 6561  ta = orgData.hea
+0001d960: 6428 6929 0a20 2020 2020 2020 2020 2020  d(i).           
+0001d970: 2020 2020 2020 2020 2072 6566 4361 6e64           refCand
+0001d980: 6c65 203d 2064 6174 612e 7461 696c 2831  le = data.tail(1
+0001d990: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001d9a0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+0001d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d9c0: 2020 2028 6c65 6e28 6461 7461 2e48 6967     (len(data.Hig
+0001d9d0: 685b 6461 7461 2e48 6967 6820 3e20 7265  h[data.High > re
+0001d9e0: 6643 616e 646c 652e 4869 6768 2e69 7465  fCandle.High.ite
+0001d9f0: 6d28 295d 2920 3d3d 2030 290a 2020 2020  m()]) == 0).    
+0001da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da10: 2020 2020 616e 6420 286c 656e 2864 6174      and (len(dat
+0001da20: 612e 4c6f 775b 6461 7461 2e4c 6f77 203c  a.Low[data.Low <
+0001da30: 2072 6566 4361 6e64 6c65 2e4c 6f77 2e69   refCandle.Low.i
+0001da40: 7465 6d28 295d 2920 3d3d 2030 290a 2020  tem()]) == 0).  
+0001da50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da60: 2020 2020 2020 616e 6420 286c 656e 2864        and (len(d
+0001da70: 6174 612e 4f70 656e 5b64 6174 612e 4f70  ata.Open[data.Op
+0001da80: 656e 203e 2072 6566 4361 6e64 6c65 2e48  en > refCandle.H
+0001da90: 6967 682e 6974 656d 2829 5d29 203d 3d20  igh.item()]) == 
+0001daa0: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+0001dab0: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
+0001dac0: 6c65 6e28 6461 7461 2e43 6c6f 7365 5b64  len(data.Close[d
+0001dad0: 6174 612e 436c 6f73 6520 3c20 7265 6643  ata.Close < refC
+0001dae0: 616e 646c 652e 4c6f 772e 6974 656d 2829  andle.Low.item()
+0001daf0: 5d29 203d 3d20 3029 0a20 2020 2020 2020  ]) == 0).       
+0001db00: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
 0001db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db20: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-0001db30: 742e 5741 524e 0a20 2020 2020 2020 2020  t.WARN.         
-0001db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db50: 2020 202b 2028 2249 6e73 6964 6520 4261     + ("Inside Ba
-0001db60: 7220 2825 6429 2220 2520 6929 0a20 2020  r (%d)" % i).   
+0001db20: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+0001db30: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
+0001db40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001db50: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+0001db60: 7665 645b 305d 0a20 2020 2020 2020 2020  ved[0].         
 0001db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db80: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-0001db90: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+0001db80: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
+0001db90: 4f4c 440a 2020 2020 2020 2020 2020 2020  OLD.            
 0001dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dbb0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0001dbc0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-0001dbd0: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
-0001dbe0: 2073 6176 6564 5b31 5d20 2b20 2249 6e73   saved[1] + "Ins
-0001dbf0: 6964 6520 4261 7220 2825 6429 2220 2520  ide Bar (%d)" % 
-0001dc00: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
-0001dc10: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001dc20: 2069 0a20 2020 2020 2020 2020 2020 2020   i.             
-0001dc30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0001dc40: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0001dc50: 7572 6e20 300a 2020 2020 2020 2020 7265  urn 0.        re
-0001dc60: 7475 726e 2030 0a0a 2020 2020 2320 4669  turn 0..    # Fi
-0001dc70: 6e64 2049 504f 2062 6173 650a 2020 2020  nd IPO base.    
-0001dc80: 6465 6620 7661 6c69 6461 7465 4970 6f42  def validateIpoB
-0001dc90: 6173 6528 7365 6c66 2c20 7374 6f63 6b2c  ase(self, stock,
-0001dca0: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
-0001dcb0: 2073 6176 6544 6963 742c 2070 6572 6365   saveDict, perce
-0001dcc0: 6e74 6167 653d 302e 3329 3a0a 2020 2020  ntage=0.3):.    
-0001dcd0: 2020 2020 6966 2064 6620 6973 204e 6f6e      if df is Non
-0001dce0: 6520 6f72 206c 656e 2864 6629 203d 3d20  e or len(df) == 
-0001dcf0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-0001dd00: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-0001dd10: 2020 2020 6461 7461 203d 2064 662e 636f      data = df.co
-0001dd20: 7079 2829 0a20 2020 2020 2020 206c 6973  py().        lis
-0001dd30: 7469 6e67 5072 6963 6520 3d20 6461 7461  tingPrice = data
-0001dd40: 5b3a 3a2d 315d 2e68 6561 6428 3129 5b22  [::-1].head(1)["
-0001dd50: 4f70 656e 225d 2e69 6c6f 635b 305d 0a20  Open"].iloc[0]. 
-0001dd60: 2020 2020 2020 2063 7572 7265 6e74 5072         currentPr
-0001dd70: 6963 6520 3d20 6461 7461 2e68 6561 6428  ice = data.head(
-0001dd80: 3129 5b22 436c 6f73 6522 5d2e 696c 6f63  1)["Close"].iloc
-0001dd90: 5b30 5d0a 2020 2020 2020 2020 4154 4820  [0].        ATH 
-0001dda0: 3d20 6461 7461 2e64 6573 6372 6962 6528  = data.describe(
-0001ddb0: 295b 2248 6967 6822 5d5b 226d 6178 225d  )["High"]["max"]
-0001ddc0: 0a20 2020 2020 2020 2069 6620 4154 4820  .        if ATH 
-0001ddd0: 3e20 286c 6973 7469 6e67 5072 6963 6520  > (listingPrice 
-0001dde0: 2b20 286c 6973 7469 6e67 5072 6963 6520  + (listingPrice 
-0001ddf0: 2a20 7065 7263 656e 7461 6765 2929 3a0a  * percentage)):.
-0001de00: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001de10: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-0001de20: 2061 7761 7920 3d20 726f 756e 6428 2828   away = round(((
-0001de30: 6375 7272 656e 7450 7269 6365 202d 206c  currentPrice - l
-0001de40: 6973 7469 6e67 5072 6963 6529 202f 206c  istingPrice) / l
-0001de50: 6973 7469 6e67 5072 6963 6529 202a 2031  istingPrice) * 1
-0001de60: 3030 2c20 3129 0a20 2020 2020 2020 2069  00, 1).        i
-0001de70: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-0001de80: 286c 6973 7469 6e67 5072 6963 6520 2d20  (listingPrice - 
-0001de90: 286c 6973 7469 6e67 5072 6963 6520 2a20  (listingPrice * 
-0001dea0: 7065 7263 656e 7461 6765 2929 0a20 2020  percentage)).   
-0001deb0: 2020 2020 2020 2020 203c 3d20 6375 7272           <= curr
-0001dec0: 656e 7450 7269 6365 0a20 2020 2020 2020  entPrice.       
-0001ded0: 2020 2020 203c 3d20 286c 6973 7469 6e67       <= (listing
-0001dee0: 5072 6963 6520 2b20 286c 6973 7469 6e67  Price + (listing
-0001def0: 5072 6963 6520 2a20 7065 7263 656e 7461  Price * percenta
-0001df00: 6765 2929 0a20 2020 2020 2020 2029 3a0a  ge)).        ):.
-0001df10: 2020 2020 2020 2020 2020 2020 7361 7665              save
-0001df20: 6420 3d20 7365 6c66 2e66 696e 6443 7572  d = self.findCur
-0001df30: 7265 6e74 5361 7665 6456 616c 7565 2873  rentSavedValue(s
-0001df40: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-0001df50: 6963 742c 2022 5061 7474 6572 6e22 290a  ict, "Pattern").
-0001df60: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-0001df70: 7761 7920 3e20 303a 0a20 2020 2020 2020  way > 0:.       
-0001df80: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-0001df90: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
-0001dfa0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0001dfb0: 2020 2020 2020 2073 6176 6564 5b30 5d20         saved[0] 
-0001dfc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001dfd0: 2020 2020 202b 2063 6f6c 6f72 5465 7874       + colorText
-0001dfe0: 2e42 4f4c 440a 2020 2020 2020 2020 2020  .BOLD.          
-0001dff0: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-0001e000: 7254 6578 742e 4752 4545 4e0a 2020 2020  rText.GREEN.    
-0001e010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e020: 2b20 6622 4950 4f20 4261 7365 2028 7b61  + f"IPO Base ({a
-0001e030: 7761 797d 2025 2922 0a20 2020 2020 2020  way} %)".       
-0001e040: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-0001e050: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
-0001e060: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0001e070: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001e080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e090: 2073 6372 6565 6e44 6963 745b 2250 6174   screenDict["Pat
-0001e0a0: 7465 726e 225d 203d 2028 0a20 2020 2020  tern"] = (.     
-0001e0b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001e0c0: 6176 6564 5b30 5d0a 2020 2020 2020 2020  aved[0].        
-0001e0d0: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-0001e0e0: 6c6f 7254 6578 742e 424f 4c44 0a20 2020  lorText.BOLD.   
-0001e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e100: 202b 2063 6f6c 6f72 5465 7874 2e47 5245   + colorText.GRE
-0001e110: 454e 0a20 2020 2020 2020 2020 2020 2020  EN.             
-0001e120: 2020 2020 2020 202b 2022 4950 4f20 4261         + "IPO Ba
-0001e130: 7365 2022 0a20 2020 2020 2020 2020 2020  se ".           
-0001e140: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-0001e150: 5465 7874 2e46 4149 4c0a 2020 2020 2020  Text.FAIL.      
-0001e160: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-0001e170: 6622 287b 6177 6179 7d20 2529 220a 2020  f"({away} %)".  
-0001e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e190: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
-0001e1a0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-0001e1b0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0001e1c0: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
-0001e1d0: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
-0001e1e0: 2066 2249 504f 2042 6173 6520 287b 6177   f"IPO Base ({aw
-0001e1f0: 6179 7d20 2529 220a 2020 2020 2020 2020  ay} %)".        
-0001e200: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-0001e210: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0001e220: 616c 7365 0a0a 2020 2020 2340 6d65 6173  alse..    #@meas
-0001e230: 7572 655f 7469 6d65 0a20 2020 2023 2056  ure_time.    # V
-0001e240: 616c 6964 6174 6520 4c6f 7265 6e74 7a69  alidate Lorentzi
-0001e250: 616e 2043 6c61 7373 6966 6963 6174 696f  an Classificatio
-0001e260: 6e20 7369 676e 616c 0a20 2020 2064 6566  n signal.    def
-0001e270: 2076 616c 6964 6174 654c 6f72 656e 747a   validateLorentz
-0001e280: 6961 6e28 7365 6c66 2c20 6466 2c20 7363  ian(self, df, sc
-0001e290: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
-0001e2a0: 6374 2c20 6c6f 6f6b 466f 723d 3329 3a0a  ct, lookFor=3):.
-0001e2b0: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
-0001e2c0: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
-0001e2d0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-0001e2e0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-0001e2f0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0001e300: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-0001e310: 2023 206c 6f6f 6b46 6f72 3a20 312d 4275   # lookFor: 1-Bu
-0001e320: 792c 2032 2d53 656c 6c2c 2033 2d41 6e79  y, 2-Sell, 3-Any
-0001e330: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-0001e340: 6461 7461 5b3a 3a2d 315d 2020 2320 5265  data[::-1]  # Re
-0001e350: 7665 7273 6520 7468 6520 6461 7461 6672  verse the datafr
-0001e360: 616d 650a 2020 2020 2020 2020 6461 7461  ame.        data
-0001e370: 203d 2064 6174 612e 7265 6e61 6d65 280a   = data.rename(.
-0001e380: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-0001e390: 6d6e 733d 7b0a 2020 2020 2020 2020 2020  mns={.          
-0001e3a0: 2020 2020 2020 224f 7065 6e22 3a20 226f        "Open": "o
-0001e3b0: 7065 6e22 2c0a 2020 2020 2020 2020 2020  pen",.          
-0001e3c0: 2020 2020 2020 2243 6c6f 7365 223a 2022        "Close": "
-0001e3d0: 636c 6f73 6522 2c0a 2020 2020 2020 2020  close",.        
-0001e3e0: 2020 2020 2020 2020 2248 6967 6822 3a20          "High": 
-0001e3f0: 2268 6967 6822 2c0a 2020 2020 2020 2020  "high",.        
-0001e400: 2020 2020 2020 2020 224c 6f77 223a 2022          "Low": "
-0001e410: 6c6f 7722 2c0a 2020 2020 2020 2020 2020  low",.          
-0001e420: 2020 2020 2020 2256 6f6c 756d 6522 3a20        "Volume": 
-0001e430: 2276 6f6c 756d 6522 2c0a 2020 2020 2020  "volume",.      
-0001e440: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-0001e450: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
-0001e460: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0001e470: 5375 7070 7265 7373 4f75 7470 7574 2873  SuppressOutput(s
-0001e480: 7570 7072 6573 735f 7374 646f 7574 3d54  uppress_stdout=T
-0001e490: 7275 652c 2073 7570 7072 6573 735f 7374  rue, suppress_st
-0001e4a0: 6465 7272 3d54 7275 6529 3a0a 2020 2020  derr=True):.    
-0001e4b0: 2020 2020 2020 2020 2020 2020 6c63 203d              lc =
-0001e4c0: 2061 7461 2e4c 6f72 656e 747a 6961 6e43   ata.LorentzianC
-0001e4d0: 6c61 7373 6966 6963 6174 696f 6e28 6461  lassification(da
-0001e4e0: 7461 3d64 6174 6129 0a20 2020 2020 2020  ta=data).       
-0001e4f0: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
-0001e500: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
-0001e510: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
-0001e520: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
-0001e530: 6174 7465 726e 2229 0a20 2020 2020 2020  attern").       
-0001e540: 2020 2020 2069 6620 6c63 2e64 662e 696c       if lc.df.il
-0001e550: 6f63 5b2d 315d 5b22 6973 4e65 7742 7579  oc[-1]["isNewBuy
-0001e560: 5369 676e 616c 225d 3a0a 2020 2020 2020  Signal"]:.      
-0001e570: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-0001e580: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-0001e590: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0001e5a0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-0001e5b0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-0001e5c0: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
-0001e5d0: 4545 4e20 2b20 224c 6f72 656e 747a 6961  EEN + "Lorentzia
-0001e5e0: 6e2d 4275 7922 202b 2063 6f6c 6f72 5465  n-Buy" + colorTe
-0001e5f0: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
-0001e600: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001e610: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-0001e620: 745b 2250 6174 7465 726e 225d 203d 2073  t["Pattern"] = s
-0001e630: 6176 6564 5b31 5d20 2b20 224c 6f72 656e  aved[1] + "Loren
-0001e640: 747a 6961 6e2d 4275 7922 0a20 2020 2020  tzian-Buy".     
-0001e650: 2020 2020 2020 2020 2020 2069 6620 6c6f             if lo
-0001e660: 6f6b 466f 7220 213d 2032 3a20 2320 4e6f  okFor != 2: # No
-0001e670: 7420 5365 6c6c 0a20 2020 2020 2020 2020  t Sell.         
-0001e680: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0001e690: 6e20 5472 7565 0a20 2020 2020 2020 2020  n True.         
-0001e6a0: 2020 2065 6c69 6620 6c63 2e64 662e 696c     elif lc.df.il
-0001e6b0: 6f63 5b2d 315d 5b22 6973 4e65 7753 656c  oc[-1]["isNewSel
-0001e6c0: 6c53 6967 6e61 6c22 5d3a 0a20 2020 2020  lSignal"]:.     
-0001e6d0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-0001e6e0: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
-0001e6f0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-0001e700: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-0001e710: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
-0001e720: 4c44 202b 2063 6f6c 6f72 5465 7874 2e46  LD + colorText.F
-0001e730: 4149 4c20 2b20 224c 6f72 656e 747a 6961  AIL + "Lorentzia
-0001e740: 6e2d 5365 6c6c 2220 2b20 636f 6c6f 7254  n-Sell" + colorT
-0001e750: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
-0001e760: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0001e770: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-0001e780: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
-0001e790: 7361 7665 645b 315d 202b 2022 4c6f 7265  saved[1] + "Lore
-0001e7a0: 6e74 7a69 616e 2d53 656c 6c22 0a20 2020  ntzian-Sell".   
-0001e7b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001e7c0: 6c6f 6f6b 466f 7220 213d 2031 3a20 2320  lookFor != 1: # 
-0001e7d0: 4e6f 7420 4275 790a 2020 2020 2020 2020  Not Buy.        
-0001e7e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001e7f0: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-0001e800: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-0001e810: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
-0001e820: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
-0001e830: 2020 2320 5661 6c75 6545 7272 6f72 3a20    # ValueError: 
-0001e840: 6f70 6572 616e 6473 2063 6f75 6c64 206e  operands could n
-0001e850: 6f74 2062 6520 6272 6f61 6463 6173 7420  ot be broadcast 
-0001e860: 746f 6765 7468 6572 2077 6974 6820 7368  together with sh
-0001e870: 6170 6573 2028 3230 2c29 2028 3236 2c29  apes (20,) (26,)
-0001e880: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
-0001e890: 696c 6520 222f 6f70 742f 686f 6d65 6272  ile "/opt/homebr
-0001e8a0: 6577 2f6c 6962 2f70 7974 686f 6e33 2e31  ew/lib/python3.1
-0001e8b0: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
-0001e8c0: 6164 7661 6e63 6564 5f74 612f 4c6f 7265  advanced_ta/Lore
-0001e8d0: 6e74 7a69 616e 436c 6173 7369 6669 6361  ntzianClassifica
-0001e8e0: 7469 6f6e 2f43 6c61 7373 6966 6965 722e  tion/Classifier.
-0001e8f0: 7079 222c 206c 696e 6520 3138 362c 2069  py", line 186, i
-0001e900: 6e20 5f5f 696e 6974 5f5f 0a20 2020 2020  n __init__.     
+0001dbb0: 2b20 636f 6c6f 7254 6578 742e 5741 524e  + colorText.WARN
+0001dbc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001dbd0: 2020 2020 2020 2020 2020 2020 202b 2028               + (
+0001dbe0: 2249 6e73 6964 6520 4261 7220 2825 6429  "Inside Bar (%d)
+0001dbf0: 2220 2520 6929 0a20 2020 2020 2020 2020  " % i).         
+0001dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc10: 2020 202b 2063 6f6c 6f72 5465 7874 2e45     + colorText.E
+0001dc20: 4e44 0a20 2020 2020 2020 2020 2020 2020  ND.             
+0001dc30: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001dc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc50: 2020 2020 2073 6176 6544 6963 745b 2250       saveDict["P
+0001dc60: 6174 7465 726e 225d 203d 2073 6176 6564  attern"] = saved
+0001dc70: 5b31 5d20 2b20 2249 6e73 6964 6520 4261  [1] + "Inside Ba
+0001dc80: 7220 2825 6429 2220 2520 690a 2020 2020  r (%d)" % i.    
+0001dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dca0: 2020 2020 7265 7475 726e 2069 0a20 2020      return i.   
+0001dcb0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0001dcc0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001dcd0: 2020 2020 2020 2072 6574 7572 6e20 300a         return 0.
+0001dce0: 2020 2020 2020 2020 7265 7475 726e 2030          return 0
+0001dcf0: 0a0a 2020 2020 2320 4669 6e64 2049 504f  ..    # Find IPO
+0001dd00: 2062 6173 650a 2020 2020 6465 6620 7661   base.    def va
+0001dd10: 6c69 6461 7465 4970 6f42 6173 6528 7365  lidateIpoBase(se
+0001dd20: 6c66 2c20 7374 6f63 6b2c 2064 662c 2073  lf, stock, df, s
+0001dd30: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+0001dd40: 6963 742c 2070 6572 6365 6e74 6167 653d  ict, percentage=
+0001dd50: 302e 3329 3a0a 2020 2020 2020 2020 6966  0.3):.        if
+0001dd60: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
+0001dd70: 656e 2864 6629 203d 3d20 303a 0a20 2020  en(df) == 0:.   
+0001dd80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001dd90: 4661 6c73 650a 2020 2020 2020 2020 6461  False.        da
+0001dda0: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
+0001ddb0: 2020 2020 2020 206c 6973 7469 6e67 5072         listingPr
+0001ddc0: 6963 6520 3d20 6461 7461 5b3a 3a2d 315d  ice = data[::-1]
+0001ddd0: 2e68 6561 6428 3129 5b22 4f70 656e 225d  .head(1)["Open"]
+0001dde0: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
+0001ddf0: 2063 7572 7265 6e74 5072 6963 6520 3d20   currentPrice = 
+0001de00: 6461 7461 2e68 6561 6428 3129 5b22 436c  data.head(1)["Cl
+0001de10: 6f73 6522 5d2e 696c 6f63 5b30 5d0a 2020  ose"].iloc[0].  
+0001de20: 2020 2020 2020 4154 4820 3d20 6461 7461        ATH = data
+0001de30: 2e64 6573 6372 6962 6528 295b 2248 6967  .describe()["Hig
+0001de40: 6822 5d5b 226d 6178 225d 0a20 2020 2020  h"]["max"].     
+0001de50: 2020 2069 6620 4154 4820 3e20 286c 6973     if ATH > (lis
+0001de60: 7469 6e67 5072 6963 6520 2b20 286c 6973  tingPrice + (lis
+0001de70: 7469 6e67 5072 6963 6520 2a20 7065 7263  tingPrice * perc
+0001de80: 656e 7461 6765 2929 3a0a 2020 2020 2020  entage)):.      
+0001de90: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+0001dea0: 7365 0a20 2020 2020 2020 2061 7761 7920  se.        away 
+0001deb0: 3d20 726f 756e 6428 2828 6375 7272 656e  = round(((curren
+0001dec0: 7450 7269 6365 202d 206c 6973 7469 6e67  tPrice - listing
+0001ded0: 5072 6963 6529 202f 206c 6973 7469 6e67  Price) / listing
+0001dee0: 5072 6963 6529 202a 2031 3030 2c20 3129  Price) * 100, 1)
+0001def0: 0a20 2020 2020 2020 2069 6620 280a 2020  .        if (.  
+0001df00: 2020 2020 2020 2020 2020 286c 6973 7469            (listi
+0001df10: 6e67 5072 6963 6520 2d20 286c 6973 7469  ngPrice - (listi
+0001df20: 6e67 5072 6963 6520 2a20 7065 7263 656e  ngPrice * percen
+0001df30: 7461 6765 2929 0a20 2020 2020 2020 2020  tage)).         
+0001df40: 2020 203c 3d20 6375 7272 656e 7450 7269     <= currentPri
+0001df50: 6365 0a20 2020 2020 2020 2020 2020 203c  ce.            <
+0001df60: 3d20 286c 6973 7469 6e67 5072 6963 6520  = (listingPrice 
+0001df70: 2b20 286c 6973 7469 6e67 5072 6963 6520  + (listingPrice 
+0001df80: 2a20 7065 7263 656e 7461 6765 2929 0a20  * percentage)). 
+0001df90: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+0001dfa0: 2020 2020 2020 7361 7665 6420 3d20 7365        saved = se
+0001dfb0: 6c66 2e66 696e 6443 7572 7265 6e74 5361  lf.findCurrentSa
+0001dfc0: 7665 6456 616c 7565 2873 6372 6565 6e44  vedValue(screenD
+0001dfd0: 6963 742c 2073 6176 6544 6963 742c 2022  ict, saveDict, "
+0001dfe0: 5061 7474 6572 6e22 290a 2020 2020 2020  Pattern").      
+0001dff0: 2020 2020 2020 6966 2061 7761 7920 3e20        if away > 
+0001e000: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+0001e010: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
+0001e020: 6174 7465 726e 225d 203d 2028 0a20 2020  attern"] = (.   
+0001e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e040: 2073 6176 6564 5b30 5d20 0a20 2020 2020   saved[0] .     
+0001e050: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+0001e060: 2063 6f6c 6f72 5465 7874 2e42 4f4c 440a   colorText.BOLD.
+0001e070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e080: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+0001e090: 4752 4545 4e0a 2020 2020 2020 2020 2020  GREEN.          
+0001e0a0: 2020 2020 2020 2020 2020 2b20 6622 4950            + f"IP
+0001e0b0: 4f20 4261 7365 2028 7b61 7761 797d 2025  O Base ({away} %
+0001e0c0: 2922 0a20 2020 2020 2020 2020 2020 2020  )".             
+0001e0d0: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+0001e0e0: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
+0001e0f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0001e100: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001e110: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+0001e120: 6e44 6963 745b 2250 6174 7465 726e 225d  nDict["Pattern"]
+0001e130: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+0001e140: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
+0001e150: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0001e160: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+0001e170: 742e 424f 4c44 0a20 2020 2020 2020 2020  t.BOLD.         
+0001e180: 2020 2020 2020 2020 2020 202b 2063 6f6c             + col
+0001e190: 6f72 5465 7874 2e47 5245 454e 0a20 2020  orText.GREEN.   
+0001e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1b0: 202b 2022 4950 4f20 4261 7365 2022 0a20   + "IPO Base ". 
+0001e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1d0: 2020 202b 2063 6f6c 6f72 5465 7874 2e46     + colorText.F
+0001e1e0: 4149 4c0a 2020 2020 2020 2020 2020 2020  AIL.            
+0001e1f0: 2020 2020 2020 2020 2b20 6622 287b 6177          + f"({aw
+0001e200: 6179 7d20 2529 220a 2020 2020 2020 2020  ay} %)".        
+0001e210: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+0001e220: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
+0001e230: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0001e240: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
+0001e250: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
+0001e260: 7361 7665 645b 315d 202b 2066 2249 504f  saved[1] + f"IPO
+0001e270: 2042 6173 6520 287b 6177 6179 7d20 2529   Base ({away} %)
+0001e280: 220a 2020 2020 2020 2020 2020 2020 7265  ".            re
+0001e290: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+0001e2a0: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
+0001e2b0: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
+0001e2c0: 6d65 0a20 2020 2023 2056 616c 6964 6174  me.    # Validat
+0001e2d0: 6520 4c6f 7265 6e74 7a69 616e 2043 6c61  e Lorentzian Cla
+0001e2e0: 7373 6966 6963 6174 696f 6e20 7369 676e  ssification sign
+0001e2f0: 616c 0a20 2020 2064 6566 2076 616c 6964  al.    def valid
+0001e300: 6174 654c 6f72 656e 747a 6961 6e28 7365  ateLorentzian(se
+0001e310: 6c66 2c20 6466 2c20 7363 7265 656e 4469  lf, df, screenDi
+0001e320: 6374 2c20 7361 7665 4469 6374 2c20 6c6f  ct, saveDict, lo
+0001e330: 6f6b 466f 723d 3329 3a0a 2020 2020 2020  okFor=3):.      
+0001e340: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
+0001e350: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
+0001e360: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0001e370: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+0001e380: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
+0001e390: 2829 0a20 2020 2020 2020 2023 206c 6f6f  ().        # loo
+0001e3a0: 6b46 6f72 3a20 312d 4275 792c 2032 2d53  kFor: 1-Buy, 2-S
+0001e3b0: 656c 6c2c 2033 2d41 6e79 0a20 2020 2020  ell, 3-Any.     
+0001e3c0: 2020 2064 6174 6120 3d20 6461 7461 5b3a     data = data[:
+0001e3d0: 3a2d 315d 2020 2320 5265 7665 7273 6520  :-1]  # Reverse 
+0001e3e0: 7468 6520 6461 7461 6672 616d 650a 2020  the dataframe.  
+0001e3f0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+0001e400: 612e 7265 6e61 6d65 280a 2020 2020 2020  a.rename(.      
+0001e410: 2020 2020 2020 636f 6c75 6d6e 733d 7b0a        columns={.
+0001e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e430: 224f 7065 6e22 3a20 226f 7065 6e22 2c0a  "Open": "open",.
+0001e440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e450: 2243 6c6f 7365 223a 2022 636c 6f73 6522  "Close": "close"
+0001e460: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001e470: 2020 2248 6967 6822 3a20 2268 6967 6822    "High": "high"
+0001e480: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001e490: 2020 224c 6f77 223a 2022 6c6f 7722 2c0a    "Low": "low",.
+0001e4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e4b0: 2256 6f6c 756d 6522 3a20 2276 6f6c 756d  "Volume": "volum
+0001e4c0: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+0001e4d0: 7d0a 2020 2020 2020 2020 290a 2020 2020  }.        ).    
+0001e4e0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0001e4f0: 2020 2020 2077 6974 6820 5375 7070 7265       with Suppre
+0001e500: 7373 4f75 7470 7574 2873 7570 7072 6573  ssOutput(suppres
+0001e510: 735f 7374 646f 7574 3d54 7275 652c 2073  s_stdout=True, s
+0001e520: 7570 7072 6573 735f 7374 6465 7272 3d54  uppress_stderr=T
+0001e530: 7275 6529 3a0a 2020 2020 2020 2020 2020  rue):.          
+0001e540: 2020 2020 2020 6c63 203d 2061 7461 2e4c        lc = ata.L
+0001e550: 6f72 656e 747a 6961 6e43 6c61 7373 6966  orentzianClassif
+0001e560: 6963 6174 696f 6e28 6461 7461 3d64 6174  ication(data=dat
+0001e570: 6129 0a20 2020 2020 2020 2020 2020 2073  a).            s
+0001e580: 6176 6564 203d 2073 656c 662e 6669 6e64  aved = self.find
+0001e590: 4375 7272 656e 7453 6176 6564 5661 6c75  CurrentSavedValu
+0001e5a0: 6528 7363 7265 656e 4469 6374 2c20 7361  e(screenDict, sa
+0001e5b0: 7665 4469 6374 2c20 2250 6174 7465 726e  veDict, "Pattern
+0001e5c0: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+0001e5d0: 6620 6c63 2e64 662e 696c 6f63 5b2d 315d  f lc.df.iloc[-1]
+0001e5e0: 5b22 6973 4e65 7742 7579 5369 676e 616c  ["isNewBuySignal
+0001e5f0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+0001e600: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+0001e610: 5061 7474 6572 6e22 5d20 3d20 280a 2020  Pattern"] = (.  
+0001e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e630: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
+0001e640: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
+0001e650: 6c6f 7254 6578 742e 4752 4545 4e20 2b20  lorText.GREEN + 
+0001e660: 224c 6f72 656e 747a 6961 6e2d 4275 7922  "Lorentzian-Buy"
+0001e670: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+0001e680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e690: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0001e6a0: 2020 2073 6176 6544 6963 745b 2250 6174     saveDict["Pat
+0001e6b0: 7465 726e 225d 203d 2073 6176 6564 5b31  tern"] = saved[1
+0001e6c0: 5d20 2b20 224c 6f72 656e 747a 6961 6e2d  ] + "Lorentzian-
+0001e6d0: 4275 7922 0a20 2020 2020 2020 2020 2020  Buy".           
+0001e6e0: 2020 2020 2069 6620 6c6f 6f6b 466f 7220       if lookFor 
+0001e6f0: 213d 2032 3a20 2320 4e6f 7420 5365 6c6c  != 2: # Not Sell
+0001e700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e710: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+0001e720: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0001e730: 6620 6c63 2e64 662e 696c 6f63 5b2d 315d  f lc.df.iloc[-1]
+0001e740: 5b22 6973 4e65 7753 656c 6c53 6967 6e61  ["isNewSellSigna
+0001e750: 6c22 5d3a 0a20 2020 2020 2020 2020 2020  l"]:.           
+0001e760: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+0001e770: 2250 6174 7465 726e 225d 203d 2028 0a20  "Pattern"] = (. 
+0001e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e790: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
+0001e7a0: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
+0001e7b0: 6f6c 6f72 5465 7874 2e46 4149 4c20 2b20  olorText.FAIL + 
+0001e7c0: 224c 6f72 656e 747a 6961 6e2d 5365 6c6c  "Lorentzian-Sell
+0001e7d0: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
+0001e7e0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+0001e7f0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001e800: 2020 2020 7361 7665 4469 6374 5b22 5061      saveDict["Pa
+0001e810: 7474 6572 6e22 5d20 3d20 7361 7665 645b  ttern"] = saved[
+0001e820: 315d 202b 2022 4c6f 7265 6e74 7a69 616e  1] + "Lorentzian
+0001e830: 2d53 656c 6c22 0a20 2020 2020 2020 2020  -Sell".         
+0001e840: 2020 2020 2020 2069 6620 6c6f 6f6b 466f         if lookFo
+0001e850: 7220 213d 2031 3a20 2320 4e6f 7420 4275  r != 1: # Not Bu
+0001e860: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+0001e870: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0001e880: 650a 2020 2020 2020 2020 6578 6365 7074  e.        except
+0001e890: 2045 7863 6570 7469 6f6e 3a20 2023 2070   Exception:  # p
+0001e8a0: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
+0001e8b0: 2020 2020 2020 2020 2020 2020 2320 5661              # Va
+0001e8c0: 6c75 6545 7272 6f72 3a20 6f70 6572 616e  lueError: operan
+0001e8d0: 6473 2063 6f75 6c64 206e 6f74 2062 6520  ds could not be 
+0001e8e0: 6272 6f61 6463 6173 7420 746f 6765 7468  broadcast togeth
+0001e8f0: 6572 2077 6974 6820 7368 6170 6573 2028  er with shapes (
+0001e900: 3230 2c29 2028 3236 2c29 0a20 2020 2020  20,) (26,).     
 0001e910: 2020 2020 2020 2023 2046 696c 6520 222f         # File "/
 0001e920: 6f70 742f 686f 6d65 6272 6577 2f6c 6962  opt/homebrew/lib
 0001e930: 2f70 7974 686f 6e33 2e31 312f 7369 7465  /python3.11/site
 0001e940: 2d70 6163 6b61 6765 732f 6164 7661 6e63  -packages/advanc
 0001e950: 6564 5f74 612f 4c6f 7265 6e74 7a69 616e  ed_ta/Lorentzian
 0001e960: 436c 6173 7369 6669 6361 7469 6f6e 2f43  Classification/C
 0001e970: 6c61 7373 6966 6965 722e 7079 222c 206c  lassifier.py", l
-0001e980: 696e 6520 3339 352c 2069 6e20 5f5f 636c  ine 395, in __cl
-0001e990: 6173 7369 6679 0a20 2020 2020 2020 2020  assify.         
-0001e9a0: 2020 2023 2046 696c 6520 222f 6f70 742f     # File "/opt/
-0001e9b0: 686f 6d65 6272 6577 2f6c 6962 2f70 7974  homebrew/lib/pyt
-0001e9c0: 686f 6e33 2e31 312f 7369 7465 2d70 6163  hon3.11/site-pac
-0001e9d0: 6b61 6765 732f 7061 6e64 6173 2f63 6f72  kages/pandas/cor
-0001e9e0: 652f 6f70 732f 636f 6d6d 6f6e 2e70 7922  e/ops/common.py"
-0001e9f0: 2c20 6c69 6e65 2037 362c 2069 6e20 6e65  , line 76, in ne
-0001ea00: 775f 6d65 7468 6f64 0a20 2020 2020 2020  w_method.       
-0001ea10: 2020 2020 2023 2046 696c 6520 222f 6f70       # File "/op
-0001ea20: 742f 686f 6d65 6272 6577 2f6c 6962 2f70  t/homebrew/lib/p
-0001ea30: 7974 686f 6e33 2e31 312f 7369 7465 2d70  ython3.11/site-p
-0001ea40: 6163 6b61 6765 732f 7061 6e64 6173 2f63  ackages/pandas/c
-0001ea50: 6f72 652f 6172 7261 796c 696b 652e 7079  ore/arraylike.py
-0001ea60: 222c 206c 696e 6520 3730 2c20 696e 205f  ", line 70, in _
-0001ea70: 5f61 6e64 5f5f 0a20 2020 2020 2020 2020  _and__.         
-0001ea80: 2020 2023 2046 696c 6520 222f 6f70 742f     # File "/opt/
-0001ea90: 686f 6d65 6272 6577 2f6c 6962 2f70 7974  homebrew/lib/pyt
-0001eaa0: 686f 6e33 2e31 312f 7369 7465 2d70 6163  hon3.11/site-pac
-0001eab0: 6b61 6765 732f 7061 6e64 6173 2f63 6f72  kages/pandas/cor
-0001eac0: 652f 7365 7269 6573 2e70 7922 2c20 6c69  e/series.py", li
-0001ead0: 6e65 2035 3831 302c 2069 6e20 5f6c 6f67  ne 5810, in _log
-0001eae0: 6963 616c 5f6d 6574 686f 640a 2020 2020  ical_method.    
-0001eaf0: 2020 2020 2020 2020 2320 4669 6c65 2022          # File "
-0001eb00: 2f6f 7074 2f68 6f6d 6562 7265 772f 6c69  /opt/homebrew/li
-0001eb10: 622f 7079 7468 6f6e 332e 3131 2f73 6974  b/python3.11/sit
-0001eb20: 652d 7061 636b 6167 6573 2f70 616e 6461  e-packages/panda
-0001eb30: 732f 636f 7265 2f6f 7073 2f61 7272 6179  s/core/ops/array
-0001eb40: 5f6f 7073 2e70 7922 2c20 6c69 6e65 2034  _ops.py", line 4
-0001eb50: 3536 2c20 696e 206c 6f67 6963 616c 5f6f  56, in logical_o
-0001eb60: 700a 2020 2020 2020 2020 2020 2020 2320  p.            # 
-0001eb70: 4669 6c65 2022 2f6f 7074 2f68 6f6d 6562  File "/opt/homeb
-0001eb80: 7265 772f 6c69 622f 7079 7468 6f6e 332e  rew/lib/python3.
-0001eb90: 3131 2f73 6974 652d 7061 636b 6167 6573  11/site-packages
-0001eba0: 2f70 616e 6461 732f 636f 7265 2f6f 7073  /pandas/core/ops
-0001ebb0: 2f61 7272 6179 5f6f 7073 2e70 7922 2c20  /array_ops.py", 
-0001ebc0: 6c69 6e65 2033 3634 2c20 696e 206e 615f  line 364, in na_
-0001ebd0: 6c6f 6769 6361 6c5f 6f70 0a20 2020 2020  logical_op.     
-0001ebe0: 2020 2020 2020 2023 2073 656c 662e 6465         # self.de
-0001ebf0: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-0001ec00: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
-0001ec10: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-0001ec20: 2070 6173 730a 2020 2020 2020 2020 7265   pass.        re
-0001ec30: 7475 726e 2046 616c 7365 0a0a 2020 2020  turn False..    
-0001ec40: 2320 7661 6c69 6461 7465 2069 6620 7468  # validate if th
-0001ec50: 6520 7374 6f63 6b20 6861 7320 6265 656e  e stock has been
-0001ec60: 2068 6176 696e 6720 6c6f 7765 7220 6c6f   having lower lo
-0001ec70: 7773 2c20 6c6f 7765 7220 6869 6768 730a  ws, lower highs.
-0001ec80: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0001ec90: 4c6f 7765 7248 6967 6873 4c6f 7765 724c  LowerHighsLowerL
-0001eca0: 6f77 7328 7365 6c66 2c20 6466 293a 0a20  ows(self, df):. 
-0001ecb0: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
-0001ecc0: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
-0001ecd0: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-0001ece0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-0001ecf0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
-0001ed00: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
-0001ed10: 6461 7930 203d 2064 6174 610a 2020 2020  day0 = data.    
-0001ed20: 2020 2020 6461 7931 203d 2064 6174 615b      day1 = data[
-0001ed30: 313a 5d0a 2020 2020 2020 2020 6461 7932  1:].        day2
-0001ed40: 203d 2064 6174 615b 323a 5d0a 2020 2020   = data[2:].    
-0001ed50: 2020 2020 6461 7933 203d 2064 6174 615b      day3 = data[
-0001ed60: 333a 5d0a 2020 2020 2020 2020 6c6f 7765  3:].        lowe
-0001ed70: 7248 6967 6873 203d 2028 0a20 2020 2020  rHighs = (.     
-0001ed80: 2020 2020 2020 2028 6461 7930 5b22 4869         (day0["Hi
-0001ed90: 6768 225d 2e69 6c6f 635b 305d 203c 2064  gh"].iloc[0] < d
-0001eda0: 6179 315b 2248 6967 6822 5d2e 696c 6f63  ay1["High"].iloc
-0001edb0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-0001edc0: 2061 6e64 2028 6461 7931 5b22 4869 6768   and (day1["High
-0001edd0: 225d 2e69 6c6f 635b 305d 203c 2064 6179  "].iloc[0] < day
-0001ede0: 325b 2248 6967 6822 5d2e 696c 6f63 5b30  2["High"].iloc[0
-0001edf0: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
-0001ee00: 6e64 2028 6461 7932 5b22 4869 6768 225d  nd (day2["High"]
-0001ee10: 2e69 6c6f 635b 305d 203c 2064 6179 335b  .iloc[0] < day3[
-0001ee20: 2248 6967 6822 5d2e 696c 6f63 5b30 5d29  "High"].iloc[0])
-0001ee30: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0001ee40: 2020 206c 6f77 6572 4c6f 7773 203d 2028     lowerLows = (
-0001ee50: 0a20 2020 2020 2020 2020 2020 2028 6461  .            (da
-0001ee60: 7930 5b22 4c6f 7722 5d2e 696c 6f63 5b30  y0["Low"].iloc[0
-0001ee70: 5d20 3c20 6461 7931 5b22 4c6f 7722 5d2e  ] < day1["Low"].
-0001ee80: 696c 6f63 5b30 5d29 0a20 2020 2020 2020  iloc[0]).       
-0001ee90: 2020 2020 2061 6e64 2028 6461 7931 5b22       and (day1["
-0001eea0: 4c6f 7722 5d2e 696c 6f63 5b30 5d20 3c20  Low"].iloc[0] < 
-0001eeb0: 6461 7932 5b22 4c6f 7722 5d2e 696c 6f63  day2["Low"].iloc
-0001eec0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-0001eed0: 2061 6e64 2028 6461 7932 5b22 4c6f 7722   and (day2["Low"
-0001eee0: 5d2e 696c 6f63 5b30 5d20 3c20 6461 7933  ].iloc[0] < day3
-0001eef0: 5b22 4c6f 7722 5d2e 696c 6f63 5b30 5d29  ["Low"].iloc[0])
-0001ef00: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0001ef10: 2020 2068 6967 6865 7252 5349 203d 2028     higherRSI = (
-0001ef20: 0a20 2020 2020 2020 2020 2020 2028 6461  .            (da
-0001ef30: 7930 5b22 5253 4922 5d2e 696c 6f63 5b30  y0["RSI"].iloc[0
-0001ef40: 5d20 3c20 6461 7931 5b22 5253 4922 5d2e  ] < day1["RSI"].
-0001ef50: 696c 6f63 5b30 5d29 0a20 2020 2020 2020  iloc[0]).       
-0001ef60: 2020 2020 2061 6e64 2028 6461 7931 5b22       and (day1["
-0001ef70: 5253 4922 5d2e 696c 6f63 5b30 5d20 3c20  RSI"].iloc[0] < 
-0001ef80: 6461 7932 5b22 5253 4922 5d2e 696c 6f63  day2["RSI"].iloc
-0001ef90: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
-0001efa0: 2061 6e64 2028 6461 7932 5b22 5253 4922   and (day2["RSI"
-0001efb0: 5d2e 696c 6f63 5b30 5d20 3c20 6461 7933  ].iloc[0] < day3
-0001efc0: 5b22 5253 4922 5d2e 696c 6f63 5b30 5d29  ["RSI"].iloc[0])
-0001efd0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-0001efe0: 2064 6179 305b 2252 5349 225d 2e69 6c6f   day0["RSI"].ilo
-0001eff0: 635b 305d 203e 3d20 3530 0a20 2020 2020  c[0] >= 50.     
-0001f000: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-0001f010: 7572 6e20 6c6f 7765 7248 6967 6873 2061  urn lowerHighs a
-0001f020: 6e64 206c 6f77 6572 4c6f 7773 2061 6e64  nd lowerLows and
-0001f030: 2068 6967 6865 7252 5349 0a0a 2020 2020   higherRSI..    
-0001f040: 2320 5661 6c69 6461 7465 2069 6620 7265  # Validate if re
-0001f050: 6365 6e74 2076 6f6c 756d 6520 6973 206c  cent volume is l
-0001f060: 6f77 6573 7420 6f66 206c 6173 7420 274e  owest of last 'N
-0001f070: 2720 4461 7973 0a20 2020 2064 6566 2076  ' Days.    def v
-0001f080: 616c 6964 6174 654c 6f77 6573 7456 6f6c  alidateLowestVol
-0001f090: 756d 6528 7365 6c66 2c20 6466 2c20 6461  ume(self, df, da
-0001f0a0: 7973 466f 724c 6f77 6573 7456 6f6c 756d  ysForLowestVolum
-0001f0b0: 6529 3a0a 2020 2020 2020 2020 6966 2064  e):.        if d
-0001f0c0: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-0001f0d0: 2864 6629 203d 3d20 303a 0a20 2020 2020  (df) == 0:.     
-0001f0e0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-0001f0f0: 6c73 650a 2020 2020 2020 2020 6461 7461  lse.        data
-0001f100: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
-0001f110: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
-0001f120: 2e66 696c 6c6e 6128 3029 0a20 2020 2020  .fillna(0).     
-0001f130: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
-0001f140: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
-0001f150: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
-0001f160: 2020 2020 2069 6620 6461 7973 466f 724c       if daysForL
-0001f170: 6f77 6573 7456 6f6c 756d 6520 6973 204e  owestVolume is N
-0001f180: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0001f190: 2064 6179 7346 6f72 4c6f 7765 7374 566f   daysForLowestVo
-0001f1a0: 6c75 6d65 203d 2033 300a 2020 2020 2020  lume = 30.      
-0001f1b0: 2020 6966 206c 656e 2864 6174 6129 203c    if len(data) <
-0001f1c0: 2064 6179 7346 6f72 4c6f 7765 7374 566f   daysForLowestVo
-0001f1d0: 6c75 6d65 3a0a 2020 2020 2020 2020 2020  lume:.          
-0001f1e0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-0001f1f0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-0001f200: 7461 2e68 6561 6428 6461 7973 466f 724c  ta.head(daysForL
-0001f210: 6f77 6573 7456 6f6c 756d 6529 0a20 2020  owestVolume).   
-0001f220: 2020 2020 2072 6563 656e 7420 3d20 6461       recent = da
-0001f230: 7461 2e68 6561 6428 3129 0a20 2020 2020  ta.head(1).     
-0001f240: 2020 2069 6620 6c65 6e28 7265 6365 6e74     if len(recent
-0001f250: 2920 3c20 313a 0a20 2020 2020 2020 2020  ) < 1:.         
-0001f260: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-0001f270: 2020 2020 2020 2020 6966 2028 7265 6365          if (rece
-0001f280: 6e74 5b22 566f 6c75 6d65 225d 2e69 6c6f  nt["Volume"].ilo
-0001f290: 635b 305d 203c 3d20 6461 7461 2e64 6573  c[0] <= data.des
-0001f2a0: 6372 6962 6528 295b 2256 6f6c 756d 6522  cribe()["Volume"
-0001f2b0: 5d5b 226d 696e 225d 2920 616e 6420 7265  ]["min"]) and re
-0001f2c0: 6365 6e74 5b0a 2020 2020 2020 2020 2020  cent[.          
-0001f2d0: 2020 2256 6f6c 756d 6522 0a20 2020 2020    "Volume".     
-0001f2e0: 2020 205d 5b30 5d20 213d 206e 702e 6e61     ][0] != np.na
-0001f2f0: 6e3a 0a20 2020 2020 2020 2020 2020 2072  n:.            r
-0001f300: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-0001f310: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-0001f320: 0a20 2020 2023 2056 616c 6964 6174 6520  .    # Validate 
-0001f330: 4c54 5020 7769 7468 696e 206c 696d 6974  LTP within limit
-0001f340: 730a 2020 2020 6465 6620 7661 6c69 6461  s.    def valida
-0001f350: 7465 4c54 5028 7365 6c66 2c20 6466 2c20  teLTP(self, df, 
-0001f360: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
-0001f370: 4469 6374 2c20 6d69 6e4c 5450 3d4e 6f6e  Dict, minLTP=Non
-0001f380: 652c 206d 6178 4c54 503d 4e6f 6e65 2c6d  e, maxLTP=None,m
-0001f390: 696e 4368 616e 6765 3d30 293a 0a20 2020  inChange=0):.   
-0001f3a0: 2020 2020 2064 6174 6120 3d20 6466 2e63       data = df.c
-0001f3b0: 6f70 7928 290a 2020 2020 2020 2020 6c74  opy().        lt
-0001f3c0: 7056 616c 6964 203d 2046 616c 7365 0a20  pValid = False. 
-0001f3d0: 2020 2020 2020 2069 6620 6d69 6e4c 5450         if minLTP
-0001f3e0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0001f3f0: 2020 2020 2020 6d69 6e4c 5450 203d 2073        minLTP = s
-0001f400: 656c 662e 636f 6e66 6967 4d61 6e61 6765  elf.configManage
-0001f410: 722e 6d69 6e4c 5450 0a20 2020 2020 2020  r.minLTP.       
-0001f420: 2069 6620 6d61 784c 5450 2069 7320 4e6f   if maxLTP is No
-0001f430: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0001f440: 6d61 784c 5450 203d 2073 656c 662e 636f  maxLTP = self.co
-0001f450: 6e66 6967 4d61 6e61 6765 722e 6d61 784c  nfigManager.maxL
-0001f460: 5450 0a20 2020 2020 2020 2064 6174 6120  TP.        data 
-0001f470: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
-0001f480: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-0001f490: 6461 7461 2e72 6570 6c61 6365 285b 6e70  data.replace([np
-0001f4a0: 2e69 6e66 2c20 2d6e 702e 696e 665d 2c20  .inf, -np.inf], 
-0001f4b0: 3029 0a20 2020 2020 2020 2072 6563 656e  0).        recen
-0001f4c0: 7420 3d20 6461 7461 2e68 6561 6428 3129  t = data.head(1)
-0001f4d0: 0a0a 2020 2020 2020 2020 7063 745f 6368  ..        pct_ch
-0001f4e0: 616e 6765 203d 2028 6461 7461 5b3a 3a2d  ange = (data[::-
-0001f4f0: 315d 5b22 436c 6f73 6522 5d2e 7063 745f  1]["Close"].pct_
-0001f500: 6368 616e 6765 2829 202a 2031 3030 292e  change() * 100).
-0001f510: 696c 6f63 5b2d 315d 0a20 2020 2020 2020  iloc[-1].       
-0001f520: 2069 6620 7063 745f 6368 616e 6765 203d   if pct_change =
-0001f530: 3d20 6e70 2e69 6e66 206f 7220 7063 745f  = np.inf or pct_
-0001f540: 6368 616e 6765 203d 3d20 2d6e 702e 696e  change == -np.in
-0001f550: 663a 0a20 2020 2020 2020 2020 2020 2070  f:.            p
-0001f560: 6374 5f63 6861 6e67 6520 3d20 300a 2020  ct_change = 0.  
-0001f570: 2020 2020 2020 7063 745f 7361 7665 203d        pct_save =
-0001f580: 2022 252e 3166 2525 2220 2520 7063 745f   "%.1f%%" % pct_
-0001f590: 6368 616e 6765 0a20 2020 2020 2020 2069  change.        i
-0001f5a0: 6620 7063 745f 6368 616e 6765 203e 2030  f pct_change > 0
-0001f5b0: 2e32 3a0a 2020 2020 2020 2020 2020 2020  .2:.            
-0001f5c0: 7063 745f 6368 616e 6765 203d 2063 6f6c  pct_change = col
-0001f5d0: 6f72 5465 7874 2e47 5245 454e 202b 2028  orText.GREEN + (
-0001f5e0: 2225 2e31 6625 2522 2025 2070 6374 5f63  "%.1f%%" % pct_c
-0001f5f0: 6861 6e67 6529 202b 2063 6f6c 6f72 5465  hange) + colorTe
-0001f600: 7874 2e45 4e44 0a20 2020 2020 2020 2065  xt.END.        e
-0001f610: 6c69 6620 7063 745f 6368 616e 6765 203c  lif pct_change <
-0001f620: 202d 302e 323a 0a20 2020 2020 2020 2020   -0.2:.         
-0001f630: 2020 2070 6374 5f63 6861 6e67 6520 3d20     pct_change = 
-0001f640: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
-0001f650: 2028 2225 2e31 6625 2522 2025 2070 6374   ("%.1f%%" % pct
-0001f660: 5f63 6861 6e67 6529 202b 2063 6f6c 6f72  _change) + color
-0001f670: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-0001f680: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001f690: 2020 2070 6374 5f63 6861 6e67 6520 3d20     pct_change = 
-0001f6a0: 636f 6c6f 7254 6578 742e 5741 524e 202b  colorText.WARN +
-0001f6b0: 2028 2225 2e31 6625 2522 2025 2070 6374   ("%.1f%%" % pct
-0001f6c0: 5f63 6861 6e67 6529 202b 2063 6f6c 6f72  _change) + color
-0001f6d0: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
-0001f6e0: 2073 6176 6544 6963 745b 2225 4368 6e67   saveDict["%Chng
-0001f6f0: 225d 203d 2070 6374 5f73 6176 650a 2020  "] = pct_save.  
-0001f700: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
-0001f710: 5b22 2543 686e 6722 5d20 3d20 7063 745f  ["%Chng"] = pct_
-0001f720: 6368 616e 6765 0a20 2020 2020 2020 206c  change.        l
-0001f730: 7470 203d 2072 6f75 6e64 2872 6563 656e  tp = round(recen
-0001f740: 745b 2243 6c6f 7365 225d 2e69 6c6f 635b  t["Close"].iloc[
-0001f750: 305d 2c20 3229 0a20 2020 2020 2020 2076  0], 2).        v
-0001f760: 6572 6966 7953 7461 6765 5477 6f20 3d20  erifyStageTwo = 
-0001f770: 5472 7565 0a20 2020 2020 2020 2069 6620  True.        if 
-0001f780: 6c65 6e28 6461 7461 2920 3e20 3235 303a  len(data) > 250:
-0001f790: 0a20 2020 2020 2020 2020 2020 2079 6561  .            yea
-0001f7a0: 726c 794c 6f77 203d 2064 6174 612e 6865  rlyLow = data.he
-0001f7b0: 6164 2832 3530 295b 2243 6c6f 7365 225d  ad(250)["Close"]
-0001f7c0: 2e6d 696e 2829 0a20 2020 2020 2020 2020  .min().         
-0001f7d0: 2020 2079 6561 726c 7948 6967 6820 3d20     yearlyHigh = 
-0001f7e0: 6461 7461 2e68 6561 6428 3235 3029 5b22  data.head(250)["
-0001f7f0: 436c 6f73 6522 5d2e 6d61 7828 290a 2020  Close"].max().  
-0001f800: 2020 2020 2020 2020 2020 6966 206c 7470            if ltp
-0001f810: 203c 2028 3220 2a20 7965 6172 6c79 4c6f   < (2 * yearlyLo
-0001f820: 7729 2061 6e64 206c 7470 203c 2028 302e  w) and ltp < (0.
-0001f830: 3735 202a 2079 6561 726c 7948 6967 6829  75 * yearlyHigh)
-0001f840: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001f850: 2020 7665 7269 6679 5374 6167 6554 776f    verifyStageTwo
-0001f860: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-0001f870: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-0001f880: 6963 745b 2253 746f 636b 225d 203d 2063  ict["Stock"] = c
-0001f890: 6f6c 6f72 5465 7874 2e46 4149 4c20 2b20  olorText.FAIL + 
-0001f8a0: 7361 7665 4469 6374 5b22 5374 6f63 6b22  saveDict["Stock"
-0001f8b0: 5d20 2b20 636f 6c6f 7254 6578 742e 454e  ] + colorText.EN
-0001f8c0: 440a 2020 2020 2020 2020 6966 206c 7470  D.        if ltp
-0001f8d0: 203e 3d20 6d69 6e4c 5450 2061 6e64 206c   >= minLTP and l
-0001f8e0: 7470 203c 3d20 6d61 784c 5450 3a0a 2020  tp <= maxLTP:.  
-0001f8f0: 2020 2020 2020 2020 2020 6c74 7056 616c            ltpVal
-0001f900: 6964 203d 2054 7275 650a 2020 2020 2020  id = True.      
-0001f910: 2020 2020 2020 6966 206d 696e 4368 616e        if minChan
-0001f920: 6765 2021 3d20 303a 0a20 2020 2020 2020  ge != 0:.       
-0001f930: 2020 2020 2020 2020 2023 2055 7365 7220           # User 
-0001f940: 6861 7320 7375 7070 6c69 6564 2073 6f6d  has supplied som
-0001f950: 6520 6669 6c74 6572 2066 6f72 2070 6572  e filter for per
-0001f960: 6365 6e74 6167 6520 6368 616e 6765 0a20  centage change. 
-0001f970: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0001f980: 7470 5661 6c69 6420 3d20 666c 6f61 7428  tpValid = float(
-0001f990: 7374 7228 7063 745f 7361 7665 292e 7265  str(pct_save).re
-0001f9a0: 706c 6163 6528 2225 222c 2222 2929 203e  place("%","")) >
-0001f9b0: 3d20 6d69 6e43 6861 6e67 650a 2020 2020  = minChange.    
-0001f9c0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-0001f9d0: 5b22 4c54 5022 5d20 3d20 726f 756e 6428  ["LTP"] = round(
-0001f9e0: 6c74 702c 2032 290a 2020 2020 2020 2020  ltp, 2).        
-0001f9f0: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
-0001fa00: 4c54 5022 5d20 3d20 2863 6f6c 6f72 5465  LTP"] = (colorTe
-0001fa10: 7874 2e47 5245 454e 2069 6620 6c74 7056  xt.GREEN if ltpV
-0001fa20: 616c 6964 2065 6c73 6520 636f 6c6f 7254  alid else colorT
-0001fa30: 6578 742e 4641 494c 2920 2b20 2822 252e  ext.FAIL) + ("%.
-0001fa40: 3266 2220 2520 6c74 7029 202b 2063 6f6c  2f" % ltp) + col
-0001fa50: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
-0001fa60: 2020 2020 2020 2072 6574 7572 6e20 6c74         return lt
-0001fa70: 7056 616c 6964 2c20 7665 7269 6679 5374  pValid, verifySt
-0001fa80: 6167 6554 776f 0a20 2020 2020 2020 2073  ageTwo.        s
-0001fa90: 6372 6565 6e44 6963 745b 224c 5450 225d  creenDict["LTP"]
-0001faa0: 203d 2063 6f6c 6f72 5465 7874 2e46 4149   = colorText.FAI
-0001fab0: 4c20 2b20 2822 252e 3266 2220 2520 6c74  L + ("%.2f" % lt
-0001fac0: 7029 202b 2063 6f6c 6f72 5465 7874 2e45  p) + colorText.E
-0001fad0: 4e44 0a20 2020 2020 2020 2073 6176 6544  ND.        saveD
-0001fae0: 6963 745b 224c 5450 225d 203d 2072 6f75  ict["LTP"] = rou
-0001faf0: 6e64 286c 7470 2c20 3229 0a20 2020 2020  nd(ltp, 2).     
-0001fb00: 2020 2072 6574 7572 6e20 6c74 7056 616c     return ltpVal
-0001fb10: 6964 2c20 7665 7269 6679 5374 6167 6554  id, verifyStageT
-0001fb20: 776f 0a0a 2020 2020 6465 6620 7661 6c69  wo..    def vali
-0001fb30: 6461 7465 4c54 5046 6f72 506f 7274 666f  dateLTPForPortfo
-0001fb40: 6c69 6f43 616c 6328 7365 6c66 2c20 6466  lioCalc(self, df
-0001fb50: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
-0001fb60: 7665 4469 6374 2c72 6571 7565 7374 6564  veDict,requested
-0001fb70: 5065 7269 6f64 3d30 293a 0a20 2020 2020  Period=0):.     
-0001fb80: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-0001fb90: 7928 290a 2020 2020 2020 2020 7065 7269  y().        peri
-0001fba0: 6f64 7320 3d20 7365 6c66 2e63 6f6e 6669  ods = self.confi
-0001fbb0: 674d 616e 6167 6572 2e70 6572 696f 6473  gManager.periods
-0001fbc0: 5261 6e67 650a 2020 2020 2020 2020 6966  Range.        if
-0001fbd0: 2072 6571 7565 7374 6564 5065 7269 6f64   requestedPeriod
-0001fbe0: 203e 2030 2061 6e64 2072 6571 7565 7374   > 0 and request
-0001fbf0: 6564 5065 7269 6f64 206e 6f74 2069 6e20  edPeriod not in 
-0001fc00: 7065 7269 6f64 733a 0a20 2020 2020 2020  periods:.       
-0001fc10: 2020 2020 2070 6572 696f 6473 2e61 7070       periods.app
-0001fc20: 656e 6428 7265 7175 6573 7465 6450 6572  end(requestedPer
-0001fc30: 696f 6429 0a20 2020 2020 2020 2070 7265  iod).        pre
-0001fc40: 7669 6f75 735f 7265 6365 6e74 203d 2064  vious_recent = d
-0001fc50: 6174 612e 6865 6164 2831 290a 2020 2020  ata.head(1).    
-0001fc60: 2020 2020 7072 6576 696f 7573 5f72 6563      previous_rec
-0001fc70: 656e 742e 7265 7365 745f 696e 6465 7828  ent.reset_index(
-0001fc80: 696e 706c 6163 653d 5472 7565 290a 2020  inplace=True).  
-0001fc90: 2020 2020 2020 6361 6c63 5f64 6174 6520        calc_date 
-0001fca0: 3d20 7374 7228 7072 6576 696f 7573 5f72  = str(previous_r
-0001fcb0: 6563 656e 742e 696c 6f63 5b3a 2c20 305d  ecent.iloc[:, 0]
-0001fcc0: 5b30 5d29 2e73 706c 6974 2822 2022 295b  [0]).split(" ")[
-0001fcd0: 305d 0a20 2020 2020 2020 2066 6f72 2070  0].        for p
-0001fce0: 7264 2069 6e20 7065 7269 6f64 733a 0a20  rd in periods:. 
-0001fcf0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-0001fd00: 6e28 6461 7461 2920 3e3d 2070 7264 202b  n(data) >= prd +
-0001fd10: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-0001fd20: 2020 2020 7072 6576 4c74 7020 3d20 6461      prevLtp = da
-0001fd30: 7461 5b22 436c 6f73 6522 5d2e 696c 6f63  ta["Close"].iloc
-0001fd40: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-0001fd50: 2020 2020 6c74 7054 6479 203d 2064 6174      ltpTdy = dat
-0001fd60: 615b 2243 6c6f 7365 225d 2e69 6c6f 635b  a["Close"].iloc[
-0001fd70: 7072 645d 0a20 2020 2020 2020 2020 2020  prd].           
-0001fd80: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0001fd90: 6365 2870 7265 764c 7470 2c70 642e 5365  ce(prevLtp,pd.Se
-0001fda0: 7269 6573 293a 0a20 2020 2020 2020 2020  ries):.         
-0001fdb0: 2020 2020 2020 2020 2020 2070 7265 764c             prevL
-0001fdc0: 7470 203d 2070 7265 764c 7470 5b30 5d0a  tp = prevLtp[0].
-0001fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fde0: 2020 2020 6c74 7054 6479 203d 206c 7470      ltpTdy = ltp
-0001fdf0: 5464 795b 305d 0a20 2020 2020 2020 2020  Tdy[0].         
-0001fe00: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-0001fe10: 745b 6622 4c54 507b 7072 647d 225d 203d  t[f"LTP{prd}"] =
-0001fe20: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0001fe30: 2020 2020 2020 2028 636f 6c6f 7254 6578         (colorTex
-0001fe40: 742e 4752 4545 4e20 6966 2028 6c74 7054  t.GREEN if (ltpT
-0001fe50: 6479 203e 3d20 7072 6576 4c74 7029 2065  dy >= prevLtp) e
-0001fe60: 6c73 6520 2863 6f6c 6f72 5465 7874 2e46  lse (colorText.F
-0001fe70: 4149 4c29 290a 2020 2020 2020 2020 2020  AIL)).          
-0001fe80: 2020 2020 2020 2020 2020 2b20 7374 7228            + str(
-0001fe90: 227b 3a2e 3266 7d22 2e66 6f72 6d61 7428  "{:.2f}".format(
-0001fea0: 6c74 7054 6479 2929 0a20 2020 2020 2020  ltpTdy)).       
-0001feb0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
-0001fec0: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
-0001fed0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0001fee0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001fef0: 6372 6565 6e44 6963 745b 6622 4772 6f77  creenDict[f"Grow
-0001ff00: 7468 7b70 7264 7d22 5d20 3d20 280a 2020  th{prd}"] = (.  
-0001ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff20: 2020 2863 6f6c 6f72 5465 7874 2e47 5245    (colorText.GRE
-0001ff30: 454e 2069 6620 286c 7470 5464 7920 3e3d  EN if (ltpTdy >=
-0001ff40: 2070 7265 764c 7470 2920 656c 7365 2028   prevLtp) else (
-0001ff50: 636f 6c6f 7254 6578 742e 4641 494c 2929  colorText.FAIL))
-0001ff60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ff70: 2020 2020 202b 2073 7472 2822 7b3a 2e32       + str("{:.2
-0001ff80: 667d 222e 666f 726d 6174 286c 7470 5464  f}".format(ltpTd
-0001ff90: 7920 2d20 7072 6576 4c74 7029 290a 2020  y - prevLtp)).  
-0001ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ffb0: 2020 2b20 636f 6c6f 7254 6578 742e 454e    + colorText.EN
-0001ffc0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
-0001ffd0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0001ffe0: 2020 2020 7361 7665 4469 6374 5b66 224c      saveDict[f"L
-0001fff0: 5450 7b70 7264 7d22 5d20 3d20 726f 756e  TP{prd}"] = roun
-00020000: 6428 6c74 7054 6479 2c20 3229 0a20 2020  d(ltpTdy, 2).   
-00020010: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00020020: 6544 6963 745b 6622 4772 6f77 7468 7b70  eDict[f"Growth{p
-00020030: 7264 7d22 5d20 3d20 726f 756e 6428 6c74  rd}"] = round(lt
-00020040: 7054 6479 202d 2070 7265 764c 7470 2c20  pTdy - prevLtp, 
-00020050: 3229 0a20 2020 2020 2020 2020 2020 2020  2).             
-00020060: 2020 2069 6620 7072 6420 3d3d 2032 3220     if prd == 22 
-00020070: 6f72 2028 7072 6420 3d3d 2072 6571 7565  or (prd == reque
-00020080: 7374 6564 5065 7269 6f64 293a 0a20 2020  stedPeriod):.   
-00020090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000200a0: 2063 6861 6e67 6550 6572 6365 6e74 203d   changePercent =
-000200b0: 2072 6f75 6e64 2828 2870 7265 764c 7470   round(((prevLtp
-000200c0: 2d6c 7470 5464 7929 2069 6620 7265 7175  -ltpTdy) if requ
-000200d0: 6573 7465 6450 6572 696f 6420 3d3d 3020  estedPeriod ==0 
-000200e0: 656c 7365 2028 6c74 7054 6479 202d 2070  else (ltpTdy - p
-000200f0: 7265 764c 7470 2929 2a31 3030 2f6c 7470  revLtp))*100/ltp
-00020100: 5464 792c 2032 290a 2020 2020 2020 2020  Tdy, 2).        
-00020110: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00020120: 4469 6374 5b66 227b 7072 647d 2d50 6420  Dict[f"{prd}-Pd 
-00020130: 2522 5d20 3d20 6622 7b63 6861 6e67 6550  %"] = f"{changeP
-00020140: 6572 6365 6e74 7d25 2220 6966 206e 6f74  ercent}%" if not
-00020150: 2070 642e 6973 6e61 2863 6861 6e67 6550   pd.isna(changeP
-00020160: 6572 6365 6e74 2920 656c 7365 2027 2d27  ercent) else '-'
-00020170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020180: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00020190: 6622 7b70 7264 7d2d 5064 2025 225d 203d  f"{prd}-Pd %"] =
-000201a0: 2028 2863 6f6c 6f72 5465 7874 2e47 5245   ((colorText.GRE
-000201b0: 454e 2069 6620 6368 616e 6765 5065 7263  EN if changePerc
-000201c0: 656e 7420 3e3d 3020 656c 7365 2063 6f6c  ent >=0 else col
-000201d0: 6f72 5465 7874 2e46 4149 4c29 202b 2066  orText.FAIL) + f
-000201e0: 227b 6368 616e 6765 5065 7263 656e 747d  "{changePercent}
-000201f0: 2522 202b 2063 6f6c 6f72 5465 7874 2e45  %" + colorText.E
-00020200: 4e44 2920 6966 206e 6f74 2070 642e 6973  ND) if not pd.is
-00020210: 6e61 2863 6861 6e67 6550 6572 6365 6e74  na(changePercent
-00020220: 2920 656c 7365 2027 2d27 0a20 2020 2020  ) else '-'.     
-00020230: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00020240: 6e44 6963 745b 2244 6174 6522 5d20 3d20  nDict["Date"] = 
-00020250: 6361 6c63 5f64 6174 650a 2020 2020 2020  calc_date.      
-00020260: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00020270: 6374 5b22 4461 7465 225d 203d 2063 616c  ct["Date"] = cal
-00020280: 635f 6461 7465 0a20 2020 2020 2020 2020  c_date.         
-00020290: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000202a0: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-000202b0: 745b 6622 4c54 507b 7072 647d 225d 203d  t[f"LTP{prd}"] =
-000202c0: 206e 702e 6e61 6e0a 2020 2020 2020 2020   np.nan.        
-000202d0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-000202e0: 5b66 2247 726f 7774 687b 7072 647d 225d  [f"Growth{prd}"]
-000202f0: 203d 206e 702e 6e61 6e0a 2020 2020 2020   = np.nan.      
-00020300: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-00020310: 4469 6374 5b22 4461 7465 225d 203d 2063  Dict["Date"] = c
-00020320: 616c 635f 6461 7465 0a20 2020 2020 2020  alc_date.       
-00020330: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00020340: 745b 2244 6174 6522 5d20 3d20 6361 6c63  t["Date"] = calc
-00020350: 5f64 6174 650a 0a20 2020 2023 2046 696e  _date..    # Fin
-00020360: 6420 7374 6f63 6b73 2074 6861 7420 6172  d stocks that ar
-00020370: 6520 6265 6172 6973 6820 696e 7472 6164  e bearish intrad
-00020380: 6179 3a20 4d61 6364 2048 6973 746f 6772  ay: Macd Histogr
-00020390: 616d 206e 6567 6174 6976 650a 2020 2020  am negative.    
-000203a0: 6465 6620 7661 6c69 6461 7465 4d41 4344  def validateMACD
-000203b0: 4869 7374 6f67 7261 6d42 656c 6f77 3028  HistogramBelow0(
-000203c0: 7365 6c66 2c20 6466 293a 0a20 2020 2020  self, df):.     
-000203d0: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
-000203e0: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
-000203f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00020400: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-00020410: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-00020420: 7928 290a 2020 2020 2020 2020 6461 7461  y().        data
-00020430: 203d 2064 6174 612e 6669 6c6c 6e61 2830   = data.fillna(0
-00020440: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
-00020450: 2064 6174 612e 7265 706c 6163 6528 5b6e   data.replace([n
-00020460: 702e 696e 662c 202d 6e70 2e69 6e66 5d2c  p.inf, -np.inf],
-00020470: 2030 290a 2020 2020 2020 2020 6461 7461   0).        data
-00020480: 203d 2064 6174 615b 3a3a 2d31 5d20 2023   = data[::-1]  #
-00020490: 2052 6576 6572 7365 2074 6865 2064 6174   Reverse the dat
-000204a0: 6166 7261 6d65 2073 6f20 7468 6174 2069  aframe so that i
-000204b0: 7473 2074 6865 206f 6c64 6573 7420 6461  ts the oldest da
-000204c0: 7465 2066 6972 7374 0a20 2020 2020 2020  te first.       
-000204d0: 206d 6163 6420 3d20 706b 7461 6c69 622e   macd = pktalib.
-000204e0: 4d41 4344 2864 6174 615b 2243 6c6f 7365  MACD(data["Close
-000204f0: 225d 2c20 3132 2c20 3236 2c20 3929 5b32  "], 12, 26, 9)[2
-00020500: 5d2e 7461 696c 2831 290a 2020 2020 2020  ].tail(1).      
-00020510: 2020 7265 7475 726e 206d 6163 642e 696c    return macd.il
-00020520: 6f63 5b3a 315d 5b30 5d20 3c20 300a 0a20  oc[:1][0] < 0.. 
-00020530: 2020 2023 406d 6561 7375 7265 5f74 696d     #@measure_tim
-00020540: 650a 2020 2020 2320 4669 6e64 2069 6620  e.    # Find if 
-00020550: 7374 6f63 6b20 6761 696e 696e 6720 6275  stock gaining bu
-00020560: 6c6c 6973 6820 6d6f 6d65 6e74 756d 0a20  llish momentum. 
-00020570: 2020 2064 6566 2076 616c 6964 6174 654d     def validateM
-00020580: 6f6d 656e 7475 6d28 7365 6c66 2c20 6466  omentum(self, df
-00020590: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
-000205a0: 7665 4469 6374 293a 0a20 2020 2020 2020  veDict):.       
-000205b0: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
-000205c0: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
-000205d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000205e0: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-000205f0: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
-00020600: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
-00020610: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-00020620: 3d20 6461 7461 2e68 6561 6428 3329 0a20  = data.head(3). 
-00020630: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00020640: 6e28 6461 7461 2920 3c20 333a 0a20 2020  n(data) < 3:.   
-00020650: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00020660: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-00020670: 2020 2020 2020 666f 7220 726f 7720 696e        for row in
-00020680: 2064 6174 612e 6974 6572 726f 7773 2829   data.iterrows()
-00020690: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000206a0: 2020 2320 416c 6c20 3320 6361 6e64 6c65    # All 3 candle
-000206b0: 7320 7368 6f75 6c64 2062 6520 4772 6565  s should be Gree
-000206c0: 6e20 616e 6420 4e4f 5420 4369 7263 7569  n and NOT Circui
-000206d0: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
-000206e0: 2020 2079 6320 3d20 726f 775b 315d 5b22     yc = row[1]["
-000206f0: 436c 6f73 6522 5d0a 2020 2020 2020 2020  Close"].        
-00020700: 2020 2020 2020 2020 796f 203d 2072 6f77          yo = row
-00020710: 5b31 5d5b 224f 7065 6e22 5d0a 2020 2020  [1]["Open"].    
-00020720: 2020 2020 2020 2020 2020 2020 6966 2079              if y
-00020730: 6320 3c3d 2079 6f3a 0a20 2020 2020 2020  c <= yo:.       
-00020740: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-00020750: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
-00020760: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
-00020770: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-00020780: 2020 2066 2753 746f 636b 3a7b 7361 7665     f'Stock:{save
-00020790: 4469 6374 5b22 5374 6f63 6b22 5d7d 2c20  Dict["Stock"]}, 
-000207a0: 6973 206e 6f74 2061 206d 6f6d 656e 7475  is not a momentu
-000207b0: 6d2d 6761 696e 6572 2062 6563 6175 7365  m-gainer because
-000207c0: 2079 6573 7465 7264 6179 2d63 6c6f 7365   yesterday-close
-000207d0: 2028 7b79 637d 2920 3c3d 2079 6573 7465   ({yc}) <= yeste
-000207e0: 7264 6179 2d6f 7065 6e20 287b 796f 7d29  rday-open ({yo})
-000207f0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00020800: 2020 2020 2020 2320 290a 2020 2020 2020        # ).      
-00020810: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00020820: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-00020830: 2020 2020 2020 206f 7065 6e44 6573 6320         openDesc 
-00020840: 3d20 6461 7461 2e73 6f72 745f 7661 6c75  = data.sort_valu
-00020850: 6573 2862 793d 5b22 4f70 656e 225d 2c20  es(by=["Open"], 
-00020860: 6173 6365 6e64 696e 673d 4661 6c73 6529  ascending=False)
-00020870: 0a20 2020 2020 2020 2020 2020 2063 6c6f  .            clo
-00020880: 7365 4465 7363 203d 2064 6174 612e 736f  seDesc = data.so
-00020890: 7274 5f76 616c 7565 7328 6279 3d5b 2243  rt_values(by=["C
-000208a0: 6c6f 7365 225d 2c20 6173 6365 6e64 696e  lose"], ascendin
-000208b0: 673d 4661 6c73 6529 0a20 2020 2020 2020  g=False).       
-000208c0: 2020 2020 2076 6f6c 4465 7363 203d 2064       volDesc = d
-000208d0: 6174 612e 736f 7274 5f76 616c 7565 7328  ata.sort_values(
-000208e0: 6279 3d5b 2256 6f6c 756d 6522 5d2c 2061  by=["Volume"], a
-000208f0: 7363 656e 6469 6e67 3d46 616c 7365 290a  scending=False).
-00020900: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00020910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020920: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-00020930: 2020 2020 2020 2020 2020 6461 7461 2e65            data.e
-00020940: 7175 616c 7328 6f70 656e 4465 7363 290a  quals(openDesc).
-00020950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020960: 2020 2020 616e 6420 6461 7461 2e65 7175      and data.equ
-00020970: 616c 7328 636c 6f73 6544 6573 6329 0a20  als(closeDesc). 
-00020980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020990: 2020 2061 6e64 2064 6174 612e 6571 7561     and data.equa
-000209a0: 6c73 2876 6f6c 4465 7363 290a 2020 2020  ls(volDesc).    
-000209b0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
-000209c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000209d0: 2020 2023 2073 656c 662e 6465 6661 756c     # self.defaul
-000209e0: 745f 6c6f 6767 6572 2e69 6e66 6f28 0a20  t_logger.info(. 
-000209f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020a00: 2020 2023 2020 2020 2066 2753 746f 636b     #     f'Stock
-00020a10: 3a7b 7361 7665 4469 6374 5b22 5374 6f63  :{saveDict["Stoc
-00020a20: 6b22 5d7d 2c20 6f70 656e 2c63 6c6f 7365  k"]}, open,close
-00020a30: 2061 6e64 2076 6f6c 756d 6520 6571 7561   and volume equa
-00020a40: 6c20 6672 6f6d 2064 6179 2062 6566 6f72  l from day befor
-00020a50: 6520 7965 7374 6572 6461 792e 2041 2070  e yesterday. A p
-00020a60: 6f74 656e 7469 616c 206d 6f6d 656e 7475  otential momentu
-00020a70: 6d2d 6761 696e 6572 2127 0a20 2020 2020  m-gainer!'.     
-00020a80: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00020a90: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00020aa0: 2020 2020 2020 2074 6f20 3d20 6461 7461         to = data
-00020ab0: 5b22 4f70 656e 225d 2e69 6c6f 635b 305d  ["Open"].iloc[0]
-00020ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020ad0: 2020 2020 2079 6320 3d20 6461 7461 5b22       yc = data["
-00020ae0: 436c 6f73 6522 5d2e 696c 6f63 5b31 5d0a  Close"].iloc[1].
-00020af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b00: 2020 2020 796f 203d 2064 6174 615b 224f      yo = data["O
-00020b10: 7065 6e22 5d2e 696c 6f63 5b31 5d0a 2020  pen"].iloc[1].  
+0001e980: 696e 6520 3138 362c 2069 6e20 5f5f 696e  ine 186, in __in
+0001e990: 6974 5f5f 0a20 2020 2020 2020 2020 2020  it__.           
+0001e9a0: 2023 2046 696c 6520 222f 6f70 742f 686f   # File "/opt/ho
+0001e9b0: 6d65 6272 6577 2f6c 6962 2f70 7974 686f  mebrew/lib/pytho
+0001e9c0: 6e33 2e31 312f 7369 7465 2d70 6163 6b61  n3.11/site-packa
+0001e9d0: 6765 732f 6164 7661 6e63 6564 5f74 612f  ges/advanced_ta/
+0001e9e0: 4c6f 7265 6e74 7a69 616e 436c 6173 7369  LorentzianClassi
+0001e9f0: 6669 6361 7469 6f6e 2f43 6c61 7373 6966  fication/Classif
+0001ea00: 6965 722e 7079 222c 206c 696e 6520 3339  ier.py", line 39
+0001ea10: 352c 2069 6e20 5f5f 636c 6173 7369 6679  5, in __classify
+0001ea20: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+0001ea30: 696c 6520 222f 6f70 742f 686f 6d65 6272  ile "/opt/homebr
+0001ea40: 6577 2f6c 6962 2f70 7974 686f 6e33 2e31  ew/lib/python3.1
+0001ea50: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
+0001ea60: 7061 6e64 6173 2f63 6f72 652f 6f70 732f  pandas/core/ops/
+0001ea70: 636f 6d6d 6f6e 2e70 7922 2c20 6c69 6e65  common.py", line
+0001ea80: 2037 362c 2069 6e20 6e65 775f 6d65 7468   76, in new_meth
+0001ea90: 6f64 0a20 2020 2020 2020 2020 2020 2023  od.            #
+0001eaa0: 2046 696c 6520 222f 6f70 742f 686f 6d65   File "/opt/home
+0001eab0: 6272 6577 2f6c 6962 2f70 7974 686f 6e33  brew/lib/python3
+0001eac0: 2e31 312f 7369 7465 2d70 6163 6b61 6765  .11/site-package
+0001ead0: 732f 7061 6e64 6173 2f63 6f72 652f 6172  s/pandas/core/ar
+0001eae0: 7261 796c 696b 652e 7079 222c 206c 696e  raylike.py", lin
+0001eaf0: 6520 3730 2c20 696e 205f 5f61 6e64 5f5f  e 70, in __and__
+0001eb00: 0a20 2020 2020 2020 2020 2020 2023 2046  .            # F
+0001eb10: 696c 6520 222f 6f70 742f 686f 6d65 6272  ile "/opt/homebr
+0001eb20: 6577 2f6c 6962 2f70 7974 686f 6e33 2e31  ew/lib/python3.1
+0001eb30: 312f 7369 7465 2d70 6163 6b61 6765 732f  1/site-packages/
+0001eb40: 7061 6e64 6173 2f63 6f72 652f 7365 7269  pandas/core/seri
+0001eb50: 6573 2e70 7922 2c20 6c69 6e65 2035 3831  es.py", line 581
+0001eb60: 302c 2069 6e20 5f6c 6f67 6963 616c 5f6d  0, in _logical_m
+0001eb70: 6574 686f 640a 2020 2020 2020 2020 2020  ethod.          
+0001eb80: 2020 2320 4669 6c65 2022 2f6f 7074 2f68    # File "/opt/h
+0001eb90: 6f6d 6562 7265 772f 6c69 622f 7079 7468  omebrew/lib/pyth
+0001eba0: 6f6e 332e 3131 2f73 6974 652d 7061 636b  on3.11/site-pack
+0001ebb0: 6167 6573 2f70 616e 6461 732f 636f 7265  ages/pandas/core
+0001ebc0: 2f6f 7073 2f61 7272 6179 5f6f 7073 2e70  /ops/array_ops.p
+0001ebd0: 7922 2c20 6c69 6e65 2034 3536 2c20 696e  y", line 456, in
+0001ebe0: 206c 6f67 6963 616c 5f6f 700a 2020 2020   logical_op.    
+0001ebf0: 2020 2020 2020 2020 2320 4669 6c65 2022          # File "
+0001ec00: 2f6f 7074 2f68 6f6d 6562 7265 772f 6c69  /opt/homebrew/li
+0001ec10: 622f 7079 7468 6f6e 332e 3131 2f73 6974  b/python3.11/sit
+0001ec20: 652d 7061 636b 6167 6573 2f70 616e 6461  e-packages/panda
+0001ec30: 732f 636f 7265 2f6f 7073 2f61 7272 6179  s/core/ops/array
+0001ec40: 5f6f 7073 2e70 7922 2c20 6c69 6e65 2033  _ops.py", line 3
+0001ec50: 3634 2c20 696e 206e 615f 6c6f 6769 6361  64, in na_logica
+0001ec60: 6c5f 6f70 0a20 2020 2020 2020 2020 2020  l_op.           
+0001ec70: 2023 2073 656c 662e 6465 6661 756c 745f   # self.default_
+0001ec80: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
+0001ec90: 6578 635f 696e 666f 3d54 7275 6529 0a20  exc_info=True). 
+0001eca0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+0001ecb0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0001ecc0: 616c 7365 0a0a 2020 2020 2320 7661 6c69  alse..    # vali
+0001ecd0: 6461 7465 2069 6620 7468 6520 7374 6f63  date if the stoc
+0001ece0: 6b20 6861 7320 6265 656e 2068 6176 696e  k has been havin
+0001ecf0: 6720 6c6f 7765 7220 6c6f 7773 2c20 6c6f  g lower lows, lo
+0001ed00: 7765 7220 6869 6768 730a 2020 2020 6465  wer highs.    de
+0001ed10: 6620 7661 6c69 6461 7465 4c6f 7765 7248  f validateLowerH
+0001ed20: 6967 6873 4c6f 7765 724c 6f77 7328 7365  ighsLowerLows(se
+0001ed30: 6c66 2c20 6466 293a 0a20 2020 2020 2020  lf, df):.       
+0001ed40: 2069 6620 6466 2069 7320 4e6f 6e65 206f   if df is None o
+0001ed50: 7220 6c65 6e28 6466 2920 3d3d 2030 3a0a  r len(df) == 0:.
+0001ed60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001ed70: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0001ed80: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
+0001ed90: 290a 2020 2020 2020 2020 6461 7930 203d  ).        day0 =
+0001eda0: 2064 6174 610a 2020 2020 2020 2020 6461   data.        da
+0001edb0: 7931 203d 2064 6174 615b 313a 5d0a 2020  y1 = data[1:].  
+0001edc0: 2020 2020 2020 6461 7932 203d 2064 6174        day2 = dat
+0001edd0: 615b 323a 5d0a 2020 2020 2020 2020 6461  a[2:].        da
+0001ede0: 7933 203d 2064 6174 615b 333a 5d0a 2020  y3 = data[3:].  
+0001edf0: 2020 2020 2020 6c6f 7765 7248 6967 6873        lowerHighs
+0001ee00: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+0001ee10: 2028 6461 7930 5b22 4869 6768 225d 2e69   (day0["High"].i
+0001ee20: 6c6f 635b 305d 203c 2064 6179 315b 2248  loc[0] < day1["H
+0001ee30: 6967 6822 5d2e 696c 6f63 5b30 5d29 0a20  igh"].iloc[0]). 
+0001ee40: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
+0001ee50: 6461 7931 5b22 4869 6768 225d 2e69 6c6f  day1["High"].ilo
+0001ee60: 635b 305d 203c 2064 6179 325b 2248 6967  c[0] < day2["Hig
+0001ee70: 6822 5d2e 696c 6f63 5b30 5d29 0a20 2020  h"].iloc[0]).   
+0001ee80: 2020 2020 2020 2020 2061 6e64 2028 6461           and (da
+0001ee90: 7932 5b22 4869 6768 225d 2e69 6c6f 635b  y2["High"].iloc[
+0001eea0: 305d 203c 2064 6179 335b 2248 6967 6822  0] < day3["High"
+0001eeb0: 5d2e 696c 6f63 5b30 5d29 0a20 2020 2020  ].iloc[0]).     
+0001eec0: 2020 2029 0a20 2020 2020 2020 206c 6f77     ).        low
+0001eed0: 6572 4c6f 7773 203d 2028 0a20 2020 2020  erLows = (.     
+0001eee0: 2020 2020 2020 2028 6461 7930 5b22 4c6f         (day0["Lo
+0001eef0: 7722 5d2e 696c 6f63 5b30 5d20 3c20 6461  w"].iloc[0] < da
+0001ef00: 7931 5b22 4c6f 7722 5d2e 696c 6f63 5b30  y1["Low"].iloc[0
+0001ef10: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
+0001ef20: 6e64 2028 6461 7931 5b22 4c6f 7722 5d2e  nd (day1["Low"].
+0001ef30: 696c 6f63 5b30 5d20 3c20 6461 7932 5b22  iloc[0] < day2["
+0001ef40: 4c6f 7722 5d2e 696c 6f63 5b30 5d29 0a20  Low"].iloc[0]). 
+0001ef50: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
+0001ef60: 6461 7932 5b22 4c6f 7722 5d2e 696c 6f63  day2["Low"].iloc
+0001ef70: 5b30 5d20 3c20 6461 7933 5b22 4c6f 7722  [0] < day3["Low"
+0001ef80: 5d2e 696c 6f63 5b30 5d29 0a20 2020 2020  ].iloc[0]).     
+0001ef90: 2020 2029 0a20 2020 2020 2020 2068 6967     ).        hig
+0001efa0: 6865 7252 5349 203d 2028 0a20 2020 2020  herRSI = (.     
+0001efb0: 2020 2020 2020 2028 6461 7930 5b22 5253         (day0["RS
+0001efc0: 4922 5d2e 696c 6f63 5b30 5d20 3c20 6461  I"].iloc[0] < da
+0001efd0: 7931 5b22 5253 4922 5d2e 696c 6f63 5b30  y1["RSI"].iloc[0
+0001efe0: 5d29 0a20 2020 2020 2020 2020 2020 2061  ]).            a
+0001eff0: 6e64 2028 6461 7931 5b22 5253 4922 5d2e  nd (day1["RSI"].
+0001f000: 696c 6f63 5b30 5d20 3c20 6461 7932 5b22  iloc[0] < day2["
+0001f010: 5253 4922 5d2e 696c 6f63 5b30 5d29 0a20  RSI"].iloc[0]). 
+0001f020: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
+0001f030: 6461 7932 5b22 5253 4922 5d2e 696c 6f63  day2["RSI"].iloc
+0001f040: 5b30 5d20 3c20 6461 7933 5b22 5253 4922  [0] < day3["RSI"
+0001f050: 5d2e 696c 6f63 5b30 5d29 0a20 2020 2020  ].iloc[0]).     
+0001f060: 2020 2020 2020 2061 6e64 2064 6179 305b         and day0[
+0001f070: 2252 5349 225d 2e69 6c6f 635b 305d 203e  "RSI"].iloc[0] >
+0001f080: 3d20 3530 0a20 2020 2020 2020 2029 0a20  = 50.        ). 
+0001f090: 2020 2020 2020 2072 6574 7572 6e20 6c6f         return lo
+0001f0a0: 7765 7248 6967 6873 2061 6e64 206c 6f77  werHighs and low
+0001f0b0: 6572 4c6f 7773 2061 6e64 2068 6967 6865  erLows and highe
+0001f0c0: 7252 5349 0a0a 2020 2020 2320 5661 6c69  rRSI..    # Vali
+0001f0d0: 6461 7465 2069 6620 7265 6365 6e74 2076  date if recent v
+0001f0e0: 6f6c 756d 6520 6973 206c 6f77 6573 7420  olume is lowest 
+0001f0f0: 6f66 206c 6173 7420 274e 2720 4461 7973  of last 'N' Days
+0001f100: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0001f110: 654c 6f77 6573 7456 6f6c 756d 6528 7365  eLowestVolume(se
+0001f120: 6c66 2c20 6466 2c20 6461 7973 466f 724c  lf, df, daysForL
+0001f130: 6f77 6573 7456 6f6c 756d 6529 3a0a 2020  owestVolume):.  
+0001f140: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
+0001f150: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
+0001f160: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+0001f170: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+0001f180: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+0001f190: 636f 7079 2829 0a20 2020 2020 2020 2064  copy().        d
+0001f1a0: 6174 6120 3d20 6461 7461 2e66 696c 6c6e  ata = data.filln
+0001f1b0: 6128 3029 0a20 2020 2020 2020 2064 6174  a(0).        dat
+0001f1c0: 6120 3d20 6461 7461 2e72 6570 6c61 6365  a = data.replace
+0001f1d0: 285b 6e70 2e69 6e66 2c20 2d6e 702e 696e  ([np.inf, -np.in
+0001f1e0: 665d 2c20 3029 0a20 2020 2020 2020 2069  f], 0).        i
+0001f1f0: 6620 6461 7973 466f 724c 6f77 6573 7456  f daysForLowestV
+0001f200: 6f6c 756d 6520 6973 204e 6f6e 653a 0a20  olume is None:. 
+0001f210: 2020 2020 2020 2020 2020 2064 6179 7346             daysF
+0001f220: 6f72 4c6f 7765 7374 566f 6c75 6d65 203d  orLowestVolume =
+0001f230: 2033 300a 2020 2020 2020 2020 6966 206c   30.        if l
+0001f240: 656e 2864 6174 6129 203c 2064 6179 7346  en(data) < daysF
+0001f250: 6f72 4c6f 7765 7374 566f 6c75 6d65 3a0a  orLowestVolume:.
+0001f260: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001f270: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0001f280: 2064 6174 6120 3d20 6461 7461 2e68 6561   data = data.hea
+0001f290: 6428 6461 7973 466f 724c 6f77 6573 7456  d(daysForLowestV
+0001f2a0: 6f6c 756d 6529 0a20 2020 2020 2020 2072  olume).        r
+0001f2b0: 6563 656e 7420 3d20 6461 7461 2e68 6561  ecent = data.hea
+0001f2c0: 6428 3129 0a20 2020 2020 2020 2069 6620  d(1).        if 
+0001f2d0: 6c65 6e28 7265 6365 6e74 2920 3c20 313a  len(recent) < 1:
+0001f2e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0001f2f0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+0001f300: 2020 6966 2028 7265 6365 6e74 5b22 566f    if (recent["Vo
+0001f310: 6c75 6d65 225d 2e69 6c6f 635b 305d 203c  lume"].iloc[0] <
+0001f320: 3d20 6461 7461 2e64 6573 6372 6962 6528  = data.describe(
+0001f330: 295b 2256 6f6c 756d 6522 5d5b 226d 696e  )["Volume"]["min
+0001f340: 225d 2920 616e 6420 7265 6365 6e74 5b0a  "]) and recent[.
+0001f350: 2020 2020 2020 2020 2020 2020 2256 6f6c              "Vol
+0001f360: 756d 6522 0a20 2020 2020 2020 205d 5b30  ume".        ][0
+0001f370: 5d20 213d 206e 702e 6e61 6e3a 0a20 2020  ] != np.nan:.   
+0001f380: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0001f390: 5472 7565 0a20 2020 2020 2020 2072 6574  True.        ret
+0001f3a0: 7572 6e20 4661 6c73 650a 0a20 2020 2023  urn False..    #
+0001f3b0: 2056 616c 6964 6174 6520 4c54 5020 7769   Validate LTP wi
+0001f3c0: 7468 696e 206c 696d 6974 730a 2020 2020  thin limits.    
+0001f3d0: 6465 6620 7661 6c69 6461 7465 4c54 5028  def validateLTP(
+0001f3e0: 7365 6c66 2c20 6466 2c20 7363 7265 656e  self, df, screen
+0001f3f0: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
+0001f400: 6d69 6e4c 5450 3d4e 6f6e 652c 206d 6178  minLTP=None, max
+0001f410: 4c54 503d 4e6f 6e65 2c6d 696e 4368 616e  LTP=None,minChan
+0001f420: 6765 3d30 293a 0a20 2020 2020 2020 2064  ge=0):.        d
+0001f430: 6174 6120 3d20 6466 2e63 6f70 7928 290a  ata = df.copy().
+0001f440: 2020 2020 2020 2020 6c74 7056 616c 6964          ltpValid
+0001f450: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+0001f460: 2069 6620 6d69 6e4c 5450 2069 7320 4e6f   if minLTP is No
+0001f470: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001f480: 6d69 6e4c 5450 203d 2073 656c 662e 636f  minLTP = self.co
+0001f490: 6e66 6967 4d61 6e61 6765 722e 6d69 6e4c  nfigManager.minL
+0001f4a0: 5450 0a20 2020 2020 2020 2069 6620 6d61  TP.        if ma
+0001f4b0: 784c 5450 2069 7320 4e6f 6e65 3a0a 2020  xLTP is None:.  
+0001f4c0: 2020 2020 2020 2020 2020 6d61 784c 5450            maxLTP
+0001f4d0: 203d 2073 656c 662e 636f 6e66 6967 4d61   = self.configMa
+0001f4e0: 6e61 6765 722e 6d61 784c 5450 0a20 2020  nager.maxLTP.   
+0001f4f0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+0001f500: 2e66 696c 6c6e 6128 3029 0a20 2020 2020  .fillna(0).     
+0001f510: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+0001f520: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
+0001f530: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
+0001f540: 2020 2020 2072 6563 656e 7420 3d20 6461       recent = da
+0001f550: 7461 2e68 6561 6428 3129 0a0a 2020 2020  ta.head(1)..    
+0001f560: 2020 2020 7063 745f 6368 616e 6765 203d      pct_change =
+0001f570: 2028 6461 7461 5b3a 3a2d 315d 5b22 436c   (data[::-1]["Cl
+0001f580: 6f73 6522 5d2e 7063 745f 6368 616e 6765  ose"].pct_change
+0001f590: 2829 202a 2031 3030 292e 696c 6f63 5b2d  () * 100).iloc[-
+0001f5a0: 315d 0a20 2020 2020 2020 2069 6620 7063  1].        if pc
+0001f5b0: 745f 6368 616e 6765 203d 3d20 6e70 2e69  t_change == np.i
+0001f5c0: 6e66 206f 7220 7063 745f 6368 616e 6765  nf or pct_change
+0001f5d0: 203d 3d20 2d6e 702e 696e 663a 0a20 2020   == -np.inf:.   
+0001f5e0: 2020 2020 2020 2020 2070 6374 5f63 6861           pct_cha
+0001f5f0: 6e67 6520 3d20 300a 2020 2020 2020 2020  nge = 0.        
+0001f600: 7063 745f 7361 7665 203d 2022 252e 3166  pct_save = "%.1f
+0001f610: 2525 2220 2520 7063 745f 6368 616e 6765  %%" % pct_change
+0001f620: 0a20 2020 2020 2020 2069 6620 7063 745f  .        if pct_
+0001f630: 6368 616e 6765 203e 2030 2e32 3a0a 2020  change > 0.2:.  
+0001f640: 2020 2020 2020 2020 2020 7063 745f 6368            pct_ch
+0001f650: 616e 6765 203d 2063 6f6c 6f72 5465 7874  ange = colorText
+0001f660: 2e47 5245 454e 202b 2028 2225 2e31 6625  .GREEN + ("%.1f%
+0001f670: 2522 2025 2070 6374 5f63 6861 6e67 6529  %" % pct_change)
+0001f680: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+0001f690: 0a20 2020 2020 2020 2065 6c69 6620 7063  .        elif pc
+0001f6a0: 745f 6368 616e 6765 203c 202d 302e 323a  t_change < -0.2:
+0001f6b0: 0a20 2020 2020 2020 2020 2020 2070 6374  .            pct
+0001f6c0: 5f63 6861 6e67 6520 3d20 636f 6c6f 7254  _change = colorT
+0001f6d0: 6578 742e 4641 494c 202b 2028 2225 2e31  ext.FAIL + ("%.1
+0001f6e0: 6625 2522 2025 2070 6374 5f63 6861 6e67  f%%" % pct_chang
+0001f6f0: 6529 202b 2063 6f6c 6f72 5465 7874 2e45  e) + colorText.E
+0001f700: 4e44 0a20 2020 2020 2020 2065 6c73 653a  ND.        else:
+0001f710: 0a20 2020 2020 2020 2020 2020 2070 6374  .            pct
+0001f720: 5f63 6861 6e67 6520 3d20 636f 6c6f 7254  _change = colorT
+0001f730: 6578 742e 5741 524e 202b 2028 2225 2e31  ext.WARN + ("%.1
+0001f740: 6625 2522 2025 2070 6374 5f63 6861 6e67  f%%" % pct_chang
+0001f750: 6529 202b 2063 6f6c 6f72 5465 7874 2e45  e) + colorText.E
+0001f760: 4e44 0a20 2020 2020 2020 2073 6176 6544  ND.        saveD
+0001f770: 6963 745b 2225 4368 6e67 225d 203d 2070  ict["%Chng"] = p
+0001f780: 6374 5f73 6176 650a 2020 2020 2020 2020  ct_save.        
+0001f790: 7363 7265 656e 4469 6374 5b22 2543 686e  screenDict["%Chn
+0001f7a0: 6722 5d20 3d20 7063 745f 6368 616e 6765  g"] = pct_change
+0001f7b0: 0a20 2020 2020 2020 206c 7470 203d 2072  .        ltp = r
+0001f7c0: 6f75 6e64 2872 6563 656e 745b 2243 6c6f  ound(recent["Clo
+0001f7d0: 7365 225d 2e69 6c6f 635b 305d 2c20 3229  se"].iloc[0], 2)
+0001f7e0: 0a20 2020 2020 2020 2076 6572 6966 7953  .        verifyS
+0001f7f0: 7461 6765 5477 6f20 3d20 5472 7565 0a20  tageTwo = True. 
+0001f800: 2020 2020 2020 2069 6620 6c65 6e28 6461         if len(da
+0001f810: 7461 2920 3e20 3235 303a 0a20 2020 2020  ta) > 250:.     
+0001f820: 2020 2020 2020 2079 6561 726c 794c 6f77         yearlyLow
+0001f830: 203d 2064 6174 612e 6865 6164 2832 3530   = data.head(250
+0001f840: 295b 2243 6c6f 7365 225d 2e6d 696e 2829  )["Close"].min()
+0001f850: 0a20 2020 2020 2020 2020 2020 2079 6561  .            yea
+0001f860: 726c 7948 6967 6820 3d20 6461 7461 2e68  rlyHigh = data.h
+0001f870: 6561 6428 3235 3029 5b22 436c 6f73 6522  ead(250)["Close"
+0001f880: 5d2e 6d61 7828 290a 2020 2020 2020 2020  ].max().        
+0001f890: 2020 2020 6966 206c 7470 203c 2028 3220      if ltp < (2 
+0001f8a0: 2a20 7965 6172 6c79 4c6f 7729 2061 6e64  * yearlyLow) and
+0001f8b0: 206c 7470 203c 2028 302e 3735 202a 2079   ltp < (0.75 * y
+0001f8c0: 6561 726c 7948 6967 6829 3a0a 2020 2020  earlyHigh):.    
+0001f8d0: 2020 2020 2020 2020 2020 2020 7665 7269              veri
+0001f8e0: 6679 5374 6167 6554 776f 203d 2046 616c  fyStageTwo = Fal
+0001f8f0: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+0001f900: 2020 2073 6372 6565 6e44 6963 745b 2253     screenDict["S
+0001f910: 746f 636b 225d 203d 2063 6f6c 6f72 5465  tock"] = colorTe
+0001f920: 7874 2e46 4149 4c20 2b20 7361 7665 4469  xt.FAIL + saveDi
+0001f930: 6374 5b22 5374 6f63 6b22 5d20 2b20 636f  ct["Stock"] + co
+0001f940: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
+0001f950: 2020 2020 6966 206c 7470 203e 3d20 6d69      if ltp >= mi
+0001f960: 6e4c 5450 2061 6e64 206c 7470 203c 3d20  nLTP and ltp <= 
+0001f970: 6d61 784c 5450 3a0a 2020 2020 2020 2020  maxLTP:.        
+0001f980: 2020 2020 6c74 7056 616c 6964 203d 2054      ltpValid = T
+0001f990: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0001f9a0: 6966 206d 696e 4368 616e 6765 2021 3d20  if minChange != 
+0001f9b0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+0001f9c0: 2020 2023 2055 7365 7220 6861 7320 7375     # User has su
+0001f9d0: 7070 6c69 6564 2073 6f6d 6520 6669 6c74  pplied some filt
+0001f9e0: 6572 2066 6f72 2070 6572 6365 6e74 6167  er for percentag
+0001f9f0: 6520 6368 616e 6765 0a20 2020 2020 2020  e change.       
+0001fa00: 2020 2020 2020 2020 206c 7470 5661 6c69           ltpVali
+0001fa10: 6420 3d20 666c 6f61 7428 7374 7228 7063  d = float(str(pc
+0001fa20: 745f 7361 7665 292e 7265 706c 6163 6528  t_save).replace(
+0001fa30: 2225 222c 2222 2929 203e 3d20 6d69 6e43  "%","")) >= minC
+0001fa40: 6861 6e67 650a 2020 2020 2020 2020 2020  hange.          
+0001fa50: 2020 7361 7665 4469 6374 5b22 4c54 5022    saveDict["LTP"
+0001fa60: 5d20 3d20 726f 756e 6428 6c74 702c 2032  ] = round(ltp, 2
+0001fa70: 290a 2020 2020 2020 2020 2020 2020 7363  ).            sc
+0001fa80: 7265 656e 4469 6374 5b22 4c54 5022 5d20  reenDict["LTP"] 
+0001fa90: 3d20 2863 6f6c 6f72 5465 7874 2e47 5245  = (colorText.GRE
+0001faa0: 454e 2069 6620 6c74 7056 616c 6964 2065  EN if ltpValid e
+0001fab0: 6c73 6520 636f 6c6f 7254 6578 742e 4641  lse colorText.FA
+0001fac0: 494c 2920 2b20 2822 252e 3266 2220 2520  IL) + ("%.2f" % 
+0001fad0: 6c74 7029 202b 2063 6f6c 6f72 5465 7874  ltp) + colorText
+0001fae0: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
+0001faf0: 2072 6574 7572 6e20 6c74 7056 616c 6964   return ltpValid
+0001fb00: 2c20 7665 7269 6679 5374 6167 6554 776f  , verifyStageTwo
+0001fb10: 0a20 2020 2020 2020 2073 6372 6565 6e44  .        screenD
+0001fb20: 6963 745b 224c 5450 225d 203d 2063 6f6c  ict["LTP"] = col
+0001fb30: 6f72 5465 7874 2e46 4149 4c20 2b20 2822  orText.FAIL + ("
+0001fb40: 252e 3266 2220 2520 6c74 7029 202b 2063  %.2f" % ltp) + c
+0001fb50: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
+0001fb60: 2020 2020 2073 6176 6544 6963 745b 224c       saveDict["L
+0001fb70: 5450 225d 203d 2072 6f75 6e64 286c 7470  TP"] = round(ltp
+0001fb80: 2c20 3229 0a20 2020 2020 2020 2072 6574  , 2).        ret
+0001fb90: 7572 6e20 6c74 7056 616c 6964 2c20 7665  urn ltpValid, ve
+0001fba0: 7269 6679 5374 6167 6554 776f 0a0a 2020  rifyStageTwo..  
+0001fbb0: 2020 6465 6620 7661 6c69 6461 7465 4c54    def validateLT
+0001fbc0: 5046 6f72 506f 7274 666f 6c69 6f43 616c  PForPortfolioCal
+0001fbd0: 6328 7365 6c66 2c20 6466 2c20 7363 7265  c(self, df, scre
+0001fbe0: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+0001fbf0: 2c72 6571 7565 7374 6564 5065 7269 6f64  ,requestedPeriod
+0001fc00: 3d30 293a 0a20 2020 2020 2020 2064 6174  =0):.        dat
+0001fc10: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
+0001fc20: 2020 2020 2020 7065 7269 6f64 7320 3d20        periods = 
+0001fc30: 7365 6c66 2e63 6f6e 6669 674d 616e 6167  self.configManag
+0001fc40: 6572 2e70 6572 696f 6473 5261 6e67 650a  er.periodsRange.
+0001fc50: 2020 2020 2020 2020 6966 2072 6571 7565          if reque
+0001fc60: 7374 6564 5065 7269 6f64 203e 2030 2061  stedPeriod > 0 a
+0001fc70: 6e64 2072 6571 7565 7374 6564 5065 7269  nd requestedPeri
+0001fc80: 6f64 206e 6f74 2069 6e20 7065 7269 6f64  od not in period
+0001fc90: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+0001fca0: 6572 696f 6473 2e61 7070 656e 6428 7265  eriods.append(re
+0001fcb0: 7175 6573 7465 6450 6572 696f 6429 0a20  questedPeriod). 
+0001fcc0: 2020 2020 2020 2070 7265 7669 6f75 735f         previous_
+0001fcd0: 7265 6365 6e74 203d 2064 6174 612e 6865  recent = data.he
+0001fce0: 6164 2831 290a 2020 2020 2020 2020 7072  ad(1).        pr
+0001fcf0: 6576 696f 7573 5f72 6563 656e 742e 7265  evious_recent.re
+0001fd00: 7365 745f 696e 6465 7828 696e 706c 6163  set_index(inplac
+0001fd10: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+0001fd20: 6361 6c63 5f64 6174 6520 3d20 7374 7228  calc_date = str(
+0001fd30: 7072 6576 696f 7573 5f72 6563 656e 742e  previous_recent.
+0001fd40: 696c 6f63 5b3a 2c20 305d 5b30 5d29 2e73  iloc[:, 0][0]).s
+0001fd50: 706c 6974 2822 2022 295b 305d 0a20 2020  plit(" ")[0].   
+0001fd60: 2020 2020 2066 6f72 2070 7264 2069 6e20       for prd in 
+0001fd70: 7065 7269 6f64 733a 0a20 2020 2020 2020  periods:.       
+0001fd80: 2020 2020 2069 6620 6c65 6e28 6461 7461       if len(data
+0001fd90: 2920 3e3d 2070 7264 202b 2031 3a0a 2020  ) >= prd + 1:.  
+0001fda0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0001fdb0: 6576 4c74 7020 3d20 6461 7461 5b22 436c  evLtp = data["Cl
+0001fdc0: 6f73 6522 5d2e 696c 6f63 5b30 5d0a 2020  ose"].iloc[0].  
+0001fdd0: 2020 2020 2020 2020 2020 2020 2020 6c74                lt
+0001fde0: 7054 6479 203d 2064 6174 615b 2243 6c6f  pTdy = data["Clo
+0001fdf0: 7365 225d 2e69 6c6f 635b 7072 645d 0a20  se"].iloc[prd]. 
+0001fe00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001fe10: 6620 6973 696e 7374 616e 6365 2870 7265  f isinstance(pre
+0001fe20: 764c 7470 2c70 642e 5365 7269 6573 293a  vLtp,pd.Series):
+0001fe30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fe40: 2020 2020 2070 7265 764c 7470 203d 2070       prevLtp = p
+0001fe50: 7265 764c 7470 5b30 5d0a 2020 2020 2020  revLtp[0].      
+0001fe60: 2020 2020 2020 2020 2020 2020 2020 6c74                lt
+0001fe70: 7054 6479 203d 206c 7470 5464 795b 305d  pTdy = ltpTdy[0]
+0001fe80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fe90: 2073 6372 6565 6e44 6963 745b 6622 4c54   screenDict[f"LT
+0001fea0: 507b 7072 647d 225d 203d 2028 0a20 2020  P{prd}"] = (.   
+0001feb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fec0: 2028 636f 6c6f 7254 6578 742e 4752 4545   (colorText.GREE
+0001fed0: 4e20 6966 2028 6c74 7054 6479 203e 3d20  N if (ltpTdy >= 
+0001fee0: 7072 6576 4c74 7029 2065 6c73 6520 2863  prevLtp) else (c
+0001fef0: 6f6c 6f72 5465 7874 2e46 4149 4c29 290a  olorText.FAIL)).
+0001ff00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ff10: 2020 2020 2b20 7374 7228 227b 3a2e 3266      + str("{:.2f
+0001ff20: 7d22 2e66 6f72 6d61 7428 6c74 7054 6479  }".format(ltpTdy
+0001ff30: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0001ff40: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
+0001ff50: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
+0001ff60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0001ff70: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+0001ff80: 6963 745b 6622 4772 6f77 7468 7b70 7264  ict[f"Growth{prd
+0001ff90: 7d22 5d20 3d20 280a 2020 2020 2020 2020  }"] = (.        
+0001ffa0: 2020 2020 2020 2020 2020 2020 2863 6f6c              (col
+0001ffb0: 6f72 5465 7874 2e47 5245 454e 2069 6620  orText.GREEN if 
+0001ffc0: 286c 7470 5464 7920 3e3d 2070 7265 764c  (ltpTdy >= prevL
+0001ffd0: 7470 2920 656c 7365 2028 636f 6c6f 7254  tp) else (colorT
+0001ffe0: 6578 742e 4641 494c 2929 0a20 2020 2020  ext.FAIL)).     
+0001fff0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00020000: 2073 7472 2822 7b3a 2e32 667d 222e 666f   str("{:.2f}".fo
+00020010: 726d 6174 286c 7470 5464 7920 2d20 7072  rmat(ltpTdy - pr
+00020020: 6576 4c74 7029 290a 2020 2020 2020 2020  evLtp)).        
+00020030: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
+00020040: 6c6f 7254 6578 742e 454e 440a 2020 2020  lorText.END.    
+00020050: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00020060: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00020070: 7665 4469 6374 5b66 224c 5450 7b70 7264  veDict[f"LTP{prd
+00020080: 7d22 5d20 3d20 726f 756e 6428 6c74 7054  }"] = round(ltpT
+00020090: 6479 2c20 3229 0a20 2020 2020 2020 2020  dy, 2).         
+000200a0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
+000200b0: 6622 4772 6f77 7468 7b70 7264 7d22 5d20  f"Growth{prd}"] 
+000200c0: 3d20 726f 756e 6428 6c74 7054 6479 202d  = round(ltpTdy -
+000200d0: 2070 7265 764c 7470 2c20 3229 0a20 2020   prevLtp, 2).   
+000200e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000200f0: 7072 6420 3d3d 2032 3220 6f72 2028 7072  prd == 22 or (pr
+00020100: 6420 3d3d 2072 6571 7565 7374 6564 5065  d == requestedPe
+00020110: 7269 6f64 293a 0a20 2020 2020 2020 2020  riod):.         
+00020120: 2020 2020 2020 2020 2020 2063 6861 6e67             chang
+00020130: 6550 6572 6365 6e74 203d 2072 6f75 6e64  ePercent = round
+00020140: 2828 2870 7265 764c 7470 2d6c 7470 5464  (((prevLtp-ltpTd
+00020150: 7929 2069 6620 7265 7175 6573 7465 6450  y) if requestedP
+00020160: 6572 696f 6420 3d3d 3020 656c 7365 2028  eriod ==0 else (
+00020170: 6c74 7054 6479 202d 2070 7265 764c 7470  ltpTdy - prevLtp
+00020180: 2929 2a31 3030 2f6c 7470 5464 792c 2032  ))*100/ltpTdy, 2
+00020190: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000201a0: 2020 2020 2020 7361 7665 4469 6374 5b66        saveDict[f
+000201b0: 227b 7072 647d 2d50 6420 2522 5d20 3d20  "{prd}-Pd %"] = 
+000201c0: 6622 7b63 6861 6e67 6550 6572 6365 6e74  f"{changePercent
+000201d0: 7d25 2220 6966 206e 6f74 2070 642e 6973  }%" if not pd.is
+000201e0: 6e61 2863 6861 6e67 6550 6572 6365 6e74  na(changePercent
+000201f0: 2920 656c 7365 2027 2d27 0a20 2020 2020  ) else '-'.     
+00020200: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00020210: 6372 6565 6e44 6963 745b 6622 7b70 7264  creenDict[f"{prd
+00020220: 7d2d 5064 2025 225d 203d 2028 2863 6f6c  }-Pd %"] = ((col
+00020230: 6f72 5465 7874 2e47 5245 454e 2069 6620  orText.GREEN if 
+00020240: 6368 616e 6765 5065 7263 656e 7420 3e3d  changePercent >=
+00020250: 3020 656c 7365 2063 6f6c 6f72 5465 7874  0 else colorText
+00020260: 2e46 4149 4c29 202b 2066 227b 6368 616e  .FAIL) + f"{chan
+00020270: 6765 5065 7263 656e 747d 2522 202b 2063  gePercent}%" + c
+00020280: 6f6c 6f72 5465 7874 2e45 4e44 2920 6966  olorText.END) if
+00020290: 206e 6f74 2070 642e 6973 6e61 2863 6861   not pd.isna(cha
+000202a0: 6e67 6550 6572 6365 6e74 2920 656c 7365  ngePercent) else
+000202b0: 2027 2d27 0a20 2020 2020 2020 2020 2020   '-'.           
+000202c0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+000202d0: 2244 6174 6522 5d20 3d20 6361 6c63 5f64  "Date"] = calc_d
+000202e0: 6174 650a 2020 2020 2020 2020 2020 2020  ate.            
+000202f0: 2020 2020 7361 7665 4469 6374 5b22 4461      saveDict["Da
+00020300: 7465 225d 203d 2063 616c 635f 6461 7465  te"] = calc_date
+00020310: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00020320: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00020330: 2020 2073 6176 6544 6963 745b 6622 4c54     saveDict[f"LT
+00020340: 507b 7072 647d 225d 203d 206e 702e 6e61  P{prd}"] = np.na
+00020350: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00020360: 2020 7361 7665 4469 6374 5b66 2247 726f    saveDict[f"Gro
+00020370: 7774 687b 7072 647d 225d 203d 206e 702e  wth{prd}"] = np.
+00020380: 6e61 6e0a 2020 2020 2020 2020 2020 2020  nan.            
+00020390: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+000203a0: 4461 7465 225d 203d 2063 616c 635f 6461  Date"] = calc_da
+000203b0: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
+000203c0: 2020 2073 6176 6544 6963 745b 2244 6174     saveDict["Dat
+000203d0: 6522 5d20 3d20 6361 6c63 5f64 6174 650a  e"] = calc_date.
+000203e0: 0a20 2020 2023 2046 696e 6420 7374 6f63  .    # Find stoc
+000203f0: 6b73 2074 6861 7420 6172 6520 6265 6172  ks that are bear
+00020400: 6973 6820 696e 7472 6164 6179 3a20 4d61  ish intraday: Ma
+00020410: 6364 2048 6973 746f 6772 616d 206e 6567  cd Histogram neg
+00020420: 6174 6976 650a 2020 2020 6465 6620 7661  ative.    def va
+00020430: 6c69 6461 7465 4d41 4344 4869 7374 6f67  lidateMACDHistog
+00020440: 7261 6d42 656c 6f77 3028 7365 6c66 2c20  ramBelow0(self, 
+00020450: 6466 293a 0a20 2020 2020 2020 2069 6620  df):.        if 
+00020460: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
+00020470: 6e28 6466 2920 3d3d 2030 3a0a 2020 2020  n(df) == 0:.    
+00020480: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00020490: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
+000204a0: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
+000204b0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+000204c0: 612e 6669 6c6c 6e61 2830 290a 2020 2020  a.fillna(0).    
+000204d0: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
+000204e0: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
+000204f0: 202d 6e70 2e69 6e66 5d2c 2030 290a 2020   -np.inf], 0).  
+00020500: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
+00020510: 615b 3a3a 2d31 5d20 2023 2052 6576 6572  a[::-1]  # Rever
+00020520: 7365 2074 6865 2064 6174 6166 7261 6d65  se the dataframe
+00020530: 2073 6f20 7468 6174 2069 7473 2074 6865   so that its the
+00020540: 206f 6c64 6573 7420 6461 7465 2066 6972   oldest date fir
+00020550: 7374 0a20 2020 2020 2020 206d 6163 6420  st.        macd 
+00020560: 3d20 706b 7461 6c69 622e 4d41 4344 2864  = pktalib.MACD(d
+00020570: 6174 615b 2243 6c6f 7365 225d 2c20 3132  ata["Close"], 12
+00020580: 2c20 3236 2c20 3929 5b32 5d2e 7461 696c  , 26, 9)[2].tail
+00020590: 2831 290a 2020 2020 2020 2020 7265 7475  (1).        retu
+000205a0: 726e 206d 6163 642e 696c 6f63 5b3a 315d  rn macd.iloc[:1]
+000205b0: 5b30 5d20 3c20 300a 0a20 2020 2023 406d  [0] < 0..    #@m
+000205c0: 6561 7375 7265 5f74 696d 650a 2020 2020  easure_time.    
+000205d0: 2320 4669 6e64 2069 6620 7374 6f63 6b20  # Find if stock 
+000205e0: 6761 696e 696e 6720 6275 6c6c 6973 6820  gaining bullish 
+000205f0: 6d6f 6d65 6e74 756d 0a20 2020 2064 6566  momentum.    def
+00020600: 2076 616c 6964 6174 654d 6f6d 656e 7475   validateMomentu
+00020610: 6d28 7365 6c66 2c20 6466 2c20 7363 7265  m(self, df, scre
+00020620: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+00020630: 293a 0a20 2020 2020 2020 2069 6620 6466  ):.        if df
+00020640: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
+00020650: 6466 2920 3d3d 2030 3a0a 2020 2020 2020  df) == 0:.      
+00020660: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+00020670: 7365 0a20 2020 2020 2020 2064 6174 6120  se.        data 
+00020680: 3d20 6466 2e63 6f70 7928 290a 2020 2020  = df.copy().    
+00020690: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000206a0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+000206b0: 2e68 6561 6428 3329 0a20 2020 2020 2020  .head(3).       
+000206c0: 2020 2020 2069 6620 6c65 6e28 6461 7461       if len(data
+000206d0: 2920 3c20 333a 0a20 2020 2020 2020 2020  ) < 3:.         
+000206e0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+000206f0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00020700: 666f 7220 726f 7720 696e 2064 6174 612e  for row in data.
+00020710: 6974 6572 726f 7773 2829 3a0a 2020 2020  iterrows():.    
+00020720: 2020 2020 2020 2020 2020 2020 2320 416c              # Al
+00020730: 6c20 3320 6361 6e64 6c65 7320 7368 6f75  l 3 candles shou
+00020740: 6c64 2062 6520 4772 6565 6e20 616e 6420  ld be Green and 
+00020750: 4e4f 5420 4369 7263 7569 7473 0a20 2020  NOT Circuits.   
+00020760: 2020 2020 2020 2020 2020 2020 2079 6320               yc 
+00020770: 3d20 726f 775b 315d 5b22 436c 6f73 6522  = row[1]["Close"
+00020780: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00020790: 2020 796f 203d 2072 6f77 5b31 5d5b 224f    yo = row[1]["O
+000207a0: 7065 6e22 5d0a 2020 2020 2020 2020 2020  pen"].          
+000207b0: 2020 2020 2020 6966 2079 6320 3c3d 2079        if yc <= y
+000207c0: 6f3a 0a20 2020 2020 2020 2020 2020 2020  o:.             
+000207d0: 2020 2020 2020 2023 2073 656c 662e 6465         # self.de
+000207e0: 6661 756c 745f 6c6f 6767 6572 2e69 6e66  fault_logger.inf
+000207f0: 6f28 0a20 2020 2020 2020 2020 2020 2020  o(.             
+00020800: 2020 2020 2020 2023 2020 2020 2066 2753         #     f'S
+00020810: 746f 636b 3a7b 7361 7665 4469 6374 5b22  tock:{saveDict["
+00020820: 5374 6f63 6b22 5d7d 2c20 6973 206e 6f74  Stock"]}, is not
+00020830: 2061 206d 6f6d 656e 7475 6d2d 6761 696e   a momentum-gain
+00020840: 6572 2062 6563 6175 7365 2079 6573 7465  er because yeste
+00020850: 7264 6179 2d63 6c6f 7365 2028 7b79 637d  rday-close ({yc}
+00020860: 2920 3c3d 2079 6573 7465 7264 6179 2d6f  ) <= yesterday-o
+00020870: 7065 6e20 287b 796f 7d29 270a 2020 2020  pen ({yo})'.    
+00020880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020890: 2320 290a 2020 2020 2020 2020 2020 2020  # ).            
+000208a0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+000208b0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+000208c0: 206f 7065 6e44 6573 6320 3d20 6461 7461   openDesc = data
+000208d0: 2e73 6f72 745f 7661 6c75 6573 2862 793d  .sort_values(by=
+000208e0: 5b22 4f70 656e 225d 2c20 6173 6365 6e64  ["Open"], ascend
+000208f0: 696e 673d 4661 6c73 6529 0a20 2020 2020  ing=False).     
+00020900: 2020 2020 2020 2063 6c6f 7365 4465 7363         closeDesc
+00020910: 203d 2064 6174 612e 736f 7274 5f76 616c   = data.sort_val
+00020920: 7565 7328 6279 3d5b 2243 6c6f 7365 225d  ues(by=["Close"]
+00020930: 2c20 6173 6365 6e64 696e 673d 4661 6c73  , ascending=Fals
+00020940: 6529 0a20 2020 2020 2020 2020 2020 2076  e).            v
+00020950: 6f6c 4465 7363 203d 2064 6174 612e 736f  olDesc = data.so
+00020960: 7274 5f76 616c 7565 7328 6279 3d5b 2256  rt_values(by=["V
+00020970: 6f6c 756d 6522 5d2c 2061 7363 656e 6469  olume"], ascendi
+00020980: 6e67 3d46 616c 7365 290a 2020 2020 2020  ng=False).      
+00020990: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+000209a0: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
+000209b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000209c0: 2020 2020 6461 7461 2e65 7175 616c 7328      data.equals(
+000209d0: 6f70 656e 4465 7363 290a 2020 2020 2020  openDesc).      
+000209e0: 2020 2020 2020 2020 2020 2020 2020 616e                an
+000209f0: 6420 6461 7461 2e65 7175 616c 7328 636c  d data.equals(cl
+00020a00: 6f73 6544 6573 6329 0a20 2020 2020 2020  oseDesc).       
+00020a10: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00020a20: 2064 6174 612e 6571 7561 6c73 2876 6f6c   data.equals(vol
+00020a30: 4465 7363 290a 2020 2020 2020 2020 2020  Desc).          
+00020a40: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+00020a50: 2020 2020 2020 2020 2020 2020 2023 2073               # s
+00020a60: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
+00020a70: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
+00020a80: 2020 2020 2020 2020 2020 2020 2023 2020               #  
+00020a90: 2020 2066 2753 746f 636b 3a7b 7361 7665     f'Stock:{save
+00020aa0: 4469 6374 5b22 5374 6f63 6b22 5d7d 2c20  Dict["Stock"]}, 
+00020ab0: 6f70 656e 2c63 6c6f 7365 2061 6e64 2076  open,close and v
+00020ac0: 6f6c 756d 6520 6571 7561 6c20 6672 6f6d  olume equal from
+00020ad0: 2064 6179 2062 6566 6f72 6520 7965 7374   day before yest
+00020ae0: 6572 6461 792e 2041 2070 6f74 656e 7469  erday. A potenti
+00020af0: 616c 206d 6f6d 656e 7475 6d2d 6761 696e  al momentum-gain
+00020b00: 6572 2127 0a20 2020 2020 2020 2020 2020  er!'.           
+00020b10: 2020 2020 2020 2020 2023 2029 0a20 2020           # ).   
 00020b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b30: 2020 6479 6320 3d20 6461 7461 5b22 436c    dyc = data["Cl
-00020b40: 6f73 6522 5d2e 696c 6f63 5b32 5d0a 2020  ose"].iloc[2].  
-00020b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b60: 2020 6966 2028 746f 203e 3d20 7963 2920    if (to >= yc) 
-00020b70: 616e 6420 2879 6f20 3e3d 2064 7963 293a  and (yo >= dyc):
-00020b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00020b90: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
-00020ba0: 6465 6661 756c 745f 6c6f 6767 6572 2e69  default_logger.i
-00020bb0: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
-00020bc0: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-00020bd0: 2020 2066 2753 746f 636b 3a7b 7361 7665     f'Stock:{save
-00020be0: 4469 6374 5b22 5374 6f63 6b22 5d7d 2c20  Dict["Stock"]}, 
-00020bf0: 6973 2061 206d 6f6d 656e 7475 6d2d 6761  is a momentum-ga
-00020c00: 696e 6572 2062 6563 6175 7365 2074 6f64  iner because tod
-00020c10: 6179 2d6f 7065 6e20 287b 746f 7d29 203e  ay-open ({to}) >
-00020c20: 3d20 7965 7374 6572 6461 792d 636c 6f73  = yesterday-clos
-00020c30: 6520 287b 7963 7d29 2061 6e64 2079 6573  e ({yc}) and yes
-00020c40: 7465 7264 6179 2d6f 7065 6e28 7b79 6f7d  terday-open({yo}
-00020c50: 2920 3e3d 2064 6179 2d62 6566 6f72 652d  ) >= day-before-
-00020c60: 636c 6f73 6528 7b64 7963 7d29 270a 2020  close({dyc})'.  
-00020c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020c80: 2020 2020 2020 2320 290a 2020 2020 2020        # ).      
-00020c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ca0: 2020 7361 7665 6420 3d20 7365 6c66 2e66    saved = self.f
-00020cb0: 696e 6443 7572 7265 6e74 5361 7665 6456  indCurrentSavedV
-00020cc0: 616c 7565 2873 6372 6565 6e44 6963 742c  alue(screenDict,
-00020cd0: 2073 6176 6544 6963 742c 2022 5061 7474   saveDict, "Patt
-00020ce0: 6572 6e22 290a 2020 2020 2020 2020 2020  ern").          
-00020cf0: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00020d00: 7265 656e 4469 6374 5b22 5061 7474 6572  reenDict["Patter
-00020d10: 6e22 5d20 3d20 280a 2020 2020 2020 2020  n"] = (.        
-00020d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d30: 2020 2020 7361 7665 645b 305d 0a20 2020      saved[0].   
-00020d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d50: 2020 2020 2020 2020 202b 2063 6f6c 6f72           + color
-00020d60: 5465 7874 2e42 4f4c 440a 2020 2020 2020  Text.BOLD.      
+00020b30: 2074 6f20 3d20 6461 7461 5b22 4f70 656e   to = data["Open
+00020b40: 225d 2e69 6c6f 635b 305d 0a20 2020 2020  "].iloc[0].     
+00020b50: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+00020b60: 6320 3d20 6461 7461 5b22 436c 6f73 6522  c = data["Close"
+00020b70: 5d2e 696c 6f63 5b31 5d0a 2020 2020 2020  ].iloc[1].      
+00020b80: 2020 2020 2020 2020 2020 2020 2020 796f                yo
+00020b90: 203d 2064 6174 615b 224f 7065 6e22 5d2e   = data["Open"].
+00020ba0: 696c 6f63 5b31 5d0a 2020 2020 2020 2020  iloc[1].        
+00020bb0: 2020 2020 2020 2020 2020 2020 6479 6320              dyc 
+00020bc0: 3d20 6461 7461 5b22 436c 6f73 6522 5d2e  = data["Close"].
+00020bd0: 696c 6f63 5b32 5d0a 2020 2020 2020 2020  iloc[2].        
+00020be0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00020bf0: 746f 203e 3d20 7963 2920 616e 6420 2879  to >= yc) and (y
+00020c00: 6f20 3e3d 2064 7963 293a 0a20 2020 2020  o >= dyc):.     
+00020c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c20: 2020 2023 2073 656c 662e 6465 6661 756c     # self.defaul
+00020c30: 745f 6c6f 6767 6572 2e69 6e66 6f28 0a20  t_logger.info(. 
+00020c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c50: 2020 2020 2020 2023 2020 2020 2066 2753         #     f'S
+00020c60: 746f 636b 3a7b 7361 7665 4469 6374 5b22  tock:{saveDict["
+00020c70: 5374 6f63 6b22 5d7d 2c20 6973 2061 206d  Stock"]}, is a m
+00020c80: 6f6d 656e 7475 6d2d 6761 696e 6572 2062  omentum-gainer b
+00020c90: 6563 6175 7365 2074 6f64 6179 2d6f 7065  ecause today-ope
+00020ca0: 6e20 287b 746f 7d29 203e 3d20 7965 7374  n ({to}) >= yest
+00020cb0: 6572 6461 792d 636c 6f73 6520 287b 7963  erday-close ({yc
+00020cc0: 7d29 2061 6e64 2079 6573 7465 7264 6179  }) and yesterday
+00020cd0: 2d6f 7065 6e28 7b79 6f7d 2920 3e3d 2064  -open({yo}) >= d
+00020ce0: 6179 2d62 6566 6f72 652d 636c 6f73 6528  ay-before-close(
+00020cf0: 7b64 7963 7d29 270a 2020 2020 2020 2020  {dyc})'.        
+00020d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d10: 2320 290a 2020 2020 2020 2020 2020 2020  # ).            
+00020d20: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00020d30: 6420 3d20 7365 6c66 2e66 696e 6443 7572  d = self.findCur
+00020d40: 7265 6e74 5361 7665 6456 616c 7565 2873  rentSavedValue(s
+00020d50: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
+00020d60: 6963 742c 2022 5061 7474 6572 6e22 290a  ict, "Pattern").
 00020d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020d80: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-00020d90: 742e 4752 4545 4e0a 2020 2020 2020 2020  t.GREEN.        
-00020da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020db0: 2020 2020 2b20 224d 6f6d 656e 7475 6d20      + "Momentum 
-00020dc0: 4761 696e 6572 220a 2020 2020 2020 2020  Gainer".        
+00020d80: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+00020d90: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
+00020da0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00020db0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00020dc0: 7665 645b 305d 0a20 2020 2020 2020 2020  ved[0].         
 00020dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020de0: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
-00020df0: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
-00020e00: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00020e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e20: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
-00020e30: 5061 7474 6572 6e22 5d20 3d20 7361 7665  Pattern"] = save
-00020e40: 645b 315d 202b 2022 4d6f 6d65 6e74 756d  d[1] + "Momentum
-00020e50: 2047 6169 6e65 7222 0a20 2020 2020 2020   Gainer".       
-00020e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e70: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00020de0: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
+00020df0: 4f4c 440a 2020 2020 2020 2020 2020 2020  OLD.            
+00020e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020e10: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
+00020e20: 4e0a 2020 2020 2020 2020 2020 2020 2020  N.              
+00020e30: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00020e40: 224d 6f6d 656e 7475 6d20 4761 696e 6572  "Momentum Gainer
+00020e50: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00020e60: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00020e70: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
 00020e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e90: 2023 2073 656c 662e 6465 6661 756c 745f   # self.default_
-00020ea0: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
-00020eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ec0: 2023 2020 2020 2066 2753 746f 636b 3a7b   #     f'Stock:{
-00020ed0: 7361 7665 4469 6374 5b22 5374 6f63 6b22  saveDict["Stock"
-00020ee0: 5d7d 2c20 6973 206e 6f74 2061 206d 6f6d  ]}, is not a mom
-00020ef0: 656e 7475 6d2d 6761 696e 6572 2062 6563  entum-gainer bec
-00020f00: 6175 7365 2065 6974 6865 7220 746f 6461  ause either toda
-00020f10: 792d 6f70 656e 2028 7b74 6f7d 2920 3c20  y-open ({to}) < 
-00020f20: 7965 7374 6572 6461 792d 636c 6f73 6520  yesterday-close 
-00020f30: 287b 7963 7d29 206f 7220 7965 7374 6572  ({yc}) or yester
-00020f40: 6461 792d 6f70 656e 287b 796f 7d29 203c  day-open({yo}) <
-00020f50: 2064 6179 2d62 6566 6f72 652d 636c 6f73   day-before-clos
-00020f60: 6528 7b64 7963 7d29 270a 2020 2020 2020  e({dyc})'.      
-00020f70: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00020f80: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
-00020f90: 6365 7074 2049 6e64 6578 4572 726f 7220  cept IndexError 
-00020fa0: 6173 2065 3a20 2320 7072 6167 6d61 3a20  as e: # pragma: 
-00020fb0: 6e6f 2063 6f76 6572 0a20 2020 2020 2020  no cover.       
-00020fc0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-00020fd0: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
-00020fe0: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
-00020ff0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-00021000: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
-00021010: 745f 6c6f 6767 6572 2e64 6562 7567 2864  t_logger.debug(d
-00021020: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
-00021030: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-00021040: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00021050: 7365 0a20 2020 2020 2020 2065 7863 6570  se.        excep
-00021060: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00021070: 3a20 2023 2070 7261 676d 613a 206e 6f20  :  # pragma: no 
-00021080: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
-00021090: 2020 7365 6c66 2e64 6566 6175 6c74 5f6c    self.default_l
-000210a0: 6f67 6765 722e 6465 6275 6728 652c 2065  ogger.debug(e, e
-000210b0: 7863 5f69 6e66 6f3d 5472 7565 290a 2020  xc_info=True).  
-000210c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000210d0: 2046 616c 7365 0a0a 2020 2020 2340 6d65   False..    #@me
-000210e0: 6173 7572 655f 7469 6d65 0a20 2020 2023  asure_time.    #
-000210f0: 2056 616c 6964 6174 6520 4d6f 7669 6e67   Validate Moving
-00021100: 2061 7665 7261 6765 7320 616e 6420 6c6f   averages and lo
-00021110: 6f6b 2066 6f72 2062 7579 2f73 656c 6c20  ok for buy/sell 
-00021120: 7369 676e 616c 730a 2020 2020 6465 6620  signals.    def 
-00021130: 7661 6c69 6461 7465 4d6f 7669 6e67 4176  validateMovingAv
-00021140: 6572 6167 6573 2873 656c 662c 2064 662c  erages(self, df,
-00021150: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
-00021160: 6544 6963 742c 206d 6152 616e 6765 3d32  eDict, maRange=2
-00021170: 2e35 2c6d 614c 656e 6774 683d 3029 3a0a  .5,maLength=0):.
-00021180: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00021190: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-000211a0: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
-000211b0: 6c6e 6128 3029 0a20 2020 2020 2020 2064  lna(0).        d
-000211c0: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
-000211d0: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
-000211e0: 696e 665d 2c20 3029 0a20 2020 2020 2020  inf], 0).       
-000211f0: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
-00021200: 6561 6428 3129 0a20 2020 2020 2020 206d  ead(1).        m
-00021210: 6153 6967 6e61 6c73 203d 205b 5d0a 2020  aSignals = [].  
-00021220: 2020 2020 2020 6966 2073 7472 286d 614c        if str(maL
-00021230: 656e 6774 6829 2069 6e20 5b22 3022 2c22  ength) in ["0","
-00021240: 3222 2c22 3322 5d3a 0a20 2020 2020 2020  2","3"]:.       
-00021250: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
-00021260: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
-00021270: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
-00021280: 6374 2c73 6176 6544 6963 742c 224d 412d  ct,saveDict,"MA-
-00021290: 5369 676e 616c 2229 0a20 2020 2020 2020  Signal").       
-000212a0: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-000212b0: 2020 2020 2020 2020 2020 7265 6365 6e74            recent
-000212c0: 5b22 534d 4122 5d2e 696c 6f63 5b30 5d20  ["SMA"].iloc[0] 
-000212d0: 3e20 7265 6365 6e74 5b22 4c4d 4122 5d2e  > recent["LMA"].
-000212e0: 696c 6f63 5b30 5d0a 2020 2020 2020 2020  iloc[0].        
-000212f0: 2020 2020 2020 2020 616e 6420 7265 6365          and rece
-00021300: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
-00021310: 5b30 5d20 3e20 7265 6365 6e74 5b22 534d  [0] > recent["SM
-00021320: 4122 5d2e 696c 6f63 5b30 5d0a 2020 2020  A"].iloc[0].    
-00021330: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-00021340: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00021350: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
-00021360: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
-00021370: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-00021380: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
-00021390: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
-000213a0: 2e47 5245 454e 202b 2022 4275 6c6c 6973  .GREEN + "Bullis
-000213b0: 6822 202b 2063 6f6c 6f72 5465 7874 2e45  h" + colorText.E
-000213c0: 4e44 0a20 2020 2020 2020 2020 2020 2020  ND.             
-000213d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000213e0: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
-000213f0: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
-00021400: 6564 5b31 5d20 2b20 2242 756c 6c69 7368  ed[1] + "Bullish
-00021410: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00021420: 2020 6d61 5369 676e 616c 732e 6170 7065    maSignals.appe
-00021430: 6e64 2822 3322 290a 2020 2020 2020 2020  nd("3").        
-00021440: 2020 2020 656c 6966 2072 6563 656e 745b      elif recent[
-00021450: 2253 4d41 225d 2e69 6c6f 635b 305d 203c  "SMA"].iloc[0] <
-00021460: 2072 6563 656e 745b 224c 4d41 225d 2e69   recent["LMA"].i
-00021470: 6c6f 635b 305d 3a0a 2020 2020 2020 2020  loc[0]:.        
-00021480: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-00021490: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-000214a0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-000214b0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
-000214c0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
-000214d0: 4420 2b20 636f 6c6f 7254 6578 742e 4641  D + colorText.FA
-000214e0: 494c 202b 2022 4265 6172 6973 6822 202b  IL + "Bearish" +
-000214f0: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
-00021500: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00021510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021520: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
-00021530: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
-00021540: 5d20 2b20 2242 6561 7269 7368 220a 2020  ] + "Bearish".  
-00021550: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00021560: 5369 676e 616c 732e 6170 7065 6e64 2822  Signals.append("
-00021570: 3222 290a 2020 2020 2020 2020 2020 2020  2").            
-00021580: 656c 6966 2072 6563 656e 745b 2253 4d41  elif recent["SMA
-00021590: 225d 2e69 6c6f 635b 305d 203d 3d20 303a  "].iloc[0] == 0:
-000215a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000215b0: 2073 6372 6565 6e44 6963 745b 224d 412d   screenDict["MA-
-000215c0: 5369 676e 616c 225d 203d 2028 0a20 2020  Signal"] = (.   
-000215d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000215e0: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
-000215f0: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
-00021600: 6f72 5465 7874 2e57 4152 4e20 2b20 2255  orText.WARN + "U
-00021610: 6e6b 6e6f 776e 2220 2b20 636f 6c6f 7254  nknown" + colorT
-00021620: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
-00021630: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00021640: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00021650: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-00021660: 3d20 7361 7665 645b 315d 202b 2022 556e  = saved[1] + "Un
-00021670: 6b6e 6f77 6e22 0a20 2020 2020 2020 2020  known".         
-00021680: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00021690: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
-000216a0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
-000216b0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-000216c0: 2020 2020 2020 2020 2073 6176 6564 5b30           saved[0
-000216d0: 5d20 2b20 636f 6c6f 7254 6578 742e 424f  ] + colorText.BO
-000216e0: 4c44 202b 2063 6f6c 6f72 5465 7874 2e57  LD + colorText.W
-000216f0: 4152 4e20 2b20 224e 6575 7472 616c 2220  ARN + "Neutral" 
-00021700: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-00021710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021720: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00021730: 2020 7361 7665 4469 6374 5b22 4d41 2d53    saveDict["MA-S
-00021740: 6967 6e61 6c22 5d20 3d20 7361 7665 645b  ignal"] = saved[
-00021750: 315d 202b 2022 4e65 7574 7261 6c22 0a20  1] + "Neutral". 
-00021760: 2020 2020 2020 2072 6576 6572 7365 6444         reversedD
-00021770: 6174 6120 3d20 6461 7461 5b3a 3a2d 315d  ata = data[::-1]
-00021780: 2020 2320 5265 7665 7273 6520 7468 6520    # Reverse the 
-00021790: 6461 7461 6672 616d 650a 2020 2020 2020  dataframe.      
-000217a0: 2020 656d 615f 3230 203d 2070 6b74 616c    ema_20 = pktal
-000217b0: 6962 2e45 4d41 2872 6576 6572 7365 6444  ib.EMA(reversedD
-000217c0: 6174 615b 2243 6c6f 7365 225d 2c32 3029  ata["Close"],20)
-000217d0: 2e74 6169 6c28 3129 2e69 6c6f 635b 305d  .tail(1).iloc[0]
-000217e0: 0a20 2020 2020 2020 2076 7761 7020 3d20  .        vwap = 
-000217f0: 706b 7461 6c69 622e 5657 4150 2872 6576  pktalib.VWAP(rev
-00021800: 6572 7365 6444 6174 615b 2248 6967 6822  ersedData["High"
-00021810: 5d2c 7265 7665 7273 6564 4461 7461 5b22  ],reversedData["
-00021820: 4c6f 7722 5d2c 7265 7665 7273 6564 4461  Low"],reversedDa
-00021830: 7461 5b22 436c 6f73 6522 5d2c 7265 7665  ta["Close"],reve
-00021840: 7273 6564 4461 7461 5b22 566f 6c75 6d65  rsedData["Volume
-00021850: 225d 292e 7461 696c 2831 292e 696c 6f63  "]).tail(1).iloc
-00021860: 5b30 5d0a 2020 2020 2020 2020 736d 6144  [0].        smaD
-00021870: 6576 203d 2064 6174 615b 2253 4d41 225d  ev = data["SMA"]
-00021880: 2e69 6c6f 635b 305d 202a 206d 6152 616e  .iloc[0] * maRan
-00021890: 6765 202f 2031 3030 0a20 2020 2020 2020  ge / 100.       
-000218a0: 206c 6d61 4465 7620 3d20 6461 7461 5b22   lmaDev = data["
-000218b0: 4c4d 4122 5d2e 696c 6f63 5b30 5d20 2a20  LMA"].iloc[0] * 
-000218c0: 6d61 5261 6e67 6520 2f20 3130 300a 2020  maRange / 100.  
-000218d0: 2020 2020 2020 656d 6144 6576 203d 2065        emaDev = e
-000218e0: 6d61 5f32 3020 2a20 6d61 5261 6e67 6520  ma_20 * maRange 
-000218f0: 2f20 3130 300a 2020 2020 2020 2020 7677  / 100.        vw
-00021900: 6170 4465 7620 3d20 7677 6170 202a 206d  apDev = vwap * m
-00021910: 6152 616e 6765 202f 2031 3030 0a20 2020  aRange / 100.   
-00021920: 2020 2020 206f 7065 6e2c 2068 6967 682c       open, high,
-00021930: 206c 6f77 2c20 636c 6f73 652c 2073 6d61   low, close, sma
-00021940: 2c20 6c6d 6120 3d20 280a 2020 2020 2020  , lma = (.      
-00021950: 2020 2020 2020 6461 7461 5b22 4f70 656e        data["Open
-00021960: 225d 2e69 6c6f 635b 305d 2c0a 2020 2020  "].iloc[0],.    
-00021970: 2020 2020 2020 2020 6461 7461 5b22 4869          data["Hi
-00021980: 6768 225d 2e69 6c6f 635b 305d 2c0a 2020  gh"].iloc[0],.  
-00021990: 2020 2020 2020 2020 2020 6461 7461 5b22            data["
-000219a0: 4c6f 7722 5d2e 696c 6f63 5b30 5d2c 0a20  Low"].iloc[0],. 
-000219b0: 2020 2020 2020 2020 2020 2064 6174 615b             data[
-000219c0: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
-000219d0: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-000219e0: 7461 5b22 534d 4122 5d2e 696c 6f63 5b30  ta["SMA"].iloc[0
-000219f0: 5d2c 0a20 2020 2020 2020 2020 2020 2064  ],.            d
-00021a00: 6174 615b 224c 4d41 225d 2e69 6c6f 635b  ata["LMA"].iloc[
-00021a10: 305d 2c0a 2020 2020 2020 2020 290a 2020  0],.        ).  
-00021a20: 2020 2020 2020 6d61 7320 3d20 5b73 6d61        mas = [sma
-00021a30: 2c6c 6d61 2c65 6d61 5f32 302c 7677 6170  ,lma,ema_20,vwap
-00021a40: 5d20 6966 206d 614c 656e 6774 683d 3d30  ] if maLength==0
-00021a50: 2065 6c73 6520 5b73 6d61 2c6c 6d61 2c65   else [sma,lma,e
-00021a60: 6d61 5f32 305d 0a20 2020 2020 2020 206d  ma_20].        m
-00021a70: 6144 6576 7320 3d20 5b73 6d61 4465 762c  aDevs = [smaDev,
-00021a80: 206c 6d61 4465 762c 2065 6d61 4465 762c   lmaDev, emaDev,
-00021a90: 2076 7761 7044 6576 5d20 6966 206d 614c   vwapDev] if maL
-00021aa0: 656e 6774 683d 3d30 2065 6c73 6520 5b73  ength==0 else [s
-00021ab0: 6d61 4465 762c 206c 6d61 4465 762c 2065  maDev, lmaDev, e
-00021ac0: 6d61 4465 765d 0a20 2020 2020 2020 206d  maDev].        m
-00021ad0: 6154 6578 7473 203d 205b 2235 304d 4122  aTexts = ["50MA"
-00021ae0: 2c22 3230 304d 4122 2c22 3230 454d 4122  ,"200MA","20EMA"
-00021af0: 2c22 5657 4150 225d 2069 6620 6d61 4c65  ,"VWAP"] if maLe
-00021b00: 6e67 7468 3d3d 3020 656c 7365 205b 2235  ngth==0 else ["5
-00021b10: 304d 4122 2c22 3230 304d 4122 2c22 3230  0MA","200MA","20
-00021b20: 454d 4122 5d0a 2020 2020 2020 2020 6d61  EMA"].        ma
-00021b30: 5265 7665 7273 616c 203d 2030 0a20 2020  Reversal = 0.   
-00021b40: 2020 2020 2069 6e64 6578 203d 2030 0a20       index = 0. 
-00021b50: 2020 2020 2020 2062 756c 6c69 7368 4361         bullishCa
-00021b60: 6e64 6c65 203d 2073 656c 662e 6765 7443  ndle = self.getC
-00021b70: 616e 646c 6554 7970 6528 6461 7461 290a  andleType(data).
-00021b80: 2020 2020 2020 2020 6966 2073 7472 286d          if str(m
-00021b90: 614c 656e 6774 6829 206e 6f74 2069 6e20  aLength) not in 
-00021ba0: 5b22 3222 2c22 3322 5d3a 0a20 2020 2020  ["2","3"]:.     
-00021bb0: 2020 2020 2020 2066 6f72 206d 6120 696e         for ma in
-00021bc0: 206d 6173 3a0a 2020 2020 2020 2020 2020   mas:.          
-00021bd0: 2020 2020 2020 7361 7665 6420 3d20 7365        saved = se
-00021be0: 6c66 2e66 696e 6443 7572 7265 6e74 5361  lf.findCurrentSa
-00021bf0: 7665 6456 616c 7565 2873 6372 6565 6e44  vedValue(screenD
-00021c00: 6963 742c 7361 7665 4469 6374 2c22 4d41  ict,saveDict,"MA
-00021c10: 2d53 6967 6e61 6c22 290a 2020 2020 2020  -Signal").      
-00021c20: 2020 2020 2020 2020 2020 2320 5461 6b69            # Taki
-00021c30: 6e67 2053 7570 706f 7274 0a20 2020 2020  ng Support.     
-00021c40: 2020 2020 2020 2020 2020 2069 6620 636c             if cl
-00021c50: 6f73 6520 3e20 6d61 2061 6e64 206c 6f77  ose > ma and low
-00021c60: 203c 3d20 286d 6120 2b20 6d61 4465 7673   <= (ma + maDevs
-00021c70: 5b69 6e64 6578 5d29 2061 6e64 2073 7472  [index]) and str
-00021c80: 286d 614c 656e 6774 6829 2069 6e20 5b22  (maLength) in ["
-00021c90: 3022 2c22 3122 5d3a 0a20 2020 2020 2020  0","1"]:.       
-00021ca0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
-00021cb0: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
-00021cc0: 616c 225d 203d 2028 0a20 2020 2020 2020  al"] = (.       
-00021cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021ce0: 2073 6176 6564 5b30 5d20 2b20 636f 6c6f   saved[0] + colo
-00021cf0: 7254 6578 742e 424f 4c44 202b 2063 6f6c  rText.BOLD + col
-00021d00: 6f72 5465 7874 2e47 5245 454e 202b 2066  orText.GREEN + f
-00021d10: 227b 6d61 5465 7874 735b 696e 6465 785d  "{maTexts[index]
-00021d20: 7d2d 5375 7070 6f72 7422 202b 2063 6f6c  }-Support" + col
-00021d30: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
-00021d40: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00021d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021d60: 2020 2020 2073 6176 6544 6963 745b 224d       saveDict["M
-00021d70: 412d 5369 676e 616c 225d 203d 2073 6176  A-Signal"] = sav
-00021d80: 6564 5b31 5d20 2b20 6622 7b6d 6154 6578  ed[1] + f"{maTex
-00021d90: 7473 5b69 6e64 6578 5d7d 2d53 7570 706f  ts[index]}-Suppo
-00021da0: 7274 220a 2020 2020 2020 2020 2020 2020  rt".            
-00021db0: 2020 2020 2020 2020 6d61 5265 7665 7273          maRevers
-00021dc0: 616c 203d 2031 0a20 2020 2020 2020 2020  al = 1.         
-00021dd0: 2020 2020 2020 2020 2020 206d 6153 6967             maSig
-00021de0: 6e61 6c73 2e61 7070 656e 6428 2231 2229  nals.append("1")
-00021df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021e00: 2023 2056 616c 6964 6174 696e 6720 5265   # Validating Re
-00021e10: 7369 7374 616e 6365 0a20 2020 2020 2020  sistance.       
-00021e20: 2020 2020 2020 2020 2065 6c69 6620 636c           elif cl
-00021e30: 6f73 6520 3c20 6d61 2061 6e64 2068 6967  ose < ma and hig
-00021e40: 6820 3e3d 2028 6d61 202d 206d 6144 6576  h >= (ma - maDev
-00021e50: 735b 696e 6465 785d 2920 616e 6420 7374  s[index]) and st
-00021e60: 7228 6d61 4c65 6e67 7468 2920 696e 205b  r(maLength) in [
-00021e70: 2230 222c 2236 225d 3a0a 2020 2020 2020  "0","6"]:.      
-00021e80: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00021e90: 7265 656e 4469 6374 5b22 4d41 2d53 6967  reenDict["MA-Sig
-00021ea0: 6e61 6c22 5d20 3d20 280a 2020 2020 2020  nal"] = (.      
-00021eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021ec0: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
-00021ed0: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
-00021ee0: 6c6f 7254 6578 742e 4641 494c 202b 2066  lorText.FAIL + f
-00021ef0: 227b 6d61 5465 7874 735b 696e 6465 785d  "{maTexts[index]
-00021f00: 7d2d 5265 7369 7374 2220 2b20 636f 6c6f  }-Resist" + colo
-00021f10: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
-00021f20: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00021f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021f40: 2020 2020 7361 7665 4469 6374 5b22 4d41      saveDict["MA
-00021f50: 2d53 6967 6e61 6c22 5d20 3d20 7361 7665  -Signal"] = save
-00021f60: 645b 315d 202b 2066 227b 6d61 5465 7874  d[1] + f"{maText
-00021f70: 735b 696e 6465 785d 7d2d 5265 7369 7374  s[index]}-Resist
-00021f80: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00021f90: 2020 2020 2020 6d61 5265 7665 7273 616c        maReversal
-00021fa0: 203d 202d 310a 2020 2020 2020 2020 2020   = -1.          
-00021fb0: 2020 2020 2020 2020 2020 6d61 5369 676e            maSign
-00021fc0: 616c 732e 6170 7065 6e64 2822 3622 290a  als.append("6").
-00021fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021fe0: 2320 466f 7220 6120 4275 6c6c 6973 6820  # For a Bullish 
-00021ff0: 4361 6e64 6c65 0a20 2020 2020 2020 2020  Candle.         
-00022000: 2020 2020 2020 2069 6620 6275 6c6c 6973         if bullis
-00022010: 6843 616e 646c 653a 0a20 2020 2020 2020  hCandle:.       
-00022020: 2020 2020 2020 2020 2020 2020 2023 2043               # C
-00022030: 726f 7373 696e 6720 7570 0a20 2020 2020  rossing up.     
-00022040: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00022050: 6620 6f70 656e 203c 206d 6120 616e 6420  f open < ma and 
-00022060: 636c 6f73 6520 3e20 6d61 2061 6e64 2073  close > ma and s
-00022070: 7472 286d 614c 656e 6774 6829 2069 6e20  tr(maLength) in 
-00022080: 5b22 3022 2c22 3522 5d3a 0a20 2020 2020  ["0","5"]:.     
-00022090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000220a0: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
-000220b0: 412d 5369 676e 616c 225d 203d 2028 0a20  A-Signal"] = (. 
-000220c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000220d0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
-000220e0: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
-000220f0: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
-00022100: 2e47 5245 454e 202b 2066 2242 756c 6c43  .GREEN + f"BullC
-00022110: 726f 7373 2d7b 6d61 5465 7874 735b 696e  ross-{maTexts[in
-00022120: 6465 785d 7d22 202b 2063 6f6c 6f72 5465  dex]}" + colorTe
-00022130: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
-00022140: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00022150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022160: 2020 2020 2020 2020 2073 6176 6544 6963           saveDic
-00022170: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
-00022180: 2073 6176 6564 5b31 5d20 2b20 6622 4275   saved[1] + f"Bu
-00022190: 6c6c 4372 6f73 732d 7b6d 6154 6578 7473  llCross-{maTexts
-000221a0: 5b69 6e64 6578 5d7d 220a 2020 2020 2020  [index]}".      
-000221b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000221c0: 2020 6d61 5265 7665 7273 616c 203d 2031    maReversal = 1
-000221d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000221e0: 2020 2020 2020 2020 206d 6153 6967 6e61           maSigna
-000221f0: 6c73 2e61 7070 656e 6428 2235 2229 0a20  ls.append("5"). 
-00022200: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00022210: 2046 6f72 2061 2042 6561 7269 7368 2043   For a Bearish C
-00022220: 616e 646c 650a 2020 2020 2020 2020 2020  andle.          
-00022230: 2020 2020 2020 656c 6966 206e 6f74 2062        elif not b
-00022240: 756c 6c69 7368 4361 6e64 6c65 3a0a 2020  ullishCandle:.  
-00022250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022260: 2020 2320 4372 6f73 7369 6e67 2064 6f77    # Crossing dow
-00022270: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00022280: 2020 2020 2020 6966 206f 7065 6e20 3e20        if open > 
-00022290: 736d 6120 616e 6420 636c 6f73 6520 3c20  sma and close < 
-000222a0: 736d 6120 616e 6420 7374 7228 6d61 4c65  sma and str(maLe
-000222b0: 6e67 7468 2920 696e 205b 2230 222c 2234  ngth) in ["0","4
-000222c0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-000222d0: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-000222e0: 656e 4469 6374 5b22 4d41 2d53 6967 6e61  enDict["MA-Signa
-000222f0: 6c22 5d20 3d20 280a 2020 2020 2020 2020  l"] = (.        
+00020e90: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00020ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020eb0: 7361 7665 4469 6374 5b22 5061 7474 6572  saveDict["Patter
+00020ec0: 6e22 5d20 3d20 7361 7665 645b 315d 202b  n"] = saved[1] +
+00020ed0: 2022 4d6f 6d65 6e74 756d 2047 6169 6e65   "Momentum Gaine
+00020ee0: 7222 0a20 2020 2020 2020 2020 2020 2020  r".             
+00020ef0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00020f00: 6e20 5472 7565 0a20 2020 2020 2020 2020  n True.         
+00020f10: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
+00020f20: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
+00020f30: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
+00020f40: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+00020f50: 2066 2753 746f 636b 3a7b 7361 7665 4469   f'Stock:{saveDi
+00020f60: 6374 5b22 5374 6f63 6b22 5d7d 2c20 6973  ct["Stock"]}, is
+00020f70: 206e 6f74 2061 206d 6f6d 656e 7475 6d2d   not a momentum-
+00020f80: 6761 696e 6572 2062 6563 6175 7365 2065  gainer because e
+00020f90: 6974 6865 7220 746f 6461 792d 6f70 656e  ither today-open
+00020fa0: 2028 7b74 6f7d 2920 3c20 7965 7374 6572   ({to}) < yester
+00020fb0: 6461 792d 636c 6f73 6520 287b 7963 7d29  day-close ({yc})
+00020fc0: 206f 7220 7965 7374 6572 6461 792d 6f70   or yesterday-op
+00020fd0: 656e 287b 796f 7d29 203c 2064 6179 2d62  en({yo}) < day-b
+00020fe0: 6566 6f72 652d 636c 6f73 6528 7b64 7963  efore-close({dyc
+00020ff0: 7d29 270a 2020 2020 2020 2020 2020 2020  })'.            
+00021000: 2020 2020 2020 2020 2320 290a 2020 2020          # ).    
+00021010: 2020 2020 2020 2020 6578 6365 7074 2049          except I
+00021020: 6e64 6578 4572 726f 7220 6173 2065 3a20  ndexError as e: 
+00021030: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+00021040: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
+00021050: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
+00021060: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
+00021070: 6578 635f 696e 666f 3d54 7275 6529 0a20  exc_info=True). 
+00021080: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00021090: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
+000210a0: 6572 2e64 6562 7567 2864 6174 6129 0a20  er.debug(data). 
+000210b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000210c0: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
+000210d0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+000210e0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+000210f0: 7074 696f 6e20 6173 2065 3a20 2023 2070  ption as e:  # p
+00021100: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
+00021110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00021120: 2e64 6566 6175 6c74 5f6c 6f67 6765 722e  .default_logger.
+00021130: 6465 6275 6728 652c 2065 7863 5f69 6e66  debug(e, exc_inf
+00021140: 6f3d 5472 7565 290a 2020 2020 2020 2020  o=True).        
+00021150: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00021160: 0a0a 2020 2020 2340 6d65 6173 7572 655f  ..    #@measure_
+00021170: 7469 6d65 0a20 2020 2023 2056 616c 6964  time.    # Valid
+00021180: 6174 6520 4d6f 7669 6e67 2061 7665 7261  ate Moving avera
+00021190: 6765 7320 616e 6420 6c6f 6f6b 2066 6f72  ges and look for
+000211a0: 2062 7579 2f73 656c 6c20 7369 676e 616c   buy/sell signal
+000211b0: 730a 2020 2020 6465 6620 7661 6c69 6461  s.    def valida
+000211c0: 7465 4d6f 7669 6e67 4176 6572 6167 6573  teMovingAverages
+000211d0: 2873 656c 662c 2064 662c 2073 6372 6565  (self, df, scree
+000211e0: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
+000211f0: 206d 6152 616e 6765 3d32 2e35 2c6d 614c   maRange=2.5,maL
+00021200: 656e 6774 683d 3029 3a0a 2020 2020 2020  ength=0):.      
+00021210: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
+00021220: 2829 0a20 2020 2020 2020 2064 6174 6120  ().        data 
+00021230: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
+00021240: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00021250: 6461 7461 2e72 6570 6c61 6365 285b 6e70  data.replace([np
+00021260: 2e69 6e66 2c20 2d6e 702e 696e 665d 2c20  .inf, -np.inf], 
+00021270: 3029 0a20 2020 2020 2020 2072 6563 656e  0).        recen
+00021280: 7420 3d20 6461 7461 2e68 6561 6428 3129  t = data.head(1)
+00021290: 0a20 2020 2020 2020 206d 6153 6967 6e61  .        maSigna
+000212a0: 6c73 203d 205b 5d0a 2020 2020 2020 2020  ls = [].        
+000212b0: 6966 2073 7472 286d 614c 656e 6774 6829  if str(maLength)
+000212c0: 2069 6e20 5b22 3022 2c22 3222 2c22 3322   in ["0","2","3"
+000212d0: 5d3a 0a20 2020 2020 2020 2020 2020 2073  ]:.            s
+000212e0: 6176 6564 203d 2073 656c 662e 6669 6e64  aved = self.find
+000212f0: 4375 7272 656e 7453 6176 6564 5661 6c75  CurrentSavedValu
+00021300: 6528 7363 7265 656e 4469 6374 2c73 6176  e(screenDict,sav
+00021310: 6544 6963 742c 224d 412d 5369 676e 616c  eDict,"MA-Signal
+00021320: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
+00021330: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00021340: 2020 2020 7265 6365 6e74 5b22 534d 4122      recent["SMA"
+00021350: 5d2e 696c 6f63 5b30 5d20 3e20 7265 6365  ].iloc[0] > rece
+00021360: 6e74 5b22 4c4d 4122 5d2e 696c 6f63 5b30  nt["LMA"].iloc[0
+00021370: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00021380: 2020 616e 6420 7265 6365 6e74 5b22 436c    and recent["Cl
+00021390: 6f73 6522 5d2e 696c 6f63 5b30 5d20 3e20  ose"].iloc[0] > 
+000213a0: 7265 6365 6e74 5b22 534d 4122 5d2e 696c  recent["SMA"].il
+000213b0: 6f63 5b30 5d0a 2020 2020 2020 2020 2020  oc[0].          
+000213c0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+000213d0: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
+000213e0: 224d 412d 5369 676e 616c 225d 203d 2028  "MA-Signal"] = (
+000213f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021400: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
+00021410: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
+00021420: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+00021430: 202b 2022 4275 6c6c 6973 6822 202b 2063   + "Bullish" + c
+00021440: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
+00021450: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00021460: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00021470: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
+00021480: 616c 225d 203d 2073 6176 6564 5b31 5d20  al"] = saved[1] 
+00021490: 2b20 2242 756c 6c69 7368 220a 2020 2020  + "Bullish".    
+000214a0: 2020 2020 2020 2020 2020 2020 6d61 5369              maSi
+000214b0: 676e 616c 732e 6170 7065 6e64 2822 3322  gnals.append("3"
+000214c0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+000214d0: 6966 2072 6563 656e 745b 2253 4d41 225d  if recent["SMA"]
+000214e0: 2e69 6c6f 635b 305d 203c 2072 6563 656e  .iloc[0] < recen
+000214f0: 745b 224c 4d41 225d 2e69 6c6f 635b 305d  t["LMA"].iloc[0]
+00021500: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00021510: 2020 7363 7265 656e 4469 6374 5b22 4d41    screenDict["MA
+00021520: 2d53 6967 6e61 6c22 5d20 3d20 280a 2020  -Signal"] = (.  
+00021530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021540: 2020 7361 7665 645b 305d 202b 2063 6f6c    saved[0] + col
+00021550: 6f72 5465 7874 2e42 4f4c 4420 2b20 636f  orText.BOLD + co
+00021560: 6c6f 7254 6578 742e 4641 494c 202b 2022  lorText.FAIL + "
+00021570: 4265 6172 6973 6822 202b 2063 6f6c 6f72  Bearish" + color
+00021580: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+00021590: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000215a0: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+000215b0: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
+000215c0: 203d 2073 6176 6564 5b31 5d20 2b20 2242   = saved[1] + "B
+000215d0: 6561 7269 7368 220a 2020 2020 2020 2020  earish".        
+000215e0: 2020 2020 2020 2020 6d61 5369 676e 616c          maSignal
+000215f0: 732e 6170 7065 6e64 2822 3222 290a 2020  s.append("2").  
+00021600: 2020 2020 2020 2020 2020 656c 6966 2072            elif r
+00021610: 6563 656e 745b 2253 4d41 225d 2e69 6c6f  ecent["SMA"].ilo
+00021620: 635b 305d 203d 3d20 303a 0a20 2020 2020  c[0] == 0:.     
+00021630: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+00021640: 6e44 6963 745b 224d 412d 5369 676e 616c  nDict["MA-Signal
+00021650: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
+00021660: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+00021670: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
+00021680: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
+00021690: 2e57 4152 4e20 2b20 2255 6e6b 6e6f 776e  .WARN + "Unknown
+000216a0: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
+000216b0: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+000216c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000216d0: 2020 2020 7361 7665 4469 6374 5b22 4d41      saveDict["MA
+000216e0: 2d53 6967 6e61 6c22 5d20 3d20 7361 7665  -Signal"] = save
+000216f0: 645b 315d 202b 2022 556e 6b6e 6f77 6e22  d[1] + "Unknown"
+00021700: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00021710: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00021720: 2020 2073 6372 6565 6e44 6963 745b 224d     screenDict["M
+00021730: 412d 5369 676e 616c 225d 203d 2028 0a20  A-Signal"] = (. 
+00021740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021750: 2020 2073 6176 6564 5b30 5d20 2b20 636f     saved[0] + co
+00021760: 6c6f 7254 6578 742e 424f 4c44 202b 2063  lorText.BOLD + c
+00021770: 6f6c 6f72 5465 7874 2e57 4152 4e20 2b20  olorText.WARN + 
+00021780: 224e 6575 7472 616c 2220 2b20 636f 6c6f  "Neutral" + colo
+00021790: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+000217a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000217b0: 2020 2020 2020 2020 2020 2020 7361 7665              save
+000217c0: 4469 6374 5b22 4d41 2d53 6967 6e61 6c22  Dict["MA-Signal"
+000217d0: 5d20 3d20 7361 7665 645b 315d 202b 2022  ] = saved[1] + "
+000217e0: 4e65 7574 7261 6c22 0a20 2020 2020 2020  Neutral".       
+000217f0: 2072 6576 6572 7365 6444 6174 6120 3d20   reversedData = 
+00021800: 6461 7461 5b3a 3a2d 315d 2020 2320 5265  data[::-1]  # Re
+00021810: 7665 7273 6520 7468 6520 6461 7461 6672  verse the datafr
+00021820: 616d 650a 2020 2020 2020 2020 656d 615f  ame.        ema_
+00021830: 3230 203d 2070 6b74 616c 6962 2e45 4d41  20 = pktalib.EMA
+00021840: 2872 6576 6572 7365 6444 6174 615b 2243  (reversedData["C
+00021850: 6c6f 7365 225d 2c32 3029 2e74 6169 6c28  lose"],20).tail(
+00021860: 3129 2e69 6c6f 635b 305d 0a20 2020 2020  1).iloc[0].     
+00021870: 2020 2076 7761 7020 3d20 706b 7461 6c69     vwap = pktali
+00021880: 622e 5657 4150 2872 6576 6572 7365 6444  b.VWAP(reversedD
+00021890: 6174 615b 2248 6967 6822 5d2c 7265 7665  ata["High"],reve
+000218a0: 7273 6564 4461 7461 5b22 4c6f 7722 5d2c  rsedData["Low"],
+000218b0: 7265 7665 7273 6564 4461 7461 5b22 436c  reversedData["Cl
+000218c0: 6f73 6522 5d2c 7265 7665 7273 6564 4461  ose"],reversedDa
+000218d0: 7461 5b22 566f 6c75 6d65 225d 292e 7461  ta["Volume"]).ta
+000218e0: 696c 2831 292e 696c 6f63 5b30 5d0a 2020  il(1).iloc[0].  
+000218f0: 2020 2020 2020 736d 6144 6576 203d 2064        smaDev = d
+00021900: 6174 615b 2253 4d41 225d 2e69 6c6f 635b  ata["SMA"].iloc[
+00021910: 305d 202a 206d 6152 616e 6765 202f 2031  0] * maRange / 1
+00021920: 3030 0a20 2020 2020 2020 206c 6d61 4465  00.        lmaDe
+00021930: 7620 3d20 6461 7461 5b22 4c4d 4122 5d2e  v = data["LMA"].
+00021940: 696c 6f63 5b30 5d20 2a20 6d61 5261 6e67  iloc[0] * maRang
+00021950: 6520 2f20 3130 300a 2020 2020 2020 2020  e / 100.        
+00021960: 656d 6144 6576 203d 2065 6d61 5f32 3020  emaDev = ema_20 
+00021970: 2a20 6d61 5261 6e67 6520 2f20 3130 300a  * maRange / 100.
+00021980: 2020 2020 2020 2020 7677 6170 4465 7620          vwapDev 
+00021990: 3d20 7677 6170 202a 206d 6152 616e 6765  = vwap * maRange
+000219a0: 202f 2031 3030 0a20 2020 2020 2020 206f   / 100.        o
+000219b0: 7065 6e2c 2068 6967 682c 206c 6f77 2c20  pen, high, low, 
+000219c0: 636c 6f73 652c 2073 6d61 2c20 6c6d 6120  close, sma, lma 
+000219d0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+000219e0: 6461 7461 5b22 4f70 656e 225d 2e69 6c6f  data["Open"].ilo
+000219f0: 635b 305d 2c0a 2020 2020 2020 2020 2020  c[0],.          
+00021a00: 2020 6461 7461 5b22 4869 6768 225d 2e69    data["High"].i
+00021a10: 6c6f 635b 305d 2c0a 2020 2020 2020 2020  loc[0],.        
+00021a20: 2020 2020 6461 7461 5b22 4c6f 7722 5d2e      data["Low"].
+00021a30: 696c 6f63 5b30 5d2c 0a20 2020 2020 2020  iloc[0],.       
+00021a40: 2020 2020 2064 6174 615b 2243 6c6f 7365       data["Close
+00021a50: 225d 2e69 6c6f 635b 305d 2c0a 2020 2020  "].iloc[0],.    
+00021a60: 2020 2020 2020 2020 6461 7461 5b22 534d          data["SM
+00021a70: 4122 5d2e 696c 6f63 5b30 5d2c 0a20 2020  A"].iloc[0],.   
+00021a80: 2020 2020 2020 2020 2064 6174 615b 224c           data["L
+00021a90: 4d41 225d 2e69 6c6f 635b 305d 2c0a 2020  MA"].iloc[0],.  
+00021aa0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00021ab0: 6d61 7320 3d20 5b73 6d61 2c6c 6d61 2c65  mas = [sma,lma,e
+00021ac0: 6d61 5f32 302c 7677 6170 5d20 6966 206d  ma_20,vwap] if m
+00021ad0: 614c 656e 6774 683d 3d30 2065 6c73 6520  aLength==0 else 
+00021ae0: 5b73 6d61 2c6c 6d61 2c65 6d61 5f32 305d  [sma,lma,ema_20]
+00021af0: 0a20 2020 2020 2020 206d 6144 6576 7320  .        maDevs 
+00021b00: 3d20 5b73 6d61 4465 762c 206c 6d61 4465  = [smaDev, lmaDe
+00021b10: 762c 2065 6d61 4465 762c 2076 7761 7044  v, emaDev, vwapD
+00021b20: 6576 5d20 6966 206d 614c 656e 6774 683d  ev] if maLength=
+00021b30: 3d30 2065 6c73 6520 5b73 6d61 4465 762c  =0 else [smaDev,
+00021b40: 206c 6d61 4465 762c 2065 6d61 4465 765d   lmaDev, emaDev]
+00021b50: 0a20 2020 2020 2020 206d 6154 6578 7473  .        maTexts
+00021b60: 203d 205b 2235 304d 4122 2c22 3230 304d   = ["50MA","200M
+00021b70: 4122 2c22 3230 454d 4122 2c22 5657 4150  A","20EMA","VWAP
+00021b80: 225d 2069 6620 6d61 4c65 6e67 7468 3d3d  "] if maLength==
+00021b90: 3020 656c 7365 205b 2235 304d 4122 2c22  0 else ["50MA","
+00021ba0: 3230 304d 4122 2c22 3230 454d 4122 5d0a  200MA","20EMA"].
+00021bb0: 2020 2020 2020 2020 6d61 5265 7665 7273          maRevers
+00021bc0: 616c 203d 2030 0a20 2020 2020 2020 2069  al = 0.        i
+00021bd0: 6e64 6578 203d 2030 0a20 2020 2020 2020  ndex = 0.       
+00021be0: 2062 756c 6c69 7368 4361 6e64 6c65 203d   bullishCandle =
+00021bf0: 2073 656c 662e 6765 7443 616e 646c 6554   self.getCandleT
+00021c00: 7970 6528 6461 7461 290a 2020 2020 2020  ype(data).      
+00021c10: 2020 6966 2073 7472 286d 614c 656e 6774    if str(maLengt
+00021c20: 6829 206e 6f74 2069 6e20 5b22 3222 2c22  h) not in ["2","
+00021c30: 3322 5d3a 0a20 2020 2020 2020 2020 2020  3"]:.           
+00021c40: 2066 6f72 206d 6120 696e 206d 6173 3a0a   for ma in mas:.
+00021c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c60: 7361 7665 6420 3d20 7365 6c66 2e66 696e  saved = self.fin
+00021c70: 6443 7572 7265 6e74 5361 7665 6456 616c  dCurrentSavedVal
+00021c80: 7565 2873 6372 6565 6e44 6963 742c 7361  ue(screenDict,sa
+00021c90: 7665 4469 6374 2c22 4d41 2d53 6967 6e61  veDict,"MA-Signa
+00021ca0: 6c22 290a 2020 2020 2020 2020 2020 2020  l").            
+00021cb0: 2020 2020 2320 5461 6b69 6e67 2053 7570      # Taking Sup
+00021cc0: 706f 7274 0a20 2020 2020 2020 2020 2020  port.           
+00021cd0: 2020 2020 2069 6620 636c 6f73 6520 3e20       if close > 
+00021ce0: 6d61 2061 6e64 206c 6f77 203c 3d20 286d  ma and low <= (m
+00021cf0: 6120 2b20 6d61 4465 7673 5b69 6e64 6578  a + maDevs[index
+00021d00: 5d29 2061 6e64 2073 7472 286d 614c 656e  ]) and str(maLen
+00021d10: 6774 6829 2069 6e20 5b22 3022 2c22 3122  gth) in ["0","1"
+00021d20: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00021d30: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
+00021d40: 745b 224d 412d 5369 676e 616c 225d 203d  t["MA-Signal"] =
+00021d50: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00021d60: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+00021d70: 5b30 5d20 2b20 636f 6c6f 7254 6578 742e  [0] + colorText.
+00021d80: 424f 4c44 202b 2063 6f6c 6f72 5465 7874  BOLD + colorText
+00021d90: 2e47 5245 454e 202b 2066 227b 6d61 5465  .GREEN + f"{maTe
+00021da0: 7874 735b 696e 6465 785d 7d2d 5375 7070  xts[index]}-Supp
+00021db0: 6f72 7422 202b 2063 6f6c 6f72 5465 7874  ort" + colorText
+00021dc0: 2e45 4e44 0a20 2020 2020 2020 2020 2020  .END.           
+00021dd0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00021de0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00021df0: 6176 6544 6963 745b 224d 412d 5369 676e  aveDict["MA-Sign
+00021e00: 616c 225d 203d 2073 6176 6564 5b31 5d20  al"] = saved[1] 
+00021e10: 2b20 6622 7b6d 6154 6578 7473 5b69 6e64  + f"{maTexts[ind
+00021e20: 6578 5d7d 2d53 7570 706f 7274 220a 2020  ex]}-Support".  
+00021e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021e40: 2020 6d61 5265 7665 7273 616c 203d 2031    maReversal = 1
+00021e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021e60: 2020 2020 206d 6153 6967 6e61 6c73 2e61       maSignals.a
+00021e70: 7070 656e 6428 2231 2229 0a20 2020 2020  ppend("1").     
+00021e80: 2020 2020 2020 2020 2020 2023 2056 616c             # Val
+00021e90: 6964 6174 696e 6720 5265 7369 7374 616e  idating Resistan
+00021ea0: 6365 0a20 2020 2020 2020 2020 2020 2020  ce.             
+00021eb0: 2020 2065 6c69 6620 636c 6f73 6520 3c20     elif close < 
+00021ec0: 6d61 2061 6e64 2068 6967 6820 3e3d 2028  ma and high >= (
+00021ed0: 6d61 202d 206d 6144 6576 735b 696e 6465  ma - maDevs[inde
+00021ee0: 785d 2920 616e 6420 7374 7228 6d61 4c65  x]) and str(maLe
+00021ef0: 6e67 7468 2920 696e 205b 2230 222c 2236  ngth) in ["0","6
+00021f00: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+00021f10: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+00021f20: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
+00021f30: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00021f40: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00021f50: 645b 305d 202b 2063 6f6c 6f72 5465 7874  d[0] + colorText
+00021f60: 2e42 4f4c 4420 2b20 636f 6c6f 7254 6578  .BOLD + colorTex
+00021f70: 742e 4641 494c 202b 2066 227b 6d61 5465  t.FAIL + f"{maTe
+00021f80: 7874 735b 696e 6465 785d 7d2d 5265 7369  xts[index]}-Resi
+00021f90: 7374 2220 2b20 636f 6c6f 7254 6578 742e  st" + colorText.
+00021fa0: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
+00021fb0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00021fc0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00021fd0: 7665 4469 6374 5b22 4d41 2d53 6967 6e61  veDict["MA-Signa
+00021fe0: 6c22 5d20 3d20 7361 7665 645b 315d 202b  l"] = saved[1] +
+00021ff0: 2066 227b 6d61 5465 7874 735b 696e 6465   f"{maTexts[inde
+00022000: 785d 7d2d 5265 7369 7374 220a 2020 2020  x]}-Resist".    
+00022010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022020: 6d61 5265 7665 7273 616c 203d 202d 310a  maReversal = -1.
+00022030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022040: 2020 2020 6d61 5369 676e 616c 732e 6170      maSignals.ap
+00022050: 7065 6e64 2822 3622 290a 2020 2020 2020  pend("6").      
+00022060: 2020 2020 2020 2020 2020 2320 466f 7220            # For 
+00022070: 6120 4275 6c6c 6973 6820 4361 6e64 6c65  a Bullish Candle
+00022080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022090: 2069 6620 6275 6c6c 6973 6843 616e 646c   if bullishCandl
+000220a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000220b0: 2020 2020 2020 2023 2043 726f 7373 696e         # Crossin
+000220c0: 6720 7570 0a20 2020 2020 2020 2020 2020  g up.           
+000220d0: 2020 2020 2020 2020 2069 6620 6f70 656e           if open
+000220e0: 203c 206d 6120 616e 6420 636c 6f73 6520   < ma and close 
+000220f0: 3e20 6d61 2061 6e64 2073 7472 286d 614c  > ma and str(maL
+00022100: 656e 6774 6829 2069 6e20 5b22 3022 2c22  ength) in ["0","
+00022110: 3522 5d3a 0a20 2020 2020 2020 2020 2020  5"]:.           
+00022120: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00022130: 6565 6e44 6963 745b 224d 412d 5369 676e  eenDict["MA-Sign
+00022140: 616c 225d 203d 2028 0a20 2020 2020 2020  al"] = (.       
+00022150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022160: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
+00022170: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
+00022180: 2063 6f6c 6f72 5465 7874 2e47 5245 454e   colorText.GREEN
+00022190: 202b 2066 2242 756c 6c43 726f 7373 2d7b   + f"BullCross-{
+000221a0: 6d61 5465 7874 735b 696e 6465 785d 7d22  maTexts[index]}"
+000221b0: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
+000221c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000221d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000221e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000221f0: 2020 2073 6176 6544 6963 745b 224d 412d     saveDict["MA-
+00022200: 5369 676e 616c 225d 203d 2073 6176 6564  Signal"] = saved
+00022210: 5b31 5d20 2b20 6622 4275 6c6c 4372 6f73  [1] + f"BullCros
+00022220: 732d 7b6d 6154 6578 7473 5b69 6e64 6578  s-{maTexts[index
+00022230: 5d7d 220a 2020 2020 2020 2020 2020 2020  ]}".            
+00022240: 2020 2020 2020 2020 2020 2020 6d61 5265              maRe
+00022250: 7665 7273 616c 203d 2031 0a20 2020 2020  versal = 1.     
+00022260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022270: 2020 206d 6153 6967 6e61 6c73 2e61 7070     maSignals.app
+00022280: 656e 6428 2235 2229 0a20 2020 2020 2020  end("5").       
+00022290: 2020 2020 2020 2020 2023 2046 6f72 2061           # For a
+000222a0: 2042 6561 7269 7368 2043 616e 646c 650a   Bearish Candle.
+000222b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000222c0: 656c 6966 206e 6f74 2062 756c 6c69 7368  elif not bullish
+000222d0: 4361 6e64 6c65 3a0a 2020 2020 2020 2020  Candle:.        
+000222e0: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
+000222f0: 6f73 7369 6e67 2064 6f77 6e0a 2020 2020  ossing down.    
 00022300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022310: 2020 2020 7361 7665 645b 305d 202b 2063      saved[0] + c
-00022320: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
-00022330: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
-00022340: 2066 2242 6561 7243 726f 7373 2d7b 6d61   f"BearCross-{ma
-00022350: 5465 7874 735b 696e 6465 785d 7d22 202b  Texts[index]}" +
-00022360: 2063 6f6c 6f72 5465 7874 2e45 4e44 0a20   colorText.END. 
-00022370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022380: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00022390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000223a0: 2073 6176 6544 6963 745b 224d 412d 5369   saveDict["MA-Si
-000223b0: 676e 616c 225d 203d 2073 6176 6564 5b31  gnal"] = saved[1
-000223c0: 5d20 2b20 6622 4265 6172 4372 6f73 732d  ] + f"BearCross-
-000223d0: 7b6d 6154 6578 7473 5b69 6e64 6578 5d7d  {maTexts[index]}
-000223e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000223f0: 2020 2020 2020 2020 2020 6d61 5265 7665            maReve
-00022400: 7273 616c 203d 202d 310a 2020 2020 2020  rsal = -1.      
-00022410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022420: 2020 6d61 5369 676e 616c 732e 6170 7065    maSignals.appe
-00022430: 6e64 2822 3422 290a 2020 2020 2020 2020  nd("4").        
-00022440: 2020 2020 2020 2020 696e 6465 7820 2b3d          index +=
-00022450: 2031 0a20 2020 2020 2020 2072 6574 7572   1.        retur
-00022460: 6e56 616c 7565 203d 206d 6152 6576 6572  nValue = maRever
-00022470: 7361 6c0a 2020 2020 2020 2020 6966 206d  sal.        if m
-00022480: 614c 656e 6774 6820 213d 2030 3a0a 2020  aLength != 0:.  
-00022490: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000224a0: 5661 6c75 6520 3d20 7374 7228 6d61 4c65  Value = str(maLe
-000224b0: 6e67 7468 2920 696e 206d 6153 6967 6e61  ngth) in maSigna
-000224c0: 6c73 0a20 2020 2020 2020 2072 6574 7572  ls.        retur
-000224d0: 6e20 7265 7475 726e 5661 6c75 650a 0a20  n returnValue.. 
-000224e0: 2020 2023 2046 696e 6420 4e52 7820 7261     # Find NRx ra
-000224f0: 6e67 6520 666f 7220 5265 7665 7273 616c  nge for Reversal
-00022500: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00022510: 654e 6172 726f 7752 616e 6765 2873 656c  eNarrowRange(sel
-00022520: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
-00022530: 742c 2073 6176 6544 6963 742c 206e 723d  t, saveDict, nr=
-00022540: 3429 3a0a 2020 2020 2020 2020 6966 2064  4):.        if d
-00022550: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
-00022560: 2864 6629 203d 3d20 303a 0a20 2020 2020  (df) == 0:.     
-00022570: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00022580: 6c73 650a 2020 2020 2020 2020 6461 7461  lse.        data
-00022590: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
-000225a0: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
-000225b0: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
-000225c0: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
-000225d0: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
-000225e0: 6174 7465 726e 2229 0a20 2020 2020 2020  attern").       
-000225f0: 2069 6620 504b 4461 7465 5574 696c 6974   if PKDateUtilit
-00022600: 6965 732e 6973 5472 6164 696e 6754 696d  ies.isTradingTim
-00022610: 6528 293a 0a20 2020 2020 2020 2020 2020  e():.           
-00022620: 2072 616e 6765 4461 7461 203d 2064 6174   rangeData = dat
-00022630: 612e 6865 6164 286e 7220 2b20 3129 5b31  a.head(nr + 1)[1
-00022640: 3a5d 0a20 2020 2020 2020 2020 2020 206e  :].            n
-00022650: 6f77 5f63 616e 646c 6520 3d20 6461 7461  ow_candle = data
-00022660: 2e68 6561 6428 3129 0a20 2020 2020 2020  .head(1).       
-00022670: 2020 2020 2072 616e 6765 4461 7461 5b22       rangeData["
-00022680: 5261 6e67 6522 5d20 3d20 6162 7328 7261  Range"] = abs(ra
-00022690: 6e67 6544 6174 615b 2243 6c6f 7365 225d  ngeData["Close"]
-000226a0: 202d 2072 616e 6765 4461 7461 5b22 4f70   - rangeData["Op
-000226b0: 656e 225d 290a 2020 2020 2020 2020 2020  en"]).          
-000226c0: 2020 7265 6365 6e74 203d 2072 616e 6765    recent = range
-000226d0: 4461 7461 2e68 6561 6428 3129 0a20 2020  Data.head(1).   
-000226e0: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
-000226f0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-00022700: 6e28 7265 6365 6e74 2920 3d3d 2031 0a20  n(recent) == 1. 
-00022710: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00022720: 6e64 2072 6563 656e 745b 2252 616e 6765  nd recent["Range
-00022730: 225d 2e69 6c6f 635b 305d 203d 3d20 7261  "].iloc[0] == ra
-00022740: 6e67 6544 6174 612e 6465 7363 7269 6265  ngeData.describe
-00022750: 2829 5b22 5261 6e67 6522 5d5b 226d 696e  ()["Range"]["min
-00022760: 225d 0a20 2020 2020 2020 2020 2020 2029  "].            )
-00022770: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00022780: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
-00022790: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000227a0: 6765 7443 616e 646c 6554 7970 6528 7265  getCandleType(re
-000227b0: 6365 6e74 290a 2020 2020 2020 2020 2020  cent).          
-000227c0: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
-000227d0: 775f 6361 6e64 6c65 5b22 436c 6f73 6522  w_candle["Close"
-000227e0: 5d2e 696c 6f63 5b30 5d20 3e3d 2072 6563  ].iloc[0] >= rec
-000227f0: 656e 745b 2243 6c6f 7365 225d 2e69 6c6f  ent["Close"].ilo
-00022800: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
-00022810: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-00022820: 2020 2020 2020 2020 2020 2020 7363 7265              scre
-00022830: 656e 4469 6374 5b22 5061 7474 6572 6e22  enDict["Pattern"
-00022840: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
-00022850: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-00022860: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
-00022870: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
-00022880: 6578 742e 4752 4545 4e20 2b20 6622 4275  ext.GREEN + f"Bu
-00022890: 792d 4e52 7b6e 727d 2220 2b20 636f 6c6f  y-NR{nr}" + colo
-000228a0: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
-000228b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-000228c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000228d0: 2020 2020 7361 7665 4469 6374 5b22 5061      saveDict["Pa
-000228e0: 7474 6572 6e22 5d20 3d20 7361 7665 645b  ttern"] = saved[
-000228f0: 315d 202b 2066 2242 7579 2d4e 527b 6e72  1] + f"Buy-NR{nr
-00022900: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-00022910: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00022920: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-00022930: 2020 2065 6c69 6620 280a 2020 2020 2020     elif (.      
-00022940: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00022950: 7420 7365 6c66 2e67 6574 4361 6e64 6c65  t self.getCandle
-00022960: 5479 7065 2872 6563 656e 7429 0a20 2020  Type(recent).   
-00022970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022980: 2061 6e64 206e 6f77 5f63 616e 646c 655b   and now_candle[
-00022990: 2243 6c6f 7365 225d 2e69 6c6f 635b 305d  "Close"].iloc[0]
-000229a0: 203c 3d20 7265 6365 6e74 5b22 436c 6f73   <= recent["Clos
-000229b0: 6522 5d2e 696c 6f63 5b30 5d0a 2020 2020  e"].iloc[0].    
-000229c0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
-000229d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000229e0: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
-000229f0: 6174 7465 726e 225d 203d 2028 0a20 2020  attern"] = (.   
-00022a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a10: 2020 2020 2073 6176 6564 5b30 5d20 2b20       saved[0] + 
-00022a20: 636f 6c6f 7254 6578 742e 424f 4c44 202b  colorText.BOLD +
-00022a30: 2063 6f6c 6f72 5465 7874 2e46 4149 4c20   colorText.FAIL 
-00022a40: 2b20 6622 5365 6c6c 2d4e 527b 6e72 7d22  + f"Sell-NR{nr}"
-00022a50: 202b 2063 6f6c 6f72 5465 7874 2e45 4e44   + colorText.END
-00022a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022a70: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00022a80: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
-00022a90: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
-00022aa0: 2073 6176 6564 5b31 5d20 2b20 6622 5365   saved[1] + f"Se
-00022ab0: 6c6c 2d4e 527b 6e72 7d22 0a20 2020 2020  ll-NR{nr}".     
-00022ac0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00022ad0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-00022ae0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00022af0: 6c73 650a 2020 2020 2020 2020 656c 7365  lse.        else
-00022b00: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00022b10: 6e67 6544 6174 6120 3d20 6461 7461 2e68  ngeData = data.h
-00022b20: 6561 6428 6e72 290a 2020 2020 2020 2020  ead(nr).        
-00022b30: 2020 2020 7261 6e67 6544 6174 612e 6c6f      rangeData.lo
-00022b40: 635b 3a2c 2752 616e 6765 275d 203d 2061  c[:,'Range'] = a
-00022b50: 6273 2872 616e 6765 4461 7461 5b22 436c  bs(rangeData["Cl
-00022b60: 6f73 6522 5d20 2d20 7261 6e67 6544 6174  ose"] - rangeDat
-00022b70: 615b 224f 7065 6e22 5d29 0a20 2020 2020  a["Open"]).     
-00022b80: 2020 2020 2020 2072 6563 656e 7420 3d20         recent = 
-00022b90: 7261 6e67 6544 6174 612e 6865 6164 2831  rangeData.head(1
-00022ba0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00022bb0: 2072 6563 656e 745b 2252 616e 6765 225d   recent["Range"]
-00022bc0: 2e69 6c6f 635b 305d 203d 3d20 7261 6e67  .iloc[0] == rang
-00022bd0: 6544 6174 612e 6465 7363 7269 6265 2829  eData.describe()
-00022be0: 5b22 5261 6e67 6522 5d5b 226d 696e 225d  ["Range"]["min"]
-00022bf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00022c00: 2020 7363 7265 656e 4469 6374 5b22 5061    screenDict["Pa
-00022c10: 7474 6572 6e22 5d20 3d20 280a 2020 2020  ttern"] = (.    
-00022c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022c30: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
-00022c40: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
-00022c50: 7254 6578 742e 4752 4545 4e20 2b20 6622  rText.GREEN + f"
-00022c60: 4e52 7b6e 727d 2220 2b20 636f 6c6f 7254  NR{nr}" + colorT
-00022c70: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
-00022c80: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00022c90: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-00022ca0: 6374 5b22 5061 7474 6572 6e22 5d20 3d20  ct["Pattern"] = 
-00022cb0: 7361 7665 645b 315d 202b 2066 224e 527b  saved[1] + f"NR{
-00022cc0: 6e72 7d22 0a20 2020 2020 2020 2020 2020  nr}".           
-00022cd0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00022ce0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00022cf0: 7572 6e20 4661 6c73 650a 0a20 2020 2023  urn False..    #
-00022d00: 2046 696e 6420 6966 2073 746f 636b 2069   Find if stock i
-00022d10: 7320 6e65 776c 7920 6c69 7374 6564 0a20  s newly listed. 
-00022d20: 2020 2064 6566 2076 616c 6964 6174 654e     def validateN
-00022d30: 6577 6c79 4c69 7374 6564 2873 656c 662c  ewlyListed(self,
-00022d40: 2064 662c 2064 6179 7354 6f4c 6f6f 6b62   df, daysToLookb
-00022d50: 6163 6b29 3a0a 2020 2020 2020 2020 6966  ack):.        if
-00022d60: 2064 6620 6973 204e 6f6e 6520 6f72 206c   df is None or l
-00022d70: 656e 2864 6629 203d 3d20 303a 0a20 2020  en(df) == 0:.   
-00022d80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00022d90: 4661 6c73 650a 2020 2020 2020 2020 6461  False.        da
-00022da0: 7461 203d 2064 662e 636f 7079 2829 0a20  ta = df.copy(). 
-00022db0: 2020 2020 2020 2064 6179 7354 6f4c 6f6f         daysToLoo
-00022dc0: 6b62 6163 6b20 3d20 696e 7428 6461 7973  kback = int(days
-00022dd0: 546f 4c6f 6f6b 6261 636b 5b3a 2d31 5d29  ToLookback[:-1])
-00022de0: 0a20 2020 2020 2020 2072 6563 656e 7420  .        recent 
-00022df0: 3d20 6461 7461 2e68 6561 6428 3129 0a20  = data.head(1). 
-00022e00: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
-00022e10: 6365 6e74 2920 3c20 313a 0a20 2020 2020  cent) < 1:.     
-00022e20: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00022e30: 6c73 650a 2020 2020 2020 2020 6966 206c  lse.        if l
-00022e40: 656e 2864 6174 6129 203c 2064 6179 7354  en(data) < daysT
-00022e50: 6f4c 6f6f 6b62 6163 6b20 616e 6420 280a  oLookback and (.
-00022e60: 2020 2020 2020 2020 2020 2020 7265 6365              rece
-00022e70: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
-00022e80: 5b30 5d20 213d 206e 702e 6e61 6e20 616e  [0] != np.nan an
-00022e90: 6420 7265 6365 6e74 5b22 436c 6f73 6522  d recent["Close"
-00022ea0: 5d2e 696c 6f63 5b30 5d20 3e20 300a 2020  ].iloc[0] > 0.  
-00022eb0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-00022ec0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00022ed0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00022ee0: 4661 6c73 650a 0a20 2020 2023 2056 616c  False..    # Val
-00022ef0: 6964 6174 6520 6966 2074 6865 2073 746f  idate if the sto
-00022f00: 636b 2070 7269 6365 7320 6172 6520 6174  ck prices are at
-00022f10: 206c 6561 7374 2072 6973 696e 6720 6279   least rising by
-00022f20: 2032 2520 666f 7220 7468 6520 6c61 7374   2% for the last
-00022f30: 2033 2073 6573 7369 6f6e 730a 2020 2020   3 sessions.    
-00022f40: 6465 6620 7661 6c69 6461 7465 5072 6963  def validatePric
-00022f50: 6552 6973 696e 6742 7941 744c 6561 7374  eRisingByAtLeast
-00022f60: 3250 6572 6365 6e74 2873 656c 662c 2064  2Percent(self, d
-00022f70: 662c 2073 6372 6565 6e44 6963 742c 2073  f, screenDict, s
-00022f80: 6176 6544 6963 7429 3a0a 2020 2020 2020  aveDict):.      
-00022f90: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
-00022fa0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
-00022fb0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00022fc0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-00022fd0: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
-00022fe0: 2829 0a20 2020 2020 2020 2064 6174 6120  ().        data 
-00022ff0: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
-00023000: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-00023010: 6461 7461 2e72 6570 6c61 6365 285b 6e70  data.replace([np
-00023020: 2e69 6e66 2c20 2d6e 702e 696e 665d 2c20  .inf, -np.inf], 
-00023030: 3029 0a20 2020 2020 2020 2064 6174 6120  0).        data 
-00023040: 3d20 6461 7461 2e68 6561 6428 3429 0a20  = data.head(4). 
-00023050: 2020 2020 2020 2069 6620 6c65 6e28 6461         if len(da
-00023060: 7461 2920 3c20 343a 0a20 2020 2020 2020  ta) < 4:.       
-00023070: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00023080: 650a 2020 2020 2020 2020 6461 7930 203d  e.        day0 =
-00023090: 2064 6174 612e 696c 6f63 5b30 5d5b 2243   data.iloc[0]["C
-000230a0: 6c6f 7365 225d 2e69 7465 6d28 290a 2020  lose"].item().  
-000230b0: 2020 2020 2020 6461 794d 696e 7573 3120        dayMinus1 
-000230c0: 3d20 6461 7461 2e69 6c6f 635b 315d 5b22  = data.iloc[1]["
-000230d0: 436c 6f73 6522 5d2e 6974 656d 2829 0a20  Close"].item(). 
-000230e0: 2020 2020 2020 2064 6179 4d69 6e75 7332         dayMinus2
-000230f0: 203d 2064 6174 612e 696c 6f63 5b32 5d5b   = data.iloc[2][
-00023100: 2243 6c6f 7365 225d 2e69 7465 6d28 290a  "Close"].item().
-00023110: 2020 2020 2020 2020 6461 794d 696e 7573          dayMinus
-00023120: 3320 3d20 6461 7461 2e69 6c6f 635b 335d  3 = data.iloc[3]
-00023130: 5b22 436c 6f73 6522 5d2e 6974 656d 2829  ["Close"].item()
-00023140: 0a20 2020 2020 2020 2070 6572 6365 6e74  .        percent
-00023150: 3320 3d20 726f 756e 6428 2864 6179 4d69  3 = round((dayMi
-00023160: 6e75 7332 202d 2064 6179 4d69 6e75 7333  nus2 - dayMinus3
-00023170: 2920 2a20 3130 3020 2f20 6461 794d 696e  ) * 100 / dayMin
-00023180: 7573 332c 2032 290a 2020 2020 2020 2020  us3, 2).        
-00023190: 7065 7263 656e 7432 203d 2072 6f75 6e64  percent2 = round
-000231a0: 2828 6461 794d 696e 7573 3120 2d20 6461  ((dayMinus1 - da
-000231b0: 794d 696e 7573 3229 202a 2031 3030 202f  yMinus2) * 100 /
-000231c0: 2064 6179 4d69 6e75 7332 2c20 3229 0a20   dayMinus2, 2). 
-000231d0: 2020 2020 2020 2070 6572 6365 6e74 3120         percent1 
-000231e0: 3d20 726f 756e 6428 2864 6179 3020 2d20  = round((day0 - 
-000231f0: 6461 794d 696e 7573 3129 202a 2031 3030  dayMinus1) * 100
-00023200: 202f 2064 6179 4d69 6e75 7331 2c20 3229   / dayMinus1, 2)
-00023210: 0a0a 2020 2020 2020 2020 6966 2070 6572  ..        if per
-00023220: 6365 6e74 3120 3e3d 2032 2061 6e64 2070  cent1 >= 2 and p
-00023230: 6572 6365 6e74 3220 3e3d 2032 2061 6e64  ercent2 >= 2 and
-00023240: 2070 6572 6365 6e74 3320 3e3d 2032 3a0a   percent3 >= 2:.
-00023250: 2020 2020 2020 2020 2020 2020 7063 745f              pct_
-00023260: 6368 616e 6765 5f74 6578 7420 3d20 280a  change_text = (.
-00023270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023280: 2822 252e 3166 2525 2220 2520 7065 7263  ("%.1f%%" % perc
-00023290: 656e 7431 290a 2020 2020 2020 2020 2020  ent1).          
-000232a0: 2020 2020 2020 2b20 2822 2028 252e 3166        + (" (%.1f
-000232b0: 2525 2c22 2025 2070 6572 6365 6e74 3229  %%," % percent2)
-000232c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000232d0: 202b 2028 2220 252e 3166 2525 2922 2025   + (" %.1f%%)" %
-000232e0: 2070 6572 6365 6e74 3329 0a20 2020 2020   percent3).     
-000232f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00023300: 2020 2020 2073 6176 6544 6963 745b 2225       saveDict["%
-00023310: 4368 6e67 225d 203d 2070 6374 5f63 6861  Chng"] = pct_cha
-00023320: 6e67 655f 7465 7874 0a20 2020 2020 2020  nge_text.       
-00023330: 2020 2020 2073 6372 6565 6e44 6963 745b       screenDict[
-00023340: 2225 4368 6e67 225d 203d 2063 6f6c 6f72  "%Chng"] = color
-00023350: 5465 7874 2e47 5245 454e 202b 2070 6374  Text.GREEN + pct
-00023360: 5f63 6861 6e67 655f 7465 7874 202b 2063  _change_text + c
-00023370: 6f6c 6f72 5465 7874 2e45 4e44 0a20 2020  olorText.END.   
-00023380: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00023390: 5472 7565 2061 6e64 2073 656c 662e 6765  True and self.ge
-000233a0: 7443 616e 646c 6554 7970 6528 6461 7461  tCandleType(data
-000233b0: 2e68 6561 6428 3129 290a 2020 2020 2020  .head(1)).      
-000233c0: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-000233d0: 2020 2020 2340 6d65 6173 7572 655f 7469      #@measure_ti
-000233e0: 6d65 0a20 2020 2023 2076 616c 6964 6174  me.    # validat
-000233f0: 6520 6966 2052 5349 2069 7320 7769 7468  e if RSI is with
-00023400: 696e 2067 6976 656e 2072 616e 6765 0a20  in given range. 
-00023410: 2020 2064 6566 2076 616c 6964 6174 6552     def validateR
-00023420: 5349 2873 656c 662c 2064 662c 2073 6372  SI(self, df, scr
-00023430: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
-00023440: 742c 206d 696e 5253 492c 206d 6178 5253  t, minRSI, maxRS
-00023450: 492c 7273 694b 6579 3d22 5253 4922 293a  I,rsiKey="RSI"):
-00023460: 0a20 2020 2020 2020 2069 6620 6466 2069  .        if df i
-00023470: 7320 4e6f 6e65 206f 7220 6c65 6e28 6466  s None or len(df
-00023480: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
-00023490: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000234a0: 0a20 2020 2020 2020 2069 6620 7273 694b  .        if rsiK
-000234b0: 6579 206e 6f74 2069 6e20 6466 2e63 6f6c  ey not in df.col
-000234c0: 756d 6e73 3a0a 2020 2020 2020 2020 2020  umns:.          
-000234d0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-000234e0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
-000234f0: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
-00023500: 6461 7461 203d 2064 6174 612e 6669 6c6c  data = data.fill
-00023510: 6e61 2830 290a 2020 2020 2020 2020 6461  na(0).        da
-00023520: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
-00023530: 6528 5b6e 702e 696e 662c 202d 6e70 2e69  e([np.inf, -np.i
-00023540: 6e66 5d2c 2030 290a 2020 2020 2020 2020  nf], 0).        
-00023550: 7273 6920 3d20 696e 7428 6461 7461 2e68  rsi = int(data.h
-00023560: 6561 6428 3129 5b72 7369 4b65 795d 2e69  ead(1)[rsiKey].i
-00023570: 6c6f 635b 305d 290a 2020 2020 2020 2020  loc[0]).        
-00023580: 7361 7665 4469 6374 5b72 7369 4b65 795d  saveDict[rsiKey]
-00023590: 203d 2072 7369 0a20 2020 2020 2020 2023   = rsi.        #
-000235a0: 2068 7474 7073 3a2f 2f63 6861 7274 696e   https://chartin
-000235b0: 6b2e 636f 6d2f 7363 7265 656e 6572 2f72  k.com/screener/r
-000235c0: 7369 2d73 6372 6565 6e69 6e67 0a20 2020  si-screening.   
-000235d0: 2020 2020 2069 6620 7273 693e 2030 2061       if rsi> 0 a
-000235e0: 6e64 2072 7369 203e 3d20 6d69 6e52 5349  nd rsi >= minRSI
-000235f0: 2061 6e64 2072 7369 203c 3d20 6d61 7852   and rsi <= maxR
-00023600: 5349 3a20 2023 206f 7220 2872 7369 203c  SI:  # or (rsi <
-00023610: 3d20 3731 2061 6e64 2072 7369 203e 3d20  = 71 and rsi >= 
-00023620: 3637 293a 0a20 2020 2020 2020 2020 2020  67):.           
-00023630: 2073 6372 6565 6e44 6963 745b 7273 694b   screenDict[rsiK
-00023640: 6579 5d20 3d20 280a 2020 2020 2020 2020  ey] = (.        
-00023650: 2020 2020 2020 2020 636f 6c6f 7254 6578          colorTex
-00023660: 742e 424f 4c44 202b 2063 6f6c 6f72 5465  t.BOLD + colorTe
-00023670: 7874 2e47 5245 454e 202b 2073 7472 2872  xt.GREEN + str(r
-00023680: 7369 2920 2b20 636f 6c6f 7254 6578 742e  si) + colorText.
-00023690: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
-000236a0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-000236b0: 7475 726e 2054 7275 6520 6966 2028 7273  turn True if (rs
-000236c0: 694b 6579 203d 3d20 2252 5349 6922 2920  iKey == "RSIi") 
-000236d0: 656c 7365 2028 7365 6c66 2e76 616c 6964  else (self.valid
-000236e0: 6174 6552 5349 2864 662c 2073 6372 6565  ateRSI(df, scree
-000236f0: 6e44 6963 742c 2073 6176 6544 6963 742c  nDict, saveDict,
-00023700: 206d 696e 5253 492c 206d 6178 5253 492c   minRSI, maxRSI,
-00023710: 7273 694b 6579 3d22 5253 4969 2229 206f  rsiKey="RSIi") o
-00023720: 7220 5472 7565 290a 2020 2020 2020 2020  r True).        
-00023730: 7363 7265 656e 4469 6374 5b72 7369 4b65  screenDict[rsiKe
-00023740: 795d 203d 2063 6f6c 6f72 5465 7874 2e42  y] = colorText.B
-00023750: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
-00023760: 4641 494c 202b 2073 7472 2872 7369 2920  FAIL + str(rsi) 
-00023770: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-00023780: 2020 2020 2020 2020 2320 4966 2065 6974          # If eit
-00023790: 6865 7220 6461 696c 7920 6f72 2069 6e74  her daily or int
-000237a0: 7261 6461 7920 5253 4920 636f 6d65 7320  raday RSI comes 
-000237b0: 7769 7468 696e 2072 616e 6765 3f0a 2020  within range?.  
-000237c0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-000237d0: 7365 2069 6620 2872 7369 4b65 7920 3d3d  se if (rsiKey ==
-000237e0: 2022 5253 4969 2229 2065 6c73 6520 2873   "RSIi") else (s
-000237f0: 656c 662e 7661 6c69 6461 7465 5253 4928  elf.validateRSI(
-00023800: 6466 2c20 7363 7265 656e 4469 6374 2c20  df, screenDict, 
-00023810: 7361 7665 4469 6374 2c20 6d69 6e52 5349  saveDict, minRSI
-00023820: 2c20 6d61 7852 5349 2c72 7369 4b65 793d  , maxRSI,rsiKey=
-00023830: 2252 5349 6922 2929 0a0a 2020 2020 2320  "RSIi"))..    # 
-00023840: 5661 6c69 6461 7465 2069 6620 7468 6520  Validate if the 
-00023850: 7374 6f63 6b20 6973 2062 756c 6c69 7368  stock is bullish
-00023860: 2069 6e20 7468 6520 7368 6f72 7420 7465   in the short te
-00023870: 726d 0a20 2020 2064 6566 2076 616c 6964  rm.    def valid
-00023880: 6174 6553 686f 7274 5465 726d 4275 6c6c  ateShortTermBull
-00023890: 6973 6828 7365 6c66 2c20 6466 2c20 7363  ish(self, df, sc
-000238a0: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
-000238b0: 6374 293a 0a20 2020 2020 2020 2069 6620  ct):.        if 
-000238c0: 6466 2069 7320 4e6f 6e65 206f 7220 6c65  df is None or le
-000238d0: 6e28 6466 2920 3d3d 2030 3a0a 2020 2020  n(df) == 0:.    
-000238e0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-000238f0: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
-00023900: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
-00023910: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
-00023920: 6368 6172 7469 6e6b 2e63 6f6d 2f73 6372  chartink.com/scr
-00023930: 6565 6e65 722f 7368 6f72 742d 7465 726d  eener/short-term
-00023940: 2d62 756c 6c69 7368 0a20 2020 2020 2020  -bullish.       
-00023950: 2064 6174 6120 3d20 6461 7461 2e66 696c   data = data.fil
-00023960: 6c6e 6128 3029 0a20 2020 2020 2020 2064  lna(0).        d
-00023970: 6174 6120 3d20 6461 7461 2e72 6570 6c61  ata = data.repla
-00023980: 6365 285b 6e70 2e69 6e66 2c20 2d6e 702e  ce([np.inf, -np.
-00023990: 696e 665d 2c20 3029 0a20 2020 2020 2020  inf], 0).       
-000239a0: 2072 6563 656e 7420 3d20 6461 7461 2e68   recent = data.h
-000239b0: 6561 6428 3129 0a20 2020 2020 2020 2066  ead(1).        f
-000239c0: 6b20 3d20 3020 6966 206c 656e 2864 6174  k = 0 if len(dat
-000239d0: 6129 203c 2033 2065 6c73 6520 6e70 2e72  a) < 3 else np.r
-000239e0: 6f75 6e64 2864 6174 615b 2246 4153 544b  ound(data["FASTK
-000239f0: 225d 2e69 6c6f 635b 325d 2c20 3529 0a20  "].iloc[2], 5). 
-00023a00: 2020 2020 2020 2023 2052 6576 6572 7365         # Reverse
-00023a10: 2074 6865 2064 6174 6166 7261 6d65 2066   the dataframe f
-00023a20: 6f72 2069 6368 696d 6f6b 7520 6361 6c63  or ichimoku calc
-00023a30: 756c 6174 696f 6e73 2077 6974 6820 6461  ulations with da
-00023a40: 7465 2069 6e20 6173 6365 6e64 696e 6720  te in ascending 
-00023a50: 6f72 6465 720a 2020 2020 2020 2020 6466  order.        df
-00023a60: 5f6e 6577 203d 2064 6174 615b 3a3a 2d31  _new = data[::-1
-00023a70: 5d0a 2020 2020 2020 2020 7472 793a 0a20  ].        try:. 
-00023a80: 2020 2020 2020 2020 2020 2064 665f 6963             df_ic
-00023a90: 6869 203d 2064 665f 6e65 772e 7265 6e61  hi = df_new.rena
-00023aa0: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
-00023ab0: 2020 2020 636f 6c75 6d6e 733d 7b0a 2020      columns={.  
-00023ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023ad0: 2020 224f 7065 6e22 3a20 226f 7065 6e22    "Open": "open"
-00023ae0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00023af0: 2020 2020 2020 2248 6967 6822 3a20 2268        "High": "h
-00023b00: 6967 6822 2c0a 2020 2020 2020 2020 2020  igh",.          
-00023b10: 2020 2020 2020 2020 2020 224c 6f77 223a            "Low":
-00023b20: 2022 6c6f 7722 2c0a 2020 2020 2020 2020   "low",.        
-00023b30: 2020 2020 2020 2020 2020 2020 2243 6c6f              "Clo
-00023b40: 7365 223a 2022 636c 6f73 6522 2c0a 2020  se": "close",.  
-00023b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023b60: 2020 2256 6f6c 756d 6522 3a20 2276 6f6c    "Volume": "vol
-00023b70: 756d 6522 2c0a 2020 2020 2020 2020 2020  ume",.          
-00023b80: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00023b90: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00023ba0: 2020 6963 6869 203d 2070 6b74 616c 6962    ichi = pktalib
-00023bb0: 2e69 6368 696d 6f6b 7528 6466 5f69 6368  .ichimoku(df_ich
-00023bc0: 692c 2039 2c20 3236 2c20 3532 2c20 3236  i, 9, 26, 52, 26
-00023bd0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00023be0: 2069 6368 6920 6973 204e 6f6e 653a 0a20   ichi is None:. 
-00023bf0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00023c00: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-00023c10: 2020 2020 2020 2020 6466 5f6e 6577 203d          df_new =
-00023c20: 2070 642e 636f 6e63 6174 285b 6466 5f6e   pd.concat([df_n
-00023c30: 6577 2c20 6963 6869 5d2c 2061 7869 733d  ew, ichi], axis=
-00023c40: 3129 0a20 2020 2020 2020 2020 2020 2023  1).            #
-00023c50: 2052 6576 6572 7365 2061 6761 696e 2074   Reverse again t
-00023c60: 6f20 6765 7420 7468 6520 6d6f 7374 2072  o get the most r
-00023c70: 6563 656e 7420 6461 7465 206f 6e20 746f  ecent date on to
-00023c80: 700a 2020 2020 2020 2020 2020 2020 6466  p.            df
-00023c90: 5f6e 6577 203d 2064 665f 6e65 775b 3a3a  _new = df_new[::
-00023ca0: 2d31 5d0a 2020 2020 2020 2020 2020 2020  -1].            
-00023cb0: 6466 5f6e 6577 203d 2064 665f 6e65 772e  df_new = df_new.
-00023cc0: 6865 6164 2831 290a 2020 2020 2020 2020  head(1).        
-00023cd0: 2020 2020 6466 5f6e 6577 5b22 636c 6f75      df_new["clou
-00023ce0: 645f 6772 6565 6e22 5d20 3d20 6466 5f6e  d_green"] = df_n
-00023cf0: 6577 5b22 4953 415f 3922 5d2e 696c 6f63  ew["ISA_9"].iloc
-00023d00: 5b30 5d20 3e20 6466 5f6e 6577 5b22 4953  [0] > df_new["IS
-00023d10: 425f 3236 225d 2e69 6c6f 635b 305d 0a20  B_26"].iloc[0]. 
-00023d20: 2020 2020 2020 2020 2020 2064 665f 6e65             df_ne
-00023d30: 775b 2263 6c6f 7564 5f72 6564 225d 203d  w["cloud_red"] =
-00023d40: 2064 665f 6e65 775b 2249 5342 5f32 3622   df_new["ISB_26"
-00023d50: 5d2e 696c 6f63 5b30 5d20 3e20 6466 5f6e  ].iloc[0] > df_n
-00023d60: 6577 5b22 4953 415f 3922 5d2e 696c 6f63  ew["ISA_9"].iloc
-00023d70: 5b30 5d0a 2020 2020 2020 2020 6578 6365  [0].        exce
-00023d80: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00023d90: 653a 2020 2320 7072 6167 6d61 3a20 6e6f  e:  # pragma: no
-00023da0: 2063 6f76 6572 0a20 2020 2020 2020 2020   cover.         
-00023db0: 2020 2073 656c 662e 6465 6661 756c 745f     self.default_
-00023dc0: 6c6f 6767 6572 2e64 6562 7567 2865 2c20  logger.debug(e, 
-00023dd0: 6578 635f 696e 666f 3d54 7275 6529 0a20  exc_info=True). 
-00023de0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00023df0: 2020 2020 2020 2020 6162 6f76 6543 6c6f          aboveClo
-00023e00: 7564 546f 7020 3d20 4661 6c73 650a 2020  udTop = False.  
-00023e10: 2020 2020 2020 2320 6261 7365 6c69 6e65        # baseline
-00023e20: 203e 2063 6c6f 7564 2074 6f70 2028 636c   > cloud top (cl
-00023e30: 6f75 6420 6973 2062 6f75 6e64 2062 7920  oud is bound by 
-00023e40: 7370 616e 2061 2061 6e64 2073 7061 6e20  span a and span 
-00023e50: 6229 2061 6e64 2063 6c6f 7365 2069 7320  b) and close is 
-00023e60: 3e20 636c 6f75 6420 746f 700a 2020 2020  > cloud top.    
-00023e70: 2020 2020 6966 2064 665f 6e65 775b 2263      if df_new["c
-00023e80: 6c6f 7564 5f67 7265 656e 225d 2e69 6c6f  loud_green"].ilo
-00023e90: 635b 305d 3a0a 2020 2020 2020 2020 2020  c[0]:.          
-00023ea0: 2020 6162 6f76 6543 6c6f 7564 546f 7020    aboveCloudTop 
-00023eb0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00023ec0: 2020 2020 6466 5f6e 6577 5b22 494b 535f      df_new["IKS_
-00023ed0: 3236 225d 2e69 6c6f 635b 305d 203e 2064  26"].iloc[0] > d
-00023ee0: 665f 6e65 775b 2249 5341 5f39 225d 2e69  f_new["ISA_9"].i
-00023ef0: 6c6f 635b 305d 0a20 2020 2020 2020 2020  loc[0].         
-00023f00: 2020 2020 2020 2061 6e64 2072 6563 656e         and recen
-00023f10: 745b 2243 6c6f 7365 225d 2e69 6c6f 635b  t["Close"].iloc[
-00023f20: 305d 203e 2064 665f 6e65 775b 2249 5341  0] > df_new["ISA
-00023f30: 5f39 225d 2e69 6c6f 635b 305d 0a20 2020  _9"].iloc[0].   
-00023f40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00023f50: 2020 2065 6c69 6620 6466 5f6e 6577 5b22     elif df_new["
-00023f60: 636c 6f75 645f 7265 6422 5d2e 696c 6f63  cloud_red"].iloc
-00023f70: 5b30 5d3a 0a20 2020 2020 2020 2020 2020  [0]:.           
-00023f80: 2061 626f 7665 436c 6f75 6454 6f70 203d   aboveCloudTop =
-00023f90: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00023fa0: 2020 2064 665f 6e65 775b 2249 4b53 5f32     df_new["IKS_2
-00023fb0: 3622 5d2e 696c 6f63 5b30 5d20 3e20 6466  6"].iloc[0] > df
-00023fc0: 5f6e 6577 5b22 4953 425f 3236 225d 2e69  _new["ISB_26"].i
-00023fd0: 6c6f 635b 305d 0a20 2020 2020 2020 2020  loc[0].         
-00023fe0: 2020 2020 2020 2061 6e64 2072 6563 656e         and recen
-00023ff0: 745b 2243 6c6f 7365 225d 2e69 6c6f 635b  t["Close"].iloc[
-00024000: 305d 203e 2064 665f 6e65 775b 2249 5342  0] > df_new["ISB
-00024010: 5f32 3622 5d2e 696c 6f63 5b30 5d0a 2020  _26"].iloc[0].  
-00024020: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00024030: 2020 2020 2023 204c 6174 6573 7420 4963       # Latest Ic
-00024040: 6869 6d6f 6b75 2062 6173 656c 696e 6520  himoku baseline 
-00024050: 6973 203c 206c 6174 6573 7420 4963 6869  is < latest Ichi
-00024060: 6d6f 6b75 2063 6f6e 7665 7273 696f 6e20  moku conversion 
-00024070: 6c69 6e65 0a20 2020 2020 2020 2069 6620  line.        if 
-00024080: 6162 6f76 6543 6c6f 7564 546f 7020 616e  aboveCloudTop an
-00024090: 6420 6466 5f6e 6577 5b22 494b 535f 3236  d df_new["IKS_26
-000240a0: 225d 2e69 6c6f 635b 305d 203c 2064 665f  "].iloc[0] < df_
-000240b0: 6e65 775b 2249 5453 5f39 225d 2e69 6c6f  new["ITS_9"].ilo
-000240c0: 635b 305d 3a0a 2020 2020 2020 2020 2020  c[0]:.          
-000240d0: 2020 2320 5374 6f63 6852 5349 2063 726f    # StochRSI cro
-000240e0: 7373 6564 2032 3020 616e 6420 5253 4920  ssed 20 and RSI 
-000240f0: 3e20 3530 0a20 2020 2020 2020 2020 2020  > 50.           
-00024100: 2069 6620 666b 203e 2032 3020 616e 6420   if fk > 20 and 
-00024110: 7265 6365 6e74 5b22 5253 4922 5d2e 696c  recent["RSI"].il
-00024120: 6f63 5b30 5d20 3e20 3530 3a0a 2020 2020  oc[0] > 50:.    
-00024130: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-00024140: 6e64 6974 696f 6e20 6f66 2063 726f 7373  ndition of cross
-00024150: 696e 6720 7468 6520 5374 6f63 6852 5349  ing the StochRSI
-00024160: 206d 6169 6e20 7369 676e 616c 206c 696e   main signal lin
-00024170: 6520 6672 6f6d 2062 6f74 746f 6d20 746f  e from bottom to
-00024180: 2074 6f70 0a20 2020 2020 2020 2020 2020   top.           
-00024190: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-000241a0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-000241b0: 7461 5b22 4641 5354 4422 5d2e 696c 6f63  ta["FASTD"].iloc
-000241c0: 5b31 3030 5d20 3c20 6461 7461 5b22 4641  [100] < data["FA
-000241d0: 5354 4b22 5d2e 696c 6f63 5b31 3030 5d0a  STK"].iloc[100].
-000241e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000241f0: 2020 2020 616e 6420 6461 7461 5b22 4641      and data["FA
-00024200: 5354 4422 5d2e 696c 6f63 5b31 3031 5d20  STD"].iloc[101] 
-00024210: 3e20 6461 7461 5b22 4641 5354 4b22 5d2e  > data["FASTK"].
-00024220: 696c 6f63 5b31 3031 5d0a 2020 2020 2020  iloc[101].      
-00024230: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00024240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024250: 2023 2063 6c6f 7365 203e 2035 3020 7065   # close > 50 pe
-00024260: 7269 6f64 2053 4d41 2f45 4d41 2061 6e64  riod SMA/EMA and
-00024270: 2032 3030 2070 6572 696f 6420 534d 412f   200 period SMA/
-00024280: 454d 410a 2020 2020 2020 2020 2020 2020  EMA.            
-00024290: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-000242a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000242b0: 2020 2020 2072 6563 656e 745b 2253 534d       recent["SSM
-000242c0: 4122 5d2e 696c 6f63 5b30 5d20 3e20 7265  A"].iloc[0] > re
-000242d0: 6365 6e74 5b22 534d 4122 5d2e 696c 6f63  cent["SMA"].iloc
-000242e0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-000242f0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00024300: 7265 6365 6e74 5b22 436c 6f73 6522 5d2e  recent["Close"].
-00024310: 696c 6f63 5b30 5d20 3e20 7265 6365 6e74  iloc[0] > recent
-00024320: 5b22 5353 4d41 225d 2e69 6c6f 635b 305d  ["SSMA"].iloc[0]
-00024330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00024340: 2020 2020 2020 2020 2061 6e64 2072 6563           and rec
-00024350: 656e 745b 2243 6c6f 7365 225d 2e69 6c6f  ent["Close"].ilo
-00024360: 635b 305d 203e 2072 6563 656e 745b 224c  c[0] > recent["L
-00024370: 4d41 225d 2e69 6c6f 635b 305d 0a20 2020  MA"].iloc[0].   
-00024380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024390: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-000243a0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-000243b0: 6420 3d20 7365 6c66 2e66 696e 6443 7572  d = self.findCur
-000243c0: 7265 6e74 5361 7665 6456 616c 7565 2873  rentSavedValue(s
-000243d0: 6372 6565 6e44 6963 742c 7361 7665 4469  creenDict,saveDi
-000243e0: 6374 2c22 4d41 2d53 6967 6e61 6c22 290a  ct,"MA-Signal").
-000243f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024400: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
-00024410: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-00024420: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00024430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024440: 7361 7665 645b 305d 202b 2063 6f6c 6f72  saved[0] + color
-00024450: 5465 7874 2e42 4f4c 4420 2b20 636f 6c6f  Text.BOLD + colo
-00024460: 7254 6578 742e 4752 4545 4e20 2b20 2242  rText.GREEN + "B
-00024470: 756c 6c69 7368 2220 2b20 636f 6c6f 7254  ullish" + colorT
-00024480: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
-00024490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000244a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000244b0: 2020 2020 2020 2020 2020 7361 7665 4469            saveDi
-000244c0: 6374 5b22 4d41 2d53 6967 6e61 6c22 5d20  ct["MA-Signal"] 
-000244d0: 3d20 7361 7665 645b 315d 202b 2022 4275  = saved[1] + "Bu
-000244e0: 6c6c 6973 6822 0a20 2020 2020 2020 2020  llish".         
-000244f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00024500: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-00024510: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00024520: 2020 2020 0a20 2020 2023 2056 616c 6964      .    # Valid
-00024530: 6174 6520 5643 5020 6173 2070 6572 204d  ate VCP as per M
-00024540: 6172 6b20 4d69 6e65 7276 696e 690a 2020  ark Minervini.  
-00024550: 2020 2320 6874 7470 733a 2f2f 6368 6172    # https://char
-00024560: 7469 6e6b 2e63 6f6d 2f73 6372 6565 6e65  tink.com/screene
-00024570: 722f 766f 6c61 7469 6c69 7479 2d63 6f6d  r/volatility-com
-00024580: 7072 6573 7369 6f6e 0a20 2020 2064 6566  pression.    def
-00024590: 2076 616c 6964 6174 6556 4350 4d61 726b   validateVCPMark
-000245a0: 4d69 6e65 7276 696e 6928 7365 6c66 2c20  Minervini(self, 
-000245b0: 6466 3a70 642e 4461 7461 4672 616d 652c  df:pd.DataFrame,
-000245c0: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
-000245d0: 6544 6963 7429 3a0a 2020 2020 2020 2020  eDict):.        
-000245e0: 6966 2064 6620 6973 204e 6f6e 6520 6f72  if df is None or
-000245f0: 206c 656e 2864 6629 203d 3d20 303a 0a20   len(df) == 0:. 
-00024600: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00024610: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-00024620: 6461 7461 203d 2064 662e 636f 7079 2829  data = df.copy()
-00024630: 0a20 2020 2020 2020 206f 686c 635f 6469  .        ohlc_di
-00024640: 6374 203d 207b 0a20 2020 2020 2020 2020  ct = {.         
-00024650: 2020 2027 4f70 656e 273a 2766 6972 7374     'Open':'first
-00024660: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-00024670: 4869 6768 273a 276d 6178 272c 0a20 2020  High':'max',.   
-00024680: 2020 2020 2020 2020 2027 4c6f 7727 3a27           'Low':'
-00024690: 6d69 6e27 2c0a 2020 2020 2020 2020 2020  min',.          
-000246a0: 2020 2743 6c6f 7365 273a 276c 6173 7427    'Close':'last'
-000246b0: 2c0a 2020 2020 2020 2020 2020 2020 2756  ,.            'V
-000246c0: 6f6c 756d 6527 3a27 7375 6d27 0a20 2020  olume':'sum'.   
-000246d0: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
-000246e0: 2066 696e 616c 5f64 6620 3d20 6466 2e72   final_df = df.r
-000246f0: 6573 616d 706c 6528 2757 2d46 5249 272c  esample('W-FRI',
-00024700: 2063 6c6f 7365 643d 276c 6566 7427 292e   closed='left').
-00024710: 6167 6728 6f68 6c63 5f64 6963 7429 2e73  agg(ohlc_dict).s
-00024720: 6869 6674 2827 3164 2729 0a20 2020 2020  hift('1d').     
-00024730: 2020 2077 6565 6b6c 7944 6174 6120 3d20     weeklyData = 
-00024740: 6461 7461 2e72 6573 616d 706c 6528 2757  data.resample('W
-00024750: 2729 2e61 6767 286f 686c 635f 6469 6374  ').agg(ohlc_dict
-00024760: 290a 2020 2020 2020 2020 7265 7665 7273  ).        revers
-00024770: 6564 4461 7461 203d 2064 6174 615b 3a3a  edData = data[::
-00024780: 2d31 5d20 2023 2052 6576 6572 7365 2074  -1]  # Reverse t
-00024790: 6865 2064 6174 6166 7261 6d65 0a20 2020  he dataframe.   
-000247a0: 2020 2020 2072 6563 656e 745f 636c 6f73       recent_clos
-000247b0: 6520 3d20 6461 7461 5b22 436c 6f73 6522  e = data["Close"
-000247c0: 5d2e 6865 6164 2831 292e 696c 6f63 5b30  ].head(1).iloc[0
-000247d0: 5d0a 2020 2020 2020 2020 775f 656d 615f  ].        w_ema_
-000247e0: 3133 203d 2070 6b74 616c 6962 2e45 4d41  13 = pktalib.EMA
-000247f0: 2877 6565 6b6c 7944 6174 615b 2243 6c6f  (weeklyData["Clo
-00024800: 7365 225d 2c74 696d 6570 6572 696f 643d  se"],timeperiod=
-00024810: 3133 292e 7461 696c 2831 292e 696c 6f63  13).tail(1).iloc
-00024820: 5b30 5d0a 2020 2020 2020 2020 775f 656d  [0].        w_em
-00024830: 615f 3236 203d 2070 6b74 616c 6962 2e45  a_26 = pktalib.E
-00024840: 4d41 2877 6565 6b6c 7944 6174 615b 2243  MA(weeklyData["C
-00024850: 6c6f 7365 225d 2c74 696d 6570 6572 696f  lose"],timeperio
-00024860: 643d 3236 292e 7461 696c 2831 292e 696c  d=26).tail(1).il
-00024870: 6f63 5b30 5d0a 2020 2020 2020 2020 775f  oc[0].        w_
-00024880: 736d 615f 3530 203d 2070 6b74 616c 6962  sma_50 = pktalib
-00024890: 2e53 4d41 2877 6565 6b6c 7944 6174 615b  .SMA(weeklyData[
-000248a0: 2243 6c6f 7365 225d 2c74 696d 6570 6572  "Close"],timeper
-000248b0: 696f 643d 3530 292e 7461 696c 2831 292e  iod=50).tail(1).
-000248c0: 696c 6f63 5b30 5d0a 2020 2020 2020 2020  iloc[0].        
-000248d0: 775f 736d 615f 3430 203d 2070 6b74 616c  w_sma_40 = pktal
-000248e0: 6962 2e53 4d41 2877 6565 6b6c 7944 6174  ib.SMA(weeklyDat
-000248f0: 615b 2243 6c6f 7365 225d 2c74 696d 6570  a["Close"],timep
-00024900: 6572 696f 643d 3430 292e 7461 696c 2831  eriod=40).tail(1
-00024910: 292e 696c 6f63 5b30 5d0a 2020 2020 2020  ).iloc[0].      
-00024920: 2020 775f 736d 615f 3430 5f35 775f 6167    w_sma_40_5w_ag
-00024930: 6f20 3d20 706b 7461 6c69 622e 534d 4128  o = pktalib.SMA(
-00024940: 7765 656b 6c79 4461 7461 2e68 6561 6428  weeklyData.head(
-00024950: 6c65 6e28 7765 656b 6c79 4461 7461 292d  len(weeklyData)-
-00024960: 3529 5b22 436c 6f73 6522 5d2c 7469 6d65  5)["Close"],time
-00024970: 7065 7269 6f64 3d34 3029 2e74 6169 6c28  period=40).tail(
-00024980: 3129 2e69 6c6f 635b 305d 0a20 2020 2020  1).iloc[0].     
-00024990: 2020 2077 5f6d 696e 5f35 3020 3d20 6d69     w_min_50 = mi
-000249a0: 6e28 312e 332a 7765 656b 6c79 4461 7461  n(1.3*weeklyData
-000249b0: 2e74 6169 6c28 3530 295b 224c 6f77 225d  .tail(50)["Low"]
-000249c0: 290a 2020 2020 2020 2020 775f 6d61 785f  ).        w_max_
-000249d0: 3530 203d 206d 6178 2830 2e37 352a 7765  50 = max(0.75*we
-000249e0: 656b 6c79 4461 7461 2e74 6169 6c28 3530  eklyData.tail(50
-000249f0: 295b 2248 6967 6822 5d29 0a20 2020 2020  )["High"]).     
-00024a00: 2020 2077 5f65 6d61 5f32 365f 3230 775f     w_ema_26_20w_
-00024a10: 6167 6f20 3d20 706b 7461 6c69 622e 454d  ago = pktalib.EM
-00024a20: 4128 7765 656b 6c79 4461 7461 2e68 6561  A(weeklyData.hea
-00024a30: 6428 6c65 6e28 7765 656b 6c79 4461 7461  d(len(weeklyData
-00024a40: 292d 3230 295b 2243 6c6f 7365 225d 2c74  )-20)["Close"],t
-00024a50: 696d 6570 6572 696f 643d 3236 292e 7461  imeperiod=26).ta
-00024a60: 696c 2831 292e 696c 6f63 5b30 5d0a 2020  il(1).iloc[0].  
-00024a70: 2020 2020 2020 7265 6365 6e74 5f65 6d61        recent_ema
-00024a80: 5f31 335f 3230 645f 6167 6f20 3d20 706b  _13_20d_ago = pk
-00024a90: 7461 6c69 622e 454d 4128 7265 7665 7273  talib.EMA(revers
-00024aa0: 6564 4461 7461 2e68 6561 6428 6c65 6e28  edData.head(len(
-00024ab0: 7265 7665 7273 6564 4461 7461 292d 3230  reversedData)-20
-00024ac0: 295b 2243 6c6f 7365 225d 2c74 696d 6570  )["Close"],timep
-00024ad0: 6572 696f 643d 3133 292e 7461 696c 2831  eriod=13).tail(1
-00024ae0: 292e 696c 6f63 5b30 5d0a 2020 2020 2020  ).iloc[0].      
-00024af0: 2020 775f 736d 615f 3430 5f35 775f 6167    w_sma_40_5w_ag
-00024b00: 6f20 3d20 706b 7461 6c69 622e 534d 4128  o = pktalib.SMA(
-00024b10: 7765 656b 6c79 4461 7461 2e68 6561 6428  weeklyData.head(
-00024b20: 6c65 6e28 7765 656b 6c79 4461 7461 292d  len(weeklyData)-
-00024b30: 3529 5b22 436c 6f73 6522 5d2c 7469 6d65  5)["Close"],time
-00024b40: 7065 7269 6f64 3d34 3029 2e74 6169 6c28  period=40).tail(
-00024b50: 3129 2e69 6c6f 635b 305d 0a20 2020 2020  1).iloc[0].     
-00024b60: 2020 2077 5f73 6d61 5f34 305f 3130 775f     w_sma_40_10w_
-00024b70: 6167 6f20 3d20 706b 7461 6c69 622e 534d  ago = pktalib.SM
-00024b80: 4128 7765 656b 6c79 4461 7461 2e68 6561  A(weeklyData.hea
-00024b90: 6428 6c65 6e28 7765 656b 6c79 4461 7461  d(len(weeklyData
-00024ba0: 292d 3130 295b 2243 6c6f 7365 225d 2c74  )-10)["Close"],t
-00024bb0: 696d 6570 6572 696f 643d 3430 292e 7461  imeperiod=40).ta
-00024bc0: 696c 2831 292e 696c 6f63 5b30 5d0a 2020  il(1).iloc[0].  
-00024bd0: 2020 2020 2020 7265 6365 6e74 5f73 6d61        recent_sma
-00024be0: 5f35 3020 3d20 706b 7461 6c69 622e 534d  _50 = pktalib.SM
-00024bf0: 4128 7265 7665 7273 6564 4461 7461 5b22  A(reversedData["
-00024c00: 436c 6f73 6522 5d2c 7469 6d65 7065 7269  Close"],timeperi
-00024c10: 6f64 3d35 3029 2e74 6169 6c28 3129 2e69  od=50).tail(1).i
-00024c20: 6c6f 635b 305d 0a20 2020 2020 2020 2077  loc[0].        w
-00024c30: 5f77 6d61 5f38 203d 2070 6b74 616c 6962  _wma_8 = pktalib
-00024c40: 2e57 4d41 2877 6565 6b6c 7944 6174 615b  .WMA(weeklyData[
-00024c50: 2243 6c6f 7365 225d 2c74 696d 6570 6572  "Close"],timeper
-00024c60: 696f 643d 3829 2e74 6169 6c28 3129 2e69  iod=8).tail(1).i
-00024c70: 6c6f 635b 305d 0a20 2020 2020 2020 2077  loc[0].        w
-00024c80: 5f73 6d61 5f38 203d 2070 6b74 616c 6962  _sma_8 = pktalib
-00024c90: 2e53 4d41 2877 6565 6b6c 7944 6174 615b  .SMA(weeklyData[
-00024ca0: 2243 6c6f 7365 225d 2c74 696d 6570 6572  "Close"],timeper
-00024cb0: 696f 643d 3829 2e74 6169 6c28 3129 2e69  iod=8).tail(1).i
-00024cc0: 6c6f 635b 305d 0a20 2020 2020 2020 200a  loc[0].        .
-00024cd0: 2020 2020 2020 2020 6973 5643 5020 3d20          isVCP = 
-00024ce0: 775f 656d 615f 3133 203e 2077 5f65 6d61  w_ema_13 > w_ema
-00024cf0: 5f32 3620 616e 6420 5c0a 2020 2020 2020  _26 and \.      
-00024d00: 2020 2020 2020 2020 2020 775f 656d 615f            w_ema_
-00024d10: 3236 203e 2077 5f73 6d61 5f35 3020 616e  26 > w_sma_50 an
-00024d20: 6420 5c0a 2020 2020 2020 2020 2020 2020  d \.            
-00024d30: 2020 2020 775f 736d 615f 3430 203e 2077      w_sma_40 > w
-00024d40: 5f73 6d61 5f34 305f 3577 5f61 676f 2061  _sma_40_5w_ago a
-00024d50: 6e64 205c 0a20 2020 2020 2020 2020 2020  nd \.           
-00024d60: 2020 2020 2072 6563 656e 745f 636c 6f73       recent_clos
-00024d70: 6520 3e3d 2077 5f6d 696e 5f35 3020 616e  e >= w_min_50 an
+00022310: 6966 206f 7065 6e20 3e20 736d 6120 616e  if open > sma an
+00022320: 6420 636c 6f73 6520 3c20 736d 6120 616e  d close < sma an
+00022330: 6420 7374 7228 6d61 4c65 6e67 7468 2920  d str(maLength) 
+00022340: 696e 205b 2230 222c 2234 225d 3a0a 2020  in ["0","4"]:.  
+00022350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022360: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+00022370: 5b22 4d41 2d53 6967 6e61 6c22 5d20 3d20  ["MA-Signal"] = 
+00022380: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00022390: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+000223a0: 7665 645b 305d 202b 2063 6f6c 6f72 5465  ved[0] + colorTe
+000223b0: 7874 2e42 4f4c 4420 2b20 636f 6c6f 7254  xt.BOLD + colorT
+000223c0: 6578 742e 4641 494c 202b 2066 2242 6561  ext.FAIL + f"Bea
+000223d0: 7243 726f 7373 2d7b 6d61 5465 7874 735b  rCross-{maTexts[
+000223e0: 696e 6465 785d 7d22 202b 2063 6f6c 6f72  index]}" + color
+000223f0: 5465 7874 2e45 4e44 0a20 2020 2020 2020  Text.END.       
+00022400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022410: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00022420: 2020 2020 2020 2020 2020 2073 6176 6544             saveD
+00022430: 6963 745b 224d 412d 5369 676e 616c 225d  ict["MA-Signal"]
+00022440: 203d 2073 6176 6564 5b31 5d20 2b20 6622   = saved[1] + f"
+00022450: 4265 6172 4372 6f73 732d 7b6d 6154 6578  BearCross-{maTex
+00022460: 7473 5b69 6e64 6578 5d7d 220a 2020 2020  ts[index]}".    
+00022470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022480: 2020 2020 6d61 5265 7665 7273 616c 203d      maReversal =
+00022490: 202d 310a 2020 2020 2020 2020 2020 2020   -1.            
+000224a0: 2020 2020 2020 2020 2020 2020 6d61 5369              maSi
+000224b0: 676e 616c 732e 6170 7065 6e64 2822 3422  gnals.append("4"
+000224c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000224d0: 2020 696e 6465 7820 2b3d 2031 0a20 2020    index += 1.   
+000224e0: 2020 2020 2072 6574 7572 6e56 616c 7565       returnValue
+000224f0: 203d 206d 6152 6576 6572 7361 6c0a 2020   = maReversal.  
+00022500: 2020 2020 2020 6966 206d 614c 656e 6774        if maLengt
+00022510: 6820 213d 2030 3a0a 2020 2020 2020 2020  h != 0:.        
+00022520: 2020 2020 7265 7475 726e 5661 6c75 6520      returnValue 
+00022530: 3d20 7374 7228 6d61 4c65 6e67 7468 2920  = str(maLength) 
+00022540: 696e 206d 6153 6967 6e61 6c73 0a20 2020  in maSignals.   
+00022550: 2020 2020 2072 6574 7572 6e20 7265 7475       return retu
+00022560: 726e 5661 6c75 650a 0a20 2020 2023 2046  rnValue..    # F
+00022570: 696e 6420 4e52 7820 7261 6e67 6520 666f  ind NRx range fo
+00022580: 7220 5265 7665 7273 616c 0a20 2020 2064  r Reversal.    d
+00022590: 6566 2076 616c 6964 6174 654e 6172 726f  ef validateNarro
+000225a0: 7752 616e 6765 2873 656c 662c 2064 662c  wRange(self, df,
+000225b0: 2073 6372 6565 6e44 6963 742c 2073 6176   screenDict, sav
+000225c0: 6544 6963 742c 206e 723d 3429 3a0a 2020  eDict, nr=4):.  
+000225d0: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
+000225e0: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
+000225f0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00022600: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+00022610: 2020 2020 2020 6461 7461 203d 2064 662e        data = df.
+00022620: 636f 7079 2829 0a20 2020 2020 2020 2073  copy().        s
+00022630: 6176 6564 203d 2073 656c 662e 6669 6e64  aved = self.find
+00022640: 4375 7272 656e 7453 6176 6564 5661 6c75  CurrentSavedValu
+00022650: 6528 7363 7265 656e 4469 6374 2c20 7361  e(screenDict, sa
+00022660: 7665 4469 6374 2c20 2250 6174 7465 726e  veDict, "Pattern
+00022670: 2229 0a20 2020 2020 2020 2069 6620 504b  ").        if PK
+00022680: 4461 7465 5574 696c 6974 6965 732e 6973  DateUtilities.is
+00022690: 5472 6164 696e 6754 696d 6528 293a 0a20  TradingTime():. 
+000226a0: 2020 2020 2020 2020 2020 2072 616e 6765             range
+000226b0: 4461 7461 203d 2064 6174 612e 6865 6164  Data = data.head
+000226c0: 286e 7220 2b20 3129 5b31 3a5d 0a20 2020  (nr + 1)[1:].   
+000226d0: 2020 2020 2020 2020 206e 6f77 5f63 616e           now_can
+000226e0: 646c 6520 3d20 6461 7461 2e68 6561 6428  dle = data.head(
+000226f0: 3129 0a20 2020 2020 2020 2020 2020 2072  1).            r
+00022700: 616e 6765 4461 7461 5b22 5261 6e67 6522  angeData["Range"
+00022710: 5d20 3d20 6162 7328 7261 6e67 6544 6174  ] = abs(rangeDat
+00022720: 615b 2243 6c6f 7365 225d 202d 2072 616e  a["Close"] - ran
+00022730: 6765 4461 7461 5b22 4f70 656e 225d 290a  geData["Open"]).
+00022740: 2020 2020 2020 2020 2020 2020 7265 6365              rece
+00022750: 6e74 203d 2072 616e 6765 4461 7461 2e68  nt = rangeData.h
+00022760: 6561 6428 3129 0a20 2020 2020 2020 2020  ead(1).         
+00022770: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+00022780: 2020 2020 2020 2020 6c65 6e28 7265 6365          len(rece
+00022790: 6e74 2920 3d3d 2031 0a20 2020 2020 2020  nt) == 1.       
+000227a0: 2020 2020 2020 2020 2061 6e64 2072 6563           and rec
+000227b0: 656e 745b 2252 616e 6765 225d 2e69 6c6f  ent["Range"].ilo
+000227c0: 635b 305d 203d 3d20 7261 6e67 6544 6174  c[0] == rangeDat
+000227d0: 612e 6465 7363 7269 6265 2829 5b22 5261  a.describe()["Ra
+000227e0: 6e67 6522 5d5b 226d 696e 225d 0a20 2020  nge"]["min"].   
+000227f0: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+00022800: 2020 2020 2020 2020 2020 2020 6966 2028              if (
+00022810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022820: 2020 2020 2073 656c 662e 6765 7443 616e       self.getCan
+00022830: 646c 6554 7970 6528 7265 6365 6e74 290a  dleType(recent).
+00022840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022850: 2020 2020 616e 6420 6e6f 775f 6361 6e64      and now_cand
+00022860: 6c65 5b22 436c 6f73 6522 5d2e 696c 6f63  le["Close"].iloc
+00022870: 5b30 5d20 3e3d 2072 6563 656e 745b 2243  [0] >= recent["C
+00022880: 6c6f 7365 225d 2e69 6c6f 635b 305d 0a20  lose"].iloc[0]. 
+00022890: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000228a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000228b0: 2020 2020 2020 7363 7265 656e 4469 6374        screenDict
+000228c0: 5b22 5061 7474 6572 6e22 5d20 3d20 280a  ["Pattern"] = (.
+000228d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000228e0: 2020 2020 2020 2020 7361 7665 645b 305d          saved[0]
+000228f0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00022900: 4420 2b20 636f 6c6f 7254 6578 742e 4752  D + colorText.GR
+00022910: 4545 4e20 2b20 6622 4275 792d 4e52 7b6e  EEN + f"Buy-NR{n
+00022920: 727d 2220 2b20 636f 6c6f 7254 6578 742e  r}" + colorText.
+00022930: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
+00022940: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00022950: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+00022960: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
+00022970: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
+00022980: 2242 7579 2d4e 527b 6e72 7d22 0a20 2020  "Buy-NR{nr}".   
+00022990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229a0: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+000229b0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+000229c0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+000229d0: 2020 2020 2020 2020 6e6f 7420 7365 6c66          not self
+000229e0: 2e67 6574 4361 6e64 6c65 5479 7065 2872  .getCandleType(r
+000229f0: 6563 656e 7429 0a20 2020 2020 2020 2020  ecent).         
+00022a00: 2020 2020 2020 2020 2020 2061 6e64 206e             and n
+00022a10: 6f77 5f63 616e 646c 655b 2243 6c6f 7365  ow_candle["Close
+00022a20: 225d 2e69 6c6f 635b 305d 203c 3d20 7265  "].iloc[0] <= re
+00022a30: 6365 6e74 5b22 436c 6f73 6522 5d2e 696c  cent["Close"].il
+00022a40: 6f63 5b30 5d0a 2020 2020 2020 2020 2020  oc[0].          
+00022a50: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+00022a60: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+00022a70: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
+00022a80: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
+00022a90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00022aa0: 6176 6564 5b30 5d20 2b20 636f 6c6f 7254  aved[0] + colorT
+00022ab0: 6578 742e 424f 4c44 202b 2063 6f6c 6f72  ext.BOLD + color
+00022ac0: 5465 7874 2e46 4149 4c20 2b20 6622 5365  Text.FAIL + f"Se
+00022ad0: 6c6c 2d4e 527b 6e72 7d22 202b 2063 6f6c  ll-NR{nr}" + col
+00022ae0: 6f72 5465 7874 2e45 4e44 0a20 2020 2020  orText.END.     
+00022af0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00022b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022b10: 2020 2020 2073 6176 6544 6963 745b 2250       saveDict["P
+00022b20: 6174 7465 726e 225d 203d 2073 6176 6564  attern"] = saved
+00022b30: 5b31 5d20 2b20 6622 5365 6c6c 2d4e 527b  [1] + f"Sell-NR{
+00022b40: 6e72 7d22 0a20 2020 2020 2020 2020 2020  nr}".           
+00022b50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00022b60: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+00022b70: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+00022b80: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00022b90: 2020 2020 2020 2020 7261 6e67 6544 6174          rangeDat
+00022ba0: 6120 3d20 6461 7461 2e68 6561 6428 6e72  a = data.head(nr
+00022bb0: 290a 2020 2020 2020 2020 2020 2020 7261  ).            ra
+00022bc0: 6e67 6544 6174 612e 6c6f 635b 3a2c 2752  ngeData.loc[:,'R
+00022bd0: 616e 6765 275d 203d 2061 6273 2872 616e  ange'] = abs(ran
+00022be0: 6765 4461 7461 5b22 436c 6f73 6522 5d20  geData["Close"] 
+00022bf0: 2d20 7261 6e67 6544 6174 615b 224f 7065  - rangeData["Ope
+00022c00: 6e22 5d29 0a20 2020 2020 2020 2020 2020  n"]).           
+00022c10: 2072 6563 656e 7420 3d20 7261 6e67 6544   recent = rangeD
+00022c20: 6174 612e 6865 6164 2831 290a 2020 2020  ata.head(1).    
+00022c30: 2020 2020 2020 2020 6966 2072 6563 656e          if recen
+00022c40: 745b 2252 616e 6765 225d 2e69 6c6f 635b  t["Range"].iloc[
+00022c50: 305d 203d 3d20 7261 6e67 6544 6174 612e  0] == rangeData.
+00022c60: 6465 7363 7269 6265 2829 5b22 5261 6e67  describe()["Rang
+00022c70: 6522 5d5b 226d 696e 225d 3a0a 2020 2020  e"]["min"]:.    
+00022c80: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+00022c90: 656e 4469 6374 5b22 5061 7474 6572 6e22  enDict["Pattern"
+00022ca0: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
+00022cb0: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+00022cc0: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
+00022cd0: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
+00022ce0: 4752 4545 4e20 2b20 6622 4e52 7b6e 727d  GREEN + f"NR{nr}
+00022cf0: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
+00022d00: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+00022d10: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00022d20: 2020 2020 7361 7665 4469 6374 5b22 5061      saveDict["Pa
+00022d30: 7474 6572 6e22 5d20 3d20 7361 7665 645b  ttern"] = saved[
+00022d40: 315d 202b 2066 224e 527b 6e72 7d22 0a20  1] + f"NR{nr}". 
+00022d50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00022d60: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00022d70: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00022d80: 6c73 650a 0a20 2020 2023 2046 696e 6420  lse..    # Find 
+00022d90: 6966 2073 746f 636b 2069 7320 6e65 776c  if stock is newl
+00022da0: 7920 6c69 7374 6564 0a20 2020 2064 6566  y listed.    def
+00022db0: 2076 616c 6964 6174 654e 6577 6c79 4c69   validateNewlyLi
+00022dc0: 7374 6564 2873 656c 662c 2064 662c 2064  sted(self, df, d
+00022dd0: 6179 7354 6f4c 6f6f 6b62 6163 6b29 3a0a  aysToLookback):.
+00022de0: 2020 2020 2020 2020 6966 2064 6620 6973          if df is
+00022df0: 204e 6f6e 6520 6f72 206c 656e 2864 6629   None or len(df)
+00022e00: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+00022e10: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00022e20: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+00022e30: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
+00022e40: 2064 6179 7354 6f4c 6f6f 6b62 6163 6b20   daysToLookback 
+00022e50: 3d20 696e 7428 6461 7973 546f 4c6f 6f6b  = int(daysToLook
+00022e60: 6261 636b 5b3a 2d31 5d29 0a20 2020 2020  back[:-1]).     
+00022e70: 2020 2072 6563 656e 7420 3d20 6461 7461     recent = data
+00022e80: 2e68 6561 6428 3129 0a20 2020 2020 2020  .head(1).       
+00022e90: 2069 6620 6c65 6e28 7265 6365 6e74 2920   if len(recent) 
+00022ea0: 3c20 313a 0a20 2020 2020 2020 2020 2020  < 1:.           
+00022eb0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+00022ec0: 2020 2020 2020 6966 206c 656e 2864 6174        if len(dat
+00022ed0: 6129 203c 2064 6179 7354 6f4c 6f6f 6b62  a) < daysToLookb
+00022ee0: 6163 6b20 616e 6420 280a 2020 2020 2020  ack and (.      
+00022ef0: 2020 2020 2020 7265 6365 6e74 5b22 436c        recent["Cl
+00022f00: 6f73 6522 5d2e 696c 6f63 5b30 5d20 213d  ose"].iloc[0] !=
+00022f10: 206e 702e 6e61 6e20 616e 6420 7265 6365   np.nan and rece
+00022f20: 6e74 5b22 436c 6f73 6522 5d2e 696c 6f63  nt["Close"].iloc
+00022f30: 5b30 5d20 3e20 300a 2020 2020 2020 2020  [0] > 0.        
+00022f40: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00022f50: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00022f60: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
+00022f70: 0a20 2020 2023 2056 616c 6964 6174 6520  .    # Validate 
+00022f80: 6966 2074 6865 2073 746f 636b 2070 7269  if the stock pri
+00022f90: 6365 7320 6172 6520 6174 206c 6561 7374  ces are at least
+00022fa0: 2072 6973 696e 6720 6279 2032 2520 666f   rising by 2% fo
+00022fb0: 7220 7468 6520 6c61 7374 2033 2073 6573  r the last 3 ses
+00022fc0: 7369 6f6e 730a 2020 2020 6465 6620 7661  sions.    def va
+00022fd0: 6c69 6461 7465 5072 6963 6552 6973 696e  lidatePriceRisin
+00022fe0: 6742 7941 744c 6561 7374 3250 6572 6365  gByAtLeast2Perce
+00022ff0: 6e74 2873 656c 662c 2064 662c 2073 6372  nt(self, df, scr
+00023000: 6565 6e44 6963 742c 2073 6176 6544 6963  eenDict, saveDic
+00023010: 7429 3a0a 2020 2020 2020 2020 6966 2064  t):.        if d
+00023020: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+00023030: 2864 6629 203d 3d20 303a 0a20 2020 2020  (df) == 0:.     
+00023040: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00023050: 6c73 650a 2020 2020 2020 2020 6461 7461  lse.        data
+00023060: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
+00023070: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+00023080: 2e66 696c 6c6e 6128 3029 0a20 2020 2020  .fillna(0).     
+00023090: 2020 2064 6174 6120 3d20 6461 7461 2e72     data = data.r
+000230a0: 6570 6c61 6365 285b 6e70 2e69 6e66 2c20  eplace([np.inf, 
+000230b0: 2d6e 702e 696e 665d 2c20 3029 0a20 2020  -np.inf], 0).   
+000230c0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+000230d0: 2e68 6561 6428 3429 0a20 2020 2020 2020  .head(4).       
+000230e0: 2069 6620 6c65 6e28 6461 7461 2920 3c20   if len(data) < 
+000230f0: 343a 0a20 2020 2020 2020 2020 2020 2072  4:.            r
+00023100: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+00023110: 2020 2020 6461 7930 203d 2064 6174 612e      day0 = data.
+00023120: 696c 6f63 5b30 5d5b 2243 6c6f 7365 225d  iloc[0]["Close"]
+00023130: 2e69 7465 6d28 290a 2020 2020 2020 2020  .item().        
+00023140: 6461 794d 696e 7573 3120 3d20 6461 7461  dayMinus1 = data
+00023150: 2e69 6c6f 635b 315d 5b22 436c 6f73 6522  .iloc[1]["Close"
+00023160: 5d2e 6974 656d 2829 0a20 2020 2020 2020  ].item().       
+00023170: 2064 6179 4d69 6e75 7332 203d 2064 6174   dayMinus2 = dat
+00023180: 612e 696c 6f63 5b32 5d5b 2243 6c6f 7365  a.iloc[2]["Close
+00023190: 225d 2e69 7465 6d28 290a 2020 2020 2020  "].item().      
+000231a0: 2020 6461 794d 696e 7573 3320 3d20 6461    dayMinus3 = da
+000231b0: 7461 2e69 6c6f 635b 335d 5b22 436c 6f73  ta.iloc[3]["Clos
+000231c0: 6522 5d2e 6974 656d 2829 0a20 2020 2020  e"].item().     
+000231d0: 2020 2070 6572 6365 6e74 3320 3d20 726f     percent3 = ro
+000231e0: 756e 6428 2864 6179 4d69 6e75 7332 202d  und((dayMinus2 -
+000231f0: 2064 6179 4d69 6e75 7333 2920 2a20 3130   dayMinus3) * 10
+00023200: 3020 2f20 6461 794d 696e 7573 332c 2032  0 / dayMinus3, 2
+00023210: 290a 2020 2020 2020 2020 7065 7263 656e  ).        percen
+00023220: 7432 203d 2072 6f75 6e64 2828 6461 794d  t2 = round((dayM
+00023230: 696e 7573 3120 2d20 6461 794d 696e 7573  inus1 - dayMinus
+00023240: 3229 202a 2031 3030 202f 2064 6179 4d69  2) * 100 / dayMi
+00023250: 6e75 7332 2c20 3229 0a20 2020 2020 2020  nus2, 2).       
+00023260: 2070 6572 6365 6e74 3120 3d20 726f 756e   percent1 = roun
+00023270: 6428 2864 6179 3020 2d20 6461 794d 696e  d((day0 - dayMin
+00023280: 7573 3129 202a 2031 3030 202f 2064 6179  us1) * 100 / day
+00023290: 4d69 6e75 7331 2c20 3229 0a0a 2020 2020  Minus1, 2)..    
+000232a0: 2020 2020 6966 2070 6572 6365 6e74 3120      if percent1 
+000232b0: 3e3d 2032 2061 6e64 2070 6572 6365 6e74  >= 2 and percent
+000232c0: 3220 3e3d 2032 2061 6e64 2070 6572 6365  2 >= 2 and perce
+000232d0: 6e74 3320 3e3d 2032 3a0a 2020 2020 2020  nt3 >= 2:.      
+000232e0: 2020 2020 2020 7063 745f 6368 616e 6765        pct_change
+000232f0: 5f74 6578 7420 3d20 280a 2020 2020 2020  _text = (.      
+00023300: 2020 2020 2020 2020 2020 2822 252e 3166            ("%.1f
+00023310: 2525 2220 2520 7065 7263 656e 7431 290a  %%" % percent1).
+00023320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023330: 2b20 2822 2028 252e 3166 2525 2c22 2025  + (" (%.1f%%," %
+00023340: 2070 6572 6365 6e74 3229 0a20 2020 2020   percent2).     
+00023350: 2020 2020 2020 2020 2020 202b 2028 2220             + (" 
+00023360: 252e 3166 2525 2922 2025 2070 6572 6365  %.1f%%)" % perce
+00023370: 6e74 3329 0a20 2020 2020 2020 2020 2020  nt3).           
+00023380: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
+00023390: 6176 6544 6963 745b 2225 4368 6e67 225d  aveDict["%Chng"]
+000233a0: 203d 2070 6374 5f63 6861 6e67 655f 7465   = pct_change_te
+000233b0: 7874 0a20 2020 2020 2020 2020 2020 2073  xt.            s
+000233c0: 6372 6565 6e44 6963 745b 2225 4368 6e67  creenDict["%Chng
+000233d0: 225d 203d 2063 6f6c 6f72 5465 7874 2e47  "] = colorText.G
+000233e0: 5245 454e 202b 2070 6374 5f63 6861 6e67  REEN + pct_chang
+000233f0: 655f 7465 7874 202b 2063 6f6c 6f72 5465  e_text + colorTe
+00023400: 7874 2e45 4e44 0a20 2020 2020 2020 2020  xt.END.         
+00023410: 2020 2072 6574 7572 6e20 5472 7565 2061     return True a
+00023420: 6e64 2073 656c 662e 6765 7443 616e 646c  nd self.getCandl
+00023430: 6554 7970 6528 6461 7461 2e68 6561 6428  eType(data.head(
+00023440: 3129 290a 2020 2020 2020 2020 7265 7475  1)).        retu
+00023450: 726e 2046 616c 7365 0a0a 2020 2020 2340  rn False..    #@
+00023460: 6d65 6173 7572 655f 7469 6d65 0a20 2020  measure_time.   
+00023470: 2023 2076 616c 6964 6174 6520 6966 2052   # validate if R
+00023480: 5349 2069 7320 7769 7468 696e 2067 6976  SI is within giv
+00023490: 656e 2072 616e 6765 0a20 2020 2064 6566  en range.    def
+000234a0: 2076 616c 6964 6174 6552 5349 2873 656c   validateRSI(sel
+000234b0: 662c 2064 662c 2073 6372 6565 6e44 6963  f, df, screenDic
+000234c0: 742c 2073 6176 6544 6963 742c 206d 696e  t, saveDict, min
+000234d0: 5253 492c 206d 6178 5253 492c 7273 694b  RSI, maxRSI,rsiK
+000234e0: 6579 3d22 5253 4922 293a 0a20 2020 2020  ey="RSI"):.     
+000234f0: 2020 2069 6620 6466 2069 7320 4e6f 6e65     if df is None
+00023500: 206f 7220 6c65 6e28 6466 2920 3d3d 2030   or len(df) == 0
+00023510: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00023520: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+00023530: 2020 2069 6620 7273 694b 6579 206e 6f74     if rsiKey not
+00023540: 2069 6e20 6466 2e63 6f6c 756d 6e73 3a0a   in df.columns:.
+00023550: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00023560: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+00023570: 2064 6174 6120 3d20 6466 2e63 6f70 7928   data = df.copy(
+00023580: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
+00023590: 2064 6174 612e 6669 6c6c 6e61 2830 290a   data.fillna(0).
+000235a0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+000235b0: 6174 612e 7265 706c 6163 6528 5b6e 702e  ata.replace([np.
+000235c0: 696e 662c 202d 6e70 2e69 6e66 5d2c 2030  inf, -np.inf], 0
+000235d0: 290a 2020 2020 2020 2020 7273 6920 3d20  ).        rsi = 
+000235e0: 696e 7428 6461 7461 2e68 6561 6428 3129  int(data.head(1)
+000235f0: 5b72 7369 4b65 795d 2e69 6c6f 635b 305d  [rsiKey].iloc[0]
+00023600: 290a 2020 2020 2020 2020 7361 7665 4469  ).        saveDi
+00023610: 6374 5b72 7369 4b65 795d 203d 2072 7369  ct[rsiKey] = rsi
+00023620: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
+00023630: 3a2f 2f63 6861 7274 696e 6b2e 636f 6d2f  ://chartink.com/
+00023640: 7363 7265 656e 6572 2f72 7369 2d73 6372  screener/rsi-scr
+00023650: 6565 6e69 6e67 0a20 2020 2020 2020 2069  eening.        i
+00023660: 6620 7273 693e 2030 2061 6e64 2072 7369  f rsi> 0 and rsi
+00023670: 203e 3d20 6d69 6e52 5349 2061 6e64 2072   >= minRSI and r
+00023680: 7369 203c 3d20 6d61 7852 5349 3a20 2023  si <= maxRSI:  #
+00023690: 206f 7220 2872 7369 203c 3d20 3731 2061   or (rsi <= 71 a
+000236a0: 6e64 2072 7369 203e 3d20 3637 293a 0a20  nd rsi >= 67):. 
+000236b0: 2020 2020 2020 2020 2020 2073 6372 6565             scree
+000236c0: 6e44 6963 745b 7273 694b 6579 5d20 3d20  nDict[rsiKey] = 
+000236d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000236e0: 2020 636f 6c6f 7254 6578 742e 424f 4c44    colorText.BOLD
+000236f0: 202b 2063 6f6c 6f72 5465 7874 2e47 5245   + colorText.GRE
+00023700: 454e 202b 2073 7472 2872 7369 2920 2b20  EN + str(rsi) + 
+00023710: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
+00023720: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00023730: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00023740: 7275 6520 6966 2028 7273 694b 6579 203d  rue if (rsiKey =
+00023750: 3d20 2252 5349 6922 2920 656c 7365 2028  = "RSIi") else (
+00023760: 7365 6c66 2e76 616c 6964 6174 6552 5349  self.validateRSI
+00023770: 2864 662c 2073 6372 6565 6e44 6963 742c  (df, screenDict,
+00023780: 2073 6176 6544 6963 742c 206d 696e 5253   saveDict, minRS
+00023790: 492c 206d 6178 5253 492c 7273 694b 6579  I, maxRSI,rsiKey
+000237a0: 3d22 5253 4969 2229 206f 7220 5472 7565  ="RSIi") or True
+000237b0: 290a 2020 2020 2020 2020 7363 7265 656e  ).        screen
+000237c0: 4469 6374 5b72 7369 4b65 795d 203d 2063  Dict[rsiKey] = c
+000237d0: 6f6c 6f72 5465 7874 2e42 4f4c 4420 2b20  olorText.BOLD + 
+000237e0: 636f 6c6f 7254 6578 742e 4641 494c 202b  colorText.FAIL +
+000237f0: 2073 7472 2872 7369 2920 2b20 636f 6c6f   str(rsi) + colo
+00023800: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+00023810: 2020 2320 4966 2065 6974 6865 7220 6461    # If either da
+00023820: 696c 7920 6f72 2069 6e74 7261 6461 7920  ily or intraday 
+00023830: 5253 4920 636f 6d65 7320 7769 7468 696e  RSI comes within
+00023840: 2072 616e 6765 3f0a 2020 2020 2020 2020   range?.        
+00023850: 7265 7475 726e 2046 616c 7365 2069 6620  return False if 
+00023860: 2872 7369 4b65 7920 3d3d 2022 5253 4969  (rsiKey == "RSIi
+00023870: 2229 2065 6c73 6520 2873 656c 662e 7661  ") else (self.va
+00023880: 6c69 6461 7465 5253 4928 6466 2c20 7363  lidateRSI(df, sc
+00023890: 7265 656e 4469 6374 2c20 7361 7665 4469  reenDict, saveDi
+000238a0: 6374 2c20 6d69 6e52 5349 2c20 6d61 7852  ct, minRSI, maxR
+000238b0: 5349 2c72 7369 4b65 793d 2252 5349 6922  SI,rsiKey="RSIi"
+000238c0: 2929 0a0a 2020 2020 2320 5661 6c69 6461  ))..    # Valida
+000238d0: 7465 2069 6620 7468 6520 7374 6f63 6b20  te if the stock 
+000238e0: 6973 2062 756c 6c69 7368 2069 6e20 7468  is bullish in th
+000238f0: 6520 7368 6f72 7420 7465 726d 0a20 2020  e short term.   
+00023900: 2064 6566 2076 616c 6964 6174 6553 686f   def validateSho
+00023910: 7274 5465 726d 4275 6c6c 6973 6828 7365  rtTermBullish(se
+00023920: 6c66 2c20 6466 2c20 7363 7265 656e 4469  lf, df, screenDi
+00023930: 6374 2c20 7361 7665 4469 6374 293a 0a20  ct, saveDict):. 
+00023940: 2020 2020 2020 2069 6620 6466 2069 7320         if df is 
+00023950: 4e6f 6e65 206f 7220 6c65 6e28 6466 2920  None or len(df) 
+00023960: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00023970: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
+00023980: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
+00023990: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
+000239a0: 2320 6874 7470 733a 2f2f 6368 6172 7469  # https://charti
+000239b0: 6e6b 2e63 6f6d 2f73 6372 6565 6e65 722f  nk.com/screener/
+000239c0: 7368 6f72 742d 7465 726d 2d62 756c 6c69  short-term-bulli
+000239d0: 7368 0a20 2020 2020 2020 2064 6174 6120  sh.        data 
+000239e0: 3d20 6461 7461 2e66 696c 6c6e 6128 3029  = data.fillna(0)
+000239f0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00023a00: 6461 7461 2e72 6570 6c61 6365 285b 6e70  data.replace([np
+00023a10: 2e69 6e66 2c20 2d6e 702e 696e 665d 2c20  .inf, -np.inf], 
+00023a20: 3029 0a20 2020 2020 2020 2072 6563 656e  0).        recen
+00023a30: 7420 3d20 6461 7461 2e68 6561 6428 3129  t = data.head(1)
+00023a40: 0a20 2020 2020 2020 2066 6b20 3d20 3020  .        fk = 0 
+00023a50: 6966 206c 656e 2864 6174 6129 203c 2033  if len(data) < 3
+00023a60: 2065 6c73 6520 6e70 2e72 6f75 6e64 2864   else np.round(d
+00023a70: 6174 615b 2246 4153 544b 225d 2e69 6c6f  ata["FASTK"].ilo
+00023a80: 635b 325d 2c20 3529 0a20 2020 2020 2020  c[2], 5).       
+00023a90: 2023 2052 6576 6572 7365 2074 6865 2064   # Reverse the d
+00023aa0: 6174 6166 7261 6d65 2066 6f72 2069 6368  ataframe for ich
+00023ab0: 696d 6f6b 7520 6361 6c63 756c 6174 696f  imoku calculatio
+00023ac0: 6e73 2077 6974 6820 6461 7465 2069 6e20  ns with date in 
+00023ad0: 6173 6365 6e64 696e 6720 6f72 6465 720a  ascending order.
+00023ae0: 2020 2020 2020 2020 6466 5f6e 6577 203d          df_new =
+00023af0: 2064 6174 615b 3a3a 2d31 5d0a 2020 2020   data[::-1].    
+00023b00: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00023b10: 2020 2020 2064 665f 6963 6869 203d 2064       df_ichi = d
+00023b20: 665f 6e65 772e 7265 6e61 6d65 280a 2020  f_new.rename(.  
+00023b30: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00023b40: 6c75 6d6e 733d 7b0a 2020 2020 2020 2020  lumns={.        
+00023b50: 2020 2020 2020 2020 2020 2020 224f 7065              "Ope
+00023b60: 6e22 3a20 226f 7065 6e22 2c0a 2020 2020  n": "open",.    
+00023b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023b80: 2248 6967 6822 3a20 2268 6967 6822 2c0a  "High": "high",.
+00023b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ba0: 2020 2020 224c 6f77 223a 2022 6c6f 7722      "Low": "low"
+00023bb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00023bc0: 2020 2020 2020 2243 6c6f 7365 223a 2022        "Close": "
+00023bd0: 636c 6f73 6522 2c0a 2020 2020 2020 2020  close",.        
+00023be0: 2020 2020 2020 2020 2020 2020 2256 6f6c              "Vol
+00023bf0: 756d 6522 3a20 2276 6f6c 756d 6522 2c0a  ume": "volume",.
+00023c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023c10: 7d0a 2020 2020 2020 2020 2020 2020 290a  }.            ).
+00023c20: 2020 2020 2020 2020 2020 2020 6963 6869              ichi
+00023c30: 203d 2070 6b74 616c 6962 2e69 6368 696d   = pktalib.ichim
+00023c40: 6f6b 7528 6466 5f69 6368 692c 2039 2c20  oku(df_ichi, 9, 
+00023c50: 3236 2c20 3532 2c20 3236 290a 2020 2020  26, 52, 26).    
+00023c60: 2020 2020 2020 2020 6966 2069 6368 6920          if ichi 
+00023c70: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00023c80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00023c90: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00023ca0: 2020 6466 5f6e 6577 203d 2070 642e 636f    df_new = pd.co
+00023cb0: 6e63 6174 285b 6466 5f6e 6577 2c20 6963  ncat([df_new, ic
+00023cc0: 6869 5d2c 2061 7869 733d 3129 0a20 2020  hi], axis=1).   
+00023cd0: 2020 2020 2020 2020 2023 2052 6576 6572           # Rever
+00023ce0: 7365 2061 6761 696e 2074 6f20 6765 7420  se again to get 
+00023cf0: 7468 6520 6d6f 7374 2072 6563 656e 7420  the most recent 
+00023d00: 6461 7465 206f 6e20 746f 700a 2020 2020  date on top.    
+00023d10: 2020 2020 2020 2020 6466 5f6e 6577 203d          df_new =
+00023d20: 2064 665f 6e65 775b 3a3a 2d31 5d0a 2020   df_new[::-1].  
+00023d30: 2020 2020 2020 2020 2020 6466 5f6e 6577            df_new
+00023d40: 203d 2064 665f 6e65 772e 6865 6164 2831   = df_new.head(1
+00023d50: 290a 2020 2020 2020 2020 2020 2020 6466  ).            df
+00023d60: 5f6e 6577 5b22 636c 6f75 645f 6772 6565  _new["cloud_gree
+00023d70: 6e22 5d20 3d20 6466 5f6e 6577 5b22 4953  n"] = df_new["IS
+00023d80: 415f 3922 5d2e 696c 6f63 5b30 5d20 3e20  A_9"].iloc[0] > 
+00023d90: 6466 5f6e 6577 5b22 4953 425f 3236 225d  df_new["ISB_26"]
+00023da0: 2e69 6c6f 635b 305d 0a20 2020 2020 2020  .iloc[0].       
+00023db0: 2020 2020 2064 665f 6e65 775b 2263 6c6f       df_new["clo
+00023dc0: 7564 5f72 6564 225d 203d 2064 665f 6e65  ud_red"] = df_ne
+00023dd0: 775b 2249 5342 5f32 3622 5d2e 696c 6f63  w["ISB_26"].iloc
+00023de0: 5b30 5d20 3e20 6466 5f6e 6577 5b22 4953  [0] > df_new["IS
+00023df0: 415f 3922 5d2e 696c 6f63 5b30 5d0a 2020  A_9"].iloc[0].  
+00023e00: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+00023e10: 6570 7469 6f6e 2061 7320 653a 2020 2320  eption as e:  # 
+00023e20: 7072 6167 6d61 3a20 6e6f 2063 6f76 6572  pragma: no cover
+00023e30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00023e40: 662e 6465 6661 756c 745f 6c6f 6767 6572  f.default_logger
+00023e50: 2e64 6562 7567 2865 2c20 6578 635f 696e  .debug(e, exc_in
+00023e60: 666f 3d54 7275 6529 0a20 2020 2020 2020  fo=True).       
+00023e70: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
+00023e80: 2020 6162 6f76 6543 6c6f 7564 546f 7020    aboveCloudTop 
+00023e90: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+00023ea0: 2320 6261 7365 6c69 6e65 203e 2063 6c6f  # baseline > clo
+00023eb0: 7564 2074 6f70 2028 636c 6f75 6420 6973  ud top (cloud is
+00023ec0: 2062 6f75 6e64 2062 7920 7370 616e 2061   bound by span a
+00023ed0: 2061 6e64 2073 7061 6e20 6229 2061 6e64   and span b) and
+00023ee0: 2063 6c6f 7365 2069 7320 3e20 636c 6f75   close is > clou
+00023ef0: 6420 746f 700a 2020 2020 2020 2020 6966  d top.        if
+00023f00: 2064 665f 6e65 775b 2263 6c6f 7564 5f67   df_new["cloud_g
+00023f10: 7265 656e 225d 2e69 6c6f 635b 305d 3a0a  reen"].iloc[0]:.
+00023f20: 2020 2020 2020 2020 2020 2020 6162 6f76              abov
+00023f30: 6543 6c6f 7564 546f 7020 3d20 280a 2020  eCloudTop = (.  
+00023f40: 2020 2020 2020 2020 2020 2020 2020 6466                df
+00023f50: 5f6e 6577 5b22 494b 535f 3236 225d 2e69  _new["IKS_26"].i
+00023f60: 6c6f 635b 305d 203e 2064 665f 6e65 775b  loc[0] > df_new[
+00023f70: 2249 5341 5f39 225d 2e69 6c6f 635b 305d  "ISA_9"].iloc[0]
+00023f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023f90: 2061 6e64 2072 6563 656e 745b 2243 6c6f   and recent["Clo
+00023fa0: 7365 225d 2e69 6c6f 635b 305d 203e 2064  se"].iloc[0] > d
+00023fb0: 665f 6e65 775b 2249 5341 5f39 225d 2e69  f_new["ISA_9"].i
+00023fc0: 6c6f 635b 305d 0a20 2020 2020 2020 2020  loc[0].         
+00023fd0: 2020 2029 0a20 2020 2020 2020 2065 6c69     ).        eli
+00023fe0: 6620 6466 5f6e 6577 5b22 636c 6f75 645f  f df_new["cloud_
+00023ff0: 7265 6422 5d2e 696c 6f63 5b30 5d3a 0a20  red"].iloc[0]:. 
+00024000: 2020 2020 2020 2020 2020 2061 626f 7665             above
+00024010: 436c 6f75 6454 6f70 203d 2028 0a20 2020  CloudTop = (.   
+00024020: 2020 2020 2020 2020 2020 2020 2064 665f               df_
+00024030: 6e65 775b 2249 4b53 5f32 3622 5d2e 696c  new["IKS_26"].il
+00024040: 6f63 5b30 5d20 3e20 6466 5f6e 6577 5b22  oc[0] > df_new["
+00024050: 4953 425f 3236 225d 2e69 6c6f 635b 305d  ISB_26"].iloc[0]
+00024060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024070: 2061 6e64 2072 6563 656e 745b 2243 6c6f   and recent["Clo
+00024080: 7365 225d 2e69 6c6f 635b 305d 203e 2064  se"].iloc[0] > d
+00024090: 665f 6e65 775b 2249 5342 5f32 3622 5d2e  f_new["ISB_26"].
+000240a0: 696c 6f63 5b30 5d0a 2020 2020 2020 2020  iloc[0].        
+000240b0: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+000240c0: 204c 6174 6573 7420 4963 6869 6d6f 6b75   Latest Ichimoku
+000240d0: 2062 6173 656c 696e 6520 6973 203c 206c   baseline is < l
+000240e0: 6174 6573 7420 4963 6869 6d6f 6b75 2063  atest Ichimoku c
+000240f0: 6f6e 7665 7273 696f 6e20 6c69 6e65 0a20  onversion line. 
+00024100: 2020 2020 2020 2069 6620 6162 6f76 6543         if aboveC
+00024110: 6c6f 7564 546f 7020 616e 6420 6466 5f6e  loudTop and df_n
+00024120: 6577 5b22 494b 535f 3236 225d 2e69 6c6f  ew["IKS_26"].ilo
+00024130: 635b 305d 203c 2064 665f 6e65 775b 2249  c[0] < df_new["I
+00024140: 5453 5f39 225d 2e69 6c6f 635b 305d 3a0a  TS_9"].iloc[0]:.
+00024150: 2020 2020 2020 2020 2020 2020 2320 5374              # St
+00024160: 6f63 6852 5349 2063 726f 7373 6564 2032  ochRSI crossed 2
+00024170: 3020 616e 6420 5253 4920 3e20 3530 0a20  0 and RSI > 50. 
+00024180: 2020 2020 2020 2020 2020 2069 6620 666b             if fk
+00024190: 203e 2032 3020 616e 6420 7265 6365 6e74   > 20 and recent
+000241a0: 5b22 5253 4922 5d2e 696c 6f63 5b30 5d20  ["RSI"].iloc[0] 
+000241b0: 3e20 3530 3a0a 2020 2020 2020 2020 2020  > 50:.          
+000241c0: 2020 2020 2020 2320 636f 6e64 6974 696f        # conditio
+000241d0: 6e20 6f66 2063 726f 7373 696e 6720 7468  n of crossing th
+000241e0: 6520 5374 6f63 6852 5349 206d 6169 6e20  e StochRSI main 
+000241f0: 7369 676e 616c 206c 696e 6520 6672 6f6d  signal line from
+00024200: 2062 6f74 746f 6d20 746f 2074 6f70 0a20   bottom to top. 
+00024210: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00024220: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00024230: 2020 2020 2020 2020 6461 7461 5b22 4641          data["FA
+00024240: 5354 4422 5d2e 696c 6f63 5b31 3030 5d20  STD"].iloc[100] 
+00024250: 3c20 6461 7461 5b22 4641 5354 4b22 5d2e  < data["FASTK"].
+00024260: 696c 6f63 5b31 3030 5d0a 2020 2020 2020  iloc[100].      
+00024270: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00024280: 6420 6461 7461 5b22 4641 5354 4422 5d2e  d data["FASTD"].
+00024290: 696c 6f63 5b31 3031 5d20 3e20 6461 7461  iloc[101] > data
+000242a0: 5b22 4641 5354 4b22 5d2e 696c 6f63 5b31  ["FASTK"].iloc[1
+000242b0: 3031 5d0a 2020 2020 2020 2020 2020 2020  01].            
+000242c0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+000242d0: 2020 2020 2020 2020 2020 2023 2063 6c6f             # clo
+000242e0: 7365 203e 2035 3020 7065 7269 6f64 2053  se > 50 period S
+000242f0: 4d41 2f45 4d41 2061 6e64 2032 3030 2070  MA/EMA and 200 p
+00024300: 6572 696f 6420 534d 412f 454d 410a 2020  eriod SMA/EMA.  
+00024310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024320: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
+00024330: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00024340: 6563 656e 745b 2253 534d 4122 5d2e 696c  ecent["SSMA"].il
+00024350: 6f63 5b30 5d20 3e20 7265 6365 6e74 5b22  oc[0] > recent["
+00024360: 534d 4122 5d2e 696c 6f63 5b30 5d0a 2020  SMA"].iloc[0].  
+00024370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024380: 2020 2020 2020 616e 6420 7265 6365 6e74        and recent
+00024390: 5b22 436c 6f73 6522 5d2e 696c 6f63 5b30  ["Close"].iloc[0
+000243a0: 5d20 3e20 7265 6365 6e74 5b22 5353 4d41  ] > recent["SSMA
+000243b0: 225d 2e69 6c6f 635b 305d 0a20 2020 2020  "].iloc[0].     
+000243c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000243d0: 2020 2061 6e64 2072 6563 656e 745b 2243     and recent["C
+000243e0: 6c6f 7365 225d 2e69 6c6f 635b 305d 203e  lose"].iloc[0] >
+000243f0: 2072 6563 656e 745b 224c 4d41 225d 2e69   recent["LMA"].i
+00024400: 6c6f 635b 305d 0a20 2020 2020 2020 2020  loc[0].         
+00024410: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
+00024420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024430: 2020 2020 2020 7361 7665 6420 3d20 7365        saved = se
+00024440: 6c66 2e66 696e 6443 7572 7265 6e74 5361  lf.findCurrentSa
+00024450: 7665 6456 616c 7565 2873 6372 6565 6e44  vedValue(screenD
+00024460: 6963 742c 7361 7665 4469 6374 2c22 4d41  ict,saveDict,"MA
+00024470: 2d53 6967 6e61 6c22 290a 2020 2020 2020  -Signal").      
+00024480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024490: 2020 7363 7265 656e 4469 6374 5b22 4d41    screenDict["MA
+000244a0: 2d53 6967 6e61 6c22 5d20 3d20 280a 2020  -Signal"] = (.  
+000244b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000244c0: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+000244d0: 305d 202b 2063 6f6c 6f72 5465 7874 2e42  0] + colorText.B
+000244e0: 4f4c 4420 2b20 636f 6c6f 7254 6578 742e  OLD + colorText.
+000244f0: 4752 4545 4e20 2b20 2242 756c 6c69 7368  GREEN + "Bullish
+00024500: 2220 2b20 636f 6c6f 7254 6578 742e 454e  " + colorText.EN
+00024510: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+00024520: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00024530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024540: 2020 2020 7361 7665 4469 6374 5b22 4d41      saveDict["MA
+00024550: 2d53 6967 6e61 6c22 5d20 3d20 7361 7665  -Signal"] = save
+00024560: 645b 315d 202b 2022 4275 6c6c 6973 6822  d[1] + "Bullish"
+00024570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024580: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00024590: 5472 7565 0a20 2020 2020 2020 2072 6574  True.        ret
+000245a0: 7572 6e20 4661 6c73 650a 2020 2020 0a20  urn False.    . 
+000245b0: 2020 2023 2056 616c 6964 6174 6520 5643     # Validate VC
+000245c0: 5020 6173 2070 6572 204d 6172 6b20 4d69  P as per Mark Mi
+000245d0: 6e65 7276 696e 690a 2020 2020 2320 6874  nervini.    # ht
+000245e0: 7470 733a 2f2f 6368 6172 7469 6e6b 2e63  tps://chartink.c
+000245f0: 6f6d 2f73 6372 6565 6e65 722f 766f 6c61  om/screener/vola
+00024600: 7469 6c69 7479 2d63 6f6d 7072 6573 7369  tility-compressi
+00024610: 6f6e 0a20 2020 2064 6566 2076 616c 6964  on.    def valid
+00024620: 6174 6556 4350 4d61 726b 4d69 6e65 7276  ateVCPMarkMinerv
+00024630: 696e 6928 7365 6c66 2c20 6466 3a70 642e  ini(self, df:pd.
+00024640: 4461 7461 4672 616d 652c 2073 6372 6565  DataFrame, scree
+00024650: 6e44 6963 742c 2073 6176 6544 6963 7429  nDict, saveDict)
+00024660: 3a0a 2020 2020 2020 2020 6966 2064 6620  :.        if df 
+00024670: 6973 204e 6f6e 6520 6f72 206c 656e 2864  is None or len(d
+00024680: 6629 203d 3d20 303a 0a20 2020 2020 2020  f) == 0:.       
+00024690: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+000246a0: 650a 2020 2020 2020 2020 6461 7461 203d  e.        data =
+000246b0: 2064 662e 636f 7079 2829 0a20 2020 2020   df.copy().     
+000246c0: 2020 206f 686c 635f 6469 6374 203d 207b     ohlc_dict = {
+000246d0: 0a20 2020 2020 2020 2020 2020 2027 4f70  .            'Op
+000246e0: 656e 273a 2766 6972 7374 272c 0a20 2020  en':'first',.   
+000246f0: 2020 2020 2020 2020 2027 4869 6768 273a           'High':
+00024700: 276d 6178 272c 0a20 2020 2020 2020 2020  'max',.         
+00024710: 2020 2027 4c6f 7727 3a27 6d69 6e27 2c0a     'Low':'min',.
+00024720: 2020 2020 2020 2020 2020 2020 2743 6c6f              'Clo
+00024730: 7365 273a 276c 6173 7427 2c0a 2020 2020  se':'last',.    
+00024740: 2020 2020 2020 2020 2756 6f6c 756d 6527          'Volume'
+00024750: 3a27 7375 6d27 0a20 2020 2020 2020 207d  :'sum'.        }
+00024760: 0a20 2020 2020 2020 2023 2066 696e 616c  .        # final
+00024770: 5f64 6620 3d20 6466 2e72 6573 616d 706c  _df = df.resampl
+00024780: 6528 2757 2d46 5249 272c 2063 6c6f 7365  e('W-FRI', close
+00024790: 643d 276c 6566 7427 292e 6167 6728 6f68  d='left').agg(oh
+000247a0: 6c63 5f64 6963 7429 2e73 6869 6674 2827  lc_dict).shift('
+000247b0: 3164 2729 0a20 2020 2020 2020 2077 6565  1d').        wee
+000247c0: 6b6c 7944 6174 6120 3d20 6461 7461 2e72  klyData = data.r
+000247d0: 6573 616d 706c 6528 2757 2729 2e61 6767  esample('W').agg
+000247e0: 286f 686c 635f 6469 6374 290a 2020 2020  (ohlc_dict).    
+000247f0: 2020 2020 7265 7665 7273 6564 4461 7461      reversedData
+00024800: 203d 2064 6174 615b 3a3a 2d31 5d20 2023   = data[::-1]  #
+00024810: 2052 6576 6572 7365 2074 6865 2064 6174   Reverse the dat
+00024820: 6166 7261 6d65 0a20 2020 2020 2020 2072  aframe.        r
+00024830: 6563 656e 745f 636c 6f73 6520 3d20 6461  ecent_close = da
+00024840: 7461 5b22 436c 6f73 6522 5d2e 6865 6164  ta["Close"].head
+00024850: 2831 292e 696c 6f63 5b30 5d0a 2020 2020  (1).iloc[0].    
+00024860: 2020 2020 775f 656d 615f 3133 203d 2070      w_ema_13 = p
+00024870: 6b74 616c 6962 2e45 4d41 2877 6565 6b6c  ktalib.EMA(weekl
+00024880: 7944 6174 615b 2243 6c6f 7365 225d 2c74  yData["Close"],t
+00024890: 696d 6570 6572 696f 643d 3133 292e 7461  imeperiod=13).ta
+000248a0: 696c 2831 292e 696c 6f63 5b30 5d0a 2020  il(1).iloc[0].  
+000248b0: 2020 2020 2020 775f 656d 615f 3236 203d        w_ema_26 =
+000248c0: 2070 6b74 616c 6962 2e45 4d41 2877 6565   pktalib.EMA(wee
+000248d0: 6b6c 7944 6174 615b 2243 6c6f 7365 225d  klyData["Close"]
+000248e0: 2c74 696d 6570 6572 696f 643d 3236 292e  ,timeperiod=26).
+000248f0: 7461 696c 2831 292e 696c 6f63 5b30 5d0a  tail(1).iloc[0].
+00024900: 2020 2020 2020 2020 775f 736d 615f 3530          w_sma_50
+00024910: 203d 2070 6b74 616c 6962 2e53 4d41 2877   = pktalib.SMA(w
+00024920: 6565 6b6c 7944 6174 615b 2243 6c6f 7365  eeklyData["Close
+00024930: 225d 2c74 696d 6570 6572 696f 643d 3530  "],timeperiod=50
+00024940: 292e 7461 696c 2831 292e 696c 6f63 5b30  ).tail(1).iloc[0
+00024950: 5d0a 2020 2020 2020 2020 775f 736d 615f  ].        w_sma_
+00024960: 3430 203d 2070 6b74 616c 6962 2e53 4d41  40 = pktalib.SMA
+00024970: 2877 6565 6b6c 7944 6174 615b 2243 6c6f  (weeklyData["Clo
+00024980: 7365 225d 2c74 696d 6570 6572 696f 643d  se"],timeperiod=
+00024990: 3430 292e 7461 696c 2831 292e 696c 6f63  40).tail(1).iloc
+000249a0: 5b30 5d0a 2020 2020 2020 2020 775f 736d  [0].        w_sm
+000249b0: 615f 3430 5f35 775f 6167 6f20 3d20 706b  a_40_5w_ago = pk
+000249c0: 7461 6c69 622e 534d 4128 7765 656b 6c79  talib.SMA(weekly
+000249d0: 4461 7461 2e68 6561 6428 6c65 6e28 7765  Data.head(len(we
+000249e0: 656b 6c79 4461 7461 292d 3529 5b22 436c  eklyData)-5)["Cl
+000249f0: 6f73 6522 5d2c 7469 6d65 7065 7269 6f64  ose"],timeperiod
+00024a00: 3d34 3029 2e74 6169 6c28 3129 2e69 6c6f  =40).tail(1).ilo
+00024a10: 635b 305d 0a20 2020 2020 2020 2077 5f6d  c[0].        w_m
+00024a20: 696e 5f35 3020 3d20 6d69 6e28 312e 332a  in_50 = min(1.3*
+00024a30: 7765 656b 6c79 4461 7461 2e74 6169 6c28  weeklyData.tail(
+00024a40: 3530 295b 224c 6f77 225d 290a 2020 2020  50)["Low"]).    
+00024a50: 2020 2020 775f 6d61 785f 3530 203d 206d      w_max_50 = m
+00024a60: 6178 2830 2e37 352a 7765 656b 6c79 4461  ax(0.75*weeklyDa
+00024a70: 7461 2e74 6169 6c28 3530 295b 2248 6967  ta.tail(50)["Hig
+00024a80: 6822 5d29 0a20 2020 2020 2020 2077 5f65  h"]).        w_e
+00024a90: 6d61 5f32 365f 3230 775f 6167 6f20 3d20  ma_26_20w_ago = 
+00024aa0: 706b 7461 6c69 622e 454d 4128 7765 656b  pktalib.EMA(week
+00024ab0: 6c79 4461 7461 2e68 6561 6428 6c65 6e28  lyData.head(len(
+00024ac0: 7765 656b 6c79 4461 7461 292d 3230 295b  weeklyData)-20)[
+00024ad0: 2243 6c6f 7365 225d 2c74 696d 6570 6572  "Close"],timeper
+00024ae0: 696f 643d 3236 292e 7461 696c 2831 292e  iod=26).tail(1).
+00024af0: 696c 6f63 5b30 5d0a 2020 2020 2020 2020  iloc[0].        
+00024b00: 7265 6365 6e74 5f65 6d61 5f31 335f 3230  recent_ema_13_20
+00024b10: 645f 6167 6f20 3d20 706b 7461 6c69 622e  d_ago = pktalib.
+00024b20: 454d 4128 7265 7665 7273 6564 4461 7461  EMA(reversedData
+00024b30: 2e68 6561 6428 6c65 6e28 7265 7665 7273  .head(len(revers
+00024b40: 6564 4461 7461 292d 3230 295b 2243 6c6f  edData)-20)["Clo
+00024b50: 7365 225d 2c74 696d 6570 6572 696f 643d  se"],timeperiod=
+00024b60: 3133 292e 7461 696c 2831 292e 696c 6f63  13).tail(1).iloc
+00024b70: 5b30 5d0a 2020 2020 2020 2020 775f 736d  [0].        w_sm
+00024b80: 615f 3430 5f35 775f 6167 6f20 3d20 706b  a_40_5w_ago = pk
+00024b90: 7461 6c69 622e 534d 4128 7765 656b 6c79  talib.SMA(weekly
+00024ba0: 4461 7461 2e68 6561 6428 6c65 6e28 7765  Data.head(len(we
+00024bb0: 656b 6c79 4461 7461 292d 3529 5b22 436c  eklyData)-5)["Cl
+00024bc0: 6f73 6522 5d2c 7469 6d65 7065 7269 6f64  ose"],timeperiod
+00024bd0: 3d34 3029 2e74 6169 6c28 3129 2e69 6c6f  =40).tail(1).ilo
+00024be0: 635b 305d 0a20 2020 2020 2020 2077 5f73  c[0].        w_s
+00024bf0: 6d61 5f34 305f 3130 775f 6167 6f20 3d20  ma_40_10w_ago = 
+00024c00: 706b 7461 6c69 622e 534d 4128 7765 656b  pktalib.SMA(week
+00024c10: 6c79 4461 7461 2e68 6561 6428 6c65 6e28  lyData.head(len(
+00024c20: 7765 656b 6c79 4461 7461 292d 3130 295b  weeklyData)-10)[
+00024c30: 2243 6c6f 7365 225d 2c74 696d 6570 6572  "Close"],timeper
+00024c40: 696f 643d 3430 292e 7461 696c 2831 292e  iod=40).tail(1).
+00024c50: 696c 6f63 5b30 5d0a 2020 2020 2020 2020  iloc[0].        
+00024c60: 7265 6365 6e74 5f73 6d61 5f35 3020 3d20  recent_sma_50 = 
+00024c70: 706b 7461 6c69 622e 534d 4128 7265 7665  pktalib.SMA(reve
+00024c80: 7273 6564 4461 7461 5b22 436c 6f73 6522  rsedData["Close"
+00024c90: 5d2c 7469 6d65 7065 7269 6f64 3d35 3029  ],timeperiod=50)
+00024ca0: 2e74 6169 6c28 3129 2e69 6c6f 635b 305d  .tail(1).iloc[0]
+00024cb0: 0a20 2020 2020 2020 2077 5f77 6d61 5f38  .        w_wma_8
+00024cc0: 203d 2070 6b74 616c 6962 2e57 4d41 2877   = pktalib.WMA(w
+00024cd0: 6565 6b6c 7944 6174 615b 2243 6c6f 7365  eeklyData["Close
+00024ce0: 225d 2c74 696d 6570 6572 696f 643d 3829  "],timeperiod=8)
+00024cf0: 2e74 6169 6c28 3129 2e69 6c6f 635b 305d  .tail(1).iloc[0]
+00024d00: 0a20 2020 2020 2020 2077 5f73 6d61 5f38  .        w_sma_8
+00024d10: 203d 2070 6b74 616c 6962 2e53 4d41 2877   = pktalib.SMA(w
+00024d20: 6565 6b6c 7944 6174 615b 2243 6c6f 7365  eeklyData["Close
+00024d30: 225d 2c74 696d 6570 6572 696f 643d 3829  "],timeperiod=8)
+00024d40: 2e74 6169 6c28 3129 2e69 6c6f 635b 305d  .tail(1).iloc[0]
+00024d50: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00024d60: 2020 6973 5643 5020 3d20 775f 656d 615f    isVCP = w_ema_
+00024d70: 3133 203e 2077 5f65 6d61 5f32 3620 616e  13 > w_ema_26 an
 00024d80: 6420 5c0a 2020 2020 2020 2020 2020 2020  d \.            
-00024d90: 2020 2020 7265 6365 6e74 5f63 6c6f 7365      recent_close
-00024da0: 203e 3d20 775f 6d61 785f 3530 2061 6e64   >= w_max_50 and
-00024db0: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-00024dc0: 2020 2072 6563 656e 745f 656d 615f 3133     recent_ema_13
-00024dd0: 5f32 3064 5f61 676f 203e 2077 5f65 6d61  _20d_ago > w_ema
-00024de0: 5f32 365f 3230 775f 6167 6f20 616e 6420  _26_20w_ago and 
-00024df0: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
-00024e00: 2020 775f 736d 615f 3430 5f35 775f 6167    w_sma_40_5w_ag
-00024e10: 6f20 3e20 775f 736d 615f 3430 5f31 3077  o > w_sma_40_10w
-00024e20: 5f61 676f 2061 6e64 205c 0a20 2020 2020  _ago and \.     
-00024e30: 2020 2020 2020 2020 2020 2072 6563 656e             recen
-00024e40: 745f 636c 6f73 6520 3e20 7265 6365 6e74  t_close > recent
-00024e50: 5f73 6d61 5f35 3020 616e 6420 5c0a 2020  _sma_50 and \.  
-00024e60: 2020 2020 2020 2020 2020 2020 2020 2877                (w
-00024e70: 5f77 6d61 5f38 202d 2077 5f73 6d61 5f38  _wma_8 - w_sma_8
-00024e80: 292a 362f 3239 203c 2030 2e35 2061 6e64  )*6/29 < 0.5 and
-00024e90: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-00024ea0: 2020 2072 6563 656e 745f 636c 6f73 6520     recent_close 
-00024eb0: 3e20 3130 0a20 2020 2020 2020 2069 6620  > 10.        if 
-00024ec0: 6973 5643 503a 0a20 2020 2020 2020 2020  isVCP:.         
-00024ed0: 2020 2073 6176 6564 203d 2073 656c 662e     saved = self.
-00024ee0: 6669 6e64 4375 7272 656e 7453 6176 6564  findCurrentSaved
-00024ef0: 5661 6c75 6528 7363 7265 656e 4469 6374  Value(screenDict
-00024f00: 2c20 7361 7665 4469 6374 2c20 2250 6174  , saveDict, "Pat
-00024f10: 7465 726e 2229 0a20 2020 2020 2020 2020  tern").         
-00024f20: 2020 2073 6372 6565 6e44 6963 745b 2250     screenDict["P
-00024f30: 6174 7465 726e 225d 203d 2028 0a20 2020  attern"] = (.   
-00024f40: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00024f50: 6564 5b30 5d20 0a20 2020 2020 2020 2020  ed[0] .         
-00024f60: 2020 2020 2020 202b 2063 6f6c 6f72 5465         + colorTe
-00024f70: 7874 2e42 4f4c 440a 2020 2020 2020 2020  xt.BOLD.        
-00024f80: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
-00024f90: 6578 742e 4752 4545 4e0a 2020 2020 2020  ext.GREEN.      
-00024fa0: 2020 2020 2020 2020 2020 2b20 6622 5643            + f"VC
-00024fb0: 5028 4d69 6e65 7276 696e 6929 220a 2020  P(Minervini)".  
-00024fc0: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00024fd0: 636f 6c6f 7254 6578 742e 454e 440a 2020  colorText.END.  
-00024fe0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00024ff0: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
-00025000: 5b22 5061 7474 6572 6e22 5d20 3d20 7361  ["Pattern"] = sa
-00025010: 7665 645b 315d 202b 2066 2256 4350 284d  ved[1] + f"VCP(M
-00025020: 696e 6572 7669 6e69 2922 0a20 2020 2020  inervini)".     
-00025030: 2020 2072 6574 7572 6e20 6973 5643 500a     return isVCP.
-00025040: 2020 2020 0a20 2020 2023 2056 616c 6964      .    # Valid
-00025050: 6174 6520 5643 500a 2020 2020 6465 6620  ate VCP.    def 
-00025060: 7661 6c69 6461 7465 5643 5028 0a20 2020  validateVCP(.   
-00025070: 2020 2020 2073 656c 662c 2064 662c 2073       self, df, s
-00025080: 6372 6565 6e44 6963 742c 2073 6176 6544  creenDict, saveD
-00025090: 6963 742c 2073 746f 636b 4e61 6d65 3d4e  ict, stockName=N
-000250a0: 6f6e 652c 2077 696e 646f 773d 332c 2070  one, window=3, p
-000250b0: 6572 6365 6e74 6167 6546 726f 6d54 6f70  ercentageFromTop
-000250c0: 3d33 0a20 2020 2029 3a0a 2020 2020 2020  =3.    ):.      
-000250d0: 2020 6966 2064 6620 6973 204e 6f6e 6520    if df is None 
-000250e0: 6f72 206c 656e 2864 6629 203d 3d20 303a  or len(df) == 0:
-000250f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00025100: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
-00025110: 2020 6461 7461 203d 2064 662e 636f 7079    data = df.copy
-00025120: 2829 0a20 2020 2020 2020 2074 7279 3a0a  ().        try:.
-00025130: 2020 2020 2020 2020 2020 2020 7065 7263              perc
-00025140: 656e 7461 6765 4672 6f6d 546f 7020 2f3d  entageFromTop /=
-00025150: 2031 3030 0a20 2020 2020 2020 2020 2020   100.           
-00025160: 2064 6174 612e 7265 7365 745f 696e 6465   data.reset_inde
-00025170: 7828 696e 706c 6163 653d 5472 7565 290a  x(inplace=True).
-00025180: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00025190: 2e72 656e 616d 6528 636f 6c75 6d6e 733d  .rename(columns=
-000251a0: 7b22 696e 6465 7822 3a20 2244 6174 6522  {"index": "Date"
-000251b0: 7d2c 2069 6e70 6c61 6365 3d54 7275 6529  }, inplace=True)
-000251c0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-000251d0: 615b 2274 6f70 7322 5d20 3d20 2864 6174  a["tops"] = (dat
-000251e0: 615b 2248 6967 6822 5d2e 696c 6f63 5b6c  a["High"].iloc[l
-000251f0: 6973 7428 706b 7461 6c69 622e 6172 6772  ist(pktalib.argr
-00025200: 656c 6578 7472 656d 6128 6e70 2e61 7272  elextrema(np.arr
-00025210: 6179 2864 6174 615b 2248 6967 6822 5d29  ay(data["High"])
-00025220: 2c20 6e70 2e67 7265 6174 6572 5f65 7175  , np.greater_equ
-00025230: 616c 2c20 6f72 6465 723d 7769 6e64 6f77  al, order=window
-00025240: 295b 305d 295d 2e68 6561 6428 3429 290a  )[0])].head(4)).
-00025250: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00025260: 5b22 626f 7473 225d 203d 2028 6461 7461  ["bots"] = (data
-00025270: 5b22 4c6f 7722 5d2e 696c 6f63 5b6c 6973  ["Low"].iloc[lis
-00025280: 7428 706b 7461 6c69 622e 6172 6772 656c  t(pktalib.argrel
-00025290: 6578 7472 656d 6128 6e70 2e61 7272 6179  extrema(np.array
-000252a0: 2864 6174 615b 224c 6f77 225d 292c 206e  (data["Low"]), n
-000252b0: 702e 6c65 7373 5f65 7175 616c 2c20 6f72  p.less_equal, or
+00024d90: 2020 2020 775f 656d 615f 3236 203e 2077      w_ema_26 > w
+00024da0: 5f73 6d61 5f35 3020 616e 6420 5c0a 2020  _sma_50 and \.  
+00024db0: 2020 2020 2020 2020 2020 2020 2020 775f                w_
+00024dc0: 736d 615f 3430 203e 2077 5f73 6d61 5f34  sma_40 > w_sma_4
+00024dd0: 305f 3577 5f61 676f 2061 6e64 205c 0a20  0_5w_ago and \. 
+00024de0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00024df0: 6563 656e 745f 636c 6f73 6520 3e3d 2077  ecent_close >= w
+00024e00: 5f6d 696e 5f35 3020 616e 6420 5c0a 2020  _min_50 and \.  
+00024e10: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00024e20: 6365 6e74 5f63 6c6f 7365 203e 3d20 775f  cent_close >= w_
+00024e30: 6d61 785f 3530 2061 6e64 205c 0a20 2020  max_50 and \.   
+00024e40: 2020 2020 2020 2020 2020 2020 2072 6563               rec
+00024e50: 656e 745f 656d 615f 3133 5f32 3064 5f61  ent_ema_13_20d_a
+00024e60: 676f 203e 2077 5f65 6d61 5f32 365f 3230  go > w_ema_26_20
+00024e70: 775f 6167 6f20 616e 6420 5c0a 2020 2020  w_ago and \.    
+00024e80: 2020 2020 2020 2020 2020 2020 775f 736d              w_sm
+00024e90: 615f 3430 5f35 775f 6167 6f20 3e20 775f  a_40_5w_ago > w_
+00024ea0: 736d 615f 3430 5f31 3077 5f61 676f 2061  sma_40_10w_ago a
+00024eb0: 6e64 205c 0a20 2020 2020 2020 2020 2020  nd \.           
+00024ec0: 2020 2020 2072 6563 656e 745f 636c 6f73       recent_clos
+00024ed0: 6520 3e20 7265 6365 6e74 5f73 6d61 5f35  e > recent_sma_5
+00024ee0: 3020 616e 6420 5c0a 2020 2020 2020 2020  0 and \.        
+00024ef0: 2020 2020 2020 2020 2877 5f77 6d61 5f38          (w_wma_8
+00024f00: 202d 2077 5f73 6d61 5f38 292a 362f 3239   - w_sma_8)*6/29
+00024f10: 203c 2030 2e35 2061 6e64 205c 0a20 2020   < 0.5 and \.   
+00024f20: 2020 2020 2020 2020 2020 2020 2072 6563               rec
+00024f30: 656e 745f 636c 6f73 6520 3e20 3130 0a20  ent_close > 10. 
+00024f40: 2020 2020 2020 2069 6620 6973 5643 503a         if isVCP:
+00024f50: 0a20 2020 2020 2020 2020 2020 2073 6176  .            sav
+00024f60: 6564 203d 2073 656c 662e 6669 6e64 4375  ed = self.findCu
+00024f70: 7272 656e 7453 6176 6564 5661 6c75 6528  rrentSavedValue(
+00024f80: 7363 7265 656e 4469 6374 2c20 7361 7665  screenDict, save
+00024f90: 4469 6374 2c20 2250 6174 7465 726e 2229  Dict, "Pattern")
+00024fa0: 0a20 2020 2020 2020 2020 2020 2073 6372  .            scr
+00024fb0: 6565 6e44 6963 745b 2250 6174 7465 726e  eenDict["Pattern
+00024fc0: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
+00024fd0: 2020 2020 2020 2073 6176 6564 5b30 5d20         saved[0] 
+00024fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00024ff0: 202b 2063 6f6c 6f72 5465 7874 2e42 4f4c   + colorText.BOL
+00025000: 440a 2020 2020 2020 2020 2020 2020 2020  D.              
+00025010: 2020 2b20 636f 6c6f 7254 6578 742e 4752    + colorText.GR
+00025020: 4545 4e0a 2020 2020 2020 2020 2020 2020  EEN.            
+00025030: 2020 2020 2b20 6622 5643 5028 4d69 6e65      + f"VCP(Mine
+00025040: 7276 696e 6929 220a 2020 2020 2020 2020  rvini)".        
+00025050: 2020 2020 2020 2020 2b20 636f 6c6f 7254          + colorT
+00025060: 6578 742e 454e 440a 2020 2020 2020 2020  ext.END.        
+00025070: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00025080: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
+00025090: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
+000250a0: 202b 2066 2256 4350 284d 696e 6572 7669   + f"VCP(Minervi
+000250b0: 6e69 2922 0a20 2020 2020 2020 2072 6574  ni)".        ret
+000250c0: 7572 6e20 6973 5643 500a 2020 2020 0a20  urn isVCP.    . 
+000250d0: 2020 2023 2056 616c 6964 6174 6520 5643     # Validate VC
+000250e0: 500a 2020 2020 6465 6620 7661 6c69 6461  P.    def valida
+000250f0: 7465 5643 5028 0a20 2020 2020 2020 2073  teVCP(.        s
+00025100: 656c 662c 2064 662c 2073 6372 6565 6e44  elf, df, screenD
+00025110: 6963 742c 2073 6176 6544 6963 742c 2073  ict, saveDict, s
+00025120: 746f 636b 4e61 6d65 3d4e 6f6e 652c 2077  tockName=None, w
+00025130: 696e 646f 773d 332c 2070 6572 6365 6e74  indow=3, percent
+00025140: 6167 6546 726f 6d54 6f70 3d33 0a20 2020  ageFromTop=3.   
+00025150: 2029 3a0a 2020 2020 2020 2020 6966 2064   ):.        if d
+00025160: 6620 6973 204e 6f6e 6520 6f72 206c 656e  f is None or len
+00025170: 2864 6629 203d 3d20 303a 0a20 2020 2020  (df) == 0:.     
+00025180: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00025190: 6c73 650a 2020 2020 2020 2020 6461 7461  lse.        data
+000251a0: 203d 2064 662e 636f 7079 2829 0a20 2020   = df.copy().   
+000251b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000251c0: 2020 2020 2020 7065 7263 656e 7461 6765        percentage
+000251d0: 4672 6f6d 546f 7020 2f3d 2031 3030 0a20  FromTop /= 100. 
+000251e0: 2020 2020 2020 2020 2020 2064 6174 612e             data.
+000251f0: 7265 7365 745f 696e 6465 7828 696e 706c  reset_index(inpl
+00025200: 6163 653d 5472 7565 290a 2020 2020 2020  ace=True).      
+00025210: 2020 2020 2020 6461 7461 2e72 656e 616d        data.renam
+00025220: 6528 636f 6c75 6d6e 733d 7b22 696e 6465  e(columns={"inde
+00025230: 7822 3a20 2244 6174 6522 7d2c 2069 6e70  x": "Date"}, inp
+00025240: 6c61 6365 3d54 7275 6529 0a20 2020 2020  lace=True).     
+00025250: 2020 2020 2020 2064 6174 615b 2274 6f70         data["top
+00025260: 7322 5d20 3d20 2864 6174 615b 2248 6967  s"] = (data["Hig
+00025270: 6822 5d2e 696c 6f63 5b6c 6973 7428 706b  h"].iloc[list(pk
+00025280: 7461 6c69 622e 6172 6772 656c 6578 7472  talib.argrelextr
+00025290: 656d 6128 6e70 2e61 7272 6179 2864 6174  ema(np.array(dat
+000252a0: 615b 2248 6967 6822 5d29 2c20 6e70 2e67  a["High"]), np.g
+000252b0: 7265 6174 6572 5f65 7175 616c 2c20 6f72  reater_equal, or
 000252c0: 6465 723d 7769 6e64 6f77 295b 305d 295d  der=window)[0])]
 000252d0: 2e68 6561 6428 3429 290a 2020 2020 2020  .head(4)).      
-000252e0: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-000252f0: 612e 6669 6c6c 6e61 2830 290a 2020 2020  a.fillna(0).    
-00025300: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-00025310: 6174 612e 7265 706c 6163 6528 5b6e 702e  ata.replace([np.
-00025320: 696e 662c 202d 6e70 2e69 6e66 5d2c 2030  inf, -np.inf], 0
-00025330: 290a 2020 2020 2020 2020 2020 2020 746f  ).            to
-00025340: 7073 203d 2064 6174 615b 6461 7461 2e74  ps = data[data.t
-00025350: 6f70 7320 3e20 305d 0a20 2020 2020 2020  ops > 0].       
-00025360: 2020 2020 2023 2062 6f74 7320 3d20 6461       # bots = da
-00025370: 7461 5b64 6174 612e 626f 7473 203e 2030  ta[data.bots > 0
-00025380: 5d0a 2020 2020 2020 2020 2020 2020 6869  ].            hi
-00025390: 6768 6573 7454 6f70 203d 2072 6f75 6e64  ghestTop = round
-000253a0: 2874 6f70 732e 6465 7363 7269 6265 2829  (tops.describe()
-000253b0: 5b22 4869 6768 225d 5b22 6d61 7822 5d2c  ["High"]["max"],
-000253c0: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
-000253d0: 6669 6c74 6572 6564 546f 7073 203d 2074  filteredTops = t
-000253e0: 6f70 735b 0a20 2020 2020 2020 2020 2020  ops[.           
-000253f0: 2020 2020 2074 6f70 732e 746f 7073 203e       tops.tops >
-00025400: 2028 6869 6768 6573 7454 6f70 202d 2028   (highestTop - (
-00025410: 6869 6768 6573 7454 6f70 202a 2070 6572  highestTop * per
-00025420: 6365 6e74 6167 6546 726f 6d54 6f70 2929  centageFromTop))
-00025430: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
-00025440: 2020 2020 2020 2020 2020 2069 6620 6669             if fi
-00025450: 6c74 6572 6564 546f 7073 2e65 7175 616c  lteredTops.equal
-00025460: 7328 746f 7073 293a 2020 2320 546f 7073  s(tops):  # Tops
-00025470: 2061 7265 2069 6e20 7468 6520 7261 6e67   are in the rang
-00025480: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00025490: 2020 6c6f 7750 6f69 6e74 7320 3d20 5b5d    lowPoints = []
-000254a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000254b0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-000254c0: 6c65 6e28 746f 7073 2920 2d20 3129 3a0a  len(tops) - 1):.
-000254d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000254e0: 2020 2020 656e 6444 6174 6520 3d20 746f      endDate = to
-000254f0: 7073 2e69 6c6f 635b 695d 5b22 4461 7465  ps.iloc[i]["Date
-00025500: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-00025510: 2020 2020 2020 2073 7461 7274 4461 7465         startDate
-00025520: 203d 2074 6f70 732e 696c 6f63 5b69 202b   = tops.iloc[i +
-00025530: 2031 5d5b 2244 6174 6522 5d0a 2020 2020   1]["Date"].    
-00025540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025550: 6c6f 7750 6f69 6e74 732e 6170 7065 6e64  lowPoints.append
-00025560: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00025570: 2020 2020 2020 2020 2020 6461 7461 5b0a            data[.
-00025580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025590: 2020 2020 2020 2020 2020 2020 2864 6174              (dat
-000255a0: 612e 4461 7465 203e 3d20 7374 6172 7444  a.Date >= startD
-000255b0: 6174 6529 2026 2028 6461 7461 2e44 6174  ate) & (data.Dat
-000255c0: 6520 3c3d 2065 6e64 4461 7465 290a 2020  e <= endDate).  
-000255d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000255e0: 2020 2020 2020 5d2e 6465 7363 7269 6265        ].describe
-000255f0: 2829 5b22 4c6f 7722 5d5b 226d 696e 225d  ()["Low"]["min"]
-00025600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025610: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00025620: 2020 2020 2020 206c 6f77 506f 696e 7473         lowPoints
-00025630: 4f72 6720 3d20 6c6f 7750 6f69 6e74 730a  Org = lowPoints.
-00025640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025650: 6c6f 7750 6f69 6e74 732e 736f 7274 2872  lowPoints.sort(r
-00025660: 6576 6572 7365 3d54 7275 6529 0a20 2020  everse=True).   
-00025670: 2020 2020 2020 2020 2020 2020 206c 6f77               low
-00025680: 506f 696e 7473 536f 7274 6564 203d 206c  PointsSorted = l
-00025690: 6f77 506f 696e 7473 0a20 2020 2020 2020  owPoints.       
-000256a0: 2020 2020 2020 2020 2069 6620 6461 7461           if data
-000256b0: 2e65 6d70 7479 206f 7220 6c65 6e28 6c6f  .empty or len(lo
-000256c0: 7750 6f69 6e74 7329 203c 2031 3a0a 2020  wPoints) < 1:.  
-000256d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000256e0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-000256f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00025700: 7470 203d 2064 6174 612e 6865 6164 2831  tp = data.head(1
-00025710: 295b 2243 6c6f 7365 225d 2e69 6c6f 635b  )["Close"].iloc[
-00025720: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
-00025730: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-00025740: 2020 2020 2020 2020 2020 2020 6c6f 7750              lowP
-00025750: 6f69 6e74 734f 7267 203d 3d20 6c6f 7750  ointsOrg == lowP
-00025760: 6f69 6e74 7353 6f72 7465 640a 2020 2020  ointsSorted.    
-00025770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025780: 616e 6420 6c74 7020 3c20 6869 6768 6573  and ltp < highes
-00025790: 7454 6f70 0a20 2020 2020 2020 2020 2020  tTop.           
-000257a0: 2020 2020 2020 2020 2061 6e64 206c 7470           and ltp
-000257b0: 203e 206c 6f77 506f 696e 7473 5b30 5d0a   > lowPoints[0].
-000257c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000257e0: 2020 2020 2020 2073 6176 6564 203d 2073         saved = s
-000257f0: 656c 662e 6669 6e64 4375 7272 656e 7453  elf.findCurrentS
-00025800: 6176 6564 5661 6c75 6528 7363 7265 656e  avedValue(screen
-00025810: 4469 6374 2c20 7361 7665 4469 6374 2c20  Dict, saveDict, 
-00025820: 2250 6174 7465 726e 2229 0a20 2020 2020  "Pattern").     
-00025830: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00025840: 6372 6565 6e44 6963 745b 2250 6174 7465  creenDict["Patte
-00025850: 726e 225d 203d 2028 0a20 2020 2020 2020  rn"] = (.       
+000252e0: 2020 2020 2020 6461 7461 5b22 626f 7473        data["bots
+000252f0: 225d 203d 2028 6461 7461 5b22 4c6f 7722  "] = (data["Low"
+00025300: 5d2e 696c 6f63 5b6c 6973 7428 706b 7461  ].iloc[list(pkta
+00025310: 6c69 622e 6172 6772 656c 6578 7472 656d  lib.argrelextrem
+00025320: 6128 6e70 2e61 7272 6179 2864 6174 615b  a(np.array(data[
+00025330: 224c 6f77 225d 292c 206e 702e 6c65 7373  "Low"]), np.less
+00025340: 5f65 7175 616c 2c20 6f72 6465 723d 7769  _equal, order=wi
+00025350: 6e64 6f77 295b 305d 295d 2e68 6561 6428  ndow)[0])].head(
+00025360: 3429 290a 2020 2020 2020 2020 2020 2020  4)).            
+00025370: 6461 7461 203d 2064 6174 612e 6669 6c6c  data = data.fill
+00025380: 6e61 2830 290a 2020 2020 2020 2020 2020  na(0).          
+00025390: 2020 6461 7461 203d 2064 6174 612e 7265    data = data.re
+000253a0: 706c 6163 6528 5b6e 702e 696e 662c 202d  place([np.inf, -
+000253b0: 6e70 2e69 6e66 5d2c 2030 290a 2020 2020  np.inf], 0).    
+000253c0: 2020 2020 2020 2020 746f 7073 203d 2064          tops = d
+000253d0: 6174 615b 6461 7461 2e74 6f70 7320 3e20  ata[data.tops > 
+000253e0: 305d 0a20 2020 2020 2020 2020 2020 2023  0].            #
+000253f0: 2062 6f74 7320 3d20 6461 7461 5b64 6174   bots = data[dat
+00025400: 612e 626f 7473 203e 2030 5d0a 2020 2020  a.bots > 0].    
+00025410: 2020 2020 2020 2020 6869 6768 6573 7454          highestT
+00025420: 6f70 203d 2072 6f75 6e64 2874 6f70 732e  op = round(tops.
+00025430: 6465 7363 7269 6265 2829 5b22 4869 6768  describe()["High
+00025440: 225d 5b22 6d61 7822 5d2c 2031 290a 2020  "]["max"], 1).  
+00025450: 2020 2020 2020 2020 2020 6669 6c74 6572            filter
+00025460: 6564 546f 7073 203d 2074 6f70 735b 0a20  edTops = tops[. 
+00025470: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00025480: 6f70 732e 746f 7073 203e 2028 6869 6768  ops.tops > (high
+00025490: 6573 7454 6f70 202d 2028 6869 6768 6573  estTop - (highes
+000254a0: 7454 6f70 202a 2070 6572 6365 6e74 6167  tTop * percentag
+000254b0: 6546 726f 6d54 6f70 2929 0a20 2020 2020  eFromTop)).     
+000254c0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+000254d0: 2020 2020 2069 6620 6669 6c74 6572 6564       if filtered
+000254e0: 546f 7073 2e65 7175 616c 7328 746f 7073  Tops.equals(tops
+000254f0: 293a 2020 2320 546f 7073 2061 7265 2069  ):  # Tops are i
+00025500: 6e20 7468 6520 7261 6e67 650a 2020 2020  n the range.    
+00025510: 2020 2020 2020 2020 2020 2020 6c6f 7750              lowP
+00025520: 6f69 6e74 7320 3d20 5b5d 0a20 2020 2020  oints = [].     
+00025530: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+00025540: 2069 6e20 7261 6e67 6528 6c65 6e28 746f   in range(len(to
+00025550: 7073 2920 2d20 3129 3a0a 2020 2020 2020  ps) - 1):.      
+00025560: 2020 2020 2020 2020 2020 2020 2020 656e                en
+00025570: 6444 6174 6520 3d20 746f 7073 2e69 6c6f  dDate = tops.ilo
+00025580: 635b 695d 5b22 4461 7465 225d 0a20 2020  c[i]["Date"].   
+00025590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000255a0: 2073 7461 7274 4461 7465 203d 2074 6f70   startDate = top
+000255b0: 732e 696c 6f63 5b69 202b 2031 5d5b 2244  s.iloc[i + 1]["D
+000255c0: 6174 6522 5d0a 2020 2020 2020 2020 2020  ate"].          
+000255d0: 2020 2020 2020 2020 2020 6c6f 7750 6f69            lowPoi
+000255e0: 6e74 732e 6170 7065 6e64 280a 2020 2020  nts.append(.    
+000255f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025600: 2020 2020 6461 7461 5b0a 2020 2020 2020      data[.      
+00025610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025620: 2020 2020 2020 2864 6174 612e 4461 7465        (data.Date
+00025630: 203e 3d20 7374 6172 7444 6174 6529 2026   >= startDate) &
+00025640: 2028 6461 7461 2e44 6174 6520 3c3d 2065   (data.Date <= e
+00025650: 6e64 4461 7465 290a 2020 2020 2020 2020  ndDate).        
+00025660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025670: 5d2e 6465 7363 7269 6265 2829 5b22 4c6f  ].describe()["Lo
+00025680: 7722 5d5b 226d 696e 225d 0a20 2020 2020  w"]["min"].     
+00025690: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000256a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000256b0: 206c 6f77 506f 696e 7473 4f72 6720 3d20   lowPointsOrg = 
+000256c0: 6c6f 7750 6f69 6e74 730a 2020 2020 2020  lowPoints.      
+000256d0: 2020 2020 2020 2020 2020 6c6f 7750 6f69            lowPoi
+000256e0: 6e74 732e 736f 7274 2872 6576 6572 7365  nts.sort(reverse
+000256f0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+00025700: 2020 2020 2020 206c 6f77 506f 696e 7473         lowPoints
+00025710: 536f 7274 6564 203d 206c 6f77 506f 696e  Sorted = lowPoin
+00025720: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
+00025730: 2020 2069 6620 6461 7461 2e65 6d70 7479     if data.empty
+00025740: 206f 7220 6c65 6e28 6c6f 7750 6f69 6e74   or len(lowPoint
+00025750: 7329 203c 2031 3a0a 2020 2020 2020 2020  s) < 1:.        
+00025760: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00025770: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+00025780: 2020 2020 2020 2020 206c 7470 203d 2064           ltp = d
+00025790: 6174 612e 6865 6164 2831 295b 2243 6c6f  ata.head(1)["Clo
+000257a0: 7365 225d 2e69 6c6f 635b 305d 0a20 2020  se"].iloc[0].   
+000257b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000257c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000257d0: 2020 2020 2020 6c6f 7750 6f69 6e74 734f        lowPointsO
+000257e0: 7267 203d 3d20 6c6f 7750 6f69 6e74 7353  rg == lowPointsS
+000257f0: 6f72 7465 640a 2020 2020 2020 2020 2020  orted.          
+00025800: 2020 2020 2020 2020 2020 616e 6420 6c74            and lt
+00025810: 7020 3c20 6869 6768 6573 7454 6f70 0a20  p < highestTop. 
+00025820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025830: 2020 2061 6e64 206c 7470 203e 206c 6f77     and ltp > low
+00025840: 506f 696e 7473 5b30 5d0a 2020 2020 2020  Points[0].      
+00025850: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
 00025860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025870: 2073 6176 6564 5b30 5d20 0a20 2020 2020   saved[0] .     
-00025880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025890: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
-000258a0: 4f4c 440a 2020 2020 2020 2020 2020 2020  OLD.            
-000258b0: 2020 2020 2020 2020 2020 2020 2b20 636f              + co
-000258c0: 6c6f 7254 6578 742e 4752 4545 4e0a 2020  lorText.GREEN.  
-000258d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000258e0: 2020 2020 2020 2b20 6622 5643 5020 2842        + f"VCP (B
-000258f0: 4f3a 207b 6869 6768 6573 7454 6f70 7d29  O: {highestTop})
-00025900: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00025910: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-00025920: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
-00025930: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00025940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025950: 2020 2020 7361 7665 4469 6374 5b22 5061      saveDict["Pa
-00025960: 7474 6572 6e22 5d20 3d20 7361 7665 645b  ttern"] = saved[
-00025970: 315d 202b 2066 2256 4350 2028 424f 3a20  1] + f"VCP (BO: 
-00025980: 7b68 6967 6865 7374 546f 707d 2922 0a20  {highestTop})". 
+00025870: 2073 6176 6564 203d 2073 656c 662e 6669   saved = self.fi
+00025880: 6e64 4375 7272 656e 7453 6176 6564 5661  ndCurrentSavedVa
+00025890: 6c75 6528 7363 7265 656e 4469 6374 2c20  lue(screenDict, 
+000258a0: 7361 7665 4469 6374 2c20 2250 6174 7465  saveDict, "Patte
+000258b0: 726e 2229 0a20 2020 2020 2020 2020 2020  rn").           
+000258c0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+000258d0: 6963 745b 2250 6174 7465 726e 225d 203d  ict["Pattern"] =
+000258e0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+000258f0: 2020 2020 2020 2020 2020 2073 6176 6564             saved
+00025900: 5b30 5d20 0a20 2020 2020 2020 2020 2020  [0] .           
+00025910: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+00025920: 6f6c 6f72 5465 7874 2e42 4f4c 440a 2020  olorText.BOLD.  
+00025930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025940: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
+00025950: 742e 4752 4545 4e0a 2020 2020 2020 2020  t.GREEN.        
+00025960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025970: 2b20 6622 5643 5020 2842 4f3a 207b 6869  + f"VCP (BO: {hi
+00025980: 6768 6573 7454 6f70 7d29 220a 2020 2020  ghestTop})".    
 00025990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000259a0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-000259b0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-000259c0: 6365 7074 696f 6e20 6173 2065 3a20 2023  ception as e:  #
-000259d0: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
-000259e0: 720a 2020 2020 2020 2020 2020 2020 7365  r.            se
-000259f0: 6c66 2e64 6566 6175 6c74 5f6c 6f67 6765  lf.default_logge
-00025a00: 722e 6465 6275 6728 652c 2065 7863 5f69  r.debug(e, exc_i
-00025a10: 6e66 6f3d 5472 7565 290a 2020 2020 2020  nfo=True).      
-00025a20: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-00025a30: 2020 2020 2320 5661 6c69 6461 7465 2069      # Validate i
-00025a40: 6620 766f 6c75 6d65 206f 6620 6c61 7374  f volume of last
-00025a50: 2064 6179 2069 7320 6869 6768 6572 2074   day is higher t
-00025a60: 6861 6e20 6176 670a 2020 2020 6465 6620  han avg.    def 
-00025a70: 7661 6c69 6461 7465 566f 6c75 6d65 280a  validateVolume(.
-00025a80: 2020 2020 2020 2020 7365 6c66 2c20 6466          self, df
-00025a90: 2c20 7363 7265 656e 4469 6374 2c20 7361  , screenDict, sa
-00025aa0: 7665 4469 6374 2c20 766f 6c75 6d65 5261  veDict, volumeRa
-00025ab0: 7469 6f3d 322e 352c 206d 696e 566f 6c75  tio=2.5, minVolu
-00025ac0: 6d65 3d31 3030 0a20 2020 2029 3a0a 2020  me=100.    ):.  
-00025ad0: 2020 2020 2020 6966 2064 6620 6973 204e        if df is N
-00025ae0: 6f6e 6520 6f72 206c 656e 2864 6629 203d  one or len(df) =
-00025af0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00025b00: 2072 6574 7572 6e20 4661 6c73 652c 2046   return False, F
-00025b10: 616c 7365 0a20 2020 2020 2020 2064 6174  alse.        dat
-00025b20: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
-00025b30: 2020 2020 2020 6461 7461 203d 2064 6174        data = dat
-00025b40: 612e 6669 6c6c 6e61 2830 290a 2020 2020  a.fillna(0).    
-00025b50: 2020 2020 6461 7461 203d 2064 6174 612e      data = data.
-00025b60: 7265 706c 6163 6528 5b6e 702e 696e 662c  replace([np.inf,
-00025b70: 202d 6e70 2e69 6e66 5d2c 2030 290a 2020   -np.inf], 0).  
-00025b80: 2020 2020 2020 7265 6365 6e74 203d 2064        recent = d
-00025b90: 6174 612e 6865 6164 2831 290a 2020 2020  ata.head(1).    
-00025ba0: 2020 2020 2320 4569 7468 6572 2074 6865      # Either the
-00025bb0: 2072 6f6c 6c69 6e67 2076 6f6c 756d 6520   rolling volume 
-00025bc0: 6f66 2070 6173 7420 3230 2073 6573 7369  of past 20 sessi
-00025bd0: 6f6e 7320 6f72 2074 6f64 6179 2773 2076  ons or today's v
-00025be0: 6f6c 756d 6520 7368 6f75 6c64 2062 6520  olume should be 
-00025bf0: 3e20 6d69 6e20 766f 6c75 6d65 0a20 2020  > min volume.   
-00025c00: 2020 2020 2068 6173 4d69 6e69 6d75 6d56       hasMinimumV
-00025c10: 6f6c 756d 6520 3d20 280a 2020 2020 2020  olume = (.      
-00025c20: 2020 2020 2020 7265 6365 6e74 5b22 566f        recent["Vo
-00025c30: 6c4d 4122 5d2e 696c 6f63 5b30 5d20 3e3d  lMA"].iloc[0] >=
-00025c40: 206d 696e 566f 6c75 6d65 0a20 2020 2020   minVolume.     
-00025c50: 2020 2020 2020 206f 7220 7265 6365 6e74         or recent
-00025c60: 5b22 566f 6c75 6d65 225d 2e69 6c6f 635b  ["Volume"].iloc[
-00025c70: 305d 203e 3d20 6d69 6e56 6f6c 756d 650a  0] >= minVolume.
-00025c80: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00025c90: 2020 6966 2072 6563 656e 745b 2256 6f6c    if recent["Vol
-00025ca0: 4d41 225d 2e69 6c6f 635b 305d 203d 3d20  MA"].iloc[0] == 
-00025cb0: 303a 2020 2320 4861 6e64 6c65 7320 4469  0:  # Handles Di
-00025cc0: 7669 6465 2062 7920 3020 7761 726e 696e  vide by 0 warnin
-00025cd0: 670a 2020 2020 2020 2020 2020 2020 7361  g.            sa
-00025ce0: 7665 4469 6374 5b22 566f 6c75 6d65 225d  veDict["Volume"]
-00025cf0: 203d 2030 2020 2320 2255 6e6b 6e6f 776e   = 0  # "Unknown
-00025d00: 220a 2020 2020 2020 2020 2020 2020 7363  ".            sc
-00025d10: 7265 656e 4469 6374 5b22 566f 6c75 6d65  reenDict["Volume
-00025d20: 225d 203d 2030 0a20 2020 2020 2020 2020  "] = 0.         
-00025d30: 2020 2072 6574 7572 6e20 4661 6c73 652c     return False,
-00025d40: 2068 6173 4d69 6e69 6d75 6d56 6f6c 756d   hasMinimumVolum
-00025d50: 650a 2020 2020 2020 2020 7261 7469 6f20  e.        ratio 
-00025d60: 3d20 726f 756e 6428 7265 6365 6e74 5b22  = round(recent["
-00025d70: 566f 6c75 6d65 225d 2e69 6c6f 635b 305d  Volume"].iloc[0]
-00025d80: 202f 2072 6563 656e 745b 2256 6f6c 4d41   / recent["VolMA
-00025d90: 225d 2e69 6c6f 635b 305d 2c20 3229 0a20  "].iloc[0], 2). 
-00025da0: 2020 2020 2020 2073 6176 6544 6963 745b         saveDict[
-00025db0: 2256 6f6c 756d 6522 5d20 3d20 7261 7469  "Volume"] = rati
-00025dc0: 6f0a 2020 2020 2020 2020 6966 2072 6174  o.        if rat
-00025dd0: 696f 203e 3d20 766f 6c75 6d65 5261 7469  io >= volumeRati
-00025de0: 6f20 616e 6420 7261 7469 6f20 213d 206e  o and ratio != n
-00025df0: 702e 6e61 6e20 616e 6420 286e 6f74 206d  p.nan and (not m
-00025e00: 6174 682e 6973 696e 6628 7261 7469 6f29  ath.isinf(ratio)
-00025e10: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00025e20: 6372 6565 6e44 6963 745b 2256 6f6c 756d  creenDict["Volum
-00025e30: 6522 5d20 3d20 7261 7469 6f0a 2020 2020  e"] = ratio.    
-00025e40: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00025e50: 7275 652c 2068 6173 4d69 6e69 6d75 6d56  rue, hasMinimumV
-00025e60: 6f6c 756d 650a 2020 2020 2020 2020 7363  olume.        sc
-00025e70: 7265 656e 4469 6374 5b22 566f 6c75 6d65  reenDict["Volume
-00025e80: 225d 203d 2072 6174 696f 0a20 2020 2020  "] = ratio.     
-00025e90: 2020 2072 6574 7572 6e20 4661 6c73 652c     return False,
-00025ea0: 2068 6173 4d69 6e69 6d75 6d56 6f6c 756d   hasMinimumVolum
-00025eb0: 650a 0a20 2020 2023 2046 696e 6420 6966  e..    # Find if
-00025ec0: 2073 746f 636b 2069 7320 7661 6c69 6461   stock is valida
-00025ed0: 7469 6e67 2076 6f6c 756d 6520 7370 7265  ting volume spre
-00025ee0: 6164 2061 6e61 6c79 7369 730a 2020 2020  ad analysis.    
-00025ef0: 6465 6620 7661 6c69 6461 7465 566f 6c75  def validateVolu
-00025f00: 6d65 5370 7265 6164 416e 616c 7973 6973  meSpreadAnalysis
-00025f10: 2873 656c 662c 2064 662c 2073 6372 6565  (self, df, scree
-00025f20: 6e44 6963 742c 2073 6176 6544 6963 7429  nDict, saveDict)
-00025f30: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
-00025f40: 2020 2020 2020 2020 2020 2069 6620 6466             if df
-00025f50: 2069 7320 4e6f 6e65 206f 7220 6c65 6e28   is None or len(
-00025f60: 6466 2920 3d3d 2030 3a0a 2020 2020 2020  df) == 0:.      
-00025f70: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00025f80: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00025f90: 2020 2064 6174 6120 3d20 6466 2e63 6f70     data = df.cop
-00025fa0: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-00025fb0: 6461 7461 203d 2064 6174 612e 6865 6164  data = data.head
-00025fc0: 2832 290a 2020 2020 2020 2020 2020 2020  (2).            
-00025fd0: 6966 206c 656e 2864 6174 6129 203c 2032  if len(data) < 2
-00025fe0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00025ff0: 2020 7265 7475 726e 2046 616c 7365 0a20    return False. 
-00026000: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-00026010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026020: 2320 4368 6563 6b20 666f 7220 7072 6576  # Check for prev
-00026030: 696f 7573 2052 4544 2063 616e 646c 6573  ious RED candles
-00026040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026050: 2023 2043 7572 7265 6e74 2063 616e 646c   # Current candl
-00026060: 6520 3d20 3074 682c 2050 7265 7669 6f75  e = 0th, Previou
-00026070: 7320 4361 6e64 6c65 203d 2031 7374 2066  s Candle = 1st f
-00026080: 6f72 2066 6f6c 6c6f 7769 6e67 206c 6f67  or following log
-00026090: 6963 0a20 2020 2020 2020 2020 2020 2020  ic.             
-000260a0: 2020 2069 6620 6461 7461 2e69 6c6f 635b     if data.iloc[
-000260b0: 315d 5b22 4f70 656e 225d 203e 3d20 6461  1]["Open"] >= da
-000260c0: 7461 2e69 6c6f 635b 315d 5b22 436c 6f73  ta.iloc[1]["Clos
-000260d0: 6522 5d3a 0a20 2020 2020 2020 2020 2020  e"]:.           
-000260e0: 2020 2020 2020 2020 2073 7072 6561 6431           spread1
-000260f0: 203d 2061 6273 2864 6174 612e 696c 6f63   = abs(data.iloc
-00026100: 5b31 5d5b 224f 7065 6e22 5d20 2d20 6461  [1]["Open"] - da
-00026110: 7461 2e69 6c6f 635b 315d 5b22 436c 6f73  ta.iloc[1]["Clos
-00026120: 6522 5d29 0a20 2020 2020 2020 2020 2020  e"]).           
-00026130: 2020 2020 2020 2020 2073 7072 6561 6430           spread0
-00026140: 203d 2061 6273 2864 6174 612e 696c 6f63   = abs(data.iloc
-00026150: 5b30 5d5b 224f 7065 6e22 5d20 2d20 6461  [0]["Open"] - da
-00026160: 7461 2e69 6c6f 635b 305d 5b22 436c 6f73  ta.iloc[0]["Clos
-00026170: 6522 5d29 0a20 2020 2020 2020 2020 2020  e"]).           
-00026180: 2020 2020 2020 2020 206c 6f77 6572 5f77           lower_w
-00026190: 6963 6b5f 7370 7265 6164 3020 3d20 280a  ick_spread0 = (.
-000261a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000261b0: 2020 2020 2020 2020 6d61 7828 6461 7461          max(data
-000261c0: 2e69 6c6f 635b 305d 5b22 4f70 656e 225d  .iloc[0]["Open"]
-000261d0: 2c20 6461 7461 2e69 6c6f 635b 305d 5b22  , data.iloc[0]["
-000261e0: 436c 6f73 6522 5d29 0a20 2020 2020 2020  Close"]).       
-000261f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026200: 202d 2064 6174 612e 696c 6f63 5b30 5d5b   - data.iloc[0][
-00026210: 224c 6f77 225d 0a20 2020 2020 2020 2020  "Low"].         
-00026220: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000259a0: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+000259b0: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
+000259c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000259d0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
+000259e0: 7665 4469 6374 5b22 5061 7474 6572 6e22  veDict["Pattern"
+000259f0: 5d20 3d20 7361 7665 645b 315d 202b 2066  ] = saved[1] + f
+00025a00: 2256 4350 2028 424f 3a20 7b68 6967 6865  "VCP (BO: {highe
+00025a10: 7374 546f 707d 2922 0a20 2020 2020 2020  stTop})".       
+00025a20: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00025a30: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+00025a40: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00025a50: 6e20 6173 2065 3a20 2023 2070 7261 676d  n as e:  # pragm
+00025a60: 613a 206e 6f20 636f 7665 720a 2020 2020  a: no cover.    
+00025a70: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
+00025a80: 6175 6c74 5f6c 6f67 6765 722e 6465 6275  ault_logger.debu
+00025a90: 6728 652c 2065 7863 5f69 6e66 6f3d 5472  g(e, exc_info=Tr
+00025aa0: 7565 290a 2020 2020 2020 2020 7265 7475  ue).        retu
+00025ab0: 726e 2046 616c 7365 0a0a 2020 2020 2320  rn False..    # 
+00025ac0: 5661 6c69 6461 7465 2069 6620 766f 6c75  Validate if volu
+00025ad0: 6d65 206f 6620 6c61 7374 2064 6179 2069  me of last day i
+00025ae0: 7320 6869 6768 6572 2074 6861 6e20 6176  s higher than av
+00025af0: 670a 2020 2020 6465 6620 7661 6c69 6461  g.    def valida
+00025b00: 7465 566f 6c75 6d65 280a 2020 2020 2020  teVolume(.      
+00025b10: 2020 7365 6c66 2c20 6466 2c20 7363 7265    self, df, scre
+00025b20: 656e 4469 6374 2c20 7361 7665 4469 6374  enDict, saveDict
+00025b30: 2c20 766f 6c75 6d65 5261 7469 6f3d 322e  , volumeRatio=2.
+00025b40: 352c 206d 696e 566f 6c75 6d65 3d31 3030  5, minVolume=100
+00025b50: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00025b60: 6966 2064 6620 6973 204e 6f6e 6520 6f72  if df is None or
+00025b70: 206c 656e 2864 6629 203d 3d20 303a 0a20   len(df) == 0:. 
+00025b80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00025b90: 6e20 4661 6c73 652c 2046 616c 7365 0a20  n False, False. 
+00025ba0: 2020 2020 2020 2064 6174 6120 3d20 6466         data = df
+00025bb0: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
+00025bc0: 6461 7461 203d 2064 6174 612e 6669 6c6c  data = data.fill
+00025bd0: 6e61 2830 290a 2020 2020 2020 2020 6461  na(0).        da
+00025be0: 7461 203d 2064 6174 612e 7265 706c 6163  ta = data.replac
+00025bf0: 6528 5b6e 702e 696e 662c 202d 6e70 2e69  e([np.inf, -np.i
+00025c00: 6e66 5d2c 2030 290a 2020 2020 2020 2020  nf], 0).        
+00025c10: 7265 6365 6e74 203d 2064 6174 612e 6865  recent = data.he
+00025c20: 6164 2831 290a 2020 2020 2020 2020 2320  ad(1).        # 
+00025c30: 4569 7468 6572 2074 6865 2072 6f6c 6c69  Either the rolli
+00025c40: 6e67 2076 6f6c 756d 6520 6f66 2070 6173  ng volume of pas
+00025c50: 7420 3230 2073 6573 7369 6f6e 7320 6f72  t 20 sessions or
+00025c60: 2074 6f64 6179 2773 2076 6f6c 756d 6520   today's volume 
+00025c70: 7368 6f75 6c64 2062 6520 3e20 6d69 6e20  should be > min 
+00025c80: 766f 6c75 6d65 0a20 2020 2020 2020 2068  volume.        h
+00025c90: 6173 4d69 6e69 6d75 6d56 6f6c 756d 6520  asMinimumVolume 
+00025ca0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00025cb0: 7265 6365 6e74 5b22 566f 6c4d 4122 5d2e  recent["VolMA"].
+00025cc0: 696c 6f63 5b30 5d20 3e3d 206d 696e 566f  iloc[0] >= minVo
+00025cd0: 6c75 6d65 0a20 2020 2020 2020 2020 2020  lume.           
+00025ce0: 206f 7220 7265 6365 6e74 5b22 566f 6c75   or recent["Volu
+00025cf0: 6d65 225d 2e69 6c6f 635b 305d 203e 3d20  me"].iloc[0] >= 
+00025d00: 6d69 6e56 6f6c 756d 650a 2020 2020 2020  minVolume.      
+00025d10: 2020 290a 2020 2020 2020 2020 6966 2072    ).        if r
+00025d20: 6563 656e 745b 2256 6f6c 4d41 225d 2e69  ecent["VolMA"].i
+00025d30: 6c6f 635b 305d 203d 3d20 303a 2020 2320  loc[0] == 0:  # 
+00025d40: 4861 6e64 6c65 7320 4469 7669 6465 2062  Handles Divide b
+00025d50: 7920 3020 7761 726e 696e 670a 2020 2020  y 0 warning.    
+00025d60: 2020 2020 2020 2020 7361 7665 4469 6374          saveDict
+00025d70: 5b22 566f 6c75 6d65 225d 203d 2030 2020  ["Volume"] = 0  
+00025d80: 2320 2255 6e6b 6e6f 776e 220a 2020 2020  # "Unknown".    
+00025d90: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+00025da0: 6374 5b22 566f 6c75 6d65 225d 203d 2030  ct["Volume"] = 0
+00025db0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00025dc0: 7572 6e20 4661 6c73 652c 2068 6173 4d69  urn False, hasMi
+00025dd0: 6e69 6d75 6d56 6f6c 756d 650a 2020 2020  nimumVolume.    
+00025de0: 2020 2020 7261 7469 6f20 3d20 726f 756e      ratio = roun
+00025df0: 6428 7265 6365 6e74 5b22 566f 6c75 6d65  d(recent["Volume
+00025e00: 225d 2e69 6c6f 635b 305d 202f 2072 6563  "].iloc[0] / rec
+00025e10: 656e 745b 2256 6f6c 4d41 225d 2e69 6c6f  ent["VolMA"].ilo
+00025e20: 635b 305d 2c20 3229 0a20 2020 2020 2020  c[0], 2).       
+00025e30: 2073 6176 6544 6963 745b 2256 6f6c 756d   saveDict["Volum
+00025e40: 6522 5d20 3d20 7261 7469 6f0a 2020 2020  e"] = ratio.    
+00025e50: 2020 2020 6966 2072 6174 696f 203e 3d20      if ratio >= 
+00025e60: 766f 6c75 6d65 5261 7469 6f20 616e 6420  volumeRatio and 
+00025e70: 7261 7469 6f20 213d 206e 702e 6e61 6e20  ratio != np.nan 
+00025e80: 616e 6420 286e 6f74 206d 6174 682e 6973  and (not math.is
+00025e90: 696e 6628 7261 7469 6f29 293a 0a20 2020  inf(ratio)):.   
+00025ea0: 2020 2020 2020 2020 2073 6372 6565 6e44           screenD
+00025eb0: 6963 745b 2256 6f6c 756d 6522 5d20 3d20  ict["Volume"] = 
+00025ec0: 7261 7469 6f0a 2020 2020 2020 2020 2020  ratio.          
+00025ed0: 2020 7265 7475 726e 2054 7275 652c 2068    return True, h
+00025ee0: 6173 4d69 6e69 6d75 6d56 6f6c 756d 650a  asMinimumVolume.
+00025ef0: 2020 2020 2020 2020 7363 7265 656e 4469          screenDi
+00025f00: 6374 5b22 566f 6c75 6d65 225d 203d 2072  ct["Volume"] = r
+00025f10: 6174 696f 0a20 2020 2020 2020 2072 6574  atio.        ret
+00025f20: 7572 6e20 4661 6c73 652c 2068 6173 4d69  urn False, hasMi
+00025f30: 6e69 6d75 6d56 6f6c 756d 650a 0a20 2020  nimumVolume..   
+00025f40: 2023 2046 696e 6420 6966 2073 746f 636b   # Find if stock
+00025f50: 2069 7320 7661 6c69 6461 7469 6e67 2076   is validating v
+00025f60: 6f6c 756d 6520 7370 7265 6164 2061 6e61  olume spread ana
+00025f70: 6c79 7369 730a 2020 2020 6465 6620 7661  lysis.    def va
+00025f80: 6c69 6461 7465 566f 6c75 6d65 5370 7265  lidateVolumeSpre
+00025f90: 6164 416e 616c 7973 6973 2873 656c 662c  adAnalysis(self,
+00025fa0: 2064 662c 2073 6372 6565 6e44 6963 742c   df, screenDict,
+00025fb0: 2073 6176 6544 6963 7429 3a0a 2020 2020   saveDict):.    
+00025fc0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00025fd0: 2020 2020 2069 6620 6466 2069 7320 4e6f       if df is No
+00025fe0: 6e65 206f 7220 6c65 6e28 6466 2920 3d3d  ne or len(df) ==
+00025ff0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00026000: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+00026010: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00026020: 6120 3d20 6466 2e63 6f70 7928 290a 2020  a = df.copy().  
+00026030: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+00026040: 2064 6174 612e 6865 6164 2832 290a 2020   data.head(2).  
+00026050: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00026060: 2864 6174 6129 203c 2032 3a0a 2020 2020  (data) < 2:.    
+00026070: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00026080: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+00026090: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000260a0: 2020 2020 2020 2020 2020 2320 4368 6563            # Chec
+000260b0: 6b20 666f 7220 7072 6576 696f 7573 2052  k for previous R
+000260c0: 4544 2063 616e 646c 6573 0a20 2020 2020  ED candles.     
+000260d0: 2020 2020 2020 2020 2020 2023 2043 7572             # Cur
+000260e0: 7265 6e74 2063 616e 646c 6520 3d20 3074  rent candle = 0t
+000260f0: 682c 2050 7265 7669 6f75 7320 4361 6e64  h, Previous Cand
+00026100: 6c65 203d 2031 7374 2066 6f72 2066 6f6c  le = 1st for fol
+00026110: 6c6f 7769 6e67 206c 6f67 6963 0a20 2020  lowing logic.   
+00026120: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00026130: 6461 7461 2e69 6c6f 635b 315d 5b22 4f70  data.iloc[1]["Op
+00026140: 656e 225d 203e 3d20 6461 7461 2e69 6c6f  en"] >= data.ilo
+00026150: 635b 315d 5b22 436c 6f73 6522 5d3a 0a20  c[1]["Close"]:. 
+00026160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026170: 2020 2073 7072 6561 6431 203d 2061 6273     spread1 = abs
+00026180: 2864 6174 612e 696c 6f63 5b31 5d5b 224f  (data.iloc[1]["O
+00026190: 7065 6e22 5d20 2d20 6461 7461 2e69 6c6f  pen"] - data.ilo
+000261a0: 635b 315d 5b22 436c 6f73 6522 5d29 0a20  c[1]["Close"]). 
+000261b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000261c0: 2020 2073 7072 6561 6430 203d 2061 6273     spread0 = abs
+000261d0: 2864 6174 612e 696c 6f63 5b30 5d5b 224f  (data.iloc[0]["O
+000261e0: 7065 6e22 5d20 2d20 6461 7461 2e69 6c6f  pen"] - data.ilo
+000261f0: 635b 305d 5b22 436c 6f73 6522 5d29 0a20  c[0]["Close"]). 
+00026200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026210: 2020 206c 6f77 6572 5f77 6963 6b5f 7370     lower_wick_sp
+00026220: 7265 6164 3020 3d20 280a 2020 2020 2020  read0 = (.      
 00026230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026240: 2076 6f6c 3120 3d20 6461 7461 2e69 6c6f   vol1 = data.ilo
-00026250: 635b 315d 5b22 566f 6c75 6d65 225d 0a20  c[1]["Volume"]. 
-00026260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026270: 2020 2076 6f6c 3020 3d20 6461 7461 2e69     vol0 = data.i
-00026280: 6c6f 635b 305d 5b22 566f 6c75 6d65 225d  loc[0]["Volume"]
-00026290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000262a0: 2020 2020 2073 6176 6564 203d 2073 656c       saved = sel
-000262b0: 662e 6669 6e64 4375 7272 656e 7453 6176  f.findCurrentSav
-000262c0: 6564 5661 6c75 6528 7363 7265 656e 4469  edValue(screenDi
-000262d0: 6374 2c20 7361 7665 4469 6374 2c20 2250  ct, saveDict, "P
-000262e0: 6174 7465 726e 2229 0a20 2020 2020 2020  attern").       
-000262f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00026300: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00026310: 2020 2020 2020 2020 2020 7370 7265 6164            spread
-00026320: 3020 3e20 7370 7265 6164 310a 2020 2020  0 > spread1.    
-00026330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026340: 2020 2020 616e 6420 766f 6c30 203c 2076      and vol0 < v
-00026350: 6f6c 310a 2020 2020 2020 2020 2020 2020  ol1.            
-00026360: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00026370: 6461 7461 2e69 6c6f 635b 305d 5b22 566f  data.iloc[0]["Vo
-00026380: 6c75 6d65 225d 203c 2064 6174 612e 696c  lume"] < data.il
-00026390: 6f63 5b30 5d5b 2256 6f6c 4d41 225d 0a20  oc[0]["VolMA"]. 
-000263a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000263b0: 2020 2020 2020 2061 6e64 2064 6174 612e         and data.
-000263c0: 696c 6f63 5b30 5d5b 2243 6c6f 7365 225d  iloc[0]["Close"]
-000263d0: 203c 3d20 6461 7461 2e69 6c6f 635b 315d   <= data.iloc[1]
-000263e0: 5b22 4f70 656e 225d 0a20 2020 2020 2020  ["Open"].       
-000263f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026400: 2061 6e64 2073 7072 6561 6430 203c 206c   and spread0 < l
-00026410: 6f77 6572 5f77 6963 6b5f 7370 7265 6164  ower_wick_spread
-00026420: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-00026430: 2020 2020 2020 2020 2020 616e 6420 6461            and da
-00026440: 7461 2e69 6c6f 635b 305d 5b22 566f 6c75  ta.iloc[0]["Volu
-00026450: 6d65 225d 203c 3d20 696e 7428 6461 7461  me"] <= int(data
-00026460: 2e69 6c6f 635b 315d 5b22 566f 6c75 6d65  .iloc[1]["Volume
-00026470: 225d 202a 2030 2e37 3529 0a20 2020 2020  "] * 0.75).     
-00026480: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00026490: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000264a0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-000264b0: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-000264c0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-000264d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000264e0: 7361 7665 645b 305d 200a 2020 2020 2020  saved[0] .      
-000264f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026500: 2020 2020 2020 2b20 636f 6c6f 7254 6578        + colorTex
-00026510: 742e 424f 4c44 0a20 2020 2020 2020 2020  t.BOLD.         
+00026240: 2020 6d61 7828 6461 7461 2e69 6c6f 635b    max(data.iloc[
+00026250: 305d 5b22 4f70 656e 225d 2c20 6461 7461  0]["Open"], data
+00026260: 2e69 6c6f 635b 305d 5b22 436c 6f73 6522  .iloc[0]["Close"
+00026270: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00026280: 2020 2020 2020 2020 2020 202d 2064 6174             - dat
+00026290: 612e 696c 6f63 5b30 5d5b 224c 6f77 225d  a.iloc[0]["Low"]
+000262a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000262b0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000262c0: 2020 2020 2020 2020 2020 2076 6f6c 3120             vol1 
+000262d0: 3d20 6461 7461 2e69 6c6f 635b 315d 5b22  = data.iloc[1]["
+000262e0: 566f 6c75 6d65 225d 0a20 2020 2020 2020  Volume"].       
+000262f0: 2020 2020 2020 2020 2020 2020 2076 6f6c               vol
+00026300: 3020 3d20 6461 7461 2e69 6c6f 635b 305d  0 = data.iloc[0]
+00026310: 5b22 566f 6c75 6d65 225d 0a20 2020 2020  ["Volume"].     
+00026320: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00026330: 6176 6564 203d 2073 656c 662e 6669 6e64  aved = self.find
+00026340: 4375 7272 656e 7453 6176 6564 5661 6c75  CurrentSavedValu
+00026350: 6528 7363 7265 656e 4469 6374 2c20 7361  e(screenDict, sa
+00026360: 7665 4469 6374 2c20 2250 6174 7465 726e  veDict, "Pattern
+00026370: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00026380: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
+00026390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000263a0: 2020 2020 7370 7265 6164 3020 3e20 7370      spread0 > sp
+000263b0: 7265 6164 310a 2020 2020 2020 2020 2020  read1.          
+000263c0: 2020 2020 2020 2020 2020 2020 2020 616e                an
+000263d0: 6420 766f 6c30 203c 2076 6f6c 310a 2020  d vol0 < vol1.  
+000263e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000263f0: 2020 2020 2020 616e 6420 6461 7461 2e69        and data.i
+00026400: 6c6f 635b 305d 5b22 566f 6c75 6d65 225d  loc[0]["Volume"]
+00026410: 203c 2064 6174 612e 696c 6f63 5b30 5d5b   < data.iloc[0][
+00026420: 2256 6f6c 4d41 225d 0a20 2020 2020 2020  "VolMA"].       
+00026430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026440: 2061 6e64 2064 6174 612e 696c 6f63 5b30   and data.iloc[0
+00026450: 5d5b 2243 6c6f 7365 225d 203c 3d20 6461  ]["Close"] <= da
+00026460: 7461 2e69 6c6f 635b 315d 5b22 4f70 656e  ta.iloc[1]["Open
+00026470: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00026480: 2020 2020 2020 2020 2020 2061 6e64 2073             and s
+00026490: 7072 6561 6430 203c 206c 6f77 6572 5f77  pread0 < lower_w
+000264a0: 6963 6b5f 7370 7265 6164 300a 2020 2020  ick_spread0.    
+000264b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000264c0: 2020 2020 616e 6420 6461 7461 2e69 6c6f      and data.ilo
+000264d0: 635b 305d 5b22 566f 6c75 6d65 225d 203c  c[0]["Volume"] <
+000264e0: 3d20 696e 7428 6461 7461 2e69 6c6f 635b  = int(data.iloc[
+000264f0: 315d 5b22 566f 6c75 6d65 225d 202a 2030  1]["Volume"] * 0
+00026500: 2e37 3529 0a20 2020 2020 2020 2020 2020  .75).           
+00026510: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
 00026520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026530: 2020 202b 2063 6f6c 6f72 5465 7874 2e47     + colorText.G
-00026540: 5245 454e 0a20 2020 2020 2020 2020 2020  REEN.           
+00026530: 2020 2020 7363 7265 656e 4469 6374 5b22      screenDict["
+00026540: 5061 7474 6572 6e22 5d20 3d20 280a 2020  Pattern"] = (.  
 00026550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026560: 202b 2022 5375 7070 6c79 2044 726f 7567   + "Supply Droug
-00026570: 6874 220a 2020 2020 2020 2020 2020 2020  ht".            
+00026560: 2020 2020 2020 2020 2020 7361 7665 645b            saved[
+00026570: 305d 200a 2020 2020 2020 2020 2020 2020  0] .            
 00026580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026590: 2b20 636f 6c6f 7254 6578 742e 454e 440a  + colorText.END.
-000265a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000265b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000265c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000265d0: 2020 7361 7665 4469 6374 5b22 5061 7474    saveDict["Patt
-000265e0: 6572 6e22 5d20 3d20 7361 7665 645b 315d  ern"] = saved[1]
-000265f0: 202b 2022 5375 7070 6c79 2044 726f 7567   + "Supply Droug
-00026600: 6874 220a 2020 2020 2020 2020 2020 2020  ht".            
-00026610: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00026620: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-00026630: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00026640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026650: 2020 2020 2020 2020 2073 7072 6561 6430           spread0
-00026660: 203c 2073 7072 6561 6431 0a20 2020 2020   < spread1.     
-00026670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026680: 2020 2061 6e64 2076 6f6c 3020 3e20 766f     and vol0 > vo
-00026690: 6c31 0a20 2020 2020 2020 2020 2020 2020  l1.             
-000266a0: 2020 2020 2020 2020 2020 2061 6e64 2064             and d
-000266b0: 6174 612e 696c 6f63 5b30 5d5b 2256 6f6c  ata.iloc[0]["Vol
-000266c0: 756d 6522 5d20 3e20 6461 7461 2e69 6c6f  ume"] > data.ilo
-000266d0: 635b 305d 5b22 566f 6c4d 4122 5d0a 2020  c[0]["VolMA"].  
-000266e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000266f0: 2020 2020 2020 616e 6420 6461 7461 2e69        and data.i
-00026700: 6c6f 635b 305d 5b22 436c 6f73 6522 5d20  loc[0]["Close"] 
-00026710: 3c3d 2064 6174 612e 696c 6f63 5b31 5d5b  <= data.iloc[1][
-00026720: 224f 7065 6e22 5d0a 2020 2020 2020 2020  "Open"].        
-00026730: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
-00026740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026750: 2020 2020 2020 2073 6372 6565 6e44 6963         screenDic
-00026760: 745b 2250 6174 7465 726e 225d 203d 2028  t["Pattern"] = (
-00026770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026780: 2020 2020 2020 2020 2020 2020 2073 6176               sav
-00026790: 6564 5b30 5d20 0a20 2020 2020 2020 2020  ed[0] .         
-000267a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000267b0: 2020 202b 2063 6f6c 6f72 5465 7874 2e42     + colorText.B
-000267c0: 4f4c 440a 2020 2020 2020 2020 2020 2020  OLD.            
+00026590: 2b20 636f 6c6f 7254 6578 742e 424f 4c44  + colorText.BOLD
+000265a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000265b0: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+000265c0: 6f6c 6f72 5465 7874 2e47 5245 454e 0a20  olorText.GREEN. 
+000265d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000265e0: 2020 2020 2020 2020 2020 202b 2022 5375             + "Su
+000265f0: 7070 6c79 2044 726f 7567 6874 220a 2020  pply Drought".  
+00026600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026610: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+00026620: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+00026630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026640: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00026650: 2020 2020 2020 2020 2020 2020 7361 7665              save
+00026660: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
+00026670: 3d20 7361 7665 645b 315d 202b 2022 5375  = saved[1] + "Su
+00026680: 7070 6c79 2044 726f 7567 6874 220a 2020  pply Drought".  
+00026690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000266a0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+000266b0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000266c0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+000266d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000266e0: 2020 2073 7072 6561 6430 203c 2073 7072     spread0 < spr
+000266f0: 6561 6431 0a20 2020 2020 2020 2020 2020  ead1.           
+00026700: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00026710: 2076 6f6c 3020 3e20 766f 6c31 0a20 2020   vol0 > vol1.   
+00026720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026730: 2020 2020 2061 6e64 2064 6174 612e 696c       and data.il
+00026740: 6f63 5b30 5d5b 2256 6f6c 756d 6522 5d20  oc[0]["Volume"] 
+00026750: 3e20 6461 7461 2e69 6c6f 635b 305d 5b22  > data.iloc[0]["
+00026760: 566f 6c4d 4122 5d0a 2020 2020 2020 2020  VolMA"].        
+00026770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026780: 616e 6420 6461 7461 2e69 6c6f 635b 305d  and data.iloc[0]
+00026790: 5b22 436c 6f73 6522 5d20 3c3d 2064 6174  ["Close"] <= dat
+000267a0: 612e 696c 6f63 5b31 5d5b 224f 7065 6e22  a.iloc[1]["Open"
+000267b0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000267c0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
 000267d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000267e0: 2b20 636f 6c6f 7254 6578 742e 4752 4545  + colorText.GREE
-000267f0: 4e0a 2020 2020 2020 2020 2020 2020 2020  N.              
-00026800: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
-00026810: 2244 656d 616e 6420 5269 7365 220a 2020  "Demand Rise".  
-00026820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026830: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
-00026840: 7254 6578 742e 454e 440a 2020 2020 2020  rText.END.      
+000267e0: 2073 6372 6565 6e44 6963 745b 2250 6174   screenDict["Pat
+000267f0: 7465 726e 225d 203d 2028 0a20 2020 2020  tern"] = (.     
+00026800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026810: 2020 2020 2020 2073 6176 6564 5b30 5d20         saved[0] 
+00026820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00026830: 2020 2020 2020 2020 2020 2020 202b 2063               + c
+00026840: 6f6c 6f72 5465 7874 2e42 4f4c 440a 2020  olorText.BOLD.  
 00026850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026860: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00026870: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00026880: 4469 6374 5b22 5061 7474 6572 6e22 5d20  Dict["Pattern"] 
-00026890: 3d20 7361 7665 645b 315d 202b 2022 4465  = saved[1] + "De
-000268a0: 6d61 6e64 2052 6973 6522 0a20 2020 2020  mand Rise".     
+00026860: 2020 2020 2020 2020 2020 2b20 636f 6c6f            + colo
+00026870: 7254 6578 742e 4752 4545 4e0a 2020 2020  rText.GREEN.    
+00026880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026890: 2020 2020 2020 2020 2b20 2244 656d 616e          + "Deman
+000268a0: 6420 5269 7365 220a 2020 2020 2020 2020  d Rise".        
 000268b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000268c0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-000268d0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-000268e0: 7420 496e 6465 7845 7272 6f72 2061 7320  t IndexError as 
-000268f0: 653a 2023 2070 7261 676d 613a 206e 6f20  e: # pragma: no 
-00026900: 636f 7665 720a 2020 2020 2020 2020 2020  cover.          
-00026910: 2020 2020 2020 7365 6c66 2e64 6566 6175        self.defau
-00026920: 6c74 5f6c 6f67 6765 722e 6465 6275 6728  lt_logger.debug(
-00026930: 652c 2065 7863 5f69 6e66 6f3d 5472 7565  e, exc_info=True
-00026940: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00026950: 2020 7061 7373 0a20 2020 2020 2020 2020    pass.         
-00026960: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00026970: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-00026980: 7863 6570 7469 6f6e 2061 7320 653a 2020  xception as e:  
-00026990: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
-000269a0: 6572 0a20 2020 2020 2020 2020 2020 2073  er.            s
-000269b0: 656c 662e 6465 6661 756c 745f 6c6f 6767  elf.default_logg
-000269c0: 6572 2e64 6562 7567 2865 2c20 6578 635f  er.debug(e, exc_
-000269d0: 696e 666f 3d54 7275 6529 0a20 2020 2020  info=True).     
-000269e0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000269f0: 6c73 650a                                lse.
+000268c0: 2020 2020 2b20 636f 6c6f 7254 6578 742e      + colorText.
+000268d0: 454e 440a 2020 2020 2020 2020 2020 2020  END.            
+000268e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000268f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026900: 2020 2020 2020 7361 7665 4469 6374 5b22        saveDict["
+00026910: 5061 7474 6572 6e22 5d20 3d20 7361 7665  Pattern"] = save
+00026920: 645b 315d 202b 2022 4465 6d61 6e64 2052  d[1] + "Demand R
+00026930: 6973 6522 0a20 2020 2020 2020 2020 2020  ise".           
+00026940: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00026950: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+00026960: 2020 2020 2065 7863 6570 7420 496e 6465       except Inde
+00026970: 7845 7272 6f72 2061 7320 653a 2023 2070  xError as e: # p
+00026980: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
+00026990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000269a0: 7365 6c66 2e64 6566 6175 6c74 5f6c 6f67  self.default_log
+000269b0: 6765 722e 6465 6275 6728 652c 2065 7863  ger.debug(e, exc
+000269c0: 5f69 6e66 6f3d 5472 7565 290a 2020 2020  _info=True).    
+000269d0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+000269e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000269f0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00026a00: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+00026a10: 6f6e 2061 7320 653a 2020 2320 7072 6167  on as e:  # prag
+00026a20: 6d61 3a20 6e6f 2063 6f76 6572 0a20 2020  ma: no cover.   
+00026a30: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00026a40: 6661 756c 745f 6c6f 6767 6572 2e64 6562  fault_logger.deb
+00026a50: 7567 2865 2c20 6578 635f 696e 666f 3d54  ug(e, exc_info=T
+00026a60: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00026a70: 2072 6574 7572 6e20 4661 6c73 650a        return False.
```

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/classes/keys.py` & `pkscreener-0.45.20240527.419/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/courbd.ttf` & `pkscreener-0.45.20240527.419/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/globals.py` & `pkscreener-0.45.20240527.419/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240527.419/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240527.419/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240527.419/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240527.419/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240527.418
+Version: 0.45.20240527.419
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240527.418.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240527.419.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.417/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240527.418/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240527.419/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.418/setup.py` & `pkscreener-0.45.20240527.419/setup.py`

 * *Files identical despite different names*

