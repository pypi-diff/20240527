# Comparing `tmp/grid2demand-0.4.5.tar.gz` & `tmp/grid2demand-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grid2demand-0.4.5.tar", last modified: Sat May 18 02:28:44 2024, max compression
+gzip compressed data, was "grid2demand-0.4.6.tar", last modified: Mon May 27 01:50:40 2024, max compression
```

## Comparing `grid2demand-0.4.5.tar` & `grid2demand-0.4.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:44.586975 grid2demand-0.4.5/
--rw-rw-rw-   0        0        0    11558 2023-09-29 02:14:50.000000 grid2demand-0.4.5/LICENSE
--rw-rw-rw-   0        0        0     8385 2024-05-18 02:28:44.585975 grid2demand-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    34624 2024-05-18 02:27:14.000000 grid2demand-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:44.551120 grid2demand-0.4.5/grid2demand/
--rw-rw-rw-   0        0        0     1689 2024-05-18 02:28:24.000000 grid2demand-0.4.5/grid2demand/__init__.py
--rw-rw-rw-   0        0        0    53439 2024-05-16 17:50:59.000000 grid2demand-0.4.5/grid2demand/_grid2demand.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:44.567452 grid2demand-0.4.5/grid2demand/func_lib/
--rw-rw-rw-   0        0        0      282 2023-09-29 02:14:50.000000 grid2demand-0.4.5/grid2demand/func_lib/__init__.py
--rw-rw-rw-   0        0        0     2548 2024-05-13 22:33:57.000000 grid2demand-0.4.5/grid2demand/func_lib/gen_agent_demand.py
--rw-rw-rw-   0        0        0    20218 2024-05-13 22:41:08.000000 grid2demand-0.4.5/grid2demand/func_lib/gen_zone.py
--rw-rw-rw-   0        0        0     4182 2024-05-13 22:24:06.000000 grid2demand-0.4.5/grid2demand/func_lib/gravity_model.py
--rw-rw-rw-   0        0        0    18686 2024-05-13 22:20:21.000000 grid2demand-0.4.5/grid2demand/func_lib/read_node_poi.py
--rw-rw-rw-   0        0        0     6991 2024-05-13 22:35:49.000000 grid2demand-0.4.5/grid2demand/func_lib/trip_rate_production_attraction.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:44.584976 grid2demand-0.4.5/grid2demand/utils_lib/
--rw-rw-rw-   0        0        0      282 2023-09-29 02:14:50.000000 grid2demand-0.4.5/grid2demand/utils_lib/__init__.py
--rw-rw-rw-   0        0        0     6019 2024-05-17 23:40:00.000000 grid2demand-0.4.5/grid2demand/utils_lib/net_utils.py
--rw-rw-rw-   0        0        0     3385 2024-05-10 20:58:54.000000 grid2demand-0.4.5/grid2demand/utils_lib/pkg_settings.py
--rw-rw-rw-   0        0        0     9295 2024-05-13 22:38:13.000000 grid2demand-0.4.5/grid2demand/utils_lib/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:44.567452 grid2demand-0.4.5/grid2demand.egg-info/
--rw-rw-rw-   0        0        0     8385 2024-05-18 02:28:44.000000 grid2demand-0.4.5/grid2demand.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2024-05-18 02:28:44.000000 grid2demand-0.4.5/grid2demand.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 02:28:44.000000 grid2demand-0.4.5/grid2demand.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-05-18 02:28:44.000000 grid2demand-0.4.5/grid2demand.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-18 02:28:44.000000 grid2demand-0.4.5/grid2demand.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 02:28:44.586975 grid2demand-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1970 2024-05-18 02:28:37.000000 grid2demand-0.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 02:28:44.584976 grid2demand-0.4.5/tests/
--rw-rw-rw-   0        0        0      552 2024-03-01 23:27:54.000000 grid2demand-0.4.5/tests/test_read_node.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:50:40.918694 grid2demand-0.4.6/
+-rw-rw-rw-   0        0        0    11558 2023-09-29 02:14:50.000000 grid2demand-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0     7137 2024-05-27 01:50:40.917680 grid2demand-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0    29991 2024-05-27 01:49:46.000000 grid2demand-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 01:50:40.860784 grid2demand-0.4.6/grid2demand/
+-rw-rw-rw-   0        0        0     1689 2024-05-27 01:50:10.000000 grid2demand-0.4.6/grid2demand/__init__.py
+-rw-rw-rw-   0        0        0    53934 2024-05-27 01:38:42.000000 grid2demand-0.4.6/grid2demand/_grid2demand.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:50:40.911823 grid2demand-0.4.6/grid2demand/func_lib/
+-rw-rw-rw-   0        0        0      282 2023-09-29 02:14:50.000000 grid2demand-0.4.6/grid2demand/func_lib/__init__.py
+-rw-rw-rw-   0        0        0     2548 2024-05-13 22:33:57.000000 grid2demand-0.4.6/grid2demand/func_lib/gen_agent_demand.py
+-rw-rw-rw-   0        0        0    20218 2024-05-13 22:41:08.000000 grid2demand-0.4.6/grid2demand/func_lib/gen_zone.py
+-rw-rw-rw-   0        0        0     4276 2024-05-27 01:23:55.000000 grid2demand-0.4.6/grid2demand/func_lib/gravity_model.py
+-rw-rw-rw-   0        0        0    18916 2024-05-27 00:08:19.000000 grid2demand-0.4.6/grid2demand/func_lib/read_node_poi.py
+-rw-rw-rw-   0        0        0     6991 2024-05-13 22:35:49.000000 grid2demand-0.4.6/grid2demand/func_lib/trip_rate_production_attraction.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:50:40.915278 grid2demand-0.4.6/grid2demand/utils_lib/
+-rw-rw-rw-   0        0        0      282 2023-09-29 02:14:50.000000 grid2demand-0.4.6/grid2demand/utils_lib/__init__.py
+-rw-rw-rw-   0        0        0     6046 2024-05-26 19:06:08.000000 grid2demand-0.4.6/grid2demand/utils_lib/net_utils.py
+-rw-rw-rw-   0        0        0     3398 2024-05-26 19:04:28.000000 grid2demand-0.4.6/grid2demand/utils_lib/pkg_settings.py
+-rw-rw-rw-   0        0        0     9295 2024-05-13 22:38:13.000000 grid2demand-0.4.6/grid2demand/utils_lib/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:50:40.907999 grid2demand-0.4.6/grid2demand.egg-info/
+-rw-rw-rw-   0        0        0     7137 2024-05-27 01:50:40.000000 grid2demand-0.4.6/grid2demand.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2024-05-27 01:50:40.000000 grid2demand-0.4.6/grid2demand.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 01:50:40.000000 grid2demand-0.4.6/grid2demand.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-27 01:50:40.000000 grid2demand-0.4.6/grid2demand.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-27 01:50:40.000000 grid2demand-0.4.6/grid2demand.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 01:50:40.918694 grid2demand-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1970 2024-05-27 01:50:26.000000 grid2demand-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 01:50:40.916282 grid2demand-0.4.6/tests/
+-rw-rw-rw-   0        0        0      552 2024-03-01 23:27:54.000000 grid2demand-0.4.6/tests/test_read_node.py
```

### Comparing `grid2demand-0.4.5/LICENSE` & `grid2demand-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.5/PKG-INFO` & `grid2demand-0.4.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid2demand
-Version: 0.4.5
+Version: 0.4.6
 Summary: A tool for generating zone-to-zone travel demand based on grid cells or TAZs and gravity model
 Home-page: https://github.com/xyluo25/grid2demand
 Author: Xiangyong Luo, Dr.Xuesong(Simon) Zhou
 Author-email: luoxiangyong01@gmail.com, xzhou74@asu.edu
 Project-URL: Homepage, https://github.com/asu-trans-ai-lab/grid2demand
 Project-URL: Documentation, https://github.com/asu-trans-ai-lab/grid2demand
 Classifier: Programming Language :: Python :: 3
