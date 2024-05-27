# Comparing `tmp/mosstool-0.1.0.tar.gz` & `tmp/mosstool-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosstool-0.1.0.tar", max compression
+gzip compressed data, was "mosstool-0.2.0.tar", max compression
```

## Comparing `mosstool-0.1.0.tar` & `mosstool-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0      219 2024-05-17 07:23:44.382163 mosstool-0.1.0/README.md
--rw-r--r--   0        0        0      268 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/__init__.py
--rw-r--r--   0        0        0    16340 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/_map_util/add_aoi_pop.py
--rw-r--r--   0        0        0    70559 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/_map_util/aoi_matcher.py
--rw-r--r--   0        0        0    16237 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/_map_util/aoiutils.py
--rw-r--r--   0        0        0     2956 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/_map_util/const.py
--rw-r--r--   0        0        0    11404 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/_map_util/convert_aoi.py
--rw-r--r--   0        0        0    16609 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/_map_util/format_checker.py
--rw-r--r--   0        0        0    21033 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/_map_util/gen_traffic_light.py
--rw-r--r--   0        0        0     1155 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/_map_util/osm_const.py
--rw-r--r--   0        0        0        0 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/_util/__init__.py
--rw-r--r--   0        0        0      444 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/_util/angle.py
--rw-r--r--   0        0        0     3626 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/_util/bezier.py
--rw-r--r--   0        0        0    12436 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/_util/line.py
--rw-r--r--   0        0        0      100 2024-05-17 07:23:45.038164 mosstool-0.1.0/mosstool/map/builder/__init__.py
--rw-r--r--   0        0        0   204550 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/builder/builder.py
--rw-r--r--   0        0        0      185 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/osm/__init__.py
--rw-r--r--   0        0        0     7162 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/osm/_motif.py
--rw-r--r--   0        0        0     2643 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/osm/_wayutil.py
--rw-r--r--   0        0        0    14567 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/osm/building.py
--rw-r--r--   0        0        0    28323 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/osm/roadnet.py
--rw-r--r--   0        0        0      373 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/public_transport/__init__.py
--rw-r--r--   0        0        0    12458 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/public_transport/get_bus.py
--rw-r--r--   0        0        0    12224 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/public_transport/get_subway.py
--rw-r--r--   0        0        0    21211 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/public_transport/get_transitland.py
--rw-r--r--   0        0        0    16145 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/public_transport/public_transport_post.py
--rw-r--r--   0        0        0       92 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/sumo/__init__.py
--rw-r--r--   0        0        0    37747 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/sumo/map.py
--rw-r--r--   0        0        0       79 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/vis/__init__.py
--rw-r--r--   0        0        0     9999 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/map/vis/map.py
--rw-r--r--   0        0        0       36 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/__init__.py
--rw-r--r--   0        0        0      758 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/generator/AIGC.py
--rw-r--r--   0        0        0      347 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/generator/__init__.py
--rw-r--r--   0        0        0      621 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/generator/_util/const.py
--rw-r--r--   0        0        0      406 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/generator/_util/utils.py
--rw-r--r--   0        0        0    18367 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/generator/generate_from_od.py
--rw-r--r--   0        0        0     3774 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/generator/gravity.py
--rw-r--r--   0        0        0     5190 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/generator/random.py
--rw-r--r--   0        0        0      702 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/generator/template.py
--rw-r--r--   0        0        0      119 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/route/__init__.py
--rw-r--r--   0        0        0     2105 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/route/client.py
--rw-r--r--   0        0        0     3398 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/route/preroute.py
--rw-r--r--   0        0        0      100 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/sumo/__init__.py
--rw-r--r--   0        0        0    37589 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/sumo/route.py
--rw-r--r--   0        0        0       78 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/vis/__init__.py
--rw-r--r--   0        0        0     8307 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/trip/vis/trip.py
--rw-r--r--   0        0        0      783 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/type/__init__.py
--rw-r--r--   0        0        0       22 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/util/__init__.py
--rw-r--r--   0        0        0      481 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/util/color.py
--rw-r--r--   0        0        0     4519 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/util/format_converter.py
--rw-r--r--   0        0        0    14922 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/util/geo_match_pop.py
--rw-r--r--   0        0        0     2039 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/util/map_merger.py
--rw-r--r--   0        0        0     6538 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/util/map_splitter.py
--rw-r--r--   0        0        0        0 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/util/test/__init__.py
--rw-r--r--   0        0        0      194 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/util/test/test_color.py
--rw-r--r--   0        0        0     1150 2024-05-17 07:23:45.042164 mosstool-0.1.0/mosstool/util/test/test_format_conveter.py
--rw-r--r--   0        0        0      853 2024-05-17 07:23:45.046164 mosstool-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 mosstool-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-27 09:17:14.447507 mosstool-0.2.0/README.md
+-rw-r--r--   0        0        0      268 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/__init__.py
+-rw-r--r--   0        0        0    16340 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/add_aoi_pop.py
+-rw-r--r--   0        0        0    70559 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/aoi_matcher.py
+-rw-r--r--   0        0        0    16237 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/aoiutils.py
+-rw-r--r--   0        0        0     2956 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/const.py
+-rw-r--r--   0        0        0    11404 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/convert_aoi.py
+-rw-r--r--   0        0        0    16609 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/format_checker.py
+-rw-r--r--   0        0        0    21033 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/gen_traffic_light.py
+-rw-r--r--   0        0        0     2045 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/map_aois_matchers.py
+-rw-r--r--   0        0        0     1155 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_map_util/osm_const.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_util/__init__.py
+-rw-r--r--   0        0        0      444 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_util/angle.py
+-rw-r--r--   0        0        0     3626 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_util/bezier.py
+-rw-r--r--   0        0        0    12436 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/_util/line.py
+-rw-r--r--   0        0        0      100 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/builder/__init__.py
+-rw-r--r--   0        0        0   206163 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/builder/builder.py
+-rw-r--r--   0        0        0      185 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/osm/__init__.py
+-rw-r--r--   0        0        0     7162 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/osm/_motif.py
+-rw-r--r--   0        0        0     2643 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/osm/_wayutil.py
+-rw-r--r--   0        0        0    14567 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/osm/building.py
+-rw-r--r--   0        0        0    28323 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/osm/roadnet.py
+-rw-r--r--   0        0        0      373 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/public_transport/__init__.py
+-rw-r--r--   0        0        0    12458 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/public_transport/get_bus.py
+-rw-r--r--   0        0        0    12224 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/public_transport/get_subway.py
+-rw-r--r--   0        0        0    21211 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/public_transport/get_transitland.py
+-rw-r--r--   0        0        0    16145 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/public_transport/public_transport_post.py
+-rw-r--r--   0        0        0       92 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/sumo/__init__.py
+-rw-r--r--   0        0        0    37747 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/sumo/map.py
+-rw-r--r--   0        0        0       79 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/vis/__init__.py
+-rw-r--r--   0        0        0     9999 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/map/vis/map.py
+-rw-r--r--   0        0        0       36 2024-05-27 09:17:15.103513 mosstool-0.2.0/mosstool/trip/__init__.py
+-rw-r--r--   0        0        0      758 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/AIGC.py
+-rw-r--r--   0        0        0      347 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/__init__.py
+-rw-r--r--   0        0        0      621 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/_util/const.py
+-rw-r--r--   0        0        0      406 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/_util/utils.py
+-rw-r--r--   0        0        0    18572 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/generate_from_od.py
+-rw-r--r--   0        0        0     3774 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/gravity.py
+-rw-r--r--   0        0        0     5190 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/random.py
+-rw-r--r--   0        0        0      702 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/generator/template.py
+-rw-r--r--   0        0        0      119 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/route/__init__.py
+-rw-r--r--   0        0        0     2105 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/route/client.py
+-rw-r--r--   0        0        0     3398 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/route/preroute.py
+-rw-r--r--   0        0        0      100 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/sumo/__init__.py
+-rw-r--r--   0        0        0    37589 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/sumo/route.py
+-rw-r--r--   0        0        0       78 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/vis/__init__.py
+-rw-r--r--   0        0        0     8307 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/trip/vis/trip.py
+-rw-r--r--   0        0        0      783 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/type/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/__init__.py
+-rw-r--r--   0        0        0      481 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/color.py
+-rw-r--r--   0        0        0     4519 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/format_converter.py
+-rw-r--r--   0        0        0    14922 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/geo_match_pop.py
+-rw-r--r--   0        0        0     2039 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/map_merger.py
+-rw-r--r--   0        0        0     6538 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/map_splitter.py
+-rw-r--r--   0        0        0        0 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/test/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/test/test_color.py
+-rw-r--r--   0        0        0     1150 2024-05-27 09:17:15.107514 mosstool-0.2.0/mosstool/util/test/test_format_conveter.py
+-rw-r--r--   0        0        0      853 2024-05-27 09:17:15.107514 mosstool-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 mosstool-0.2.0/PKG-INFO
```

### Comparing `mosstool-0.1.0/mosstool/map/_map_util/add_aoi_pop.py` & `mosstool-0.2.0/mosstool/map/_map_util/add_aoi_pop.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/_map_util/aoi_matcher.py` & `mosstool-0.2.0/mosstool/map/_map_util/aoi_matcher.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/_map_util/aoiutils.py` & `mosstool-0.2.0/mosstool/map/_map_util/aoiutils.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/_map_util/const.py` & `mosstool-0.2.0/mosstool/map/_map_util/const.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/_map_util/convert_aoi.py` & `mosstool-0.2.0/mosstool/map/_map_util/convert_aoi.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/_map_util/format_checker.py` & `mosstool-0.2.0/mosstool/map/_map_util/format_checker.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/_map_util/gen_traffic_light.py` & `mosstool-0.2.0/mosstool/map/_map_util/gen_traffic_light.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/_map_util/osm_const.py` & `mosstool-0.2.0/mosstool/map/_map_util/osm_const.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/_util/bezier.py` & `mosstool-0.2.0/mosstool/map/_util/bezier.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/_util/line.py` & `mosstool-0.2.0/mosstool/map/_util/line.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/builder/builder.py` & `mosstool-0.2.0/mosstool/map/builder/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from .._map_util.aoi_matcher import add_aoi_to_map
 from .._map_util.aoiutils import generate_aoi_poi
 from .._map_util.const import *
 from .._map_util.convert_aoi import convert_aoi, convert_poi
 from .._map_util.format_checker import (geojson_format_check,
                                         output_format_check)
 from .._map_util.gen_traffic_light import generate_traffic_light
