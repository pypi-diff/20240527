# Comparing `tmp/starling-sim-0.9.0.tar.gz` & `tmp/starling-sim-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starling-sim-0.9.0.tar", last modified: Tue Aug  2 13:15:01 2022, max compression
+gzip compressed data, was "starling-sim-0.9.1.tar", last modified: Tue Aug  9 19:22:48 2022, max compression
```

## Comparing `starling-sim-0.9.0.tar` & `starling-sim-0.9.1.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.760326 starling-sim-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)    21415 2022-08-02 13:14:44.000000 starling-sim-0.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-02 13:14:44.000000 starling-sim-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-08-02 13:15:01.760326 starling-sim-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4648 2022-08-02 13:14:44.000000 starling-sim-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-02 13:15:01.760326 starling-sim-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3025 2022-08-02 13:14:44.000000 starling-sim-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.748326 starling-sim-0.9.0/starling_sim/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.748326 starling-sim-0.9.0/starling_sim/basemodel/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.752326 starling-sim-0.9.0/starling_sim/basemodel/agent/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10447 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     9026 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/moving_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.752326 starling-sim-0.9.0/starling_sim/basemodel/agent/operators/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26216 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/operators/operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/operators/station_based_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.752326 starling-sim-0.9.0/starling_sim/basemodel/agent/persons/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/persons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13219 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/persons/person.py
--rw-r--r--   0 runner    (1001) docker     (121)    16177 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/requests.py
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/spatial_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.752326 starling-sim-0.9.0/starling_sim/basemodel/agent/stations/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/stations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/stations/station.py
--rw-r--r--   0 runner    (1001) docker     (121)     6483 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/stations/vehicle_sharing_station.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.752326 starling-sim-0.9.0/starling_sim/basemodel/agent/vehicles/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/vehicles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4119 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/vehicles/repositioning_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (121)    13972 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/vehicles/service_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/vehicles/station_based_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (121)     3837 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/agent/vehicles/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.752326 starling-sim-0.9.0/starling_sim/basemodel/algorithms/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/algorithms/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)     4438 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/algorithms/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)    14968 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/algorithms/pal_zhang_GCH.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/algorithms/pal_zhang_dispatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.752326 starling-sim-0.9.0/starling_sim/basemodel/environment/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21751 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/environment/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.752326 starling-sim-0.9.0/starling_sim/basemodel/input/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25474 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/input/dynamic_input.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.756326 starling-sim-0.9.0/starling_sim/basemodel/output/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6042 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/output/feature_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     9906 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/output/geojson_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     6000 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/output/information_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/output/kpi_output.py
--rw-r--r--   0 runner    (1001) docker     (121)    30363 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/output/kpis.py
--rw-r--r--   0 runner    (1001) docker     (121)     7429 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/output/output_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.756326 starling-sim-0.9.0/starling_sim/basemodel/population/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/population/agent_population.py
--rw-r--r--   0 runner    (1001) docker     (121)     2964 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/population/dict_population.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.756326 starling-sim-0.9.0/starling_sim/basemodel/schedule/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/schedule/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     6333 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/simulation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.756326 starling-sim-0.9.0/starling_sim/basemodel/topology/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2184 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/topology/bike_weight_osm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/topology/network_weight.py
--rw-r--r--   0 runner    (1001) docker     (121)     3913 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/topology/osm_network.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/topology/simple_time_weight.py
--rw-r--r--   0 runner    (1001) docker     (121)     8054 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/topology/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.756326 starling-sim-0.9.0/starling_sim/basemodel/trace/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12329 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/trace/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/basemodel/trace/trace.py
--rw-r--r--   0 runner    (1001) docker     (121)     5834 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/model_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.756326 starling-sim-0.9.0/starling_sim/models/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.756326 starling-sim-0.9.0/starling_sim/models/FF_VS/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/FF_VS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/FF_VS/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/FF_VS/output.py
--rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/FF_VS/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.756326 starling-sim-0.9.0/starling_sim/models/SB_VS/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/SB_VS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/SB_VS/input.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/SB_VS/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/SB_VS/output.py
--rw-r--r--   0 runner    (1001) docker     (121)     8640 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/SB_VS/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.760326 starling-sim-0.9.0/starling_sim/models/SB_VS_R/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/SB_VS_R/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/SB_VS_R/input.py
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/SB_VS_R/model.py
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/SB_VS_R/operator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/SB_VS_R/output.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/SB_VS_R/repositioning_staff.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.760326 starling-sim-0.9.0/starling_sim/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.760326 starling-sim-0.9.0/starling_sim/schemas/geojson/
--rw-r--r--   0 runner    (1001) docker     (121)    13638 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/geojson/Feature.json
--rw-r--r--   0 runner    (1001) docker     (121)    17008 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/geojson/FeatureCollection.json
--rw-r--r--   0 runner    (1001) docker     (121)    45759 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/geojson/GeoJSON.json
--rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/geojson/Geometry.json
--rw-r--r--   0 runner    (1001) docker     (121)     6065 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/geojson/GeometryCollection.json
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/geojson/LineString.json
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/geojson/MultiLineString.json
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/geojson/MultiPoint.json
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/geojson/MultiPolygon.json
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/geojson/Point.json
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/geojson/Polygon.json
--rw-r--r--   0 runner    (1001) docker     (121)     9114 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/parameters.schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/schemas/starling_config.schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     4306 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/simulation_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.760326 starling-sim-0.9.0/starling_sim/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     5847 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/utils/data_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)    13127 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     4446 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/utils/simulation_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     6579 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/utils/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    31895 2022-08-02 13:14:44.000000 starling-sim-0.9.0/starling_sim/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-02 13:14:52.000000 starling-sim-0.9.0/starling_sim/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 13:15:01.748326 starling-sim-0.9.0/starling_sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-08-02 13:15:01.000000 starling-sim-0.9.0/starling_sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4207 2022-08-02 13:15:01.000000 starling-sim-0.9.0/starling_sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 13:15:01.000000 starling-sim-0.9.0/starling_sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-08-02 13:15:01.000000 starling-sim-0.9.0/starling_sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-02 13:15:01.000000 starling-sim-0.9.0/starling_sim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.015637 starling-sim-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    21415 2022-08-09 19:22:30.000000 starling-sim-0.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-09 19:22:30.000000 starling-sim-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-08-09 19:22:48.015637 starling-sim-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4648 2022-08-09 19:22:30.000000 starling-sim-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:22:48.015637 starling-sim-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3025 2022-08-09 19:22:30.000000 starling-sim-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.007637 starling-sim-0.9.1/starling_sim/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.007637 starling-sim-0.9.1/starling_sim/basemodel/
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.007637 starling-sim-0.9.1/starling_sim/basemodel/agent/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10447 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9026 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/moving_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.007637 starling-sim-0.9.1/starling_sim/basemodel/agent/operators/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26216 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/operators/operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/operators/station_based_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.007637 starling-sim-0.9.1/starling_sim/basemodel/agent/persons/
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/persons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13219 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/persons/person.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16177 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/requests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      780 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/spatial_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.007637 starling-sim-0.9.1/starling_sim/basemodel/agent/stations/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/stations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      787 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/stations/station.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6483 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/stations/vehicle_sharing_station.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.007637 starling-sim-0.9.1/starling_sim/basemodel/agent/vehicles/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/vehicles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4119 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/vehicles/repositioning_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13972 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/vehicles/service_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/vehicles/station_based_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3837 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/agent/vehicles/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.007637 starling-sim-0.9.1/starling_sim/basemodel/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/algorithms/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4438 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/algorithms/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14968 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/algorithms/pal_zhang_GCH.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/algorithms/pal_zhang_dispatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.007637 starling-sim-0.9.1/starling_sim/basemodel/environment/
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21751 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/environment/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.011637 starling-sim-0.9.1/starling_sim/basemodel/input/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25474 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/input/dynamic_input.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.011637 starling-sim-0.9.1/starling_sim/basemodel/output/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6042 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/output/feature_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9906 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/output/geojson_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6000 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/output/information_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/output/kpi_output.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30363 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/output/kpis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7429 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/output/output_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.011637 starling-sim-0.9.1/starling_sim/basemodel/population/
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/population/agent_population.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2964 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/population/dict_population.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.011637 starling-sim-0.9.1/starling_sim/basemodel/schedule/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/schedule/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6333 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/simulation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.011637 starling-sim-0.9.1/starling_sim/basemodel/topology/
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2184 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/topology/bike_weight_osm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/topology/network_weight.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3913 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/topology/osm_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/topology/simple_time_weight.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8054 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/topology/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.011637 starling-sim-0.9.1/starling_sim/basemodel/trace/
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12329 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/trace/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/basemodel/trace/trace.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6000 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/model_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.011637 starling-sim-0.9.1/starling_sim/models/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.011637 starling-sim-0.9.1/starling_sim/models/FF_VS/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/FF_VS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/FF_VS/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/FF_VS/output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/FF_VS/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.011637 starling-sim-0.9.1/starling_sim/models/SB_VS/
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/SB_VS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/SB_VS/input.py
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/SB_VS/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/SB_VS/output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8640 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/SB_VS/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.011637 starling-sim-0.9.1/starling_sim/models/SB_VS_R/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/SB_VS_R/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/SB_VS_R/input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/SB_VS_R/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      864 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/SB_VS_R/operator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/SB_VS_R/output.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/SB_VS_R/repositioning_staff.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/run.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.011637 starling-sim-0.9.1/starling_sim/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.015637 starling-sim-0.9.1/starling_sim/schemas/geojson/
+-rw-r--r--   0 runner    (1001) docker     (121)    13638 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/geojson/Feature.json
+-rw-r--r--   0 runner    (1001) docker     (121)    17008 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/geojson/FeatureCollection.json
+-rw-r--r--   0 runner    (1001) docker     (121)    45759 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/geojson/GeoJSON.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/geojson/Geometry.json
+-rw-r--r--   0 runner    (1001) docker     (121)     6065 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/geojson/GeometryCollection.json
+-rw-r--r--   0 runner    (1001) docker     (121)      646 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/geojson/LineString.json
+-rw-r--r--   0 runner    (1001) docker     (121)      727 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/geojson/MultiLineString.json
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/geojson/MultiPoint.json
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/geojson/MultiPolygon.json
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/geojson/Point.json
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/geojson/Polygon.json
+-rw-r--r--   0 runner    (1001) docker     (121)     9303 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/parameters.schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/schemas/starling_config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     4806 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/simulation_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.015637 starling-sim-0.9.1/starling_sim/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5847 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/utils/data_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13127 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4446 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/utils/simulation_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6579 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/utils/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33863 2022-08-09 19:22:30.000000 starling-sim-0.9.1/starling_sim/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-09 19:22:38.000000 starling-sim-0.9.1/starling_sim/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:22:48.007637 starling-sim-0.9.1/starling_sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-08-09 19:22:47.000000 starling-sim-0.9.1/starling_sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4207 2022-08-09 19:22:48.000000 starling-sim-0.9.1/starling_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:22:47.000000 starling-sim-0.9.1/starling_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-08-09 19:22:47.000000 starling-sim-0.9.1/starling_sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-08-09 19:22:47.000000 starling-sim-0.9.1/starling_sim.egg-info/top_level.txt
```

### Comparing `starling-sim-0.9.0/LICENSE.txt` & `starling-sim-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/PKG-INFO` & `starling-sim-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starling-sim
-Version: 0.9.0
+Version: 0.9.1
 Summary: Agent-based framework for mobility simulation
 Home-page: https://github.com/tellae/starling
 Author: Tellae
 Author-email: starling@tellae.fr
 License: CECILL-B
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `starling-sim-0.9.0/README.md` & `starling-sim-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/setup.py` & `starling-sim-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/agent.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/agent.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/moving_agent.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/moving_agent.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/operators/operator.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/operators/operator.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/operators/station_based_operator.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/operators/station_based_operator.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/persons/person.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/persons/person.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/requests.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/requests.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/spatial_agent.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/spatial_agent.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/stations/station.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/stations/station.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/stations/vehicle_sharing_station.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/stations/vehicle_sharing_station.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/vehicles/repositioning_vehicle.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/vehicles/repositioning_vehicle.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/vehicles/service_vehicle.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/vehicles/service_vehicle.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/vehicles/station_based_vehicle.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/vehicles/station_based_vehicle.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/agent/vehicles/vehicle.py` & `starling-sim-0.9.1/starling_sim/basemodel/agent/vehicles/vehicle.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/algorithms/algorithm.py` & `starling-sim-0.9.1/starling_sim/basemodel/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/algorithms/dispatcher.py` & `starling-sim-0.9.1/starling_sim/basemodel/algorithms/dispatcher.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/algorithms/pal_zhang_GCH.py` & `starling-sim-0.9.1/starling_sim/basemodel/algorithms/pal_zhang_GCH.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/algorithms/pal_zhang_dispatcher.py` & `starling-sim-0.9.1/starling_sim/basemodel/algorithms/pal_zhang_dispatcher.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/environment/environment.py` & `starling-sim-0.9.1/starling_sim/basemodel/environment/environment.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/input/dynamic_input.py` & `starling-sim-0.9.1/starling_sim/basemodel/input/dynamic_input.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/output/feature_factory.py` & `starling-sim-0.9.1/starling_sim/basemodel/output/feature_factory.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/output/geojson_output.py` & `starling-sim-0.9.1/starling_sim/basemodel/output/geojson_output.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/output/information_factory.py` & `starling-sim-0.9.1/starling_sim/basemodel/output/information_factory.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/output/kpi_output.py` & `starling-sim-0.9.1/starling_sim/basemodel/output/kpi_output.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/output/kpis.py` & `starling-sim-0.9.1/starling_sim/basemodel/output/kpis.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/output/output_factory.py` & `starling-sim-0.9.1/starling_sim/basemodel/output/output_factory.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/population/agent_population.py` & `starling-sim-0.9.1/starling_sim/basemodel/population/agent_population.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/population/dict_population.py` & `starling-sim-0.9.1/starling_sim/basemodel/population/dict_population.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/schedule/scheduler.py` & `starling-sim-0.9.1/starling_sim/basemodel/schedule/scheduler.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/simulation_model.py` & `starling-sim-0.9.1/starling_sim/basemodel/simulation_model.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/topology/bike_weight_osm.py` & `starling-sim-0.9.1/starling_sim/basemodel/topology/bike_weight_osm.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/topology/network_weight.py` & `starling-sim-0.9.1/starling_sim/basemodel/topology/network_weight.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/topology/osm_network.py` & `starling-sim-0.9.1/starling_sim/basemodel/topology/osm_network.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/topology/topology.py` & `starling-sim-0.9.1/starling_sim/basemodel/topology/topology.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/trace/events.py` & `starling-sim-0.9.1/starling_sim/basemodel/trace/events.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/basemodel/trace/trace.py` & `starling-sim-0.9.1/starling_sim/basemodel/trace/trace.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/model_simulator.py` & `starling-sim-0.9.1/starling_sim/model_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from starling_sim.models.SB_VS.model import Model as SB_VS_model
 from starling_sim.models.SB_VS_R.model import Model as SB_VS_R_model
 from starling_sim.models.FF_VS.model import Model as FF_VS_model
 from starling_sim.simulation_scenario import SimulationScenario
 from starling_sim.utils.paths import model_import_path
+from starling_sim.utils.utils import create_sub_scenarios
 
 import logging
 import time
 import importlib
 
 models_dict = {"SB_VS": SB_VS_model, "SB_VS_R": SB_VS_R_model, "FF_VS": FF_VS_model}
 
@@ -116,28 +117,32 @@
 
     get_model_class = staticmethod(get_model_class)
 
 
 def launch_simulation(scenario_path, pkg):
     """
     Realises the initialisation, setup, run and output of the simulation
-    using the given parameters file. Displays logs of execution times
+    using the given parameters file. Displays log of execution times
 
     :param scenario_path: path to scenario folder
     :param pkg: name of the source package
     """
 
     if scenario_path is None:
         raise ValueError("No scenario folder provided to simulation launcher.")
 
     # initialise simulation scenario from folder path
     simulation_scenario = SimulationScenario(scenario_path)
     # read simulation parameters
     simulation_scenario.get_scenario_parameters()
 
+    if "multiple" in simulation_scenario:
+        create_sub_scenarios(simulation_scenario)
+        exit(0)
+
     # init the simulator
     logging.info(
         "Initializing simulator for the model code "
         + simulation_scenario["code"]
         + ", scenario "
         + simulation_scenario["scenario"]
         + "\n"
```

