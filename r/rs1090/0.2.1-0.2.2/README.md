# Comparing `tmp/rs1090-0.2.1.tar.gz` & `tmp/rs1090-0.2.2.tar.gz`

## Comparing `rs1090-0.2.1.tar` & `rs1090-0.2.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0     1001      127     1097 2024-05-23 21:53:59.000000 rs1090-0.2.1/crates/rs1090/Cargo.toml
--rw-r--r--   0     1001      127     2869 2024-05-23 21:53:59.000000 rs1090-0.2.1/crates/rs1090/benches/long_flight.rs
--rw-r--r--   0     1001      127  1829500 2024-05-23 21:53:59.000000 rs1090-0.2.1/crates/rs1090/data/airports.json
--rw-r--r--   0     1001      127 13658890 2024-05-23 21:53:59.000000 rs1090-0.2.1/crates/rs1090/data/flarm.csv
--rw-r--r--   0     1001      127 10186581 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/data/long_flight.csv
--rw-r--r--   0     1001      127    56601 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/data/patterns.json
--rw-r--r--   0     1001      127      640 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/examples/airports.rs
--rw-r--r--   0     1001      127      319 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/examples/basic.rs
--rw-r--r--   0     1001      127     2341 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/examples/flight.rs
--rw-r--r--   0     1001      127     4413 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/readme.md
--rw-r--r--   0     1001      127     1414 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/data/airports.rs
--rw-r--r--   0     1001      127       50 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/data/mod.rs
--rw-r--r--   0     1001      127     1132 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/data/patterns.rs
--rw-r--r--   0     1001      127    16778 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/data/tail.rs
--rw-r--r--   0     1001      127     4956 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/adsb.rs
--rw-r--r--   0     1001      127     4794 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds05.rs
--rw-r--r--   0     1001      127     5338 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds06.rs
--rw-r--r--   0     1001      127     7761 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds08.rs
--rw-r--r--   0     1001      127    14592 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds09.rs
--rw-r--r--   0     1001      127     4713 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds10.rs
--rw-r--r--   0     1001      127     6158 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds17.rs
--rw-r--r--   0     1001      127     1760 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds20.rs
--rw-r--r--   0     1001      127     5945 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds30.rs
--rw-r--r--   0     1001      127     5133 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds40.rs
--rw-r--r--   0     1001      127     5885 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds44.rs
--rw-r--r--   0     1001      127     6611 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds50.rs
--rw-r--r--   0     1001      127     7132 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds60.rs
--rw-r--r--   0     1001      127     2461 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds61.rs
--rw-r--r--   0     1001      127     8982 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds62.rs
--rw-r--r--   0     1001      127    12441 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/bds65.rs
--rw-r--r--   0     1001      127      225 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/bds/mod.rs
--rw-r--r--   0     1001      127     6285 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/commb.rs
--rw-r--r--   0     1001      127    20142 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/cpr.rs
--rw-r--r--   0     1001      127     6422 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/crc.rs
--rw-r--r--   0     1001      127    14003 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/flarm.rs
--rw-r--r--   0     1001      127    27430 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/decode/mod.rs
--rw-r--r--   0     1001      127     1172 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/lib.rs
--rw-r--r--   0     1001      127     3963 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/source/beast.rs
--rw-r--r--   0     1001      127       78 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/source/mod.rs
--rw-r--r--   0     1001      127     2643 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/source/radarcape.rs
--rw-r--r--   0     1001      127    20992 2024-05-23 21:54:00.000000 rs1090-0.2.1/crates/rs1090/src/source/rtlsdr.rs
--rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 rs1090-0.2.1/python/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/.gitignore
--rw-r--r--   0     1001      127     8431 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/examples/bench_pms.py
--rw-r--r--   0     1001      127     2255 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/examples/benchmark.py
--rw-r--r--   0     1001      127    15135 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/examples/benchmark.svg
--rw-r--r--   0     1001      127    54306 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/examples/flarm.png
--rw-r--r--   0     1001      127     2266 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/examples/flarm.py
--rw-r--r--   0     1001      127      753 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/examples/long_flight.py
--rw-r--r--   0     1001      127     1654 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/readme.md
--rw-r--r--   0     1001      127     4403 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/rs1090/__init__.py
--rw-r--r--   0     1001      127      689 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/rs1090/_rust.pyi
--rw-r--r--   0     1001      127        0 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/rs1090/py.typed
--rw-r--r--   0     1001      127    18575 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/rs1090/stubs.py
--rw-r--r--   0     1001      127     7222 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/src/lib.rs
--rw-r--r--   0     1001      127     2091 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/tests/test_adsb.py
--rw-r--r--   0     1001      127      281 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/tests/test_aircraft.py
--rw-r--r--   0     1001      127     1340 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/tests/test_commb.py
--rw-r--r--   0     1001      127     1282 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/tests/test_common.py
--rw-r--r--   0     1001      127     1554 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/tests/test_flarm.py
--rw-r--r--   0     1001      127      423 2024-05-23 21:54:00.000000 rs1090-0.2.1/python/tests/test_full.py
--rw-r--r--   0     1001      127    83296 2024-05-23 21:53:59.000000 rs1090-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 rs1090-0.2.1/Cargo.toml
--rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 rs1090-0.2.1/pyproject.toml
--rw-r--r--   0     1001      127     4403 2024-05-23 21:54:00.000000 rs1090-0.2.1/rs1090/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-23 21:54:00.000000 rs1090-0.2.1/rs1090/py.typed
--rw-r--r--   0     1001      127      689 2024-05-23 21:54:00.000000 rs1090-0.2.1/rs1090/_rust.pyi
--rw-r--r--   0     1001      127    18575 2024-05-23 21:54:00.000000 rs1090-0.2.1/rs1090/stubs.py
--rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 rs1090-0.2.1/PKG-INFO
+-rw-r--r--   0     1001      127     1097 2024-05-27 14:00:37.000000 rs1090-0.2.2/crates/rs1090/Cargo.toml
+-rw-r--r--   0     1001      127     2869 2024-05-27 14:00:37.000000 rs1090-0.2.2/crates/rs1090/benches/long_flight.rs
+-rw-r--r--   0     1001      127  1829500 2024-05-27 14:00:37.000000 rs1090-0.2.2/crates/rs1090/data/airports.json
+-rw-r--r--   0     1001      127 13658890 2024-05-27 14:00:37.000000 rs1090-0.2.2/crates/rs1090/data/flarm.csv
+-rw-r--r--   0     1001      127 10186581 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/data/long_flight.csv
+-rw-r--r--   0     1001      127    56601 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/data/patterns.json
+-rw-r--r--   0     1001      127      640 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/examples/airports.rs
+-rw-r--r--   0     1001      127      319 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/examples/basic.rs
+-rw-r--r--   0     1001      127     2427 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/examples/flight.rs
+-rw-r--r--   0     1001      127     4413 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/readme.md
+-rw-r--r--   0     1001      127     1414 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/data/airports.rs
+-rw-r--r--   0     1001      127       50 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/data/mod.rs
+-rw-r--r--   0     1001      127     1132 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/data/patterns.rs
+-rw-r--r--   0     1001      127    16778 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/data/tail.rs
+-rw-r--r--   0     1001      127     4956 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/adsb.rs
+-rw-r--r--   0     1001      127     4794 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds05.rs
+-rw-r--r--   0     1001      127     5338 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds06.rs
+-rw-r--r--   0     1001      127     7761 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds08.rs
+-rw-r--r--   0     1001      127    14592 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds09.rs
+-rw-r--r--   0     1001      127     4713 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds10.rs
+-rw-r--r--   0     1001      127     6158 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds17.rs
+-rw-r--r--   0     1001      127     1760 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds20.rs
+-rw-r--r--   0     1001      127     5945 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds30.rs
+-rw-r--r--   0     1001      127     5133 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds40.rs
+-rw-r--r--   0     1001      127     5885 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds44.rs
+-rw-r--r--   0     1001      127     6611 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds50.rs
+-rw-r--r--   0     1001      127     7132 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds60.rs
+-rw-r--r--   0     1001      127     2461 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds61.rs
+-rw-r--r--   0     1001      127     8982 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds62.rs
+-rw-r--r--   0     1001      127    12441 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/bds65.rs
+-rw-r--r--   0     1001      127      225 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/bds/mod.rs
+-rw-r--r--   0     1001      127     6285 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/commb.rs
+-rw-r--r--   0     1001      127    20142 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/cpr.rs
+-rw-r--r--   0     1001      127     6422 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/crc.rs
+-rw-r--r--   0     1001      127    14003 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/flarm.rs
+-rw-r--r--   0     1001      127    27811 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/decode/mod.rs
+-rw-r--r--   0     1001      127     1172 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/lib.rs
+-rw-r--r--   0     1001      127     3963 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/source/beast.rs
+-rw-r--r--   0     1001      127       78 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/source/mod.rs
+-rw-r--r--   0     1001      127     3075 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/source/radarcape.rs
+-rw-r--r--   0     1001      127    21137 2024-05-27 14:00:38.000000 rs1090-0.2.2/crates/rs1090/src/source/rtlsdr.rs
+-rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 rs1090-0.2.2/python/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/.gitignore
+-rw-r--r--   0     1001      127     8431 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/examples/bench_pms.py
+-rw-r--r--   0     1001      127     2255 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/examples/benchmark.py
+-rw-r--r--   0     1001      127    15135 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/examples/benchmark.svg
+-rw-r--r--   0     1001      127    54306 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/examples/flarm.png
+-rw-r--r--   0     1001      127     2266 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/examples/flarm.py
+-rw-r--r--   0     1001      127      753 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/examples/long_flight.py
+-rw-r--r--   0     1001      127     1654 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/readme.md
+-rw-r--r--   0     1001      127     4403 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/rs1090/__init__.py
+-rw-r--r--   0     1001      127      689 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/rs1090/_rust.pyi
+-rw-r--r--   0     1001      127        0 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/rs1090/py.typed
+-rw-r--r--   0     1001      127    18575 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/rs1090/stubs.py
+-rw-r--r--   0     1001      127     7314 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/src/lib.rs
+-rw-r--r--   0     1001      127     2091 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/tests/test_adsb.py
+-rw-r--r--   0     1001      127      281 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/tests/test_aircraft.py
+-rw-r--r--   0     1001      127     1340 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/tests/test_commb.py
+-rw-r--r--   0     1001      127     1282 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/tests/test_common.py
+-rw-r--r--   0     1001      127     1554 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/tests/test_flarm.py
+-rw-r--r--   0     1001      127      423 2024-05-27 14:00:38.000000 rs1090-0.2.2/python/tests/test_full.py
+-rw-r--r--   0     1001      127    83741 2024-05-27 14:00:37.000000 rs1090-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 rs1090-0.2.2/Cargo.toml
+-rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 rs1090-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      127     4403 2024-05-27 14:00:38.000000 rs1090-0.2.2/rs1090/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-27 14:00:38.000000 rs1090-0.2.2/rs1090/py.typed
+-rw-r--r--   0     1001      127      689 2024-05-27 14:00:38.000000 rs1090-0.2.2/rs1090/_rust.pyi
+-rw-r--r--   0     1001      127    18575 2024-05-27 14:00:38.000000 rs1090-0.2.2/rs1090/stubs.py
+-rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 rs1090-0.2.2/PKG-INFO
```

### Comparing `rs1090-0.2.1/crates/rs1090/Cargo.toml` & `rs1090-0.2.2/crates/rs1090/Cargo.toml`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/benches/long_flight.rs` & `rs1090-0.2.2/crates/rs1090/benches/long_flight.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/data/airports.json` & `rs1090-0.2.2/crates/rs1090/data/airports.json`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/data/flarm.csv` & `rs1090-0.2.2/crates/rs1090/data/flarm.csv`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/data/long_flight.csv` & `rs1090-0.2.2/crates/rs1090/data/long_flight.csv`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/data/patterns.json` & `rs1090-0.2.2/crates/rs1090/data/patterns.json`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/examples/airports.rs` & `rs1090-0.2.2/crates/rs1090/examples/airports.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/examples/flight.rs` & `rs1090-0.2.2/crates/rs1090/examples/flight.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use rayon::prelude::*;
 use rs1090::decode::cpr::{decode_positions, Position};
+use rs1090::decode::TimeSource;
 use rs1090::prelude::*;
 
 use std::env;
 use std::fs::File;
 use std::io::{self, BufRead, BufReader, Read};
 use std::vec::Vec;
 
@@ -60,14 +61,15 @@
                     parts.next().unwrap().parse::<f64>().expect("not a float");
                 let msg = parts.next().unwrap();
                 let hex = &mut msg.to_string()[18..].to_string();
                 let bytes = hex::decode(&hex).unwrap();
                 let (_, msg) = Message::from_bytes((&bytes, 0)).unwrap();
                 res.push(TimedMessage {
                     timestamp,
+                    timesource: TimeSource::External,
                     frame: hex.to_string(),
                     message: Some(msg),
                     idx: 0,
                 });
             }
             res
         })
```

