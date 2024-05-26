# Comparing `tmp/oresat_star_tracker-0.2.1.tar.gz` & `tmp/oresat_star_tracker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_star_tracker-0.2.1.tar", last modified: Thu May 23 03:46:50 2024, max compression
+gzip compressed data, was "oresat_star_tracker-0.3.0.tar", last modified: Sun May 26 23:45:10 2024, max compression
```

## Comparing `oresat_star_tracker-0.2.1.tar` & `oresat_star_tracker-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.567559 oresat_star_tracker-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.567559 oresat_star_tracker-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.567559 oresat_star_tracker-0.2.1/oresat_star_tracker/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/oresat_star_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/oresat_star_tracker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/oresat_star_tracker/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/oresat_star_tracker/star_tracker_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/oresat_star_tracker/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/oresat_star_tracker/templates/star_tracker.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 03:46:50.000000 oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:46:50.571559 oresat_star_tracker-0.2.1/tests/images/
--rw-r--r--   0 runner    (1001) docker     (127)  1929648 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/tests/images/capture-2022-09-25-09-40-25.png
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-23 03:46:45.000000 oresat_star_tracker-0.2.1/tests/test_lost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:45:10.082605 oresat_star_tracker-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:45:10.074605 oresat_star_tracker-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:45:10.078605 oresat_star_tracker-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-26 23:45:10.082605 oresat_star_tracker-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:45:10.078605 oresat_star_tracker-0.3.0/oresat_star_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/oresat_star_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/oresat_star_tracker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-26 23:45:09.000000 oresat_star_tracker-0.3.0/oresat_star_tracker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/oresat_star_tracker/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/oresat_star_tracker/star_tracker_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:45:10.078605 oresat_star_tracker-0.3.0/oresat_star_tracker/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/oresat_star_tracker/templates/star_tracker.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:45:10.082605 oresat_star_tracker-0.3.0/oresat_star_tracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-26 23:45:10.000000 oresat_star_tracker-0.3.0/oresat_star_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-26 23:45:10.000000 oresat_star_tracker-0.3.0/oresat_star_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 23:45:10.000000 oresat_star_tracker-0.3.0/oresat_star_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-26 23:45:10.000000 oresat_star_tracker-0.3.0/oresat_star_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-26 23:45:10.000000 oresat_star_tracker-0.3.0/oresat_star_tracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-26 23:45:10.000000 oresat_star_tracker-0.3.0/oresat_star_tracker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 23:45:10.082605 oresat_star_tracker-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:45:10.078605 oresat_star_tracker-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 23:45:10.078605 oresat_star_tracker-0.3.0/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (127)  1929648 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/tests/images/capture-2022-09-25-09-40-25.png
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-26 23:45:02.000000 oresat_star_tracker-0.3.0/tests/test_lost.py
```

### Comparing `oresat_star_tracker-0.2.1/.github/workflows/pypi.yaml` & `oresat_star_tracker-0.3.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.1/.github/workflows/tests.yaml` & `oresat_star_tracker-0.3.0/.github/workflows/tests.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -6,49 +6,48 @@
       - master
   pull_request:
     branches:
       - master
 
 jobs:
   tests:
-
     runs-on: ubuntu-latest
 
     steps:
-    - name: Clone oresat-star-tracker repository
-      uses: actions/checkout@v3
+      - name: Clone oresat-star-tracker repository
+        uses: actions/checkout@v3
 
