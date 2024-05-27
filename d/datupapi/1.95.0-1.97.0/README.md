# Comparing `tmp/datupapi-1.95.0.tar.gz` & `tmp/datupapi-1.97.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datupapi-1.95.0.tar", last modified: Thu May 23 17:40:00 2024, max compression
+gzip compressed data, was "datupapi-1.97.0.tar", last modified: Mon May 27 20:54:08 2024, max compression
```

## Comparing `datupapi-1.95.0.tar` & `datupapi-1.97.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.206116 datupapi-1.95.0/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-05-23 17:40:00.205116 datupapi-1.95.0/PKG-INFO
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.192116 datupapi-1.95.0/datupapi/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.193116 datupapi-1.95.0/datupapi/configure/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/configure/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5750 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/configure/config.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.191115 datupapi-1.95.0/datupapi/distribution/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.194115 datupapi-1.95.0/datupapi/distribution/conf/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.95.0/datupapi/distribution/conf/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.191115 datupapi-1.95.0/datupapi/distribution/src/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.194115 datupapi-1.95.0/datupapi/distribution/src/DistributionFunctions/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.95.0/datupapi/distribution/src/DistributionFunctions/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9390 2023-12-22 18:43:58.000000 datupapi-1.95.0/datupapi/distribution/src/DistributionFunctions/functions_distribution.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.194115 datupapi-1.95.0/datupapi/evaluate/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/evaluate/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7039 2023-07-06 13:37:00.000000 datupapi-1.95.0/datupapi/evaluate/errors.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.196116 datupapi-1.95.0/datupapi/extract/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/extract/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    69213 2024-05-21 16:19:09.000000 datupapi-1.95.0/datupapi/extract/io.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9338 2023-08-28 15:15:16.000000 datupapi-1.95.0/datupapi/extract/io_citrix.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.196116 datupapi-1.95.0/datupapi/feateng/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/feateng/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7922 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/feateng/relation.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4425 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/feateng/scale.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.197116 datupapi-1.95.0/datupapi/inventory/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/inventory/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.197116 datupapi-1.95.0/datupapi/inventory/conf/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.95.0/datupapi/inventory/conf/__init__.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.192116 datupapi-1.95.0/datupapi/inventory/src/
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.197116 datupapi-1.95.0/datupapi/inventory/src/DailyUsage/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.95.0/datupapi/inventory/src/DailyUsage/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7915 2023-08-28 15:14:13.000000 datupapi-1.95.0/datupapi/inventory/src/DailyUsage/daily_usage.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.198116 datupapi-1.95.0/datupapi/inventory/src/Format/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.95.0/datupapi/inventory/src/Format/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5774 2024-05-23 17:38:44.000000 datupapi-1.95.0/datupapi/inventory/src/Format/inventory_format.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.198116 datupapi-1.95.0/datupapi/inventory/src/InventoryFunctions/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.95.0/datupapi/inventory/src/InventoryFunctions/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10157 2024-02-26 21:37:34.000000 datupapi-1.95.0/datupapi/inventory/src/InventoryFunctions/functions_inventory.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.199116 datupapi-1.95.0/datupapi/inventory/src/ProcessForecast/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.95.0/datupapi/inventory/src/ProcessForecast/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10560 2023-08-28 15:14:13.000000 datupapi-1.95.0/datupapi/inventory/src/ProcessForecast/define_periods.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7391 2023-08-28 15:14:13.000000 datupapi-1.95.0/datupapi/inventory/src/ProcessForecast/extract_forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.199116 datupapi-1.95.0/datupapi/inventory/src/SuggestedForecast/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.95.0/datupapi/inventory/src/SuggestedForecast/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    14066 2023-08-28 15:14:13.000000 datupapi-1.95.0/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.200116 datupapi-1.95.0/datupapi/inventory/src/Transformation/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.95.0/datupapi/inventory/src/Transformation/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1219 2023-08-28 15:14:13.000000 datupapi-1.95.0/datupapi/inventory/src/Transformation/inventory_transformation.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    80578 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/inventory/stocks.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.200116 datupapi-1.95.0/datupapi/predict/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/predict/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    27677 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/predict/forecast.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.201115 datupapi-1.95.0/datupapi/prepare/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/prepare/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1922 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/prepare/cleanse.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    20792 2024-05-08 23:46:05.000000 datupapi-1.95.0/datupapi/prepare/format.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4800 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/prepare/format_dask.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.203116 datupapi-1.95.0/datupapi/training/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/training/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    25158 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/training/attup.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    31654 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/training/deepar.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    22819 2024-05-08 16:06:10.000000 datupapi-1.95.0/datupapi/training/tft.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.204115 datupapi-1.95.0/datupapi/transform/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/transform/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    18233 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/transform/backtesting.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)    56492 2024-05-08 16:06:10.000000 datupapi-1.95.0/datupapi/transform/forecasting.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7943 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/transform/ranking.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.204115 datupapi-1.95.0/datupapi/utils/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/utils/__init__.py
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4637 2023-06-26 23:14:24.000000 datupapi-1.95.0/datupapi/utils/utils.py
-drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-23 17:40:00.205116 datupapi-1.95.0/datupapi.egg-info/
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-05-23 17:40:00.000000 datupapi-1.95.0/datupapi.egg-info/PKG-INFO
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1925 2024-05-23 17:40:00.000000 datupapi-1.95.0/datupapi.egg-info/SOURCES.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        1 2024-05-23 17:40:00.000000 datupapi-1.95.0/datupapi.egg-info/dependency_links.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)      539 2024-05-23 17:40:00.000000 datupapi-1.95.0/datupapi.egg-info/requires.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)        9 2024-05-23 17:40:00.000000 datupapi-1.95.0/datupapi.egg-info/top_level.txt
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)       87 2023-12-19 15:43:19.000000 datupapi-1.95.0/pyproject.toml
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)       38 2024-05-23 17:40:00.206116 datupapi-1.95.0/setup.cfg
--rw-r--r--   0 neosagan  (1000) neosagan  (1000)     2129 2024-05-23 17:38:44.000000 datupapi-1.95.0/setup.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:08.000168 datupapi-1.97.0/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-05-27 20:54:07.999168 datupapi-1.97.0/PKG-INFO
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.983168 datupapi-1.97.0/datupapi/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.984168 datupapi-1.97.0/datupapi/configure/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/configure/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5750 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/configure/config.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.980168 datupapi-1.97.0/datupapi/distribution/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.984168 datupapi-1.97.0/datupapi/distribution/conf/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.97.0/datupapi/distribution/conf/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.981168 datupapi-1.97.0/datupapi/distribution/src/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.985168 datupapi-1.97.0/datupapi/distribution/src/DistributionFunctions/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-12-14 13:56:50.000000 datupapi-1.97.0/datupapi/distribution/src/DistributionFunctions/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9390 2023-12-22 18:43:58.000000 datupapi-1.97.0/datupapi/distribution/src/DistributionFunctions/functions_distribution.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.985168 datupapi-1.97.0/datupapi/evaluate/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/evaluate/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7039 2023-07-06 13:37:00.000000 datupapi-1.97.0/datupapi/evaluate/errors.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.986168 datupapi-1.97.0/datupapi/extract/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/extract/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    69213 2024-05-21 16:19:09.000000 datupapi-1.97.0/datupapi/extract/io.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     9338 2023-08-28 15:15:16.000000 datupapi-1.97.0/datupapi/extract/io_citrix.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.987168 datupapi-1.97.0/datupapi/feateng/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/feateng/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7922 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/feateng/relation.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4425 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/feateng/scale.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.988168 datupapi-1.97.0/datupapi/inventory/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/inventory/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.989168 datupapi-1.97.0/datupapi/inventory/conf/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/conf/__init__.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.982168 datupapi-1.97.0/datupapi/inventory/src/
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.989168 datupapi-1.97.0/datupapi/inventory/src/DailyUsage/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/DailyUsage/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7915 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/DailyUsage/daily_usage.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.990168 datupapi-1.97.0/datupapi/inventory/src/Format/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/Format/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     5822 2024-05-27 20:50:16.000000 datupapi-1.97.0/datupapi/inventory/src/Format/inventory_format.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.990168 datupapi-1.97.0/datupapi/inventory/src/InventoryFunctions/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/InventoryFunctions/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    13036 2024-05-27 20:50:16.000000 datupapi-1.97.0/datupapi/inventory/src/InventoryFunctions/functions_inventory.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.991168 datupapi-1.97.0/datupapi/inventory/src/ProcessForecast/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/ProcessForecast/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    10560 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/ProcessForecast/define_periods.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7391 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/ProcessForecast/extract_forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.991168 datupapi-1.97.0/datupapi/inventory/src/SuggestedForecast/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/SuggestedForecast/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    14066 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.992168 datupapi-1.97.0/datupapi/inventory/src/Transformation/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/Transformation/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1219 2023-08-28 15:14:13.000000 datupapi-1.97.0/datupapi/inventory/src/Transformation/inventory_transformation.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    80578 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/inventory/stocks.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.992168 datupapi-1.97.0/datupapi/predict/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/predict/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    27677 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/predict/forecast.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.994168 datupapi-1.97.0/datupapi/prepare/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/prepare/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1922 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/prepare/cleanse.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    20792 2024-05-08 23:46:05.000000 datupapi-1.97.0/datupapi/prepare/format.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4800 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/prepare/format_dask.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.995168 datupapi-1.97.0/datupapi/training/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/training/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    25158 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/training/attup.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    31654 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/training/deepar.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    22819 2024-05-08 16:06:10.000000 datupapi-1.97.0/datupapi/training/tft.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.997168 datupapi-1.97.0/datupapi/transform/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/transform/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    18233 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/transform/backtesting.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)    56492 2024-05-08 16:06:10.000000 datupapi-1.97.0/datupapi/transform/forecasting.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     7943 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/transform/ranking.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.997168 datupapi-1.97.0/datupapi/utils/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        0 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/utils/__init__.py
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     4637 2023-06-26 23:14:24.000000 datupapi-1.97.0/datupapi/utils/utils.py
+drwxr-xr-x   0 neosagan  (1000) neosagan  (1000)        0 2024-05-27 20:54:07.998168 datupapi-1.97.0/datupapi.egg-info/
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1218 2024-05-27 20:54:07.000000 datupapi-1.97.0/datupapi.egg-info/PKG-INFO
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     1925 2024-05-27 20:54:07.000000 datupapi-1.97.0/datupapi.egg-info/SOURCES.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        1 2024-05-27 20:54:07.000000 datupapi-1.97.0/datupapi.egg-info/dependency_links.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)      539 2024-05-27 20:54:07.000000 datupapi-1.97.0/datupapi.egg-info/requires.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)        9 2024-05-27 20:54:07.000000 datupapi-1.97.0/datupapi.egg-info/top_level.txt
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)       87 2023-12-19 15:43:19.000000 datupapi-1.97.0/pyproject.toml
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)       38 2024-05-27 20:54:08.000168 datupapi-1.97.0/setup.cfg
+-rw-r--r--   0 neosagan  (1000) neosagan  (1000)     2129 2024-05-27 20:52:51.000000 datupapi-1.97.0/setup.py
```

### Comparing `datupapi-1.95.0/PKG-INFO` & `datupapi-1.97.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datupapi
-Version: 1.95.0
+Version: 1.97.0
 Summary: Utility library to support Datup AI MLOps processes
 Author: Datup AI
 Author-email: ramiro@datup.ai
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4>=4.9.3
 Requires-Dist: boto3>=1.16.54
 Requires-Dist: catboost>=1.0.4