### Comparing `rs1090-0.2.1/crates/rs1090/readme.md` & `rs1090-0.2.2/crates/rs1090/readme.md`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/data/airports.rs` & `rs1090-0.2.2/crates/rs1090/src/data/airports.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/data/patterns.rs` & `rs1090-0.2.2/crates/rs1090/src/data/patterns.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/data/tail.rs` & `rs1090-0.2.2/crates/rs1090/src/data/tail.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/adsb.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/adsb.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds05.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds05.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds06.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds06.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds08.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds08.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds09.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds09.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds10.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds10.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds17.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds17.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds20.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds20.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds30.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds30.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds40.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds40.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds44.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds44.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds50.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds50.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds60.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds60.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds61.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds61.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds62.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds62.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/bds/bds65.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/bds/bds65.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/commb.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/commb.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/cpr.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/cpr.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/crc.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/crc.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/flarm.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/flarm.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/decode/mod.rs` & `rs1090-0.2.2/crates/rs1090/src/decode/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -397,17 +397,30 @@
             }
         }
         Ok(())
     }
 }
 
 #[derive(Serialize)]
+#[serde(rename_all = "lowercase")]
+pub enum TimeSource {
+    /// The timestamp is provided by the system when it receives the message
+    System,
+    /// The timestamp is provided by the GPS in the header of the message
+    Radarcape,
+    /// The timestamp is provided by the user asking to decode the message
+    External,
+}
+
+#[derive(Serialize)]
 pub struct TimedMessage {
     pub timestamp: f64,
 
+    pub timesource: TimeSource,
+
     pub frame: String,
 
     #[serde(flatten)]
     pub message: Option<Message>,
 
     pub idx: usize,
 }
