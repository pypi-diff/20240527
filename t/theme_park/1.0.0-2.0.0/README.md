# Comparing `tmp/theme_park-1.0.0.tar.gz` & `tmp/theme_park-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theme_park-1.0.0.tar", max compression
+gzip compressed data, was "theme_park-2.0.0.tar", max compression
```

## Comparing `theme_park-1.0.0.tar` & `theme_park-2.0.0.tar`

### file list

```diff
@@ -1,272 +1,385 @@
--rwxr-xr-x   0        0        0     1750 2024-05-18 02:43:42.616176 theme_park-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0     2072 2024-05-18 02:40:26.206357 theme_park-1.0.0/readme.md
--rwxr-xr-x   0        0        0     1155 2024-05-18 02:40:47.994115 theme_park-1.0.0/venue.S.HTML
--rwxr-xr-x   0        0        0       74 2024-04-08 20:59:40.730227 theme_park-1.0.0/venues/stages/theme_park/___objectives/itinerary - aspirations.S.HTML
--rwxr-xr-x   0        0        0      822 2024-05-18 02:40:44.022159 theme_park-1.0.0/venues/stages/theme_park/___objectives/itinerary.S.HTML
--rwxr-xr-x   0        0        0      574 2024-04-08 21:03:27.655704 theme_park-1.0.0/venues/stages/theme_park/___objectives/sequentials/sequentials.S.HTML
--rwxr-xr-x   0        0        0    51873 2024-03-17 02:26:50.689331 theme_park-1.0.0/venues/stages/theme_park/___objectives/sporatic/TradingView Screen.png
--rwxr-xr-x   0        0        0      381 2024-03-31 19:05:52.370949 theme_park-1.0.0/venues/stages/theme_park/___objectives/sporatic/itinerary.S.HTML
--rwxr-xr-x   0        0        0      225 2024-04-09 02:15:48.675989 theme_park-1.0.0/venues/stages/theme_park/__data_nodes/moon/clique.py
--rwxr-xr-x   0        0        0   845985 2024-04-05 04:00:12.449831 theme_park-1.0.0/venues/stages/theme_park/__data_nodes/moon/listing_status.csv
--rwxr-xr-x   0        0        0      499 2024-05-18 02:40:43.986160 theme_park-1.0.0/venues/stages/theme_park/__data_nodes/moon/mongo.S.HTML
--rwxr-xr-x   0        0        0      378 2024-05-18 02:40:44.038159 theme_park-1.0.0/venues/stages/theme_park/__glossary/theme_park_1
--rwxr-xr-x   0        0        0       45 2024-04-04 18:35:08.441995 theme_park-1.0.0/venues/stages/theme_park/__init__.py
--rwxr-xr-x   0        0        0     1945 2024-05-18 02:40:44.030159 theme_park-1.0.0/venues/stages/theme_park/_interfaces/clique/__init__.py
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 theme_park-1.0.0/venues/stages/theme_park/_interfaces/clique/group/__init__.py
--rwxr-xr-x   0        0        0       53 2024-03-31 19:15:22.692288 theme_park-1.0.0/venues/stages/theme_park/_interfaces/sanic_trails/strails.S.HTML
--rwxr-xr-x   0        0        0   246698 2024-05-18 02:41:07.817895 theme_park-1.0.0/venues/stages/theme_park/_status/DB/records.json
--rwxr-xr-x   0        0        0     1314 2024-04-17 00:35:43.012056 theme_park-1.0.0/venues/stages/theme_park/_status/clouds_status.proc.py
--rwxr-xr-x   0        0        0     1193 2024-04-17 00:35:40.616088 theme_park-1.0.0/venues/stages/theme_park/_status/status.proc.py
--rwxr-xr-x   0        0        0      114 2024-03-17 06:14:54.911123 theme_park-1.0.0/venues/stages/theme_park/_status/status_1.py
--rwxr-xr-x   0        0        0       53 2024-04-26 00:14:43.452870 theme_park-1.0.0/venues/stages/theme_park/adventures/adventures.S.HTML
--rwxr-xr-x   0        0        0      568 2024-04-26 01:07:20.514284 theme_park-1.0.0/venues/stages/theme_park/adventures/meter/meter.S.HTML
--rwxr-xr-x   0        0        0      129 2024-01-26 16:01:45.729782 theme_park-1.0.0/venues/stages/theme_park/charts/charts.s.HTML
--rwxr-xr-x   0        0        0      821 2024-03-17 23:24:26.718972 theme_park-1.0.0/venues/stages/theme_park/charts/plotly/plotly.s.HTML
--rwxr-xr-x   0        0        0      652 2024-05-18 02:40:43.990160 theme_park-1.0.0/venues/stages/theme_park/climate/__init__.py
--rwxr-xr-x   0        0        0       79 2024-05-12 03:05:51.809724 theme_park-1.0.0/venues/stages/theme_park/climate/climate.S.HTML
--rwxr-xr-x   0        0        0      170 2024-04-04 19:34:53.736179 theme_park-1.0.0/venues/stages/theme_park/clouds/AV/AV.s.HTML
--rwxr-xr-x   0        0        0      276 2024-03-17 21:13:24.014422 theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/Alpaca.s.HTML
--rwxr-xr-x   0        0        0      160 2024-04-09 00:53:14.647459 theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/_data_API/data.S.HTML
--rwxr-xr-x   0        0        0      795 2024-05-18 02:40:44.054159 theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/_data_API/v2/stock/symbol/bars.py
--rwxr-xr-x   0        0        0      761 2024-05-18 02:40:44.058159 theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/_status/API_status_1.py
--rwxr-xr-x   0        0        0      445 2024-05-18 02:40:44.058159 theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/crypto.S.HTML
--rwxr-xr-x   0        0        0      977 2024-05-18 02:40:44.058159 theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/retrieve.py
--rwxr-xr-x   0        0        0     1758 2024-05-18 02:40:44.058159 theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/structure_1.py
--rwxr-xr-x   0        0        0       83 2024-04-04 20:04:06.732691 theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/options/options.S.HTML
--rwxr-xr-x   0        0        0      390 2024-03-22 18:49:35.640871 theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/shares/retrieve_one.py
--rwxr-xr-x   0        0        0      979 2024-05-18 02:40:44.054159 theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/shares/retrieve_spans.py
--rwxr-xr-x   0        0        0      107 2024-03-17 18:08:13.242881 theme_park-1.0.0/venues/stages/theme_park/clouds/Bybit/Bybit.S.HTML
--rwxr-xr-x   0        0        0      171 2024-05-18 02:40:44.050159 theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/CCXT.s.HTML
--rwxr-xr-x   0        0        0     1036 2024-05-18 02:40:44.046159 theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/__init__.py
--rwxr-xr-x   0        0        0     1591 2024-05-18 02:40:44.046159 theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles/__init__.py
--rwxr-xr-x   0        0        0      565 2024-01-03 02:25:01.331601 theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles/candles.s.HTML
--rwxr-xr-x   0        0        0     2510 2024-05-18 02:40:44.046159 theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles_v1/__init__.py
--rwxr-xr-x   0        0        0      565 2024-01-03 02:25:01.331601 theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles_v1/candles.s.HTML
--rwxr-xr-x   0        0        0        3 2023-12-28 22:53:18.327445 theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/__init__.py
--rwxr-xr-x   0        0        0       62 2023-12-28 22:54:25.050671 theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/coinbase/coinbase.s.HTML
--rwxr-xr-x   0        0        0      359 2024-05-18 02:40:44.050159 theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/symbols/array.py
--rwxr-xr-x   0        0        0      331 2024-04-05 17:46:08.984778 theme_park-1.0.0/venues/stages/theme_park/clouds/Clouds Crypto.S.HTML
--rwxr-xr-x   0        0        0     1024 2024-05-18 02:40:44.062159 theme_park-1.0.0/venues/stages/theme_park/clouds/Clouds Shares.S.HTML
--rwxr-xr-x   0        0        0      597 2024-03-31 19:49:32.345940 theme_park-1.0.0/venues/stages/theme_park/clouds/Clouds.S.HTML
--rwxr-xr-x   0        0        0     2723 2024-05-18 02:40:44.050159 theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/API/__init__.py
--rwxr-xr-x   0        0        0      711 2024-05-18 02:40:44.050159 theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/API/accounts/__init__.py
--rwxr-xr-x   0        0        0     2039 2024-05-18 02:40:44.054159 theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/API/build_JWT.py
--rwxr-xr-x   0        0        0     1251 2024-05-18 02:40:44.054159 theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/API/orders/order_IDs.py
--rwxr-xr-x   0        0        0     3269 2024-05-18 02:40:44.050159 theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/API/products/candles.py
--rwxr-xr-x   0        0        0      972 2024-05-18 02:40:44.050159 theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/API/products/catalogue.py
--rwxr-xr-x   0        0        0      696 2024-05-18 02:40:44.054159 theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/Coinbase.s.HTML
--rwxr-xr-x   0        0        0     1540 2024-05-18 02:40:44.054159 theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/orders/place.py
--rwxr-xr-x   0        0        0      614 2023-11-25 04:03:55.921174 theme_park-1.0.0/venues/stages/theme_park/clouds/DOGE/doge.s.HTML
--rwxr-xr-x   0        0        0        0 2024-03-17 22:41:32.234375 theme_park-1.0.0/venues/stages/theme_park/clouds/Finnhub/Finnhub.S.HTML
--rwxr-xr-x   0        0        0       47 2024-03-24 04:04:49.775241 theme_park-1.0.0/venues/stages/theme_park/clouds/Finviz.com/Finviz.com.S.HTML
--rwxr-xr-x   0        0        0      193 2023-11-25 19:05:12.524729 theme_park-1.0.0/venues/stages/theme_park/clouds/LedgerX/LedgerX.s.HTML
--rwxr-xr-x   0        0        0       10 2023-12-12 05:12:16.566568 theme_park-1.0.0/venues/stages/theme_park/clouds/MQL5/MQL5.s.HTML
--rwxr-xr-x   0        0        0      226 2023-11-20 05:36:28.995516 theme_park-1.0.0/venues/stages/theme_park/clouds/Robinhood/Robinhood.s.HTML
--rwxr-xr-x   0        0        0       80 2024-03-17 22:16:54.374127 theme_park-1.0.0/venues/stages/theme_park/clouds/Tiingo/Tiingo.S.HTML
--rwxr-xr-x   0        0        0      126 2024-05-18 02:40:44.046159 theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/Tradier.s.HTML
--rwxr-xr-x   0        0        0      525 2024-05-18 02:40:44.046159 theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/_status/API_status_combine_1.py
--rwxr-xr-x   0        0        0       36 2024-04-04 19:14:12.097804 theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/procedures/exchanges/__init__.py
--rwxr-xr-x   0        0        0      122 2024-04-04 19:13:46.242103 theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/procedures/exchanges/exchanges.S.HTML
--rwxr-xr-x   0        0        0     1339 2024-05-18 02:40:44.038159 theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/procedures/options/combine.py
--rwxr-xr-x   0        0        0   220164 2023-11-21 17:07:07.643477 theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/procedures/options/example_responses/NOVA_options_chain.JSON
--rwxr-xr-x   0        0        0      212 2023-10-19 20:16:35.898645 theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/uo_tradier_api.s.HTML
--rwxr-xr-x   0        0        0     1128 2024-05-18 02:40:44.038159 theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/lookup/__init__.py
--rwxr-xr-x   0        0        0     1228 2024-05-18 02:40:44.042159 theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/options/chains/__init__.py
--rwxr-xr-x   0        0        0     1769 2024-04-04 20:05:04.392129 theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/options/chains/parse_1.py
--rwxr-xr-x   0        0        0      631 2024-05-18 02:40:44.042159 theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/options/expirations/__init__.py
--rwxr-xr-x   0        0        0      216 2024-03-18 04:26:59.460093 theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/TV.s.HTML
--rwxr-xr-x   0        0        0       77 2024-05-18 02:40:44.062159 theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/fluctuators/fluctuators.S.HTML
--rwxr-xr-x   0        0        0      300 2023-12-12 05:03:24.406023 theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/sensors/__init__.py
--rwxr-xr-x   0        0        0      237 2024-03-22 19:42:45.277679 theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/sensors/sensors.S.HTML
--rwxr-xr-x   0        0        0     3458 2024-03-17 05:35:01.529000 theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/treasure/indicators/RMI_Trend_Sniper.pine
--rwxr-xr-x   0        0        0      163 2024-03-17 05:34:46.185162 theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/treasure/indicators/indicators.S.HTML
--rwxr-xr-x   0        0        0     3830 2024-05-18 02:40:44.062159 theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals/__init__.py
--rwxr-xr-x   0        0        0     1508 2024-05-18 02:40:44.058159 theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals_v2/__init__.py
--rwxr-xr-x   0        0        0      813 2024-03-22 19:47:25.962582 theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py
--rwxr-xr-x   0        0        0     1829 2024-03-22 19:46:48.770994 theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py
--rwxr-xr-x   0        0        0      495 2024-03-28 00:15:40.797119 theme_park-1.0.0/venues/stages/theme_park/clouds/USA/IRS/IRA/IRA.S.HTML
--rwxr-xr-x   0        0        0      407 2024-05-18 02:40:44.046159 theme_park-1.0.0/venues/stages/theme_park/clouds/USA/IRS/taxes/income/__init__.py
--rwxr-xr-x   0        0        0       60 2023-11-10 17:23:06.947404 theme_park-1.0.0/venues/stages/theme_park/clouds/USA/SEC/6K/__init__.py
--rwxr-xr-x   0        0        0      496 2023-11-10 17:40:32.497079 theme_park-1.0.0/venues/stages/theme_park/clouds/USA/SEC/balance_sheets/__init__.py
--rwxr-xr-x   0        0        0       18 2023-11-10 17:15:04.345938 theme_park-1.0.0/venues/stages/theme_park/clouds/USA/SEC/balance_sheets/balance_sheets.s.HTML
--rwxr-xr-x   0        0        0      198 2023-11-10 17:28:03.521299 theme_park-1.0.0/venues/stages/theme_park/clouds/USA/SEC/balance_sheets/equity/__init__.py
--rwxr-xr-x   0        0        0      420 2023-11-10 17:53:32.039501 theme_park-1.0.0/venues/stages/theme_park/clouds/USA/SEC/income/__init__.py
--rwxr-xr-x   0        0        0       51 2023-11-10 17:34:28.536151 theme_park-1.0.0/venues/stages/theme_park/clouds/USA/SEC/income/income.s.HTML
--rwxr-xr-x   0        0        0        0 2023-11-09 20:40:55.437403 theme_park-1.0.0/venues/stages/theme_park/clouds/USA/SEC/statements.s.HTML
--rwxr-xr-x   0        0        0      212 2023-11-14 04:12:06.841989 theme_park-1.0.0/venues/stages/theme_park/clouds/Yahoo/Yahoo.s.HTML
--rwxr-xr-x   0        0        0     1821 2024-05-18 02:40:44.046159 theme_park-1.0.0/venues/stages/theme_park/clouds/Yahoo/retrieve.py
--rwxr-xr-x   0        0        0      931 2024-05-18 02:40:44.046159 theme_park-1.0.0/venues/stages/theme_park/clouds/Yahoo/retrieve_change.py
--rwxr-xr-x   0        0        0       32 2023-11-14 05:19:00.214473 theme_park-1.0.0/venues/stages/theme_park/clouds/twelve_data/twelve_data.s.HTML
--rwxr-xr-x   0        0        0       16 2024-03-24 03:14:51.054648 theme_park-1.0.0/venues/stages/theme_park/emojis.MD
--rwxr-xr-x   0        0        0     2589 2023-11-14 05:42:13.790956 theme_park-1.0.0/venues/stages/theme_park/fluctuators/bt/strategies/example_1.py
--rwxr-xr-x   0        0        0      130 2024-04-08 20:48:05.178188 theme_park-1.0.0/venues/stages/theme_park/fluctuators/fluctuators - itinerary.s.HTML
--rwxr-xr-x   0        0        0      787 2024-04-08 20:48:43.589745 theme_park-1.0.0/venues/stages/theme_park/fluctuators/fluctuators.S.HTML
--rwxr-xr-x   0        0        0      121 2023-11-28 03:26:29.420655 theme_park-1.0.0/venues/stages/theme_park/fluctuators/lumi/lumi.s.HTML
--rwxr-xr-x   0        0        0      100 2023-12-19 04:49:40.656260 theme_park-1.0.0/venues/stages/theme_park/fluctuators/rover_1/rover_1.s.HTML
--rwxr-xr-x   0        0        0      443 2024-05-18 02:40:43.998160 theme_park-1.0.0/venues/stages/theme_park/gadgets/clock/UTC/ISO.py
--rwxr-xr-x   0        0        0      349 2024-05-18 02:40:43.998160 theme_park-1.0.0/venues/stages/theme_park/gadgets/clock/UTC/current.py
--rwxr-xr-x   0        0        0      981 2024-05-18 02:40:43.998160 theme_park-1.0.0/venues/stages/theme_park/gadgets/clock/UTC/greatness_1.py
--rwxr-xr-x   0        0        0      288 2024-04-09 02:03:24.336835 theme_park-1.0.0/venues/stages/theme_park/gadgets/clock/clock.s.HTML
--rwxr-xr-x   0        0        0      620 2023-11-09 20:46:40.432504 theme_park-1.0.0/venues/stages/theme_park/gadgets/format_percentage.py
--rwxr-xr-x   0        0        0      151 2023-11-23 05:19:27.179399 theme_park-1.0.0/venues/stages/theme_park/gadgets/math/slope/__init__.py
--rwxr-xr-x   0        0        0       79 2024-01-10 05:54:37.773115 theme_park-1.0.0/venues/stages/theme_park/gadgets/pandas/DF/DF.s.HTML
--rwxr-xr-x   0        0        0      513 2024-05-18 02:40:43.994160 theme_park-1.0.0/venues/stages/theme_park/gadgets/pandas/DF/_status/status_from_1.py
--rwxr-xr-x   0        0        0      249 2024-05-18 02:40:43.994160 theme_park-1.0.0/venues/stages/theme_park/gadgets/pandas/DF/from_list.py
--rwxr-xr-x   0        0        0      323 2024-05-18 02:40:43.994160 theme_park-1.0.0/venues/stages/theme_park/gadgets/pandas/DF/to_list.py
--rwxr-xr-x   0        0        0      690 2024-01-13 06:12:46.871796 theme_park-1.0.0/venues/stages/theme_park/gadgets/pandas/pandas.s.HTML
--rwxr-xr-x   0        0        0      399 2024-05-18 02:40:43.994160 theme_park-1.0.0/venues/stages/theme_park/gadgets/ratio.py
--rwxr-xr-x   0        0        0      454 2024-05-18 02:40:43.990160 theme_park-1.0.0/venues/stages/theme_park/gadgets/summation/__init__.py
--rwxr-xr-x   0        0        0      374 2024-05-18 02:40:43.990160 theme_park-1.0.0/venues/stages/theme_park/gadgets/summation/status_1.py
--rwxr-xr-x   0        0        0    18282 2023-12-28 23:17:20.176165 theme_park-1.0.0/venues/stages/theme_park/gadgets/summation/summation.svg
--rwxr-xr-x   0        0        0      100 2024-04-09 02:03:10.212995 theme_park-1.0.0/venues/stages/theme_park/gadgets/tools.s.HTML
--rwxr-xr-x   0        0        0     2072 2024-05-18 02:40:44.038159 theme_park-1.0.0/venues/stages/theme_park/home.MD
--rwxr-xr-x   0        0        0     1075 2024-05-18 02:40:44.062159 theme_park-1.0.0/venues/stages/theme_park/home.s.HTML
--rwxr-xr-x   0        0        0      305 2024-04-26 00:08:58.840689 theme_park-1.0.0/venues/stages/theme_park/platforms/accounts/accounts.S.HTML
--rwxr-xr-x   0        0        0      142 2024-04-26 01:32:14.574003 theme_park-1.0.0/venues/stages/theme_park/platforms/biorecon/biorecon.S.HTML
--rwxr-xr-x   0        0        0      503 2024-04-26 00:27:03.696837 theme_park-1.0.0/venues/stages/theme_park/platforms/platforms.S.HTML
--rwxr-xr-x   0        0        0      425 2024-04-09 02:33:16.647876 theme_park-1.0.0/venues/stages/theme_park/rides/rides - formats.S.HTML
--rwxr-xr-x   0        0        0      115 2024-04-27 16:24:01.727436 theme_park-1.0.0/venues/stages/theme_park/rides/rides - objectives possibilities.S.HTML
--rwxr-xr-x   0        0        0      321 2024-04-27 16:19:46.237010 theme_park-1.0.0/venues/stages/theme_park/rides/rides - objectives.S.HTML
--rwxr-xr-x   0        0        0     1416 2024-05-18 02:40:44.014159 theme_park-1.0.0/venues/stages/theme_park/rides/rides.S.HTML
--rwxr-xr-x   0        0        0      489 2023-12-31 05:03:05.192136 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/ATR/ATR.s.HTML
--rwxr-xr-x   0        0        0     2941 2024-05-18 02:40:44.018159 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py
--rwxr-xr-x   0        0        0     1585 2024-05-18 02:40:44.018159 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/ATR/__init__.py
--rwxr-xr-x   0        0        0     1239 2024-05-18 02:40:44.018159 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/ATR/_status/status_1.py
--rwxr-xr-x   0        0        0     1731 2024-01-02 03:23:31.042432 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/Andean_Oscillator/AO.pine
--rwxr-xr-x   0        0        0      134 2023-12-01 02:49:14.211328 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/Andean_Oscillator/Andean.r.HTML
--rwxr-xr-x   0        0        0      273 2023-12-31 06:36:06.223233 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/EMA/EMA.s.HTML
--rwxr-xr-x   0        0        0       82 2023-11-14 05:05:08.114737 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/EMA/__init__.py
--rwxr-xr-x   0        0        0     4821 2024-01-02 03:23:31.085431 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/HHLL/indicator.pine
--rwxr-xr-x   0        0        0       72 2023-12-03 22:10:44.686991 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/MA/MA.r.HTML
--rwxr-xr-x   0        0        0       91 2023-12-12 04:16:31.428608 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/MACD/MACD.s.HTML
--rwxr-xr-x   0        0        0       48 2023-12-02 00:37:47.807470 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/QQE/QQE.r.HTML
--rwxr-xr-x   0        0        0      201 2023-12-03 02:58:48.769709 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/RSI/RSI.r.HTML
--rwxr-xr-x   0        0        0      779 2024-05-18 02:40:44.014159 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/RSI/__init__.py
--rwxr-xr-x   0        0        0      250 2024-01-02 06:36:59.547427 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/SMA/__init__.py
--rwxr-xr-x   0        0        0      397 2024-01-02 03:23:31.177430 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/TR/TR.s.HTML
--rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/TR/True Range.svg
--rwxr-xr-x   0        0        0     1625 2024-05-18 02:40:44.014159 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/TR/__init__.py
--rwxr-xr-x   0        0        0      520 2024-05-18 02:40:44.014159 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/TR/_status/status_1.py
--rwxr-xr-x   0        0        0      789 2024-05-18 02:40:44.018159 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/TR/_status/status_2.py
--rwxr-xr-x   0        0        0      254 2023-11-29 18:25:15.058846 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/TV.r.HTML
--rwxr-xr-x   0        0        0       46 2023-11-21 16:46:45.097491 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/VWAP/VWAP.r.HTML
--rwxr-xr-x   0        0        0      590 2024-05-18 02:40:44.014159 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/VWAP/__init__.py
--rwxr-xr-x   0        0        0       47 2023-11-21 16:46:17.697805 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/VWMA/VWMA.r.HTML
--rwxr-xr-x   0        0        0       24 2023-11-14 04:28:20.239207 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/bolinger_bands/bolinger_bands.r.html
--rwxr-xr-x   0        0        0        0 2023-11-30 18:13:51.268620 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/chandlier_exit/chandelier exit.r.HTML
--rwxr-xr-x   0        0        0      543 2024-05-18 02:40:44.014159 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/indicators.s.HTML
--rwxr-xr-x   0        0        0     1266 2024-01-02 03:23:31.097431 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/pivot_point/pivot_point.s.HTML
--rwxr-xr-x   0        0        0       28 2023-11-21 16:43:07.835981 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/relative_volume/relative volume.r.HTML
--rwxr-xr-x   0        0        0     2829 2024-05-18 02:40:44.018159 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py
--rwxr-xr-x   0        0        0     1092 2024-05-18 02:40:44.018159 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/supertrend/__init__.py
--rwxr-xr-x   0        0        0     1240 2024-05-18 02:40:44.018159 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/supertrend/_status/status_1.py
--rwxr-xr-x   0        0        0      358 2024-01-06 00:03:10.850549 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/supertrend/pandas_ta/__init__.py
--rwxr-xr-x   0        0        0      225 2023-12-03 02:59:17.552392 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/supertrend/supertrend.s.HTML
--rwxr-xr-x   0        0        0        0 2024-01-02 03:30:08.272935 theme_park-1.0.0/venues/stages/theme_park/rides/season_1/supertrend2/__init__.py
--rwxr-xr-x   0        0        0     1209 2024-05-18 02:40:44.002159 theme_park-1.0.0/venues/stages/theme_park/rides/season_2/AAS/__init__.py
--rwxr-xr-x   0        0        0     1227 2024-05-18 02:40:44.002159 theme_park-1.0.0/venues/stages/theme_park/rides/season_2/AAS/_status/status_1.py
--rwxr-xr-x   0        0        0      334 2024-01-06 07:25:23.819962 theme_park-1.0.0/venues/stages/theme_park/rides/season_2/AS/AS.s.HTML
--rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 theme_park-1.0.0/venues/stages/theme_park/rides/season_2/AS/AS.svg
--rwxr-xr-x   0        0        0     1541 2024-05-18 02:40:43.998160 theme_park-1.0.0/venues/stages/theme_park/rides/season_2/AS/__init__.py
--rwxr-xr-x   0        0        0      508 2024-05-18 02:40:43.998160 theme_park-1.0.0/venues/stages/theme_park/rides/season_2/AS/_status/status_1.py
--rwxr-xr-x   0        0        0      780 2024-05-18 02:40:43.998160 theme_park-1.0.0/venues/stages/theme_park/rides/season_2/AS/_status/status_2.py
--rwxr-xr-x   0        0        0     1093 2024-01-06 07:15:37.995569 theme_park-1.0.0/venues/stages/theme_park/rides/season_2/pecdency/__init__.py
--rwxr-xr-x   0        0        0     1344 2024-05-18 02:40:43.998160 theme_park-1.0.0/venues/stages/theme_park/rides/season_2/pecdency/__init__v1.py
--rwxr-xr-x   0        0        0     4110 2024-05-18 02:40:44.002159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/ST/__init__.py
--rwxr-xr-x   0        0        0      430 2024-05-18 02:40:44.010159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/VDA/__init__.py
--rwxr-xr-x   0        0        0      564 2024-05-18 02:40:44.006159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/VSA/__init__.py
--rwxr-xr-x   0        0        0      334 2024-01-09 01:54:38.423714 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span/AS.s.HTML
--rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span/AS.svg
--rwxr-xr-x   0        0        0     1554 2024-05-18 02:40:44.006159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span/__init__.py
--rwxr-xr-x   0        0        0      519 2024-05-18 02:40:44.006159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span/_status/status_1.py
--rwxr-xr-x   0        0        0      787 2024-05-18 02:40:44.010159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span/_status/status_2.py
--rwxr-xr-x   0        0        0     1177 2024-05-18 02:40:44.002159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span_average/__init__.py
--rwxr-xr-x   0        0        0     1245 2024-05-18 02:40:44.002159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span_average/_status/status_1.py
--rwxr-xr-x   0        0        0     3679 2024-05-18 02:40:44.010159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span_reversals/__init__.py
--rwxr-xr-x   0        0        0     3577 2024-05-18 02:40:44.006159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span_roads_v1/__init__.py
--rwxr-xr-x   0        0        0     3859 2024-05-18 02:40:44.006159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/super_hero_trend/__init__.py
--rwxr-xr-x   0        0        0     1756 2024-05-18 02:40:44.006159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/super_hero_trend/win_rates/shares_trading.py
--rwxr-xr-x   0        0        0      958 2024-05-18 02:40:44.006159 theme_park-1.0.0/venues/stages/theme_park/rides/season_3/supertrend/__init__.py
--rwxr-xr-x   0        0        0     1822 2024-05-18 02:40:44.014159 theme_park-1.0.0/venues/stages/theme_park/rides/season_4/AO/__init__.py
--rwxr-xr-x   0        0        0     5968 2024-04-11 03:49:19.489710 theme_park-1.0.0/venues/stages/theme_park/rides/season_4/ML_Lorentzian/KernelFunctions.ps
--rwxr-xr-x   0        0        0    36151 2024-04-11 03:49:38.505474 theme_park-1.0.0/venues/stages/theme_park/rides/season_4/ML_Lorentzian/Lorentzian Classification.ps
--rwxr-xr-x   0        0        0    18799 2024-04-11 03:48:20.246452 theme_park-1.0.0/venues/stages/theme_park/rides/season_4/ML_Lorentzian/MLExtensions.ps
--rwxr-xr-x   0        0        0     3923 2024-05-18 02:40:44.010159 theme_park-1.0.0/venues/stages/theme_park/rides/season_4/superb/__init__.py
--rwxr-xr-x   0        0        0       13 2024-02-01 15:34:15.615610 theme_park-1.0.0/venues/stages/theme_park/rides/season_4/superb/superb.s.HTML
--rwxr-xr-x   0        0        0     1783 2024-05-18 02:40:44.010159 theme_park-1.0.0/venues/stages/theme_park/rides/season_4/superb/win_rates/shares_trading.py
--rwxr-xr-x   0        0        0     3997 2024-05-18 02:40:43.982160 theme_park-1.0.0/venues/stages/theme_park/scans/_clique/ETF.py
--rwxr-xr-x   0        0        0        2 2024-04-04 18:06:03.015402 theme_park-1.0.0/venues/stages/theme_park/scans/_clique/REIT.py
--rwxr-xr-x   0        0        0     2159 2024-05-18 02:40:43.986160 theme_park-1.0.0/venues/stages/theme_park/scans/_clique/TV.py
--rwxr-xr-x   0        0        0     1408 2024-05-18 02:40:43.982160 theme_park-1.0.0/venues/stages/theme_park/scans/_clique/currency.py
--rwxr-xr-x   0        0        0       42 2024-04-04 18:06:43.814870 theme_park-1.0.0/venues/stages/theme_park/scans/_clique/penny_stocks.py
--rwxr-xr-x   0        0        0      412 2024-05-18 02:40:43.986160 theme_park-1.0.0/venues/stages/theme_park/scans/clique.py
--rwxr-xr-x   0        0        0      180 2024-04-15 19:29:36.357014 theme_park-1.0.0/venues/stages/theme_park/scans/screeners.S.HTML
--rwxr-xr-x   0        0        0      116 2024-05-18 02:40:43.986160 theme_park-1.0.0/venues/stages/theme_park/scans/symbol/__init__.py
--rwxr-xr-x   0        0        0      938 2024-05-18 02:40:43.986160 theme_park-1.0.0/venues/stages/theme_park/scans/symbol/symbols.S.HTML
--rwxr-xr-x   0        0        0       84 2024-04-08 20:53:48.054233 theme_park-1.0.0/venues/stages/theme_park/stats/VHLOC/MACD/MACD.S.HTML
--rwxr-xr-x   0        0        0      102 2024-05-18 02:40:44.022159 theme_park-1.0.0/venues/stages/theme_park/stats/VHLOC/MACD/__init__.py
--rwxr-xr-x   0        0        0        0 2024-04-08 20:53:19.026568 theme_park-1.0.0/venues/stages/theme_park/stats/VHLOC/MACD/procedure.ps
--rwxr-xr-x   0        0        0     5111 2024-05-18 02:40:44.026159 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/__init__.py
--rwxr-xr-x   0        0        0     1952 2024-05-18 02:40:44.030159 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/squeeze pc ratios.r.HTML
--rwxr-xr-x   0        0        0   388314 2023-11-09 20:42:52.592079 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/examples/1.JSON
--rwxr-xr-x   0        0        0     1567 2023-11-09 20:42:52.591079 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/examples/2.JSON
--rwxr-xr-x   0        0        0      590 2024-05-18 02:40:44.026159 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/status_1.py
--rwxr-xr-x   0        0        0     1857 2024-05-18 02:40:44.030159 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/status_2.py
--rwxr-xr-x   0        0        0     2902 2024-05-18 02:40:44.022159 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/__init__.py
--rwxr-xr-x   0        0        0     2290 2023-12-04 02:47:32.197228 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/examples/0.JSON
--rwxr-xr-x   0        0        0   388314 2023-11-09 20:42:52.592079 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/examples/1.JSON
--rwxr-xr-x   0        0        0     1567 2023-11-09 20:42:52.591079 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/examples/2.JSON
--rwxr-xr-x   0        0        0     1502 2024-05-18 02:40:44.022159 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/status_1.py
--rwxr-xr-x   0        0        0      788 2024-05-18 02:40:44.026159 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/status_2.py
--rwxr-xr-x   0        0        0      997 2024-05-18 02:40:44.022159 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/aggregate break even.s.HTML
--rwxr-xr-x   0        0        0        0 2024-03-31 19:07:37.005708 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/clique.py
--rwxr-xr-x   0        0        0      889 2024-05-18 02:40:44.022159 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/show/__init__.py
--rwxr-xr-x   0        0        0     1599 2024-03-31 18:39:18.393448 theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_multiplier/aggregate_multipliers.r.HTML
--rwxr-xr-x   0        0        0     1409 2024-05-18 02:40:44.026159 theme_park-1.0.0/venues/stages/theme_park/stats/clique.py
--rwxr-xr-x   0        0        0      311 2024-04-05 04:21:31.280203 theme_park-1.0.0/venues/stages/theme_park/stats/option_priceyness/option_priceyness.S.HTML
--rwxr-xr-x   0        0        0      616 2024-05-04 03:34:27.890705 theme_park-1.0.0/venues/stages/theme_park/stats/stats.s.HTML
--rwxr-xr-x   0        0        0      349 2024-05-18 02:40:44.022159 theme_park-1.0.0/venues/stages/theme_park/stats/the_multiplier/__init__.py
--rwxr-xr-x   0        0        0      911 2024-03-17 21:11:40.987538 theme_park-1.0.0/venues/stages/theme_park/treasures/commodities/commodities.s.HTML
--rwxr-xr-x   0        0        0       89 2024-04-08 22:27:54.205084 theme_park-1.0.0/venues/stages/theme_park/treasures/contracts/contracts.S.HTML
--rwxr-xr-x   0        0        0      339 2024-04-13 19:27:27.156565 theme_park-1.0.0/venues/stages/theme_park/treasures/crypto/L1/L1.S.HTML
--rwxr-xr-x   0        0        0      725 2024-04-13 19:19:01.872575 theme_park-1.0.0/venues/stages/theme_park/treasures/crypto/crypto.S.HTML
--rwxr-xr-x   0        0        0       61 2024-04-13 19:26:04.032669 theme_park-1.0.0/venues/stages/theme_park/treasures/crypto/crypto_rust.S.HTML
--rwxr-xr-x   0        0        0      641 2024-04-13 19:19:32.260629 theme_park-1.0.0/venues/stages/theme_park/treasures/crypto/crypto_usual_features.S.HTML
--rwxr-xr-x   0        0        0      127 2024-04-25 23:58:14.336246 theme_park-1.0.0/venues/stages/theme_park/treasures/forex/forex.s.HTML
--rwxr-xr-x   0        0        0       75 2024-01-30 00:33:10.380046 theme_park-1.0.0/venues/stages/theme_park/treasures/futures/futures.s.HTML
--rwxr-xr-x   0        0        0      186 2024-04-19 20:08:05.560255 theme_park-1.0.0/venues/stages/theme_park/treasures/gems/gems.S.HTML
--rwxr-xr-x   0        0        0       48 2024-04-08 17:11:40.338334 theme_park-1.0.0/venues/stages/theme_park/treasures/options/greeks/greeks.S.HTML
--rwxr-xr-x   0        0        0     1562 2024-05-18 02:40:43.982160 theme_park-1.0.0/venues/stages/theme_park/treasures/options/movement_calculator/__init__.py
--rwxr-xr-x   0        0        0     1167 2023-11-23 05:20:06.387999 theme_park-1.0.0/venues/stages/theme_park/treasures/options/movement_calculator/slope.s.HTML
--rwxr-xr-x   0        0        0     2569 2024-05-18 02:40:43.982160 theme_park-1.0.0/venues/stages/theme_park/treasures/options/multipliers/__init__.py
--rwxr-xr-x   0        0        0      358 2024-04-08 17:12:06.086114 theme_park-1.0.0/venues/stages/theme_park/treasures/options/options.s.HTML
--rwxr-xr-x   0        0        0     1495 2024-05-18 02:40:43.982160 theme_park-1.0.0/venues/stages/theme_park/treasures/options/shapes/shape_1/__init__.py
--rwxr-xr-x   0        0        0      489 2023-11-21 17:09:02.275163 theme_park-1.0.0/venues/stages/theme_park/treasures/options/shapes/shape_1/shape_1.s.HTML
--rwxr-xr-x   0        0        0      144 2024-05-18 02:40:43.978160 theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/__init__.py
--rwxr-xr-x   0        0        0      156 2024-04-08 23:27:06.857428 theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/loans/loans.S.HTML
--rwxr-xr-x   0        0        0      431 2024-04-08 21:38:29.659326 theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/constant.py
--rwxr-xr-x   0        0        0       95 2024-04-08 21:54:20.848024 theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/insurance/insurance.S.HTML
--rwxr-xr-x   0        0        0      587 2024-04-08 22:05:05.892491 theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/loan - varieties.S.HTML
--rwxr-xr-x   0        0        0     1202 2024-04-08 22:40:59.788117 theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/loan.S.HTML
--rwxr-xr-x   0        0        0     1463 2024-04-09 00:50:23.861466 theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/sources/sources.S.HTML
--rwxr-xr-x   0        0        0      414 2024-04-08 22:42:58.322845 theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/real_estate.S.HTML
--rwxr-xr-x   0        0        0      437 2024-04-08 21:43:11.491928 theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/sends.S.HTML
--rwxr-xr-x   0        0        0      127 2024-04-08 21:37:42.099907 theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/tax/__init__.py
--rwxr-xr-x   0        0        0       97 2024-04-08 21:48:11.608365 theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/tax/tax.S.HTML
--rwxr-xr-x   0        0        0     2434 2024-04-08 22:08:51.961985 theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/varieties/varieties.S.HTML
--rwxr-xr-x   0        0        0     1190 2024-03-31 19:49:32.365940 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/ETF/ETF.s.HTML
--rwxr-xr-x   0        0        0      114 2023-11-15 06:29:25.238807 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/ETF/comprehensive/comprehensive.s.HTML
--rwxr-xr-x   0        0        0       42 2023-11-15 06:37:06.461104 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/ETF/sectors/airlines/airlines.r.HTML
--rwxr-xr-x   0        0        0       45 2023-11-15 06:38:49.083268 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/ETF/sectors/electronics/semiconductors.r.HTML
--rwxr-xr-x   0        0        0       81 2023-11-15 06:34:55.671168 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/ETF/sectors/farming/farming.r.HTML
--rwxr-xr-x   0        0        0       84 2023-11-15 06:37:33.924880 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/ETF/sectors/real estate/real estate.r.HTML
--rwxr-xr-x   0        0        0      157 2024-03-17 04:50:30.861349 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/ETF/sectors/sectors.S.HTML
--rwxr-xr-x   0        0        0       14 2023-11-15 06:36:56.273187 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/ETF/sectors/vehicles/vehicles.r.HTML
--rwxr-xr-x   0        0        0        7 2024-03-24 04:01:12.905095 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/__init__.py
--rwxr-xr-x   0        0        0       13 2023-11-15 06:11:36.293215 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/companies/companies.s.HTML
--rwxr-xr-x   0        0        0       11 2023-11-21 16:53:15.238020 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/shapes/shape_1/__init__.py
--rwxr-xr-x   0        0        0      135 2023-11-21 16:52:53.862265 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/shapes/shape_1/shape_1.s.HTML
--rwxr-xr-x   0        0        0      106 2024-04-08 19:07:13.173774 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/shares.s.HTML
--rwxr-xr-x   0        0        0       43 2023-11-17 19:16:25.824071 theme_park-1.0.0/venues/stages/theme_park/treasures/shares/splits.s.HTML
--rwxr-xr-x   0        0        0       90 2024-04-08 19:06:53.069998 theme_park-1.0.0/venues/stages/theme_park/treasures/treasures.s.HTML
--rw-r--r--   0        0        0     4452 1970-01-01 00:00:00.000000 theme_park-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     2332 2024-05-27 03:18:12.977012 theme_park-2.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0     2072 2024-05-18 02:40:26.206357 theme_park-2.0.0/readme.md
+-rwxr-xr-x   0        0        0     1246 2024-05-27 02:45:44.533548 theme_park-2.0.0/venue.S.HTML
+-rwxr-xr-x   0        0        0      899 2024-05-26 02:31:15.624142 theme_park-2.0.0/venues/stages/theme_park/[_quests]/quests.S.HTML
+-rwxr-xr-x   0        0        0       74 2024-04-08 20:59:40.730227 theme_park-2.0.0/venues/stages/theme_park/[_quests]/quests: tough.S.HTML
+-rwxr-xr-x   0        0        0      574 2024-04-08 21:03:27.655704 theme_park-2.0.0/venues/stages/theme_park/[_quests]/sequentials/sequentials.S.HTML
+-rwxr-xr-x   0        0        0    51873 2024-03-17 02:26:50.689331 theme_park-2.0.0/venues/stages/theme_park/[_quests]/sporatic/TradingView Screen.png
+-rwxr-xr-x   0        0        0      381 2024-03-31 19:05:52.370949 theme_park-2.0.0/venues/stages/theme_park/[_quests]/sporatic/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      225 2024-04-09 02:15:48.675989 theme_park-2.0.0/venues/stages/theme_park/__data_nodes/moon/clique.py
+-rwxr-xr-x   0        0        0   845985 2024-04-05 04:00:12.449831 theme_park-2.0.0/venues/stages/theme_park/__data_nodes/moon/listing_status.csv
+-rwxr-xr-x   0        0        0      499 2024-05-18 02:40:43.986160 theme_park-2.0.0/venues/stages/theme_park/__data_nodes/moon/mongo.S.HTML
+-rwxr-xr-x   0        0        0      378 2024-05-18 02:40:44.038159 theme_park-2.0.0/venues/stages/theme_park/__glossary/theme_park_1
+-rwxr-xr-x   0        0        0       34 2024-05-27 02:47:58.716067 theme_park-2.0.0/venues/stages/theme_park/__init__.py
+-rwxr-xr-x   0        0        0     2139 2024-05-27 03:11:31.525345 theme_park-2.0.0/venues/stages/theme_park/_clique/__init__.py
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 theme_park-2.0.0/venues/stages/theme_park/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0     1162 2024-05-27 03:07:13.892068 theme_park-2.0.0/venues/stages/theme_park/_essence/__init__.py
+-rwxr-xr-x   0        0        0     2438 2024-05-13 00:59:57.240563 theme_park-2.0.0/venues/stages/theme_park/_essence/activate_alert--/__init__.py
+-rwxr-xr-x   0        0        0      505 2024-05-13 00:59:57.240563 theme_park-2.0.0/venues/stages/theme_park/_essence/activate_alert--/parse_exception.py
+-rwxr-xr-x   0        0        0      202 2024-04-27 16:49:31.955662 theme_park-2.0.0/venues/stages/theme_park/_essence/essence.S.HTML
+-rwxr-xr-x   0        0        0     3748 2024-05-27 03:13:49.959860 theme_park-2.0.0/venues/stages/theme_park/_essence/merge/__init__.py
+-rwxr-xr-x   0        0        0      719 2024-05-02 02:39:12.702510 theme_park-2.0.0/venues/stages/theme_park/_essence/scan/__init__.py
+-rwxr-xr-x   0        0        0      855 2024-05-27 03:10:48.409805 theme_park-2.0.0/venues/stages/theme_park/_essence/seek/__init__.py
+-rwxr-xr-x   0        0        0   246698 2024-05-18 02:41:07.817895 theme_park-2.0.0/venues/stages/theme_park/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1314 2024-04-17 00:35:43.012056 theme_park-2.0.0/venues/stages/theme_park/_status/clouds_status.proc.py
+-rwxr-xr-x   0        0        0     1193 2024-04-17 00:35:40.616088 theme_park-2.0.0/venues/stages/theme_park/_status/status.proc.py
+-rwxr-xr-x   0        0        0      114 2024-03-17 06:14:54.911123 theme_park-2.0.0/venues/stages/theme_park/_status/status_1.py
+-rwxr-xr-x   0        0        0       53 2024-04-26 00:14:43.452870 theme_park-2.0.0/venues/stages/theme_park/adventures/adventures.S.HTML
+-rwxr-xr-x   0        0        0     2486 2024-05-27 03:02:15.775114 theme_park-2.0.0/venues/stages/theme_park/adventures/alerting/__init__.py
+-rwxr-xr-x   0        0        0      505 2024-05-13 00:59:57.232563 theme_park-2.0.0/venues/stages/theme_park/adventures/alerting/parse_exception.py
+-rwxr-xr-x   0        0        0     1327 2024-01-25 05:00:54.191593 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/HA.s.HTML
+-rwxr-xr-x   0        0        0      238 2023-12-02 04:53:31.462384 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/SSL/SSL.r.HTML
+-rwxr-xr-x   0        0        0      985 2023-12-14 02:01:36.217926 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/SSL/__init__.py
+-rwxr-xr-x   0        0        0     1757 2023-12-01 23:15:16.435121 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/SSL/certificate.pem
+-rwxr-xr-x   0        0        0     3272 2023-12-01 23:15:16.430121 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/SSL/certificate.pem.key
+-rwxr-xr-x   0        0        0      346 2023-12-01 18:00:33.471576 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/__init__.py
+-rwxr-xr-x   0        0        0      344 2024-05-26 04:21:07.379855 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/_controls/_clique.py
+-rwxr-xr-x   0        0        0      315 2024-05-27 03:12:23.864785 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/_controls/build.py
+-rwxr-xr-x   0        0        0      625 2024-05-27 03:12:23.880785 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/_controls/is_on.py
+-rwxr-xr-x   0        0        0       77 2024-05-10 01:44:23.514282 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/_controls/off.py
+-rwxr-xr-x   0        0        0     1141 2024-05-27 03:12:23.892785 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/_controls/on.py
+-rwxr-xr-x   0        0        0     1295 2023-12-02 01:06:44.630336 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/configs/HTTPS_to_HTTP/1.py
+-rwxr-xr-x   0        0        0      567 2023-12-04 23:16:04.198925 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/configs/HTTPS_to_HTTP/HTTPS_to_HTTP.s.HTML
+-rwxr-xr-x   0        0        0     1895 2024-05-27 03:12:23.904785 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/configs/HTTPS_to_HTTP/__init__.py
+-rwxr-xr-x   0        0        0     1296 2023-12-01 22:31:43.018311 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/configs/HTTP_balancer/__init__.py
+-rwxr-xr-x   0        0        0      277 2023-12-01 21:44:47.102165 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/configs/HTTP_balancer/examples/example_1.cfg
+-rwxr-xr-x   0        0        0     3286 2023-12-01 18:05:41.851249 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/configs/examples/haproxy.cfg
+-rwxr-xr-x   0        0        0     2457 2023-12-01 21:46:11.432916 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/configs/examples/haproxy_2.cfg
+-rwxr-xr-x   0        0        0     2191 2024-01-25 05:03:52.719628 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/configs/external_reverse/__init__.py
+-rwxr-xr-x   0        0        0      217 2024-05-10 00:51:31.625386 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/demux.S.HTML
+-rwxr-xr-x   0        0        0      229 2023-12-02 01:03:02.539647 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/journalctl/journalctl.r.HTML
+-rwxr-xr-x   0        0        0      227 2023-12-02 01:02:28.789164 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/systemctl/systemctl.S.HTML
+-rwxr-xr-x   0        0        0      454 2024-05-27 03:12:23.904785 theme_park-2.0.0/venues/stages/theme_park/adventures/demux_hap/venture.py
+-rwxr-xr-x   0        0        0      568 2024-04-26 01:07:20.514284 theme_park-2.0.0/venues/stages/theme_park/adventures/meter/meter.S.HTML
+-rwxr-xr-x   0        0        0       14 2024-04-24 01:06:32.184393 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/.gitignore
+-rwxr-xr-x   0        0        0      772 2024-05-26 02:25:44.135938 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/_controls/_clique.py
+-rwxr-xr-x   0        0        0      758 2024-05-26 02:25:44.155938 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/_controls/build.py
+-rwxr-xr-x   0        0        0      963 2024-05-27 02:55:32.706999 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/_controls/off.py
+-rwxr-xr-x   0        0        0     1938 2024-05-27 02:50:43.106240 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/_controls/on.py
+-rwxr-xr-x   0        0        0     1663 2024-05-26 02:25:44.207938 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/_controls/saves/_clique.py
+-rwxr-xr-x   0        0        0     1586 2024-05-26 02:25:44.219937 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/_controls/saves/dumps/dump.py
+-rwxr-xr-x   0        0        0     1514 2024-05-26 02:25:44.235937 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/_controls/saves/dumps/restore.py
+-rwxr-xr-x   0        0        0     1469 2024-05-26 02:25:44.251937 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/_controls/saves/exports/monetary_export.py
+-rwxr-xr-x   0        0        0     1427 2024-05-26 02:25:44.263937 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/_controls/saves/exports/monetary_import.py
+-rwxr-xr-x   0        0        0      390 2024-04-23 20:10:51.728325 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/_controls/saves/memories.S.HTML
+-rwxr-xr-x   0        0        0      999 2024-05-27 02:52:44.972879 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/_controls/status.py
+-rwxr-xr-x   0        0        0      459 2024-05-13 00:59:57.240563 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/monetary.S.HTML
+-rwxr-xr-x   0        0        0      460 2024-05-27 02:46:28.805060 theme_park-2.0.0/venues/stages/theme_park/adventures/monetary/venture.py
+-rwxr-xr-x   0        0        0      730 2024-05-12 20:01:09.578794 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/[objectives]/objectives.S.HTML
+-rwxr-xr-x   0        0        0      900 2024-05-23 03:54:36.162629 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/_controls/is_on.py
+-rwxr-xr-x   0        0        0     1061 2024-05-23 03:55:13.562189 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/_controls/off.py
+-rwxr-xr-x   0        0        0     2551 2024-05-27 03:09:29.230645 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/_controls/on.py
+-rwxr-xr-x   0        0        0     2080 2024-05-22 19:04:00.745851 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/_controls/on_v1.py
+-rwxr-xr-x   0        0        0      549 2024-05-27 03:06:02.576809 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/_controls/refresh.py
+-rwxr-xr-x   0        0        0     1076 2024-05-27 03:06:02.596809 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/_status/API_status_besties__food_USDA__nature_v2__FDC_ID_1.py
+-rwxr-xr-x   0        0        0     2645 2024-05-27 03:08:29.847272 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/harbor/__init__.py
+-rw-r--r--   0        0        0     2942 2024-05-27 03:06:02.624808 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/harbor/guest_regions_vue/__init__.py
+-rw-r--r--   0        0        0      563 2024-05-26 04:29:46.733100 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/harbor/guest_regions_vue/caching.S.HTML
+-rwxr-xr-x   0        0        0      428 2024-05-27 03:06:02.644808 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/harbor/guest_sockets/__init__.py
+-rwxr-xr-x   0        0        0      259 2024-05-22 20:10:50.989908 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/middles/middles.S.HTML
+-rwxr-xr-x   0        0        0      530 2024-05-13 00:59:01.405145 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0      545 2024-05-27 03:06:02.660808 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/utilities/check_key/__init__.py
+-rwxr-xr-x   0        0        0     1538 2024-05-09 23:04:59.513271 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/utilities/generate_inventory_paths.py
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      302 2024-05-27 03:06:02.676808 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/utilities/retrieve_sanique_URL.py
+-rwxr-xr-x   0        0        0      834 2024-05-27 03:06:02.676808 theme_park-2.0.0/venues/stages/theme_park/adventures/sanique/venture.py
+-rw-r--r--   0        0        0      694 2024-05-27 03:12:53.632466 theme_park-2.0.0/venues/stages/theme_park/adventures/ventures.py
+-rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/.eslintrc.js--
+-rwxr-xr-x   0        0        0       94 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/.gitignore
+-rwxr-xr-x   0        0        0       26 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/.npmrc
+-rwxr-xr-x   0        0        0      939 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/README.md
+-rwxr-xr-x   0        0        0     1324 2024-05-22 20:32:05.875257 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/[proposals]/objectives -- possibilities.S.HTML
+-rwxr-xr-x   0        0        0       48 2024-05-22 20:31:54.975363 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/[proposals]/objectives.S.HTML
+-rwxr-xr-x   0        0        0        0 2024-05-14 21:36:02.546959 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/_controls/build.py
+-rwxr-xr-x   0        0        0        2 2024-05-08 21:03:01.449009 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/_controls/off.py
+-rwxr-xr-x   0        0        0        0 2024-05-08 21:06:04.803018 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/_controls/on.py
+-rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/school/.eslintrc.cjs
+-rwxr-xr-x   0        0        0      353 2024-05-09 21:32:18.768121 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/school/index.html
+-rwxr-xr-x   0        0        0      370 2024-05-10 02:14:54.482607 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/school/package.json
+-rwxr-xr-x   0        0        0     1435 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/school/public/typescript.svg
+-rwxr-xr-x   0        0        0     1497 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/school/public/vite.svg
+-rwxr-xr-x   0        0        0       23 2024-05-09 21:32:59.207717 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/school/src/main.js
+-rwxr-xr-x   0        0        0       75 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/school/tsconfig.json--
+-rwxr-xr-x   0        0        0      365 2024-05-10 02:14:10.075052 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/school/vite.config.js
+-rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/staff/.eslintrc.cjs
+-rwxr-xr-x   0        0        0      363 2024-05-09 21:34:48.778605 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/staff/index.html
+-rwxr-xr-x   0        0        0      397 2024-05-10 02:10:36.785101 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/staff/package.json
+-rwxr-xr-x   0        0        0     1435 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/staff/public/typescript.svg
+-rwxr-xr-x   0        0        0     1497 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/staff/public/vite.svg
+-rwxr-xr-x   0        0        0        1 2024-05-09 21:33:50.275202 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/staff/src/main.js
+-rwxr-xr-x   0        0        0      367 2024-05-10 02:08:38.618156 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/staff/vite.config.js
+-rwxr-xr-x   0        0        0      127 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/.eslintrc.cjs--
+-rwxr-xr-x   0        0        0      556 2024-05-08 22:05:09.904886 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/.eslintrc.json
+-rwxr-xr-x   0        0        0      745 2024-05-26 04:20:09.120517 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/index.html
+-rwxr-xr-x   0        0        0      632 2024-05-26 04:18:14.661726 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/package.json
+-rwxr-xr-x   0        0        0      311 2024-05-26 04:56:53.858282 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/src/apps/Earth/app.js
+-rwxr-xr-x   0        0        0     1888 2024-05-23 23:37:23.015065 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/guests/index.js
+-rwxr-xr-x   0        0        0      553 2024-05-26 04:56:46.058384 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/index.js
+-rwxr-xr-x   0        0        0       27 2023-12-08 17:29:39.919713 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/src/apps/Earth/logistics/logistics.s.HTML
+-rwxr-xr-x   0        0        0      116 2024-05-26 04:36:43.456163 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/field.js
+-rwxr-xr-x   0        0        0      734 2024-05-27 03:19:09.292399 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/src/apps/Earth/scenery/planet/field.vue
+-rwxr-xr-x   0        0        0     1202 2024-03-21 19:29:12.760368 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/src/apps/Earth/warehouses/layout/index.js
+-rwxr-xr-x   0        0        0      373 2023-11-14 00:07:17.821680 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/src/assets/main.css
+-rwxr-xr-x   0        0        0       59 2024-02-11 19:01:30.792959 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/src/main.js
+-rw-r--r--   0        0        0      251 2024-05-27 03:19:10.000391 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/the_build/assets/0.1.0_index.css
+-rw-r--r--   0        0        0   905823 2024-05-27 03:19:10.004391 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/the_build/assets/0.1.0_index.js
+-rw-r--r--   0        0        0      827 2024-05-27 03:19:10.000391 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/the_build/index.html
+-rwxr-xr-x   0        0        0       75 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/tsconfig.json--
+-rwxr-xr-x   0        0        0      728 2024-05-15 03:49:51.737456 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/vite.config.js
+-rwxr-xr-x   0        0        0      556 2024-05-08 21:11:26.687514 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/apps/web/vitest.config.js
+-rwxr-xr-x   0        0        0   358624 2024-05-13 01:01:34.311552 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/bun.lockb
+-rwxr-xr-x   0        0        0      521 2024-05-13 00:59:57.104565 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/find_symlinks.py
+-rwxr-xr-x   0        0        0      420 2024-05-10 02:12:07.564248 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/package.json
+-rwxr-xr-x   0        0        0      236 2024-05-08 19:30:19.000000 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/turbo.json
+-rwxr-xr-x   0        0        0      809 2024-05-26 04:57:44.941621 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/venture_build.py
+-rwxr-xr-x   0        0        0      608 2024-05-22 19:26:09.810018 theme_park-2.0.0/venues/stages/theme_park/adventures/vv_turbo/venture_dev.py
+-rwxr-xr-x   0        0        0      129 2024-01-26 16:01:45.729782 theme_park-2.0.0/venues/stages/theme_park/charts/charts.s.HTML
+-rwxr-xr-x   0        0        0      821 2024-03-17 23:24:26.718972 theme_park-2.0.0/venues/stages/theme_park/charts/plotly/plotly.s.HTML
+-rwxr-xr-x   0        0        0      671 2024-05-26 02:32:26.611328 theme_park-2.0.0/venues/stages/theme_park/climate/__init__.py
+-rwxr-xr-x   0        0        0       79 2024-05-12 03:05:51.809724 theme_park-2.0.0/venues/stages/theme_park/climate/climate.S.HTML
+-rwxr-xr-x   0        0        0      170 2024-04-04 19:34:53.736179 theme_park-2.0.0/venues/stages/theme_park/clouds/AV/AV.s.HTML
+-rwxr-xr-x   0        0        0      276 2024-03-17 21:13:24.014422 theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/Alpaca.s.HTML
+-rwxr-xr-x   0        0        0      160 2024-04-09 00:53:14.647459 theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/_data_API/data.S.HTML
+-rwxr-xr-x   0        0        0      795 2024-05-18 02:40:44.054159 theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/_data_API/v2/stock/symbol/bars.py
+-rwxr-xr-x   0        0        0      761 2024-05-18 02:40:44.058159 theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/_status/API_status_1.py
+-rwxr-xr-x   0        0        0      445 2024-05-18 02:40:44.058159 theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/crypto.S.HTML
+-rwxr-xr-x   0        0        0      977 2024-05-18 02:40:44.058159 theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/retrieve.py
+-rwxr-xr-x   0        0        0     1758 2024-05-18 02:40:44.058159 theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/structure_1.py
+-rwxr-xr-x   0        0        0       83 2024-04-04 20:04:06.732691 theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/options/options.S.HTML
+-rwxr-xr-x   0        0        0      390 2024-03-22 18:49:35.640871 theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/shares/retrieve_one.py
+-rwxr-xr-x   0        0        0      979 2024-05-18 02:40:44.054159 theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/shares/retrieve_spans.py
+-rwxr-xr-x   0        0        0      107 2024-03-17 18:08:13.242881 theme_park-2.0.0/venues/stages/theme_park/clouds/Bybit/Bybit.S.HTML
+-rwxr-xr-x   0        0        0      171 2024-05-18 02:40:44.050159 theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/CCXT.s.HTML
+-rwxr-xr-x   0        0        0     1036 2024-05-18 02:40:44.046159 theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/__init__.py
+-rwxr-xr-x   0        0        0     1591 2024-05-18 02:40:44.046159 theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles/__init__.py
+-rwxr-xr-x   0        0        0      565 2024-01-03 02:25:01.331601 theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles/candles.s.HTML
+-rwxr-xr-x   0        0        0     2510 2024-05-18 02:40:44.046159 theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles_v1/__init__.py
+-rwxr-xr-x   0        0        0      565 2024-01-03 02:25:01.331601 theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles_v1/candles.s.HTML
+-rwxr-xr-x   0        0        0        3 2023-12-28 22:53:18.327445 theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/__init__.py
+-rwxr-xr-x   0        0        0       62 2023-12-28 22:54:25.050671 theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/coinbase/coinbase.s.HTML
+-rwxr-xr-x   0        0        0      359 2024-05-18 02:40:44.050159 theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/symbols/array.py
+-rwxr-xr-x   0        0        0      331 2024-04-05 17:46:08.984778 theme_park-2.0.0/venues/stages/theme_park/clouds/Clouds Crypto.S.HTML
+-rwxr-xr-x   0        0        0     1024 2024-05-18 02:40:44.062159 theme_park-2.0.0/venues/stages/theme_park/clouds/Clouds Shares.S.HTML
+-rwxr-xr-x   0        0        0      597 2024-03-31 19:49:32.345940 theme_park-2.0.0/venues/stages/theme_park/clouds/Clouds.S.HTML
+-rwxr-xr-x   0        0        0     2723 2024-05-18 02:40:44.050159 theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/API/__init__.py
+-rwxr-xr-x   0        0        0      711 2024-05-18 02:40:44.050159 theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/API/accounts/__init__.py
+-rwxr-xr-x   0        0        0     2039 2024-05-18 02:40:44.054159 theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/API/build_JWT.py
+-rwxr-xr-x   0        0        0     1251 2024-05-18 02:40:44.054159 theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/API/orders/order_IDs.py
+-rwxr-xr-x   0        0        0     3269 2024-05-18 02:40:44.050159 theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/API/products/candles.py
+-rwxr-xr-x   0        0        0      972 2024-05-18 02:40:44.050159 theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/API/products/catalogue.py
+-rwxr-xr-x   0        0        0      696 2024-05-18 02:40:44.054159 theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/Coinbase.s.HTML
+-rwxr-xr-x   0        0        0     1540 2024-05-18 02:40:44.054159 theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/orders/place.py
+-rwxr-xr-x   0        0        0      614 2023-11-25 04:03:55.921174 theme_park-2.0.0/venues/stages/theme_park/clouds/DOGE/doge.s.HTML
+-rwxr-xr-x   0        0        0        0 2024-03-17 22:41:32.234375 theme_park-2.0.0/venues/stages/theme_park/clouds/Finnhub/Finnhub.S.HTML
+-rwxr-xr-x   0        0        0       47 2024-03-24 04:04:49.775241 theme_park-2.0.0/venues/stages/theme_park/clouds/Finviz.com/Finviz.com.S.HTML
+-rwxr-xr-x   0        0        0      193 2023-11-25 19:05:12.524729 theme_park-2.0.0/venues/stages/theme_park/clouds/LedgerX/LedgerX.s.HTML
+-rwxr-xr-x   0        0        0       10 2023-12-12 05:12:16.566568 theme_park-2.0.0/venues/stages/theme_park/clouds/MQL5/MQL5.s.HTML
+-rwxr-xr-x   0        0        0      226 2023-11-20 05:36:28.995516 theme_park-2.0.0/venues/stages/theme_park/clouds/Robinhood/Robinhood.s.HTML
+-rwxr-xr-x   0        0        0       80 2024-03-17 22:16:54.374127 theme_park-2.0.0/venues/stages/theme_park/clouds/Tiingo/Tiingo.S.HTML
+-rwxr-xr-x   0        0        0      126 2024-05-18 02:40:44.046159 theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/Tradier.s.HTML
+-rwxr-xr-x   0        0        0      525 2024-05-18 02:40:44.046159 theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/_status/API_status_combine_1.py
+-rwxr-xr-x   0        0        0       36 2024-04-04 19:14:12.097804 theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/procedures/exchanges/__init__.py
+-rwxr-xr-x   0        0        0      122 2024-04-04 19:13:46.242103 theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/procedures/exchanges/exchanges.S.HTML
+-rwxr-xr-x   0        0        0     1339 2024-05-18 02:40:44.038159 theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/procedures/options/combine.py
+-rwxr-xr-x   0        0        0   220164 2023-11-21 17:07:07.643477 theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/procedures/options/example_responses/NOVA_options_chain.JSON
+-rwxr-xr-x   0        0        0      212 2023-10-19 20:16:35.898645 theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/uo_tradier_api.s.HTML
+-rwxr-xr-x   0        0        0     1128 2024-05-18 02:40:44.038159 theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/lookup/__init__.py
+-rwxr-xr-x   0        0        0     1228 2024-05-18 02:40:44.042159 theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/options/chains/__init__.py
+-rwxr-xr-x   0        0        0     1769 2024-04-04 20:05:04.392129 theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/options/chains/parse_1.py
+-rwxr-xr-x   0        0        0      631 2024-05-18 02:40:44.042159 theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/options/expirations/__init__.py
+-rwxr-xr-x   0        0        0      216 2024-03-18 04:26:59.460093 theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/TV.s.HTML
+-rwxr-xr-x   0        0        0       77 2024-05-18 02:40:44.062159 theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/fluctuators/fluctuators.S.HTML
+-rwxr-xr-x   0        0        0      300 2023-12-12 05:03:24.406023 theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/sensors/__init__.py
+-rwxr-xr-x   0        0        0      237 2024-03-22 19:42:45.277679 theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/sensors/sensors.S.HTML
+-rwxr-xr-x   0        0        0     3458 2024-03-17 05:35:01.529000 theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/treasure/indicators/RMI_Trend_Sniper.pine
+-rwxr-xr-x   0        0        0      163 2024-03-17 05:34:46.185162 theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/treasure/indicators/indicators.S.HTML
+-rwxr-xr-x   0        0        0     3830 2024-05-18 02:40:44.062159 theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals/__init__.py
+-rwxr-xr-x   0        0        0     1508 2024-05-18 02:40:44.058159 theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals_v2/__init__.py
+-rwxr-xr-x   0        0        0      813 2024-03-22 19:47:25.962582 theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py
+-rwxr-xr-x   0        0        0     1829 2024-03-22 19:46:48.770994 theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py
+-rwxr-xr-x   0        0        0      495 2024-03-28 00:15:40.797119 theme_park-2.0.0/venues/stages/theme_park/clouds/USA/IRS/IRA/IRA.S.HTML
+-rwxr-xr-x   0        0        0      407 2024-05-18 02:40:44.046159 theme_park-2.0.0/venues/stages/theme_park/clouds/USA/IRS/taxes/income/__init__.py
+-rwxr-xr-x   0        0        0       60 2023-11-10 17:23:06.947404 theme_park-2.0.0/venues/stages/theme_park/clouds/USA/SEC/6K/__init__.py
+-rwxr-xr-x   0        0        0      496 2023-11-10 17:40:32.497079 theme_park-2.0.0/venues/stages/theme_park/clouds/USA/SEC/balance_sheets/__init__.py
+-rwxr-xr-x   0        0        0       18 2023-11-10 17:15:04.345938 theme_park-2.0.0/venues/stages/theme_park/clouds/USA/SEC/balance_sheets/balance_sheets.s.HTML
+-rwxr-xr-x   0        0        0      198 2023-11-10 17:28:03.521299 theme_park-2.0.0/venues/stages/theme_park/clouds/USA/SEC/balance_sheets/equity/__init__.py
+-rwxr-xr-x   0        0        0      420 2023-11-10 17:53:32.039501 theme_park-2.0.0/venues/stages/theme_park/clouds/USA/SEC/income/__init__.py
+-rwxr-xr-x   0        0        0       51 2023-11-10 17:34:28.536151 theme_park-2.0.0/venues/stages/theme_park/clouds/USA/SEC/income/income.s.HTML
+-rwxr-xr-x   0        0        0        0 2023-11-09 20:40:55.437403 theme_park-2.0.0/venues/stages/theme_park/clouds/USA/SEC/statements.s.HTML
+-rwxr-xr-x   0        0        0      212 2023-11-14 04:12:06.841989 theme_park-2.0.0/venues/stages/theme_park/clouds/Yahoo/Yahoo.s.HTML
+-rwxr-xr-x   0        0        0     1821 2024-05-18 02:40:44.046159 theme_park-2.0.0/venues/stages/theme_park/clouds/Yahoo/retrieve.py
+-rwxr-xr-x   0        0        0      931 2024-05-18 02:40:44.046159 theme_park-2.0.0/venues/stages/theme_park/clouds/Yahoo/retrieve_change.py
+-rwxr-xr-x   0        0        0       32 2023-11-14 05:19:00.214473 theme_park-2.0.0/venues/stages/theme_park/clouds/twelve_data/twelve_data.s.HTML
+-rwxr-xr-x   0        0        0       16 2024-03-24 03:14:51.054648 theme_park-2.0.0/venues/stages/theme_park/emojis.MD
+-rwxr-xr-x   0        0        0     2589 2023-11-14 05:42:13.790956 theme_park-2.0.0/venues/stages/theme_park/fluctuators/bt/strategies/example_1.py
+-rwxr-xr-x   0        0        0      130 2024-04-08 20:48:05.178188 theme_park-2.0.0/venues/stages/theme_park/fluctuators/fluctuators - itinerary.s.HTML
+-rwxr-xr-x   0        0        0      787 2024-04-08 20:48:43.589745 theme_park-2.0.0/venues/stages/theme_park/fluctuators/fluctuators.S.HTML
+-rwxr-xr-x   0        0        0      121 2023-11-28 03:26:29.420655 theme_park-2.0.0/venues/stages/theme_park/fluctuators/lumi/lumi.s.HTML
+-rwxr-xr-x   0        0        0      100 2023-12-19 04:49:40.656260 theme_park-2.0.0/venues/stages/theme_park/fluctuators/rover_1/rover_1.s.HTML
+-rwxr-xr-x   0        0        0      443 2024-05-18 02:40:43.998160 theme_park-2.0.0/venues/stages/theme_park/gadgets/clock/UTC/ISO.py
+-rwxr-xr-x   0        0        0      349 2024-05-18 02:40:43.998160 theme_park-2.0.0/venues/stages/theme_park/gadgets/clock/UTC/current.py
+-rwxr-xr-x   0        0        0      981 2024-05-18 02:40:43.998160 theme_park-2.0.0/venues/stages/theme_park/gadgets/clock/UTC/greatness_1.py
+-rwxr-xr-x   0        0        0      288 2024-04-09 02:03:24.336835 theme_park-2.0.0/venues/stages/theme_park/gadgets/clock/clock.s.HTML
+-rwxr-xr-x   0        0        0      620 2023-11-09 20:46:40.432504 theme_park-2.0.0/venues/stages/theme_park/gadgets/format_percentage.py
+-rwxr-xr-x   0        0        0      151 2023-11-23 05:19:27.179399 theme_park-2.0.0/venues/stages/theme_park/gadgets/math/slope/__init__.py
+-rwxr-xr-x   0        0        0       79 2024-01-10 05:54:37.773115 theme_park-2.0.0/venues/stages/theme_park/gadgets/pandas/DF/DF.s.HTML
+-rwxr-xr-x   0        0        0      513 2024-05-18 02:40:43.994160 theme_park-2.0.0/venues/stages/theme_park/gadgets/pandas/DF/_status/status_from_1.py
+-rwxr-xr-x   0        0        0      249 2024-05-18 02:40:43.994160 theme_park-2.0.0/venues/stages/theme_park/gadgets/pandas/DF/from_list.py
+-rwxr-xr-x   0        0        0      323 2024-05-18 02:40:43.994160 theme_park-2.0.0/venues/stages/theme_park/gadgets/pandas/DF/to_list.py
+-rwxr-xr-x   0        0        0      690 2024-01-13 06:12:46.871796 theme_park-2.0.0/venues/stages/theme_park/gadgets/pandas/pandas.s.HTML
+-rwxr-xr-x   0        0        0      399 2024-05-18 02:40:43.994160 theme_park-2.0.0/venues/stages/theme_park/gadgets/ratio.py
+-rwxr-xr-x   0        0        0      454 2024-05-18 02:40:43.990160 theme_park-2.0.0/venues/stages/theme_park/gadgets/summation/__init__.py
+-rwxr-xr-x   0        0        0      374 2024-05-18 02:40:43.990160 theme_park-2.0.0/venues/stages/theme_park/gadgets/summation/status_1.py
+-rwxr-xr-x   0        0        0    18282 2023-12-28 23:17:20.176165 theme_park-2.0.0/venues/stages/theme_park/gadgets/summation/summation.svg
+-rwxr-xr-x   0        0        0      100 2024-04-09 02:03:10.212995 theme_park-2.0.0/venues/stages/theme_park/gadgets/tools.s.HTML
+-rwxr-xr-x   0        0        0     1075 2024-05-18 02:40:44.062159 theme_park-2.0.0/venues/stages/theme_park/home.s.HTML
+-rwxr-xr-x   0        0        0      305 2024-04-26 00:08:58.840689 theme_park-2.0.0/venues/stages/theme_park/platforms/accounts/accounts.S.HTML
+-rwxr-xr-x   0        0        0      142 2024-04-26 01:32:14.574003 theme_park-2.0.0/venues/stages/theme_park/platforms/biorecon/biorecon.S.HTML
+-rwxr-xr-x   0        0        0      503 2024-04-26 00:27:03.696837 theme_park-2.0.0/venues/stages/theme_park/platforms/platforms.S.HTML
+-rwxr-xr-x   0        0        0     2086 2024-05-27 03:20:01.071834 theme_park-2.0.0/venues/stages/theme_park/readme.md
+-rwxr-xr-x   0        0        0      425 2024-04-09 02:33:16.647876 theme_park-2.0.0/venues/stages/theme_park/rides/rides - formats.S.HTML
+-rwxr-xr-x   0        0        0      115 2024-04-27 16:24:01.727436 theme_park-2.0.0/venues/stages/theme_park/rides/rides - objectives possibilities.S.HTML
+-rwxr-xr-x   0        0        0      321 2024-04-27 16:19:46.237010 theme_park-2.0.0/venues/stages/theme_park/rides/rides - objectives.S.HTML
+-rwxr-xr-x   0        0        0     1416 2024-05-18 02:40:44.014159 theme_park-2.0.0/venues/stages/theme_park/rides/rides.S.HTML
+-rwxr-xr-x   0        0        0      489 2023-12-31 05:03:05.192136 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/ATR/ATR.s.HTML
+-rwxr-xr-x   0        0        0     2941 2024-05-18 02:40:44.018159 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py
+-rwxr-xr-x   0        0        0     1585 2024-05-18 02:40:44.018159 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/ATR/__init__.py
+-rwxr-xr-x   0        0        0     1239 2024-05-18 02:40:44.018159 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/ATR/_status/status_1.py
+-rwxr-xr-x   0        0        0     1731 2024-01-02 03:23:31.042432 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/Andean_Oscillator/AO.pine
+-rwxr-xr-x   0        0        0      134 2023-12-01 02:49:14.211328 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/Andean_Oscillator/Andean.r.HTML
+-rwxr-xr-x   0        0        0      273 2023-12-31 06:36:06.223233 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/EMA/EMA.s.HTML
+-rwxr-xr-x   0        0        0       82 2023-11-14 05:05:08.114737 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/EMA/__init__.py
+-rwxr-xr-x   0        0        0     4821 2024-01-02 03:23:31.085431 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/HHLL/indicator.pine
+-rwxr-xr-x   0        0        0       72 2023-12-03 22:10:44.686991 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/MA/MA.r.HTML
+-rwxr-xr-x   0        0        0       91 2023-12-12 04:16:31.428608 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/MACD/MACD.s.HTML
+-rwxr-xr-x   0        0        0       48 2023-12-02 00:37:47.807470 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/QQE/QQE.r.HTML
+-rwxr-xr-x   0        0        0      201 2023-12-03 02:58:48.769709 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/RSI/RSI.r.HTML
+-rwxr-xr-x   0        0        0      779 2024-05-18 02:40:44.014159 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/RSI/__init__.py
+-rwxr-xr-x   0        0        0      250 2024-01-02 06:36:59.547427 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/SMA/__init__.py
+-rwxr-xr-x   0        0        0      397 2024-01-02 03:23:31.177430 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/TR/TR.s.HTML
+-rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/TR/True Range.svg
+-rwxr-xr-x   0        0        0     1625 2024-05-18 02:40:44.014159 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/TR/__init__.py
+-rwxr-xr-x   0        0        0      520 2024-05-18 02:40:44.014159 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/TR/_status/status_1.py
+-rwxr-xr-x   0        0        0      789 2024-05-18 02:40:44.018159 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/TR/_status/status_2.py
+-rwxr-xr-x   0        0        0      254 2023-11-29 18:25:15.058846 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/TV.r.HTML
+-rwxr-xr-x   0        0        0       46 2023-11-21 16:46:45.097491 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/VWAP/VWAP.r.HTML
+-rwxr-xr-x   0        0        0      590 2024-05-18 02:40:44.014159 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/VWAP/__init__.py
+-rwxr-xr-x   0        0        0       47 2023-11-21 16:46:17.697805 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/VWMA/VWMA.r.HTML
+-rwxr-xr-x   0        0        0       24 2023-11-14 04:28:20.239207 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/bolinger_bands/bolinger_bands.r.html
+-rwxr-xr-x   0        0        0        0 2023-11-30 18:13:51.268620 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/chandlier_exit/chandelier exit.r.HTML
+-rwxr-xr-x   0        0        0      543 2024-05-18 02:40:44.014159 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/indicators.s.HTML
+-rwxr-xr-x   0        0        0     1266 2024-01-02 03:23:31.097431 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/pivot_point/pivot_point.s.HTML
+-rwxr-xr-x   0        0        0       28 2023-11-21 16:43:07.835981 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/relative_volume/relative volume.r.HTML
+-rwxr-xr-x   0        0        0     2829 2024-05-18 02:40:44.018159 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py
+-rwxr-xr-x   0        0        0     1092 2024-05-18 02:40:44.018159 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/supertrend/__init__.py
+-rwxr-xr-x   0        0        0     1240 2024-05-18 02:40:44.018159 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/supertrend/_status/status_1.py
+-rwxr-xr-x   0        0        0      358 2024-01-06 00:03:10.850549 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/supertrend/pandas_ta/__init__.py
+-rwxr-xr-x   0        0        0      225 2023-12-03 02:59:17.552392 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/supertrend/supertrend.s.HTML
+-rwxr-xr-x   0        0        0        0 2024-01-02 03:30:08.272935 theme_park-2.0.0/venues/stages/theme_park/rides/season_1/supertrend2/__init__.py
+-rwxr-xr-x   0        0        0     1209 2024-05-18 02:40:44.002159 theme_park-2.0.0/venues/stages/theme_park/rides/season_2/AAS/__init__.py
+-rwxr-xr-x   0        0        0     1227 2024-05-18 02:40:44.002159 theme_park-2.0.0/venues/stages/theme_park/rides/season_2/AAS/_status/status_1.py
+-rwxr-xr-x   0        0        0      334 2024-01-06 07:25:23.819962 theme_park-2.0.0/venues/stages/theme_park/rides/season_2/AS/AS.s.HTML
+-rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 theme_park-2.0.0/venues/stages/theme_park/rides/season_2/AS/AS.svg
+-rwxr-xr-x   0        0        0     1541 2024-05-18 02:40:43.998160 theme_park-2.0.0/venues/stages/theme_park/rides/season_2/AS/__init__.py
+-rwxr-xr-x   0        0        0      508 2024-05-18 02:40:43.998160 theme_park-2.0.0/venues/stages/theme_park/rides/season_2/AS/_status/status_1.py
+-rwxr-xr-x   0        0        0      780 2024-05-18 02:40:43.998160 theme_park-2.0.0/venues/stages/theme_park/rides/season_2/AS/_status/status_2.py
+-rwxr-xr-x   0        0        0     1093 2024-01-06 07:15:37.995569 theme_park-2.0.0/venues/stages/theme_park/rides/season_2/pecdency/__init__.py
+-rwxr-xr-x   0        0        0     1344 2024-05-18 02:40:43.998160 theme_park-2.0.0/venues/stages/theme_park/rides/season_2/pecdency/__init__v1.py
+-rwxr-xr-x   0        0        0     4110 2024-05-18 02:40:44.002159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/ST/__init__.py
+-rwxr-xr-x   0        0        0      430 2024-05-18 02:40:44.010159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/VDA/__init__.py
+-rwxr-xr-x   0        0        0      564 2024-05-18 02:40:44.006159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/VSA/__init__.py
+-rwxr-xr-x   0        0        0      334 2024-01-09 01:54:38.423714 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span/AS.s.HTML
+-rwxr-xr-x   0        0        0    47171 2023-12-28 18:38:03.620071 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span/AS.svg
+-rwxr-xr-x   0        0        0     1554 2024-05-18 02:40:44.006159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span/__init__.py
+-rwxr-xr-x   0        0        0      519 2024-05-18 02:40:44.006159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span/_status/status_1.py
+-rwxr-xr-x   0        0        0      787 2024-05-18 02:40:44.010159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span/_status/status_2.py
+-rwxr-xr-x   0        0        0     1177 2024-05-18 02:40:44.002159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span_average/__init__.py
+-rwxr-xr-x   0        0        0     1245 2024-05-18 02:40:44.002159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span_average/_status/status_1.py
+-rwxr-xr-x   0        0        0     3679 2024-05-18 02:40:44.010159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span_reversals/__init__.py
+-rwxr-xr-x   0        0        0     3577 2024-05-18 02:40:44.006159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span_roads_v1/__init__.py
+-rwxr-xr-x   0        0        0     3859 2024-05-18 02:40:44.006159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/super_hero_trend/__init__.py
+-rwxr-xr-x   0        0        0     1756 2024-05-18 02:40:44.006159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/super_hero_trend/win_rates/shares_trading.py
+-rwxr-xr-x   0        0        0      958 2024-05-18 02:40:44.006159 theme_park-2.0.0/venues/stages/theme_park/rides/season_3/supertrend/__init__.py
+-rwxr-xr-x   0        0        0     1822 2024-05-18 02:40:44.014159 theme_park-2.0.0/venues/stages/theme_park/rides/season_4/AO/__init__.py
+-rwxr-xr-x   0        0        0     5968 2024-04-11 03:49:19.489710 theme_park-2.0.0/venues/stages/theme_park/rides/season_4/ML_Lorentzian/KernelFunctions.ps
+-rwxr-xr-x   0        0        0    36151 2024-04-11 03:49:38.505474 theme_park-2.0.0/venues/stages/theme_park/rides/season_4/ML_Lorentzian/Lorentzian Classification.ps
+-rwxr-xr-x   0        0        0    18799 2024-04-11 03:48:20.246452 theme_park-2.0.0/venues/stages/theme_park/rides/season_4/ML_Lorentzian/MLExtensions.ps
+-rwxr-xr-x   0        0        0     3923 2024-05-18 02:40:44.010159 theme_park-2.0.0/venues/stages/theme_park/rides/season_4/superb/__init__.py
+-rwxr-xr-x   0        0        0       13 2024-02-01 15:34:15.615610 theme_park-2.0.0/venues/stages/theme_park/rides/season_4/superb/superb.s.HTML
+-rwxr-xr-x   0        0        0     1783 2024-05-18 02:40:44.010159 theme_park-2.0.0/venues/stages/theme_park/rides/season_4/superb/win_rates/shares_trading.py
+-rwxr-xr-x   0        0        0     3997 2024-05-18 02:40:43.982160 theme_park-2.0.0/venues/stages/theme_park/scans/_clique/ETF.py
+-rwxr-xr-x   0        0        0        2 2024-04-04 18:06:03.015402 theme_park-2.0.0/venues/stages/theme_park/scans/_clique/REIT.py
+-rwxr-xr-x   0        0        0     2159 2024-05-18 02:40:43.986160 theme_park-2.0.0/venues/stages/theme_park/scans/_clique/TV.py
+-rwxr-xr-x   0        0        0     1408 2024-05-18 02:40:43.982160 theme_park-2.0.0/venues/stages/theme_park/scans/_clique/currency.py
+-rwxr-xr-x   0        0        0       42 2024-04-04 18:06:43.814870 theme_park-2.0.0/venues/stages/theme_park/scans/_clique/penny_stocks.py
+-rwxr-xr-x   0        0        0      412 2024-05-18 02:40:43.986160 theme_park-2.0.0/venues/stages/theme_park/scans/clique.py
+-rwxr-xr-x   0        0        0      180 2024-04-15 19:29:36.357014 theme_park-2.0.0/venues/stages/theme_park/scans/screeners.S.HTML
+-rwxr-xr-x   0        0        0      116 2024-05-18 02:40:43.986160 theme_park-2.0.0/venues/stages/theme_park/scans/symbol/__init__.py
+-rwxr-xr-x   0        0        0      938 2024-05-18 02:40:43.986160 theme_park-2.0.0/venues/stages/theme_park/scans/symbol/symbols.S.HTML
+-rwxr-xr-x   0        0        0       84 2024-04-08 20:53:48.054233 theme_park-2.0.0/venues/stages/theme_park/stats/VHLOC/MACD/MACD.S.HTML
+-rwxr-xr-x   0        0        0      102 2024-05-18 02:40:44.022159 theme_park-2.0.0/venues/stages/theme_park/stats/VHLOC/MACD/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-04-08 20:53:19.026568 theme_park-2.0.0/venues/stages/theme_park/stats/VHLOC/MACD/procedure.ps
+-rwxr-xr-x   0        0        0     5111 2024-05-18 02:40:44.026159 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/__init__.py
+-rwxr-xr-x   0        0        0     1952 2024-05-18 02:40:44.030159 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/squeeze pc ratios.r.HTML
+-rwxr-xr-x   0        0        0   388314 2023-11-09 20:42:52.592079 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/examples/1.JSON
+-rwxr-xr-x   0        0        0     1567 2023-11-09 20:42:52.591079 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/examples/2.JSON
+-rwxr-xr-x   0        0        0      590 2024-05-18 02:40:44.026159 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/status_1.py
+-rwxr-xr-x   0        0        0     1857 2024-05-18 02:40:44.030159 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/status_2.py
+-rwxr-xr-x   0        0        0     2902 2024-05-18 02:40:44.022159 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/__init__.py
+-rwxr-xr-x   0        0        0     2290 2023-12-04 02:47:32.197228 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/examples/0.JSON
+-rwxr-xr-x   0        0        0   388314 2023-11-09 20:42:52.592079 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/examples/1.JSON
+-rwxr-xr-x   0        0        0     1567 2023-11-09 20:42:52.591079 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/examples/2.JSON
+-rwxr-xr-x   0        0        0     1502 2024-05-18 02:40:44.022159 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/status_1.py
+-rwxr-xr-x   0        0        0      788 2024-05-18 02:40:44.026159 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/status_2.py
+-rwxr-xr-x   0        0        0      997 2024-05-18 02:40:44.022159 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/aggregate break even.s.HTML
+-rwxr-xr-x   0        0        0        0 2024-03-31 19:07:37.005708 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/clique.py
+-rwxr-xr-x   0        0        0      889 2024-05-18 02:40:44.022159 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/show/__init__.py
+-rwxr-xr-x   0        0        0     1599 2024-03-31 18:39:18.393448 theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_multiplier/aggregate_multipliers.r.HTML
+-rwxr-xr-x   0        0        0     1409 2024-05-18 02:40:44.026159 theme_park-2.0.0/venues/stages/theme_park/stats/clique.py
+-rwxr-xr-x   0        0        0      311 2024-04-05 04:21:31.280203 theme_park-2.0.0/venues/stages/theme_park/stats/option_priceyness/option_priceyness.S.HTML
+-rwxr-xr-x   0        0        0      616 2024-05-04 03:34:27.890705 theme_park-2.0.0/venues/stages/theme_park/stats/stats.s.HTML
+-rwxr-xr-x   0        0        0      349 2024-05-18 02:40:44.022159 theme_park-2.0.0/venues/stages/theme_park/stats/the_multiplier/__init__.py
+-rwxr-xr-x   0        0        0      911 2024-03-17 21:11:40.987538 theme_park-2.0.0/venues/stages/theme_park/treasures/commodities/commodities.s.HTML
+-rwxr-xr-x   0        0        0       89 2024-04-08 22:27:54.205084 theme_park-2.0.0/venues/stages/theme_park/treasures/contracts/contracts.S.HTML
+-rwxr-xr-x   0        0        0      339 2024-04-13 19:27:27.156565 theme_park-2.0.0/venues/stages/theme_park/treasures/crypto/L1/L1.S.HTML
+-rwxr-xr-x   0        0        0      725 2024-04-13 19:19:01.872575 theme_park-2.0.0/venues/stages/theme_park/treasures/crypto/crypto.S.HTML
+-rwxr-xr-x   0        0        0       61 2024-04-13 19:26:04.032669 theme_park-2.0.0/venues/stages/theme_park/treasures/crypto/crypto_rust.S.HTML
+-rwxr-xr-x   0        0        0      641 2024-04-13 19:19:32.260629 theme_park-2.0.0/venues/stages/theme_park/treasures/crypto/crypto_usual_features.S.HTML
+-rwxr-xr-x   0        0        0      127 2024-04-25 23:58:14.336246 theme_park-2.0.0/venues/stages/theme_park/treasures/forex/forex.s.HTML
+-rwxr-xr-x   0        0        0       75 2024-01-30 00:33:10.380046 theme_park-2.0.0/venues/stages/theme_park/treasures/futures/futures.s.HTML
+-rwxr-xr-x   0        0        0      186 2024-04-19 20:08:05.560255 theme_park-2.0.0/venues/stages/theme_park/treasures/gems/gems.S.HTML
+-rwxr-xr-x   0        0        0       48 2024-04-08 17:11:40.338334 theme_park-2.0.0/venues/stages/theme_park/treasures/options/greeks/greeks.S.HTML
+-rwxr-xr-x   0        0        0     1562 2024-05-18 02:40:43.982160 theme_park-2.0.0/venues/stages/theme_park/treasures/options/movement_calculator/__init__.py
+-rwxr-xr-x   0        0        0     1167 2023-11-23 05:20:06.387999 theme_park-2.0.0/venues/stages/theme_park/treasures/options/movement_calculator/slope.s.HTML
+-rwxr-xr-x   0        0        0     2569 2024-05-18 02:40:43.982160 theme_park-2.0.0/venues/stages/theme_park/treasures/options/multipliers/__init__.py
+-rwxr-xr-x   0        0        0      358 2024-04-08 17:12:06.086114 theme_park-2.0.0/venues/stages/theme_park/treasures/options/options.s.HTML
+-rwxr-xr-x   0        0        0     1495 2024-05-18 02:40:43.982160 theme_park-2.0.0/venues/stages/theme_park/treasures/options/shapes/shape_1/__init__.py
+-rwxr-xr-x   0        0        0      489 2023-11-21 17:09:02.275163 theme_park-2.0.0/venues/stages/theme_park/treasures/options/shapes/shape_1/shape_1.s.HTML
+-rwxr-xr-x   0        0        0      144 2024-05-18 02:40:43.978160 theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/__init__.py
+-rwxr-xr-x   0        0        0      156 2024-04-08 23:27:06.857428 theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/loans/loans.S.HTML
+-rwxr-xr-x   0        0        0      431 2024-04-08 21:38:29.659326 theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/constant.py
+-rwxr-xr-x   0        0        0       95 2024-04-08 21:54:20.848024 theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/insurance/insurance.S.HTML
+-rwxr-xr-x   0        0        0      587 2024-04-08 22:05:05.892491 theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/loan - varieties.S.HTML
+-rwxr-xr-x   0        0        0     1202 2024-04-08 22:40:59.788117 theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/loan.S.HTML
+-rwxr-xr-x   0        0        0     1463 2024-04-09 00:50:23.861466 theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/sources/sources.S.HTML
+-rwxr-xr-x   0        0        0      414 2024-04-08 22:42:58.322845 theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/real_estate.S.HTML
+-rwxr-xr-x   0        0        0      437 2024-04-08 21:43:11.491928 theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/sends.S.HTML
+-rwxr-xr-x   0        0        0      127 2024-04-08 21:37:42.099907 theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/tax/__init__.py
+-rwxr-xr-x   0        0        0       97 2024-04-08 21:48:11.608365 theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/tax/tax.S.HTML
+-rwxr-xr-x   0        0        0     2434 2024-04-08 22:08:51.961985 theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/varieties/varieties.S.HTML
+-rwxr-xr-x   0        0        0     1190 2024-03-31 19:49:32.365940 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/ETF/ETF.s.HTML
+-rwxr-xr-x   0        0        0      114 2023-11-15 06:29:25.238807 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/ETF/comprehensive/comprehensive.s.HTML
+-rwxr-xr-x   0        0        0       42 2023-11-15 06:37:06.461104 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/ETF/sectors/airlines/airlines.r.HTML
+-rwxr-xr-x   0        0        0       45 2023-11-15 06:38:49.083268 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/ETF/sectors/electronics/semiconductors.r.HTML
+-rwxr-xr-x   0        0        0       81 2023-11-15 06:34:55.671168 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/ETF/sectors/farming/farming.r.HTML
+-rwxr-xr-x   0        0        0       84 2023-11-15 06:37:33.924880 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/ETF/sectors/real estate/real estate.r.HTML
+-rwxr-xr-x   0        0        0      157 2024-03-17 04:50:30.861349 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/ETF/sectors/sectors.S.HTML
+-rwxr-xr-x   0        0        0       14 2023-11-15 06:36:56.273187 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/ETF/sectors/vehicles/vehicles.r.HTML
+-rwxr-xr-x   0        0        0        7 2024-03-24 04:01:12.905095 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/__init__.py
+-rwxr-xr-x   0        0        0       13 2023-11-15 06:11:36.293215 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/companies/companies.s.HTML
+-rwxr-xr-x   0        0        0       11 2023-11-21 16:53:15.238020 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/shapes/shape_1/__init__.py
+-rwxr-xr-x   0        0        0      135 2023-11-21 16:52:53.862265 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/shapes/shape_1/shape_1.s.HTML
+-rwxr-xr-x   0        0        0      106 2024-04-08 19:07:13.173774 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/shares.s.HTML
+-rwxr-xr-x   0        0        0       43 2023-11-17 19:16:25.824071 theme_park-2.0.0/venues/stages/theme_park/treasures/shares/splits.s.HTML
+-rwxr-xr-x   0        0        0      109 2024-05-27 02:47:16.288536 theme_park-2.0.0/venues/stages/theme_park/treasures/treasures.s.HTML
+-rw-r--r--   0        0        0     4493 1970-01-01 00:00:00.000000 theme_park-2.0.0/PKG-INFO
```

### Comparing `theme_park-1.0.0/readme.md` & `theme_park-2.0.0/readme.md`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venue.S.HTML` & `theme_park-2.0.0/venue.S.HTML`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 
 <pre>
 
 	<h1>theme_park</h1>
 		# theme_park
 		# rollecoaster
 		# vortex
