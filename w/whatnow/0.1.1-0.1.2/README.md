# Comparing `tmp/whatnow-0.1.1.tar.gz` & `tmp/whatnow-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatnow-0.1.1.tar", last modified: Mon May 27 10:13:21 2024, max compression
+gzip compressed data, was "whatnow-0.1.2.tar", last modified: Mon May 27 10:14:58 2024, max compression
```

## Comparing `whatnow-0.1.1.tar` & `whatnow-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 student-4318  (1001) student-4318  (1001)        0 2024-05-27 10:13:21.893119 whatnow-0.1.1/
--rw-rw-r--   0 student-4318  (1001) student-4318  (1001)        0 2024-05-26 16:05:33.000000 whatnow-0.1.1/LICENSE
--rw-r--r--   0 student-4318  (1001) student-4318  (1001)     2977 2024-05-27 10:13:21.893119 whatnow-0.1.1/PKG-INFO
--rw-rw-r--   0 student-4318  (1001) student-4318  (1001)     2507 2024-05-27 10:03:18.000000 whatnow-0.1.1/README.md
--rw-rw-r--   0 student-4318  (1001) student-4318  (1001)       38 2024-05-27 10:13:21.893119 whatnow-0.1.1/setup.cfg
--rw-rw-r--   0 student-4318  (1001) student-4318  (1001)      658 2024-05-27 10:07:19.000000 whatnow-0.1.1/setup.py
-drwxrwxr-x   0 student-4318  (1001) student-4318  (1001)        0 2024-05-27 10:13:21.893119 whatnow-0.1.1/whatnow/
--rw-rw-r--   0 student-4318  (1001) student-4318  (1001)      304 2024-05-26 17:58:00.000000 whatnow-0.1.1/whatnow/__init__.py
--rw-rw-r--   0 student-4318  (1001) student-4318  (1001)     2384 2024-05-26 20:36:02.000000 whatnow-0.1.1/whatnow/what.py
-drwxrwxr-x   0 student-4318  (1001) student-4318  (1001)        0 2024-05-27 10:13:21.893119 whatnow-0.1.1/whatnow.egg-info/
--rw-r--r--   0 student-4318  (1001) student-4318  (1001)     2977 2024-05-27 10:13:21.000000 whatnow-0.1.1/whatnow.egg-info/PKG-INFO
--rw-rw-r--   0 student-4318  (1001) student-4318  (1001)      186 2024-05-27 10:13:21.000000 whatnow-0.1.1/whatnow.egg-info/SOURCES.txt
--rw-rw-r--   0 student-4318  (1001) student-4318  (1001)        1 2024-05-27 10:13:21.000000 whatnow-0.1.1/whatnow.egg-info/dependency_links.txt
--rw-rw-r--   0 student-4318  (1001) student-4318  (1001)        8 2024-05-27 10:13:21.000000 whatnow-0.1.1/whatnow.egg-info/top_level.txt
+drwxrwxr-x   0 student-4318  (1001) student-4318  (1001)        0 2024-05-27 10:14:58.242429 whatnow-0.1.2/
+-rw-rw-r--   0 student-4318  (1001) student-4318  (1001)        0 2024-05-26 16:05:33.000000 whatnow-0.1.2/LICENSE
+-rw-r--r--   0 student-4318  (1001) student-4318  (1001)     2971 2024-05-27 10:14:58.242429 whatnow-0.1.2/PKG-INFO
+-rw-rw-r--   0 student-4318  (1001) student-4318  (1001)     2501 2024-05-27 10:14:43.000000 whatnow-0.1.2/README.md
+-rw-rw-r--   0 student-4318  (1001) student-4318  (1001)       38 2024-05-27 10:14:58.242429 whatnow-0.1.2/setup.cfg
+-rw-rw-r--   0 student-4318  (1001) student-4318  (1001)      658 2024-05-27 10:14:51.000000 whatnow-0.1.2/setup.py
+drwxrwxr-x   0 student-4318  (1001) student-4318  (1001)        0 2024-05-27 10:14:58.242429 whatnow-0.1.2/whatnow/
+-rw-rw-r--   0 student-4318  (1001) student-4318  (1001)      304 2024-05-26 17:58:00.000000 whatnow-0.1.2/whatnow/__init__.py
+-rw-rw-r--   0 student-4318  (1001) student-4318  (1001)     2384 2024-05-26 20:36:02.000000 whatnow-0.1.2/whatnow/what.py
+drwxrwxr-x   0 student-4318  (1001) student-4318  (1001)        0 2024-05-27 10:14:58.242429 whatnow-0.1.2/whatnow.egg-info/
+-rw-r--r--   0 student-4318  (1001) student-4318  (1001)     2971 2024-05-27 10:14:58.000000 whatnow-0.1.2/whatnow.egg-info/PKG-INFO
+-rw-rw-r--   0 student-4318  (1001) student-4318  (1001)      186 2024-05-27 10:14:58.000000 whatnow-0.1.2/whatnow.egg-info/SOURCES.txt
+-rw-rw-r--   0 student-4318  (1001) student-4318  (1001)        1 2024-05-27 10:14:58.000000 whatnow-0.1.2/whatnow.egg-info/dependency_links.txt
+-rw-rw-r--   0 student-4318  (1001) student-4318  (1001)        8 2024-05-27 10:14:58.000000 whatnow-0.1.2/whatnow.egg-info/top_level.txt
```

### Comparing `whatnow-0.1.1/PKG-INFO` & `whatnow-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: whatnow
-Version: 0.1.1
+Version: 0.1.2
 Summary: A module to get the the current Day, Date, Time and Temperature
 Home-page: https://github.com/inspironman/whatnow
 Author: Deepak Kumar Upadhayay
 Author-email: dku3132@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# WeatherNow