```

### Comparing `rs1090-0.2.1/crates/rs1090/src/lib.rs` & `rs1090-0.2.2/crates/rs1090/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/source/beast.rs` & `rs1090-0.2.2/crates/rs1090/src/source/beast.rs`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/crates/rs1090/src/source/rtlsdr.rs` & `rs1090-0.2.2/crates/rs1090/src/source/rtlsdr.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use std::time::{SystemTime, UNIX_EPOCH};
 
 use num_complex::Complex;
 use soapysdr::{Device, Direction};
 use tokio::sync::mpsc;
 
 use crate::decode::crc::modes_checksum;
-use crate::decode::TimedMessage;
+use crate::decode::{TimeSource, TimedMessage};
 use std::fmt::{self, Display, Formatter};
 
 const DIRECTION: Direction = Direction::Rx;
 const MODES_FREQ: f64 = 1.09e9;
 const RTLSDR_RATE: f64 = 2.4e6;
 const RTLSDR_GAIN: f64 = 49.6;
 
@@ -40,32 +40,35 @@
 
     let mut stream = device.rx_stream::<Complex<i16>>(&[channel]).unwrap();
 
     let mut buf = vec![Complex::new(0, 0); stream.mtu().unwrap()];
     stream.activate(None).unwrap();
 
     // Spawn a thread to send messages
-    loop {
+    'receive: loop {
         match stream.read(&mut [&mut buf], 5_000_000) {
             Ok(len) => {
                 let buf = &buf[..len];
                 let outbuf = magnitude(buf);
                 let resulting_data = demodulate2400(&outbuf).unwrap();
                 for data in resulting_data {
                     let timestamp = SystemTime::now()
                         .duration_since(UNIX_EPOCH)
                         .expect("SystemTime before unix epoch")
-                        .as_secs_f64();
+                        .as_micros();
                     let msg = TimedMessage {
-                        timestamp,
+                        timestamp: timestamp as f64 * 1e-6,
+                        timesource: TimeSource::System,
                         frame: hex::encode(data),
                         message: None,
                         idx,
                     };
-                    tx.send(msg).await.expect("Failed to send message");
+                    if tx.send(msg).await.is_err() {
+                        break 'receive;
+                    }
                 }
             }
             Err(e) => {
                 eprintln!("SoapySDR read error: {}", e);
             }
         }
     }
```