@@ -52,38 +52,31 @@
 ```python
 from __future__ import absolute_import
 import grid2demand as gd
 
 if __name__ == "__main__":
 
     # Specify input directory
-    path_node = "your-path-to-node.csv"
-    path_poi = "your-path-to-poi.csv"
+    input_dir = "your-data-folder"
 
     # Initialize a GRID2DEMAND object
-    net = gd.GRID2DEMAND(node_file = path_node, poi_file = path_poi)
+    net = gd.GRID2DEMAND(input_dir=input_dir)
 
     # load network: node and poi
     net.load_network()
 
     # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
     net.net2zone(num_x_blocks=10, num_y_blocks=10)
     # net.net2zone(cell_width=10, cell_height=10, unit="km")
 
-    # Synchronize geometry info between zone, node and poi
-    # if you want to save updated node, poi, zone without demand,
-    # you can skip net.run_gravity_model()
-    # and run net.save_results_to_csv(overwrite_file=True) directly
-    net.sync_geometry_between_zone_and_node_poi()
-
     # Calculate demand by running gravity model
     net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
-    net.save_results_to_csv(overwrite_file=True)
+    net.save_results_to_csv()
 ```
 
 # Generate Demand with node.csv, poi.csv and zone.csv (geometry filed in zone.csv)
 
 ```python
 from __future__ import absolute_import
 import grid2demand as gd
@@ -100,20 +93,14 @@
 
     # load network: node and poi
     net.load_network()
 
     # Generate zone
     net.taz2zone()
 
-    # Synchronize geometry info between zone, node and poi
-    # if you want to save updated node, poi, zone without demand,
-    # you can skip net.run_gravity_model()
-    # and run net.save_results_to_csv(overwrite_file=True) directly
-    net.sync_geometry_between_zone_and_node_poi()
-
     # Calculate demand by running gravity model
     net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
@@ -135,20 +122,14 @@
 
     # load network: node and poi
     net.load_network()
 
     # Generate zone
     net.taz2zone()
 
-    # Synchronize geometry info between zone, node and poi
-    # if you want to save updated node, poi, zone without demand,
-    # you can skip net.run_gravity_model()
-    # and run net.save_results_to_csv(overwrite_file=True) directly
-    net.sync_geometry_between_zone_and_node_poi()
-
     # Calculate demand by running gravity model
     net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
@@ -170,20 +151,14 @@
     # load network: node and poi
     net.load_network()
 
     # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
     net.net2zone(num_x_blocks=10, num_y_blocks=10)
     # net.net2zone(cell_width=10, cell_height=10, unit="km")
 
-    # Synchronize geometry info between zone, node and poi
-    # if you want to save updated node, poi, zone without demand,
-    # you can skip net.run_gravity_model()
-    # and run net.save_results_to_csv(overwrite_file=True) directly
-    net.sync_geometry_between_zone_and_node_poi()
-
     # Calculate demand by running gravity model
     net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
@@ -205,10 +180,9 @@
 
 For more information about the ways you can contribute to grid2demand, visit [our GitHub](https://github.com/asu-trans-ai-lab/grid2demand). If you' re unsure where to start or how your skills fit in, reach out! You can ask by opening a new issue or leaving a comment on a relevant issue that is already open on GitHub.
 
 ## Citing grid2demand
 
 If you use grid2demand in your research please use the following BibTeX entry:
 
-```cite
-Xiangyong Luo, Dustin Carlino, and Xuesong Simon Zhou. (2023). xyluo25/grid2demand: new lease to v0.4.1. Zenodo. https://doi.org/10.5281/zenodo.10899860
-```
+
+Xiangyong Luo, Dustin Carlino, and Xuesong Simon Zhou. (2023). [xyluo25/grid2demand](https://github.com/xyluo25/grid2demand/): Zenodo. https://doi.org/10.5281/zenodo.11212556
```