### Comparing `starling-sim-0.9.0/starling_sim/models/FF_VS/model.py` & `starling-sim-0.9.1/starling_sim/models/FF_VS/model.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/models/FF_VS/output.py` & `starling-sim-0.9.1/starling_sim/models/FF_VS/output.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/models/FF_VS/user.py` & `starling-sim-0.9.1/starling_sim/models/FF_VS/user.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/models/SB_VS/input.py` & `starling-sim-0.9.1/starling_sim/models/SB_VS/input.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/models/SB_VS/model.py` & `starling-sim-0.9.1/starling_sim/models/SB_VS/model.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/models/SB_VS/output.py` & `starling-sim-0.9.1/starling_sim/models/SB_VS/output.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/models/SB_VS/user.py` & `starling-sim-0.9.1/starling_sim/models/SB_VS/user.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/models/SB_VS_R/input.py` & `starling-sim-0.9.1/starling_sim/models/SB_VS_R/input.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/models/SB_VS_R/model.py` & `starling-sim-0.9.1/starling_sim/models/SB_VS_R/model.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/models/SB_VS_R/operator.py` & `starling-sim-0.9.1/starling_sim/models/SB_VS_R/operator.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/models/SB_VS_R/output.py` & `starling-sim-0.9.1/starling_sim/models/SB_VS_R/output.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/models/SB_VS_R/repositioning_staff.py` & `starling-sim-0.9.1/starling_sim/models/SB_VS_R/repositioning_staff.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/run.py` & `starling-sim-0.9.1/starling_sim/run.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/schemas/geojson/Feature.json` & `starling-sim-0.9.1/starling_sim/schemas/geojson/Feature.json`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/schemas/geojson/FeatureCollection.json` & `starling-sim-0.9.1/starling_sim/schemas/geojson/FeatureCollection.json`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/schemas/geojson/GeoJSON.json` & `starling-sim-0.9.1/starling_sim/schemas/geojson/GeoJSON.json`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/schemas/geojson/Geometry.json` & `starling-sim-0.9.1/starling_sim/schemas/geojson/Geometry.json`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/schemas/geojson/GeometryCollection.json` & `starling-sim-0.9.1/starling_sim/schemas/geojson/GeometryCollection.json`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/schemas/geojson/LineString.json` & `starling-sim-0.9.1/starling_sim/schemas/geojson/LineString.json`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/schemas/geojson/MultiLineString.json` & `starling-sim-0.9.1/starling_sim/schemas/geojson/MultiLineString.json`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/schemas/geojson/MultiPoint.json` & `starling-sim-0.9.1/starling_sim/schemas/geojson/MultiPoint.json`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/schemas/geojson/MultiPolygon.json` & `starling-sim-0.9.1/starling_sim/schemas/geojson/MultiPolygon.json`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/schemas/geojson/Point.json` & `starling-sim-0.9.1/starling_sim/schemas/geojson/Point.json`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/schemas/geojson/Polygon.json` & `starling-sim-0.9.1/starling_sim/schemas/geojson/Polygon.json`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/schemas/parameters.schema.json` & `starling-sim-0.9.1/starling_sim/schemas/parameters.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957983193277311%*

 * *Differences: {"'properties'": "{'multiple': OrderedDict([('advanced', True), ('type', 'integer'), ('title', "*

 * *                 "'Multiple scenario'), ('description', 'Number of sub scenarios to generate'), "*

 * *                 "('minimum', 1)])}"}*