+from .._map_util.map_aois_matchers import match_map_aois
 from .._util.angle import abs_delta_angle, delta_angle
 from .._util.line import (align_line, connect_line_string, get_line_angle,
                           get_start_vector, line_extend, line_max_curvature,
                           merge_line_start_end, offset_lane)
 
 __all__ = ["Builder"]
 
@@ -44,14 +45,15 @@
 
     def __init__(
         self,
         net: Union[FeatureCollection, Map],
         proj_str: str,
         aois: Optional[FeatureCollection] = None,
         pois: Optional[FeatureCollection] = None,
+        reuse_map: Optional[Map] = None,
         public_transport: Optional[Dict[str, List]] = None,
         pop_tif_path: Optional[str] = None,
         landuse_shp_path: Optional[str] = None,
         traffic_light_min_direction_group: int = 3,
         default_lane_width: float = 3.2,
         gen_sidewalk_speed_limit: float = 0,
         expand_roads: bool = False,
@@ -63,14 +65,15 @@
     ):
         """
         Args:
         - net (FeatureCollection | Map): road network
         - proj_str (str): projection string
         - aois (FeatureCollection): area of interest
         - pois (FeatureCollection): point of interest
+        - reuse_map (Map): aoi and poi of this Map will be reused
         - public_transport (Dict[str, List]): public transports in json format
         - pop_tif_path (str): path to population tif file
         - landuse_shp_path (str): path to landuse shape file
         - traffic_light_min_direction_group (int): minimum number of lane directions for traffic-light generation
         - default_lane_width (float): default lane width
         - gen_sidewalk_speed_limit (float): speed limit to generate sidewalk
         - expand_roads (bool): expand roads according to junction type
@@ -96,14 +99,15 @@
         self.public_transport_uid = PUBLIC_LINE_START_ID
         self.proj_str = proj_str
         self.projector = pyproj.Proj(proj_str)
         self.pop_tif_path = pop_tif_path
         self.landuse_shp_path = landuse_shp_path
         self.traffic_light_min_direction_group = traffic_light_min_direction_group
         self.strict_mode = strict_mode
+        self.reuse_map = reuse_map
         self.workers = workers
         # id mapping relationship
         self.uid_mapping = {}
         """
         Intersection category: (in_cluster, out_cluster) -> []jid
         The junctions that have been processed are deleted from here.
         """
@@ -178,14 +182,15 @@
                     self.uid_mapping[feature["uid"]] = feature["id"]
                 elif feature["geometry"]["type"] == "LineString":
                     self.ways[feature["id"]] = feature
                     self.uid_mapping[feature["uid"]] = feature["id"]
             self.junction_types = defaultdict(list)
         elif net_type == Map:
             logging.info("Reading from pb files")
+            self.net = net
             self.from_pb = True
             # map_lanes & lane2data
             for l in net.lanes:
                 line = LineString([[n.x, n.y, n.z] for n in l.center_line.nodes])
                 l_id = l.id
                 self.map_lanes[l_id] = line
                 self.lane2data[line] = {
@@ -3916,14 +3921,57 @@
                 line_id += 1
 
         self.public_transport_data = {
             "lines": lines,
             "stations": stations,
         }
         return public_road_uids
+    def _reuse_aoi(self):
+        """Match aoi to road network"""
+        d_right_lanes = [
+            w["lanes"][-1]
+            for w in self.map_roads.values()
+            if w["lanes"]
+        ]
+        d_matcher = [
+            {
+                "id": self.lane2data[geo]["uid"],
+                "geo": geo,
+                # middle point
+                "point": geo.interpolate(0.5, normalized=True).coords[:][0],
+                "length": geo.length,
+            }
+            for geo in d_right_lanes
+        ]
+        w_lanes = [
+            l
+            for l, d in self.lane2data.items()
+            if d["type"] == mapv2.LANE_TYPE_WALKING
+        ]
+        w_matcher = [
+            {
+                "id": self.lane2data[geo]["uid"],
+                "geo": geo,
+                "point": geo.interpolate(0.5, normalized=True).coords[:][0],
+                "length": geo.length,
+            }
+            for geo in w_lanes
+        ]
+        logging.info("Reusing AOIs")
+        matchers = {
+            "drive": d_matcher,
+            "walk": w_matcher,
+        }
+        reuse_map = cast(Map,self.reuse_map)
+        (self.map_aois, self.map_pois) = match_map_aois(
+            net = reuse_map,
+            matchers=matchers,
+            workers=self.workers
+        )
+        
 
     def _add_aoi(self):
         """Match aoi to road network"""
         public_road_uids = self._add_public_transport()
         aois, stops = convert_aoi(
             self.raw_aois, self.public_transport_data, self.proj_str
         )
@@ -4052,15 +4100,15 @@
         public_lines = self.public_transport_data["lines"]
         public_stations = self.public_transport_data["stations"]
         # output aoi
         logging.info("Making output aois")
         self.output_aois = {}
         for uid, d in self.map_aois.items():
             # d["name"] = "" # The specific name of the AOI needs to be obtained by running patcher. The default is an empty string.
-            external = d["external"]
+            external = d.get("external",{})
             if "stop_id" in external:
                 station_type = external["station_type"]
                 stop_id = external["stop_id"]
                 sta = public_stations[station_type][stop_id]
                 sta["aoi_uid"] = uid
                 d["name"] = sta["name"]
                 if not "duration" in external:
@@ -4254,15 +4302,18 @@
             self._classify()
             self._classify_main_way_ids()  # Identify main and auxiliary roads before connecting to the road network for road shortening
             self._create_junction_for_1_n()
             self._create_junction_for_n_n()
             self._create_walking_lanes()
             self._expand_remain_roads()
             self._post_process()
-        self._add_aoi()
+        if self.reuse_map is not None:
+            self._reuse_aoi()
+        else:
+            self._add_aoi()
         output_map = self.get_output_map(name)
         output_format_check(output_map)
         return output_map
 
 
 # def main():
 #     # Configure log and store it in the file mapbuilder2.log
```

### Comparing `mosstool-0.1.0/mosstool/map/osm/_motif.py` & `mosstool-0.2.0/mosstool/map/osm/_motif.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/osm/_wayutil.py` & `mosstool-0.2.0/mosstool/map/osm/_wayutil.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/osm/building.py` & `mosstool-0.2.0/mosstool/map/osm/building.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/osm/roadnet.py` & `mosstool-0.2.0/mosstool/map/osm/roadnet.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/public_transport/get_bus.py` & `mosstool-0.2.0/mosstool/map/public_transport/get_bus.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/public_transport/get_subway.py` & `mosstool-0.2.0/mosstool/map/public_transport/get_subway.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/public_transport/get_transitland.py` & `mosstool-0.2.0/mosstool/map/public_transport/get_transitland.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/public_transport/public_transport_post.py` & `mosstool-0.2.0/mosstool/map/public_transport/public_transport_post.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/sumo/map.py` & `mosstool-0.2.0/mosstool/map/sumo/map.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/map/vis/map.py` & `mosstool-0.2.0/mosstool/map/vis/map.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/trip/generator/AIGC.py` & `mosstool-0.2.0/mosstool/trip/generator/AIGC.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/trip/generator/_util/const.py` & `mosstool-0.2.0/mosstool/trip/generator/_util/const.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/trip/generator/generate_from_od.py` & `mosstool-0.2.0/mosstool/trip/generator/generate_from_od.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,16 +473,16 @@
             self.persons.append(p)
 
     def generate_persons(
         self,
         od_matrix: np.ndarray,
         areas: GeoDataFrame,
         departure_time_curve: Optional[list[float]] = None,
-        agent_num: int = 10000,
         seed: int = 0,
+        agent_num: Optional[int] = None,
     ) -> List[Person]:
         """
         Args:
         - od_matrix (numpy.ndarray): The OD matrix.
         - areas (GeoDataFrame): The area data.
         - departure_time_curve (list[float]): The departure time of a day (24h). The resolution must >=1h.
         - agent_num (int): number of agents to generate.