+# Whatnow
 
-WeatherNow is a Python module that retrieves the current weather details for your location. It uses the OpenWeatherMap API to fetch weather data and geocoder to determine your current location based on your IP address.
+Whatnow is a Python module that retrieves the current weather details for your location. It uses the OpenWeatherMap API to fetch weather data and geocoder to determine your current location based on your IP address.
 
 ## Features
 
 - Get current temperature, humidity, wind speed, and cloudiness
 - Check if it is raining or snowing
 - Display the current date, time, and day of the week
```

### Comparing `whatnow-0.1.1/README.md` & `whatnow-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# WeatherNow
+# Whatnow
 
-WeatherNow is a Python module that retrieves the current weather details for your location. It uses the OpenWeatherMap API to fetch weather data and geocoder to determine your current location based on your IP address.
+Whatnow is a Python module that retrieves the current weather details for your location. It uses the OpenWeatherMap API to fetch weather data and geocoder to determine your current location based on your IP address.
 
 ## Features
 
 - Get current temperature, humidity, wind speed, and cloudiness
 - Check if it is raining or snowing
 - Display the current date, time, and day of the week
```

### Comparing `whatnow-0.1.1/setup.py` & `whatnow-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="whatnow",
-    version="0.1.1",
+    version="0.1.2",
     author="Deepak Kumar Upadhayay",
     author_email="dku3132@gmail.com",
     description="A module to get the the current Day, Date, Time and Temperature",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/inspironman/whatnow",  # Replace with your repo URL
     packages=find_packages(),
```

### Comparing `whatnow-0.1.1/whatnow/what.py` & `whatnow-0.1.2/whatnow/what.py`

 * *Files identical despite different names*

### Comparing `whatnow-0.1.1/whatnow.egg-info/PKG-INFO` & `whatnow-0.1.2/whatnow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: whatnow
-Version: 0.1.1
+Version: 0.1.2
 Summary: A module to get the the current Day, Date, Time and Temperature
 Home-page: https://github.com/inspironman/whatnow
 Author: Deepak Kumar Upadhayay
 Author-email: dku3132@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# WeatherNow
+# Whatnow
 
-WeatherNow is a Python module that retrieves the current weather details for your location. It uses the OpenWeatherMap API to fetch weather data and geocoder to determine your current location based on your IP address.
+Whatnow is a Python module that retrieves the current weather details for your location. It uses the OpenWeatherMap API to fetch weather data and geocoder to determine your current location based on your IP address.
 
 ## Features
 
 - Get current temperature, humidity, wind speed, and cloudiness
 - Check if it is raining or snowing
 - Display the current date, time, and day of the week
```

