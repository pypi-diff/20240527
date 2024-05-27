# Comparing `tmp/foxes-0.7.1.tar.gz` & `tmp/foxes-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxes-0.7.1.tar", last modified: Fri May 24 09:03:02 2024, max compression
+gzip compressed data, was "foxes-0.7.2.tar", last modified: Mon May 27 20:13:48 2024, max compression
```

## Comparing `foxes-0.7.1.tar` & `foxes-0.7.2.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.682548 foxes-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 09:02:58.000000 foxes-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40774 2024-05-24 09:02:58.000000 foxes-0.7.1/Logo_FOXES.svg
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-24 09:02:58.000000 foxes-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-24 09:03:02.682548 foxes-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-24 09:02:58.000000 foxes-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.638548 foxes-0.7.1/foxes/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.638548 foxes-0.7.1/foxes/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.638548 foxes-0.7.1/foxes/algorithms/downwind/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21652 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/downwind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.642548 foxes-0.7.1/foxes/algorithms/downwind/models/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/farm_wakes_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/init_farm_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/point_wakes_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/reorder_farm_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/set_amb_farm_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/downwind/models/set_amb_point_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.642548 foxes-0.7.1/foxes/algorithms/iterative/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/iterative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/iterative/iterative.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.642548 foxes-0.7.1/foxes/algorithms/iterative/models/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/iterative/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/iterative/models/convergence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/iterative/models/farm_wakes_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/iterative/models/urelax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.642548 foxes-0.7.1/foxes/algorithms/sequential/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/sequential/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.642548 foxes-0.7.1/foxes/algorithms/sequential/models/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/sequential/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/sequential/models/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/sequential/models/seq_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/algorithms/sequential/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.646548 foxes-0.7.1/foxes/core/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15169 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/axial_induction_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14581 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/data_calc_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/farm_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/farm_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/farm_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/partial_wakes_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/point_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/rotor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/turbine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/turbine_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/turbine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/vertical_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/wake_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/wake_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/wake_superposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/core/wind_farm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.646548 foxes-0.7.1/foxes/data/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.646548 foxes-0.7.1/foxes/data/farms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/farms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/farms/test_farm_67.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.650548 foxes-0.7.1/foxes/data/power_ct_curves/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/power_ct_curves/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.650548 foxes-0.7.1/foxes/data/states/
--rw-r--r--   0 runner    (1001) docker     (127)   427815 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/WRF-Timeseries-4464.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   126124 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/abl_states_6000.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/timeseries_100.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/timeseries_3000.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)    78694 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/timeseries_8000.csv.gz
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/wind_rose_bremen.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/wind_rotation.nc
--rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/states/winds100.tab
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/data/static_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.650548 foxes-0.7.1/foxes/input/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/input/farm_layout/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/from_df.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/from_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/from_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/farm_layout/row.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/input/states/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/input/states/create/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/create/random_abl_states.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/create/random_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)    18693 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/field_data_nc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/multi_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/scan_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/single.py
--rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/states/states_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/input/windio/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/windio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/input/windio/windio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/models/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/models/axial_induction_models/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/axial_induction_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/axial_induction_models/betz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/axial_induction_models/madsen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/models/farm_controllers/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/farm_controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/farm_controllers/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.654548 foxes-0.7.1/foxes/models/farm_models/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/farm_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/farm_models/turbine2farm.py
--rw-r--r--   0 runner    (1001) docker     (127)    26376 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/model_book.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.658548 foxes-0.7.1/foxes/models/partial_wakes/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/axiwake.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/centre.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/rotor_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/segregated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/partial_wakes/top_hat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.658548 foxes-0.7.1/foxes/models/point_models/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/point_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/point_models/set_uniform_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/point_models/tke2ti.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/point_models/wake_deltas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.658548 foxes-0.7.1/foxes/models/rotor_models/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/rotor_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/rotor_models/centre.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/rotor_models/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/rotor_models/levels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.658548 foxes-0.7.1/foxes/models/turbine_models/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/kTI_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/lookup_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/power_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/rotor_centre_calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/sector_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/set_farm_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/table_factors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/thrust2ct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/yaw2yawm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_models/yawm2yaw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.662548 foxes-0.7.1/foxes/models/turbine_types/
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/CpCt_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/CpCt_from_two.py
--rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/PCt_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/PCt_from_two.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/null_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/wsrho2PCt_from_two.py
--rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/turbine_types/wsti2PCt_from_two.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.662548 foxes-0.7.1/foxes/models/vertical_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/abl_log_neutral_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/abl_log_stable_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/abl_log_unstable_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/abl_log_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/data_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/sheared_ws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/vertical_profiles/uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.662548 foxes-0.7.1/foxes/models/wake_frames/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/farm_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/rotor_wd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/seq_dynamic_wakes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/timelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_frames/yawed_wakes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.666548 foxes-0.7.1/foxes/models/wake_models/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/axisymmetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/dist_sliced.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.666548 foxes-0.7.1/foxes/models/wake_models/induction/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/induction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/induction/rankine_half_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/induction/rathmann.py
--rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/induction/self_similar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/induction/self_similar2020.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.666548 foxes-0.7.1/foxes/models/wake_models/ti/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/ti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/ti/crespo_hernandez.py
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/ti/iec_ti.py
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/top_hat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/wake_mirror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.666548 foxes-0.7.1/foxes/models/wake_models/wind/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/wind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/wind/bastankhah14.py
--rw-r--r--   0 runner    (1001) docker     (127)    17629 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/wind/bastankhah16.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/wind/jensen.py
--rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_models/wind/turbopark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.666548 foxes-0.7.1/foxes/models/wake_superpositions/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ti_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ti_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ti_pow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ti_quadratic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ws_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     9380 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ws_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ws_pow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ws_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/models/wake_superpositions/ws_quadratic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.670548 foxes-0.7.1/foxes/opt/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.670548 foxes-0.7.1/foxes/opt/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/constraints/area_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/constraints/min_dist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.670548 foxes-0.7.1/foxes/opt/core/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/core/farm_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/core/farm_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/core/farm_opt_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/core/farm_vars_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/core/pop_states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.670548 foxes-0.7.1/foxes/opt/objectives/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/objectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/objectives/farm_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/objectives/max_n_turbines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.670548 foxes-0.7.1/foxes/opt/problems/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.670548 foxes-0.7.1/foxes/opt/problems/layout/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/farm_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.674548 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
--rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/reggrids_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/layout/regular_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    19425 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/opt/problems/opt_farm_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.674548 foxes-0.7.1/foxes/output/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/calc_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/farm_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    17663 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/farm_results_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.674548 foxes-0.7.1/foxes/output/flow_plots_2d/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/flow_plots_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/flow_plots_2d/flow_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/flow_plots_2d/get_fig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/flow_plots_2d/seq_flow_ani_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/flow_plots_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/results_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/rose_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/rotor_point_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/round.py
--rw-r--r--   0 runner    (1001) docker     (127)    31519 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/slice_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/state_turbine_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/output/turbine_type_curves.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.678548 foxes-0.7.1/foxes/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.678548 foxes-0.7.1/foxes/utils/abl/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/abl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/abl/neutral.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/abl/sheared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/abl/stable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/abl/unstable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/cubic_roots.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/data_book.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/exec_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.682548 foxes-0.7.1/foxes/utils/geom2d/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19120 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/area_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/example_intersection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/example_union.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/half_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geom2d/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geopandas_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/geopandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/pandas_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/random_xy.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/regularize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.682548 foxes-0.7.1/foxes/utils/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/runners/runners.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/subclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/tab_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/two_circles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/wind_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/windrose_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/utils/xarray_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-24 09:02:58.000000 foxes-0.7.1/foxes/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:02.682548 foxes-0.7.1/foxes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-24 09:03:02.000000 foxes-0.7.1/foxes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-05-24 09:03:02.000000 foxes-0.7.1/foxes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:03:02.000000 foxes-0.7.1/foxes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-24 09:03:02.000000 foxes-0.7.1/foxes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 09:03:02.000000 foxes-0.7.1/foxes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:03:02.000000 foxes-0.7.1/foxes.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-24 09:02:58.000000 foxes-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-24 09:03:02.682548 foxes-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 09:02:58.000000 foxes-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.735039 foxes-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-27 20:13:44.000000 foxes-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40774 2024-05-27 20:13:44.000000 foxes-0.7.2/Logo_FOXES.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-27 20:13:44.000000 foxes-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-27 20:13:48.731039 foxes-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-27 20:13:44.000000 foxes-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.687039 foxes-0.7.2/foxes/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.687039 foxes-0.7.2/foxes/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.687039 foxes-0.7.2/foxes/algorithms/downwind/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/downwind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21690 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/downwind/downwind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.687039 foxes-0.7.2/foxes/algorithms/downwind/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/downwind/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/downwind/models/farm_wakes_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/downwind/models/init_farm_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/downwind/models/point_wakes_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/downwind/models/reorder_farm_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/downwind/models/set_amb_farm_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/downwind/models/set_amb_point_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.691039 foxes-0.7.2/foxes/algorithms/iterative/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/iterative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/iterative/iterative.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.691039 foxes-0.7.2/foxes/algorithms/iterative/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/iterative/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/iterative/models/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/iterative/models/farm_wakes_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/iterative/models/urelax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.691039 foxes-0.7.2/foxes/algorithms/sequential/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/sequential/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.691039 foxes-0.7.2/foxes/algorithms/sequential/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/sequential/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/sequential/models/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/sequential/models/seq_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/algorithms/sequential/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.695039 foxes-0.7.2/foxes/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15169 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/axial_induction_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14581 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/data_calc_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/farm_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/farm_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/farm_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/partial_wakes_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/point_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/rotor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/turbine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/turbine_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/turbine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/vertical_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/wake_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/wake_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/wake_superposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/core/wind_farm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.695039 foxes-0.7.2/foxes/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.695039 foxes-0.7.2/foxes/data/farms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/farms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/farms/test_farm_67.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.695039 foxes-0.7.2/foxes/data/power_ct_curves/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/power_ct_curves/DTU-10MW-D178d3-H119.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/power_ct_curves/IEA-15MW-D240-H150.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/power_ct_curves/NREL-5MW-D126-H90.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/power_ct_curves/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.699039 foxes-0.7.2/foxes/data/states/
+-rw-r--r--   0 runner    (1001) docker     (127)   427815 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/states/WRF-Timeseries-4464.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126124 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/states/abl_states_6000.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/states/timeseries_100.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/states/timeseries_3000.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    78694 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/states/timeseries_8000.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/states/wind_rose_bremen.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/states/wind_rotation.nc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3061 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/states/winds100.tab
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/data/static_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.699039 foxes-0.7.2/foxes/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.699039 foxes-0.7.2/foxes/input/farm_layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/farm_layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/farm_layout/from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/farm_layout/from_df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/farm_layout/from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/farm_layout/from_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/farm_layout/from_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/farm_layout/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/farm_layout/row.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.699039 foxes-0.7.2/foxes/input/states/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.703039 foxes-0.7.2/foxes/input/states/create/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/states/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/states/create/random_abl_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/states/create/random_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18693 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/states/field_data_nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/states/multi_height.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/states/scan_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/states/single.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/states/states_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.703039 foxes-0.7.2/foxes/input/windio/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/windio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/input/windio/windio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.703039 foxes-0.7.2/foxes/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.703039 foxes-0.7.2/foxes/models/axial_induction/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/axial_induction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/axial_induction/betz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/axial_induction/madsen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.703039 foxes-0.7.2/foxes/models/farm_controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/farm_controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/farm_controllers/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.703039 foxes-0.7.2/foxes/models/farm_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/farm_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/farm_models/turbine2farm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26786 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/model_book.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.703039 foxes-0.7.2/foxes/models/partial_wakes/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/partial_wakes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/partial_wakes/axiwake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/partial_wakes/centre.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/partial_wakes/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/partial_wakes/rotor_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/partial_wakes/segregated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/partial_wakes/top_hat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.707039 foxes-0.7.2/foxes/models/point_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/point_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/point_models/set_uniform_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/point_models/tke2ti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/point_models/wake_deltas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.707039 foxes-0.7.2/foxes/models/rotor_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/rotor_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/rotor_models/centre.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/rotor_models/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/rotor_models/levels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.707039 foxes-0.7.2/foxes/models/turbine_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_models/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_models/kTI_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_models/lookup_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_models/power_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_models/rotor_centre_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_models/sector_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_models/set_farm_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_models/table_factors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_models/thrust2ct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_models/yaw2yawm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_models/yawm2yaw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.711039 foxes-0.7.2/foxes/models/turbine_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_types/CpCt_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_types/CpCt_from_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_types/PCt_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_types/PCt_from_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_types/null_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11143 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_types/wsrho2PCt_from_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/turbine_types/wsti2PCt_from_two.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.711039 foxes-0.7.2/foxes/models/vertical_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/vertical_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/vertical_profiles/abl_log_neutral_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/vertical_profiles/abl_log_stable_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/vertical_profiles/abl_log_unstable_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/vertical_profiles/abl_log_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/vertical_profiles/data_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/vertical_profiles/sheared_ws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/vertical_profiles/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.711039 foxes-0.7.2/foxes/models/wake_frames/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_frames/farm_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_frames/rotor_wd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_frames/seq_dynamic_wakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_frames/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_frames/timelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_frames/yawed_wakes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.711039 foxes-0.7.2/foxes/models/wake_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/axisymmetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/dist_sliced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.715039 foxes-0.7.2/foxes/models/wake_models/induction/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/induction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/induction/rankine_half_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/induction/rathmann.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/induction/self_similar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/induction/self_similar2020.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.715039 foxes-0.7.2/foxes/models/wake_models/ti/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/ti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/ti/crespo_hernandez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/ti/iec_ti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/top_hat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/wake_mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.715039 foxes-0.7.2/foxes/models/wake_models/wind/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/wind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/wind/bastankhah14.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17629 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/wind/bastankhah16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/wind/jensen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15250 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_models/wind/turbopark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.715039 foxes-0.7.2/foxes/models/wake_superpositions/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_superpositions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_superpositions/ti_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_superpositions/ti_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_superpositions/ti_pow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_superpositions/ti_quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_superpositions/ws_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_superpositions/ws_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9602 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_superpositions/ws_pow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_superpositions/ws_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/models/wake_superpositions/ws_quadratic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.719039 foxes-0.7.2/foxes/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.719039 foxes-0.7.2/foxes/opt/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/constraints/area_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/constraints/min_dist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.719039 foxes-0.7.2/foxes/opt/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/core/farm_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/core/farm_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/core/farm_opt_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/core/farm_vars_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/core/pop_states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.719039 foxes-0.7.2/foxes/opt/objectives/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/objectives/farm_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/objectives/max_n_turbines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.719039 foxes-0.7.2/foxes/opt/problems/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.719039 foxes-0.7.2/foxes/opt/problems/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/layout/farm_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.723039 foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/geom_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14222 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17834 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/layout/reggrids_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/layout/regular_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19425 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/opt/problems/opt_farm_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.723039 foxes-0.7.2/foxes/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/calc_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10981 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/farm_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17663 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/farm_results_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.723039 foxes-0.7.2/foxes/output/flow_plots_2d/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/flow_plots_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/flow_plots_2d/flow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/flow_plots_2d/get_fig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/flow_plots_2d/seq_flow_ani_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/flow_plots_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/results_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/rose_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/rotor_point_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/round.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31519 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/slice_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/state_turbine_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/output/turbine_type_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.727039 foxes-0.7.2/foxes/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.731039 foxes-0.7.2/foxes/utils/abl/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/abl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/abl/neutral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/abl/sheared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/abl/stable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/abl/unstable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/cubic_roots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/data_book.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/exec_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.731039 foxes-0.7.2/foxes/utils/geom2d/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/geom2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19120 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/geom2d/area_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/geom2d/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/geom2d/example_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/geom2d/example_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/geom2d/half_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/geom2d/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/geopandas_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/geopandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/pandas_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/random_xy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/regularize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.731039 foxes-0.7.2/foxes/utils/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/runners/runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/tab_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/two_circles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/wind_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/windrose_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/utils/xarray_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-27 20:13:44.000000 foxes-0.7.2/foxes/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:13:48.731039 foxes-0.7.2/foxes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-27 20:13:48.000000 foxes-0.7.2/foxes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9575 2024-05-27 20:13:48.000000 foxes-0.7.2/foxes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:13:48.000000 foxes-0.7.2/foxes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-27 20:13:48.000000 foxes-0.7.2/foxes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 20:13:48.000000 foxes-0.7.2/foxes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:13:48.000000 foxes-0.7.2/foxes.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-27 20:13:44.000000 foxes-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-27 20:13:48.735039 foxes-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 20:13:44.000000 foxes-0.7.2/setup.py
```

### Comparing `foxes-0.7.1/LICENSE` & `foxes-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/Logo_FOXES.svg` & `foxes-0.7.2/Logo_FOXES.svg`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/PKG-INFO` & `foxes-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.7.1
+Version: 0.7.2
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
```

