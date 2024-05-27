# Comparing `tmp/tqsdk-3.5.8.tar.gz` & `tmp/tqsdk-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tqsdk-3.5.8.tar", last modified: Mon Apr 29 10:12:41 2024, max compression
+gzip compressed data, was "dist/tqsdk-3.5.9.tar", last modified: Thu May  9 06:36:18 2024, max compression
```

## Comparing `tqsdk-3.5.8.tar` & `tqsdk-3.5.9.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/rangeset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/baseModule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/stockprofit.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/datetime_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)    19888 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tqwebhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/data_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/sm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/demo/example/
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/aberration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/rbreaker2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/doublema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/turtle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/gridtrading.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/vwap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/dualthrust.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/gridtrading_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/rbreaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/momentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/escalator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/fairy_four_price.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/example/random_forest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t70.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t20.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t30.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t91.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t93.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/replay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t80.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/replay2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t71.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t92.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t60.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t90.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t96.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t40.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t41.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/underlying_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t94.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t95.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/tutorial/t72.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/multiaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/download_orders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/ta_option.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o41.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o72.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o30.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o71.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o40.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o20.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o70.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o74.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o73.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/option_tutorial/o60.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/demo/ta.py
--rw-r--r--   0 runner    (1001) docker     (127)    21994 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/objs_not_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/trading_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/backtest/
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/backtest/replay.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/backtest/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44023 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/backtest/backtest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/__pyinstaller/hook-tqsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/risk_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)    15912 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/algorithm/time_table_generater.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/algorithm/twap.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/multiaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/baseApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/risk_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/utils_symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/lib/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/lib/time_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/lib/target_pos_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40355 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/lib/target_pos_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    52750 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tafunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    37797 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/objs.py
--rw-r--r--   0 runner    (1001) docker     (127)   210312 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/trade_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)   132245 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/expired_quotes.json.lzma
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/tradeable/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/
--rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/tqsim.py
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/trade_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    36480 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/trade_future.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27585 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/trade_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/tqsim_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)    18113 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/sim/basesim.py
--rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/tradeable/otg/
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/otg/tqkq.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/otg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/otg/tqaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/otg/tqzq.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/otg/base_otg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tradeable/tradeable.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/web/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/web/js/
--rw-r--r--   0 runner    (1001) docker     (127)  1787845 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/js/chunk-vendors.d7fceff6.js
--rw-r--r--   0 runner    (1001) docker     (127)    62759 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/js/app.2c843c86.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/web/img/
--rw-r--r--   0 runner    (1001) docker     (127)   555353 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/img/ionicons.a2c4a261.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/web/img/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/ms-icon-70x70.png
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-48x48.png
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/favicon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-36x36.png
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/msapplication-icon-144x144.png.png
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/ms-icon-310x310.png
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-57x57.png
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/notes
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/ms-icon-150x150.png
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-29 10:12:09.000000 tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/web/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   197740 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/fonts/ionicons.99ac3308.woff
--rw-r--r--   0 runner    (1001) docker     (127)   197664 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/fonts/ionicons.d535a25a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    82216 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/fonts/ionicons.143146fa.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   246120 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/d3.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/service-worker.js
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/web/css/
--rw-r--r--   0 runner    (1001) docker     (127)   279508 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/css/chunk-vendors.c93e9127.css
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/css/app.d72d8978.css
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/web/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tools/dead_ins.lzma
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21566 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/tools/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    20440 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    91538 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/ta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)    22562 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/ins_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    23562 2024-04-29 10:12:08.000000 tqsdk-3.5.8/tqsdk/data_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-29 10:12:08.000000 tqsdk-3.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-29 10:12:08.000000 tqsdk-3.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-29 10:12:41.000000 tqsdk-3.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-29 10:12:08.000000 tqsdk-3.5.8/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 10:12:41.000000 tqsdk-3.5.8/tqsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-29 10:12:41.000000 tqsdk-3.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-29 10:12:08.000000 tqsdk-3.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/baseModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/stockprofit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/datetime_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19888 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tqwebhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/data_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/sm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/demo/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/aberration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/rbreaker2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/doublema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/gridtrading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/vwap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/dualthrust.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/gridtrading_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/rbreaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/escalator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/fairy_four_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/example/random_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t70.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t30.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t91.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t93.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t80.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/replay2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t71.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t92.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t60.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t90.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t96.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t40.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t41.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/underlying_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t94.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t95.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/tutorial/t72.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/multiaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/download_orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/ta_option.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/o41.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/o72.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/o30.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/o71.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/o40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/o20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/o10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/o70.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/o74.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/o73.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/option_tutorial/o60.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/demo/ta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21994 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/objs_not_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/trading_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/backtest/
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/backtest/replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/backtest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/backtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44023 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/backtest/backtest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/__pyinstaller/hook-tqsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/risk_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)    15912 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/algorithm/time_table_generater.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/algorithm/twap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/multiaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/baseApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/risk_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/utils_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/lib/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/lib/time_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/lib/target_pos_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40355 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/lib/target_pos_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52750 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tafunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37797 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/objs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   210546 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/trade_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)   132245 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/expired_quotes.json.lzma
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/tradeable/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/tradeable/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/sim/tqsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/sim/trade_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36480 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/sim/trade_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/sim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27585 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/sim/trade_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/sim/tqsim_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18113 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/sim/basesim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/tradeable/otg/
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/otg/tqkq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/otg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/otg/tqaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/otg/tqzq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/otg/base_otg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tradeable/tradeable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/web/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/web/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  1787845 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/js/chunk-vendors.d7fceff6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    62759 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/js/app.2c843c86.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/web/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   555353 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/ionicons.a2c4a261.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/web/img/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/ms-icon-70x70.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/android-icon-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/favicon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/android-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/android-icon-36x36.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/msapplication-icon-144x144.png.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/android-icon-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/ms-icon-310x310.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/android-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-57x57.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/notes
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/android-icon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/ms-icon-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-09 06:35:40.000000 tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/web/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   197740 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/web/fonts/ionicons.99ac3308.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   197664 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/web/fonts/ionicons.d535a25a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    82216 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/web/fonts/ionicons.143146fa.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/web/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   246120 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/web/d3.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/web/service-worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/web/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/web/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/web/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   279508 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/web/css/chunk-vendors.c93e9127.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/web/css/app.d72d8978.css
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/web/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tools/dead_ins.lzma
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19058 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/tools/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20440 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91538 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/ta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22562 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/ins_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20938 2024-05-09 06:35:39.000000 tqsdk-3.5.9/tqsdk/data_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-05-09 06:35:39.000000 tqsdk-3.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-05-09 06:35:39.000000 tqsdk-3.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-09 06:36:18.000000 tqsdk-3.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-09 06:35:39.000000 tqsdk-3.5.9/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-09 06:36:17.000000 tqsdk-3.5.9/tqsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:36:17.000000 tqsdk-3.5.9/tqsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-09 06:36:17.000000 tqsdk-3.5.9/tqsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 06:36:18.000000 tqsdk-3.5.9/tqsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 06:36:18.000000 tqsdk-3.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-09 06:35:39.000000 tqsdk-3.5.9/setup.py
```

### Comparing `tqsdk-3.5.8/tqsdk/rangeset.py` & `tqsdk-3.5.9/tqsdk/rangeset.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/baseModule.py` & `tqsdk-3.5.9/tqsdk/baseModule.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/stockprofit.py` & `tqsdk-3.5.9/tqsdk/stockprofit.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/datetime_state.py` & `tqsdk-3.5.9/tqsdk/datetime_state.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/datetime.py` & `tqsdk-3.5.9/tqsdk/datetime.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tqwebhelper.py` & `tqsdk-3.5.9/tqsdk/tqwebhelper.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/symbols.py` & `tqsdk-3.5.9/tqsdk/symbols.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/data_extension.py` & `tqsdk-3.5.9/tqsdk/data_extension.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/sm.py` & `tqsdk-3.5.9/tqsdk/sm.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/aberration.py` & `tqsdk-3.5.9/tqsdk/demo/example/aberration.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/rbreaker2.py` & `tqsdk-3.5.9/tqsdk/demo/example/rbreaker2.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/doublema.py` & `tqsdk-3.5.9/tqsdk/demo/example/doublema.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/turtle.py` & `tqsdk-3.5.9/tqsdk/demo/example/turtle.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/gridtrading.py` & `tqsdk-3.5.9/tqsdk/demo/example/gridtrading.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/vwap.py` & `tqsdk-3.5.9/tqsdk/demo/example/vwap.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/dualthrust.py` & `tqsdk-3.5.9/tqsdk/demo/example/dualthrust.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/gridtrading_async.py` & `tqsdk-3.5.9/tqsdk/demo/example/gridtrading_async.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/rbreaker.py` & `tqsdk-3.5.9/tqsdk/demo/example/rbreaker.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/momentum.py` & `tqsdk-3.5.9/tqsdk/demo/example/momentum.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/escalator.py` & `tqsdk-3.5.9/tqsdk/demo/example/escalator.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/fairy_four_price.py` & `tqsdk-3.5.9/tqsdk/demo/example/fairy_four_price.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/example/random_forest.py` & `tqsdk-3.5.9/tqsdk/demo/example/random_forest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t70.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t70.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t20.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t20.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t30.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t30.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t91.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t91.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t93.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t93.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/replay.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/replay.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t80.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t80.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/replay2.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/replay2.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t71.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t71.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t92.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t92.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/downloader.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/downloader.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t60.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t60.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t90.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t90.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t96.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t96.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t40.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t40.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t41.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t41.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/backtest.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/backtest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t94.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t94.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t95.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t95.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/tutorial/t72.py` & `tqsdk-3.5.9/tqsdk/demo/tutorial/t72.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/multiaccount.py` & `tqsdk-3.5.9/tqsdk/demo/multiaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/download_orders.py` & `tqsdk-3.5.9/tqsdk/demo/download_orders.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/ta_option.py` & `tqsdk-3.5.9/tqsdk/demo/ta_option.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o41.py` & `tqsdk-3.5.9/tqsdk/demo/option_tutorial/o41.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o72.py` & `tqsdk-3.5.9/tqsdk/demo/option_tutorial/o72.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o30.py` & `tqsdk-3.5.9/tqsdk/demo/option_tutorial/o30.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o71.py` & `tqsdk-3.5.9/tqsdk/demo/option_tutorial/o71.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o40.py` & `tqsdk-3.5.9/tqsdk/demo/option_tutorial/o40.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o20.py` & `tqsdk-3.5.9/tqsdk/demo/option_tutorial/o20.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o70.py` & `tqsdk-3.5.9/tqsdk/demo/option_tutorial/o70.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o74.py` & `tqsdk-3.5.9/tqsdk/demo/option_tutorial/o74.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o73.py` & `tqsdk-3.5.9/tqsdk/demo/option_tutorial/o73.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/option_tutorial/o60.py` & `tqsdk-3.5.9/tqsdk/demo/option_tutorial/o60.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/demo/ta.py` & `tqsdk-3.5.9/tqsdk/demo/ta.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/connect.py` & `tqsdk-3.5.9/tqsdk/connect.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/objs_not_entity.py` & `tqsdk-3.5.9/tqsdk/objs_not_entity.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/auth.py` & `tqsdk-3.5.9/tqsdk/auth.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/trading_status.py` & `tqsdk-3.5.9/tqsdk/trading_status.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/backtest/replay.py` & `tqsdk-3.5.9/tqsdk/backtest/replay.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/backtest/utils.py` & `tqsdk-3.5.9/tqsdk/backtest/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/backtest/backtest.py` & `tqsdk-3.5.9/tqsdk/backtest/backtest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/risk_rule.py` & `tqsdk-3.5.9/tqsdk/risk_rule.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/algorithm/time_table_generater.py` & `tqsdk-3.5.9/tqsdk/algorithm/time_table_generater.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/algorithm/twap.py` & `tqsdk-3.5.9/tqsdk/algorithm/twap.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/__init__.py` & `tqsdk-3.5.9/tqsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/multiaccount.py` & `tqsdk-3.5.9/tqsdk/multiaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/baseApi.py` & `tqsdk-3.5.9/tqsdk/baseApi.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/calendar.py` & `tqsdk-3.5.9/tqsdk/calendar.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/risk_manager.py` & `tqsdk-3.5.9/tqsdk/risk_manager.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/utils_symbols.py` & `tqsdk-3.5.9/tqsdk/utils_symbols.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/lib/notify.py` & `tqsdk-3.5.9/tqsdk/lib/notify.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/lib/target_pos_scheduler.py` & `tqsdk-3.5.9/tqsdk/lib/target_pos_scheduler.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/lib/utils.py` & `tqsdk-3.5.9/tqsdk/lib/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/lib/target_pos_task.py` & `tqsdk-3.5.9/tqsdk/lib/target_pos_task.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tafunc.py` & `tqsdk-3.5.9/tqsdk/tafunc.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/exceptions.py` & `tqsdk-3.5.9/tqsdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/log.py` & `tqsdk-3.5.9/tqsdk/log.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/objs.py` & `tqsdk-3.5.9/tqsdk/objs.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/api.py` & `tqsdk-3.5.9/tqsdk/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2924,15 +2924,17 @@
     def query_all_level_finance_options(self, underlying_symbol, underlying_price, option_class,
                                         nearbys: Union[int, List[int]], has_A: bool = None) -> SymbolList:
         """
         发送合约服务请求查询，针对 ETF 期权和股指期权，只查询未下市合约，可以按照距离最后行权日的距离的远近，查询符合条件的期权列表，返回全部的实值、平值、虚值期权
 
         Args:
             underlying_symbol (str): [必填] 标的合约 （针对 ETF 期权和股指期权，只支持以下几个合约）
-                * "SSE.000300" 为中金所股指期权标的
+                * "SSE.000300" 为中金所沪深 300 股指期权(IO)标的
+                * "SSE.000852" 为中金所中证 1000 股指期权(MO)标的
+                * "SSE.000016" 为中金所上证 50 股指期权(HO)标的
                 * "SSE.510050" 为上交所华夏上证 50 ETF 期权标的
                 * "SSE.510300" 为上交所华泰柏瑞沪深 300 ETF 期权标的
                 * "SZSE.159919" 为深交所嘉实沪深 300 ETF 期权标的
                 * "SZSE.159915" 为深交所易方达创业板 ETF 期权标的
                 * "SZSE.159922" 为深交所嘉实中证 500 ETF 期权标的
                 * "SSE.510500" 为上交所南方中证 500 ETF 期权标的
 
@@ -2987,15 +2989,16 @@
             print(in_money_options)  # 实值期权列表
             print(at_money_options)  # 平值期权列表
             print(out_of_money_options)  # 虚值期权列表
 
         """
         if self._stock is False:
             raise Exception("期货行情系统(_stock = False)不支持当前接口调用")