```

### Comparing `datupapi-1.95.0/datupapi/configure/config.py` & `datupapi-1.97.0/datupapi/configure/config.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/distribution/src/DistributionFunctions/functions_distribution.py` & `datupapi-1.97.0/datupapi/distribution/src/DistributionFunctions/functions_distribution.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/evaluate/errors.py` & `datupapi-1.97.0/datupapi/evaluate/errors.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/extract/io.py` & `datupapi-1.97.0/datupapi/extract/io.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/extract/io_citrix.py` & `datupapi-1.97.0/datupapi/extract/io_citrix.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/feateng/relation.py` & `datupapi-1.97.0/datupapi/feateng/relation.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/feateng/scale.py` & `datupapi-1.97.0/datupapi/feateng/scale.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/inventory/src/DailyUsage/daily_usage.py` & `datupapi-1.97.0/datupapi/inventory/src/DailyUsage/daily_usage.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/inventory/src/Format/inventory_format.py` & `datupapi-1.97.0/datupapi/inventory/src/Format/inventory_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         #formatType : 1 - Format_and_clean Function format (sort the values at the end of the function and do not fill the nans with 0 at the beginning)
         #formatType : 2 - format_tblinv Function format (fill the nans with 0 at the beginning and do not sort the df at the end)
         
         cleanAndFormatIndicators = ["Item","ItemDescription","Location","LocationDescription","Inventory","Transit", "Transfer","Committed",
                                     "InventoryTransit","InventoryTransitForecast","StockoutDays","InvTransStockoutDays","DemandHistory",
                                     "SuggestedForecast","MinSuggestedForecast","BackSuggestedForecast","NextSuggestedForecast","ForecastStockoutDays",
                                     "Ranking","AvgDailyUsage","MaxDailyUsage","AvgLeadTime","MaxLeadTime","LeadTimeDemand","SecurityStock","SecurityStockDays",
-                                    "MinReorderPoint","ReorderPoint","ReorderPointDays","ReorderFreq","MinCoverage","MaxCoverage","ReorderStatus","ReorderQtyBase","ReorderQty",
+                                    "MinReorderPoint","ReorderPoint","ReorderPointDays","ReorderFreq","MinCoverage","MaxCoverage","ReorderStatus","ReorderQtyBase","ReorderQty","NextOrderReorderQtyBase","NextOrderReorderQty",
                                     "BackReorderQtyBase","BackReorderQty","NextReorderQtyBase","NextReorderQty","PurchaseFactor","ReorderQtyFactor","Provider",
                                     "ProviderDescription","UM","MinOrderQty","MaxOrderQty","DeliveryFactor","PurchaseOrderUnit","PalletFactor","SecurityStockDaysRef",
                                     "Exhibitions","ExhibitionsStatus","UnitCost","TotalCost","LastCost","UnitPrice","Stability","Customer","Country","ProductType","Weight","Dimension","Color","Origen","Gama",
                                     "Marca","MateriaPrima","JefeProducto","JefeProductoDescription","GrupoCompra","Familia","Seccion","Categoria", "Linea","Canal",
                                     "InventoryUnit","Comments"]
 
         cleanAndFormatCols = ["Inventory","ReorderFreq","MinCoverage","MaxCoverage","Transit","Committed","Transfer","DemandHistory","SuggestedForecast",
```

### Comparing `datupapi-1.95.0/datupapi/inventory/src/InventoryFunctions/functions_inventory.py` & `datupapi-1.97.0/datupapi/inventory/src/InventoryFunctions/functions_inventory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,84 @@
 import os
 import re
 import pandas as pd
 import numpy as np
 from datupapi.configure.config import Config
+from datetime import datetime
 from datupapi.inventory.src.Format.inventory_format import InventoryFormat
 
 
 class FunctionsInventory(InventoryFormat):
     """
         Class for return a dataframe with all the indicators         
         : param df_inv: Inventory's Dataframe with the columns Item, Location(Optional), Inventory, Transit, DemandHistory  SuggestedForecast AvgDailyUsage MaxDailyUsage
         : param committed: Boolean to enable InventoryTransit computation including Committed
         : param min_inv: Boolean to allow the minimum amount of inventory in location
         : param div_purfac: Boolean to allow data divided by purchase days 
         : param ref_secstock: Boolean to allow Security Stock Ref 
         : param exhibitions: Boolean to allow Exhibitions
+        : param order_date (str): date of the next order %Y-%m-%d 
 
         >>> df_inv = FunctionsInventory(df_inv,committed=True, min_inv=False, div_purfac=False, ref_secstock=False, exhibitions=False).functions_inventory()
     """
 
-    def __init__(self, df_inv, committed, min_inv, ref_secstock, exhibitions, seasonality=False) -> None:      
+    def __init__(self, df_inv, committed, min_inv, ref_secstock, exhibitions, order_date=None, seasonality=False, reorder_new=False) -> None:      
         self.df_inv = df_inv
         self.committed = committed
         self.min_inv = min_inv        
         self.ref_secstock = ref_secstock
+        self.order_date = order_date
         self.exhibitions = exhibitions
         self.seasonality = seasonality
+        self.reorder_new = reorder_new
 
     def inventory(self,df):
         if (self.committed==True):
             df['InventoryTransit'] = df['Inventory'] + df['Transit'] - df['Committed']
         else:
             df['InventoryTransit'] = df['Inventory'] + df['Transit']
         
         df['InventoryTransitForecast'] = df['InventoryTransit'] - df['SuggestedForecast']
         df['LeadTimeDemand'] = df['SuggestedForecast']
+
+        if self.reorder_new is False:
+            df["NextOrderLeadTimeDemand"] = "N/A"
+        
+        else:
+            df["NextOrderLeadTimeDemand"] = df["NextOrderSuggestedForecast"]
+
         return df
 
 
     def stock(self , df):
 
         if ((self.ref_secstock==False) & (self.exhibitions==False) & (self.seasonality==False)):
             df['SecurityStock'] = ((df['MaxDailyUsage']*df['MaxLeadTime']) - (df['AvgDailyUsage']*df['AvgLeadTime']))
         
         elif ((self.ref_secstock==True) & (self.exhibitions==False) & (self.seasonality==False)):
             df['SecurityStock'] = df['SecurityStockDaysRef'] * df['AvgDailyUsage']
         
         elif ((self.ref_secstock==False) & (self.exhibitions==True) & (self.seasonality==False)):
             df['SecurityStock'] = (((df['MaxDailyUsage']*df['MaxLeadTime']) - (df['AvgDailyUsage']*df['AvgLeadTime']))) + df['Exhibitions']
-
-            df['ExhibitionsStatus'] = df.apply(lambda x: "Available" if x["Exhibitions"]>0 else "Unavailable", axis=1)
         
         elif ((self.ref_secstock==True) & (self.exhibitions==True) & (self.seasonality==False)):
             df['SecurityStock'] = (df['SecurityStockDaysRef'] * df['AvgDailyUsage']) + df['Exhibitions']                  
         
 
         elif ((self.ref_secstock==False) & (self.exhibitions==False) & (self.seasonality==True)):
             df['SecurityStock'] = ((df['MaxDailyUsageSeasonality']*df['MaxLeadTime']) - (df['AvgDailyUsageSeasonality']*df['AvgLeadTime']))
         
         elif ((self.ref_secstock==True) & (self.exhibitions==False) & (self.seasonality==True)):
             df['SecurityStock'] = df['SecurityStockDaysRef'] * df['AvgDailyUsageSeasonality']
         
         elif ((self.ref_secstock==False) & (self.exhibitions==True) & (self.seasonality==True)):
             df['SecurityStock'] = (((df['MaxDailyUsageSeasonality']*df['MaxLeadTime']) - (df['AvgDailyUsageSeasonality']*df['AvgLeadTime']))) + df['Exhibitions']
-
-            df['ExhibitionsStatus'] = df.apply(lambda x: "Available" if x["Exhibitions"]>0 else "Unavailable", axis=1)
         
         elif ((self.ref_secstock==True) & (self.exhibitions==True) & (self.seasonality==True)):
-            df['SecurityStock'] = (df['SecurityStockDaysRef'] * df['AvgDailyUsageSeasonality']) + df['Exhibitions']
-
-            df['ExhibitionsStatus'] = df.apply(lambda x: "Available" if x["Exhibitions"]>0 else "Unavailable", axis=1)      
+            df['SecurityStock'] = (df['SecurityStockDaysRef'] * df['AvgDailyUsageSeasonality']) + df['Exhibitions']      
 
 
         df['SecurityStock'] = df['SecurityStock'].fillna(0)
         df['SecurityStock'] = df['SecurityStock'].map(lambda x: 0 if x < 1 else x)
         
         df['SecurityStockDays'] = (df['SecurityStock']) / (df['AvgDailyUsage'])
         InventoryFormat(df).general_indicators_format('SecurityStockDays')
@@ -85,57 +90,194 @@
         InventoryFormat(df).general_indicators_format('InvTransStockoutDays')
         
         df['ForecastStockoutDays'] = (df['InventoryTransitForecast']-df['SecurityStock'])/df['AvgDailyUsage']
         InventoryFormat(df).general_indicators_format('ForecastStockoutDays')
         return df
 
 
-    def reorder(self,df):        
-        df['ReorderPoint'] = (df['LeadTimeDemand'] + df['SecurityStock']).map(lambda x: 0 if x < 0 else x) 
-        df['MinReorderPoint'] = (df['MinSuggestedForecast'] + df['SecurityStock']).map(lambda x: 0 if x < 0 else x)                                
-        df['ReorderPointDays'] = df['ReorderPoint'] / (df['AvgDailyUsage'])
+
+    def order_days(self, df:pd.DataFrame):
+  
+        """
+        Function to get number of days until the next order
+
+        : param df_f: Inventory's Dataframe
+        """
+
+        if self.reorder_new is False: 
+            
+            df["OrderDays"] = "N/A"
+        
+        else: 
+
+            order_date = self.order_date
+
+            actual_date = datetime.today().date()
+            order_date = datetime.strptime(order_date, "%Y-%m-%d").date()
+            difference = order_date - actual_date
+            order_days = int(difference.days)
+
+            df['OrderDays'] = order_days
+
+        return df 
+
+
+
+    def reorder(self, df):
+
+
+        df['ReorderPoint'] = (df['LeadTimeDemand'] + df['SecurityStock']).map(lambda x: max(0, x))
+        df['MinReorderPoint'] = (df['MinSuggestedForecast'] + df['SecurityStock']).map(lambda x: max(0, x))
+        df['ReorderPointDays'] = df['ReorderPoint'] / df['AvgDailyUsage']
+        df['RQty'] = (df['ReorderPoint'] - df['InventoryTransit']).map(lambda x: max(0, x))
+
+
         InventoryFormat(df).general_indicators_format('ReorderPointDays')
 
-        df['ReorderStatus'] = df[['InventoryTransit','MinReorderPoint','SecurityStock']].apply(lambda x: 'Order' if (x['InventoryTransit'] < x['MinReorderPoint'] or x['InventoryTransit'] < x['SecurityStock']) else 'Hold', axis=1)
-        df['ReorderStatus'] = df[['InventoryTransit','MinReorderPoint','ReorderStatus']].apply(lambda x: 'Hold' if (((x['MinReorderPoint'] - x['InventoryTransit']) <1 ) & ((x['MinReorderPoint'] - x['InventoryTransit']) >0 ) & (x['ReorderStatus']=='Order')) else x['ReorderStatus'], axis=1)
-                
+
+        if self.reorder_new is False: 
+
+            df['ReorderStatus'] = df.apply(
+                lambda x: 'Order' if (
+                    x['InventoryTransit'] < x['MinReorderPoint'] or 
+                    x['InventoryTransit'] < x['SecurityStock']
+                ) else 'Hold', axis=1
+            )
+
+            df['ReorderStatus'] = df.apply(
+                lambda x: 'Hold' if (
+                    (0 < x['MinReorderPoint'] - x['InventoryTransit'] < 1) and 
+                    x['ReorderStatus'] == 'Order'
+                ) else x['ReorderStatus'], axis=1
+            )
+
+        else:
+
+            df['ReorderStatus'] = df.apply(
+                lambda x: 'Order' if (
+                    x['InventoryTransit'] < x['ReorderPoint'] or 
+                    x['InventoryTransit'] < x['SecurityStock']
+                ) else 'Hold', axis=1
+            )
+
+            df['ReorderStatus'] = df.apply(
+                lambda x: 'Hold' if (
+                    (0 < x['ReorderPoint'] - x['InventoryTransit'] < 1) and 
+                    x['ReorderStatus'] == 'Order'
+                ) else x['ReorderStatus'], axis=1
+            )
+
+            df['ReorderStatus'] = df.apply(
+                lambda x: 'Order' if (
+                    x['ReorderStatus'] == 'Order' and 
+                    (x['InvTransStockoutDays'] <= x['AvgLeadTime'] or x['OrderDays'] == 0)
+                ) else x['ReorderStatus'], axis=1
+            )
+
+
         if self.min_inv == False:
-            df['RQty'] = (df['ReorderPoint'] - df['InventoryTransit'] ).map(lambda x: 0 if x < 1 else x)
-            df['ReorderQty'] = df[['ReorderStatus','RQty']].apply(lambda x: x['RQty'] if (x['ReorderStatus']=='Order') else 0 , axis=1 )
-            df['ReorderQty'] = df[['ReorderQty','ReorderStatus']].apply(lambda x: (0 if (x['ReorderQty'] < 1) else x['ReorderQty']) if(x['ReorderStatus']=='Order') else x['ReorderQty'], axis=1)
+
+            df['ReorderQty'] = df.apply(
+                lambda x: x['RQty'] if x['ReorderStatus'] == 'Order' else 0, axis=1
+            )
+
+            df['ReorderQty'] = df.apply(
+                lambda x: 0 if x['ReorderQty'] < 1 else x['ReorderQty'], axis=1
+            )
+
+        else:
             
-        if self.min_inv == True:
-            df['RQty'] = (df['ReorderPoint'] - df['InventoryTransit']).map(lambda x: 0 if x < 1 else x)
-            df['ReorderQty'] = df[['ReorderStatus','RQty','DemandHistory']].apply(lambda x: x['RQty'] if (x['ReorderStatus']=='Order') else x['DemandHistory'] , axis=1 )
-            df['ReorderQty'] = df[['ReorderQty','ReorderStatus']].apply(lambda x: (0 if (x['ReorderQty'] < 1) else x['ReorderQty']), axis=1)
-        return df 
+            df['ReorderQty'] = df.apply(
+                lambda x: x['RQty'] if x['ReorderStatus'] == 'Order' else x['DemandHistory'], axis=1
+            )
+
+            df['ReorderQty'] = df.apply(
+                lambda x: 0 if x['ReorderQty'] < 1 else x['ReorderQty'], axis=1
+            )
+
+        return df
+
+
+
+
+    def next_order_reorder(self, df):
+
+
+        if self.reorder_new is False:
+
+            df["NextOrderReorderPoint"] = "N/A"
+            df["NextOrderRQty"] = "N/A"
+            df["NextOrderReorderQty"] = "N/A"
+                
+        else:
+
+            df['NextOrderReorderPoint'] = (df['NextOrderLeadTimeDemand'] + df['SecurityStock']).map(lambda x: max(0, x))
+            df['NextOrderRQty'] = (df['NextOrderReorderPoint'] - df['InventoryTransit']).map(lambda x: max(0, x))
+
 
+            if self.min_inv == False:
 
-    def minmax(self, df):                    
+                df['NextOrderReorderQty'] = df.apply(
+                    lambda x: x['NextOrderRQty'] if x['ReorderStatus'] == 'Order' else 0, axis=1
+                )
+
+                df['NextOrderReorderQty'] = df.apply(
+                    lambda x: 0 if x['NextOrderReorderQty'] < 1 else x['NextOrderReorderQty'], axis=1
+                )
+
+            else:
+                
+                df['NextOrderReorderQty'] = df.apply(
+                    lambda x: x['NextOrderRQty'] if x['ReorderStatus'] == 'Order' else x['DemandHistory'], axis=1
+                )
+
+                df['NextOrderReorderQty'] = df.apply(
+                    lambda x: 0 if x['NextOrderReorderQty'] < 1 else x['NextOrderReorderQty'], axis=1
+                )
+
+        return df
+
+
+
+
+    def minmax(self, df): 
+                           
         df['MinQty'] = (df['BackSuggestedForecast'] + df['SecurityStock']- df['InventoryTransit']).map(lambda x: 0 if x < 1 else x)   
         df['MaxQty'] = (df['NextSuggestedForecast'] + df['SecurityStock']- df['InventoryTransit'] ).map(lambda x: 0 if x < 1 else x)        
         
-        df['MinReorderQty'] = df[['ReorderStatus','MinQty','MaxQty']].apply(lambda x: (x['MinQty'] if (x['MinQty']<x['MaxQty']) else x['MaxQty']) if (x['ReorderStatus']=='Order') else 0 , axis=1 )
-        df['MinReorderQty'] = df[['MinReorderQty','ReorderStatus']].apply(lambda x: (0 if (x['MinReorderQty'] < 1) else x['MinReorderQty']) if(x['ReorderStatus']=='Order') else x['MinReorderQty'], axis=1)
+        df['MinReorderQty'] = df.apply(lambda x: (x['MinQty'] if (x['MinQty']<x['MaxQty']) else x['MaxQty']) if (x['ReorderStatus']=='Order') else 0 , axis=1 )
+        df['MinReorderQty'] = df.apply(lambda x: (0 if (x['MinReorderQty'] < 1) else x['MinReorderQty']) if(x['ReorderStatus']=='Order') else x['MinReorderQty'], axis=1)
         
-        df['MaxReorderQty'] = df[['ReorderStatus','MinQty','MaxQty']].apply(lambda x: (x['MinQty'] if (x['MinQty']>x['MaxQty']) else x['MaxQty']) if (x['ReorderStatus']=='Order') else 0 , axis=1 )
-        df['MaxReorderQty'] = df[['MaxReorderQty','ReorderStatus']].apply(lambda x: (0 if (x['MaxReorderQty'] < 1 )else x['MaxReorderQty']) if(x['ReorderStatus']=='Order') else x['MaxReorderQty'], axis=1)        
+        df['MaxReorderQty'] = df.apply(lambda x: (x['MinQty'] if (x['MinQty']>x['MaxQty']) else x['MaxQty']) if (x['ReorderStatus']=='Order') else 0 , axis=1 )
+        df['MaxReorderQty'] = df.apply(lambda x: (0 if (x['MaxReorderQty'] < 1 ) else x['MaxReorderQty']) if(x['ReorderStatus']=='Order') else x['MaxReorderQty'], axis=1)        
 
         return df
 
 
     def purchase_factor(self,df):
-        df['ReorderQtyBase'] = df['ReorderQty']
-        df['BackReorderQtyBase'] = df['MinReorderQty']
-        df['NextReorderQtyBase'] = df['MaxReorderQty']        
-        df['ReorderQty'] = ((df['ReorderQty']/df['PurchaseFactor']).apply(np.ceil))*df['PurchaseFactor']
-        df['BackReorderQty'] = ((df['MinReorderQty']/df['PurchaseFactor']).apply(np.ceil))*df['PurchaseFactor']
-        df['NextReorderQty'] = ((df['MaxReorderQty']/df['PurchaseFactor']).apply(np.ceil))*df['PurchaseFactor']
 
-        df['ReorderQtyFactor'] = round(df['ReorderQty']/df['PurchaseFactor'])
+
+        if self.reorder_new is False:
+
+            df["NextOrderReorderQtyBase"] = "N/A"
+
+            df['ReorderQtyBase'] = df['ReorderQty']
+            df['BackReorderQtyBase'] = df['MinReorderQty']
+            df['NextReorderQtyBase'] = df['MaxReorderQty']        
+            df['ReorderQty'] = ((df['ReorderQty']/df['PurchaseFactor']).apply(np.ceil))*df['PurchaseFactor']
+            df['BackReorderQty'] = ((df['MinReorderQty']/df['PurchaseFactor']).apply(np.ceil))*df['PurchaseFactor']
+            df['NextReorderQty'] = ((df['MaxReorderQty']/df['PurchaseFactor']).apply(np.ceil))*df['PurchaseFactor']
+
+            df['ReorderQtyFactor'] = round(df['ReorderQty']/df['PurchaseFactor'])
+
+        else:
+
+            df['NextOrderReorderQtyBase'] = df['NextOrderReorderQty']   
+            df['NextOrderReorderQty'] = ((df['NextOrderReorderQty']/df['PurchaseFactor']).apply(np.ceil))*df['PurchaseFactor']
+
 
         return df
 
              
     def functions_inventory(self):
         """
             Return a dataframe with all the indicators         
@@ -147,18 +289,20 @@
 
             >>> df_inv = functions_inventory(df_inv,min_inv=False,div_purfac=False,ref_secstock=False,exhibitions=False)  
         """
         try:            
             df = self.df_inv         
             df = self.inventory(df)
             df = self.stock(df)
+            df = self.order_days(df)
             df = self.reorder(df)
+            df = self.next_order_reorder(df)
             df = self.minmax(df)                                   
             df = self.purchase_factor(df)  
-            df.drop(columns=['RQty','MinQty','MaxQty'], inplace=True) 
+            df.drop(columns=['RQty','NextOrderRQty','MinQty','MaxQty'], inplace=True) 
 
             if 'UnitCost' not in df.columns:
                 df.loc[:,'UnitCost'] = 0           
 
             if 'TotalCost' not in df.columns:        
                 df.loc[:,'TotalCost'] = df['UnitCost'] * df['ReorderQty']
```

### Comparing `datupapi-1.95.0/datupapi/inventory/src/ProcessForecast/define_periods.py` & `datupapi-1.97.0/datupapi/inventory/src/ProcessForecast/define_periods.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/inventory/src/ProcessForecast/extract_forecast.py` & `datupapi-1.97.0/datupapi/inventory/src/ProcessForecast/extract_forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py` & `datupapi-1.97.0/datupapi/inventory/src/SuggestedForecast/suggested_forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/inventory/src/Transformation/inventory_transformation.py` & `datupapi-1.97.0/datupapi/inventory/src/Transformation/inventory_transformation.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/inventory/stocks.py` & `datupapi-1.97.0/datupapi/inventory/stocks.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/predict/forecast.py` & `datupapi-1.97.0/datupapi/predict/forecast.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/prepare/cleanse.py` & `datupapi-1.97.0/datupapi/prepare/cleanse.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/prepare/format.py` & `datupapi-1.97.0/datupapi/prepare/format.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/prepare/format_dask.py` & `datupapi-1.97.0/datupapi/prepare/format_dask.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/training/attup.py` & `datupapi-1.97.0/datupapi/training/attup.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/training/deepar.py` & `datupapi-1.97.0/datupapi/training/deepar.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/training/tft.py` & `datupapi-1.97.0/datupapi/training/tft.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/transform/backtesting.py` & `datupapi-1.97.0/datupapi/transform/backtesting.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/transform/forecasting.py` & `datupapi-1.97.0/datupapi/transform/forecasting.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/transform/ranking.py` & `datupapi-1.97.0/datupapi/transform/ranking.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi/utils/utils.py` & `datupapi-1.97.0/datupapi/utils/utils.py`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi.egg-info/PKG-INFO` & `datupapi-1.97.0/datupapi.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datupapi
-Version: 1.95.0
+Version: 1.97.0
 Summary: Utility library to support Datup AI MLOps processes
 Author: Datup AI
 Author-email: ramiro@datup.ai
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4>=4.9.3
 Requires-Dist: boto3>=1.16.54
 Requires-Dist: catboost>=1.0.4
```

### Comparing `datupapi-1.95.0/datupapi.egg-info/SOURCES.txt` & `datupapi-1.97.0/datupapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/datupapi.egg-info/requires.txt` & `datupapi-1.97.0/datupapi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datupapi-1.95.0/setup.py` & `datupapi-1.97.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='datupapi',
-      version='1.95.0',
+      version='1.97.0',
       description='Utility library to support Datup AI MLOps processes',
       long_description_content_type="text/markdown",
       long_description="foo bar baz",
       author='Datup AI',
       author_email='ramiro@datup.ai',
       packages=[
           'datupapi',
```