### Comparing `foxes-0.7.1/README.md` & `foxes-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/__init__.py` & `foxes-0.7.2/foxes/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/downwind/downwind.py` & `foxes-0.7.2/foxes/algorithms/downwind/downwind.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,17 @@
             for i, (w, p) in enumerate(self.partial_wakes.items()):
                 print(f"    {i}) {w}: {p.name}, {p}")
             print(deco)
             print(f"  turbine models:")
             for i, m in enumerate(self.farm_controller.pre_rotor_models.models):
                 print(f"    {i}) {m.name}: {m} [pre-rotor]")
             for i, m in enumerate(self.farm_controller.post_rotor_models.models):
-                print(f"    {i+len(self.farm_controller.pre_rotor_models.models)}) {m.name}: {m}")
+                print(
+                    f"    {i+len(self.farm_controller.pre_rotor_models.models)}) {m.name}: {m}"
+                )
             print(deco)
             print()
 
     def _print_model_oder(self, mlist, calc_pars):
         """
         Helper function for printing model names
         """
```

### Comparing `foxes-0.7.1/foxes/algorithms/downwind/models/farm_wakes_calc.py` & `foxes-0.7.2/foxes/algorithms/downwind/models/farm_wakes_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/downwind/models/init_farm_data.py` & `foxes-0.7.2/foxes/algorithms/downwind/models/init_farm_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/downwind/models/point_wakes_calc.py` & `foxes-0.7.2/foxes/algorithms/downwind/models/point_wakes_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/downwind/models/reorder_farm_output.py` & `foxes-0.7.2/foxes/algorithms/downwind/models/reorder_farm_output.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/downwind/models/set_amb_farm_results.py` & `foxes-0.7.2/foxes/algorithms/downwind/models/set_amb_farm_results.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/downwind/models/set_amb_point_results.py` & `foxes-0.7.2/foxes/algorithms/downwind/models/set_amb_point_results.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/iterative/iterative.py` & `foxes-0.7.2/foxes/algorithms/iterative/iterative.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/iterative/models/convergence.py` & `foxes-0.7.2/foxes/algorithms/iterative/models/convergence.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/iterative/models/farm_wakes_calc.py` & `foxes-0.7.2/foxes/algorithms/iterative/models/farm_wakes_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/iterative/models/urelax.py` & `foxes-0.7.2/foxes/algorithms/iterative/models/urelax.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/sequential/models/plugin.py` & `foxes-0.7.2/foxes/algorithms/sequential/models/plugin.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/sequential/models/seq_state.py` & `foxes-0.7.2/foxes/algorithms/sequential/models/seq_state.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/algorithms/sequential/sequential.py` & `foxes-0.7.2/foxes/algorithms/sequential/sequential.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/constants.py` & `foxes-0.7.2/foxes/constants.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/__init__.py` & `foxes-0.7.2/foxes/core/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/algorithm.py` & `foxes-0.7.2/foxes/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/data.py` & `foxes-0.7.2/foxes/core/data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/data_calc_model.py` & `foxes-0.7.2/foxes/core/data_calc_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/farm_controller.py` & `foxes-0.7.2/foxes/core/farm_controller.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/farm_data_model.py` & `foxes-0.7.2/foxes/core/farm_data_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/model.py` & `foxes-0.7.2/foxes/core/model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/partial_wakes_model.py` & `foxes-0.7.2/foxes/core/partial_wakes_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/point_data_model.py` & `foxes-0.7.2/foxes/core/point_data_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/rotor_model.py` & `foxes-0.7.2/foxes/core/rotor_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/states.py` & `foxes-0.7.2/foxes/core/states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/turbine.py` & `foxes-0.7.2/foxes/core/turbine.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/turbine_model.py` & `foxes-0.7.2/foxes/core/turbine_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/turbine_type.py` & `foxes-0.7.2/foxes/core/turbine_type.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/vertical_profile.py` & `foxes-0.7.2/foxes/core/vertical_profile.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/wake_frame.py` & `foxes-0.7.2/foxes/core/wake_frame.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/wake_model.py` & `foxes-0.7.2/foxes/core/wake_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/wake_superposition.py` & `foxes-0.7.2/foxes/core/wake_superposition.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/core/wind_farm.py` & `foxes-0.7.2/foxes/core/wind_farm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/data/farms/test_farm_67.csv` & `foxes-0.7.2/foxes/data/farms/test_farm_67.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/data/parse.py` & `foxes-0.7.2/foxes/data/parse.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv` & `foxes-0.7.2/foxes/data/power_ct_curves/IWT-7d5MW-D164-H100.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/data/states/WRF-Timeseries-4464.csv.gz` & `foxes-0.7.2/foxes/data/states/WRF-Timeseries-4464.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/data/states/abl_states_6000.csv.gz` & `foxes-0.7.2/foxes/data/states/abl_states_6000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/data/states/timeseries_3000.csv.gz` & `foxes-0.7.2/foxes/data/states/timeseries_3000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/data/states/timeseries_8000.csv.gz` & `foxes-0.7.2/foxes/data/states/timeseries_8000.csv.gz`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/data/states/wind_rose_bremen.csv` & `foxes-0.7.2/foxes/data/states/wind_rose_bremen.csv`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/data/states/wind_rotation.nc` & `foxes-0.7.2/foxes/data/states/wind_rotation.nc`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/data/states/winds100.tab` & `foxes-0.7.2/foxes/data/states/winds100.tab`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/data/static_data.py` & `foxes-0.7.2/foxes/data/static_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/farm_layout/from_csv.py` & `foxes-0.7.2/foxes/input/farm_layout/from_csv.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/farm_layout/from_df.py` & `foxes-0.7.2/foxes/input/farm_layout/from_df.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/farm_layout/from_file.py` & `foxes-0.7.2/foxes/input/farm_layout/from_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/farm_layout/from_json.py` & `foxes-0.7.2/foxes/input/farm_layout/from_json.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/farm_layout/from_random.py` & `foxes-0.7.2/foxes/input/farm_layout/from_random.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/farm_layout/grid.py` & `foxes-0.7.2/foxes/input/farm_layout/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/farm_layout/row.py` & `foxes-0.7.2/foxes/input/farm_layout/row.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/states/create/random_abl_states.py` & `foxes-0.7.2/foxes/input/states/create/random_abl_states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/states/create/random_timeseries.py` & `foxes-0.7.2/foxes/input/states/create/random_timeseries.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/states/field_data_nc.py` & `foxes-0.7.2/foxes/input/states/field_data_nc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/states/multi_height.py` & `foxes-0.7.2/foxes/input/states/multi_height.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/states/scan_ws.py` & `foxes-0.7.2/foxes/input/states/scan_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/states/single.py` & `foxes-0.7.2/foxes/input/states/single.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/states/states_table.py` & `foxes-0.7.2/foxes/input/states/states_table.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/input/windio/windio.py` & `foxes-0.7.2/foxes/input/windio/windio.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/axial_induction_models/betz.py` & `foxes-0.7.2/foxes/models/axial_induction/betz.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/axial_induction_models/madsen.py` & `foxes-0.7.2/foxes/models/axial_induction/madsen.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/farm_models/turbine2farm.py` & `foxes-0.7.2/foxes/models/farm_models/turbine2farm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/model_book.py` & `foxes-0.7.2/foxes/models/model_book.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from math import sqrt
 import foxes.models as fm
 import foxes.variables as FV