### Comparing `rs1090-0.2.1/python/Cargo.toml` & `rs1090-0.2.2/python/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "_rust"
 crate-type = ["cdylib"]
 
 [dependencies]
 hex = "0.4.3"
-pyo3 = "0.19.0"
+pyo3 = "0.21.2"
 rayon = "1.9.0"
 regex = "1.10.4"
-rs1090 = { version= "0.2.1", path = "../crates/rs1090" }
+rs1090 = { version= "0.2.2", path = "../crates/rs1090" }
 serde-pickle = "1.1.1"
```

### Comparing `rs1090-0.2.1/python/.gitignore` & `rs1090-0.2.2/python/.gitignore`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/examples/bench_pms.py` & `rs1090-0.2.2/python/examples/bench_pms.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/examples/benchmark.py` & `rs1090-0.2.2/python/examples/benchmark.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/examples/benchmark.svg` & `rs1090-0.2.2/python/examples/benchmark.svg`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/examples/flarm.png` & `rs1090-0.2.2/python/examples/flarm.png`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/examples/flarm.py` & `rs1090-0.2.2/python/examples/flarm.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/examples/long_flight.py` & `rs1090-0.2.2/python/examples/long_flight.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/readme.md` & `rs1090-0.2.2/python/readme.md`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/rs1090/__init__.py` & `rs1090-0.2.2/python/rs1090/__init__.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/rs1090/_rust.pyi` & `rs1090-0.2.2/python/rs1090/_rust.pyi`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/rs1090/stubs.py` & `rs1090-0.2.2/python/rs1090/stubs.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/src/lib.rs` & `rs1090-0.2.2/python/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 use pyo3::prelude::*;
 use rayon::prelude::*;
 use regex::Regex;
 use rs1090::data::patterns::PATTERNS;
 use rs1090::data::tail::tail;
 use rs1090::decode::cpr::{decode_positions, Position};
 use rs1090::decode::flarm::Flarm;
+use rs1090::decode::TimeSource;
 use rs1090::prelude::*;
 
 #[pyfunction]
 fn decode_1090(msg: String) -> PyResult<Vec<u8>> {
     let bytes = hex::decode(msg).unwrap();
     if let Ok((_, msg)) = Message::from_bytes((&bytes, 0)) {
         let pkl = serde_pickle::to_vec(&msg, Default::default()).unwrap();
@@ -57,14 +58,15 @@
             msgs.iter()
                 .zip(ts)
                 .filter_map(|(msg, timestamp)| {
                     let bytes = hex::decode(msg).unwrap();
                     if let Ok((_, message)) = Message::from_bytes((&bytes, 0)) {
                         Some(TimedMessage {
                             timestamp,
+                            timesource: TimeSource::External,
                             frame: msg.to_string(),
                             message: Some(message),
                             idx: 0,
                         })
                     } else {
                         None
                     }
@@ -211,15 +213,15 @@
     }
 
     Ok(reg)
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
-fn _rust(_py: Python, m: &PyModule) -> PyResult<()> {
+fn _rust(m: &Bound<'_, PyModule>) -> PyResult<()> {
     // Decoding functions
     m.add_function(wrap_pyfunction!(decode_1090, m)?)?;
     m.add_function(wrap_pyfunction!(decode_1090_vec, m)?)?;
     m.add_function(wrap_pyfunction!(decode_1090t_vec, m)?)?;
     m.add_function(wrap_pyfunction!(decode_flarm, m)?)?;
     m.add_function(wrap_pyfunction!(decode_flarm_vec, m)?)?;
```

### Comparing `rs1090-0.2.1/python/tests/test_adsb.py` & `rs1090-0.2.2/python/tests/test_adsb.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/tests/test_commb.py` & `rs1090-0.2.2/python/tests/test_commb.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/tests/test_common.py` & `rs1090-0.2.2/python/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/python/tests/test_flarm.py` & `rs1090-0.2.2/python/tests/test_flarm.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/Cargo.lock` & `rs1090-0.2.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -38,26 +38,26 @@
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "allocator-api2"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
@@ -83,55 +83,56 @@
 checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.11"
