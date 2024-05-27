# Comparing `tmp/pyastroweatherio-0.50.0.dev13.tar.gz` & `tmp/pyastroweatherio-0.50.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.50.0.dev13.tar", last modified: Thu May 23 18:39:58 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.50.1.tar", last modified: Mon May 27 07:58:51 2024, max compression
```

## Comparing `pyastroweatherio-0.50.0.dev13.tar` & `pyastroweatherio-0.50.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-23 18:39:58.343311 pyastroweatherio-0.50.0.dev13/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.0.dev13/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1118 2024-05-23 18:39:58.343311 pyastroweatherio-0.50.0.dev13/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.0.dev13/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-23 18:39:58.335311 pyastroweatherio-0.50.0.dev13/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-05-23 16:56:37.000000 pyastroweatherio-0.50.0.dev13/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    42012 2024-05-23 16:56:37.000000 pyastroweatherio-0.50.0.dev13/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     6068 2024-05-23 16:56:37.000000 pyastroweatherio-0.50.0.dev13/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    24839 2024-05-23 16:56:37.000000 pyastroweatherio-0.50.0.dev13/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2024-05-23 16:56:37.000000 pyastroweatherio-0.50.0.dev13/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    53103 2024-05-23 16:56:37.000000 pyastroweatherio-0.50.0.dev13/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-23 18:39:58.343311 pyastroweatherio-0.50.0.dev13/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1118 2024-05-23 18:39:58.000000 pyastroweatherio-0.50.0.dev13/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-05-23 18:39:58.000000 pyastroweatherio-0.50.0.dev13/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-05-23 18:39:58.000000 pyastroweatherio-0.50.0.dev13/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       25 2024-05-23 18:39:58.000000 pyastroweatherio-0.50.0.dev13/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-05-23 18:39:58.000000 pyastroweatherio-0.50.0.dev13/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-05-23 18:39:58.347311 pyastroweatherio-0.50.0.dev13/setup.cfg
--rw-r--r--   0 markus    (1000) markus    (1000)     1403 2024-05-23 16:56:37.000000 pyastroweatherio-0.50.0.dev13/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-27 07:58:51.190609 pyastroweatherio-0.50.1/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.50.1/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1112 2024-05-27 07:58:51.190609 pyastroweatherio-0.50.1/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.50.1/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-27 07:58:51.186609 pyastroweatherio-0.50.1/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      284 2024-05-27 06:33:40.000000 pyastroweatherio-0.50.1/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    42587 2024-05-27 06:33:53.000000 pyastroweatherio-0.50.1/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     6068 2024-05-25 14:57:18.000000 pyastroweatherio-0.50.1/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    24883 2024-05-27 06:34:20.000000 pyastroweatherio-0.50.1/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2024-05-25 14:57:18.000000 pyastroweatherio-0.50.1/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    47443 2024-05-27 07:50:12.000000 pyastroweatherio-0.50.1/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-05-27 07:58:51.190609 pyastroweatherio-0.50.1/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1112 2024-05-27 07:58:51.000000 pyastroweatherio-0.50.1/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-05-27 07:58:51.000000 pyastroweatherio-0.50.1/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-05-27 07:58:51.000000 pyastroweatherio-0.50.1/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       25 2024-05-27 07:58:51.000000 pyastroweatherio-0.50.1/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-05-27 07:58:51.000000 pyastroweatherio-0.50.1/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-05-27 07:58:51.190609 pyastroweatherio-0.50.1/setup.cfg
+-rw-r--r--   0 markus    (1000) markus    (1000)     1397 2024-05-27 06:37:57.000000 pyastroweatherio-0.50.1/setup.py
```

### Comparing `pyastroweatherio-0.50.0.dev13/LICENSE` & `pyastroweatherio-0.50.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev13/PKG-INFO` & `pyastroweatherio-0.50.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.0.dev13
+Version: 0.50.1
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.0.dev13/README.md` & `pyastroweatherio-0.50.1/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev13/pyastroweatherio/client.py` & `pyastroweatherio-0.50.1/pyastroweatherio/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 """Define a client to interact with 7Timer."""
 
 import asyncio
+from datetime import UTC, datetime, timedelta
 import json
 from json.decoder import JSONDecodeError
 import logging
-import os.path
 import math
-from datetime import datetime, timedelta, timezone, UTC
+import os.path
 from typing import Optional
+
+import aiofiles
 from aiohttp import ClientSession, ClientTimeout
 from aiohttp.client_exceptions import ClientError
 
-import pprint
-
-pp = pprint.PrettyPrinter()
-
 from pyastroweatherio.const import (
-    BASE_URL_SEVENTIMER,
     BASE_URL_MET,
-    HEADERS,
-    DEFAULT_TIMEOUT,
+    BASE_URL_SEVENTIMER,
     DEFAULT_CACHE_TIMEOUT,
-    DEFAULT_TIMEZONE,
+    DEFAULT_CONDITION_CALM_WEIGHT,
+    DEFAULT_CONDITION_CLOUDCOVER_HIGH_WEAKENING,
+    DEFAULT_CONDITION_CLOUDCOVER_LOW_WEAKENING,
+    DEFAULT_CONDITION_CLOUDCOVER_MEDIUM_WEAKENING,
+    DEFAULT_CONDITION_CLOUDCOVER_WEIGHT,
+    DEFAULT_CONDITION_SEEING_WEIGHT,
+    DEFAULT_CONDITION_TRANSPARENCY_WEIGHT,
+    DEFAULT_ELEVATION,
     DEFAULT_LATITUDE,
     DEFAULT_LONGITUDE,
-    DEFAULT_ELEVATION,
+    DEFAULT_TIMEOUT,
+    DEFAULT_TIMEZONE,
+    FORECAST_TYPE_HOURLY,
+    HEADERS,
+    MAG_DEGRATION_MAX,
     SEEING,
     SEEING_MAX,
     TRANSPARENCY,
-    MAG_DEGRATION_MAX,
     WIND10M_MAX,
-    DEFAULT_CONDITION_CLOUDCOVER_WEIGHT,
-    DEFAULT_CONDITION_CLOUDCOVER_HIGH_WEAKENING,
-    DEFAULT_CONDITION_CLOUDCOVER_MEDIUM_WEAKENING,
-    DEFAULT_CONDITION_CLOUDCOVER_LOW_WEAKENING,
-    DEFAULT_CONDITION_SEEING_WEIGHT,
-    DEFAULT_CONDITION_TRANSPARENCY_WEIGHT,
-    DEFAULT_CONDITION_CALM_WEIGHT,
-    FORECAST_TYPE_HOURLY,
 )
 from pyastroweatherio.dataclasses import (
+    DSOUpTonight,
     ForecastData,
     LocationData,
     NightlyConditionsData,
-    DSOUpTonight,
 )
 from pyastroweatherio.errors import RequestError
 from pyastroweatherio.helper_functions import (
-    ConversionFunctions,
     AstronomicalRoutines,
     AtmosphericRoutines,
+    ConversionFunctions,
 )
 
 _LOGGER = logging.getLogger(__name__)
 _NOT_AVAILABLE = -9999
 
 
 class AstroWeather:
@@ -128,22 +126,25 @@
             self._test_mode = True
 
     # Public functions
     async def get_location_data(
         self,
     ) -> None:
         """Returns station Weather Forecast."""
+
         return await self._get_location_data()
 
     async def get_hourly_forecast(self) -> None:
         """Returns hourly Weather Forecast."""
+
         return await self._get_forecast_data(FORECAST_TYPE_HOURLY, 72)
 
     async def get_deepsky_forecast(self) -> None:
         """Returns Deep Sky Forecast."""
+
         return await self._get_deepsky_forecast()
 
     # Private functions
     async def _get_location_data(self) -> None:
         """Return Forecast data"""
 
         cnv = ConversionFunctions()
@@ -553,15 +554,15 @@
 
         self._forecast_data = items
 
         _LOGGER.debug("Forceast Length: %s", str(len(items)))
         return items
 
     async def _get_deepsky_forecast(self):
-        """Return Deepsky Forecast data"""
+        """Return Deepsky Forecast data."""
 
         cnv = ConversionFunctions()
         items = []
 
         if self._forecast_data == None:
             await self._get_forecast_data(FORECAST_TYPE_HOURLY, 72)
 
@@ -691,15 +692,15 @@
         cloudcover_high,
         cloudcover_medium,
         cloudcover_low,
         seeing,
         transparency,
         wind_speed,
     ):