-
 	
-
 	<h2>on</h2>
-		<h3>terminal 1</h3>
-			docker compose up -d;
-			docker exec -it pheromone.1 bash
+		<h3>session 1</h3>
+			docker compose up -d; docker exec -it theme_park.1 bash;
+			source /habitat/_controls/build_1.sh
+			cd /habitat/venues/_contructions/
+			theme_park_1
 		
-		<h3>terminal 2</h3>
-			docker exec -it pheromone.1 bash
-			source /habitat/_controls/source_2.sh
+		<h3>session 2</h3>
+			docker exec -it theme_park.1 bash
+			source /habitat/_controls/build_2.sh
+
+	
 
 	<h2>publishing</h2>
 		
 		#
 		#	statuses
 		#
 		python3 /habitat/venues/stages/theme_park/_status/status.proc.py
```

### Comparing `theme_park-1.0.0/venues/stages/theme_park/___objectives/itinerary.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/[_quests]/quests.S.HTML`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 
 
 
 <pre>
 
-	<h1>itinerary</h1>
+	<h1>quests</h1>
 
 	<h2>ranked</h2>
 			
+		[  ] TradingView Rider
+				"bionic_eye_contact_rider"
+			
+					[  ] mongo
+			
 		[ ] screen by shareholder's equity percentage
 			change by quarter.
 			
 				example:
 					2023 Q4 to 2024 Q1
 					
 						2023_Q4: $120m
```