-    - name: Clone oresat-configs repository
-      uses: actions/checkout@v3
-      with:
-        repository: oresat/oresat-configs
-        path: resources/oresat-configs
-
-    - name: Set up Python 3.9
-      uses: actions/setup-python@v3
-      with:
-        python-version: "3.9"
-
-    - name: Build and install oresat-configs
-      working-directory: resources/oresat-configs
-      run: |
-        python -m pip install --upgrade pip
-        pip install -r requirements.txt
-        python -m build
-        pip install dist/*.whl
-
-    - name: Clean up oresat-configs
-      run: rm -rf resources/oresat-configs
-
-    - name: Install Python dependencies
-      run: |
-        python -m pip install --upgrade pip
-        pip install -r requirements.txt
+      - name: Clone oresat-configs repository
+        uses: actions/checkout@v3
+        with:
+          repository: oresat/oresat-configs
+          path: resources/oresat-configs
+
+      - name: Set up Python 3.9
+        uses: actions/setup-python@v3
+        with:
+          python-version: "3.9"
+
+      - name: Build and install oresat-configs
+        working-directory: resources/oresat-configs
+        run: |
+          python -m pip install --upgrade pip
+          pip install -r requirements.txt
+          python -m build
+          pip install dist/*.whl
+
+      - name: Clean up oresat-configs
+        run: rm -rf resources/oresat-configs
+
+      - name: Install Python dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install -r requirements.txt
 
-    - name: Check format with Black
-      run: black --check --diff .
+      - name: Check format with Black
+        run: black --check --diff .
 
-    - name: Check format with isort
-      run: isort --check --diff .
+      - name: Check format with isort
+        run: isort --check --diff .
 
-    - name: Test building pypi package
-      run: python -m build
+      - name: Test building pypi package
+        run: python -m build
```

### Comparing `oresat_star_tracker-0.2.1/.gitignore` & `oresat_star_tracker-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.1/LICENSE` & `oresat_star_tracker-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.1/PKG-INFO` & `oresat_star_tracker-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-star-tracker
-Version: 0.2.1
+Version: 0.3.0
 Summary: OreSat Star Tracker OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -76,10 +76,11 @@
 
 ```bash
 $ python3 -m unittest
 ```
 
 [LOST]: https://github.com/UWCubeSat/lost
 [NASA-COTS]: https://github.com/nasa/COTS-Star-Tracker
+[Flask]: https://flask.palletsprojects.com/en/latest/
 [oresat-olaf repo]: https://github.com/oresat/oresat-olaf
 [CANopen for Python]: https://github.com/christiansandberg/canopen
 [oresat-prucam-ar013x repo]: https://github.com/oresat/oresat-prucam-ar013x
```

### Comparing `oresat_star_tracker-0.2.1/README.md` & `oresat_star_tracker-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -51,10 +51,11 @@
 
 ```bash
 $ python3 -m unittest
 ```
 
 [LOST]: https://github.com/UWCubeSat/lost
 [NASA-COTS]: https://github.com/nasa/COTS-Star-Tracker
+[Flask]: https://flask.palletsprojects.com/en/latest/
 [oresat-olaf repo]: https://github.com/oresat/oresat-olaf
 [CANopen for Python]: https://github.com/christiansandberg/canopen
 [oresat-prucam-ar013x repo]: https://github.com/oresat/oresat-prucam-ar013x
```

### Comparing `oresat_star_tracker-0.2.1/oresat_star_tracker/__main__.py` & `oresat_star_tracker-0.3.0/oresat_star_tracker/__main__.py`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.1/oresat_star_tracker/star_tracker_service.py` & `oresat_star_tracker-0.3.0/oresat_star_tracker/star_tracker_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import canopen
 import cv2
 import lost
 import numpy as np
 import tifffile as tiff
 from olaf import Service, logger, new_oresat_file  # , set_cpufreq_gov
 
-from .camera import Camera, CameraError
+from .camera import Camera, CameraError, CameraState
 
 
 class State(IntEnum):
     """All star tracker states."""
 
     OFF = 0x0
     BOOT = 0x1
@@ -184,15 +184,21 @@
         return True
 
     def _star_track(self):
         """Star track once."""
 
         # Take the image
         ts = time()
-        data = self._camera.capture()
+        try:
+            data = self._camera.capture()
+        except Exception:
+            self._state = State.ERROR
+            logger.error("Camera capture failure")
+            logger.info(f"changing status: {self._state.name} -> {State.STANDBY.name}")
+            return
 
         # NOTE: Lost currently writes the capture to disk temporarily
         lost_args = lost.identify_args(algo="tetra")
         lost_data = lost.identify(data, lost_args)
 
         self._right_ascension_obj.value = int(lost_data["attitude_ra"])
         self._declination_obj.value = int(lost_data["attitude_de"])
@@ -220,15 +226,21 @@
         start_timestamp = time()
 
         # Take images until either time runs out or image count has been reached
         while time() - start_timestamp < self._capture_duration_obj.value and (
             self._image_count_obj.value == 0 or img_count < self._image_count_obj.value
         ):
             ts = time()
-            data = self._camera.capture()  # Take the image
+            try:
+                data = self._camera.capture()
+            except Exception:
+                self._state = State.ERROR
+                logger.error("Camera capture failure")
+                logger.info(f"changing status: {self._state.name} -> {State.STANDBY.name}")
+                return
 
             # Check if image passes filter
             if not self._filter_enable_obj.value or not self._filter(data):
                 logger.debug("capture did not pass filter")
                 continue
 
             self._last_capture_time.value = int(ts)
@@ -261,30 +273,36 @@
         if error is CameraError:
             logger.critical(error)
             self._state = State.ERROR
         elif error is ValueError:
             logger.error(error)
         else:
             logger.critical(f"Unkown error {error}")
-            self._state = State.ERROR
+        self._state = State.ERROR
 
     def on_read_status(self) -> int:
         """SDO read callback for star tracker status."""
 
         return self._state.value
 
     def on_write_status(self, value: int):
         """SDO write callback for star tracker status."""
+        new_status = self._state
 
-        new_status = State.BOOT
-        try:
-            new_status = State(value)
-        except ValueError:
-            logger.error(f"invalid state: {value}")
-            return
+        if self._camera.state == CameraState.LOCKOUT:
+            logger.error("Cannot transition camera to lockout state")
+        elif self._camera.state == CameraState.ERROR:
+            logger.error("Camera is in error state")
+            new_status = State.ERROR
+        else:
+            try:
+                new_status = State(value)
+            except ValueError:
+                logger.error(f"invalid state: {value}")
+                return
 
         if new_status == self._state:
             return  # nothing to change
 
         if self._state == State.BOOT:
             logger.error("cannot transfer out of BOOT state by command")
             return
```

### Comparing `oresat_star_tracker-0.2.1/oresat_star_tracker/templates/star_tracker.html` & `oresat_star_tracker-0.3.0/oresat_star_tracker/templates/star_tracker.html`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/PKG-INFO` & `oresat_star_tracker-0.3.0/oresat_star_tracker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-star-tracker
-Version: 0.2.1
+Version: 0.3.0
 Summary: OreSat Star Tracker OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -76,10 +76,11 @@
 
 ```bash
 $ python3 -m unittest
 ```
 
 [LOST]: https://github.com/UWCubeSat/lost
 [NASA-COTS]: https://github.com/nasa/COTS-Star-Tracker
+[Flask]: https://flask.palletsprojects.com/en/latest/
 [oresat-olaf repo]: https://github.com/oresat/oresat-olaf
 [CANopen for Python]: https://github.com/christiansandberg/canopen
 [oresat-prucam-ar013x repo]: https://github.com/oresat/oresat-prucam-ar013x
```

### Comparing `oresat_star_tracker-0.2.1/oresat_star_tracker.egg-info/SOURCES.txt` & `oresat_star_tracker-0.3.0/oresat_star_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.1/pyproject.toml` & `oresat_star_tracker-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.1/tests/images/capture-2022-09-25-09-40-25.png` & `oresat_star_tracker-0.3.0/tests/images/capture-2022-09-25-09-40-25.png`

 * *Files identical despite different names*

### Comparing `oresat_star_tracker-0.2.1/tests/test_lost.py` & `oresat_star_tracker-0.3.0/tests/test_lost.py`

 * *Files identical despite different names*