+version = "0.6.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6e2e1ebcb11de5c03c67de28a7df593d32191b44939c482e97702baaaa6ab6a5"
+checksum = "418c75fa768af9c03be99d17643f93f79bbba589895012a80e3452a19ddda15b"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
+ "is_terminal_polyfill",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+checksum = "c03a11a9034d92058ceb6ee011ce58af4a9bf61491aa7e1e59ecd24bd40d22d4"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+checksum = "a64c907d4e79225ac72e2a354c9ce84d50ebb4586dee56c82b3ee73004f537f5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "3.0.2"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+checksum = "61a38449feb7068f52bb06c12759005cf459ee52bb4adc1d5a7c4322d716fb19"
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "approx"
@@ -166,28 +167,34 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
+name = "atomic-waker"
+version = "1.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1505bd5d3d116872e7271a6d4e16d81d0c8570876c8de68093a09ac269d8aac0"
+
+[[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -208,39 +215,39 @@
 
 [[package]]
 name = "bindgen"
 version = "0.66.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f2b84e06fc203107bfbad243f4aba2af864eb7db3b1cf46ea0a023b0b433d2a7"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cexpr",
  "clang-sys",
  "lazy_static",
  "lazycell",
  "peeking_take_while",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bitvec"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
 dependencies = [
@@ -257,29 +264,29 @@
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.3"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ea184aa71bb362a1157c896979544cc23974e08fd265f29ea96b59f0b4a555b"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "bzip2"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bdb116a6ef3f6c3698828873ad02c3014b3c85cadb88496095628e3ef1e347f8"
 dependencies = [
@@ -317,19 +324,21 @@
 checksum = "8a17ed5635fc8536268e5d4de1e22e81ac34419e5f052d4d51f4e01dcc263fcc"
 dependencies = [
  "rustversion",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.88"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02f341c093d19155a6e41631ce5971aac4e9a868262212153124c15fa22d1cdc"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 dependencies = [
+ "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cexpr"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
@@ -341,24 +350,24 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
- "windows-targets 0.52.3",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "ciborium"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42e69ffd6f0917f5c029256a24d0161db17cea3997d185db0d35926308770f0e"
@@ -392,78 +401,69 @@
 dependencies = [
  "crypto-common",
  "inout",
 ]
 
 [[package]]
 name = "clang-sys"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67523a3b4be3ce1989d607a828d036249522dd9c1c8de7f4dd2dae43a37369d1"
+checksum = "a483f3cbf7cec2e153d424d0e92329d816becc6421389bd494375c6065921b9b"
 dependencies = [
  "glob",
  "libc",
  "libloading",
 ]
 
 [[package]]
 name = "clap"
-version = "4.5.1"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c918d541ef2913577a0f9566e9ce27cb35b6df072075769e0b26cb5a554520da"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.5.1"
+version = "4.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f3e7391dad68afb0c2ede1bf619f579a3dc9c2ec67f089baa397123a2f3d1eb"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
 dependencies = [
  "anstream",
  "anstyle",
  "clap_lex",
- "strsim 0.11.0",
+ "strsim 0.11.1",
  "terminal_size",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.5.0"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "307bc0538d5f0f83b8248db3087aa92fe504e4691294d0c96c0eabc33f47ba47"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
- "heck",
+ "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
-name = "cmake"
-version = "0.1.50"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
-dependencies = [
- "cc",
-]
-
-[[package]]
 name = "colorchoice"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+checksum = "0b6a852b24ab71dffc585bcb46eaf7959d175cb865a7152e35b348d1b2960422"
 
 [[package]]
 name = "compact_str"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f86b9c4c00838774a6d902ef931eff7470720c51d90c2e32cfe15dc304737b3f"
 dependencies = [
@@ -518,17 +518,17 @@
 name = "crc-catalog"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19d374276b40fb8bbdee95aef7c7fa6b5316ec764510eb64b8dd0e2ed0d7e7f5"
 
 [[package]]
 name = "crc32fast"
-version = "1.4.0"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
+checksum = "a97769d94ddab943e4510d138150169a2758b5ef3eb191a9ee688de3e23ef7b3"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "criterion"
 version = "0.5.1"
@@ -582,25 +582,25 @@
 checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "crossterm"
 version = "0.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f476fe445d41c9e991fd07515a6f463074b782242ccf4a5b7b1d1012e70824df"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "crossterm_winapi",
  "futures-core",
  "libc",
  "mio",
  "parking_lot",
  "signal-hook",
  "signal-hook-mio",
@@ -665,21 +665,21 @@
  "darling_core",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "data-encoding"
-version = "2.5.0"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e962a19be5cfc3f3bf6dd8f61eb50107f356ad6270fbb3ed41476571db78be5"
+checksum = "e8566979429cf69b49a5c740c60791108e86440e8be149bbea4fe54d2c32d6e2"
 
 [[package]]
 name = "decode1090"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "clap",
  "deku",
  "futures-util",
  "hex",
  "rs1090",
  "serde",
@@ -729,15 +729,15 @@
 name = "derive_arbitrary"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67e77553c4162a157adbf834ebae5b415acbecbeafc7a74b0e886657506a7611"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
@@ -751,43 +751,43 @@
 name = "displaydoc"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "487585f4d0c6655fe74905e2504d8ad6908e4db67f744eb140876906c2f3175d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.33"
+version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
+checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fallible-iterator"
@@ -810,15 +810,14 @@
 [[package]]
 name = "flate2"
 version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
- "libz-ng-sys",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -906,15 +905,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -951,17 +950,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -974,17 +973,17 @@
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "h2"
-version = "0.3.25"
+version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fbd2820c5e49886948654ab546d0688ff24530286bdcf8fca3cefb16d4618eb"
+checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http 0.2.12",
@@ -993,46 +992,46 @@
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "h2"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "816ec7294445779408f36fe57bc5b7fc1cf59664059096c65f905c1c61f58069"
+checksum = "fa82e28a107a8cc405f0839610bdc9b15f1e25ec7d696aa5cf173edbcb1486ab"
 dependencies = [
+ "atomic-waker",
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
- "futures-util",
  "http 1.1.0",
  "indexmap",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "half"
-version = "2.3.1"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
  "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 dependencies = [
  "ahash",
  "allocator-api2",
 ]
 
 [[package]]
 name = "hashlink"
@@ -1070,18 +1069,24 @@
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
+name = "heck"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
+
+[[package]]
 name = "hermit-abi"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "379dada1584ad501b383485dd706b8afb7a70fcbc7f4da7d780638a5a6124a60"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
@@ -1174,15 +1179,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
- "h2 0.3.25",
+ "h2 0.3.26",
  "http 0.2.12",
  "http-body 0.4.6",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
  "socket2",
@@ -1197,15 +1202,15 @@
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe575dd17d0862a9a33781c8c4696a55c320909004a67a00fb286ba8b1bc496d"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
- "h2 0.4.4",
+ "h2 0.4.5",
  "http 1.1.0",
  "http-body 1.0.0",
  "httparse",
  "itoa",
  "pin-project-lite",
  "smallvec",
  "tokio",
@@ -1226,17 +1231,17 @@
  "tokio",
  "tokio-native-tls",
  "tower-service",
 ]
 
 [[package]]
 name = "hyper-util"
-version = "0.1.3"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
+checksum = "3d8d52be92d09acc2e01dddb7fde3ad983fc6489c7db4837e605bc3fca4cb63e"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
  "http 1.1.0",
  "http-body 1.0.0",
  "hyper 1.3.1",
@@ -1285,30 +1290,24 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.2.3"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "233cf39063f058ea2caae4091bf4a3ef70a653afbc026f5c4a4135d114e3c177"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
-
-[[package]]
-name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "inout"
 version = "0.1.3"
@@ -1332,14 +1331,20 @@
 dependencies = [
  "hermit-abi",
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "is_terminal_polyfill"
+version = "1.70.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8478577c03552c21db0e2724ffb8986a5ce7af88107e6be5d2ee6e158c12800"
+
+[[package]]
 name = "iter-read"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c397ca3ea05ad509c4ec451fea28b4771236a376ca1c69fd5143aae0cf8f93c4"
 
 [[package]]
 name = "itertools"
@@ -1357,21 +1362,21 @@
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jet1090"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "chrono",
  "clap",
  "crossterm",
  "deku",
  "futures",
  "futures-util",
@@ -1385,18 +1390,27 @@
  "soapysdr",
  "tokio",
  "warp",
  "zip",
 ]
 
 [[package]]
+name = "jobserver"
+version = "0.1.31"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "js-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -1407,26 +1421,26 @@
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-targets 0.52.3",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
@@ -1439,44 +1453,40 @@
 dependencies = [
  "cc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
-name = "libz-ng-sys"
-version = "1.1.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6409efc61b12687963e602df8ecf70e8ddacf95bc6576bcf16e3ac6328083c5"
-dependencies = [
- "cmake",
- "libc",
-]
-
-[[package]]
 name = "linux-raw-sys"
-version = "0.4.13"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "lockfree-object-pool"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9374ef4228402d4b7e403e5838cb880d9ee663314b0a900d5a6aabf0c213552e"
+
+[[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "lru"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3262e75e648fce39813cb56ac41f3c3e3f65217ebf3844d818d1f9398cfb0dc"
 dependencies = [
@@ -1491,23 +1501,23 @@
 dependencies = [
  "byteorder",
  "crc",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
@@ -1528,26 +1538,26 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.10"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
@@ -1595,28 +1605,27 @@
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
+checksum = "c165a9ab64cf766f73521c0dd2cfdff64f488b8f0b3e621face3462d3db536d7"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-conv"
 version = "0.1.0"
@@ -1630,17 +1639,17 @@
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -1674,15 +1683,15 @@
 
 [[package]]
 name = "openssl"
 version = "0.10.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95a0481286a310808298130d22dd1fef0fa571e05a8f44ec801801e84b216b1f"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
@@ -1691,15 +1700,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -1714,40 +1723,40 @@
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
 
 [[package]]
 name = "pbkdf2"
 version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8ed6a7761f76e3b9f92dfb0a60a6a6477c61024b775147ff0973a02653abaf2"
 dependencies = [
@@ -1780,22 +1789,22 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -1803,41 +1812,47 @@
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "plotters"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
+checksum = "a15b6eccb8484002195a3e44fe65a4ce8e93a625797a063735536fd59cb01cf3"
 dependencies = [
  "num-traits",
  "plotters-backend",
  "plotters-svg",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "plotters-backend"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e76628b4d3a7581389a35d5b6e2139607ad7c75b17aed325f210aa91f4a9609"
+checksum = "414cec62c6634ae900ea1c56128dfe87cf63e7caece0852ec76aba307cebadb7"
 
 [[package]]
 name = "plotters-svg"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
+checksum = "81b30686a7d9c3e010b84284bdd26a29f2138574f52f5eb6f794fc0ad924e705"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "powerfmt"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
 [[package]]
 name = "ppv-lite86"
@@ -1853,86 +1868,89 @@
 dependencies = [
  "once_cell",
  "toml_edit",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
- "indoc 1.0.9",
+ "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.2"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
+ "heck 0.4.1",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -1967,37 +1985,37 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "ratatui"
-version = "0.26.1"
+version = "0.26.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcb12f8fbf6c62614b0d56eb352af54f6a22410c3b079eb53ee93c7b97dd31d8"
+checksum = "f44c9e68fd46eda15c646fbb85e1040b657a58cdc8c98db1d97a55930d991eef"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cassowary",
  "compact_str",
  "crossterm",
- "indoc 2.0.5",
  "itertools 0.12.1",
  "lru",
  "paste",
  "stability",
  "strum",
  "unicode-segmentation",
+ "unicode-truncate",
  "unicode-width",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -2007,19 +2025,19 @@
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
@@ -2028,56 +2046,56 @@
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "566cafdd92868e0939d3fb961bd0dc25fcfaaed179291093b3d43e6b3150ea10"
 dependencies = [
  "base64 0.22.1",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
- "h2 0.4.4",
+ "h2 0.4.5",
  "http 1.1.0",
  "http-body 1.0.0",
  "http-body-util",
  "hyper 1.3.1",
  "hyper-tls",
  "hyper-util",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "native-tls",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls-pemfile 2.1.2",
+ "rustls-pemfile",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper",
  "system-configuration",
  "tokio",
  "tokio-native-tls",
@@ -2087,15 +2105,15 @@
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
 name = "rs1090"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "ansi_term",
  "approx",
  "async-stream",
  "criterion",
  "deku",
  "futures",
@@ -2111,15 +2129,15 @@
  "serde_json",
  "soapysdr",
  "tokio",
 ]
 
 [[package]]
 name = "rs1090-python"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "hex",
  "pyo3",
  "rayon",
  "regex",
  "rs1090",
  "serde-pickle",
@@ -2127,58 +2145,49 @@
 
 [[package]]
 name = "rusqlite"
 version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b838eba278d213a8beaf485bd313fd580ca4505a00d5871caeb1457c55322cae"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "fallible-iterator",
  "fallible-streaming-iterator",
  "hashlink",
  "libsqlite3-sys",
  "smallvec",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
-dependencies = [
- "base64 0.21.7",
-]
-
-[[package]]
-name = "rustls-pemfile"
 version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
 dependencies = [
  "base64 0.22.1",
  "rustls-pki-types",
 ]
@@ -2187,23 +2196,23 @@
 name = "rustls-pki-types"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "976295e77ce332211c0d24d92c0e83e50f5c5f046d11082cea19f3df13a3562d"
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "955d28af4278de8121b7ebeb796b6a45735dc01436d898801014aced2773a3d6"
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -2229,19 +2238,19 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "security-framework"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
+checksum = "c627723fd09706bacdb5cf41499e95098555af3c3c29d014dc3c458ef6be11c0"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
@@ -2252,17 +2261,17 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-pickle"
 version = "1.1.1"
@@ -2274,28 +2283,28 @@
  "num-bigint",
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2346,17 +2355,17 @@
  "libc",
  "mio",
  "signal-hook",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "simd-adler32"
 version = "0.3.7"
@@ -2370,17 +2379,17 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "soapysdr"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24e2578203d938a532667e3e5d74917e65abd7afb17b4c2ebb7594f75de911ac"
 dependencies = [
@@ -2398,36 +2407,36 @@
  "bindgen",
  "cc",
  "pkg-config",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 
 [[package]]
 name = "stability"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ebd1b177894da2a2d9120208c3386066af06a488255caabc5de8ddca22dbc3ce"
+checksum = "2ff9eaf853dec4c8802325d8b6d3dffa86cc707fd7a1a4cdbf416e13b061787a"
 dependencies = [
  "quote",
- "syn 1.0.109",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
@@ -2436,17 +2445,17 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "strsim"
-version = "0.11.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ee073c9e4cd00e28217186dbe12796d692868f432bf2e97ee73bed0c56dfa01"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "strum"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d8cec3501a5194c432b2b7976db6b7d10ec95c253208b45f83f7136aa985e29"
 dependencies = [
@@ -2455,19 +2464,19 @@
 
 [[package]]
 name = "strum_macros"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
 dependencies = [
- "heck",
+ "heck 0.4.1",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
@@ -2481,17 +2490,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.50"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74f1bdc9872430ce9b75da68329d1c1746faf50ffac5f19e02b71e37ff881ffb"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2553,30 +2562,30 @@
 dependencies = [
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "time"
 version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
@@ -2617,17 +2626,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
@@ -2642,69 +2651,57 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
 dependencies = [
  "native-tls",
  "tokio",
 ]
 
 [[package]]
-name = "tokio-stream"
-version = "0.1.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "267ac89e0bec6e691e5813911606935d77c476ff49024f98abcea3e7b15e37af"
-dependencies = [
- "futures-core",
- "pin-project-lite",
- "tokio",
-]
-
-[[package]]
 name = "tokio-tungstenite"
-version = "0.20.1"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "212d5dcb2a1ce06d81107c3d0ffa3121fe974b73f068c8282cb1c32328113b6c"
+checksum = "c83b561d025642014097b66e6c1bb422783339e0909e4429cde4749d1990bc38"
 dependencies = [
  "futures-util",
  "log",
  "tokio",
  "tungstenite",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.10"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+checksum = "9cf6b47b3771c49ac75ad09a6162f53ad4b8088b76ac60e8ec1455b31a189fe1"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
- "tracing",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
+checksum = "4badfd56924ae69bcc9039335b2e017639ce3f9b001c393c1b2d1ef846ce2cbf"
 
 [[package]]
 name = "toml_edit"
 version = "0.19.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b5bb770da30e5cbfde35a2d7b9b8a2c4b8ef89548a7a6aeab5c9a576e3e7421"
 dependencies = [
@@ -2722,15 +2719,14 @@
  "futures-core",
  "futures-util",
  "pin-project",
  "pin-project-lite",
  "tokio",
  "tower-layer",
  "tower-service",
- "tracing",
 ]
 
 [[package]]
 name = "tower-layer"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
@@ -2765,38 +2761,32 @@
 name = "try-lock"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
 
 [[package]]
 name = "tungstenite"
-version = "0.20.1"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e3dac10fd62eaf6617d3a904ae222845979aec67c615d1c842b4002c7666fb9"
+checksum = "9ef1a641ea34f399a848dea702823bbecfb4c486f911735368f1f137cb8257e1"
 dependencies = [
  "byteorder",
  "bytes",
  "data-encoding",
- "http 0.2.12",
+ "http 1.1.0",
  "httparse",
  "log",
  "rand",
  "sha1",
  "thiserror",
  "url",
  "utf-8",
 ]
 
 [[package]]
-name = "typed-arena"
-version = "2.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
-
-[[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "unicase"
@@ -2831,24 +2821,34 @@
 [[package]]
 name = "unicode-segmentation"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
+name = "unicode-truncate"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a5fbabedabe362c618c714dbefda9927b5afc8e2a8102f47f081089a9019226"
+dependencies = [
+ "itertools 0.12.1",
+ "unicode-width",
+]
+
+[[package]]
 name = "unicode-width"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "url"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
@@ -2879,17 +2879,17 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
@@ -2898,120 +2898,118 @@
 checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
 dependencies = [
  "try-lock",
 ]
 
 [[package]]
 name = "warp"
-version = "0.3.6"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1e92e22e03ff1230c03a1a8ee37d2f89cd489e2e541b7550d6afad96faed169"
+checksum = "4378d202ff965b011c64817db11d5829506d3404edeadb61f190d111da3f231c"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
  "headers",
  "http 0.2.12",
  "hyper 0.14.28",
  "log",
  "mime",
  "mime_guess",
  "multer",
  "percent-encoding",
  "pin-project",
- "rustls-pemfile 1.0.4",
  "scoped-tls",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "tokio",
- "tokio-stream",
  "tokio-tungstenite",
  "tokio-util",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.41"
+version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "877b9c3f61ceea0e56331985743b13f3d25c406a7098d45180fb5f09bc19ed97"
+checksum = "76bc14366121efc8dbb487ab05bcc9d346b3b5ec0eaa76e46594cabbe51762c0"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "web-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96565907687f7aceb35bc5fc03770a8a0471d82e479f25832f54a0e3f4b28446"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -3027,34 +3025,34 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.3",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -3064,15 +3062,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.3",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -3084,110 +3082,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d380ba1dc7187569a8a9e91ed34b8ccfc33123bbacb8c0aed2d1ad7f3ef2dc5f"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.3",
- "windows_aarch64_msvc 0.52.3",
- "windows_i686_gnu 0.52.3",
- "windows_i686_msvc 0.52.3",
- "windows_x86_64_gnu 0.52.3",
- "windows_x86_64_gnullvm 0.52.3",
- "windows_x86_64_msvc 0.52.3",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68e5dcfb9413f53afd9c8f86e56a7b4d86d9a2fa26090ea2dc9e40fba56c6ec6"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8dab469ebbc45798319e69eebf92308e541ce46760b49b18c6b3fe5e8965b30f"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.3"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a4e9b6a7cac734a8b4138a4e1044eac3404d8326b6c0f939276560687a033fb"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28b0ec9c422ca95ff34a78755cfa6ad4a51371da2a5ace67500cf7ca5f232c58"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "704131571ba93e89d7cd43482277d6632589b18ecf4468f591fbae0a8b101614"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42079295511643151e98d61c38c0acc444e52dd42ab456f7ccfd5152e8ecf21c"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0770833d60a970638e989b3fa9fd2bb1aaadcf88963d1659fd7d9990196ed2d6"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
 version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
@@ -3211,90 +3216,93 @@
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
 
 [[package]]
 name = "zerocopy"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.7.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
+checksum = "ced3678a2879b30306d323f4542626697a464a97c0a07c9aebf7ebca65cd4dde"
 dependencies = [
  "zeroize_derive",
 ]
 
 [[package]]
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "zip"
-version = "1.2.3"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c700ea425e148de30c29c580c1f9508b93ca57ad31c9f4e96b83c194c37a7a8f"
+checksum = "e2568cd0f20e86cd9a7349fe05178f7bd22f22724678448ae5a9bac266df2689"
 dependencies = [
  "aes",
  "arbitrary",
  "bzip2",
  "constant_time_eq",
  "crc32fast",
  "crossbeam-utils",
  "deflate64",
  "displaydoc",
  "flate2",
  "hmac",
  "indexmap",
  "lzma-rs",
+ "memchr",
  "pbkdf2",
  "rand",
  "sha1",
  "thiserror",
  "time",
  "zeroize",
  "zopfli",
  "zstd",
 ]
 
 [[package]]
 name = "zopfli"
-version = "0.8.0"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c1f48f3508a3a3f2faee01629564400bc12260f6214a056d06a3aaaa6ef0736"
+checksum = "e5019f391bac5cf252e93bbcc53d039ffd62c7bfb7c150414d61369afe57e946"
 dependencies = [
+ "bumpalo",
  "crc32fast",
+ "lockfree-object-pool",
  "log",
+ "once_cell",
  "simd-adler32",
- "typed-arena",
 ]
 
 [[package]]
 name = "zstd"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
```

### Comparing `rs1090-0.2.1/Cargo.toml` & `rs1090-0.2.2/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 members = ["crates/*", "python"]
 resolver = "2"
 
 [workspace.package]
 license = "MIT"
 edition = "2021"
 readme = "readme.md"
-version = "0.2.1"
+version = "0.2.2"
 authors = ["Xavier Olive <git@xoolive.org>"]
 
 # Config for 'cargo dist'
 [workspace.metadata.dist]
 # The preferred cargo-dist version to use in CI (Cargo.toml SemVer syntax)
 cargo-dist-version = "0.11.1"
 # CI backends to support
```

### Comparing `rs1090-0.2.1/pyproject.toml` & `rs1090-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/rs1090/__init__.py` & `rs1090-0.2.2/rs1090/__init__.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/rs1090/_rust.pyi` & `rs1090-0.2.2/rs1090/_rust.pyi`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/rs1090/stubs.py` & `rs1090-0.2.2/rs1090/stubs.py`

 * *Files identical despite different names*

### Comparing `rs1090-0.2.1/PKG-INFO` & `rs1090-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rs1090
-Version: 0.2.1
+Version: 0.2.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pandas >=2.2.0
 Requires-Dist: typing-extensions >=4.10.0
 Requires-Dist: mypy >=1.8.0 ; extra == 'dev'
 Requires-Dist: pytest >=8.0.2 ; extra == 'dev'
```