-        if underlying_symbol not in ["SSE.000300", "SSE.510050", "SSE.510300", "SZSE.159919", "SZSE.159915", "SZSE.159922", "SSE.510500"]:
+        if underlying_symbol not in ["SSE.000300", "SSE.510050", "SSE.510300", "SZSE.159919", "SZSE.159915", "SZSE.159922", "SSE.510500",
+                                     "SSE.000016", "SSE.000852"]:
             raise Exception("不支持的标的合约")
         if option_class not in ['CALL', 'PUT']:
             raise Exception("option_class 参数错误，option_class 必须是 'CALL' 或者 'PUT'")
         nearbys = nearbys if isinstance(nearbys, list) else [nearbys]
         if underlying_symbol == "SSE.000300":  # 股指期权
             if any([i not in [0, 1, 2, 3, 4, 5] for i in nearbys]):
                 raise Exception(f"股指期权标的为：{underlying_symbol}，exercise_date 参数应该是在 [0, 1, 2, 3, 4, 5] 之间。")
```

### Comparing `tqsdk-3.5.8/tqsdk/entity.py` & `tqsdk-3.5.9/tqsdk/entity.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/trade_extension.py` & `tqsdk-3.5.9/tqsdk/trade_extension.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/expired_quotes.json.lzma` & `tqsdk-3.5.9/tqsdk/expired_quotes.json.lzma`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/channel.py` & `tqsdk-3.5.9/tqsdk/channel.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/sim/tqsim.py` & `tqsdk-3.5.9/tqsdk/tradeable/sim/tqsim.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/sim/trade_base.py` & `tqsdk-3.5.9/tqsdk/tradeable/sim/trade_base.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/sim/trade_future.py` & `tqsdk-3.5.9/tqsdk/tradeable/sim/trade_future.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/sim/utils.py` & `tqsdk-3.5.9/tqsdk/tradeable/sim/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/sim/trade_stock.py` & `tqsdk-3.5.9/tqsdk/tradeable/sim/trade_stock.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/sim/tqsim_stock.py` & `tqsdk-3.5.9/tqsdk/tradeable/sim/tqsim_stock.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/sim/basesim.py` & `tqsdk-3.5.9/tqsdk/tradeable/sim/basesim.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/mixin.py` & `tqsdk-3.5.9/tqsdk/tradeable/mixin.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/otg/tqkq.py` & `tqsdk-3.5.9/tqsdk/tradeable/otg/tqkq.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/otg/tqaccount.py` & `tqsdk-3.5.9/tqsdk/tradeable/otg/tqaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/otg/tqzq.py` & `tqsdk-3.5.9/tqsdk/tradeable/otg/tqzq.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/otg/base_otg.py` & `tqsdk-3.5.9/tqsdk/tradeable/otg/base_otg.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tradeable/tradeable.py` & `tqsdk-3.5.9/tqsdk/tradeable/tradeable.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/js/chunk-vendors.d7fceff6.js` & `tqsdk-3.5.9/tqsdk/web/js/chunk-vendors.d7fceff6.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/js/app.2c843c86.js` & `tqsdk-3.5.9/tqsdk/web/js/app.2c843c86.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/ionicons.a2c4a261.svg` & `tqsdk-3.5.9/tqsdk/web/img/ionicons.a2c4a261.svg`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/ms-icon-70x70.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/android-chrome-192x192.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-60x60.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/mstile-150x150.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-76x76.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-48x48.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/favicon-96x96.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-144x144.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-144x144.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-72x72.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-36x36.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-152x152.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/favicon.ico` & `tqsdk-3.5.9/tqsdk/web/img/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/msapplication-icon-144x144.png.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/msapplication-icon-144x144.png.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-192x192.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-114x114.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/ms-icon-310x310.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-72x72.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/favicon-32x32.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-57x57.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/notes` & `tqsdk-3.5.9/tqsdk/web/img/icons/notes`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/android-icon-96x96.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/favicon-16x16.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-120x120.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/ms-icon-150x150.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-precomposed.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/manifest.json` & `tqsdk-3.5.9/tqsdk/web/img/icons/manifest.json`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/img/icons/apple-touch-icon-180x180.png` & `tqsdk-3.5.9/tqsdk/web/img/icons/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js` & `tqsdk-3.5.9/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/fonts/ionicons.99ac3308.woff` & `tqsdk-3.5.9/tqsdk/web/fonts/ionicons.99ac3308.woff`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/fonts/ionicons.d535a25a.ttf` & `tqsdk-3.5.9/tqsdk/web/fonts/ionicons.d535a25a.ttf`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/fonts/ionicons.143146fa.woff2` & `tqsdk-3.5.9/tqsdk/web/fonts/ionicons.143146fa.woff2`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/favicon.ico` & `tqsdk-3.5.9/tqsdk/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/d3.min.js` & `tqsdk-3.5.9/tqsdk/web/d3.min.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/service-worker.js` & `tqsdk-3.5.9/tqsdk/web/service-worker.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/index.html` & `tqsdk-3.5.9/tqsdk/web/index.html`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/css/chunk-vendors.c93e9127.css` & `tqsdk-3.5.9/tqsdk/web/css/chunk-vendors.c93e9127.css`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/css/app.d72d8978.css` & `tqsdk-3.5.9/tqsdk/web/css/app.d72d8978.css`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/web/manifest.json` & `tqsdk-3.5.9/tqsdk/web/manifest.json`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tools/dead_ins.lzma` & `tqsdk-3.5.9/tqsdk/tools/dead_ins.lzma`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/tools/downloader.py` & `tqsdk-3.5.9/tqsdk/tools/downloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 import lzma
 
 import pandas
 
 from tqsdk.api import TqApi
 from tqsdk.datetime import _cst_tz, _convert_user_input_to_nano
 from tqsdk.diff import _get_obj