### Comparing `theme_park-1.0.0/venues/stages/theme_park/___objectives/sequentials/sequentials.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/[_quests]/sequentials/sequentials.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/___objectives/sporatic/TradingView Screen.png` & `theme_park-2.0.0/venues/stages/theme_park/[_quests]/sporatic/TradingView Screen.png`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/__data_nodes/moon/listing_status.csv` & `theme_park-2.0.0/venues/stages/theme_park/__data_nodes/moon/listing_status.csv`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/_interfaces/clique/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/_clique/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 
 
 
 
-
+#/
+#
 from .group import clique as clique_group
-
+#
 from theme_park.stats.clique import stats_group
 from theme_park.scans.clique import scans_group
 from theme_park.__data_nodes.moon.clique import moon_group
+#
+from ..adventures.ventures import retrieve_ventures
+#
+#
+from ventures.clique import ventures_clique
+#
+#\
 
 def clique ():
 	import click
 	@click.group ()
 	def group ():
 		pass
 
 	import click
-	@click.command ("help")
+	@click.command ("school")
 	@click.option ('--port', default = "20000", required = False)
 	def open_sphene (port):	
 		import pathlib
 		from os.path import dirname, join, normpath
 		this_folder_path = pathlib.Path (__file__).parent.resolve ()
 		this_module_path = normpath (join (this_folder_path, "../.."))
 
