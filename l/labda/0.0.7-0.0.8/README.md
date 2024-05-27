# Comparing `tmp/labda-0.0.7.tar.gz` & `tmp/labda-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labda-0.0.7.tar", max compression
+gzip compressed data, was "labda-0.0.8.tar", max compression
```

## Comparing `labda-0.0.7.tar` & `labda-0.0.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      548 2024-05-15 11:09:04.880673 labda-0.0.7/CHANGELOG.md
--rw-r--r--   0        0        0      219 2024-05-15 11:09:04.890673 labda-0.0.7/LICENSE.md
--rw-r--r--   0        0        0      916 2024-05-15 11:09:04.890673 labda-0.0.7/README.md
--rw-r--r--   0        0        0      183 2024-05-15 11:09:04.890673 labda-0.0.7/labda/__init__.py
--rw-r--r--   0        0        0      142 2024-03-26 12:17:08.741130 labda-0.0.7/labda/assets/__init__.py
--rw-r--r--   0        0        0     1195 2024-03-26 15:39:19.404282 labda-0.0.7/labda/assets/counts_cut_points.py
--rw-r--r--   0        0        0      808 2024-05-02 13:33:35.759080 labda-0.0.7/labda/assets/transportation_cut_points.py
--rw-r--r--   0        0        0      152 2024-02-06 17:52:16.176389 labda-0.0.7/labda/expanders/__init__.py
--rw-r--r--   0        0        0      656 2024-03-26 07:45:27.272975 labda-0.0.7/labda/expanders/accelerometer.py
--rw-r--r--   0        0        0      964 2024-03-26 07:45:27.272975 labda-0.0.7/labda/expanders/extras.py
--rw-r--r--   0        0        0     7377 2024-04-02 08:48:51.335892 labda-0.0.7/labda/expanders/spatial.py
--rw-r--r--   0        0        0     1238 2024-05-16 07:03:10.802566 labda-0.0.7/labda/logging.py
--rw-r--r--   0        0        0     1163 2024-05-15 11:09:04.890673 labda-0.0.7/labda/parallel.py
--rw-r--r--   0        0        0      201 2024-04-23 07:15:17.838214 labda-0.0.7/labda/parsers/__init__.py
--rw-r--r--   0        0        0     6852 2024-05-15 11:09:04.890673 labda-0.0.7/labda/parsers/actigraph.py
--rw-r--r--   0        0        0     1013 2024-05-15 11:09:04.890673 labda-0.0.7/labda/parsers/bulk.py
--rw-r--r--   0        0        0     6508 2024-04-08 08:01:34.897150 labda-0.0.7/labda/parsers/gadgetbridge.py
--rw-r--r--   0        0        0     2332 2024-02-06 17:52:16.176389 labda-0.0.7/labda/parsers/garmin.py
--rw-r--r--   0        0        0    10993 2024-05-15 11:09:04.890673 labda-0.0.7/labda/parsers/qstarz.py
--rw-r--r--   0        0        0     8586 2024-05-15 12:06:39.577189 labda-0.0.7/labda/parsers/sens.py
--rw-r--r--   0        0        0     8898 2024-05-15 12:06:18.811945 labda-0.0.7/labda/parsers/traccar.py
--rw-r--r--   0        0        0       37 2024-05-15 11:09:04.890673 labda-0.0.7/labda/processing/__init__.py
--rw-r--r--   0        0        0       88 2024-03-26 13:31:05.536930 labda-0.0.7/labda/processing/accelerometer/__init__.py
--rw-r--r--   0        0        0     1580 2024-03-26 13:51:21.538869 labda-0.0.7/labda/processing/accelerometer/activity_intensity.py
--rw-r--r--   0        0        0      616 2024-03-26 07:45:27.282975 labda-0.0.7/labda/processing/accelerometer/steps.py
--rw-r--r--   0        0        0      913 2024-03-26 07:45:27.282975 labda-0.0.7/labda/processing/accelerometer/wear.py
--rw-r--r--   0        0        0     2803 2024-03-26 07:45:27.282975 labda-0.0.7/labda/processing/bouts.py
--rw-r--r--   0        0        0     2635 2024-05-15 11:09:04.890673 labda-0.0.7/labda/processing/context.py
--rw-r--r--   0        0        0      488 2024-03-26 07:45:27.282975 labda-0.0.7/labda/processing/manipulations.py
--rw-r--r--   0        0        0      197 2024-03-26 14:28:15.353873 labda-0.0.7/labda/processing/spatial/__init__.py
--rw-r--r--   0        0        0     6142 2024-04-02 09:39:10.496322 labda-0.0.7/labda/processing/spatial/manipulations.py
--rw-r--r--   0        0        0     3277 2024-04-03 14:44:06.593954 labda-0.0.7/labda/processing/spatial/timeline.py
--rw-r--r--   0        0        0     3792 2024-05-01 14:19:00.081204 labda-0.0.7/labda/processing/spatial/transportation.py
--rw-r--r--   0        0        0    26117 2024-05-02 13:42:51.176141 labda-0.0.7/labda/processing/spatial/trips.py
--rw-r--r--   0        0        0     2247 2024-03-05 08:22:02.089665 labda-0.0.7/labda/processing/wear_validity.py
--rw-r--r--   0        0        0      252 2024-05-15 11:09:04.890673 labda-0.0.7/labda/structure/__init__.py
--rw-r--r--   0        0        0     4852 2024-05-15 11:09:04.890673 labda-0.0.7/labda/structure/collection.py
--rw-r--r--   0        0        0     2595 2024-05-15 11:09:04.890673 labda-0.0.7/labda/structure/contexts.py
--rw-r--r--   0        0        0      600 2024-04-08 08:01:34.897150 labda-0.0.7/labda/structure/linkage.py
--rw-r--r--   0        0        0     8790 2024-05-16 07:03:10.802566 labda-0.0.7/labda/structure/merging.py
--rw-r--r--   0        0        0     3423 2024-05-16 07:03:10.802566 labda-0.0.7/labda/structure/resampling.py
--rw-r--r--   0        0        0    15046 2024-05-16 08:08:03.793217 labda-0.0.7/labda/structure/subject.py
--rw-r--r--   0        0        0        0 2024-03-26 07:45:27.282975 labda-0.0.7/labda/structure/validation/__init__.py
--rw-r--r--   0        0        0     1337 2024-05-15 11:09:04.890673 labda-0.0.7/labda/structure/validation/context.py
--rw-r--r--   0        0        0      833 2024-02-09 12:37:10.070190 labda-0.0.7/labda/structure/validation/linkage.py
--rw-r--r--   0        0        0    11339 2024-05-15 11:09:04.890673 labda-0.0.7/labda/structure/validation/subject.py
--rw-r--r--   0        0        0     9961 2024-05-15 11:09:04.890673 labda-0.0.7/labda/utils.py
--rw-r--r--   0        0        0        0 2024-02-06 17:52:16.176389 labda-0.0.7/labda/visualisation/__init__.py
--rw-r--r--   0        0        0     3785 2024-05-15 11:09:04.890673 labda-0.0.7/labda/visualisation/spatial.py
--rw-r--r--   0        0        0     1670 2024-05-16 08:35:54.413823 labda-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 labda-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      294 2024-05-27 07:21:21.966442 labda-0.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0      219 2024-05-06 14:08:06.476463 labda-0.0.8/LICENSE.md
+-rw-r--r--   0        0        0      949 2024-05-27 07:21:21.976442 labda-0.0.8/README.md
+-rw-r--r--   0        0        0      183 2024-05-11 06:11:49.000349 labda-0.0.8/labda/__init__.py
+-rw-r--r--   0        0        0      142 2024-04-17 03:56:15.837647 labda-0.0.8/labda/assets/__init__.py
+-rw-r--r--   0        0        0     1195 2024-04-17 03:56:15.837647 labda-0.0.8/labda/assets/counts_cut_points.py
+-rw-r--r--   0        0        0      808 2024-05-06 14:08:06.646463 labda-0.0.8/labda/assets/transportation_cut_points.py
+-rw-r--r--   0        0        0      152 2024-04-17 03:56:15.837647 labda-0.0.8/labda/expanders/__init__.py
+-rw-r--r--   0        0        0      656 2024-04-17 03:56:15.837647 labda-0.0.8/labda/expanders/accelerometer.py
+-rw-r--r--   0        0        0      964 2024-04-17 03:56:15.837647 labda-0.0.8/labda/expanders/extras.py
+-rw-r--r--   0        0        0     7377 2024-04-17 03:56:15.837647 labda-0.0.8/labda/expanders/spatial.py
+-rw-r--r--   0        0        0     1238 2024-05-27 07:21:22.236442 labda-0.0.8/labda/logging.py
+-rw-r--r--   0        0        0     1163 2024-05-09 08:50:19.212123 labda-0.0.8/labda/parallel.py
+-rw-r--r--   0        0        0      201 2024-05-06 14:08:06.646463 labda-0.0.8/labda/parsers/__init__.py
+-rw-r--r--   0        0        0     6852 2024-05-09 16:16:33.961740 labda-0.0.8/labda/parsers/actigraph.py
+-rw-r--r--   0        0        0     1013 2024-05-09 08:47:40.902125 labda-0.0.8/labda/parsers/bulk.py
+-rw-r--r--   0        0        0     6508 2024-04-17 03:56:15.837647 labda-0.0.8/labda/parsers/gadgetbridge.py
+-rw-r--r--   0        0        0     2332 2024-04-17 03:56:15.837647 labda-0.0.8/labda/parsers/garmin.py
+-rw-r--r--   0        0        0    10993 2024-05-09 16:26:39.781731 labda-0.0.8/labda/parsers/qstarz.py
+-rw-r--r--   0        0        0     8566 2024-05-27 07:21:22.236442 labda-0.0.8/labda/parsers/sens.py
+-rw-r--r--   0        0        0     9835 2024-05-27 07:21:22.236442 labda-0.0.8/labda/parsers/traccar.py
+-rw-r--r--   0        0        0       37 2024-05-09 16:43:23.301717 labda-0.0.8/labda/processing/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/accelerometer/__init__.py
+-rw-r--r--   0        0        0     1580 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/accelerometer/activity_intensity.py
+-rw-r--r--   0        0        0      616 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/accelerometer/steps.py
+-rw-r--r--   0        0        0      913 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/accelerometer/wear.py
+-rw-r--r--   0        0        0     2803 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/bouts.py
+-rw-r--r--   0        0        0     2635 2024-05-11 12:15:33.238139 labda-0.0.8/labda/processing/context.py
+-rw-r--r--   0        0        0      536 2024-05-27 07:21:22.236442 labda-0.0.8/labda/processing/manipulations.py
+-rw-r--r--   0        0        0      197 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/spatial/__init__.py
+-rw-r--r--   0        0        0     6880 2024-05-27 07:21:22.236442 labda-0.0.8/labda/processing/spatial/manipulations.py
+-rw-r--r--   0        0        0     3277 2024-04-17 03:56:15.837647 labda-0.0.8/labda/processing/spatial/timeline.py
+-rw-r--r--   0        0        0     3797 2024-05-27 07:21:22.236442 labda-0.0.8/labda/processing/spatial/transportation.py
+-rw-r--r--   0        0        0    26484 2024-05-27 07:21:22.236442 labda-0.0.8/labda/processing/spatial/trips.py
+-rw-r--r--   0        0        0     2622 2024-05-27 07:21:22.236442 labda-0.0.8/labda/processing/wear_validity.py
+-rw-r--r--   0        0        0      252 2024-05-11 06:12:01.210349 labda-0.0.8/labda/structure/__init__.py
+-rw-r--r--   0        0        0     5196 2024-05-27 07:21:22.236442 labda-0.0.8/labda/structure/collection.py
+-rw-r--r--   0        0        0     2595 2024-05-11 07:41:03.550336 labda-0.0.8/labda/structure/contexts.py
+-rw-r--r--   0        0        0      600 2024-04-17 03:56:15.847647 labda-0.0.8/labda/structure/linkage.py
+-rw-r--r--   0        0        0     8766 2024-05-27 07:21:22.236442 labda-0.0.8/labda/structure/merging.py
+-rw-r--r--   0        0        0     3435 2024-05-27 07:21:22.236442 labda-0.0.8/labda/structure/resampling.py
+-rw-r--r--   0        0        0    20115 2024-05-27 07:21:22.236442 labda-0.0.8/labda/structure/subject.py
+-rw-r--r--   0        0        0        0 2024-04-17 03:56:15.847647 labda-0.0.8/labda/structure/validation/__init__.py
+-rw-r--r--   0        0        0     1337 2024-05-09 14:43:53.361819 labda-0.0.8/labda/structure/validation/context.py
+-rw-r--r--   0        0        0      833 2024-04-17 03:56:15.847647 labda-0.0.8/labda/structure/validation/linkage.py
+-rw-r--r--   0        0        0    11339 2024-05-11 12:15:54.098139 labda-0.0.8/labda/structure/validation/subject.py
+-rw-r--r--   0        0        0     9961 2024-05-09 16:15:48.251740 labda-0.0.8/labda/utils.py
+-rw-r--r--   0        0        0        0 2024-02-03 08:38:41.168015 labda-0.0.8/labda/visualisation/__init__.py
+-rw-r--r--   0        0        0     3785 2024-05-11 09:52:34.810315 labda-0.0.8/labda/visualisation/spatial.py
+-rw-r--r--   0        0        0     1697 2024-05-27 07:21:33.146442 labda-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 labda-0.0.8/PKG-INFO
```

### Comparing `labda-0.0.7/README.md` & `labda-0.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # LABDA: Library for Advanced Behavioural Data Analysis
 
 [![pypi](https://img.shields.io/pypi/v/labda.svg)](https://pypi.python.org/pypi/labda)
 [![downloads](https://static.pepy.tech/badge/labda/month)](https://pepy.tech/project/labda)
 [![versions](https://img.shields.io/pypi/pyversions/labda.svg)](https://github.com/josefheidler/labda)
-![discord](https://img.shields.io/discord/1165947556807848016)
+[![discord](https://img.shields.io/discord/1165947556807848016)](https://discord.gg/qu6ax5Q64j)
 
 **LABDA is currently under development and may undergo significant API changes that could result in breaking changes.**
 
 ## What is it?
 
 TO-DO...
```

### Comparing `labda-0.0.7/labda/assets/counts_cut_points.py` & `labda-0.0.8/labda/assets/counts_cut_points.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/assets/transportation_cut_points.py` & `labda-0.0.8/labda/assets/transportation_cut_points.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/expanders/accelerometer.py` & `labda-0.0.8/labda/expanders/accelerometer.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/expanders/extras.py` & `labda-0.0.8/labda/expanders/extras.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/expanders/spatial.py` & `labda-0.0.8/labda/expanders/spatial.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/logging.py` & `labda-0.0.8/labda/logging.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/parallel.py` & `labda-0.0.8/labda/parallel.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/parsers/actigraph.py` & `labda-0.0.8/labda/parsers/actigraph.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/parsers/bulk.py` & `labda-0.0.8/labda/parsers/bulk.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/parsers/gadgetbridge.py` & `labda-0.0.8/labda/parsers/gadgetbridge.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/parsers/garmin.py` & `labda-0.0.8/labda/parsers/garmin.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/parsers/qstarz.py` & `labda-0.0.8/labda/parsers/qstarz.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/parsers/sens.py` & `labda-0.0.8/labda/parsers/sens.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         path (str | Path): The path to the CSV file.
         subject_id (str, optional): The ID of the subject. If not provided, it will be set to the file name.
         start (datetime, optional): The start time of the data to fetch. If not provided, it will fetch all available data.
         end (datetime, optional): The end time of the data to fetch. If not provided, it will fetch all available data.
         sampling_frequency (float, optional): The sampling frequency of the data. If not provided, it will be infered from data.
         timezone (str, optional): The timezone of the data. If None it will be set to the local timezone. Otherwise, it will be set to the provided timezone.
         sensor_id (str, optional): The ID of the sensor. If not provided, it will be set to the file name.
-        vendor (Vendor, optional): The vendor of the sensor. Defaults to "Sens".
+        vendor (Vendor, optional): The vendor of the sensor.
         model (str, optional): The model of the sensor.
         serial_number (str, optional): The serial number of the sensor.
         firmware_version (str, optional): The firmware version of the sensor.
 
 
     Returns:
         Subject: A Subject object containing the fetched and processed dataframe containing information: datetime, wear, position, steps, activity_intensity, activity_value and activity.
```

### Comparing `labda-0.0.7/labda/parsers/traccar.py` & `labda-0.0.8/labda/parsers/traccar.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,23 @@
     change_crs,
     change_timezone,
     get_crs,
     get_sampling_frequency,
     get_timezone,
 )
 
+# TODO: Environment determination based on GNSS_ACCURACY, not accurate points should be removed, others should be considered as indoor or outdoor points
+# (for example, remove points with accuracy over 1000 -> no signal, points with less -> 100 should be indoor, other outdoor), something like that, or actually option to specify the limit or to remove - multiple ways, but still one parameter.
+
+
+def _remove_not_accurate_points(df: pd.DataFrame, limit: int | float) -> pd.DataFrame:
+    # Unit defaults to meters
+    # TODO: Best value needs to be determined.
+    return df[df[Column.GNSS_ACCURACY] <= limit]
+
 
 def _knots_to_kmh(knots):
     return knots * 1.852
 
 
 def _get_device(
     url: str,
@@ -159,14 +168,15 @@
     crs: str | None = "infer",
     timezone: str | None = "infer",
     sensor_id: str | None = None,
     vendor: Vendor = Vendor.TRACCAR,
     model: str | None = None,
     serial_number: str | None = None,
     firmware_version: str | None = None,
+    accuracy: int | float | None = None,
 ) -> Subject:
     """
     The Traccar API allows you to download data from a specific server (URL) using your login credentials (username and password). To obtain data for a particular device, you must specify a subject ID (which corresponds to the device identifier). Optionally, you can define a date and time range to download data for a specific timeframe. If no date range is provided (from/to), all data for the chosen device will be downloaded.
 
     The downloaded data will be parsed and validated according to the schema defined in the structure module.
 
     Args:
@@ -180,14 +190,15 @@
         timezone (str, optional): The timezone of the data. If set to "infer" it will be inferred from the data. If None it will be set to the local timezone. Otherwise, it will be set to the provided timezone.
         crs (str, optional): The coordinate reference system (CRS) of the data. If set to "infer" it will be inferred from the data. If None it will be set to "EPSG:4326". Otherwise, it will be set to the provided CRS.
         sensor_id (str, optional): The ID of the sensor to fetch data for. If not provided, unique device ID from Traccar server will be used (if available).
         vendor (Vendor, optional): The vendor of the device. Defaults to "Traccar".
         model (str, optional): The model of the device. If not provided, it will be fetched from the Traccar server (device - extra, phone + model) if available.
         serial_number (str, optional): The serial number of the device.
         firmware_version (str, optional): The firmware version of the device.
+        accuracy (int | float, optional): The maximum allowed GPS accuracy. If not provided, all points will be included, otherwise only points with accuracy less or equal to the provided value will be included.
 
     Returns:
         Subject: A Subject object containing the fetched and processed dataframe containing information: datetime, latitude, longitude, gps_accuracy, distance, elevation, and speed.
 
 
     Raises:
         HTTPError: HTTP request to the Traccar server failed.
@@ -241,14 +252,17 @@
         df = change_crs(df, origin_crs, crs)
 
     if not sampling_frequency:
         sampling_frequency = get_sampling_frequency(df)
 
     df = align_datetimes(df, sampling_frequency)
 
+    if accuracy:
+        df = _remove_not_accurate_points(df, accuracy)
+
     # Order columns as defined in Column, remove extra columns
     records_columns = [col.value for col in Column]
     ordered_columns = [col for col in records_columns if col in df.columns]
     df = df[ordered_columns]
 
     df = SCHEMA.validate(df)
```

### Comparing `labda-0.0.7/labda/processing/accelerometer/activity_intensity.py` & `labda-0.0.8/labda/processing/accelerometer/activity_intensity.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/processing/accelerometer/steps.py` & `labda-0.0.8/labda/processing/accelerometer/steps.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/processing/accelerometer/wear.py` & `labda-0.0.8/labda/processing/accelerometer/wear.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/processing/bouts.py` & `labda-0.0.8/labda/processing/bouts.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/processing/context.py` & `labda-0.0.8/labda/processing/context.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/processing/spatial/manipulations.py` & `labda-0.0.8/labda/processing/spatial/manipulations.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,14 +65,35 @@
                 df.loc[selected_rows.index, name] = True
 
             buffer.popleft()
 
     return df.astype({name: "boolean"})
 
 
+def speed_splitter(
+    df: pd.DataFrame,
+    *,
+    max_speed: int | float,
+    crs: str | None = None,
+    name: str = "segment",
+    overwrite: bool = False,
+) -> pd.DataFrame:
+    columns_not_exists(df, [name], overwrite=overwrite)
+    df = df.copy()
+
+    speed_colname = get_unique_column_name(df)
+    df = add_speed(df, crs=crs, name=speed_colname)
+
+    df[name] = df[speed_colname] > max_speed  # type: ignore
+    df[name] = df[name].apply(lambda x: 1 if x else 0).cumsum() + 1
+    df.drop(columns=[speed_colname], inplace=True)
+
+    return df.astype({name: "UInt16"})
+
+
 def min_distance_filter(
     df: pd.DataFrame,
     *,
     min_distance: int | float,
     crs: str | None = None,
     name: str = "min_distance",
     overwrite: bool = False,
@@ -123,14 +144,16 @@
     df: pd.DataFrame,
     *,
     max_speed: int | float | None = None,
     crs: str | None = None,
     name: str = "max_speed",
     overwrite: bool = False,
 ) -> pd.DataFrame:
+    # TODO: Do not use this filter yet.
+    # FIXME: Maybe rework it, because now it deletes all the consecutive points until the speed is below the threshold.
     """
     Filters the DataFrame based on the maximum speed value.
 
     Args:
         df (pd.DataFrame): The input DataFrame.
         max_speed (int | float): The maximum speed value to filter by.
         crs (str | None, optional): The coordinate reference system. Defaults to None.
```

### Comparing `labda-0.0.7/labda/processing/spatial/timeline.py` & `labda-0.0.8/labda/processing/spatial/timeline.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/processing/spatial/transportation.py` & `labda-0.0.8/labda/processing/spatial/transportation.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 def _fill_trip_mode_pauses(df: pd.DataFrame, fill: str) -> pd.DataFrame:
     if fill == "forward":
         df[Column.TRIP_MODE] = df[Column.TRIP_MODE].ffill()
     elif fill == "backward":
         df[Column.TRIP_MODE] = df[Column.TRIP_MODE].bfill()
     else:
-        raise ValueError("fill must be either 'ffill' or 'bfill'")
+        raise ValueError("fill must be either 'forward' or 'backward'")
 
     return df
 
 
 def _set_trip_mode(df: pd.DataFrame, name: str):
     modes = df[name].value_counts()
     dominant_mode = modes.idxmax()
```

### Comparing `labda-0.0.7/labda/processing/spatial/trips.py` & `labda-0.0.8/labda/processing/spatial/trips.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 from ...expanders import add_distance
 from ...structure.validation.subject import SCHEMA
 from ...utils import (
     columns_not_exists,
     convert_distance_parameter,
 )
 from ..manipulations import gap_splitter
-from .manipulations import max_speed_filter, min_distance_filter, stop_splitter
+from .manipulations import (
+    min_distance_filter,
+    speed_splitter,
+    stop_splitter,
+)
 
 # TODO: Fix docstring.
 # TODO: Change column names to constants (Column).
 
 
 def _get_trips(
     df: pd.DataFrame,
@@ -338,14 +342,15 @@
         mask = df.set_index(["segment_id", "trip_id"]).index.isin(
             removed_trips.set_index(["segment_id", "trip_id"]).index
         )
         df.loc[mask, "trip_id"] = pd.NA
         # df.loc[mask, "trip_status"] = (
         #     pd.NA  # HACK: Possibly set this to "stationary" if removed trips should be part of locations, but then need to adjust the stationary_id as well.
         # )
+        # FIXME: This should be propably NA, because it is not stationary, but it is not a trip either.
         df.loc[mask, "trip_status"] = "stationary"
         df.loc[mask, "stationary_id"] = df.loc[mask, "stationary_id"].ffill()
 
 
 def _change_indoor_trip_to_stationary(df: pd.DataFrame, limit: float) -> str | None:
     environment = df["environment"].value_counts()
     dominant_environment = environment.idxmax()
@@ -383,28 +388,28 @@
         mask = df.set_index(["segment_id", "trip_id"]).index.isin(
             removed_trips.set_index(["segment_id", "trip_id"]).index
         )
         df.loc[mask, "trip_id"] = pd.NA
         # df.loc[mask, "trip_status"] = (
         #     pd.NA  # HACK: Possibly set this to "stationary" if removed trips should be part of locations, but then need to adjust the stationary_id as well.
         # )
+        # FIXME: This should be propably NA, because it is not stationary, but it is not a trip either.
         df.loc[mask, "trip_status"] = "stationary"
         df.loc[mask, "stationary_id"] = df.loc[mask, "stationary_id"].bfill()
 
 
 def _get_segment_trips(
     df: pd.DataFrame,
     crs: str,
     sampling_frequency: float,
     stop_radius: int | float,
     stop_duration: timedelta,
     pause_radius: int | float | None = None,
     pause_duration: timedelta | None = None,
     min_distance: int | float | None = None,
-    max_speed: int | float | None = None,
 ):
     """
     Processes the given DataFrame to identify and label trips based on various parameters.
 
     This function applies several filters to the DataFrame, including a minimum distance filter and a maximum speed filter.
     It then identifies and labels trips based on the given maximum radius, stop duration, and pause duration.
 
@@ -412,32 +417,26 @@
         df (pd.DataFrame): The input DataFrame to process.
         crs (str): The coordinate reference system to use when processing the DataFrame. The latitude and longitude columns must be in this CRS, otherwise the results will be incorrect.
         sampling_frequency (float): The sampling frequency of the data in seconds. This is used to convert the minimum distance to the correct units.
         max_radius (int | float): The maximum radius to use when splitting stops.
         stop_duration (timedelta): The minimum duration to consider a stop.
         pause_duration (timedelta): The minimum duration to consider a pause.
         min_distance (int | float | None, optional): The minimum distance between points. Points that are closer than this distance are filtered out. If None, no minimum distance filter is applied.
-        max_speed (int | float | None, optional): The maximum speed. Points that are faster than this speed are filtered out. If None, no maximum speed filter is applied.
 
     Returns:
         pd.DataFrame: The processed DataFrame with added 'trip_id', 'trip_status' columns.
     """
     origin = df
 
     # Filter out points that are too close to each other.
     if min_distance is not None:
         min_distance = convert_distance_parameter(min_distance, sampling_frequency)
         df = min_distance_filter(df, min_distance=min_distance, crs=crs)
         df = df[df["min_distance"]]  # type: ignore
 
-    # Filter out points that are too fast.
-    if max_speed is not None:
-        df = max_speed_filter(df, max_speed=max_speed, crs=crs)
-        df = df[df["max_speed"]]  # type: ignore
-
     # Get the trips from the DataFrame.
     df = _get_trips(df, crs=crs, stop_radius=stop_radius, stop_duration=stop_duration)
 
     # Get the pauses from the DataFrame.
     if not pause_radius and not pause_duration:
         pauses = pd.Series(name="partial_status")
     else:
@@ -552,14 +551,33 @@
     # Get the segments from the DataFrame.
     segments = gap_splitter(
         df[working_cols],
         name="segment_id",
         min_duration=gap_duration,
         overwrite=overwrite,
     )
+
+    # Split segments based on max speed.
+    if max_speed:
+        segments = (
+            segments.groupby("segment_id").apply(
+                lambda x: speed_splitter(
+                    x, max_speed=max_speed, crs=crs, name="speed_id"
+                )
+            )
+        ).reset_index(level=0, drop=True)
+        segments["segment_id"] = (
+            pd.factorize(
+                segments["segment_id"].astype(str)
+                + "_"
+                + segments["speed_id"].astype(str)
+            )[0]
+            + 1
+        )
+
     df = df.join(
         segments[["segment_id"]],
         how="left",
     )
 
     working_cols.append("segment_id")
     if "environment" in df.columns:
@@ -574,15 +592,14 @@
                 crs=crs,
                 sampling_frequency=sampling_frequency,
                 stop_radius=stop_radius,
                 stop_duration=stop_duration,
                 pause_radius=pause_radius,
                 pause_duration=pause_duration,
                 min_distance=min_distance,
-                max_speed=max_speed,
             )
         )
         .reset_index(level=0, drop=True)
     )  # type: ignore
 
     # Remove trips that are too short (duration).
     if min_duration:
@@ -600,27 +617,29 @@
     trip_mask = temp_df["trip_id"].notna()
     stationary_mask = temp_df["stationary_id"].notna()
 
     # Renumbers the trip IDs to be unique across all segments.
     temp_df.loc[trip_mask, "trip_id"] = (
         pd.factorize(
             temp_df.loc[trip_mask, "segment_id"].astype(str)
+            + "_"
             + temp_df.loc[trip_mask, "trip_id"].astype(str)
         )[0]
         + 1
     )
 
     # Renumbers the stationary IDs to be unique across all segments.
     temp_df["stationary_id"] = (
         temp_df["stationary_id"].isna().astype(int).diff().ne(0).cumsum()
     ).where(stationary_mask)
 
     temp_df.loc[stationary_mask, "stationary_id"] = (
         pd.factorize(
             temp_df.loc[stationary_mask, "segment_id"].astype(str)
+            + "_"
             + temp_df.loc[stationary_mask, "stationary_id"].astype(str)
         )[0]
         + 1
     )
 
     # Merge the processed DataFrame with the original DataFrame.
     df = df.join(
```

### Comparing `labda-0.0.7/labda/processing/wear_validity.py` & `labda-0.0.8/labda/processing/wear_validity.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,25 +4,41 @@
 import pandas as pd
 
 from ..structure.validation.subject import SCHEMA
 
 # TODO: Need to be tested, probably refactored!
 
 
-def get_wear_time(df: pd.DataFrame, sampling_frequency: float) -> pd.Series:
+def get_daily_wear_time(df: pd.DataFrame, sampling_frequency: float) -> pd.Series:
     series = df.groupby(pd.Grouper(level="datetime", freq="D"))["wear"].sum()
     series = series.rename("wear_time")
     series = series.apply(lambda x: timedelta(seconds=(x * sampling_frequency)))
     return series
 
 
+def get_wear_time(
+    df: pd.DataFrame,
+    sampling_frequency: float,
+) -> pd.DataFrame:
+    days = get_daily_wear_time(df, sampling_frequency).to_frame()
+
+    days["day"] = days.index.day_name()  # type: ignore
+
+    return days
+
+
+# Functions below are not used anymore, but are kept for future reference. Whole wear validity needs to be refactored.
+
+
 def get_wear_days(
-    df: pd.DataFrame, sampling_frequency: float, min_time: timedelta
+    df: pd.DataFrame,
+    sampling_frequency: float,
+    min_time: timedelta,
 ) -> pd.DataFrame:
-    days = get_wear_time(df, sampling_frequency).to_frame()
+    days = get_daily_wear_time(df, sampling_frequency).to_frame()
 
     days["valid"] = days["wear_time"] >= min_time
     days["day"] = days.index.day_of_week  # type: ignore
     days["day_type"] = days["day"].apply(lambda x: "weekend" if x > 4 else "weekday")
 
     return days.drop(columns=["day"])
```

### Comparing `labda-0.0.7/labda/structure/collection.py` & `labda-0.0.8/labda/structure/collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 
 from ..parallel import parallel_processing
 from .subject import Subject
 
 logger = logging.getLogger("default")
 
 
-def _to_parquet_with_path(subject, path, overwrite):
+def _to_parquet_with_path(subject, path, overwrite, validate):
     subject_path = path / f"{subject.metadata.id}.parquet"
-    return Subject.to_parquet(subject, path=subject_path, overwrite=overwrite)
+    return Subject.to_parquet(
+        subject, path=subject_path, overwrite=overwrite, validate=validate
+    )
 
 
 class Collection(BaseModel):
     id: Optional[str] = Field(default_factory=lambda: secrets.token_hex(4))
     subjects: list[Subject] = Field(default_factory=list)
 
     def __repr__(self):
@@ -40,52 +42,66 @@
     def get_subject(self, id: str) -> Subject:
         for subject in self.subjects:
             if subject.metadata.id == id:
                 return subject
         raise ValueError(f"Subject with id '{id}' not found.")
 
     @classmethod
-    def from_folder(cls, path: str | Path, id: str | None = None) -> "Collection":
+    def from_folder(
+        cls,
+        path: str | Path,
+        id: str | None = None,
+        *,
+        validate: bool = True,
+    ) -> "Collection":
         if isinstance(path, str):
             path = Path(path)
 
         files = list(path.glob("*.parquet"))
 
         if not files:
             raise ValueError(f"No parquet files found in '{path}'.")
 
-        subjects = [Subject.from_parquet(file) for file in files]
+        subjects = [Subject.from_parquet(file, validate=validate) for file in files]
         return cls(id=id, subjects=subjects)
 
     def to_folder(
         self,
         path: str | Path,
         *,
         parallel: bool = True,
         n_cores: int | str = "max",
         overwrite: bool = False,
+        validate: bool = True,
     ):
         if isinstance(path, str):
             path = Path(path)
 
         path.mkdir(parents=True, exist_ok=True)
 
         if not path.is_dir():
             raise ValueError(f"'{path}' is not a valid directory.")
 
         if parallel:
             self.subjects = parallel_processing(
-                partial(_to_parquet_with_path, path=path, overwrite=overwrite),
+                partial(
+                    _to_parquet_with_path,
+                    path=path,
+                    overwrite=overwrite,
+                    validate=validate,
+                ),
                 self.subjects,
                 n_cores,
             )
         else:
             for subject in self.subjects:
                 subject.to_parquet(
-                    path / f"{subject.metadata.id}.parquet", overwrite=overwrite
+                    path / f"{subject.metadata.id}.parquet",
+                    overwrite=overwrite,
+                    validate=validate,
                 )
 
     def detect_trips(
         self,
         *,
         parallel: bool = True,
         n_cores: int | str = "max",
```

### Comparing `labda-0.0.7/labda/structure/contexts.py` & `labda-0.0.8/labda/structure/contexts.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/structure/linkage.py` & `labda-0.0.8/labda/structure/linkage.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/structure/merging.py` & `labda-0.0.8/labda/structure/merging.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
 def merge_collections(
     left: Collection,
     right: Collection,
     id: str | None = None,
     *,
     how: str = "inner",
-    # keep: bool = False,
+    keep: bool = False,
     **kwargs,
 ) -> Collection:
     origin = f"{__name__}.merge_collections"
 
     if not isinstance(left, Collection) and not isinstance(right, Collection):
         message = f"Unsupported types: {type(left)} and {type(right)}"
         logger.error(
@@ -240,25 +240,25 @@
 
             # FIXME: Fix, it is not working
             # FIXME: Suffix to check if exists
             # FIXME: Native pd.merge function adds suffixes to columns with the same name otherwise not (no suffixes and we don't know the origin of the column)
             # TODO: This could be reworked, maybe not needed to do KEEP, just outer join.
             # TODO: Maybe completely remove the keep argument.
 
-            # if keep:
-            #     if left_subject:
-            #         # suffix = kwargs.get("suffixes")
-            #         # if suffix:
-            #         #     left_subject.df = left_subject.df.add_suffix(suffix[0])
-            #         collection.add_subject(left_subject)
-            #     elif right_subject:
-            #         # suffix = kwargs.get("suffixes")
-            #         # if suffix:
-            #         #     right_subject.df = right_subject.df.add_suffix(suffix[1])
-            #         collection.add_subject(right_subject)
+            if keep:
+                if left_subject:
+                    # suffix = kwargs.get("suffixes")
+                    # if suffix:
+                    #     left_subject.df = left_subject.df.add_suffix(suffix[0])
+                    collection.add_subject(left_subject)
+                elif right_subject:
+                    # suffix = kwargs.get("suffixes")
+                    # if suffix:
+                    #     right_subject.df = right_subject.df.add_suffix(suffix[1])
+                    collection.add_subject(right_subject)
 
     logger.info(
         f"From {len(subjects)} subjects, {len(collection.subjects)} were merged.",
         extra={"origin": origin, "object": collection.id},
     )
 
     return collection
```

### Comparing `labda-0.0.7/labda/structure/resampling.py` & `labda-0.0.8/labda/structure/resampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from ..structure.validation.subject import Column
 
 # TODO: Create one big configuration with SCHEMA (validation) and RESAMPLING
 
 logger = logging.getLogger("default")
 
 
-def log_upsample(id: str, from_sf: float, to_sf: float, origin: str):
-    message = f"Subject's data upsampled from {from_sf}s to {to_sf}s."
+def log_downsample(id: str, from_sf: float, to_sf: float, origin: str):
+    message = f"Subject's data downsampled from {from_sf}s to {to_sf}s."
 
     logger.info(message, extra={"origin": origin, "object": id})
 
 
 def mode(x):
     vals = x.to_list()
     return max(vals, key=vals.count)
 
 
-UPSAMPLING = [
+DOWNSAMPLING = [
     {"column": Column.SUBJECT_ID, "method": "first"},
     {"column": Column.WEAR, "method": mode},
     {"column": Column.TIMEDELTA, "method": "sum"},
     # ---
     {"column": Column.VERTICAL_COUNTS, "method": "sum"},
     {"column": Column.HORIZONTAL_COUNTS, "method": "sum"},
     {"column": Column.PERPENDICULAR_COUNTS, "method": "sum"},
@@ -58,15 +58,15 @@
     {"column": Column.ACTIVITY_INTENSITY, "method": mode},
     # TODO: ACTIVITY_VALUE - This is should be discussed a lot.
     {"column": Column.ACTIVITY_VALUE, "method": "mean"},
     {"column": Column.ACTIVITY, "method": mode},
 ]
 
 
-def upsample(
+def downsample(
     id: str,
     df: pd.DataFrame,
     from_sf: float,
     to_sf: float,
     mapper: list[dict[str, Any]] | None = None,
 ) -> pd.DataFrame:
     if from_sf > to_sf:
@@ -74,15 +74,15 @@
     elif from_sf == to_sf:
         print(f"Sampling frequencies are the same | {from_sf} = {to_sf}")
         return df
 
     df = df.copy()
 
     if not mapper:
-        mapper = UPSAMPLING
+        mapper = DOWNSAMPLING
 
     resampling = {v["column"]: v["method"] for v in mapper if v["column"] in df.columns}
 
     dropped = [
         colname for colname in df.columns if colname not in resampling.keys()
     ]  # TODO: Check that it works properly.
     if dropped:
@@ -91,10 +91,10 @@
         )  # TODO: Write warning what columns are dropped.
 
     df = df.resample(f"{to_sf}s").agg(resampling)  # type: ignore
     df.dropna(
         axis=0, how="all", inplace=True
     )  # Dropping rows with all NaN values - they were created by resampling.
 
-    log_upsample(id, from_sf, to_sf, origin="Subject.upsample")
+    log_downsample(id, from_sf, to_sf, origin="Subject.upsample")
 
     return df
```

### Comparing `labda-0.0.7/labda/structure/subject.py` & `labda-0.0.8/labda/structure/subject.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from datetime import datetime, timedelta
 from enum import StrEnum
-from math import log
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Optional
 
 import geopandas as gpd
 
 if TYPE_CHECKING:
     # This is a workaround to avoid circular imports.
     # TODO: Is there a better way to do this?
     from .collection import Collection
 import logging
 
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, SkipValidation
 from shapely.geometry import MultiPolygon
 
 from ..expanders import (
     add_acceleration,
     add_direction,
     add_distance,
     add_speed,
     add_timedelta,
 )
 from ..processing.accelerometer import detect_activity_intensity, detect_wear
 from ..processing.context import detect_contexts
 from ..processing.spatial import detect_transportation, detect_trips, get_timeline
-from ..structure.resampling import upsample
+from ..processing.wear_validity import get_wear_time
+from ..structure.resampling import downsample
 from ..visualisation.spatial import plot
 from .validation.subject import SCHEMA, Column
 
 logger = logging.getLogger("default")
 
 
 def log_message(subject: "Subject", message: str, origin: str):
@@ -107,23 +107,24 @@
         raise NotImplementedError("This method is not implemented yet.")
 
     def to_parquet(
         self,
         path: str | Path,
         *,
         overwrite: bool = False,
+        validate: bool = True,
     ) -> None:
         """
         Writes the subject's data to a Parquet file. The metadata is stored in the file's schema.
 
         Before saving, the subject's DataFrame is validated to ensure it conforms to the schema LABDA standard format.
 
         Args:
             path (str | Path): The path to write the Parquet file to.
-            overwrite (bool, optional): Whether to overwrite an existing file at the path. Defaults to `False`.
+            overwrite (bool, optional): Whether to overwrite an existing file at the path.
 
         Raises:
             FileExistsError: If a file already exists at the path and `overwrite` is `False`.
         """
         if isinstance(path, str):
             path = Path(path)
 
@@ -131,28 +132,35 @@
             raise FileExistsError(
                 f"The file '{path}' already exists. If you want to overwrite it, set the 'overwrite' argument to 'True'."
             )
         else:
             path.parent.mkdir(parents=True, exist_ok=True)
 
         custom_metadata = {"labda".encode(): self.metadata.model_dump_json().encode()}
-        self.validate()
+        if validate:
+            self.validate()
         table = pa.Table.from_pandas(self.df)
 
         existing_metadata = table.schema.metadata
         combined_meta = {**custom_metadata, **existing_metadata}
 
         table = table.replace_schema_metadata(combined_meta)
         pq.write_table(table, path)
         log_message(self, f"Subject exported: {path}", origin=f"{__name__}.to_parquet")
 
     @classmethod
-    def from_parquet(cls, path: str | Path) -> "Subject":
+    def from_parquet(
+        cls,
+        path: str | Path,
+        *,
+        validate: bool = True,
+    ) -> "Subject":
         """
-        Loads a subject from a Parquet file. While loading, subject's data is validated to ensure it conforms to the schema LABDA standard format.
+        Loads a subject from a Parquet file. While loading, subject's data is validated to ensure
+        it conforms to the schema LABDA standard format.
 
         Args:
             path (str | Path): The path to read the Parquet file from.
 
         Returns:
             Subject: A new Subject instance with the data read from the Parquet file.
 
@@ -164,15 +172,18 @@
 
         table = pq.read_table(path)
         df = table.to_pandas()
         custom_metadata = Metadata.model_validate_json(
             table.schema.metadata["labda".encode()]
         )
         cls = cls(metadata=custom_metadata, df=df)
-        cls.validate()
+
+        if validate:
+            cls.validate()
+
         log_message(cls, f"Subject imported: {path}", origin=f"{__name__}.from_parquet")
 
         return cls
 
     def validate(
         self,
         *,
@@ -203,16 +214,16 @@
         """
         Adds a timedelta column to the subject's DataFrame.
 
         This function calculates the time difference between each row and the previous row in the
         subject's DataFrame. The calculated timedelta is added as a new column to the DataFrame.
 
         Args:
-            name (str, optional): The name of the new timedelta column. Defaults to Column.TIMEDELTA.
-            overwrite (bool, optional): Whether to overwrite the existing timedelta column if it exists. Defaults to False.
+            name (str, optional): The name of the new timedelta column.
+            overwrite (bool, optional): Whether to overwrite the existing timedelta column if it exists.
 
         Raises:
             ValueError: If a column with the specified name already exists and 'overwrite' is False.
         """
         self.df = add_timedelta(self.df, name=name, overwrite=overwrite)
         log_message(self, "Timedelta column added.", origin=f"{__name__}.add_timedelta")
 
@@ -227,15 +238,15 @@
 
         This function calculates the distance between each row and the previous row in the
         subject's DataFrame. The calculated distance is added as a new column to the DataFrame.
         Units are based on the CRS.
 
         Args:
             name (str, optional): The name of the new distance column. Defaults to Column.DISTANCE.
-            overwrite (bool, optional): Whether to overwrite the existing distance column if it exists. Defaults to False.
+            overwrite (bool, optional): Whether to overwrite the existing distance column if it exists.
 
         Raises:
             ValueError: If a column with the specified name already exists and 'overwrite' is False.
         """
         self.df = add_distance(
             self.df, crs=self.metadata.crs, name=name, overwrite=overwrite
         )
@@ -251,16 +262,16 @@
         Adds a speed column to the subject's DataFrame.
 
         This function calculates the speed for each row in the subject's DataFrame based on the distance and time
         difference to the previous row. The calculated speed is added as a new column to the DataFrame.
         Units are based on the CRS. If units are in metres, the speed is converted to km/h.
 
         Args:
-            name (str, optional): The name of the new speed column. Defaults to Column.SPEED.
-            overwrite (bool, optional): Whether to overwrite the existing speed column if it exists. Defaults to False.
+            name (str, optional): The name of the new speed column.
+            overwrite (bool, optional): Whether to overwrite the existing speed column if it exists.
 
         Raises:
             ValueError: If a column with the specified name already exists and 'overwrite' is False.
         """
         self.df = add_speed(
             self.df, crs=self.metadata.crs, name=name, overwrite=overwrite
         )
@@ -286,44 +297,105 @@
         Adds a direction column to the subject's DataFrame.
 
         This function calculates the direction of movement for each row in the
         subject's DataFrame. The calculated direction is added as a new column to the DataFrame.
         The direction value is a bearing in degrees.
 
         Args:
-            name (str, optional): The name of the new direction column. Defaults to Column.DIRECTION.
-            overwrite (bool, optional): Whether to overwrite the existing direction column if it exists. Defaults to False.
+            name (str, optional): The name of the new direction column.
+            overwrite (bool, optional): Whether to overwrite the existing direction column if it exists.
 
         Raises:
             ValueError: If a column with the specified name already exists and 'overwrite' is False.
         """
         self.df = add_direction(self.df, name=name, overwrite=overwrite)
         log_message(self, "Direction column added.", origin=f"{__name__}.add_direction")
 
     def detect_trips(
         self,
-        cut_points: dict[str, Any] | None = None,
-        *,
         gap_duration: timedelta,
         stop_radius: int | float,
         stop_duration: timedelta,
-        window: int | None = None,
-        pause_fill: str | None = None,
-        activity: bool = False,
+        *,
+        max_speed: int | float | None = None,
+        min_distance: int | float | None = None,
         pause_radius: int | float | None = None,
         pause_duration: timedelta | None = None,
+        pause_fill: str | None = None,
         min_duration: timedelta | None = None,
         min_length: int | float | None = None,
-        min_distance: int | float | None = None,
-        max_speed: int | float | None = None,
+        cut_points: dict[str, Any] | None = None,
+        window: int | None = None,
+        activity: bool = False,
         indoor_limit: float | None = None,
         overwrite: bool = False,
     ) -> None:
+        """Detects trips and transportation modes in the subject's data based on the specified parameters.
+        The detected trips are stored in the subject's timeline and DataFrame is annotated with trip and
+        transportation mode information.
+
+        You can load prepared cut points for transportation mode detection or provide your own, see the example below.
+
+        Args:
+            gap_duration (timedelta): The minimum duration to consider a gap, i.e. if there is missing data for longer than this duration, the data is split into a new segment and analysed separately.
+            stop_radius (int | float): The maximum radius that subject needs to stay in to be considered a stop.
+            stop_duration (timedelta): The minimum duration to subject need to stay in specified radius to be considered a stop.
+            max_speed (int | float | None): The maximum speed between points. If the speed between points is higher than this value, data are split into a new segment and analysed separately.
+            min_distance (int | float | None): The minimum distance between points. Points that are closer than this distance are filtered out.
+            pause_radius (int | float | None): The maximum radius that subject needs to stay in to be considered a as a trip pause.
+            pause_duration (timedelta | None): The minimum duration to subject need to stay in specified radius to be considered as a trip pause.
+            pause_fill (str | None): If pauses should also have transportation mode. Options are "forward" or "backward" fill (based on the previous or next transportation mode of the trip).
+            min_duration (timedelta | None): The minimum duration of a trip. Trips shorter than this duration are annotated as stationary (stop) points.
+            min_length (int | float | None): The minimum length of a trip. Trips shorter than this length are annotated as stationary (stop) points.
+            cut_points (dict[str, Any] | None): Dictionary of cut points for transportation modes identification. If not provided, transportation modes are not detected.
+            window (int | None): The window size for moving average for transportation mode detection.
+            activity (bool): Wheter to use data from activity intensity column for transportation mode detection (combination of cut points and activity intensity column is used for detection).
+            indoor_limit (float | None): How much of the data needs to be identified as indoor for the whole trip to be removed (changed to stationary).
+            overwrite (bool): Whether to overwrite existing trip data.
+
+        Raises:
+            ValueError: If the subject's CRS is not defined.
+            ValueError: If the timeline already exists and 'overwrite' is False.
+
+        Returns:
+            None
+
+        Examples:
+            Here's how to call the function. For this example we assume that the subject's data has information for physical activity intensity
+            and environment (indoor/outdoor) and data are collected in less than 1 minute intervals.
+
+            ```python
+            from datetime import timedelta
+
+            from labda import Subject
+            from labda.assets import TRANSPORTATION_CUT_POINTS
+
+            subject = Subject.from_parquet("subject.parquet")
+
+            subject.detect_trips(
+                "gap_duration": timedelta(minutes=1),
+                "stop_radius": 25,
+                "stop_duration": timedelta(minutes=3),
+                "max_speed": 220,
+                "min_distance": None,
+                "pause_radius": 15,
+                "pause_duration": timedelta(minutes=1.5),
+                "pause_fill": "forward",
+                "min_duration": timedelta(minutes=2),
+                "min_length": None,
+                "cut_points": TRANSPORTATION_CUT_POINTS[1],
+                "window": 3,
+                "activity": True,
+                "indoor_limit": 92.5,
+                "overwrite": True,
+                )
+            ```
+        """
         if not self.metadata.crs:
-            raise ValueError("Records object does not have a CRS defined.")
+            raise ValueError("Subject CRS is not defined.")
 
         self.df = detect_trips(
             self.df,
             crs=self.metadata.crs,
             sampling_frequency=self.metadata.sampling_frequency,
             overwrite=overwrite,
             gap_duration=gap_duration,
@@ -350,14 +422,21 @@
             )
 
         if not overwrite and self.timeline:
             raise ValueError("Timeline already exists. Set 'overwrite' to 'True'.")
         else:
             self.timeline = get_timeline(self.df, crs=self.metadata.crs)
 
+        number_of_trips = self.timeline["trip_id"].nunique()
+        log_message(
+            self,
+            f"Number of trips detected: {number_of_trips}.",
+            origin=f"{__name__}.detect_trips",
+        )
+
     def detect_contexts(
         self,
         contexts: gpd.GeoDataFrame,
     ) -> None:
         self.df, contexts_dicts = detect_contexts(
             self.metadata.id, self.df, contexts, self.metadata.crs
         )
@@ -387,49 +466,71 @@
             self.df,
             self.metadata.sampling_frequency,
             min_duration,
             interruption_duration=interruption_duration,
             overwrite=overwrite,
         )
 
-    def upsample(
+    @property
+    def wear_time(
+        self,
+    ) -> pd.DataFrame:
+        return get_wear_time(self.df, self.metadata.sampling_frequency)
+
+    def downsample(
         self,
         sampling_frequency: float,
         *,
         mapper: list[dict[str, Any]] | None = None,
     ) -> None:
         """
-        Upsamples the subject's data to the specified sampling frequency.
+        Downsamples the subject's data to the specified sampling frequency.
 
-        This function upsamples the data in the DataFrame from the original sampling frequency to a new sampling frequency.
-        The upsampling is done using the methods specified in the mapper for each column. If no mapper is provided, a default
+        This function downsamples the data in the DataFrame from the original sampling frequency to a new sampling frequency.
+        The downsampling is done using the methods specified in the mapper for each column. If no mapper is provided, a default
         mapper is used. Columns not included in the mapper are dropped from the DataFrame.
 
         Args:
-            sampling_frequency (float): The new sampling frequency to upsample to in seconds.
+            sampling_frequency (float): The new sampling frequency to downsample to in seconds.
             mapper (list[dict[str, Any]], optional): A list of dictionaries that map the columns in the DataFrame to the
-                methods used to upsample the data in those columns. Each dictionary should have a 'column' key that specifies
+                methods used to downsample the data in those columns. Each dictionary should have a 'column' key that specifies
                 the column and a 'method' key that specifies the method. Methods are based on the pandas resample method. If not provided, a default mapper is used.
 
         Returns:
-            pd.DataFrame: The upsampled DataFrame.
+            pd.DataFrame: The downsampled DataFrame.
 
         Raises:
             ValueError: If the new sampling frequency is less than the original sampling frequency.
         """
-        self.df = upsample(
+        self.df = downsample(
             self.metadata.id,
             self.df,
             self.metadata.sampling_frequency,
             sampling_frequency,
             mapper,
         )
         self.metadata.sampling_frequency = sampling_frequency
 
     def plot(self, kind: str) -> Any:
+        """
+        Plots the subject's data based on the specified kind.
+
+        The kind of plot to produce is specified by the 'kind' argument. The following kinds are supported:
+        - 'gps': Plots the subject's raw GPS data.
+        - 'timeline': Plots the subject's timeline data (trips with pauses and stationary points).
+
+        Args:
+            kind (str): The kind of plot to produce. Must be either 'timeline' or 'gps'.
+
+        Returns:
+            Any: The resulting plot.
+
+        Raises:
+            ValueError: If 'kind' is not 'timeline' or 'gps', or if 'kind' is 'timeline' but the timeline data does not exist.
+        """
         match kind:
             case "timeline":
                 if isinstance(self.timeline, pd.DataFrame):
                     df = self.timeline
                 else:
                     raise ValueError("Timeline does not exist. Run 'detect_trips'.")
             case "gps":
```

### Comparing `labda-0.0.7/labda/structure/validation/context.py` & `labda-0.0.8/labda/structure/validation/context.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/structure/validation/linkage.py` & `labda-0.0.8/labda/structure/validation/linkage.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/structure/validation/subject.py` & `labda-0.0.8/labda/structure/validation/subject.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/utils.py` & `labda-0.0.8/labda/utils.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/labda/visualisation/spatial.py` & `labda-0.0.8/labda/visualisation/spatial.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.7/pyproject.toml` & `labda-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labda"
-version = "0.0.7"
+version = "0.0.8"
 description = "Library for Advanced Behavioural Data Analysis"
 authors = ["Josef Heidler <jheidler@health.sdu.dk>"]
 maintainers = ["Josef Heidler <jheidler@health.sdu.dk>"]
 
 readme = "README.md"
 license = "	CC-BY-SA-4.0"
 homepage = "https://labda.josefheidler.cz"
@@ -53,11 +53,12 @@
 [tool.poetry.group.jupyter.dependencies]
 ipykernel = "^6.29.0"
 nbformat = "^5.9.2"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-glightbox = "^0.3.7"
+mkdocs-jupyter = "^0.24.7"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `labda-0.0.7/PKG-INFO` & `labda-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labda
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library for Advanced Behavioural Data Analysis
 Home-page: https://labda.josefheidler.cz
 License: 	CC-BY-SA-4.0
 Keywords: analysis,health,behaviour,data,spatial,temporal
 Author: Josef Heidler
 Author-email: jheidler@health.sdu.dk
 Maintainer: Josef Heidler
@@ -37,15 +37,15 @@
 Description-Content-Type: text/markdown
 
 # LABDA: Library for Advanced Behavioural Data Analysis
 
 [![pypi](https://img.shields.io/pypi/v/labda.svg)](https://pypi.python.org/pypi/labda)
 [![downloads](https://static.pepy.tech/badge/labda/month)](https://pepy.tech/project/labda)
 [![versions](https://img.shields.io/pypi/pyversions/labda.svg)](https://github.com/josefheidler/labda)
-![discord](https://img.shields.io/discord/1165947556807848016)
+[![discord](https://img.shields.io/discord/1165947556807848016)](https://discord.gg/qu6ax5Q64j)
 
 **LABDA is currently under development and may undergo significant API changes that could result in breaking changes.**
 
 ## What is it?
 
 TO-DO...
```