@@ -502,9 +502,14 @@
             self.departure_prob = None
         self.od_matrix = od_matrix
         self.areas = areas
         self._read_aois()
         self._read_regions()
         self._read_od_matrix()
         self._match_aoi2region()
+        if agent_num is None:
+            agent_num = int(np.sum(self.od) / self.LEN_OD_TIMES)
+        if agent_num <= 0:
+            logging.warning("agent_num should >=1")
+            return []
         self._generate_mobi(agent_num, seed)
         return self.persons
```

### Comparing `mosstool-0.1.0/mosstool/trip/generator/gravity.py` & `mosstool-0.2.0/mosstool/trip/generator/gravity.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/trip/generator/random.py` & `mosstool-0.2.0/mosstool/trip/generator/random.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/trip/generator/template.py` & `mosstool-0.2.0/mosstool/trip/generator/template.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/trip/route/client.py` & `mosstool-0.2.0/mosstool/trip/route/client.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/trip/route/preroute.py` & `mosstool-0.2.0/mosstool/trip/route/preroute.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/trip/sumo/route.py` & `mosstool-0.2.0/mosstool/trip/sumo/route.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/trip/vis/trip.py` & `mosstool-0.2.0/mosstool/trip/vis/trip.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/type/__init__.py` & `mosstool-0.2.0/mosstool/type/__init__.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/util/format_converter.py` & `mosstool-0.2.0/mosstool/util/format_converter.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/util/geo_match_pop.py` & `mosstool-0.2.0/mosstool/util/geo_match_pop.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/util/map_merger.py` & `mosstool-0.2.0/mosstool/util/map_merger.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/util/map_splitter.py` & `mosstool-0.2.0/mosstool/util/map_splitter.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/mosstool/util/test/test_format_conveter.py` & `mosstool-0.2.0/mosstool/util/test/test_format_conveter.py`

 * *Files identical despite different names*

### Comparing `mosstool-0.1.0/pyproject.toml` & `mosstool-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mosstool"
-version = "0.1.0"
+version = "0.2.0"
 description = "MObility Simulation System toolbox "
 authors = ["Jun Zhang <zhangjun990222@qq.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `mosstool-0.1.0/PKG-INFO` & `mosstool-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosstool
-Version: 0.1.0
+Version: 0.2.0
 Summary: MObility Simulation System toolbox 
 License: MIT
 Author: Jun Zhang
 Author-email: zhangjun990222@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -38,11 +38,11 @@
 # mosstool
 
 MObility Simulation System (MOSS) Toolbox
 
 ## Installation
 
 ```bash
-pip install mosstool --index-url https://__token__:glpat-fq6C-NTr45Z_Te4BV4kC@git.fiblab.net/api/v4/projects/110/packages/pypi/simple
+pip install mosstool
 ```
```