@@ -70,14 +78,18 @@
 			]
 		)
 
 		rich.print_json (data = symbols_indicators)
 
 		TV_treasure_tech.print_symbols_table (symbols_indicators)
 
+	group.add_command (ventures_clique ({
+		"ventures": retrieve_ventures ()
+	}))
+
 	group.add_command (example_command)
 	group.add_command (open_sphene)
 
 	group.add_command (clique_group ())
 	group.add_command (stats_group ())	
 	group.add_command (scans_group ())
```

### Comparing `theme_park-1.0.0/venues/stages/theme_park/_status/DB/records.json` & `theme_park-2.0.0/venues/stages/theme_park/_status/DB/records.json`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/_status/clouds_status.proc.py` & `theme_park-2.0.0/venues/stages/theme_park/_status/clouds_status.proc.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/_status/status.proc.py` & `theme_park-2.0.0/venues/stages/theme_park/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/adventures/meter/meter.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/adventures/meter/meter.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/charts/plotly/plotly.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/charts/plotly/plotly.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/climate/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/climate/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Tradier = climate.find ("Tradier")
 '''
 
 import copy
 
 def retrieve_Tradier ():
 	import json
-	fp = open ("/online/crowns_theme_park/mint/tradier.com/online.JSON", "r")
+	fp = open ("/online/locker/vaccines_rollercoaster/treasures/tradier.com.1/online.JSON", "r")
 	Tradier_authorization = json.loads (fp.read ()) ["authorization"]
 	fp.close ()
 	
 	return Tradier_authorization
 	
 
 climate = {
```

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/_data_API/v2/stock/symbol/bars.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/_data_API/v2/stock/symbol/bars.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/_status/API_status_1.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/_status/API_status_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/retrieve.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/retrieve.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/structure_1.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/crypto/structure_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Alpaca/shares/retrieve_spans.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Alpaca/shares/retrieve_spans.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles/candles.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles/candles.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles_v1/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles_v1/candles.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/clouds/CCXT/OHLCV/candles_v1/candles.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Clouds Shares.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Clouds Shares.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Clouds.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Clouds.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/API/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/API/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/API/accounts/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/API/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/API/build_JWT.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/API/build_JWT.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/API/orders/order_IDs.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/API/orders/order_IDs.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/API/products/candles.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/API/products/candles.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/API/products/catalogue.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/API/products/catalogue.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/Coinbase.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/Coinbase.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Coinbase/orders/place.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Coinbase/orders/place.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/DOGE/doge.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/clouds/DOGE/doge.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/_status/API_status_combine_1.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/_status/API_status_combine_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/procedures/options/combine.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/procedures/options/combine.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/procedures/options/example_responses/NOVA_options_chain.JSON` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/procedures/options/example_responses/NOVA_options_chain.JSON`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/lookup/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/options/chains/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/options/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/options/chains/parse_1.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/options/chains/parse_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/options/expirations/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Tradier/v1/markets/options/expirations/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/treasure/indicators/RMI_Trend_Sniper.pine` & `theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/treasure/indicators/RMI_Trend_Sniper.pine`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals_v2/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals_v2/rooms/print_symbols_table.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/TradingView/treasure/technicals_v2/rooms/scan_symbol.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Yahoo/retrieve.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Yahoo/retrieve.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/clouds/Yahoo/retrieve_change.py` & `theme_park-2.0.0/venues/stages/theme_park/clouds/Yahoo/retrieve_change.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/fluctuators/bt/strategies/example_1.py` & `theme_park-2.0.0/venues/stages/theme_park/fluctuators/bt/strategies/example_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/fluctuators/fluctuators.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/fluctuators/fluctuators.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/gadgets/clock/UTC/greatness_1.py` & `theme_park-2.0.0/venues/stages/theme_park/gadgets/clock/UTC/greatness_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/gadgets/format_percentage.py` & `theme_park-2.0.0/venues/stages/theme_park/gadgets/format_percentage.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/gadgets/pandas/DF/_status/status_from_1.py` & `theme_park-2.0.0/venues/stages/theme_park/gadgets/pandas/DF/_status/status_from_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/gadgets/pandas/pandas.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/gadgets/pandas/pandas.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/gadgets/summation/summation.svg` & `theme_park-2.0.0/venues/stages/theme_park/gadgets/summation/summation.svg`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/home.MD` & `theme_park-2.0.0/venues/stages/theme_park/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 
+
 Bravo! You have received a Mercantilism Diploma in "theme_park" from the Orbital Convergence University International Air and Water Embassy of the Tangerine Planet (the planet that is one ellipse further from the Sun than Earth's ellipse).
 
 You are now officially certified to include "theme_park" in your practice.
 
 --
 # theme_park
 
@@ -11,23 +12,26 @@
 ```
 pip install theme_park
 ```
 
 ## tutorial
 This starts a dashboard on port 20000 that can be opened in a browser.
 ```
-theme_park help
+theme_park school
 ```
 ```
-theme_park help --port 20001
+theme_park school --port 20001
 ```
 
 
 ## rides (OCHLV)
+```
 rides.season_3.super_hero_trend
+```
+
 
 ## stats (options)
 ### stats.aggregate_break_even
 ```
 """
 	formula:
 		for each contract:
```

### Comparing `theme_park-1.0.0/venues/stages/theme_park/home.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/home.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/rides.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/rides/rides.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/ATR/ChatGPT_ATR_1/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/ATR/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/ATR/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/ATR/_status/status_1.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/ATR/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/Andean_Oscillator/AO.pine` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/Andean_Oscillator/AO.pine`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/HHLL/indicator.pine` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/HHLL/indicator.pine`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/RSI/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/RSI/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/TR/True Range.svg` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/TR/True Range.svg`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/TR/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/TR/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/TR/_status/status_1.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/TR/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/TR/_status/status_2.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/TR/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/VWAP/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/VWAP/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/indicators.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/indicators.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/pivot_point/pivot_point.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/pivot_point/pivot_point.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/supertrend/ST_1_ChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/supertrend/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/supertrend/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_1/supertrend/_status/status_1.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_1/supertrend/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_2/AAS/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_2/AAS/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_2/AAS/_status/status_1.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_2/AAS/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_2/AS/AS.svg` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_2/AS/AS.svg`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_2/AS/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_2/AS/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_2/AS/_status/status_2.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_2/AS/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_2/pecdency/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_2/pecdency/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_2/pecdency/__init__v1.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_2/pecdency/__init__v1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/ST/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/ST/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/VSA/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/VSA/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span/AS.svg` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span/AS.svg`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span/_status/status_1.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span/_status/status_2.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span_average/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span_average/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span_average/_status/status_1.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span_average/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span_reversals/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span_reversals/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/physical_span_roads_v1/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/physical_span_roads_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/super_hero_trend/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/super_hero_trend/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/super_hero_trend/win_rates/shares_trading.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/super_hero_trend/win_rates/shares_trading.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_3/supertrend/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_3/supertrend/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_4/AO/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_4/AO/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_4/ML_Lorentzian/KernelFunctions.ps` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_4/ML_Lorentzian/KernelFunctions.ps`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_4/ML_Lorentzian/Lorentzian Classification.ps` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_4/ML_Lorentzian/Lorentzian Classification.ps`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_4/ML_Lorentzian/MLExtensions.ps` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_4/ML_Lorentzian/MLExtensions.ps`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_4/superb/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_4/superb/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/rides/season_4/superb/win_rates/shares_trading.py` & `theme_park-2.0.0/venues/stages/theme_park/rides/season_4/superb/win_rates/shares_trading.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/scans/_clique/ETF.py` & `theme_park-2.0.0/venues/stages/theme_park/scans/_clique/ETF.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/scans/_clique/TV.py` & `theme_park-2.0.0/venues/stages/theme_park/scans/_clique/TV.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/scans/_clique/currency.py` & `theme_park-2.0.0/venues/stages/theme_park/scans/_clique/currency.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/scans/symbol/symbols.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/scans/symbol/symbols.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/squeeze pc ratios.r.HTML` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/squeeze pc ratios.r.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/examples/1.JSON` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/examples/1.JSON`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/examples/2.JSON` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/examples/2.JSON`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/status_1.py` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/status_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/status_2.py` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_PC_ratio/status/status_2.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/examples/0.JSON` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/examples/0.JSON`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/examples/1.JSON` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/examples/1.JSON`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/examples/2.JSON` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/examples/2.JSON`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/status_1.py` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/status_2.py` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/_status/status_2.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/aggregate break even.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/aggregate break even.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_break_even/show/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_break_even/show/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/aggregate_multiplier/aggregate_multipliers.r.HTML` & `theme_park-2.0.0/venues/stages/theme_park/stats/aggregate_multiplier/aggregate_multipliers.r.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/clique.py` & `theme_park-2.0.0/venues/stages/theme_park/stats/clique.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/stats/stats.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/stats/stats.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/treasures/commodities/commodities.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/treasures/commodities/commodities.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/treasures/crypto/crypto.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/treasures/crypto/crypto.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/treasures/crypto/crypto_usual_features.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/treasures/crypto/crypto_usual_features.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/treasures/options/movement_calculator/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/treasures/options/movement_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/treasures/options/movement_calculator/slope.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/treasures/options/movement_calculator/slope.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/treasures/options/multipliers/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/treasures/options/multipliers/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/treasures/options/shapes/shape_1/__init__.py` & `theme_park-2.0.0/venues/stages/theme_park/treasures/options/shapes/shape_1/__init__.py`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/loan - varieties.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/loan - varieties.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/loan.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/loan.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/sources/sources.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/loans/mortgages/sources/sources.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/treasures/real_estate/varieties/varieties.S.HTML` & `theme_park-2.0.0/venues/stages/theme_park/treasures/real_estate/varieties/varieties.S.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/venues/stages/theme_park/treasures/shares/ETF/ETF.s.HTML` & `theme_park-2.0.0/venues/stages/theme_park/treasures/shares/ETF/ETF.s.HTML`

 * *Files identical despite different names*

### Comparing `theme_park-1.0.0/PKG-INFO` & `theme_park-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theme_park
-Version: 1.0.0
+Version: 2.0.0
 Summary: Welcome friends and fam!  The theme park is open! :)
 License: GPL 3.0 + CC BY-NC-SA 4.0 + Mongo SSPL
 Keywords: rollercoaster through layer 9,non-repulsive,attractive,vortex,rain & pour,economic estimation,finance,commerce,wealth,money,treasures,treasury,subconscious trading,implicit trading
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -42,14 +42,15 @@
 Requires-Dist: ta (>=0.11.0,<0.12.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: talipp (>=2.2.0,<3.0.0)
 Requires-Dist: technical-indicators-lib (>=0.0.2,<0.0.3)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tradingview-screener (>=2.4.1,<3.0.0)
 Requires-Dist: tradingview-ta (>=3.3.0,<4.0.0)
+Requires-Dist: ventures (>=1.6.0,<2.0.0)
 Requires-Dist: yahooquery (>=2.3.7,<3.0.0)
 Requires-Dist: yfinance (>=0.2.37,<0.3.0)
 Project-URL: GitLab, https://gitlab.com/reptilian_climates/modules_series_4/apoplast
 Description-Content-Type: text/markdown
```

