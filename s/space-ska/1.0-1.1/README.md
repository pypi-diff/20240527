# Comparing `tmp/space_ska-1.0.tar.gz` & `tmp/space_ska-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_ska-1.0.tar", max compression
+gzip compressed data, was "space_ska-1.1.tar", max compression
```

## Comparing `space_ska-1.0.tar` & `space_ska-1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-03-27 14:16:49.669953 space_ska-1.0/LICENSE
--rw-r--r--   0        0        0      251 2024-05-23 13:50:14.310648 space_ska-1.0/README.md
--rw-r--r--   0        0        0      657 2024-05-23 20:31:57.467242 space_ska-1.0/pyproject.toml
--rw-r--r--   0        0        0      699 2024-05-23 20:17:13.947568 space_ska-1.0/ska/__init__.py
--rw-r--r--   0        0        0     1924 2024-05-23 20:17:43.571273 space_ska-1.0/ska/cache.py
--rw-r--r--   0        0        0     5654 2024-05-23 20:17:43.599273 space_ska-1.0/ska/cli.py
--rw-r--r--   0        0        0     7954 2024-05-23 20:17:43.615273 space_ska-1.0/ska/filter.py
--rw-r--r--   0        0        0     7856 2024-05-23 20:17:43.603273 space_ska-1.0/ska/spectrum.py
--rw-r--r--   0        0        0     3291 2024-05-23 20:17:43.583273 space_ska-1.0/ska/svo.py
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 space_ska-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-27 14:16:49.669953 space_ska-1.1/LICENSE
+-rw-r--r--   0        0        0      251 2024-05-23 13:50:14.310648 space_ska-1.1/README.md
+-rw-r--r--   0        0        0      775 2024-05-27 06:42:39.221278 space_ska-1.1/pyproject.toml
+-rw-r--r--   0        0        0      865 2024-05-27 06:40:49.194784 space_ska-1.1/ska/__init__.py
+-rw-r--r--   0        0        0     3388 2024-05-27 06:40:01.687440 space_ska-1.1/ska/cache.py
+-rw-r--r--   0        0        0     6799 2024-05-27 06:40:01.687440 space_ska-1.1/ska/cli.py
+-rw-r--r--   0        0        0     7954 2024-05-23 20:17:43.615273 space_ska-1.1/ska/filter.py
+-rw-r--r--   0        0        0     9888 2024-05-27 06:40:01.687440 space_ska-1.1/ska/spectrum.py
+-rw-r--r--   0        0        0     3291 2024-05-23 20:17:43.583273 space_ska-1.1/ska/svo.py
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 space_ska-1.1/PKG-INFO
```

### Comparing `space_ska-1.0/LICENSE` & `space_ska-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `space_ska-1.0/pyproject.toml` & `space_ska-1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 [tool.poetry]
 name = "space-ska"
-version = "1.0"
+version = "1.1"
 description = "Spectral-Kit for Asteroids"
 authors = ["Benoit Carry <benoit.carry@oca.eu>", "Max Mahlke"]
 license = "MIT"
 readme = "README.md"
 packages = [{'include' = 'ska'}]
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.10"
 requests = "^2.31.0"
 pandas = "^2.2.1"
 click = "^8.1.7"
 rich = "^13.7.1"
 astropy = "^6.0.1"
 numpy = "^1.26.4"
+matplotlib = "^3.5"
+furo = "^2022.9.15"
+sphinx-copybutton = "^0.5.0"
+sphinx_design = "^0.3.0"
+sphinx-hoverxref = "*"
+
 
 
 [tool.poetry.extras]
 docs = [
   "furo",
   "sphinx",
   "sphinx-copybutton",
```

### Comparing `space_ska-1.0/ska/__init__.py` & `space_ska-1.1/ska/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """Spectral-Kit for Asteroids."""
 
 import os
 
 from .filter import Filter  # noqa
 from .spectrum import Spectrum  # noqa
 from . import svo  # noqa
-from .cache import download_sun_vega  # noqa
+from .cache import download_sun_and_vega, download_mahlke_taxonomy  # noqa
 
-__version__ = "1.0.0"
+__version__ = "1.1"
 
 # Cache location
 PATH_CACHE = os.path.join(os.path.expanduser("~"), ".cache/ska")
 os.makedirs(PATH_CACHE, exist_ok=True)
 
 # SKA Auxiliary data