```diff
@@ -80,14 +80,21 @@
                     "const": "ghosts",
                     "description": "Make all inputs static for the resolution, then remove prebooked==False from solution and insert them dynamically."
                 }
             ],
             "title": "Make inputs static",
             "type": "string"
         },
+        "multiple": {
+            "advanced": true,
+            "description": "Number of sub scenarios to generate",
+            "minimum": 1,
+            "title": "Multiple scenario",
+            "type": "integer"
+        },
         "scenario": {
             "description": "Name of the simulation scenario",
             "example": "example_scenario",
             "title": "Scenario name",
             "type": "string"
         },
         "seed": {
```

### Comparing `starling-sim-0.9.0/starling_sim/schemas/starling_config.schema.json` & `starling-sim-0.9.1/starling_sim/schemas/starling_config.schema.json`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/simulation_scenario.py` & `starling-sim-0.9.1/starling_sim/simulation_scenario.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,21 +48,29 @@
         Paths are built according to the structure enforced by the functions of starling_sim.utils.paths.
 
         :param scenario_folder_path: path to the scenario folder
         """
 
         # check scenario folder
         self.scenario_folder = os.path.join(scenario_folder_path, "")
-        if not os.path.exists(self.scenario_folder):
-            raise ValueError("The scenario folder does not exist : {}".format(self.scenario_folder))
+        if not (os.path.exists(self.scenario_folder) and os.path.isdir(self.scenario_folder)):
+            raise ValueError(
+                "The scenario folder does not exist or is not a folder : {}".format(
+                    self.scenario_folder
+                )
+            )
 
         # check inputs folder
         self.inputs_folder = paths.scenario_inputs_folder(self.scenario_folder)
-        if not os.path.exists(self.inputs_folder):
-            raise ValueError("The inputs folder does not exist : {}".format(self.inputs_folder))
+        if not (os.path.exists(self.inputs_folder) and os.path.isdir(self.inputs_folder)):
+            raise ValueError(
+                "The inputs folder does not exist or is not a folder : {}".format(
+                    self.inputs_folder
+                )
+            )
 
         # create outputs folder if it does not exist
         if "OUTPUT_FOLDER" in os.environ:
             output_folder = os.path.join(os.environ["OUTPUT_FOLDER"], "")
         else:
             output_folder = paths.scenario_outputs_folder(self.scenario_folder)
         self.outputs_folder = output_folder
@@ -81,14 +89,18 @@
         try:
             parameters_path = paths.scenario_parameters_filepath(self.scenario_folder)
             self.parameters = json_load(parameters_path)
 
         except (FileNotFoundError, json.JSONDecodeError) as e:
             raise ValueError("Error while loading the scenario parameters : {}".format(str(e)))
 
+        # check scenario folder against scenario name
+        if os.path.basename(os.path.dirname(self.scenario_folder)) != self.parameters["scenario"]:
+            raise ValueError("The scenario folder must be named after the scenario name")
+
         # parameters validation
         schema = json_load(paths.schemas_folder() + self.BASE_PARAM_SCHEMA)
         validate_against_schema(self.parameters, schema)
 
         # change date format from YYYY-MM-DD to YYYYMMDD
         if "date" in self.parameters:
             self.parameters["date"] = self.parameters["date"].replace("-", "")
```

### Comparing `starling-sim-0.9.0/starling_sim/utils/config.py` & `starling-sim-0.9.1/starling_sim/utils/config.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/utils/constants.py` & `starling-sim-0.9.1/starling_sim/utils/constants.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/utils/data_tree.py` & `starling-sim-0.9.1/starling_sim/utils/data_tree.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/utils/paths.py` & `starling-sim-0.9.1/starling_sim/utils/paths.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/utils/simulation_logging.py` & `starling-sim-0.9.1/starling_sim/utils/simulation_logging.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/utils/test_models.py` & `starling-sim-0.9.1/starling_sim/utils/test_models.py`

 * *Files identical despite different names*

### Comparing `starling-sim-0.9.0/starling_sim/utils/utils.py` & `starling-sim-0.9.1/starling_sim/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,22 @@
 import osmnx as ox
 import gzip
 import shutil
 import copy
 from shapely.geometry import Polygon, LineString
 from numbers import Integral
 from jsonschema import Draft7Validator, Draft4Validator, validators, ValidationError, RefResolver
-from starling_sim.utils.paths import schemas_folder, gtfs_feeds_folder, osm_graphs_folder
+from starling_sim.utils.paths import (
+    schemas_folder,
+    gtfs_feeds_folder,
+    osm_graphs_folder,
+    scenario_inputs_folder,
+    PARAMETERS_FILENAME,
+    INPUT_FOLDER_NAME,
+)
 
 pd.set_option("display.expand_frame_repr", False)
 
 
 # Starling exceptions
 
 
@@ -1060,7 +1067,57 @@
 
 
 def get_git_revision_hash() -> str:
     """
     Get current git commit hash
     """
     return subprocess.check_output(["git", "rev-parse", "HEAD"]).decode("ascii").strip()
+
+
+# multiple scenarios
+
+
+def create_sub_scenarios(simulation_scenario):
+
+    nb_scenarios = simulation_scenario["multiple"]
+    scenarios_folder = os.path.join(simulation_scenario.scenario_folder, "scenarios")
+    create_if_not_exists(scenarios_folder)
+
+    # set random seed
+    np.random.seed(simulation_scenario["seed"])
+    seeds = np.random.randint(100000, size=nb_scenarios)
+
+    sub_scenario_name_format = "{base_scenario}-{index}"
+
+    for i in range(nb_scenarios):
+
+        sub_scenario_name = sub_scenario_name_format.format(
+            base_scenario=simulation_scenario.name, index=i + 1
+        )
+        sub_scenario_folder = os.path.join(scenarios_folder, sub_scenario_name)
+        sub_scenario_inputs_folder = scenario_inputs_folder(sub_scenario_folder)
+
+        if os.path.exists(sub_scenario_folder):
+            print("Scenario {} already created".format(sub_scenario_name))
+            continue
+        else:
+            print("Creating scenario " + sub_scenario_name)
+
+        # create sub scenario folders
+        create_if_not_exists(sub_scenario_folder)
+        create_if_not_exists(sub_scenario_inputs_folder)
+
+        # sub scenario inputs
+        sub_parameters = simulation_scenario.copy_parameters()
+        sub_parameters["scenario"] = sub_scenario_name
+        sub_parameters["seed"] = int(seeds[i])
+        del sub_parameters["multiple"]
+        json_pretty_dump(
+            sub_parameters, os.path.join(sub_scenario_inputs_folder, PARAMETERS_FILENAME)
+        )
+
+        # create symlinks to original inputs
+        for input_file in os.listdir(simulation_scenario.inputs_folder):
+            if input_file == PARAMETERS_FILENAME:
+                continue
+            input_filepath = os.path.join("..", "..", "..", INPUT_FOLDER_NAME, input_file)
+            os.symlink(input_filepath, os.path.join(sub_scenario_inputs_folder, input_file))
```

### Comparing `starling-sim-0.9.0/starling_sim.egg-info/PKG-INFO` & `starling-sim-0.9.1/starling_sim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starling-sim
-Version: 0.9.0
+Version: 0.9.1
 Summary: Agent-based framework for mobility simulation
 Home-page: https://github.com/tellae/starling
 Author: Tellae
 Author-email: starling@tellae.fr
 License: CECILL-B
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `starling-sim-0.9.0/starling_sim.egg-info/SOURCES.txt` & `starling-sim-0.9.1/starling_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