### Comparing `grid2demand-0.4.5/README.md` & `grid2demand-0.4.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 GRID2DEMAND: A tool for generating zone-to-zone travel demand based on grid cells or TAZs and gravity model
 
 - [**Grid2demand**](#grid2demand)
   - [**Code Examples**](#code-examples)
     - [**Installation**](#installation)
     - [**Simple Example**](#simple-example)
       - [**Generate Demand with node.csv and poi.csv**](#generate-demand-with-nodecsv-and-poicsv)
-      - [**Generate Demand with node.csv, poi.csv and zone.csv (geometry filed in zone.csv)**](#generate-demand-with-nodecsv-poicsv-and-zonecsv-geometry-filed-in-zonecsv)
-      - [**Generate Demand with node.csv, poi.csv and zone.csv (x\_coord, y\_coord fields represent zone centroids)**](#generate-demand-with-nodecsv-poicsv-and-zonecsv-x_coord-y_coord-fields-represent-zone-centroids)
-      - [**Generate Demand with node.csv (if zone\_id field exist, generated zone boundary cover zone\_id that are not empty) and poi.csv**](#generate-demand-with-nodecsv-if-zone_id-field-exist-generated-zone-boundary-cover-zone_id-that-are-not-empty-and-poicsv)
     - [**Call for Contributions**](#call-for-contributions)
     - [**Citing grid2demand**](#citing-grid2demand)
   - [**Starting with Grid2demand - Learning Sources**](#starting-with-grid2demand---learning-sources)
   - [**Introduction and Background Knowledge**](#introduction-and-background-knowledge)
     - [**4-step transportation forecasting**](#4-step-transportation-forecasting)
     - [**Productions and Attractions**](#productions-and-attractions)
     - [**Estimate Trip Productions/Attractions Using Trip Rates**](#estimate-trip-productionsattractions-using-trip-rates)
@@ -49,177 +46,62 @@
 ```python
 from __future__ import absolute_import
 import grid2demand as gd
 
 if __name__ == "__main__":
 
     # Specify input directory
-    path_node = "your-path-to-node.csv"
-    path_poi = "your-path-to-poi.csv"
+    input_dir = "your-data-folder"
 
     # Initialize a GRID2DEMAND object
-    net = gd.GRID2DEMAND(node_file = path_node, poi_file = path_poi)
+    net = gd.GRID2DEMAND(input_dir=input_dir)
 
     # load network: node and poi
     net.load_network()
 
     # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
     net.net2zone(num_x_blocks=10, num_y_blocks=10)
     # net.net2zone(cell_width=10, cell_height=10, unit="km")
 
-    # Synchronize geometry info between zone, node and poi
-    # if you want to save updated node, poi, zone without demand,
-    # you can skip net.run_gravity_model()
-    # and run net.save_results_to_csv(overwrite_file=True) directly
-    net.sync_geometry_between_zone_and_node_poi()
-
-    # Calculate demand by running gravity model
-    net.run_gravity_model()
-
-    # Save demand, zone, updated node, updated poi to csv
-    net.save_results_to_csv(overwrite_file=True)
-```
-
-#### **Generate Demand with node.csv, poi.csv and zone.csv (geometry filed in zone.csv)**
-
-```python
-from __future__ import absolute_import
-import grid2demand as gd
-
-if __name__ == "__main__":
-
-    # Specify input directory
-    path_node = "your-path-to-node.csv"
-    path_poi = "your-path-to-poi.csv"
-    path_zone = "your-path-to-zone.csv"  # zone_id, geometry are required columns
-
-    # Initialize a GRID2DEMAND object
-    net = gd.GRID2DEMAND(zone_file = path_zone, node_file = path_node, poi_file = path_poi)
-
-    # load network: node and poi
-    net.load_network()
-
-    # Generate zone
-    net.taz2zone()
-
-    # Synchronize geometry info between zone, node and poi
-    # if you want to save updated node, poi, zone without demand,
-    # you can skip net.run_gravity_model()
-    # and run net.save_results_to_csv(overwrite_file=True) directly
-    net.sync_geometry_between_zone_and_node_poi()
-
-    # Calculate demand by running gravity model
-    net.run_gravity_model()
-
-    # Save demand, zone, updated node, updated poi to csv
-    net.save_results_to_csv(overwrite_file=True)
-```
-
-#### **Generate Demand with node.csv, poi.csv and zone.csv (x_coord, y_coord fields represent zone centroids)**
-
-```python
-from __future__ import absolute_import
-import grid2demand as gd
-
-if __name__ == "__main__":
-
-    # Specify input directory
-    path_node = "your-path-to-node.csv"
-    path_poi = "your-path-to-poi.csv"
-    path_zone = "your-path-to-zone.csv"  # zone_id, x_coord, y_coord are required columns
-
-    # Initialize a GRID2DEMAND object
-    net = gd.GRID2DEMAND(zone_file = path_zone, node_file = path_node, poi_file = path_poi)
-
-    # load network: node and poi
-    net.load_network()
-
-    # Generate zone
-    net.taz2zone()
-
-    # Synchronize geometry info between zone, node and poi
-    # if you want to save updated node, poi, zone without demand,
-    # you can skip net.run_gravity_model()
-    # and run net.save_results_to_csv(overwrite_file=True) directly
-    net.sync_geometry_between_zone_and_node_poi()
-
     # Calculate demand by running gravity model
     net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
-    net.save_results_to_csv(overwrite_file=True)
-```
-
-#### **Generate Demand with node.csv (if zone_id field exist, generated zone boundary cover zone_id that are not empty) and poi.csv**
-
-```python
-from __future__ import absolute_import
-import grid2demand as gd
-
-if __name__ == "__main__":
-
-    # Specify input directory
-    path_node = "your-path-to-node.csv"  # make sure you have zone_id field in node.csv
-    path_poi = "your-path-to-poi.csv"
-
-    # Initialize a GRID2DEMAND object
-    net = gd.GRID2DEMAND(node_file = path_node, poi_file = path_poi, use_zone_id=True)
-
-    # load network: node and poi
-    net.load_network()
-
-    # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
-    net.net2zone(num_x_blocks=10, num_y_blocks=10)
-    # net.net2zone(cell_width=10, cell_height=10, unit="km")
-
-    # Synchronize geometry info between zone, node and poi
-    # if you want to save updated node, poi, zone without demand,
-    # you can skip net.run_gravity_model()
-    # and run net.save_results_to_csv(overwrite_file=True) directly
-    net.sync_geometry_between_zone_and_node_poi()
-
-    # Calculate demand by running gravity model
-    net.run_gravity_model()
-
-    # Save demand, zone, updated node, updated poi to csv
-    net.save_results_to_csv(overwrite_file=True)
+    net.save_results_to_csv()
 ```
 
 ### **Call for Contributions**
 
 The grid2demand project welcomes your expertise and enthusiasm!
 
 Small improvements or fixes are always appreciated. If you are considering larger contributions to the source code, please contact us through email: [Xiangyong Luo](mailto:luoxiangyong01@gmail.com), [Dr. Xuesong Simon Zhou](mailto:xzhou74@asu.edu)
 
 Writing code isn't the only way to contribute to grid2demand. You can also:
-   * review pull requests
-   * help us stay on top of new and old issues
-   * develop tutorials, presentations, and other educational materials
-   * develop graphic design for our brand assets and promotional materials
-   * translate website content
-   * help with outreach and onboard new contributors
-   * write grant proposals and help with other fundraising efforts
+
+- review pull requests
+- help us stay on top of new and old issues
+- develop tutorials, presentations, and other educational materials
+- develop graphic design for our brand assets and promotional materials
+- translate website content
+- help with outreach and onboard new contributors
+- write grant proposals and help with other fundraising efforts
 
 For more information about the ways you can contribute to grid2demand, visit [our GitHub](https://github.com/asu-trans-ai-lab/grid2demand). If you' re unsure where to start or how your skills fit in, reach out! You can ask by opening a new issue or leaving a comment on a relevant issue that is already open on GitHub.
 
 ### **Citing grid2demand**
 
 If you use grid2demand in your research please use the following BibTeX entry:
 
-```cite
-Xiangyong Luo, Dustin Carlino, and Xuesong Simon Zhou. (2023). xyluo25/grid2demand: new lease to v0.4.1. Zenodo. https://doi.org/10.5281/zenodo.10899860
-```
-
-
+Xiangyong Luo, Dustin Carlino, and Xuesong Simon Zhou. (2023). [xyluo25/grid2demand](https://github.com/xyluo25/grid2demand/): Zenodo. https://doi.org/10.5281/zenodo.11212556
 
 ## **Starting with Grid2demand - Learning Sources**
 
--   How to quickly generate **initial origin-destination transportation demand** for engaging traffic simulation games such as A/B street and DTALite?
--   How to teach our undergraduate students the important **trip generation and trip distribution steps**, using their own beautiful campus as examples?
--   How to analyze the resident locations and other land use properties using flexible **grid zones, based on POI data from OpenStreetMap** data and using **open transportation modeling format**
+- How to quickly generate **initial origin-destination transportation demand** for engaging traffic simulation games such as A/B street and DTALite?
+- How to teach our undergraduate students the important **trip generation and trip distribution steps**, using their own beautiful campus as examples?
+- How to analyze the resident locations and other land use properties using flexible **grid zones, based on POI data from OpenStreetMap** data and using **open transportation modeling format**
 
 <img src="docs/media/9ed9631f17469d631f9dfe97e4320c10.png" style="zoom:80%;" />
 
 If you have not used Grid2demand before, here are some advices to get started.
 
 1. Read the user guide or watch the video at https://www.youtube.com/watch?v=EfjCERQQGTs.
 
@@ -246,15 +128,15 @@
 ([https://github.com/asu-trans-ai-lab/grid2demand](https://github.com/asu-trans-ai-lab/grid2demand)). The Jupyter notebook example can be found at
 [https://github.com/asu-trans-ai-lab/grid2demand/blob/main/grid2demand.ipynb](https://github.com/asu-trans-ai-lab/grid2demand/blob/main/grid2demand_tutorial.ipynb), which is also accessible through Google Colab.
 
 Mini teaching lesson: [https://www.youtube.com/watch?v=EfjCERQQGTs](https://www.youtube.com/watch?v=EfjCERQQGTs)
 
 ## **Introduction and Background Knowledge**
 
-###  **4-step transportation forecasting**
+### **4-step transportation forecasting**
 
 Trip generation and trip distribution are the first 2 steps in the larger context of the 4-step process in transportation planning. The standard four steps are briefly described below.
 
 - Trip Generation: Estimate how many trips enter or leave a zone/traffic-analysis-zone (TAZ)
 - Trip Distribution: Estimate how many trips from each zone/TAZ end in all zones/TAZs
 - Mode Choice: Estimate which travel-method is used (e.g., vehicle, transit, walk) to complete those trips
 - Traffic Assignment: Distribute vehicles/traffic flow to different paths during travel
```

### Comparing `grid2demand-0.4.5/grid2demand/__init__.py` & `grid2demand-0.4.6/grid2demand/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                                 calc_zone_od_matrix)
 from .func_lib.gravity_model import (run_gravity_model,
                                      calc_zone_production_attraction)
 from .func_lib.gen_agent_demand import gen_agent_based_demand
 from .utils_lib.pkg_settings import pkg_settings
 from ._grid2demand import GRID2DEMAND
 
-print('grid2demand, version 0.4.5')
+print('grid2demand, version 0.4.6')
 print("Python version for running the model is 3.10 or higher")
 
 
 __all__ = ["read_node", "read_poi", "read_network",
            "read_zone_by_geometry", "read_zone_by_centroid",
            "gen_poi_trip_rate", "gen_node_prod_attr",
            "net2zone",
```

### Comparing `grid2demand-0.4.5/grid2demand/_grid2demand.py` & `grid2demand-0.4.6/grid2demand/_grid2demand.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,18 @@
             self.output_dir = self.input_dir
         else:
             self.output_dir = path2linux(os.getcwd())
 
         self.verbose = verbose
         self.use_zone_id = use_zone_id
 
+        # load default package settings,
+        # user can modify the settings before running the model
+        self.__load_pkg_settings()
+
         # if use_zone_id is True, this parameter will be implemented
         self.node_as_zone_centroid = node_as_zone_centroid
 
         # # check input directory if specified input directory
         if self.input_dir:
             self.__check_input_dir()
 
@@ -120,18 +124,15 @@
         self.is_centroid = False
 
         # set default poi_trip_rate, node_prod_attr, zone_prod_attr as False
         self.is_poi_trip_rate = False
         self.is_node_prod_attr = False
         self.is_zone_prod_attr = False
         self.is_zone_od_dist_matrix = False
-
-        # load default package settings,
-        # user can modify the settings before running the model
-        self.__load_pkg_settings()
+        self.is_sync_geometry = False
 
     def __check_input_dir(self) -> None:
         """check input directory
 
         Raises:
             NotADirectoryError: Error: Input directory _input_dir_ does not exist.
             Exception: Error: Required files are not satisfied. Please check _required_files_ in _input_dir_.
@@ -555,14 +556,15 @@
         #     self.poi_dict = zone_poi_dict.get('poi_dict')
         # except Exception as e:
         #     raise Exception(
         #         f"Error in running {self.sync_geometry_between_zone_and_node_poi.__name__}: \
         #           not valid zone_dict or poi_dict"
         #     ) from e
 
+        self.is_sync_geometry = True
         return {"zone_dict": self.zone_dict,
                 "node_dict": self.node_dict,
                 "poi_dict": self.poi_dict} if return_value else None
 
     def calc_zone_od_distance_matrix(self, zone_dict: dict = "", return_value: bool = False) -> dict[tuple, float]:
         """calculate zone-to-zone od distance matrix
 
@@ -752,14 +754,18 @@
         if alpha:
             self.alpha = alpha
         if beta:
             self.beta = beta
         if gamma:
             self.gamma = gamma
 
+        # synchronize geometry between zone and node/poi
+        if not self.is_sync_geometry:
+            self.sync_geometry_between_zone_and_node_poi()
+
         # calculate zone production and attraction based on node production and attraction
         if not self.is_zone_prod_attr:
             self.calc_zone_prod_attr(zone_dict=self.zone_dict,
                                      node_dict=self.node_dict,
                                      poi_dict=self.poi_dict,
                                      trip_rate_file=self.trip_rate_file,
                                      trip_purpose=self.trip_purpose)
@@ -927,14 +933,16 @@
                 # update node data if centroid is used, ignore zone_id if original zone_id is empty
                 if self.is_centroid:
                     for i in range(len(node_df)):
                         original_zone_id = node_df.loc[i, "_zone_id"]
                         if original_zone_id == -1:
                             node_df.loc[i, "zone_id"] = None
 
+                # change column name from id to node_id
+                node_df.rename(columns={"id": "node_id"}, inplace=True)
                 node_df.to_csv(path_output, index=False)
                 print(f"  : Successfully saved updated node to node.csv to {self.output_dir}")
 
         if poi:
             # specify output path
             if overwrite_file:
                 path_output = path2linux(os.path.join(self.output_dir, "poi.csv"))
@@ -942,14 +950,17 @@
                 path_output = generate_unique_filename(path2linux(os.path.join(self.output_dir, "poi.csv")))
 
             # check if poi_dict exists
             if not hasattr(self, "poi_dict"):
                 print("  : Could not save updated poi file: poi_dict does not exist. Please run load_poi() first.")
             else:
                 poi_df = pd.DataFrame(self.poi_dict.values())
+
+                # rename column name from id to poi_id
+                poi_df.rename(columns={"id": "poi_id"}, inplace=True)
                 poi_df.to_csv(path_output, index=False)
                 print(f"  : Successfully saved updated poi to poi.csv to {self.output_dir}")
 
         if zone_od_dist_table:
             # specify output path
             if overwrite_file:
                 path_output = path2linux(os.path.join(self.output_dir, "zone_od_dist_table.csv"))
```

### Comparing `grid2demand-0.4.5/grid2demand/func_lib/gen_agent_demand.py` & `grid2demand-0.4.6/grid2demand/func_lib/gen_agent_demand.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.5/grid2demand/func_lib/gen_zone.py` & `grid2demand-0.4.6/grid2demand/func_lib/gen_zone.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.5/grid2demand/func_lib/gravity_model.py` & `grid2demand-0.4.6/grid2demand/func_lib/gravity_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 
 
 def calc_zone_production_attraction(node_dict: dict, zone_dict: dict, verbose: bool = False) -> dict:
     # calculate zone production and attraction based on node production and attraction
     for zone_name in zone_dict:
         if zone_dict[zone_name].node_id_list:
             for node_id in zone_dict[zone_name].node_id_list:
-                zone_dict[zone_name].production += node_dict[node_id].production
-                zone_dict[zone_name].attraction += node_dict[node_id].attraction
+                try:
+                    zone_dict[zone_name].production += node_dict[node_id].production
+                    zone_dict[zone_name].attraction += node_dict[node_id].attraction
+                except KeyError:
+                    continue
 
     if verbose:
         print("  : Successfully calculated zone production and attraction based on node production and attraction.")
 
     return zone_dict
```

### Comparing `grid2demand-0.4.5/grid2demand/func_lib/read_node_poi.py` & `grid2demand-0.4.6/grid2demand/func_lib/read_node_poi.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             except Exception:
                 _zone_id = -1
 
             node = Node(
                 id=df_node.loc[i, 'node_id'],
                 activity_type=activity_type,
                 activity_location_tab=activity_location_tab,
+                ctrl_type=df_node.loc[i, 'ctrl_type'],
                 x_coord=df_node.loc[i, 'x_coord'],
                 y_coord=df_node.loc[i, 'y_coord'],
                 poi_id=df_node.loc[i, 'poi_id'],
                 boundary_flag=boundary_flag,
                 geometry=shapely.Point(df_node.loc[i, 'x_coord'], df_node.loc[i, 'y_coord']),
                 _zone_id=_zone_id
             )
@@ -232,20 +233,22 @@
     # read node.csv with specified columns and chunksize for iterations
     node_required_cols = pkg_settings["node_fields"]
     chunk_size = pkg_settings["data_chunk_size"]
 
     # read first two rows to check whether required fields are in node.csv
     df_node_2rows = pd.read_csv(node_file, nrows=2)
     col_names = df_node_2rows.columns.tolist()
+
     if "zone_id" in col_names:
         node_required_cols.append("zone_id")
 
     if verbose:
         print(f"  : Reading node.csv with specified columns: {node_required_cols} \
                     \n    and chunksize {chunk_size} for iterations...")
+
     df_node_chunk = pd.read_csv(node_file, usecols=node_required_cols, chunksize=chunk_size)
 
     if verbose:
         print(f"  : Parallel creating Nodes using Pool with {cpu_cores} CPUs. Please wait...")
     node_dict_final = {}
 
     # Parallel processing using Pool
@@ -296,15 +299,18 @@
     # Read poi.csv with specified columns and chunksize for iterations
     poi_required_cols = pkg_settings["poi_fields"]
     chunk_size = pkg_settings["data_chunk_size"]
 
     if verbose:
         print(f"  : Reading poi.csv with specified columns: {poi_required_cols} \
                     \n    and chunksize {chunk_size} for iterations...")
-    df_poi_chunk = pd.read_csv(poi_file, usecols=poi_required_cols, chunksize=chunk_size)
+    try:
+        df_poi_chunk = pd.read_csv(poi_file, usecols=poi_required_cols, chunksize=chunk_size, encoding='utf-8')
+    except Exception:
+        df_poi_chunk = pd.read_csv(poi_file, usecols=poi_required_cols, chunksize=chunk_size, encoding='latin-1')
 
     # Parallel processing using Pool
     if verbose:
         print(f"  : Parallel creating POIs using Pool with {cpu_cores} CPUs. Please wait...")
     poi_dict_final = {}
 
     with Pool(cpu_cores) as pool:
```

### Comparing `grid2demand-0.4.5/grid2demand/func_lib/trip_rate_production_attraction.py` & `grid2demand-0.4.6/grid2demand/func_lib/trip_rate_production_attraction.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.5/grid2demand/utils_lib/net_utils.py` & `grid2demand-0.4.6/grid2demand/utils_lib/net_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,19 +26,20 @@
         activity_type: The activity type of the node. provided from osm2gmns such as motoway, residential, ...
         activity_location_tab: The activity location tab of the node.
         geometry: The geometry of the node. based on wkt format.
         _zone_id: The zone ID. default == -1,
                 this will be assigned if field zone_id exists in the node.csv and is not empty
     """
     id: int = 0
-    x_coord: float = 0
-    y_coord: float = 0
+    x_coord: float = -1
+    y_coord: float = -1
     production: float = 0
     attraction: float = 0
     boundary_flag: int = 0
+    ctrl_type: int = -1
     zone_id: int = -1
     poi_id: int = -1
     activity_type: str = ''
     activity_location_tab: str = ''
     geometry: str = ''
     _zone_id: int = -1
```

### Comparing `grid2demand-0.4.5/grid2demand/utils_lib/pkg_settings.py` & `grid2demand-0.4.6/grid2demand/utils_lib/pkg_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 pkg_settings = {
     # specify required files for grid2demand, and optional files for grid2demand
     "required_files": ["node.csv", "poi.csv"],
     "optional_files": ["zone.csv"],
 
     # specify required fields for node.csv and poi.csv and zone.csv (optional)
     "node_fields": ["node_id", "x_coord", "y_coord",
-                    "activity_type", "is_boundary", "poi_id"],
+                    "activity_type", "is_boundary", "ctrl_type", "poi_id"],
     "poi_fields": ["poi_id", "building", "centroid", "area", "geometry"],
     "zone_geometry_fields": ["zone_id", "geometry"],
     "zone_centroid_fields": ["zone_id", "x_coord", "y_coord"],
 
     # if input data is too large, you can split the input data into chunks and process them separately
     "data_chunk_size": 10000,
```

### Comparing `grid2demand-0.4.5/grid2demand/utils_lib/utils.py` & `grid2demand-0.4.6/grid2demand/utils_lib/utils.py`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.5/grid2demand.egg-info/PKG-INFO` & `grid2demand-0.4.6/grid2demand.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grid2demand
-Version: 0.4.5
+Version: 0.4.6
 Summary: A tool for generating zone-to-zone travel demand based on grid cells or TAZs and gravity model
 Home-page: https://github.com/xyluo25/grid2demand
 Author: Xiangyong Luo, Dr.Xuesong(Simon) Zhou
 Author-email: luoxiangyong01@gmail.com, xzhou74@asu.edu
 Project-URL: Homepage, https://github.com/asu-trans-ai-lab/grid2demand
 Project-URL: Documentation, https://github.com/asu-trans-ai-lab/grid2demand
 Classifier: Programming Language :: Python :: 3
@@ -52,38 +52,31 @@
 ```python
 from __future__ import absolute_import
 import grid2demand as gd
 
 if __name__ == "__main__":
 
     # Specify input directory
-    path_node = "your-path-to-node.csv"
-    path_poi = "your-path-to-poi.csv"
+    input_dir = "your-data-folder"
 
     # Initialize a GRID2DEMAND object
-    net = gd.GRID2DEMAND(node_file = path_node, poi_file = path_poi)
+    net = gd.GRID2DEMAND(input_dir=input_dir)
 
     # load network: node and poi
     net.load_network()
 
     # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
     net.net2zone(num_x_blocks=10, num_y_blocks=10)
     # net.net2zone(cell_width=10, cell_height=10, unit="km")
 
-    # Synchronize geometry info between zone, node and poi
-    # if you want to save updated node, poi, zone without demand,
-    # you can skip net.run_gravity_model()
-    # and run net.save_results_to_csv(overwrite_file=True) directly
-    net.sync_geometry_between_zone_and_node_poi()
-
     # Calculate demand by running gravity model
     net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
-    net.save_results_to_csv(overwrite_file=True)
+    net.save_results_to_csv()
 ```
 
 # Generate Demand with node.csv, poi.csv and zone.csv (geometry filed in zone.csv)
 
 ```python
 from __future__ import absolute_import
 import grid2demand as gd
@@ -100,20 +93,14 @@
 
     # load network: node and poi
     net.load_network()
 
     # Generate zone
     net.taz2zone()
 
-    # Synchronize geometry info between zone, node and poi
-    # if you want to save updated node, poi, zone without demand,
-    # you can skip net.run_gravity_model()
-    # and run net.save_results_to_csv(overwrite_file=True) directly
-    net.sync_geometry_between_zone_and_node_poi()
-
     # Calculate demand by running gravity model
     net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
@@ -135,20 +122,14 @@
 
     # load network: node and poi
     net.load_network()
 
     # Generate zone
     net.taz2zone()
 
-    # Synchronize geometry info between zone, node and poi
-    # if you want to save updated node, poi, zone without demand,
-    # you can skip net.run_gravity_model()
-    # and run net.save_results_to_csv(overwrite_file=True) directly
-    net.sync_geometry_between_zone_and_node_poi()
-
     # Calculate demand by running gravity model
     net.run_gravity_model()
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
@@ -170,20 +151,14 @@
     # load network: node and poi
     net.load_network()
 
     # Generate zone dictionary from node dictionary by specifying number of x blocks and y blocks
     net.net2zone(num_x_blocks=10, num_y_blocks=10)
     # net.net2zone(cell_width=10, cell_height=10, unit="km")
 
-    # Synchronize geometry info between zone, node and poi
-    # if you want to save updated node, poi, zone without demand,
-    # you can skip net.run_gravity_model()
-    # and run net.save_results_to_csv(overwrite_file=True) directly
-    net.sync_geometry_between_zone_and_node_poi()
-
     # Calculate demand by running gravity model
     net.run_gravity_model(zone_prod_attr, zone_od_distance_matrix)
 
     # Save demand, zone, updated node, updated poi to csv
     net.save_results_to_csv(overwrite_file=True)
 ```
 
@@ -205,10 +180,9 @@
 
 For more information about the ways you can contribute to grid2demand, visit [our GitHub](https://github.com/asu-trans-ai-lab/grid2demand). If you' re unsure where to start or how your skills fit in, reach out! You can ask by opening a new issue or leaving a comment on a relevant issue that is already open on GitHub.
 
 ## Citing grid2demand
 
 If you use grid2demand in your research please use the following BibTeX entry:
 
-```cite
-Xiangyong Luo, Dustin Carlino, and Xuesong Simon Zhou. (2023). xyluo25/grid2demand: new lease to v0.4.1. Zenodo. https://doi.org/10.5281/zenodo.10899860
-```
+
+Xiangyong Luo, Dustin Carlino, and Xuesong Simon Zhou. (2023). [xyluo25/grid2demand](https://github.com/xyluo25/grid2demand/): Zenodo. https://doi.org/10.5281/zenodo.11212556
```

### Comparing `grid2demand-0.4.5/grid2demand.egg-info/SOURCES.txt` & `grid2demand-0.4.6/grid2demand.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grid2demand-0.4.5/setup.py` & `grid2demand-0.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     with open("requirements.txt", "r", encoding="utf-8") as f:
         modules_needed = [i.strip() for i in f.readlines()]
 except Exception:
     modules_needed = []
 
 setuptools.setup(
     name="grid2demand",  # Replace with your own username
-    version="0.4.5",
+    version="0.4.6",
     author="Xiangyong Luo, Dr.Xuesong(Simon) Zhou",
     author_email="luoxiangyong01@gmail.com, xzhou74@asu.edu",
     description="A tool for generating zone-to-zone travel demand based on grid cells or TAZs and gravity model",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xyluo25/grid2demand",
```

### Comparing `grid2demand-0.4.5/tests/test_read_node.py` & `grid2demand-0.4.6/tests/test_read_node.py`

 * *Files identical despite different names*