-        """Return condition based on cloud cover, seeing, transparency, and wind speed"""
+        """Return condition based on cloud cover, seeing, transparency, and wind speed."""
 
         if not all(
             v is not None
             for v in [
                 cloudcover_high,
                 cloudcover_medium,
                 cloudcover_low,
@@ -754,15 +755,15 @@
         #     str(self._calm_weight),
         #     condition,
         # )
 
         return condition
 
     async def _get_deepsky_objects(self):
-        """Return Deepsky Objects for today"""
+        """Return Deepsky Objects for today."""
 
         items = []
 
         await self.retrieve_data_uptonight()
 
         # Create list of deep sky objects
         if self._weather_data_uptonight is not None:
@@ -791,15 +792,15 @@
                 #     str(item["foto"]),
                 # )
 
             return items
         return None
 
     async def retrieve_data_seventimer(self):
-        """Retrieves current data from 7timer"""
+        """Retrieves current data from 7timer."""
 
         if (
             (datetime.now() - self._weather_data_seventimer_timestamp).total_seconds()
         ) > DEFAULT_CACHE_TIMEOUT:
             self._weather_data_seventimer_timestamp = datetime.now()
             _LOGGER.debug("Updating data from 7Timer")
 
@@ -831,14 +832,15 @@
 
             if astro_dataseries != {} and not self._experimental_features:
                 self._weather_data_seventimer = astro_dataseries
                 self._weather_data_seventimer_init = json_data_astro.get("init")
             else:
                 # Fake 7timer weather data if service is broken
                 # This eliminates consideration of seeing, transparency, and lifted_index
+                # and switches automatically to experimental functions.
                 self._weather_data_seventimer = []
                 for index in range(0, 20):
                     self._weather_data_seventimer.append(
                         {
                             "timepoint": index * 3,
                             "seeing": _NOT_AVAILABLE,
                             "transparency": _NOT_AVAILABLE,
@@ -896,15 +898,15 @@
             return {}
 
         finally:
             if not use_running_session:
                 await session.close()
 
     def _get_data_seventimer_timer(self, anchor_timestamp, datetime):
-        """Return 7Timer datapoint of interest"""
+        """Return 7Timer datapoint of interest."""
 
         seventimer_index = 0
         for index, row7 in enumerate(self._weather_data_seventimer):
             if anchor_timestamp + timedelta(hours=row7["timepoint"]) > datetime:
                 seventimer_index = index - 1
                 break
             # index += 1
@@ -915,15 +917,15 @@
                 "transparency": _NOT_AVAILABLE,
                 "lifted_index": _NOT_AVAILABLE,
             }
         else:
             return self._weather_data_seventimer[seventimer_index]
 
     async def retrieve_data_metno(self):
-        """Retrieves current data from met"""
+        """Retrieves current data from met."""
 
         if (
             (datetime.now() - self._weather_data_metno_timestamp).total_seconds()
         ) > DEFAULT_CACHE_TIMEOUT:
             self._weather_data_metno_timestamp = datetime.now()
             _LOGGER.debug("Updating data from Met.no")
 
@@ -1008,20 +1010,30 @@
             (datetime.now() - self._data_uptonight_timestamp).total_seconds()
         ) > DEFAULT_CACHE_TIMEOUT:
             self._data_uptonight_timestamp = datetime.now()
             _LOGGER.debug("Updating data from uptonight")
 
             dataseries = None
 
-            if os.path.isfile(self._uptonight_path + "/uptonight-report.json"):
-                # _LOGGER.debug(f"Uptonight report found")
-                with open(self._uptonight_path + "/uptonight-report.json") as json_file:
-                    dataseries = json.load(json_file)
+            if os.path.exists(self._uptonight_path):
+                if os.path.isfile(self._uptonight_path + "/uptonight-report.json"):
+                    # _LOGGER.debug(f"Uptonight report found")
+                    async with aiofiles.open(
+                        self._uptonight_path + "/uptonight-report.json", mode="r"
+                    ) as json_file:
+                        # with open(self._uptonight_path + "/uptonight-report.json") as json_file:
+                        contents = await json_file.read()
+                        # dataseries = json.load(json_file)
+                    dataseries = json.loads(contents)
                     _LOGGER.debug(f"Uptonight imported")
+                else:
+                    _LOGGER.debug(
+                        f"File uptonight-report.json not found in {self._uptonight_path}"
+                    )
             else:
                 _LOGGER.debug(
-                    f"uptonight-report.json not found. Current path: {self._uptonight_path}/uptonight-report.json"
+                    f"Path for uptonight-report.json not found. Current path: {self._uptonight_path}/uptonight-report.json"
                 )
 
             self._weather_data_uptonight = dataseries
         else:
             _LOGGER.debug("Using cached data for uptonight")
```

### Comparing `pyastroweatherio-0.50.0.dev13/pyastroweatherio/const.py` & `pyastroweatherio-0.50.1/pyastroweatherio/const.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.50.0.dev13/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.50.1/pyastroweatherio/dataclasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Defines the Data Classes used."""
 
 from datetime import datetime, timezone
 import math
 
 from pyastroweatherio.const import (
     SEEING_MAX,
-    # SEEING_PLAIN,
     MAG_DEGRATION_MAX,
-    # TRANSPARENCY_PLAIN,
     LIFTED_INDEX_VALUE,
     LIFTED_INDEX_RANGE,
     LIFTED_INDEX_PLAIN,
     WIND10M_VALUE,
     WIND10M_RANGE,
     WIND10M_PLAIN,
     WIND10M_DIRECTON,
@@ -48,193 +46,219 @@
         self._weather = data["weather"]
         self._weather6 = data["weather6"]
         self._precipitation_amount = data["precipitation_amount"]
 
     @property
     def seventimer_init(self) -> datetime:
         """Return Forecast Anchor."""
+        
         if self._seventimer_init is not None:
             return self._seventimer_init.replace(microsecond=0, tzinfo=timezone.utc)
         return None
 
     @property
     def seventimer_timepoint(self) -> int:
         """Return Forecast Hour."""
+        
         if self._seventimer_timepoint is not None:
             return self._seventimer_timepoint
         return None
 
     @property
     def forecast_time(self) -> datetime:
         """Return Forecast Timestamp."""
+        
         if self._forecast_time is not None:
             return self._forecast_time.replace(microsecond=0, tzinfo=timezone.utc)
         return None
 
     @property
     def condition_percentage(self) -> int:
-        """Return condition based on cloud cover, seeing and transparency"""
+        """Return condition based on cloud cover, seeing and transparency."""
+        
         if self._condition_percentage is not None:
             return int(self._condition_percentage)
         return None
 
     @property
     def cloudcover(self) -> int:
         """Return Cloud Coverage."""
+        
         if self._cloudcover is not None:
             return int(self._cloudcover)
         return None
 
     @property
     def cloudcover_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
+        
         if self._cloudcover is not None:
             return int(self._cloudcover)
         return None
 
     @property
     def cloudless_percentage(self) -> int:
         """Return Cloudless Percentage."""
+        
         if self._cloudcover is not None:
             return 100 - int(self._cloudcover)
         return None
 
     @property
     def cloud_area_fraction_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
+        
         if self._cloud_area_fraction is not None:
             return int(self._cloud_area_fraction)
         return None
 
     @property
     def cloud_area_fraction_high_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
+        
         if self._cloud_area_fraction_high is not None:
             return int(self._cloud_area_fraction_high)
         return None
 
     @property
     def cloud_area_fraction_medium_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
+        
         if self._cloud_area_fraction_medium is not None:
             return int(self._cloud_area_fraction_medium)
         return None
 
     @property
     def cloud_area_fraction_low_percentage(self) -> int:
         """Return Cloud Cover Percentage."""
+        
         if self._cloud_area_fraction_low is not None:
             return int(self._cloud_area_fraction_low)
         return None
 
     @property
     def fog_area_fraction_percentage(self) -> int:
         """Return Fog Area Percentage."""
+        
         if self._fog_area_fraction is not None:
             return int(self._fog_area_fraction)
         return None
 
     @property
     def seeing(self) -> float:
         """Return Seeing."""
+        
         if self._seeing is not None:
             return round(self._seeing, 2)
         return None
 
     @property
     def seeing_percentage(self) -> int:
         """Return Seeing."""
+        
         if self._seeing is not None:
             return int(100 - self._seeing * 100 / SEEING_MAX)
         return None
 
     @property
     def transparency(self) -> float:
         """Return Transparency."""
+        
         if self._transparency is not None:
             return round(self._transparency, 2)
         return None
 
     @property
     def transparency_percentage(self) -> int:
         """Return Transparency."""
+        
         if self._transparency is not None:
             return int(100 - self._transparency * 100 / MAG_DEGRATION_MAX)
         return None
 
     @property
     def lifted_index(self) -> float:
         """Return Lifted Index."""
+        
         if self._lifted_index is not None:
             return round(self._lifted_index, 2)
         return None
 
     @property
     def rh2m(self) -> int:
         """Return 2m Relative Humidity."""
+        
         if self._rh2m is not None:
             return self._rh2m
         return None
 
     @property
     def wind10m_speed(self) -> float:
         """Return 10m Wind Speed."""
+        
         if self._wind_speed is not None:
             return self._wind_speed
         return None
 
     @property
     def calm_percentage(self) -> int:
         """Return 10m Wind Speed."""
+        
         if self._wind_speed is not None:
             return int(100 - self._wind_speed * (100 / WIND10M_MAX))
         return None
 
     @property
     def wind10m_direction(self) -> str:
         """Return 10m Wind Direction."""
+        
         if self._wind_from_direction is not None:
             direction = self._wind_from_direction
             direction += 22.5
             direction = direction % 360
             direction = int(direction / 45)  # values 0 to 7
             return WIND10M_DIRECTON[max(0, min(7, direction))]
         return None
 
     @property
     def temp2m(self) -> int:
         """Return 2m Temperature."""
+        
         if self._temp2m is not None:
             return self._temp2m
         return None
 
     @property
     def dewpoint2m(self) -> float:
         """Return 2m Dew Point."""
+        
         if self._dewpoint2m is not None:
             return round(self._dewpoint2m, 1)
         return None
 
     @property
     def weather(self) -> str:
         """Return Current Weather."""
+        
         if self._weather is not None:
             return self._weather.replace("_", " ").capitalize()
         return None
 
     @property
     def weather6(self) -> str:
         """Return Current Weather."""
+        
         if self._weather6 is not None:
             return self._weather6.replace("_", " ").capitalize()
         return None
 
     @property
     def precipitation_amount(self) -> float:
         """Return Current Weather."""
+        
         if self._precipitation_amount is not None:
             return self._precipitation_amount
         return None
 
 
 class LocationData(BaseData):
     """A representation of the Location AstroWeather Data."""
@@ -269,70 +293,56 @@
         self._deep_sky_darkness = data["deep_sky_darkness"]
         self._deepsky_forecast = data["deepsky_forecast"]
         self._uptonight = data["uptonight"]
 
     @property
     def time_shift(self) -> int:
         """Return Forecast Timestamp."""
+        
         if self._time_shift is not None:
             return self._time_shift
         return None
 
     @property
     def forecast_length(self) -> int:
-        """Return Forecast Length in Hours"""
+        """Return Forecast Length in Hours."""
+        
         if self._forecast_length is not None:
             return self._forecast_length
         return None
 
     @property
     def latitude(self) -> float:
         """Return Latitude."""
+        
         if self._latitude is not None:
             return self._latitude
         return None
 
     @property
     def longitude(self) -> float:
         """Return Longitude."""
+        
         if self._longitude is not None:
             return self._longitude
         return None
 
     @property
     def elevation(self) -> float:
         """Return Elevation."""
+        
         if self._elevation is not None:
             return self._elevation
         return None
 
-    # @property
-    # def cloudcover_plain(self) -> str:
-    #     """Return Cloud Coverage."""
-    #     cover = self._cloudcover
-    #     if cover >= 1 and cover <= 9:
-    #         return CLOUDCOVER_PLAIN[cover - 1]
-    #     return None
-
     @property
     def seeing_plain(self) -> str:
         """Return Seeing."""
+        
         return "Deprecated. Use seeing instead."
-        # seeing = self._seeing
-        # if seeing >= 1 and seeing <= 8:
-        #     return SEEING_PLAIN[seeing - 1]
-        # return None
-
-    # @property
-    # def transparency_plain(self) -> str:
-    #     """Return Transparency."""
-    #     transparency = self._transparency
-    #     if transparency >= 1 and transparency <= 8:
-    #         return TRANSPARENCY_PLAIN[self._transparency - 1]
-    #     return None
 
     @property
     def wind10m_speed_plain(self) -> str:
         """Return wind speed plain."""
 
         if self._wind_speed is not None:
             wind_speed_value = 0
@@ -355,23 +365,25 @@
 
             return LIFTED_INDEX_PLAIN[max(0, min(7, lifted_index_value - 1))]
         return None
 
     @property
     def deep_sky_view(self) -> bool:
         """Return True if Deep Sky should be possible."""
+        
         if self.condition_percentage is not None:
             if self.condition_percentage >= DEEP_SKY_THRESHOLD:
                 return True
             return False
         return None
 
     @property
     def condition_plain(self) -> str:
         """Return Current View Conditions."""
+        
         if self.condition_percentage is not None:
             if self.condition_percentage > 80:
                 return CONDITION_PLAIN[0].capitalize()
             if self.condition_percentage > 60:
                 return CONDITION_PLAIN[1].capitalize()
             if self.condition_percentage > 40:
                 return CONDITION_PLAIN[2].capitalize()
@@ -379,254 +391,287 @@
                 return CONDITION_PLAIN[3].capitalize()
             return CONDITION_PLAIN[4].capitalize()
         return None
 
     @property
     def sun_next_rising(self) -> datetime:
         """Return Sun Next Rising Civil."""
+        
         if isinstance(self._sun_next_rising, datetime):
             return self._sun_next_rising
         return None
 
     @property
     def sun_next_rising_nautical(self) -> datetime:
         """Return Sun Next Rising Nautical."""
+        
         if isinstance(self._sun_next_rising_nautical, datetime):
             return self._sun_next_rising_nautical
         return None
 
     @property
     def sun_next_rising_astro(self) -> datetime:
         """Return Sun Next Rising Astronomical."""
+        
         if isinstance(self._sun_next_rising_astro, datetime):
             return self._sun_next_rising_astro
         return None
 
     @property
     def sun_next_setting(self) -> datetime:
         """Return Next Setting Civil."""
+        
         if isinstance(self._sun_next_setting, datetime):
             return self._sun_next_setting
         return None
 
     @property
     def sun_next_setting_nautical(self) -> datetime:
         """Return Sun Next Setting Nautical."""
+        
         if isinstance(self._sun_next_setting_nautical, datetime):
             return self._sun_next_setting_nautical
         return None
 
     @property
     def sun_next_setting_astro(self) -> datetime:
         """Return Sun Next Setting Astronomical."""
+        
         if isinstance(self._sun_next_setting_astro, datetime):
             return self._sun_next_setting_astro
         return None
 
     @property
     def sun_altitude(self) -> float:
         """Return Sun Altitude."""
+        
         if self._sun_altitude is not None:
             return round(self._sun_altitude, 3)
         return None
 
     @property
     def sun_azimuth(self) -> float:
         """Return sun Azimuth."""
+        
         if self._sun_azimuth is not None:
             return round(self._sun_azimuth, 3)
         return None
 
     @property
     def moon_next_rising(self) -> datetime:
         """Return Moon Next Rising."""
+        
         if isinstance(self._moon_next_rising, datetime):
             return self._moon_next_rising
         return None
 
     @property
     def moon_next_setting(self) -> datetime:
         """Return Moon Next Setting."""
+        
         if isinstance(self._moon_next_setting, datetime):
             return self._moon_next_setting
         return None
 
     @property
     def moon_phase(self) -> float:
         """Return Moon Phase."""
+        
         if self._moon_phase is not None:
             return round(self._moon_phase, 1)
         return None
 
     @property
     def moon_next_new_moon(self) -> datetime:
         """Return Moon Next New Moon."""
+        
         if isinstance(self._moon_next_new_moon, datetime):
             return self._moon_next_new_moon
         return None
 
     @property
     def moon_next_full_moon(self) -> datetime:
         """Return Moon Next Full Moon."""
+        
         if isinstance(self._moon_next_full_moon, datetime):
             return self._moon_next_full_moon
         return None
 
     @property
     def moon_altitude(self) -> float:
         """Return Moon Altitude."""
+        
         if self._moon_altitude is not None:
             return round(self._moon_altitude, 3)
         return None
 
     @property
     def moon_azimuth(self) -> float:
         """Return Moon Azimuth."""
+        
         if self._moon_azimuth is not None:
             return round(self._moon_azimuth, 3)
         return None
 
     @property
     def night_duration_astronomical(self) -> float:
         """Returns the remaining timespan of astronomical darkness."""
+        
         if self._night_duration_astronomical is not None:
             return self._night_duration_astronomical
         return None
 
     @property
     def deep_sky_darkness_moon_rises(self) -> bool:
         """Returns true if moon rises during astronomical night."""
+        
         if self._deep_sky_darkness_moon_rises is not None:
             return self._deep_sky_darkness_moon_rises
         return None
 
     @property
     def deep_sky_darkness_moon_sets(self) -> bool:
         """Returns true if moon sets during astronomical night."""
+        
         if self._deep_sky_darkness_moon_sets is not None:
             return self._deep_sky_darkness_moon_sets
         return None
 
     @property
     def deep_sky_darkness_moon_always_up(self) -> bool:
         """Returns true if moon is up during astronomical night."""
+        
         if self._deep_sky_darkness_moon_always_up is not None:
             return self._deep_sky_darkness_moon_always_up
         return None
 
     @property
     def deep_sky_darkness_moon_always_down(self) -> bool:
         """Returns true if moon is down during astronomical night."""
+        
         if self._deep_sky_darkness_moon_always_down is not None:
             return self._deep_sky_darkness_moon_always_down
         return None
 
     @property
     def deep_sky_darkness(self) -> float:
         """Returns the remaining timespan of deep sky darkness."""
+        
         if self._deep_sky_darkness is not None:
             return self._deep_sky_darkness
         return None
 
     @property
     def deepsky_forecast_today(self) -> int:
         """Return Forecas Today in Percent."""
+        
         if self._deepsky_forecast is not None:
             nightly_condition_sum = 0
             if len(self._deepsky_forecast) > 0:
                 for nightly_condition in self._deepsky_forecast[0].nightly_conditions:
                     nightly_condition_sum += nightly_condition
                 return int(round(nightly_condition_sum / len(self._deepsky_forecast[0].nightly_conditions)))
         return None
 
     @property
     def deepsky_forecast_today_dayname(self):
         """Return Forecast Todays Dayname."""
+        
         if self._deepsky_forecast is not None:
             if len(self._deepsky_forecast) > 0:
                 nightly_conditions = self._deepsky_forecast[0]
                 return nightly_conditions.dayname
         return None
 
     @property
     def deepsky_forecast_today_plain(self):
         """Return Forecast Today."""
+        
         if self._deepsky_forecast is not None:
             out = ""
             if len(self._deepsky_forecast) > 0:
                 for nightly_condition in self._deepsky_forecast[0].nightly_conditions:
                     out += CONDITION[4 - math.floor(nightly_condition / 20)].capitalize()
             return out
         return None
 
     @property
     def deepsky_forecast_today_desc(self):
         """Return Forecast Today Description."""
+        
         if self._deepsky_forecast is not None:
             if len(self._deepsky_forecast) > 0:
                 nightly_conditions = self._deepsky_forecast[0]
                 return nightly_conditions.weather.replace("_", " ").capitalize()
         return None
 
     @property
     def deepsky_forecast_tomorrow(self) -> int:
         """Return Forecas Tomorrow in Percentt."""
+        
         if self._deepsky_forecast is not None:
             nightly_condition_sum = 0
             if len(self._deepsky_forecast) > 1:
                 for nightly_condition in self._deepsky_forecast[1].nightly_conditions:
                     nightly_condition_sum += nightly_condition
                 return int(round(nightly_condition_sum / len(self._deepsky_forecast[1].nightly_conditions)))
         return None
 
     @property
     def deepsky_forecast_tomorrow_dayname(self):
         """Return Forecast Todays Dayname."""
+        
         if self._deepsky_forecast is not None:
             if len(self._deepsky_forecast) > 1:
                 nightly_conditions = self._deepsky_forecast[1]
                 return nightly_conditions.dayname
         return None
 
     @property
     def deepsky_forecast_tomorrow_plain(self):
         """Return Forecast Tomorrow."""
+        
         if self._deepsky_forecast is not None:
             out = ""
             if len(self._deepsky_forecast) > 1:
                 for nightly_condition in self._deepsky_forecast[1].nightly_conditions:
                     out += CONDITION[4 - math.floor(nightly_condition / 20)].capitalize()
             return out
         return None
 
     @property
     def deepsky_forecast_tomorrow_desc(self):
         """Return Forecast Tomorrow Description."""
+        
         if self._deepsky_forecast is not None:
             if len(self._deepsky_forecast) > 1:
                 nightly_conditions = self._deepsky_forecast[1]
                 return nightly_conditions.weather.replace("_", " ").capitalize()
         return None
 
     @property
     def deepsky_forecast(self):
         """Return Deepsky Forecast."""
+        
         if self._deepsky_forecast is not None:
             return self._deepsky_forecast
         return None
 
     @property
     def uptonight(self) -> int:
         """Return the number of best DSOs for tonight."""
+        
         if self._uptonight is not None:
             return len(self._uptonight)
         return None
 
     @property
     def uptonight_list(self) -> []:
+        """Return the list of UpTonight targets."""
+        
         if self._uptonight is not None:
             return self._uptonight
         return None
 
 
 class ForecastData(BaseData):
     """A representation of 3-Hour Based Forecast AstroWeather Data."""
@@ -634,21 +679,23 @@
     def __init__(self, data):
         super().__init__(data)
         self._hour = data["hour"]
 
     @property
     def hour(self) -> int:
         """Return Forecast Hour of the day."""
+        
         if self._hour is not None:
             return self._hour
         return None
 
     @property
     def deep_sky_view(self) -> bool:
         """Return True if Deep Sky should be possible."""
+        
         if self.condition_percentage is not None:
             if self.condition_percentage <= DEEP_SKY_THRESHOLD:
                 return True
             return False
         return None
 
 
@@ -661,42 +708,47 @@
         self._hour = data["hour"]
         self._nightly_conditions = data["nightly_conditions"]
         self._weather = data["weather"]
 
     @property
     def seventimer_init(self) -> datetime:
         """Return Forecast Anchor."""
+        
         if self._seventimer_init is not None:
             return self._seventimer_init
         return None
 
     @property
     def dayname(self) -> str:
         """Return Forecast Name of the Day."""
+        
         if self._dayname is not None:
             return self._dayname
         return None
 
     @property
     def hour(self) -> int:
         """Return Forecast Hour."""
+        
         if self._hour is not None:
             return self._hour
         return None
 
     @property
     def nightly_conditions(self) -> int:
         """Return Forecast Hour."""
+        
         if self._nightly_conditions is not None:
             return self._nightly_conditions
         return None
 
     @property
     def weather(self) -> str:
         """Return Current Weather."""
+        
         if self._weather is not None:
             return self._weather.replace("_", " ").capitalize()
         return None
 
 
 class DSOUpTonight:
     """A representation of uptonight DSO."""
@@ -707,38 +759,43 @@
         self._constellation = data["constellation"]
         self._size = data["size"]
         self._foto = data["foto"]
 
     @property
     def target_name(self) -> str:
         """Return Forecast Name of the Day."""
+        
         if self._target_name is not None:
             return self._target_name
         return None
 
     @property
     def type(self) -> str:
         """Return Forecast Name of the Day."""
+        
         if self._type is not None:
             return self._type
         return None
 
     @property
     def constellation(self) -> str:
         """Return Forecast Name of the Day."""
+        
         if self._constellation is not None:
             return self._constellation
         return None
 
     @property
     def size(self) -> str:
         """Return Forecast Name of the Day."""
+        
         if self._size is not None:
             return self._size
         return None
 
     @property
     def foto(self) -> str:
         """Return Forecast Name of the Day."""
+        
         if self._foto is not None:
             return self._foto
         return None
```

### Comparing `pyastroweatherio-0.50.0.dev13/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.50.1/pyastroweatherio/helper_functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 """Contains Helper functions for AstroWeather."""
 
+from datetime import UTC, datetime, timedelta, timezone
+from decimal import Decimal
 import logging
-import ephem
 import math
-from datetime import datetime, timedelta, timezone, UTC
+from math import degrees as deg
 from zoneinfo import ZoneInfo
-from decimal import Decimal
+
+import ephem
 from ephem import degree
-from math import degrees as deg
-# import pytz
 
-# The introduction of the module [timezonefinder](https://github.com/jannikmi/timezonefinder)
-# with it's nested dependency to [py-h3](https://github.com/uber/h3-py) failed while compiling
-# the `c`-module h3 on some home assistant deployment variants (e.g. Home Assistant
-# Operating System on RPi).
-# from timezonefinder import TimezoneFinder
 from pyastroweatherio.const import (
-    DEFAULT_TIMEZONE,
+    ASTRONOMICAL_DUSK_DAWN,
+    CIVIL_DUSK_DAWN,
+    DEFAULT_ELEVATION,
     DEFAULT_LATITUDE,
     DEFAULT_LONGITUDE,
-    DEFAULT_ELEVATION,
-    CIVIL_TWILIGHT,
-    CIVIL_DUSK_DAWN,
-    NAUTICAL_TWILIGHT,
+    DEFAULT_TIMEZONE,
+    MAG_DEGRATION_MAX,
     NAUTICAL_DUSK_DAWN,
-    ASTRONOMICAL_TWILIGHT,
-    ASTRONOMICAL_DUSK_DAWN,
     SEEING_MAX,
-    MAG_DEGRATION_MAX,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ConversionFunctions:
     """Convert between different units."""
 
     async def epoch_to_datetime(self, value) -> str:
         """Converts EPOC time to Date Time String."""
+
         return datetime.datetime.fromtimestamp(int(value)).strftime("%Y-%m-%d %H:%M:%S")
 
     async def anchor_timestamp(self, value) -> datetime:
         """Converts the datetime string from 7Timer to DateTime."""
+
         return datetime.strptime(value, "%Y%m%d%H")
 
 
 class AtmosphericRoutines:
-    """Calculate atmospheric lifted index"""
+    """Calculate atmospheric attributes."""
 
     def __init__(
         self,
     ):
         _LOGGER.debug("AtmosphericRoutines calculation mode active")
 
         # Relative humidity (0.0 to 1.0)
@@ -62,17 +56,16 @@
         # Dew point temperature in Celsius
         # Air pressure at sea level in hPa
         # aerosol_density in kg/m^3
 
     # #####################################################
     # Calculate lifted index
     # #####################################################
-    async def calculate_lifted_index(
-        self, temperature, altitude, dew_point_temperature, air_pressure_at_sea_level
-    ):
+    async def calculate_lifted_index(self, temperature, altitude, dew_point_temperature, air_pressure_at_sea_level):
+        """Calculate atmospheric lifted index."""
         # https://en.wikipedia.org/wiki/Lifted_index
 
         if not all(
             v is not None
             for v in [
                 temperature,
                 altitude,
@@ -87,53 +80,40 @@
 
         # Calculate saturation vapor pressure at surface temperature
         # Checked with https://www.weather.gov/epz/wxcalc_vaporpressure
         es = self._calculate_vapor_pressure(temperature)
 
         # Calculate actual vapor pressure at surface
         # Checked with https://www.weather.gov/epz/wxcalc_vaporpressure
-        e = self._calculate_vapor_pressure(
-            dew_point_temperature
-        )  # 6.112 * (10 ** (7.5 * (Td - Tn) / (Td - 35.85)))
+        e = self._calculate_vapor_pressure(dew_point_temperature)  # 6.112 * (10 ** (7.5 * (Td - Tn) / (Td - 35.85)))
 
         # Calculate mixing ratio at surface in grams per kilogram
         # Checked with https://www.weather.gov/epz/wxcalc_mixingratio
         w = self._calculate_mixing_ratio(e, air_pressure_at_sea_level)
 
         # Calculate Lifting Condensation Level
         lcl = self._calculate_lifting_condensation_level(w, air_pressure_at_sea_level)
 
-        _LOGGER.debug(
-            "Air pressure at sea level (AP): {:.2f} mbar".format(
-                air_pressure_at_sea_level
-            )
-        )
-        _LOGGER.debug("Dew point(DP): {:.2f} °C".format(dew_point_temperature))
-        _LOGGER.debug("Temperature (T): {:.2f} °C".format(temperature))
-        _LOGGER.debug(
-            "Saturation vapor pressure at surface (ES): {:.2f} mbar".format(es)
-        )
-        _LOGGER.debug("Actual vapor pressure at surface (E): {:.2f} mbar".format(e))
-        _LOGGER.debug("Mixing ratio at surface (W): {:.2f} grams per kg".format(w))
-        _LOGGER.debug("Lifting Condensation Level (LCL): {:.2f} meters".format(lcl))
-
         # Calculate temperature of lifted parcel at 500 mb level
-        lifted_temp_500mb = (
-            env_temp_500mb + (temperature - lcl) * 0.5
-        )  # Assumption: 500 mb is halfway through the troposphere
+        lifted_temp_500mb = env_temp_500mb + (temperature - lcl) * 0.5  # Assumption: 500 mb is halfway through the troposphere
 
         # Calculate Lifted Index
         lifted_index = env_temp_500mb - lifted_temp_500mb
 
         _LOGGER.debug(
-            "Temperature of the lifted parcel (T Parcel): {:.2f} °C".format(
-                lifted_temp_500mb
-            )
+            "Lifted Index (LI): {:.2f} °C (".format(lifted_index)
+            + "Air pressure at sea level (AP): {:.2f} mbar, ".format(air_pressure_at_sea_level)
+            + "Dew point(DP): {:.2f} °C, ".format(dew_point_temperature)
+            + "Temperature (T): {:.2f} °C, ".format(temperature)
+            + "Saturation vapor pressure at surface (ES): {:.2f} mbar, ".format(es)
+            + "Actual vapor pressure at surface (E): {:.2f} mbar, ".format(e)
+            + "Mixing ratio at surface (W): {:.2f} grams per kg, ".format(w)
+            + "Lifting Condensation Level (LCL): {:.2f} meters, ".format(lcl)
+            + "Temperature of the lifted parcel (T Parcel): {:.2f} °C)".format(lifted_temp_500mb)
         )
-        _LOGGER.debug("Lifted Index (LI): {:.2f} °C".format(lifted_index))
 
         return lifted_index
 
     # #####################################################
     # Calculate magniture degradation based on transparency
     # #####################################################
     async def magnitude_degradation(
@@ -176,17 +156,15 @@
                 altitude,
                 dew_point_temperature,
                 air_pressure_at_sea_level,
             ]
         ):
             return None
 
-        lifted_index = await self.calculate_lifted_index(
-            temperature, altitude, dew_point_temperature, air_pressure_at_sea_level
-        )
+        lifted_index = await self.calculate_lifted_index(temperature, altitude, dew_point_temperature, air_pressure_at_sea_level)
         seeing = await self.calculate_seeing(
             temperature,
             humidity,
             dew_point_temperature,
             wind_speed,
             cloud_cover,
             altitude,
@@ -203,20 +181,22 @@
             dew_point_temperature,
             air_pressure_at_sea_level,
             lifted_index,
             seeing,
         )
 
         # Convert transparency to magnitude degradation
-        magnitude_degradation = self._transparency_to_magnitude_degradation(
-            transparency
-        )
+        magnitude_degradation = self._transparency_to_magnitude_degradation(transparency)
 
-        _LOGGER.debug("Estimated Atmospheric Transparency: {:.2f}".format(transparency))
-        _LOGGER.debug("Magnitude Degradation: {:.2f} mag".format(magnitude_degradation))
+        _LOGGER.debug(
+            "Magnitude Degradation: {:.2f} mag (".format(magnitude_degradation)
+            + "Lifted Index (LI): {:.2f} °C, ".format(lifted_index)
+            + "Seeing: {:.2f} arcsec, ".format(seeing)
+            + "Estimated Atmospheric Transparency: {:.2f})".format(transparency)
+        )
 
         return magnitude_degradation
 
     # #####################################################
     # Calculate atmospheric seeing
     # #####################################################
     # Modell 6:
@@ -248,14 +228,21 @@
         - wind_speed: Wind speed in meters per second.
         - cloud_cover: Cloud cover in Percent.
         - altitude: Altitude in meters.
         - air_pressure_at_sea_level: Air pressure at sea level.
 
         Returns:
         - seeing: In Arcsecs
+
+        Flow:
+        - _calculate_water_vapor_pressure
+        - adjusted_pressure
+        - relative_pressure
+        - seeing_factor
+        - seeing
         """
 
         if not all(
             v is not None
             for v in [
                 temperature,
                 humidity,
@@ -265,150 +252,104 @@
                 altitude,
                 air_pressure_at_sea_level,
             ]
         ):
             return None
 
         # Constants
-        C = 1.7
+        C = 6.5  # 1.7
 
-        water_vapor_pressure = self._calculate_water_vapor_pressure(
-            dew_point_temperature, humidity
-        )
+        water_vapor_pressure = self._calculate_water_vapor_pressure(dew_point_temperature, humidity)
 
-        adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
+        # adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
+        adjusted_pressure = self._calculate_adjusted_pressure(air_pressure_at_sea_level, altitude)
         relative_pressure = adjusted_pressure / air_pressure_at_sea_level
 
-        seeing_factor = (
-            C
-            * (water_vapor_pressure / 10) ** 0.35
-            * (wind_speed / 10) ** 0.65
-            * relative_pressure
-        )
+        # seeing_factor = (
+        #     C
+        #     * (water_vapor_pressure / 10) ** 0.25
+        #     * (wind_speed / 10) ** 0.75
+        #     * relative_pressure
+        # )
+        seeing_factor = C * (water_vapor_pressure / 10) ** 1 * relative_pressure
         seeing = 0.98 / seeing_factor
 
-        _LOGGER.debug("Water Vapor Pressure: {:.2f} mbar".format(water_vapor_pressure))
-        _LOGGER.debug("Relative Pressure: {:.2f} mbar".format(relative_pressure))
-        _LOGGER.debug("Seeing Factor: {:.2f}".format(seeing_factor))
-        _LOGGER.debug("Seeing: {:.2f} arcsec".format(seeing))
+        _LOGGER.debug(
+            "Seeing: {:.2f} arcsec (".format(seeing)
+            + "Water Vapor Pressure: {:.2f} mbar, ".format(water_vapor_pressure)
+            + "Wind Speed: {:.2f} m/s, ".format(wind_speed)
+            + "Relative Pressure: {:.2f} mbar, ".format(relative_pressure)
+            + "Seeing Factor: {:.2f})".format(seeing_factor)
+        )
 
         if seeing > SEEING_MAX:
             seeing = SEEING_MAX  # max out seeing
 
         return seeing
 
-    # Modell 7:
-    # This algorithm first calculates the seeing factor based on temperature, humidity, wind speed
-    # and altitude above sea level. It is similar to Model 6 but takes the cloud coverage into account.
-    # This somehow doesn't seem to be correct, since seeing can be good even with clouds.
-    async def calculate_seeing7(
-        self,
-        temperature,
-        humidity,
-        dew_point_temperature,
-        wind_speed,
-        cloud_cover,
-        altitude,
-        air_pressure_at_sea_level,
-    ):
+    # #####################################################
+    # Atmospheric calculations
+    # #####################################################
+    def _calculate_adjusted_pressure(self, pressure_sea_level, altitude):
         """
-        The seeing of the atmosphere calculated This algorithm first calculates the seeing factor based on temperature,
-        humidity, wind speed and altitude above sea level. The seeing factor is then used to calculate the astronomical
-        seeing in arcseconds. The empirical relationship used here states that the seeing in arcseconds is approximately
-        equal to the reciprocal of the seeing factor multiplied by a conversion factor of 0.98.
-
-        Used by: magnitude degradation
-
-        Args:
-        - temperature: Surface temperature in Celsius.
-        - humidity: Humidity in Percent.
-        - dew_point_temperature: Dew point temperature in Celsius.
-        - wind_speed: Wind speed in meters per second.
-        - cloud_cover: Cloud cover in Percent.
-        - altitude: Altitude in meters.
-        - air_pressure_at_sea_level: Air pressure at sea level.
-
-        Returns:
-        - seeing: In Arcsecs
+        Calculate the adjusted pressure at a given altitude above sea level.
         """
 
-        if not all(
-            v is not None
-            for v in [
-                temperature,
-                humidity,
-                dew_point_temperature,
-                wind_speed,
-                cloud_cover,
-                altitude,
-                air_pressure_at_sea_level,
-            ]
-        ):
-            return None
-
-        # Constants
-        C = 1.7
+        lapse_rate = -0.0065  # Temperature lapse rate in K/m
+        temperature_sea_level = 288.15  # Temperature at sea level in K
+        gravity = 9.80665  # Acceleration due to gravity in m/s^2
+        molar_mass_air = 0.02896  # Molar mass of Earth's air in kg/mol
+        gas_constant = 8.31447  # Universal gas constant in J/(mol*K)
 
-        water_vapor_pressure = self._calculate_water_vapor_pressure(
-            dew_point_temperature, humidity
+        pressure_adjusted = pressure_sea_level * (1 - (lapse_rate * altitude) / temperature_sea_level) ** (
+            (gravity * molar_mass_air) / (gas_constant * lapse_rate)
         )
 
-        adjusted_pressure = air_pressure_at_sea_level * math.exp(-0.00012 * altitude)
-        relative_pressure = adjusted_pressure / air_pressure_at_sea_level
-
-        # Take care on the clouds
-        cloud_factor = 1 - (cloud_cover / 100)
+        return pressure_adjusted
 
-        seeing_factor = (
-            C
-            * (water_vapor_pressure / 10) ** 0.2
-            * (wind_speed / 10) ** 0.6
-            * relative_pressure**0.3
-            * cloud_factor
-        )
-        if seeing_factor == 0:
-            seeing = 2.5  # max out seeing
-        else:
-            seeing = 0.98 / seeing_factor
-
-        _LOGGER.debug("Water Vapor Pressure: {:.2f} mbar".format(water_vapor_pressure))
-        _LOGGER.debug("Relative Pressure: {:.2f} mbar".format(relative_pressure))
-        _LOGGER.debug("Seeing Factor: {:.2f}".format(seeing_factor))
-        _LOGGER.debug("Seeing: {:.2f} arcsec".format(seeing))
-
-        if seeing > 2.5:
-            seeing = 2.5  # max out seeing
-
-        return seeing
-
-    # #####################################################
-    # Atmospheric calculations
-    # #####################################################
     def _calculate_vapor_pressure(self, temperature):
         """
         Calculate the actual or saturation vapor pressure at the surface using the Magnus-Tetens formula.
         If the surface temperature is given, the actual vapor pressure is calculated.
         The dew point temperature calculates ths saturation vapor pressure.
 
         Used by: lifted index, seeing
 
         Args:
         - temperature: Surface or dew point temperature in Celsius.
 
         Returns:
         - e: Actual vapor pressure at the surface in millibars (mb) or hectopascals (hPa).
-        """
 
-        # Constants
-        A = 6.112
-        B = 17.67
-        C = 243.5
+        Magnus coefficients:
+
+        Temperatures in between -45°C bis 60°C:
+            a=17.62
+            b=243.12
+        Temperatures in between 0°C bis 100°C:
+            a=7.5
+            b=237.7
+        Temperatures in between -10°C bis 50°C:
+            a=17.27
+            b=237.7
+        """
+        # # Constants
+        # A = 17.62
+        # B = 243.12
+
+        # # Monteith and Unsworth (2008) provide Tetens' formula for temperatures above 0 °C
+        A = 17.27
+        B = 237.3
+
+        # Murray (1967) provides Tetens' equation for temperatures below 0 °C
+        # A = 21.875
+        # B = 265.5
 
         # Calculate vapor pressure using Magnus-Tetens formula
-        e = A * math.exp((B * temperature) / (temperature + C))
+        e = 0.61078 * math.exp((A * temperature) / (temperature + B))
 
         return e
 
     def _calculate_water_vapor_pressure(self, dew_point_temperature, humidity):
         """
         Calculate the water vapor pressure based on temperature and humiditye.
 
@@ -467,18 +408,16 @@
         - lcl: LCL in meters
         """
 
         # Constants
         A = 2440
         B = 0.00029
 
-        # Calculate actual vapor pressure using Magnus-Tetens formula
-        lcl = (A * w) / (
-            (air_pressure_at_sea_level - w) * (1 - B * air_pressure_at_sea_level)
-        )
+        # Calculate Lifting Condensation Level using the Clausius-Clapeyron equation
+        lcl = (A * w) / ((air_pressure_at_sea_level - w) * (1 - B * air_pressure_at_sea_level))
 
         return lcl
 
     def _calculate_transparency(
         self,
         humidity,
         temperature,
@@ -508,76 +447,41 @@
         - w: Mixing ratio
 
         Returns:
         - transparency: In the range of 0 to 1
         """
 
         # Coefficients for the linear model (you can adjust these based on your requirements)
-        # humidity_coefficient = 0.02  # 0.02
-        # temperature_coefficient = 0.03  #0.03
-        # cloud_cover_coefficient = -0.1
-        # wind_speed_coefficient = -0.05
-        # altitude_coefficient = -0.01
-        # dew_point_temperature_coefficient = 0.02
-        # air_pressure_coefficient = 0.01
-
-        # temp_weight = 0.15
-        # humidity_weight = 0.15
-        # wind_weight = 0.10
-        # dew_point_weight = 0.15
-        # lifted_index_weight = 0.20
-        # seeing_weight = 0.15
-        # pressure_weight = 0.15
-        # cloud_cover_weight = 0.10
-        # altitude_weight = 0.10
-
-        # Constants
         temp_weight = 0.10
         humidity_weight = 0.10
         wind_weight = 0.10
         dew_point_weight = 0.10
         lifted_index_weight = 0.15
         seeing_weight = 0.15
         pressure_weight = 0.10
         cloud_cover_weight = 0.10
         altitude_weight = 0.10
 
         # Normalize values (optional)
-        temp_normalized = (temperature - (-10)) / (
-            40 - (-10)
-        )  # Assuming typical temperature range from -10°C to 40°C
+        # Assuming typical temperature range from -10°C to 40°C
+        temp_normalized = (temperature - (-10)) / (40 - (-10))
         humidity_normalized = humidity / 100.0
-        wind_normalized = (
-            wind_speed / 20.0
-        )  # Assuming maximum typical wind speed as 20 m/s
-        dew_point_normalized = (dew_point_temperature - (-10)) / (
-            30 - (-10)
-        )  # Assuming typical dew point range from -10°C to 30°C
-        lifted_index_normalized = (
-            lifted_index + 8
-        ) / 16.0  # Assuming lifted index range from -8 to 8
-        seeing_normalized = (
-            10 - seeing
-        ) / 10.0  # Assuming typical seeing conditions from 0 to 10 arcseconds
-        pressure_normalized = (air_pressure_at_sea_level - 900) / (
-            1100 - 900
-        )  # Assuming typical pressure range from 900 to 1100 mb
+        # Assuming maximum typical wind speed as 20 m/s
+        wind_normalized = wind_speed / 20.0
+        # Assuming typical dew point range from -10°C to 30°C
+        dew_point_normalized = (dew_point_temperature - (-10)) / (30 - (-10))
+        # Assuming lifted index range from -8 to 8
+        lifted_index_normalized = (lifted_index + 8) / 16.0
+        # Assuming typical seeing conditions from 0 to 10 arcseconds
+        seeing_normalized = (10 - seeing) / 10.0
+        # Assuming typical pressure range from 900 to 1100 mb
+        pressure_normalized = (air_pressure_at_sea_level - 900) / (1100 - 900)
         cloud_cover_normalized = cloud_cover / 100.0
-        altitude_normalized = (
-            altitude / 5000.0
-        )  # Assuming typical altitude range from 0 to 5000 meters
-
-        # Calculate transparency using the linear model
-        # transparency = (1 - (humidity * humidity_coefficient) +
-        #                 (temperature * temperature_coefficient) +
-        #                 (cloud_cover * cloud_cover_coefficient / 100) +
-        #                 (wind_speed * wind_speed_coefficient) +
-        #                 # (altitude * altitude_coefficient) +
-        #                 # (air_pressure_at_sea_level * air_pressure_coefficient) +
-        #                 (dew_point_temperature * dew_point_temperature_coefficient))
+        # Assuming typical altitude range from 0 to 5000 meters
+        altitude_normalized = altitude / 5000.0
 
         transparency = 1 - (
             temp_weight * temp_normalized
             + humidity_weight * humidity_normalized
             + wind_weight * wind_normalized
             + dew_point_weight * dew_point_normalized
             + lifted_index_weight * lifted_index_normalized
@@ -603,21 +507,18 @@
 
         Returns:
         - magniture_degradation: In magnitude.
         """
 
         if transparency == 0:
             return float(MAG_DEGRATION_MAX)
-        else:
-            magnitude_degradation = -MAG_DEGRATION_MAX * math.log(transparency)
-            magnitude_degradation = max(
-                0, min(MAG_DEGRATION_MAX, magnitude_degradation)
-            )
+        magnitude_degradation = -MAG_DEGRATION_MAX * math.log(transparency)
+        magnitude_degradation = max(0, min(MAG_DEGRATION_MAX, magnitude_degradation))
 
-            return magnitude_degradation
+        return magnitude_degradation
 
 
 class AstronomicalRoutines:
     """Calculate different astronomical objects."""
 
     def __init__(
         self,
@@ -723,217 +624,145 @@
         if self._sun_observer_astro is None:
             self._sun_observer_astro = self.get_sun_observer(ASTRONOMICAL_DUSK_DAWN)
         if self._sun is None:
             self._sun = ephem.Sun()
 
         # Rise and Setting (Civil)
         try:
-            self._sun_next_rising_civil = (
-                self._sun_observer.next_rising(ephem.Sun(), use_center=True)
-                .datetime()
-                .replace(tzinfo=UTC)
-            )
+            self._sun_next_rising_civil = self._sun_observer.next_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next rising
             start = self._sun_observer.date.datetime()
             end = self._sun_observer.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer.date = timestamp
                 try:
-                    self._sun_next_rising_astro = self._sun_observer.next_rising(
-                        ephem.Sun(), use_center=True
-                    ).datetime()
+                    self._sun_next_rising_astro = self._sun_observer.next_rising(ephem.Sun(), use_center=True).datetime()
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
-            self._sun_next_setting_civil = (
-                self._sun_observer.next_setting(ephem.Sun(), use_center=True)
-                .datetime()
-                .replace(tzinfo=UTC)
-            )
+            self._sun_next_setting_civil = self._sun_observer.next_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next setting
             start = self._sun_observer.date.datetime()
             end = self._sun_observer.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer.date = timestamp
                 try:
-                    self._sun_next_setting_astro = self._sun_observer.next_setting(
-                        ephem.Sun(), use_center=True
-                    ).datetime()
+                    self._sun_next_setting_astro = self._sun_observer.next_setting(ephem.Sun(), use_center=True).datetime()
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         # Rise and Setting (Nautical)
         self._sun_observer_nautical.date = self._forecast_time
         self._sun.compute(self._sun_observer_nautical)
 
         try:
-            self._sun_next_rising_nautical = (
-                self._sun_observer_nautical.next_rising(ephem.Sun(), use_center=True)
-                .datetime()
-                .replace(tzinfo=UTC)
-            )
+            self._sun_next_rising_nautical = self._sun_observer_nautical.next_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next astronomical rising
             start = self._sun_observer_nautical.date.datetime()
             end = self._sun_observer_nautical.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer_nautical.date = timestamp
                 try:
-                    self._sun_next_rising_nautical = (
-                        self._sun_observer_nautical.next_rising(
-                            ephem.Sun(), use_center=True
-                        )
-                        .datetime()
-                        .replace(tzinfo=UTC)
-                    )
+                    self._sun_next_rising_nautical = self._sun_observer_nautical.next_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
-            self._sun_next_setting_nautical = (
-                self._sun_observer_nautical.next_setting(ephem.Sun(), use_center=True)
-                .datetime()
-                .replace(tzinfo=UTC)
-            )
+            self._sun_next_setting_nautical = self._sun_observer_nautical.next_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next astronomical setting
             start = self._sun_observer_nautical.date.datetime()
             end = self._sun_observer_nautical.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer_nautical.date = timestamp
                 try:
-                    self._sun_next_setting_nautical = (
-                        self._sun_observer_nautical.next_setting(
-                            ephem.Sun(), use_center=True
-                        )
-                        .datetime()
-                        .replace(tzinfo=UTC)
-                    )
+                    self._sun_next_setting_nautical = self._sun_observer_nautical.next_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         # Rise and Setting (Astronomical)
         self._sun_observer_astro.date = self._forecast_time
         self._sun.compute(self._sun_observer_astro)
 
         try:
-            self._sun_next_rising_astro = (
-                self._sun_observer_astro.next_rising(ephem.Sun(), use_center=True)
-                .datetime()
-                .replace(tzinfo=UTC)
-            )
+            self._sun_next_rising_astro = self._sun_observer_astro.next_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next astronomical rising
             start = self._sun_observer_astro.date.datetime()
             end = self._sun_observer_astro.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer_astro.date = timestamp
                 try:
-                    self._sun_next_rising_astro = (
-                        self._sun_observer_astro.next_rising(
-                            ephem.Sun(), use_center=True
-                        )
-                        .datetime()
-                        .replace(tzinfo=UTC)
-                    )
+                    self._sun_next_rising_astro = self._sun_observer_astro.next_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
-            self._sun_previous_rising_astro = (
-                self._sun_observer_astro.previous_rising(ephem.Sun(), use_center=True)
-                .datetime()
-                .replace(tzinfo=UTC)
-            )
+            self._sun_previous_rising_astro = self._sun_observer_astro.previous_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the previous astronomical rising
             start = self._sun_observer_astro.date.datetime()
             end = self._sun_observer_astro.date.datetime() - timedelta(days=365)
             timestamp = start
             while timestamp > end:
                 timestamp -= timedelta(minutes=1440)
                 self._sun_observer_astro.date = timestamp
                 try:
-                    self._sun_previous_rising_astro = (
-                        self._sun_observer_astro.previous_rising(
-                            ephem.Sun(), use_center=True
-                        )
-                        .datetime()
-                        .replace(tzinfo=UTC)
-                    )
+                    self._sun_previous_rising_astro = self._sun_observer_astro.previous_rising(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
-            self._sun_next_setting_astro = (
-                self._sun_observer_astro.next_setting(ephem.Sun(), use_center=True)
-                .datetime()
-                .replace(tzinfo=UTC)
-            )
+            self._sun_next_setting_astro = self._sun_observer_astro.next_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the next astronomical setting
             start = self._sun_observer_astro.date.datetime()
             end = self._sun_observer_astro.date.datetime() + timedelta(days=365)
             timestamp = start
             while timestamp < end:
                 timestamp += timedelta(minutes=1440)
                 self._sun_observer_astro.date = timestamp
                 try:
-                    self._sun_next_setting_astro = (
-                        self._sun_observer_astro.next_setting(
-                            ephem.Sun(), use_center=True
-                        )
-                        .datetime()
-                        .replace(tzinfo=UTC)
-                    )
+                    self._sun_next_setting_astro = self._sun_observer_astro.next_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
         try:
-            self._sun_previous_setting_astro = (
-                self._sun_observer_astro.previous_setting(ephem.Sun(), use_center=True)
-                .datetime()
-                .replace(tzinfo=UTC)
-            )
+            self._sun_previous_setting_astro = self._sun_observer_astro.previous_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             # Search for the previous astronomical setting
             start = self._sun_observer_astro.date.datetime()
             end = self._sun_observer_astro.date.datetime() - timedelta(days=365)
             timestamp = start
             while timestamp > end:
                 timestamp -= timedelta(minutes=1440)
                 self._sun_observer_astro.date = timestamp
                 try:
-                    self._sun_previous_setting_astro = (
-                        self._sun_observer_astro.previous_setting(
-                            ephem.Sun(), use_center=True
-                        )
-                        .datetime()
-                        .replace(tzinfo=UTC)
-                    )
+                    self._sun_previous_setting_astro = self._sun_observer_astro.previous_setting(ephem.Sun(), use_center=True).datetime().replace(tzinfo=UTC)
                 except (ephem.AlwaysUpError, ephem.NeverUpError):
                     continue
                 break
 
     def calculate_sun_altaz(self):
         """Calculates sun altitude and azimuth."""
 
@@ -960,46 +789,30 @@
             self._moon = ephem.Moon()
 
         # Rise and Setting
         self._moon_observer.date = self._forecast_time
         self._moon.compute(self._moon_observer)
 
         try:
-            self._moon_next_rising = (
-                self._moon_observer.next_rising(ephem.Moon())
-                .datetime()
-                .replace(tzinfo=UTC)
-            )
+            self._moon_next_rising = self._moon_observer.next_rising(ephem.Moon()).datetime().replace(tzinfo=UTC)
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             pass
 
         try:
-            self._moon_next_setting = (
-                self._moon_observer.next_setting(ephem.Moon())
-                .datetime()
-                .replace(tzinfo=UTC)
-            )
+            self._moon_next_setting = self._moon_observer.next_setting(ephem.Moon()).datetime().replace(tzinfo=UTC)
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             pass
 
         try:
-            self._moon_previous_rising = (
-                self._moon_observer.previous_rising(ephem.Moon())
-                .datetime()
-                .replace(tzinfo=UTC)
-            )
+            self._moon_previous_rising = self._moon_observer.previous_rising(ephem.Moon()).datetime().replace(tzinfo=UTC)
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             pass
 
         try:
-            self._moon_previous_setting = (
-                self._moon_observer.previous_setting(ephem.Moon())
-                .datetime()
-                .replace(tzinfo=UTC)
-            )
+            self._moon_previous_setting = self._moon_observer.previous_setting(ephem.Moon()).datetime().replace(tzinfo=UTC)
         except (ephem.AlwaysUpError, ephem.NeverUpError):
             pass
 
         # self._moon_observer.date = self._forecast_time + timedelta(days=1)
         # self._moon.compute(self._moon_observer)
 
         # try:
@@ -1009,22 +822,18 @@
 
         # try:
         #     self._moon_day_after_next_setting = self._moon_observer.next_setting(ephem.Moon()).datetime().replace(tzinfo=UTC)
         # except (ephem.AlwaysUpError, ephem.NeverUpError):
         #     pass
 
         # Next new Moon
-        self._moon_next_new_moon = (
-            ephem.next_new_moon(self._forecast_time).datetime().replace(tzinfo=UTC)
-        )
+        self._moon_next_new_moon = ephem.next_new_moon(self._forecast_time).datetime().replace(tzinfo=UTC)
 
         # Next full Moon
-        self._moon_next_full_moon = (
-            ephem.next_full_moon(self._forecast_time).datetime().replace(tzinfo=UTC)
-        )
+        self._moon_next_full_moon = ephem.next_full_moon(self._forecast_time).datetime().replace(tzinfo=UTC)
 
     def calculate_moon_altaz(self):
         """Calculates moon altitude and azimuth."""
 
         if self._moon_observer is None:
             self._moon_observer = self.get_moon_observer()
         if self._moon is None:
@@ -1038,36 +847,26 @@
 
         # Moon Azimuth
         self._moon_azimuth = deg(float(self._moon.az))
 
     async def sun_previous_rising_astro(self) -> datetime:
         """Returns sun previous astronomical rising."""
 
-        if (
-            self._sun_previous_rising_astro is None
-            or self._forecast_time > self._sun_previous_rising_astro
-        ):
-            _LOGGER.debug(
-                "Astronomical calculations updating sun_previous_rising_astro"
-            )
+        if self._sun_previous_rising_astro is None or self._forecast_time > self._sun_previous_rising_astro:
+            _LOGGER.debug("Astronomical calculations updating sun_previous_rising_astro")
             self.calculate_sun()
 
         if self._sun_previous_rising_astro is not None:
             return self._sun_previous_rising_astro
 
     async def sun_previous_setting_astro(self) -> datetime:
         """Returns sun previous astronomical setting."""
 
-        if (
-            self._sun_previous_setting_astro is None
-            or self._forecast_time > self._sun_previous_setting_astro
-        ):
-            _LOGGER.debug(
-                "Astronomical calculations updating sun_previous_setting_astro"
-            )
+        if self._sun_previous_setting_astro is None or self._forecast_time > self._sun_previous_setting_astro:
+            _LOGGER.debug("Astronomical calculations updating sun_previous_setting_astro")
             self.calculate_sun()
 
         if self._sun_previous_setting_astro is not None:
             return self._sun_previous_setting_astro
 
     def astronomical_darkness(self) -> bool:
         """Returns true during astronomical night."""
@@ -1143,44 +942,35 @@
             return self._sun_next_rising_nautical
         if self._sun_next_rising_civil is not None:
             return self._sun_next_rising_civil
 
     async def sun_next_rising_civil(self) -> datetime:
         """Returns sun next rising."""
 
-        if (
-            self._sun_next_setting_civil is None
-            or self._forecast_time > self._sun_next_setting_civil
-        ):
+        if self._sun_next_setting_civil is None or self._forecast_time > self._sun_next_setting_civil:
             _LOGGER.debug("Astronomical calculations updating sun_next_rising_civil")
             self.calculate_sun()
 
         if self._sun_next_rising_civil is not None:
             return self._sun_next_rising_civil
 
     async def sun_next_rising_nautical(self) -> datetime:
         """Returns sun next nautical rising."""
 
-        if (
-            self._sun_next_rising_nautical is None
-            or self._forecast_time > self._sun_next_rising_nautical
-        ):
+        if self._sun_next_rising_nautical is None or self._forecast_time > self._sun_next_rising_nautical:
             _LOGGER.debug("Astronomical calculations updating sun_next_rising_nautical")
             self.calculate_sun()
 
         if self._sun_next_rising_nautical is not None:
             return self._sun_next_rising_nautical
 
     async def sun_next_rising_astro(self) -> datetime:
         """Returns sun next astronomical rising."""
 
-        if (
-            self._sun_next_rising_astro is None
-            or self._forecast_time > self._sun_next_rising_astro
-        ):
+        if self._sun_next_rising_astro is None or self._forecast_time > self._sun_next_rising_astro:
             _LOGGER.debug("Astronomical calculations updating sun_next_rising_astro")
             self.calculate_sun()
 
         if self._sun_next_rising_astro is not None:
             return self._sun_next_rising_astro
 
     async def sun_next_setting(self) -> datetime:
@@ -1203,46 +993,35 @@
             return self._sun_next_setting_nautical
         if self._sun_next_setting_civil is not None:
             return self._sun_next_setting_civil
 
     async def sun_next_setting_civil(self) -> datetime:
         """Returns sun next setting."""
 
-        if (
-            self._sun_next_setting_civil is None
-            or self._forecast_time > self._sun_next_setting_civil
-        ):
+        if self._sun_next_setting_civil is None or self._forecast_time > self._sun_next_setting_civil:
             _LOGGER.debug("Astronomical calculations updating sun_next_setting_civil")
             self.calculate_sun()
 
         if self._sun_next_setting_civil is not None:
             return self._sun_next_setting_civil
 
     async def sun_next_setting_nautical(self) -> datetime:
         """Returns sun next nautical setting."""
 
-        if (
-            self._sun_next_setting_nautical is None
-            or self._forecast_time > self._sun_next_setting_nautical
-        ):
-            _LOGGER.debug(
-                "Astronomical calculations updating sun_next_setting_nautical"
-            )
+        if self._sun_next_setting_nautical is None or self._forecast_time > self._sun_next_setting_nautical:
+            _LOGGER.debug("Astronomical calculations updating sun_next_setting_nautical")
             self.calculate_sun()
 
         if self._sun_next_setting_nautical is not None:
             return self._sun_next_setting_nautical
 
     async def sun_next_setting_astro(self) -> datetime:
         """Returns sun next astronomical setting."""
 
-        if (
-            self._sun_next_setting_astro is None
-            or self._forecast_time > self._sun_next_setting_astro
-        ):
+        if self._sun_next_setting_astro is None or self._forecast_time > self._sun_next_setting_astro:
             _LOGGER.debug("Astronomical calculations updating sun_next_setting_astro")
             self.calculate_sun()
 
         if self._sun_next_setting_astro is not None:
             return self._sun_next_setting_astro
 
     async def sun_altitude(self) -> float:
@@ -1261,31 +1040,25 @@
         if self._sun_azimuth is not None:
             return self._sun_azimuth
 
     # Return Moon information
     async def moon_next_rising(self) -> datetime:
         """Returns moon next rising."""
 
-        if (
-            self._moon_next_rising is None
-            or self._forecast_time > self._moon_next_rising
-        ):
+        if self._moon_next_rising is None or self._forecast_time > self._moon_next_rising:
             _LOGGER.debug("Astronomical calculations updating moon_next_rising")
             self.calculate_moon()
 
         if self._moon_next_rising is not None:
             return self._moon_next_rising
 
     async def moon_next_setting(self) -> datetime:
         """Returns moon next setting."""
 
-        if (
-            self._moon_next_setting is None
-            or self._forecast_time > self._moon_next_setting
-        ):
+        if self._moon_next_setting is None or self._forecast_time > self._moon_next_setting:
             _LOGGER.debug("Astronomical calculations updating moon_next_setting")
             self.calculate_moon()
 
         if self._moon_next_setting is not None:
             return self._moon_next_setting
 
     async def moon_phase(self) -> float:
@@ -1295,31 +1068,25 @@
 
         if self._moon is not None:
             return self._moon.phase
 
     async def moon_next_new_moon(self) -> float:
         """Returns the next new moon."""
 
-        if (
-            self._moon_next_new_moon is None
-            or self._forecast_time > self._moon_next_new_moon
-        ):
+        if self._moon_next_new_moon is None or self._forecast_time > self._moon_next_new_moon:
             _LOGGER.debug("Astronomical calculations updating moon_next_new_moon")
             self.calculate_moon()
 
         if self._moon_next_new_moon is not None:
             return self._moon_next_new_moon
 
     async def moon_next_full_moon(self) -> float:
         """Returns the next full moon."""
 
-        if (
-            self._moon_next_full_moon is None
-            or self._forecast_time > self._moon_next_full_moon
-        ):
+        if self._moon_next_full_moon is None or self._forecast_time > self._moon_next_full_moon:
             _LOGGER.debug("Astronomical calculations updating moon_next_full_moon")
             self.calculate_moon()
 
         if self._moon_next_full_moon is not None:
             return self._moon_next_full_moon
 
     async def moon_altitude(self) -> float:
@@ -1361,19 +1128,16 @@
 
         # Are we already in darkness?
         if self.astronomical_darkness():
             start_timestamp = self._sun_previous_setting_astro
         else:
             start_timestamp = self._sun_next_setting_astro
 
-        if (
-            self._moon_next_rising > start_timestamp
-            and self._moon_next_rising < self._sun_next_rising_astro
-        ):
-            _LOGGER.debug("DSD - Moon rises during astronomical night")
+        if self._moon_next_rising > start_timestamp and self._moon_next_rising < self._sun_next_rising_astro:
+            _LOGGER.debug("DSD: Moon rises during astronomical night")
             return True
         return False
 
     async def deep_sky_darkness_moon_sets(self) -> bool:
         """Returns true if moon sets during astronomical night."""
 
         start_timestamp = None
@@ -1386,99 +1150,90 @@
 
         # Did Moon already set in darkness?
         if self.moon_down() and self.astronomical_darkness():
             start_timestamp_moon = self._moon_previous_setting
         else:
             start_timestamp_moon = self._moon_next_setting
 
-        if (
-            start_timestamp_moon > start_timestamp
-            and start_timestamp_moon < self._sun_next_rising_astro
-        ):
-            _LOGGER.debug("DSD - Moon sets during astronomical night")
+        if start_timestamp_moon > start_timestamp and start_timestamp_moon < self._sun_next_rising_astro:
+            _LOGGER.debug("DSD: Moon sets during astronomical night")
             return True
         return False
 
     async def deep_sky_darkness_moon_always_up(self) -> bool:
         """Returns true if moon is up during astronomical night."""
 
         start_timestamp = None
 
         # Are we already in darkness?
         if self.astronomical_darkness():
             start_timestamp = self._sun_previous_setting_astro
         else:
             start_timestamp = self._sun_next_setting_astro
 
-        if (
-            self._moon_next_rising < start_timestamp
-            and self._moon_next_setting > self._sun_next_rising_astro
-        ):
-            _LOGGER.debug("DSD - Moon is up during astronomical night")
+        if self._moon_next_rising < start_timestamp and self._moon_next_setting > self._sun_next_rising_astro:
+            _LOGGER.debug("DSD: Moon is up during astronomical night")
             return True
         return False
 
     async def deep_sky_darkness_moon_always_down(self) -> bool:
         """Returns true if moon is down during astronomical night."""
 
         start_timestamp = None
 
         # Are we already in darkness?
         if self.astronomical_darkness():
             start_timestamp = self._sun_previous_setting_astro
         else:
             start_timestamp = self._sun_next_setting_astro
 
-        if (
-            self._moon_previous_setting < start_timestamp
-            and self._moon_next_rising > self._sun_next_rising_astro
-        ):
-            _LOGGER.debug("DSD - Moon is down during astronomical night")
+        if self._moon_previous_setting < start_timestamp and self._moon_next_rising > self._sun_next_rising_astro:
+            _LOGGER.debug("DSD: Moon is down during astronomical night")
             return True
         return False
 
     async def deep_sky_darkness(self) -> float:
         """Returns the remaining timespan of deep sky darkness."""
 
         dsd = timedelta(0)
 
         if self.astronomical_darkness():
-            _LOGGER.debug(f"DSD - In astronomical darkness")
+            _LOGGER.debug(f"DSD: In astronomical darkness")
             if await self.deep_sky_darkness_moon_rises():
                 dsd = self._moon_next_rising - self._forecast_time
-                _LOGGER.debug(f"DSD - Sun down, Moon rises {dsd}")
+                _LOGGER.debug(f"DSD: Sun down, Moon rises {dsd}")
 
             if await self.deep_sky_darkness_moon_sets():
                 if self.moon_down():
                     dsd = self._sun_next_rising_astro - self._forecast_time
-                    _LOGGER.debug(f"DSD - Sun down, Moon is down {dsd}")
+                    _LOGGER.debug(f"DSD: Sun down, Moon is down {dsd}")
                 else:
                     dsd = self._sun_next_rising_astro - self._moon_next_setting
-                    _LOGGER.debug(f"DSD - Sun down, Moon sets {dsd}")
+                    _LOGGER.debug(f"DSD: Sun down, Moon sets {dsd}")
 
             if await self.deep_sky_darkness_moon_always_down():
                 dsd = self._sun_next_rising_astro - self._forecast_time
-                _LOGGER.debug(f"DSD - Moon always down {dsd}")
+                _LOGGER.debug(f"DSD: Moon always down {dsd}")
             else:
-                _LOGGER.debug(f"DSD - Moon NOT always down {dsd}")
+                _LOGGER.debug(f"DSD: Moon NOT always down {dsd}")
 
         if not self.astronomical_darkness():
-            _LOGGER.debug(f"DSD - At sunlight")
+            _LOGGER.debug(f"DSD: At sunlight")
             if await self.deep_sky_darkness_moon_rises():
                 dsd = self._moon_next_rising - self._sun_next_setting_astro
-                _LOGGER.debug(f"DSD - Sun up, Moon rises {dsd}")
+                _LOGGER.debug(f"DSD: Sun up, Moon rises {dsd}")
 
             if await self.deep_sky_darkness_moon_sets():
                 dsd = self._sun_next_rising_astro - self._moon_next_setting
-                _LOGGER.debug(f"DSD - Sun up, Moon sets {dsd}")
+                _LOGGER.debug(f"DSD: Sun up, Moon sets {dsd}")
 
             if await self.deep_sky_darkness_moon_always_down():
                 dsd = self._sun_next_rising_astro - self._sun_next_setting_astro
-                _LOGGER.debug(f"DSD - Sun up, Moon down {dsd}")
+                _LOGGER.debug(f"DSD: Sun up, Moon down {dsd}")
 
         if await self.deep_sky_darkness_moon_always_up():
             dsd = timedelta(0)
-            _LOGGER.debug(f"DSD - Moon always up {dsd}")
+            _LOGGER.debug(f"DSD: Moon always up {dsd}")
         else:
-            _LOGGER.debug(f"DSD - Moon NOT always up {dsd}")
+            _LOGGER.debug(f"DSD: Moon NOT always up {dsd}")
 
         return dsd.total_seconds()
```

### Comparing `pyastroweatherio-0.50.0.dev13/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.50.1/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.50.0.dev13
+Version: 0.50.1
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.50.0.dev13/setup.py` & `pyastroweatherio-0.50.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.50.0.dev13",
+    version="0.50.1",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