-from tqsdk.tafunc import get_dividend_df
-from tqsdk.utils import _generate_uuid
+from tqsdk.utils import _generate_uuid, _get_dividend_factor
 
 try:
     file_path = os.path.split(os.path.abspath(__file__))[0]
     with lzma.open(os.path.join(file_path, "dead_ins.lzma"), "rt", encoding="utf-8") as dead_ins_file:
         DEAD_INS = {l.strip() for l in dead_ins_file}
 except:
     DEAD_INS = {}
@@ -184,54 +183,15 @@
                 self._data_series = pandas.read_csv(self._csv_file_name)
             return self._data_series
         else:
             raise Exception('DataDownloader._get_data_series 接口仅支持 csv_file_name 參數为 str 时使用')
 
     async def _ensure_dividend_factor(self, quote, timestamp):
         if quote.instrument_id not in self._dividend_cache:
-            # 对每个除权除息矩阵增加 factor 序列，为当日的复权因子
-            df = get_dividend_df(quote.stock_dividend_ratio, quote.cash_dividend_ratio)
-            df = df[df["datetime"].between(timestamp, self._end_dt_nano, inclusive="right")]  # 只需要第一笔行情时间～结束时间之间的复权因子, 左开右闭
-            df["pre_close"] = float('nan')  # 初始化 pre_close 为 nan
-            for i in range(len(df)):
-                chart_info = {
-                    "aid": "set_chart",
-                    "chart_id": _generate_uuid("PYSDK_downloader"),
-                    "ins_list": quote.instrument_id,
-                    "duration": 86400 * 1000000000,
-                    "view_width": 2,
-                    "focus_datetime": int(df["datetime"].iloc[i]),
-                    "focus_position": 1
-                }
-                await self._api._send_chan.send(chart_info)
-                chart = _get_obj(self._api._data, ["charts", chart_info["chart_id"]])
-                serial = _get_obj(self._api._data, ["klines", quote.instrument_id, str(86400000000000)])
-                try:
-                    async with self._api.register_update_notify() as update_chan:
-                        async for _ in update_chan:
-                            if not (chart_info.items() <= _get_obj(chart, ["state"]).items()):
-                                continue  # 当前请求还没收齐回应, 不应继续处理
-                            if chart.get("ready", False) is False:
-                                continue  # 合约的数据是否收到
-                            left_id = chart.get("left_id", -1)
-                            assert left_id != -1  # 需要下载除权除息日的前一天行情，即这一天一定是有行情的，left_id 一定不是 -1
-                            last_item = serial["data"].get(str(left_id), {})
-                            # 复权时间点的昨收盘
-                            df.loc[i, 'pre_close'] = last_item['close'] if last_item.get('close') else float('nan')
-                            break
-                finally:
-                    await self._api._send_chan.send({
-                        "aid": "set_chart",
-                        "chart_id": chart_info["chart_id"],
-                        "ins_list": "",
-                        "duration": 86400000000000,
-                        "view_width": 2
-                    })
-            df["factor"] = (df["pre_close"] - df["cash_dividend"]) / df["pre_close"] / (1 + df["stock_dividend"])
-            df["factor"].fillna(1.0, inplace=True)
+            df = await _get_dividend_factor(self._api, quote, timestamp, self._end_dt_nano, chart_id_prefix="PYSDK_downloader")
             # 插入结束时间这条记录, 因为可能存在行情时间等于 _end_dt_nano 的行情，因此这里 +1
             df = df.append({"datetime": self._end_dt_nano+1, "factor": 1.0}, ignore_index=True)
             if self._adj_type == "F":
                 df["factor"] = df["factor"].iloc[::-1].cumprod().iloc[::-1]
             elif self._adj_type == "B":
                 # 后复权按定义上应该从第一笔行情之后产生的复权事件开始
                 # 第一笔行情时间一定小于 df["datetime"].iloc[0], 因此复权是从 df["datetime"].iloc[0] 开始