+PATH_FILTER_LIST = os.path.join(PATH_CACHE, "svo_filters.txt")
 PATH_VEGA = os.path.join(PATH_CACHE, "spectrum_vega.csv")
 PATH_SUN = os.path.join(PATH_CACHE, "spectrum_sun.csv")
-PATH_FILTER_LIST = os.path.join(PATH_CACHE, "svo_filters.txt")
+PATH_MAHLKE = os.path.join(PATH_CACHE, "template_mahlke2022.csv")
 
 if not os.path.isfile(PATH_FILTER_LIST):
     svo.download_filter_list()
 
 if not os.path.isfile(PATH_VEGA) or not os.path.isfile(PATH_SUN):
-    download_sun_vega()
+    download_sun_and_vega()
+
+if not os.path.isfile(PATH_MAHLKE):
+    download_mahlke_taxonomy()
```

### Comparing `space_ska-1.0/ska/cli.py` & `space_ska-1.1/ska/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,51 +29,79 @@
 def status(clear, update):
     """Echo the status of the cached filters."""
     from rich import prompt
 
     from ska import cache
 
     # ------
-    # Check filter list
+    # Inventory of filters
     if not os.path.isfile(ska.PATH_FILTER_LIST):
         ska.svo.download_filter_list()
+    cached_filter_ids, cached_filter_xmls = cache.filter_inventory()
 
     # ------
