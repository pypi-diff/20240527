# Comparing `tmp/desimpy-0.0.4.tar.gz` & `tmp/desimpy-0.0.5.tar.gz`

## Comparing `desimpy-0.0.4.tar` & `desimpy-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 desimpy-0.0.4/mkdocs.yml
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 desimpy-0.0.4/requirements.txt
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 desimpy-0.0.4/update.sh
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 desimpy-0.0.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 desimpy-0.0.4/docs/about.md
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 desimpy-0.0.4/docs/examples.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 desimpy-0.0.4/docs/index.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 desimpy-0.0.4/docs/methodology.md
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 desimpy-0.0.4/examples/car.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 desimpy-0.0.4/src/desimpy/__init__.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 desimpy-0.0.4/src/desimpy/core.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 desimpy-0.0.4/src/desimpy/distributions.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 desimpy-0.0.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 desimpy-0.0.4/LICENSE
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 desimpy-0.0.4/README.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 desimpy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 desimpy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 desimpy-0.0.5/mkdocs.yml
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 desimpy-0.0.5/requirements.txt
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 desimpy-0.0.5/update.sh
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 desimpy-0.0.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 desimpy-0.0.5/docs/examples.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 desimpy-0.0.5/docs/index.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 desimpy-0.0.5/docs/methodology.md
+-rw-r--r--   0        0        0   227791 2020-02-02 00:00:00.000000 desimpy-0.0.5/docs/assets/logo.jpg
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 desimpy-0.0.5/examples/car.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 desimpy-0.0.5/examples/example_0.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 desimpy-0.0.5/examples/mmc.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 desimpy-0.0.5/examples/mmc_2.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 desimpy-0.0.5/examples/mminfinity.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 desimpy-0.0.5/examples/test_example_0.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 desimpy-0.0.5/src/desimpy/__init__.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 desimpy-0.0.5/src/desimpy/core.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 desimpy-0.0.5/src/desimpy/distributions.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 desimpy-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 desimpy-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 desimpy-0.0.5/README.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 desimpy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 desimpy-0.0.5/PKG-INFO
```

### Comparing `desimpy-0.0.4/mkdocs.yml` & `desimpy-0.0.5/mkdocs.yml`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     - icon: fontawesome/brands/github
       link: https://github.com/galenseilis/DESimPy
 
 nav:
   - Overview: index.md
   - Methodology: methodology.md
   - Examples: examples.md
-  - About: about.md
 
 plugins:
   - search
   - mkdocstrings:
       handlers:
         python:
           options:
@@ -59,10 +58,9 @@
   - pymdownx.inlinehilite
   - pymdownx.snippets
   - pymdownx.superfences
   - pymdownx.arithmatex: 
       generic: true
 
 extra_javascript: 
-  - javascripts/mathjax.js
   - https://polyfill.io/v3/polyfill.min.js?features=es6
   - https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
```

### Comparing `desimpy-0.0.4/requirements.txt` & `desimpy-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `desimpy-0.0.4/.github/workflows/ci.yml` & `desimpy-0.0.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `desimpy-0.0.4/docs/examples.md` & `desimpy-0.0.5/docs/examples.md`

 * *Files 17% similar despite different names*

```diff
@@ -14,63 +14,65 @@
 ### Clock Example
 
 ### First Car Example
 
 Let us consider the [first car example](https://simpy.readthedocs.io/en/latest/simpy_intro/basic_concepts.html#our-first-process) from the SimPy documentation. A car alternates between driving and parking for the duration of the simulation. 
 
 ```python
-# first_car.py
 from typing import NoReturn
 
 from desimpy import core
 
+
 class StartParking(core.Event):
     """Make the car park."""
 
-    def execute(self) -> NoReturn:
+    def execute(self, env) -> NoReturn:
         """Start parking and schedule next drive."""
 
-        print(f"Start parking at {self.env.now}")
+        print(f"Start parking at {env.now}")
 
-        scheduled_driving_time = self.env.now + 5
+        scheduled_driving_time = env.now + 5
 
-        driving_event = StartDriving(self.env, scheduled_driving_time)
+        driving_event = StartDriving(scheduled_driving_time)
 
-        self.env.schedule_event(driving_event)
+        env.schedule_event(driving_event)
 
 
 class StartDriving(core.Event):
     """Make the car drive."""
 
-    def execute(self) -> NoReturn:
+    def execute(self, env) -> NoReturn:
         """Start driving and schedule for next parking."""
 
-        print(f"Start driving at {self.env.now}")
+        print(f"Start driving at {env.now}")
 
-        scheduled_parking_time = self.env.now + 2
+        scheduled_parking_time = env.now + 2
 
-        parking_event = StartParking(self.env, scheduled_parking_time)
+        parking_event = StartParking(scheduled_parking_time)
 
-        self.env.schedule_event(parking_event)
+        env.schedule_event(parking_event)
 
 
 class CarSimulation:
     """Our car simulation."""
 
     def __init__(self) -> NoReturn:
         self.simulation = core.Environment()
 
     def run_simulation(self) -> NoReturn:
-        arrival_event = StartParking(self.simulation, 0)
+        arrival_event = StartParking(0)
         self.simulation.schedule_event(arrival_event)
         self.simulation.run(15)
 
-if __name__ == '__main__':
-	example = CarSimulation()
-	example.run_simulation()
+
+if __name__ == "__main__":
+    example = CarSimulation()
+    example.run_simulation()
+
 ```
 
 When called as a script it should print the following:
 
 ```bash
 $ python first_car.py
 Start parking at 0
```

### Comparing `desimpy-0.0.4/docs/methodology.md` & `desimpy-0.0.5/docs/methodology.md`

 * *Files identical despite different names*

### Comparing `desimpy-0.0.4/examples/car.py` & `desimpy-0.0.5/examples/car.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import NoReturn
 
 from desimpy import core
 
+
 class StartParking(core.Event):
     """Make the car park."""
 
     def execute(self, env) -> NoReturn:
         """Start parking and schedule next drive."""
 
         print(f"Start parking at {env.now}")
 
         scheduled_driving_time = env.now + 5
 
-        driving_event = StartDriving(env, scheduled_driving_time)
+        driving_event = StartDriving(scheduled_driving_time)
 
         env.schedule_event(driving_event)
 
 
 class StartDriving(core.Event):
     """Make the car drive."""
 
@@ -39,10 +40,11 @@
         self.simulation = core.Environment()
 
     def run_simulation(self) -> NoReturn:
         arrival_event = StartParking(0)
         self.simulation.schedule_event(arrival_event)
         self.simulation.run(15)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     example = CarSimulation()
     example.run_simulation()
```

### Comparing `desimpy-0.0.4/src/desimpy/core.py` & `desimpy-0.0.5/src/desimpy/core.py`

 * *Files identical despite different names*

### Comparing `desimpy-0.0.4/src/desimpy/distributions.py` & `desimpy-0.0.5/src/desimpy/distributions.py`

 * *Files identical despite different names*

### Comparing `desimpy-0.0.4/.gitignore` & `desimpy-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `desimpy-0.0.4/LICENSE` & `desimpy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `desimpy-0.0.4/README.md` & `desimpy-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # DESimPy
 Event-driven [discrete event simulation](https://en.wikipedia.org/wiki/Discrete-event_simulation) in Python (DESimPy).
 
+![](docs/assets/logo.jpg)
+
 ## Overview
 
 DESimPy is an event-driven simulation framework based on standard Python and inspired by [SimPy](https://simpy.readthedocs.io/en/latest/).
 
 Processes in DESimPy are defined by methods owned by Python objects inherited from the `Event` abstract base class. These processes can be used to model system-level or component level changes in a modelled system. Such systems might include customers or patients flowing through services, vehicles in traffic, or agents competing in games.
 
 DESimPy implements time-to-event simulation where the next event in a schedule is processed next regardless of the amount of time in the simulated present to that event. This constrasts with "time sweeping" in which a step size is used to increment foreward in time. It is possible to combine time-to-event with time sweeping (see [Palmer & Tian 2021](https://www.semanticscholar.org/paper/Implementing-hybrid-simulations-that-integrate-in-Palmer-Tian/bea73e8d6c828e15290bc4f01c8dd1a4347c46d0)), however this package does not provide any explicit support for that.
```

### Comparing `desimpy-0.0.4/pyproject.toml` & `desimpy-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DESimpy"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Galen Seilis", email="galen.seilis@seilis.ca" },
 ]
 description = "A discrete event simulation environment in Python."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `desimpy-0.0.4/PKG-INFO` & `desimpy-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: DESimpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A discrete event simulation environment in Python.
 Project-URL: Homepage, https://github.com/pypa/DESimpy
 Project-URL: Issues, https://github.com/pypa/DESimpy/issues
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # DESimPy
 Event-driven [discrete event simulation](https://en.wikipedia.org/wiki/Discrete-event_simulation) in Python (DESimPy).
 
+![](docs/assets/logo.jpg)
+
 ## Overview
 
 DESimPy is an event-driven simulation framework based on standard Python and inspired by [SimPy](https://simpy.readthedocs.io/en/latest/).
 
 Processes in DESimPy are defined by methods owned by Python objects inherited from the `Event` abstract base class. These processes can be used to model system-level or component level changes in a modelled system. Such systems might include customers or patients flowing through services, vehicles in traffic, or agents competing in games.
 
 DESimPy implements time-to-event simulation where the next event in a schedule is processed next regardless of the amount of time in the simulated present to that event. This constrasts with "time sweeping" in which a step size is used to increment foreward in time. It is possible to combine time-to-event with time sweeping (see [Palmer & Tian 2021](https://www.semanticscholar.org/paper/Implementing-hybrid-simulations-that-integrate-in-Palmer-Tian/bea73e8d6c828e15290bc4f01c8dd1a4347c46d0)), however this package does not provide any explicit support for that.
```