```

### Comparing `tqsdk-3.5.8/tqsdk/report.py` & `tqsdk-3.5.9/tqsdk/report.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/ta.py` & `tqsdk-3.5.9/tqsdk/ta.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/diff.py` & `tqsdk-3.5.9/tqsdk/diff.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/ins_schema.py` & `tqsdk-3.5.9/tqsdk/ins_schema.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/tqsdk/data_series.py` & `tqsdk-3.5.9/tqsdk/data_series.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 import numpy as np
 import pandas as pd
 from filelock import FileLock
 
 from tqsdk.channel import TqChan
 from tqsdk.diff import _get_obj
 from tqsdk.rangeset import _rangeset_difference, _rangeset_intersection
-from tqsdk.tafunc import get_dividend_df
-from tqsdk.utils import _generate_uuid
+from tqsdk.utils import _generate_uuid, _get_dividend_factor
 
 CACHE_DIR = os.path.join(os.path.expanduser('~'), ".tqsdk/data_series_1")
 
 
 class DataSeries:
     """
     获取数据模块，支持用户获取任意时间段内的 Kline / Tick 数据，返回格式为 pandas.DataFrame
@@ -140,15 +139,16 @@
                 self.df[c] = array[c]
             self.df["symbol"] = symbol
             self.df["duration"] = self._dur_nano
 
             # 复权, 如果存在 STOCK / FUND 并且 adj_type is not None, 这里需要提前准备下载时间段内的复权因子
             quote = self._api.get_quote(symbol)
             if self._adj_type and quote.ins_class in ["STOCK", "FUND"]:
-                factor_df = await self._update_dividend_factor(symbol)  # 复权需要根据日线计算除权因子，todo: 如果本地下载过日线，不需要再从服务器获取日线数据
+                factor_df = await _get_dividend_factor(self._api, quote, self._start_dt_nano, self._end_dt_nano,
+                                                       chart_id_prefix="PYSDK_data_factor")  # 复权需要根据日线计算除权因子，todo: 如果本地下载过日线，不需要再从服务器获取日线数据
                 if self._adj_type == "F":
                     # 倒序循环 factor_df, 对于小于当前 factor_df[datetime] 的行 乘以 factor_df[factor]
                     for i in range(factor_df.shape[0] - 1, -1, -1):
                         dt = factor_df.iloc[i].datetime
                         factor = factor_df.iloc[i].factor
                         adj_cols = DataSeries._get_adj_cols(symbol, self._dur_nano)
                         lt = self.df["datetime"].lt(dt)
@@ -208,21 +208,20 @@
         serial = _get_obj(self._api._data, path)
         cols = DataSeries._get_data_cols(symbol, self._dur_nano)
         try:
             async with self._api.register_update_notify() as update_chan:
                 async for _ in update_chan:
                     if not (chart_info.items() <= _get_obj(chart, ["state"]).items()):
                         continue  # 当前请求还没收齐回应, 不应继续处理
+                    if chart.get("ready", False) is False:
+                        continue  # 数据还没全部收到
+                    if serial.get("last_id", -1) == -1:
+                        return  # 合约没有任何数据
                     left_id = chart.get("left_id", -1)
                     right_id = chart.get("right_id", -1)
-                    if (left_id == -1 and right_id == -1) or self._api._data.get("mdhis_more_data", True):
-                        continue  # 定位信息还没收到, 或数据序列还没收到
-                    # 检查合约的数据是否收到
-                    if serial.get("last_id", -1) == -1:
-                        continue
                     if current_id is None:
                         current_id = max(left_id, 0)
                     while current_id <= right_id:
                         item = serial["data"].get(str(current_id), {})
                         if item.get("datetime", 0) == 0 or item["datetime"] >= end_dt:
                             return  # 当前 id 已超出 last_id 或k线数据的时间已经超过用户限定的右端
                         row = [current_id, item["datetime"]] + [DataSeries._get_float_value(item, c) for c in cols]
@@ -241,59 +240,14 @@
                 "aid": "set_chart",
                 "chart_id": chart_info["chart_id"],
                 "ins_list": "",
                 "duration": self._dur_nano,
                 "view_width": 2000,
             })
 
-    async def _update_dividend_factor(self, symbol):
-        quote = self._api.get_quote(symbol)
-        df = get_dividend_df(quote.stock_dividend_ratio, quote.cash_dividend_ratio)
-        between = df["datetime"].between(self._start_dt_nano, self._end_dt_nano)  # 只需要开始时间～结束时间之间的复权因子
-        df["pre_close"] = float('nan')
-        for i in df[between].index:
-            chart_info = {
-                "aid": "set_chart",
-                "chart_id": _generate_uuid("PYSDK_data_factor"),
-                "ins_list": symbol,
-                "duration": 86400 * 1000000000,
-                "view_width": 2,
-                "focus_datetime": int(df.iloc[i].datetime),
-                "focus_position": 1
-            }
-            await self._api._send_chan.send(chart_info)
-            chart = _get_obj(self._api._data, ["charts", chart_info["chart_id"]])
-            serial = _get_obj(self._api._data, ["klines", symbol, str(86400000000000)])
-            try:
-                async with self._api.register_update_notify() as update_chan:
-                    async for _ in update_chan:
-                        if not (chart_info.items() <= _get_obj(chart, ["state"]).items()):
-                            continue  # 当前请求还没收齐回应, 不应继续处理
-                        left_id = chart.get("left_id", -1)
-                        right_id = chart.get("right_id", -1)
-                        if (left_id == -1 and right_id == -1) or self._api._data.get("mdhis_more_data",
-                                                                                     True) or serial.get("last_id",
-                                                                                                         -1) == -1:
-                            continue  # 定位信息还没收到, 或数据序列还没收到, 合约的数据是否收到
-                        last_item = serial["data"].get(str(left_id), {})
-                        # 复权时间点的昨收盘
-                        df.loc[i, 'pre_close'] = last_item['close'] if last_item.get('close') else float('nan')
-                        break
-            finally:
-                await self._api._send_chan.send({
-                    "aid": "set_chart",
-                    "chart_id": chart_info["chart_id"],
-                    "ins_list": "",
-                    "duration": 86400000000000,
-                    "view_width": 2
-                })
-        df["factor"] = (df["pre_close"] - df["cash_dividend"]) / df["pre_close"] / (1 + df["stock_dividend"])
-        df["factor"].fillna(1, inplace=True)
-        return df
-
     def _merge_rangeset(self):
         symbol = self._symbol_list[0]
         rangeset = DataSeries._get_rangeset_id(symbol, self._dur_nano)
         if len(rangeset) <= 1:
             return
         # 可以 merge 的 rangset 分组, rangset_group 类型是 list_of_list, [[(start, end, rows), ], [], ....]
         # 内层列表的每个元素值为 range 的 start, end，用来找到正确的文件名，rows 表示 merge 文件时，应该从当前一段 range 里 merge 多少行
```

### Comparing `tqsdk-3.5.8/README.md` & `tqsdk-3.5.9/README.md`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/LICENSE` & `tqsdk-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/PKG-INFO` & `tqsdk-3.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqsdk
-Version: 3.5.8
+Version: 3.5.9
 Summary: TianQin SDK
 Home-page: https://www.shinnytech.com/tqsdk
 Author: TianQin
 Author-email: tianqincn@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tqsdk-3.5.8/tqsdk.egg-info/PKG-INFO` & `tqsdk-3.5.9/tqsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqsdk
-Version: 3.5.8
+Version: 3.5.9
 Summary: TianQin SDK
 Home-page: https://www.shinnytech.com/tqsdk
 Author: TianQin
 Author-email: tianqincn@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tqsdk-3.5.8/tqsdk.egg-info/SOURCES.txt` & `tqsdk-3.5.9/tqsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.8/setup.py` & `tqsdk-3.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", mode="r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tqsdk',
-    version="3.5.8",
+    version="3.5.9",
     description='TianQin SDK',
     author='TianQin',
     author_email='tianqincn@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://www.shinnytech.com/tqsdk',
     packages=setuptools.find_packages(exclude=["tqsdk.test", "tqsdk.test.*"]),
```