-    # Echo inventory
-    cached_ids, cached_xmls = cache.take_inventory()
+    # Inventory of spectra
+    cached_spectra, cached_templates = cache.spectra_inventory()
 
     rich.print(
         f"""\nContents of {ska.PATH_CACHE}:
 
-        {len(cached_xmls)} filters\n"""
+        {len(cached_filter_xmls)} filters
+        {len(cached_spectra)} spectra
+        {len(cached_templates)} spectral template files"""
     )
-
-    # Update or clear
-    if cached_xmls:
+    
+    # Filters: Update or clear
+    if cached_filter_xmls:
         if not clear and not update:
             decision = prompt.Prompt.ask(
-                "Update or clear the cached filters and filter list?\n"
+                "\nUpdate or clear the cached [bright_cyan]filters and filter list[/bright_cyan]?\n"
                 "[blue][0][/blue] No "
                 "[blue][1][/blue] Clear cache "
                 "[blue][2][/blue] Update data ",
                 choices=["0", "1", "2"],
                 show_choices=False,
                 default="0",
             )
         else:
             decision = "none"
 
         if clear or decision == "1":
             rich.print("\nClearing the cached filters and filter list..")
-            cache.clear()
+            cache.clear_filters()
 
         elif update or decision == "2":
-            rich.print(cached_ids)
+            rich.print(cached_filter_ids)
             rich.print("\nDownload filters from SVO Filter Service..")
-            cache.update_filters(cached_ids, force=True)
+            cache.update_filters(cached_filter_ids, force=True)
+
+
+    # Spectra: Update or clear
+    if cached_spectra or cached_templates:
+        if not clear and not update:
+            decision = prompt.Prompt.ask(
+                "\nUpdate or clear the cached [bright_cyan]spectra and templates[/bright_cyan]?\n"
+                "[blue][0][/blue] No "
+                "[blue][1][/blue] Clear cache "
+                "[blue][2][/blue] Update data ",
+                choices=["0", "1", "2"],
+                show_choices=False,
+                default="0",
+            )
+        else:
+            decision = "none"
+
+        if clear or decision == "1":
+            rich.print("\nClearing the cached spectra and templates..")
+            cache.clear_spectra()
+
+        elif update or decision == "2":
+            rich.print("\nUpdate spectra and templates..")
+            cache.download_sun_and_vega()
+            cache.download_mahlke_taxonomy()
 
 
 # --------------------------------------------------------------------------------
 # Fuzzy search among filters ID
 @cli_ska.command()
 def id():
     """Fuzzy-search SVO filter index."""
```

### Comparing `space_ska-1.0/ska/filter.py` & `space_ska-1.1/ska/filter.py`

 * *Files identical despite different names*

### Comparing `space_ska-1.0/ska/spectrum.py` & `space_ska-1.1/ska/spectrum.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,33 +16,48 @@
         # Store attributes
         self.Wavelength = None
         self.Flux = None
         self.Reflectance = False
 
         if "input" in locals():
 
-            # Initialize from a file
+            # Initialize from a str: file or a taxonomic class
             if isinstance(input, str):
-                self.from_csv(input)
+                
+                if os.path.isfile(input):
+                    self.from_csv(input)
+                else:
+                    self.from_taxonomy(input)
 
             # Initialize from a numpy.ndarray
             if isinstance(input, np.ndarray):
                 self.from_numpy(input)
 
             # Initialize from a pandas.DataFrame
             if isinstance(input, pd.DataFrame):
                 self.from_dataframe(input)
 
+            # Initialize from a temperature (simple float or int) -> Blackbody
+            if isinstance(input, int) | isinstance(input, float):
+                self.from_blackbody(input)
+
+
+
     # --------------------------------------------------------------------------------
     def copy(self):
         from copy import deepcopy
 
         return deepcopy(self)
 
     # --------------------------------------------------------------------------------
+    # --------------------------------------------------------------------------------
+    # --------------------------------------------------------------------------------
+    # Spectrum from Input
+
+    # --------------------------------------------------------------------------------
     def from_csv(self, file):
         if not os.path.isfile(file):
             rich.print(f"[red]Spectrum file {file} not found.[/red].")
             sys.exit(1)
 
         # Read spectrum
         try:
@@ -98,14 +113,49 @@
         self.Wavelength = np.array(df.loc[order, "Wavelength"].values)
         if check_flux:
             self.Flux = np.array(df.loc[order, "Flux"].values)
         if check_refl:
             self.Flux = np.array(df.loc[order, "Reflectance"].values)
             self.Reflectance = True
 
+
+    # --------------------------------------------------------------------------------
+    def from_taxonomy(self, type):
+
+        # Read template spectra of Mahlke+2022 taxonomy
+        templates = pd.read_csv(ska.PATH_MAHLKE)
+
+        # Select the requested type
+        if type in templates.columns:
+            cols = ['feature', type] 
+            df = templates[cols]
+            df.columns = ['Wavelength', 'Reflectance']
+            self.from_dataframe(df)
+        else:
+            rich.print(f"[red]Type[/red] [bright_cyan]{type}[/bright_cyan] [red]not found in Mahlke+2022 taxonomy.[/red]")
+        
+
+    # --------------------------------------------------------------------------------
+    def from_blackbody(self, T):
+
+        from astropy.modeling.models import BlackBody
+        from astropy import units as u
+
+        # Blackbody function
+        bb = BlackBody(temperature=float(T)*u.K, scale=1.0 * u.erg / (u.s * (0.1*u.nm) * u.sr * u.cm**2) )
+        wave = np.linspace(0.05, 5, num=1000) * u.micron
+        flux = bb(wave)
+        self.from_numpy( np.array([wave.value,flux.value]).T )
+
+
+    # --------------------------------------------------------------------------------
+    # --------------------------------------------------------------------------------
+    # --------------------------------------------------------------------------------
+    # Color computation
+
     # --------------------------------------------------------------------------------
     def compute_color(self, filter1, filter2, phot_sys="Vega", vega=None):
         """Computes filter_1-filter_2 color of spectrum in the requested system.
 
         Parameters
         ==========
         filter_1: ska.Filter
```

### Comparing `space_ska-1.0/ska/svo.py` & `space_ska-1.1/ska/svo.py`

 * *Files identical despite different names*

### Comparing `space_ska-1.0/PKG-INFO` & `space_ska-1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: space-ska
-Version: 1.0
+Version: 1.1
 Summary: Spectral-Kit for Asteroids
 License: MIT
 Author: Benoit Carry
 Author-email: benoit.carry@oca.eu
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: docs
 Requires-Dist: astropy (>=6.0.1,<7.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: furo (>=2022.9.15,<2023.0.0) ; extra == "docs"
+Requires-Dist: matplotlib (>=3.5,<4.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0) ; extra == "docs"
+Requires-Dist: sphinx-hoverxref ; extra == "docs"
+Requires-Dist: sphinx_design (>=0.3.0,<0.4.0)
 Description-Content-Type: text/markdown
 
 # ska - Spectral-Kit for Asteroids
 
 Suites of tools to compute colors from spectra or reflectance spectra using the
 [SVO Filter Service](http://svo2.cab.inta-csic.es/theory/fps/index.php?mode=voservice)
 in different photometric system: Vega, AB, ST.
```