-from foxes.utils import Dict, FDict
+from foxes.utils import FDict
 
 from foxes.core import (
     PointDataModel,
     FarmDataModel,
     FarmController,
     RotorModel,
     TurbineType,
@@ -21,50 +21,50 @@
 
 class ModelBook:
     """
     Container for all kinds of models.
 
     Attributes
     ----------
-    point_models: foxes.utils.Dict
+    point_models: foxes.utils.FDict
         The point models. Keys: model name str,
         values: foxes.core.PointDataModel
-    rotor_models: foxes.utils.Dict
+    rotor_models: foxes.utils.FDict
         The rotor models. Keys: model name str,
         values: foxes.core.RotorModel
-    turbine_types: foxes.utils.Dict
+    turbine_types: foxes.utils.FDict
         The turbine type models. Keys: model name str,
         values: foxes.core.TurbineType
-    turbine_models: foxes.utils.Dict
+    turbine_models: foxes.utils.FDict
         The turbine models. Keys: model name str,
         values: foxes.core.TurbineModel
-    farm_models: foxes.utils.Dict
+    farm_models: foxes.utils.FDict
         The farm models. Keys: model name str,
         values: foxes.core.FarmModel
-    farm_controllers: foxes.utils.Dict
+    farm_controllers: foxes.utils.FDict
         The farm controllers. Keys: model name str,
         values: foxes.core.FarmController
-    partial_wakes: foxes.utils.Dict
+    partial_wakes: foxes.utils.FDict
         The partial wakes. Keys: model name str,
         values: foxes.core.PartialWakeModel
-    wake_frames: foxes.utils.Dict
+    wake_frames: foxes.utils.FDict
         The wake frames. Keys: model name str,
         values: foxes.core.WakeFrame
-    wake_superpositions: foxes.utils.Dict
+    wake_superpositions: foxes.utils.FDict
         The wake superposition models. Keys: model name str,
         values: foxes.core.WakeSuperposition
-    wake_models: foxes.utils.Dict
+    wake_models: foxes.utils.FDict
         The wake models. Keys: model name str,
         values: foxes.core.WakeModel
-    induction_models: foxes.utils.Dict
+    induction_models: foxes.utils.FDict
         The induction models. Keys: model name str,
         values: foxes.core.AxialInductionModel
-    sources: foxes.utils.Dict
+    sources: foxes.utils.FDict
         All sources dict
-    base_classes: foxes.utils.Dict
+    base_classes: foxes.utils.FDict
         The base classes for all model types
 
     :group: models
 
     """
 
     def __init__(self, Pct_file=None):
@@ -73,59 +73,62 @@
 
         Parameters
         ----------
         Pct_file: str, optional
             Path to power/ct curve file, for creation
             of default turbine type model
         """
-        self.point_models = Dict(name="point_models")
+        self.point_models = FDict(name="point_models")
         self.point_models["tke2ti"] = fm.point_models.TKE2TI()
 
         self.rotor_models = FDict(name="rotor_models")
         rvars = [FV.REWS, FV.REWS2, FV.REWS3, FV.TI, FV.RHO]
         self.rotor_models["centre"] = fm.rotor_models.CentreRotor(calc_vars=rvars)
 
         def _n2n(n2):
             n2 = float(n2)
             n = int(sqrt(n2))
             if n**2 != n2:
-                raise Exception(f"GridRotor factory: Value {n2} is not the square of an integer")
+                raise Exception(
+                    f"GridRotor factory: Value {n2} is not the square of an integer"
+                )
             return n
+
         self.rotor_models.add_factory(
             fm.rotor_models.GridRotor,
             "grid<n2>",
             kwargs=dict(calc_vars=rvars, reduce=True),
             var2arg={"n2": "n"},
             n2=_n2n,
             hints={"n2": "(Number of points in square grid)"},
         )
         self.rotor_models.add_factory(
             fm.rotor_models.GridRotor,
-            "raw_grid<n2>",
+            "grid<n2>_raw",
             kwargs=dict(calc_vars=rvars, reduce=False),
             var2arg={"n2": "n"},
             n2=_n2n,
             hints={"n2": "(Number of points in square grid)"},
         )
         self.rotor_models.add_factory(
             fm.rotor_models.LevelRotor,
             "level<n>",
             kwargs=dict(calc_vars=rvars, reduce=True),
             n=lambda x: int(x),
             hints={"n": "(Number of vertical levels)"},
         )
         self.rotor_models.add_factory(
             fm.rotor_models.LevelRotor,
-            "raw_level<n>",
+            "level<n>_raw",
             kwargs=dict(calc_vars=rvars, reduce=False),
             n=lambda x: int(x),
             hints={"n": "(Number of vertical levels)"},
         )
 
-        self.turbine_types = Dict(name="turbine_types")
+        self.turbine_types = FDict(name="turbine_types")
         self.turbine_types["null_type"] = fm.turbine_types.NullType()
         self.turbine_types["NREL5MW"] = fm.turbine_types.PCtFile(
             "NREL-5MW-D126-H90.csv", rho=1.225
         )
         self.turbine_types["DTU10MW"] = fm.turbine_types.PCtFile(
             "DTU-10MW-D178d3-H119.csv", rho=1.225
         )
@@ -161,45 +164,49 @@
             hints={"kTI": "(Value, e.g. 004 for 0.04)"},
         )
         self.turbine_models.add_factory(
             fm.turbine_models.kTI,
             "kTI_<kTI>_<kb>",
             kTI=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
             kb=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
-            hints={"kTI": "(Value, e.g. 004 for 0.04)",
-                   "kb": "(Value, e.g. 004 for 0.04)"},
+            hints={
+                "kTI": "(Value, e.g. 004 for 0.04)",
+                "kb": "(Value, e.g. 004 for 0.04)",
+            },
         )
         self.turbine_models.add_factory(
             fm.turbine_models.kTI,
             "kTI_amb_<kTI>_<kb>",
             kwargs=dict(ti_var=FV.AMB_TI),
             kTI=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
             kb=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
-            hints={"kTI": "(Value, e.g. 004 for 0.04)",
-                   "kb": "(Value, e.g. 004 for 0.04)"},
+            hints={
+                "kTI": "(Value, e.g. 004 for 0.04)",
+                "kb": "(Value, e.g. 004 for 0.04)",
+            },
         )
 
         self.turbine_models["hubh_data"] = fm.turbine_models.RotorCentreCalc(
             {
                 f"{FV.WD}_HH": FV.WD,
                 f"{FV.WS}_HH": FV.WS,
                 f"{FV.TI}_HH": FV.TI,
                 f"{FV.RHO}_HH": FV.RHO,
             }
         )
 
-        self.farm_models = Dict(
+        self.farm_models = FDict(
             name="farm_models",
             **{
                 f"farm_{mname}": fm.farm_models.Turbine2FarmModel(m)
                 for mname, m in self.turbine_models.items()
             },
         )
 
-        self.farm_controllers = Dict(
+        self.farm_controllers = FDict(
             name="farm_controllers",
             basic_ctrl=fm.farm_controllers.BasicFarmController(),
         )
 
         self.partial_wakes = FDict(
             name="partial_wakes",
             rotor_points=fm.partial_wakes.RotorPoints(),
@@ -242,19 +249,21 @@
             fm.wake_frames.Streamlines2D,
             "streamlines_<step>",
             step=lambda x: float(x),
             hints={"step": "(Step size in m)"},
         )
 
         self.wake_frames["timelines"] = fm.wake_frames.Timelines()
+
         def _todt(x):
             if x[-1] == "s":
-                return float(x[:-1])/60
+                return float(x[:-1]) / 60
             elif x[-3:] == "min":
                 return float(x[:-3])
+
         self.wake_frames.add_factory(
             fm.wake_frames.Timelines,
             "timelines_<dt>",
             dt=_todt,
             var2arg={"dt": "dt_min"},
             hints={"dt": "(Time step, e.g '10s', '1min' etc.)"},
         )
@@ -262,15 +271,15 @@
             fm.wake_frames.SeqDynamicWakes,
             "seq_dyn_wakes_<dt>",
             dt=_todt,
             var2arg={"dt": "dt_min"},
             hints={"dt": "(Time step, e.g '10s', '1min' etc.)"},
         )
 
-        self.wake_superpositions = Dict(
+        self.wake_superpositions = FDict(
             name="wake_superpositions",
             ws_linear=fm.wake_superpositions.WSLinear(scale_amb=False),
             ws_linear_lim=fm.wake_superpositions.WSLinear(
                 scale_amb=False, lim_low=1e-4
             ),
             ws_linear_amb=fm.wake_superpositions.WSLinear(scale_amb=True),
             ws_linear_amb_lim=fm.wake_superpositions.WSLinear(
@@ -305,35 +314,35 @@
             ti_linear=fm.wake_superpositions.TILinear(superp_to_amb="quadratic"),
             ti_quadratic=fm.wake_superpositions.TIQuadratic(superp_to_amb="quadratic"),
             ti_cubic=fm.wake_superpositions.TIPow(pow=3, superp_to_amb="quadratic"),
             ti_quartic=fm.wake_superpositions.TIPow(pow=4, superp_to_amb="quadratic"),
             ti_max=fm.wake_superpositions.TIMax(superp_to_amb="quadratic"),
         )
 
-        self.axial_induction = Dict(name="induction_models")
-        self.axial_induction["Betz"] = fm.axial_induction_models.BetzAxialInduction()
-        self.axial_induction["Madsen"] = (
-            fm.axial_induction_models.MadsenAxialInduction()
-        )
+        self.axial_induction = FDict(name="induction_models")
+        self.axial_induction["Betz"] = fm.axial_induction.BetzAxialInduction()
+        self.axial_induction["Madsen"] = fm.axial_induction.MadsenAxialInduction()
 
         self.wake_models = FDict(name="wake_models")
 
         self.wake_models.add_factory(
             fm.wake_models.wind.JensenWake,
             "Jensen_<superposition>",
             superposition=lambda s: f"ws_{s}",
             hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.JensenWake,
             "Jensen_<superposition>_k<k>",
             superposition=lambda s: f"ws_{s}",
             k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
-            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
-                   "k": "(Value, e.g. 004 for 0.04)"},
+            hints={
+                "superposition": "(Superposition, e.g. linear for ws_linear)",
+                "k": "(Value, e.g. 004 for 0.04)",
+            },
         )
 
         self.wake_models.add_factory(
             fm.wake_models.wind.Bastankhah2014,
             "Bastankhah2014_<superposition>",
             kwargs=dict(sbeta_factor=0.2),
             superposition=lambda s: f"ws_{s}",
@@ -341,146 +350,166 @@
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.Bastankhah2014,
             "Bastankhah2014_<superposition>_k<k>",
             kwargs=dict(sbeta_factor=0.2),
             superposition=lambda s: f"ws_{s}",
             k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
-            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
-                   "k": "(Value, e.g. 004 for 0.04)"},
+            hints={
+                "superposition": "(Superposition, e.g. linear for ws_linear)",
+                "k": "(Value, e.g. 004 for 0.04)",
+            },
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.Bastankhah2014,
             "Bastankhah2014B_<superposition>",
             kwargs=dict(sbeta_factor=0.2, induction="Betz"),
             superposition=lambda s: f"ws_{s}",
             hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.Bastankhah2014,
             "Bastankhah2014B_<superposition>_k<k>",
             kwargs=dict(sbeta_factor=0.2, induction="Betz"),
             superposition=lambda s: f"ws_{s}",
             k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
-            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
-                   "k": "(Value, e.g. 004 for 0.04)"},
+            hints={
+                "superposition": "(Superposition, e.g. linear for ws_linear)",
+                "k": "(Value, e.g. 004 for 0.04)",
+            },
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.Bastankhah2014,
             "Bastankhah025_<superposition>",
             kwargs=dict(sbeta_factor=0.25),
             superposition=lambda s: f"ws_{s}",
             hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.Bastankhah2014,
             "Bastankhah025_<superposition>_k<k>",
             kwargs=dict(sbeta_factor=0.25),
             superposition=lambda s: f"ws_{s}",
             k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
-            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
-                   "k": "(Value, e.g. 004 for 0.04)"},
+            hints={
+                "superposition": "(Superposition, e.g. linear for ws_linear)",
+                "k": "(Value, e.g. 004 for 0.04)",
+            },
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.Bastankhah2014,
             "Bastankhah025B_<superposition>",
             kwargs=dict(sbeta_factor=0.25, induction="Betz"),
             superposition=lambda s: f"ws_{s}",
             hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.Bastankhah2014,
             "Bastankhah025B_<superposition>_k<k>",
             kwargs=dict(sbeta_factor=0.25, induction="Betz"),
             superposition=lambda s: f"ws_{s}",
             k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
-            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
-                   "k": "(Value, e.g. 004 for 0.04)"},
+            hints={
+                "superposition": "(Superposition, e.g. linear for ws_linear)",
+                "k": "(Value, e.g. 004 for 0.04)",
+            },
         )
 
         self.wake_models.add_factory(
             fm.wake_models.wind.Bastankhah2016,
             "Bastankhah2016_<superposition>",
             superposition=lambda s: f"ws_{s}",
             hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.Bastankhah2016,
             "Bastankhah2016_<superposition>_k<k>",
             superposition=lambda s: f"ws_{s}",
             k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
-            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
-                   "k": "(Value, e.g. 004 for 0.04)"},
+            hints={
+                "superposition": "(Superposition, e.g. linear for ws_linear)",
+                "k": "(Value, e.g. 004 for 0.04)",
+            },
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.Bastankhah2016,
             "Bastankhah2016B_<superposition>",
             kwargs=dict(induction="Betz"),
             superposition=lambda s: f"ws_{s}",
             hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.Bastankhah2016,
             "Bastankhah2016B_<superposition>_k<k>",
             kwargs=dict(induction="Betz"),
             superposition=lambda s: f"ws_{s}",
             k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
-            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
-                   "k": "(Value, e.g. 004 for 0.04)"},
+            hints={
+                "superposition": "(Superposition, e.g. linear for ws_linear)",
+                "k": "(Value, e.g. 004 for 0.04)",
+            },
         )
 
         self.wake_models.add_factory(
             fm.wake_models.wind.TurbOParkWake,
             "TurbOPark_<superposition>",
             superposition=lambda s: f"ws_{s}",
             hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.TurbOParkWake,
             "TurbOPark_<superposition>_k<k>",
             superposition=lambda s: f"ws_{s}",
             k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
-            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
-                   "k": "(Value, e.g. 004 for 0.04)"},
+            hints={
+                "superposition": "(Superposition, e.g. linear for ws_linear)",
+                "k": "(Value, e.g. 004 for 0.04)",
+            },
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.TurbOParkWake,
             "TurbOParkB_<superposition>",
             kwargs=dict(induction="Betz"),
             superposition=lambda s: f"ws_{s}",
             hints={"superposition": "(Superposition, e.g. linear for ws_linear)"},
         )
         self.wake_models.add_factory(
             fm.wake_models.wind.TurbOParkWake,
             "TurbOParkB_<superposition>_k<k>",
             kwargs=dict(induction="Betz"),
             superposition=lambda s: f"ws_{s}",
             k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
-            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
-                   "k": "(Value, e.g. 004 for 0.04)"},
+            hints={
+                "superposition": "(Superposition, e.g. linear for ws_linear)",
+                "k": "(Value, e.g. 004 for 0.04)",
+            },
         )
 
         self.wake_models.add_factory(
             fm.wake_models.wind.TurbOParkWakeIX,
             "TurbOParkIX_<superposition>_dx<dx>",
             superposition=lambda s: f"ws_{s}",
             dx=lambda x: float(x),
-            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
-                   "dx": "(Integration step in m)"},
+            hints={
+                "superposition": "(Superposition, e.g. linear for ws_linear)",
+                "dx": "(Integration step in m)",
+            },
         )
 
         self.wake_models.add_factory(
             fm.wake_models.wind.TurbOParkWakeIX,
             "TurbOParkIX_<superposition>_k<k>_dx<dx>",
             superposition=lambda s: f"ws_{s}",
             k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
             dx=lambda x: float(x),
-            hints={"superposition": "(Superposition, e.g. linear for ws_linear)",
-                   "k": "(Value, e.g. 004 for 0.04)",
-                   "dx": "(Integration step in m)"},
+            hints={
+                "superposition": "(Superposition, e.g. linear for ws_linear)",
+                "k": "(Value, e.g. 004 for 0.04)",
+                "dx": "(Integration step in m)",
+            },
         )
 
         self.wake_models.add_factory(
             fm.wake_models.ti.CrespoHernandezTIWake,
             "CrespoHernandez_<superposition>",
             kwargs=dict(use_ambti=False),
             superposition=lambda s: f"ti_{s}",
@@ -489,16 +518,18 @@
 
         self.wake_models.add_factory(
             fm.wake_models.ti.CrespoHernandezTIWake,
             "CrespoHernandez_<superposition>_k<k>",
             kwargs=dict(use_ambti=False),
             superposition=lambda s: f"ti_{s}",
             k=lambda x: float(f"0.{x[1:]}" if x[0] == "0" else float(x)),
-            hints={"superposition": "(Superposition, e.g. linear for ti_linear)",
-                   "k": "(Value, e.g. 004 for 0.04)"},
+            hints={
+                "superposition": "(Superposition, e.g. linear for ti_linear)",
+                "k": "(Value, e.g. 004 for 0.04)",
+            },
         )
 
         self.wake_models.add_factory(
             fm.wake_models.ti.IECTIWake,
             "IECTI2005_<superposition>",
             kwargs=dict(iec_type="2005"),
             superposition=lambda s: f"ti_{s}",
@@ -516,29 +547,29 @@
         self.wake_models[f"RHB"] = fm.wake_models.induction.RankineHalfBody()
         self.wake_models[f"Rathmann"] = fm.wake_models.induction.Rathmann()
         self.wake_models[f"SelfSimilar"] = fm.wake_models.induction.SelfSimilar()
         self.wake_models[f"SelfSimilar2020"] = (
             fm.wake_models.induction.SelfSimilar2020()
         )
 
-        self.sources = Dict(
+        self.sources = FDict(
             name="sources",
             point_models=self.point_models,
             rotor_models=self.rotor_models,
             turbine_types=self.turbine_types,
             turbine_models=self.turbine_models,
             farm_models=self.farm_models,
             farm_controllers=self.farm_controllers,
             partial_wakes=self.partial_wakes,
             wake_frames=self.wake_frames,
             wake_superpositions=self.wake_superpositions,
             wake_models=self.wake_models,
             axial_induction=self.axial_induction,
         )
-        self.base_classes = Dict(
+        self.base_classes = FDict(
             name="base_classes",
             point_models=PointDataModel,
             rotor_models=RotorModel,
             turbine_types=TurbineType,
             turbine_models=TurbineModel,
             farm_models=FarmDataModel,
             farm_controllers=FarmController,
@@ -659,11 +690,11 @@
         algo: foxes.core.Algorithm
             The calculation algorithm
         verbosity: int
             The verbosity level, 0 = silent
 
         """
         for ms in self.sources.values():
-            if isinstance(ms, Dict):
+            if isinstance(ms, FDict):
                 for m in ms.values():
                     if m.initialized:
                         m.finalize(algo, verbosity)
```

### Comparing `foxes-0.7.1/foxes/models/partial_wakes/axiwake.py` & `foxes-0.7.2/foxes/models/partial_wakes/axiwake.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/partial_wakes/centre.py` & `foxes-0.7.2/foxes/models/partial_wakes/centre.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/partial_wakes/grid.py` & `foxes-0.7.2/foxes/models/partial_wakes/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/partial_wakes/rotor_points.py` & `foxes-0.7.2/foxes/models/partial_wakes/rotor_points.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/partial_wakes/segregated.py` & `foxes-0.7.2/foxes/models/partial_wakes/segregated.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/partial_wakes/top_hat.py` & `foxes-0.7.2/foxes/models/partial_wakes/top_hat.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/point_models/set_uniform_data.py` & `foxes-0.7.2/foxes/models/point_models/set_uniform_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/point_models/tke2ti.py` & `foxes-0.7.2/foxes/models/point_models/tke2ti.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/point_models/wake_deltas.py` & `foxes-0.7.2/foxes/models/point_models/wake_deltas.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/rotor_models/centre.py` & `foxes-0.7.2/foxes/models/rotor_models/centre.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/rotor_models/grid.py` & `foxes-0.7.2/foxes/models/rotor_models/grid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/rotor_models/levels.py` & `foxes-0.7.2/foxes/models/rotor_models/levels.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_models/calculator.py` & `foxes-0.7.2/foxes/models/turbine_models/calculator.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_models/kTI_model.py` & `foxes-0.7.2/foxes/models/turbine_models/kTI_model.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_models/lookup_table.py` & `foxes-0.7.2/foxes/models/turbine_models/lookup_table.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_models/power_mask.py` & `foxes-0.7.2/foxes/models/turbine_models/power_mask.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_models/rotor_centre_calc.py` & `foxes-0.7.2/foxes/models/turbine_models/rotor_centre_calc.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_models/sector_management.py` & `foxes-0.7.2/foxes/models/turbine_models/sector_management.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_models/set_farm_vars.py` & `foxes-0.7.2/foxes/models/turbine_models/set_farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_models/table_factors.py` & `foxes-0.7.2/foxes/models/turbine_models/table_factors.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_models/thrust2ct.py` & `foxes-0.7.2/foxes/models/turbine_models/thrust2ct.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_models/yaw2yawm.py` & `foxes-0.7.2/foxes/models/turbine_models/yaw2yawm.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_models/yawm2yaw.py` & `foxes-0.7.2/foxes/models/turbine_models/yawm2yaw.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_types/CpCt_file.py` & `foxes-0.7.2/foxes/models/turbine_types/CpCt_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_types/CpCt_from_two.py` & `foxes-0.7.2/foxes/models/turbine_types/CpCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_types/PCt_file.py` & `foxes-0.7.2/foxes/models/turbine_types/PCt_file.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_types/PCt_from_two.py` & `foxes-0.7.2/foxes/models/turbine_types/PCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_types/null_type.py` & `foxes-0.7.2/foxes/models/turbine_types/null_type.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_types/wsrho2PCt_from_two.py` & `foxes-0.7.2/foxes/models/turbine_types/wsrho2PCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/turbine_types/wsti2PCt_from_two.py` & `foxes-0.7.2/foxes/models/turbine_types/wsti2PCt_from_two.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/vertical_profiles/abl_log_neutral_ws.py` & `foxes-0.7.2/foxes/models/vertical_profiles/abl_log_neutral_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/vertical_profiles/abl_log_stable_ws.py` & `foxes-0.7.2/foxes/models/vertical_profiles/abl_log_stable_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/vertical_profiles/abl_log_unstable_ws.py` & `foxes-0.7.2/foxes/models/vertical_profiles/abl_log_unstable_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/vertical_profiles/abl_log_ws.py` & `foxes-0.7.2/foxes/models/vertical_profiles/abl_log_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/vertical_profiles/data_profile.py` & `foxes-0.7.2/foxes/models/vertical_profiles/data_profile.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/vertical_profiles/sheared_ws.py` & `foxes-0.7.2/foxes/models/vertical_profiles/sheared_ws.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/vertical_profiles/uniform.py` & `foxes-0.7.2/foxes/models/vertical_profiles/uniform.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_frames/farm_order.py` & `foxes-0.7.2/foxes/models/wake_frames/farm_order.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_frames/rotor_wd.py` & `foxes-0.7.2/foxes/models/wake_frames/rotor_wd.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_frames/seq_dynamic_wakes.py` & `foxes-0.7.2/foxes/models/wake_frames/seq_dynamic_wakes.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_frames/streamlines.py` & `foxes-0.7.2/foxes/models/wake_frames/streamlines.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_frames/timelines.py` & `foxes-0.7.2/foxes/models/wake_frames/timelines.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_frames/yawed_wakes.py` & `foxes-0.7.2/foxes/models/wake_frames/yawed_wakes.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/axisymmetric.py` & `foxes-0.7.2/foxes/models/wake_models/axisymmetric.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/dist_sliced.py` & `foxes-0.7.2/foxes/models/wake_models/dist_sliced.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/gaussian.py` & `foxes-0.7.2/foxes/models/wake_models/gaussian.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/induction/rankine_half_body.py` & `foxes-0.7.2/foxes/models/wake_models/induction/rankine_half_body.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/induction/rathmann.py` & `foxes-0.7.2/foxes/models/wake_models/induction/rathmann.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/induction/self_similar.py` & `foxes-0.7.2/foxes/models/wake_models/induction/self_similar.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/induction/self_similar2020.py` & `foxes-0.7.2/foxes/models/wake_models/induction/self_similar2020.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/ti/crespo_hernandez.py` & `foxes-0.7.2/foxes/models/wake_models/ti/crespo_hernandez.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/ti/iec_ti.py` & `foxes-0.7.2/foxes/models/wake_models/ti/iec_ti.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/top_hat.py` & `foxes-0.7.2/foxes/models/wake_models/top_hat.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/wake_mirror.py` & `foxes-0.7.2/foxes/models/wake_models/wake_mirror.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/wind/bastankhah14.py` & `foxes-0.7.2/foxes/models/wake_models/wind/bastankhah14.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/wind/bastankhah16.py` & `foxes-0.7.2/foxes/models/wake_models/wind/bastankhah16.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/wind/jensen.py` & `foxes-0.7.2/foxes/models/wake_models/wind/jensen.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_models/wind/turbopark.py` & `foxes-0.7.2/foxes/models/wake_models/wind/turbopark.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_superpositions/ti_linear.py` & `foxes-0.7.2/foxes/models/wake_superpositions/ti_linear.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_superpositions/ti_max.py` & `foxes-0.7.2/foxes/models/wake_superpositions/ti_max.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_superpositions/ti_pow.py` & `foxes-0.7.2/foxes/models/wake_superpositions/ti_pow.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_superpositions/ti_quadratic.py` & `foxes-0.7.2/foxes/models/wake_superpositions/ti_quadratic.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_superpositions/ws_linear.py` & `foxes-0.7.2/foxes/models/wake_superpositions/ws_linear.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_superpositions/ws_max.py` & `foxes-0.7.2/foxes/models/wake_superpositions/ws_max.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,14 +178,15 @@
         w = -wake_delta
         if self.lim_low is not None:
             w = np.maximum(w, self.lim_low - amb_results)
         if self.lim_high is not None:
             w = np.minimum(w, self.lim_high - amb_results)
         return w
 
+
 class WSMaxLocal(WakeSuperposition):
     """
     Local max supersposition of wind deficit results
 
     Attributes
     ----------
     lim_low: float
```

### Comparing `foxes-0.7.1/foxes/models/wake_superpositions/ws_pow.py` & `foxes-0.7.2/foxes/models/wake_superpositions/ws_pow.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,15 @@
         w = -(wake_delta ** (1 / self.pow))
         if self.lim_low is not None:
             w = np.maximum(w, self.lim_low - amb_results)
         if self.lim_high is not None:
             w = np.minimum(w, self.lim_high - amb_results)
         return w
 
+
 class WSPowLocal(WakeSuperposition):
     """
     Local power supersposition of wind deficit results
 
     Attributes
     ----------
     pow: float
```

### Comparing `foxes-0.7.1/foxes/models/wake_superpositions/ws_product.py` & `foxes-0.7.2/foxes/models/wake_superpositions/ws_product.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/models/wake_superpositions/ws_quadratic.py` & `foxes-0.7.2/foxes/models/wake_superpositions/ws_quadratic.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,14 +175,15 @@
         w = -np.sqrt(wake_delta)
         if self.lim_low is not None:
             w = np.maximum(w, self.lim_low - amb_results)
         if self.lim_high is not None:
             w = np.minimum(w, self.lim_high - amb_results)
         return w
 
+
 class WSQuadraticLocal(WakeSuperposition):
     """
     Local quadratic supersposition of wind deficit results
 
     Attributes
     ----------
     lim_low: float
```

### Comparing `foxes-0.7.1/foxes/opt/constraints/area_geometry.py` & `foxes-0.7.2/foxes/opt/constraints/area_geometry.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/constraints/min_dist.py` & `foxes-0.7.2/foxes/opt/constraints/min_dist.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/core/farm_constraint.py` & `foxes-0.7.2/foxes/opt/core/farm_constraint.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/core/farm_objective.py` & `foxes-0.7.2/foxes/opt/core/farm_objective.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/core/farm_opt_problem.py` & `foxes-0.7.2/foxes/opt/core/farm_opt_problem.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/core/farm_vars_problem.py` & `foxes-0.7.2/foxes/opt/core/farm_vars_problem.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/core/pop_states.py` & `foxes-0.7.2/foxes/opt/core/pop_states.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/objectives/farm_vars.py` & `foxes-0.7.2/foxes/opt/objectives/farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/objectives/max_n_turbines.py` & `foxes-0.7.2/foxes/opt/objectives/max_n_turbines.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/problems/layout/farm_layout.py` & `foxes-0.7.2/foxes/opt/problems/layout/farm_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/constraints.py` & `foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/constraints.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_layout.py` & `foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/geom_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py` & `foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/geom_layout_gridded.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py` & `foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/geom_reggrid.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py` & `foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/geom_reggrids.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/problems/layout/geom_layouts/objectives.py` & `foxes-0.7.2/foxes/opt/problems/layout/geom_layouts/objectives.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/problems/layout/reggrids_layout.py` & `foxes-0.7.2/foxes/opt/problems/layout/reggrids_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/problems/layout/regular_layout.py` & `foxes-0.7.2/foxes/opt/problems/layout/regular_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/opt/problems/opt_farm_vars.py` & `foxes-0.7.2/foxes/opt/problems/opt_farm_vars.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/__init__.py` & `foxes-0.7.2/foxes/output/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/animation.py` & `foxes-0.7.2/foxes/output/animation.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/calc_points.py` & `foxes-0.7.2/foxes/output/calc_points.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/farm_layout.py` & `foxes-0.7.2/foxes/output/farm_layout.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/farm_results_eval.py` & `foxes-0.7.2/foxes/output/farm_results_eval.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/flow_plots_2d/flow_plots.py` & `foxes-0.7.2/foxes/output/flow_plots_2d/flow_plots.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/flow_plots_2d/get_fig.py` & `foxes-0.7.2/foxes/output/flow_plots_2d/get_fig.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/flow_plots_2d/seq_flow_ani_plugin.py` & `foxes-0.7.2/foxes/output/flow_plots_2d/seq_flow_ani_plugin.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/grids.py` & `foxes-0.7.2/foxes/output/grids.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/output.py` & `foxes-0.7.2/foxes/output/output.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/results_writer.py` & `foxes-0.7.2/foxes/output/results_writer.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/rose_plot.py` & `foxes-0.7.2/foxes/output/rose_plot.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/rotor_point_plots.py` & `foxes-0.7.2/foxes/output/rotor_point_plots.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/slice_data.py` & `foxes-0.7.2/foxes/output/slice_data.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/state_turbine_map.py` & `foxes-0.7.2/foxes/output/state_turbine_map.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/output/turbine_type_curves.py` & `foxes-0.7.2/foxes/output/turbine_type_curves.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/__init__.py` & `foxes-0.7.2/foxes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/abl/neutral.py` & `foxes-0.7.2/foxes/utils/abl/neutral.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/abl/stable.py` & `foxes-0.7.2/foxes/utils/abl/stable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/abl/unstable.py` & `foxes-0.7.2/foxes/utils/abl/unstable.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/cubic_roots.py` & `foxes-0.7.2/foxes/utils/cubic_roots.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/data_book.py` & `foxes-0.7.2/foxes/utils/data_book.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/dict.py` & `foxes-0.7.2/foxes/utils/dict.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/exec_python.py` & `foxes-0.7.2/foxes/utils/exec_python.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/factory.py` & `foxes-0.7.2/foxes/utils/factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import numpy as np
+
 from .dict import Dict
 
+
 class Factory:
     """
-    Constructs objects from a choice of allowed 
+    Constructs objects from a choice of allowed
     constructor parameters
-    
+
     Attributes
     ----------
     base: class
         The class of which objects are to be created
     name_template: str
         The name template, e.g. 'name_<A>_<B>_<C>' for
         variables A, B, C
@@ -18,33 +21,34 @@
         Fixed arguments for the base class
     var2arg: dict
         Mapping from variable to constructor argument
     hints: dict
         Hints for print_toc, only for variables for which the
         options are functions or missing
     options: dict
-        For each variable, e.g. A, B or C, the list or dict 
+        For each variable, e.g. A, B or C, the list or dict
         or function that maps a str to the actual value
 
     :group: utils
-    
+
     """
+
     def __init__(
-            self,
-            base,
-            name_template,
-            args=(),
-            kwargs={},
-            var2arg={},
-            hints={},
-            **options,
-        ):
+        self,
+        base,
+        name_template,
+        args=(),
+        kwargs={},
+        var2arg={},
+        hints={},
+        **options,
+    ):
         """
         Constructor.
-        
+
         Parameters
         ----------
         base: class
             The class of which objects are to be created
         name_template: str
             The name template, e.g. 'name_<A>_<B>_<C>' for
             variables A, B, C
@@ -54,187 +58,198 @@
             Fixed arguments for the base class
         var2arg: dict
             Mapping from variable to constructor argument
         hints: dict
             Hints for print_toc, only for variables for which the
             options are functions or missing
         options: dict
-            For each variable, e.g. A, B or C, the list or dict 
+            For each variable, e.g. A, B or C, the list or dict
             or function that maps a str to the actual value
-        
+
         """
         self.base = base
         self.name_template = name_template
         self.args = args
         self.kwargs = kwargs
         self.var2arg = var2arg
         self.hints = hints
 
         parts = name_template.split(">")
         if len(parts) < 2:
-            raise ValueError(f"Factory '{name_template}': Expecting at least one variable in template, pattern '<..>'")
+            raise ValueError(
+                f"Factory '{name_template}': Expecting at least one variable in template, pattern '<..>'"
+            )
 
         self._vars = []
         self._pre = []
         for i, p in enumerate(parts):
             if i < len(parts) - 1:
                 parts2 = p.split("<")
                 if len(parts2) != 2:
-                    raise ValueError(f"Factory '{name_template}': incomplete pattern brackets '<..>'")
+                    raise ValueError(
+                        f"Factory '{name_template}': incomplete pattern brackets '<..>' between variables, e.g. '_'"
+                    )
+                if i > 0 and len(parts2[0]) == 0:
+                    raise ValueError(
+                        f"Factory '{name_template}': Missing seperator like '_' in template between variables '{self._vars[-1]}' and '{parts[1]}'"
+                    )
                 self._pre.append(parts2[0])
                 self._vars.append(parts2[1])
             else:
                 self._pre.append(p)
 
         if len(self.variables) > 1:
             for vi, v in enumerate(self.variables):
                 p = self._pre[vi]
                 if vi < len(self.variables) - 1 and p == "":
-                    raise ValueError(f"Factory '{name_template}': Require indicator before variable '{v}' in template, e.g. '{v}<{v}>'")
-        
+                    raise ValueError(
+                        f"Factory '{name_template}': Require indicator before variable '{v}' in template, e.g. '{v}<{v}>'"
+                    )
+
         self.options = Dict(name=f"{self._pre[0]}_options")
-        for v, o  in options.items():
+        for v, o in options.items():
             if v not in self.variables:
-                raise KeyError(f"Factory '{name_template}': Variable '{v}' found in options, but not in template")
+                raise KeyError(
+                    f"Factory '{name_template}': Variable '{v}' found in options, but not in template"
+                )
             if isinstance(o, list) or isinstance(o, tuple):
                 o = {str(k): k for k in o}
             if isinstance(o, dict):
                 for k in o.keys():
                     if not isinstance(k, str):
-                        raise TypeError(f"Factory '{name_template}': Found option for variable '{v}' that is not a str, {k}")
+                        raise TypeError(
+                            f"Factory '{name_template}': Found option for variable '{v}' that is not a str, {k}"
+                        )
                 self.options[v] = Dict(name=f"{self._pre[0]}_options_{v}", **o)
             elif hasattr(o, "__call__"):
                 self.options[v] = o
             else:
-                raise ValueError(f"Factory '{name_template}': Variable '{v}' has option of type '{type(v).__name__}'. Only list, tuple, dict or function are supported")
-    
+                raise ValueError(
+                    f"Factory '{name_template}': Variable '{v}' has option of type '{type(v).__name__}'. Only list, tuple, dict or function are supported"
+                )
+
     @property
     def name_prefix(self):
         """
         The beginning of the name template
-        
+
         Returns
         -------
         nbase: str
             The beginning of the name template
-        
+
         """
         return self._pre[0]
 
     @property
     def name_suffix(self):
         """
         The ending of the name template
-        
+
         Returns
         -------
         nbase: str
             The ending of the name template
-        
+
         """
         return self._pre[-1]
-    
+
     @property
     def variables(self):
         """
         The list of variables
-        
+
         Returns
         -------
         vrs: list of str
             The variables
-        
+
         """
         return self._vars
-    
+
     def __str__(self):
-        """ String representation """
+        """String representation"""
         s = f"{self.name_template}: {self.base.__name__} with"
         for k, d in self.kwargs.items():
             s += f"\n  {k}={d}"
         for v in self.variables:
             if v in self.options and isinstance(self.options[v], dict):
                 s += f"\n  {v} from {list(self.options[v])}"
             else:
                 s += f"\n  {v}={self.hints.get(v, '(value)')}"
         return s
-    
+
     def check_match(self, name):
         """
         Tests if a name matches the template
-        
+
         Parameters
         ----------
         name: str
             The name to be checked
 
         Returns
         -------
         success: bool
             True if the template is matched
-        
+
         """
         data_str = name
         for vi in range(len(self.variables)):
             p = self._pre[vi]
             i = data_str.find(p)
             j = i + len(p)
             if i < 0 or len(data_str) <= j:
                 return False
             data_str = data_str[j:]
 
-            q = self._pre[vi+1]
+            q = self._pre[vi + 1]
             if q != "":
                 i = data_str.find(q)
                 j = i + len(q)
                 if i < 0 or len(data_str) <= j:
                     return False
             else:
                 data_str = ""
-        
+
         return True
 
     def construct(self, name):
         """
         Create an object of the base class.
-        
+
         Parameters
         ----------
         name: str
             The name, matching the template
-        
+
         Returns
         -------
         obj: object
             The instance of the base class
-        
+
         """
-        data_str = name
+        j = 0
         wlist = []
-        for vi, v in enumerate(self.variables):
-            p = self._pre[vi]
-            i = data_str.find(p)
-            j = i + len(p)
-            if i < 0 or len(data_str) <= j:
-                raise ValueError(f"Factory '{self.name_template}': Name '{name}' not matching template")
-            data_str = data_str[j:]
-
-            q = self._pre[vi+1]
-            if q != "":
-                i = data_str.find(q)
-                j = i + len(q)
-                if i < 0 or len(data_str) <= j:
-                    raise ValueError(f"Factory '{self.name_template}': Name '{name}' not matching template")
-                wlist.append(data_str[:i])
+        for pi, p in enumerate(self._pre):
+            if len(p) > 0:
+                i = name[j:].find(p)
+                if i < 0 or (pi == 0 and i > 0):
+                    raise ValueError(
+                        f"Factory '{self.name_template}': Name '{name}' not matching template"
+                    )
+                w = name[j : j + i]
+                j += i + len(p)
             else:
-                wlist.append(data_str)
-                data_str = ""
+                w = name[j:]
+            if pi > 0:
+                wlist.append(w)
 
         kwargs = {}
-        for vi, v in enumerate(self.variables):          
+        for vi, v in enumerate(self.variables):
             w = self.var2arg.get(v, v)
             data = wlist[vi]
             if v in self.options:
                 o = self.options[v]
                 if hasattr(o, "__call__"):
                     kwargs[w] = o(data)
                 else:
@@ -242,64 +257,66 @@
             else:
                 kwargs[w] = data
 
         kwargs.update(self.kwargs)
 
         return self.base(*self.args, **kwargs)
 
+
 class FDict(Dict):
     """
     A dictionary with factory support
-    
+
     Attributes
     ----------
     store_created: bool
         Flag for storing created objects
     factories: list of foxes.utils.Factory
         The factories
-    
+
     :group: utils
-    
+
     """
+
     def __init__(self, *args, store_created=True, **kwargs):
         """
         Constructor.
-        
+
         Parameters
         ----------
         args: tuple, optional
             Parameters for the base class
         store_created: bool
             Flag for storing created objects
         kwargs: dict, optional
             Parameters for the base class
-        
+
         """
         super().__init__(*args, **kwargs)
         self.store_created = store_created
         self.factories = []
 
     def add_factory(self, *args, **kwargs):
         """
         Constructor.
-        
+
         Parameters
         ----------
         args: tuple, optional
             Parameters for the Factory constructor
         kwargs: dict, optional
             Parameters for the Factory constructor
-        
+
         """
         f = Factory(*args, **kwargs)
         i = len(self.factories)
         for gi in range(len(self.factories) - 1, -1, -1):
             g = self.factories[gi]
             if (
-                g.name_prefix == f.name_prefix 
+                g.name_prefix == f.name_prefix
                 and g.name_suffix == f.name_suffix
                 and len(f.variables) > len(g.variables)
             ):
                 i = gi
 
         if i == len(self.factories):
             self.factories.append(f)
@@ -326,8 +343,7 @@
                     return obj
                 except ValueError:
                     pass
 
         k = ", ".join(sorted(list(self.keys())))
         e = f"{self.name}: Cannot find key '{key}', also no factory matches. Known keys: {k}. Known factories: {[f.name_template for f in self.factories]}"
         raise KeyError(e)
-
```

### Comparing `foxes-0.7.1/foxes/utils/geom2d/area_geometry.py` & `foxes-0.7.2/foxes/utils/geom2d/area_geometry.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/geom2d/circle.py` & `foxes-0.7.2/foxes/utils/geom2d/circle.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/geom2d/example_intersection.py` & `foxes-0.7.2/foxes/utils/geom2d/example_intersection.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/geom2d/example_union.py` & `foxes-0.7.2/foxes/utils/geom2d/example_union.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/geom2d/half_plane.py` & `foxes-0.7.2/foxes/utils/geom2d/half_plane.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/geom2d/polygon.py` & `foxes-0.7.2/foxes/utils/geom2d/polygon.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/geopandas_helpers.py` & `foxes-0.7.2/foxes/utils/geopandas_helpers.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/geopandas_utils.py` & `foxes-0.7.2/foxes/utils/geopandas_utils.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/load.py` & `foxes-0.7.2/foxes/utils/load.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/pandas_helpers.py` & `foxes-0.7.2/foxes/utils/pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/pandas_utils.py` & `foxes-0.7.2/foxes/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/random_xy.py` & `foxes-0.7.2/foxes/utils/random_xy.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/regularize.py` & `foxes-0.7.2/foxes/utils/regularize.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/runners/runners.py` & `foxes-0.7.2/foxes/utils/runners/runners.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/tab_files.py` & `foxes-0.7.2/foxes/utils/tab_files.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/two_circles.py` & `foxes-0.7.2/foxes/utils/two_circles.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/wind_dir.py` & `foxes-0.7.2/foxes/utils/wind_dir.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/windrose_plot.py` & `foxes-0.7.2/foxes/utils/windrose_plot.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/utils/xarray_utils.py` & `foxes-0.7.2/foxes/utils/xarray_utils.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes/variables.py` & `foxes-0.7.2/foxes/variables.py`

 * *Files identical despite different names*

### Comparing `foxes-0.7.1/foxes.egg-info/PKG-INFO` & `foxes-0.7.2/foxes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxes
-Version: 0.7.1
+Version: 0.7.2
 Summary: Farm Optimization and eXtended yield Evaluation Software
 Author: Fraunhofer IWES
 Author-email: jonas.schmidt@iwes.fraunhofer.de
 License: MIT
 Project-URL: Source Code, https://github.com/FraunhoferIWES/foxes
 Project-URL: Bug Tracker, https://github.com/FraunhoferIWES/foxes/issues
 Project-URL: Documentation, https://fraunhoferiwes.github.io/foxes.docs/index.html
```

### Comparing `foxes-0.7.1/foxes.egg-info/SOURCES.txt` & `foxes-0.7.2/foxes.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -94,17 +94,17 @@
 foxes/input/states/create/__init__.py
 foxes/input/states/create/random_abl_states.py
 foxes/input/states/create/random_timeseries.py
 foxes/input/windio/__init__.py
 foxes/input/windio/windio.py
 foxes/models/__init__.py
 foxes/models/model_book.py
-foxes/models/axial_induction_models/__init__.py
-foxes/models/axial_induction_models/betz.py
-foxes/models/axial_induction_models/madsen.py
+foxes/models/axial_induction/__init__.py
+foxes/models/axial_induction/betz.py
+foxes/models/axial_induction/madsen.py
 foxes/models/farm_controllers/__init__.py
 foxes/models/farm_controllers/basic.py
 foxes/models/farm_models/__init__.py
 foxes/models/farm_models/turbine2farm.py
 foxes/models/partial_wakes/__init__.py
 foxes/models/partial_wakes/axiwake.py
 foxes/models/partial_wakes/centre.py
```

### Comparing `foxes-0.7.1/setup.cfg` & `foxes-0.7.2/setup.cfg`

 * *Files identical despite different names*

