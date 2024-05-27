# Comparing `tmp/sbmltoodejax-0.4.2.tar.gz` & `tmp/sbmltoodejax-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmltoodejax-0.4.2.tar", last modified: Mon Feb 26 16:18:13 2024, max compression
+gzip compressed data, was "sbmltoodejax-0.4.3.tar", last modified: Mon May 27 09:50:41 2024, max compression
```

## Comparing `sbmltoodejax-0.4.2.tar` & `sbmltoodejax-0.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2024-02-26 16:18:13.264850 sbmltoodejax-0.4.2/
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2760 2023-06-06 15:00:48.000000 sbmltoodejax-0.4.2/LICENSE
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     9498 2024-02-26 16:18:13.264850 sbmltoodejax-0.4.2/PKG-INFO
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     8963 2024-02-26 12:31:44.000000 sbmltoodejax-0.4.2/README.md
-drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2024-02-26 16:18:13.264850 sbmltoodejax-0.4.2/sbmltoodejax/
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      346 2024-02-26 16:07:26.000000 sbmltoodejax-0.4.2/sbmltoodejax/__init__.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     6062 2023-06-06 15:27:10.000000 sbmltoodejax-0.4.2/sbmltoodejax/biomodels_api.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2552 2023-06-06 15:27:10.000000 sbmltoodejax-0.4.2/sbmltoodejax/jaxfuncs.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)    26059 2024-02-26 16:08:36.000000 sbmltoodejax-0.4.2/sbmltoodejax/modulegeneration.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2689 2023-06-06 15:27:10.000000 sbmltoodejax-0.4.2/sbmltoodejax/parse.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     3294 2024-02-26 16:14:30.000000 sbmltoodejax-0.4.2/sbmltoodejax/utils.py
-drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2024-02-26 16:18:13.264850 sbmltoodejax-0.4.2/sbmltoodejax.egg-info/
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     9498 2024-02-26 16:18:13.000000 sbmltoodejax-0.4.2/sbmltoodejax.egg-info/PKG-INFO
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      414 2024-02-26 16:18:13.000000 sbmltoodejax-0.4.2/sbmltoodejax.egg-info/SOURCES.txt
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)        1 2024-02-26 16:18:13.000000 sbmltoodejax-0.4.2/sbmltoodejax.egg-info/dependency_links.txt
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       29 2024-02-26 16:18:13.000000 sbmltoodejax-0.4.2/sbmltoodejax.egg-info/requires.txt
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       13 2024-02-26 16:18:13.000000 sbmltoodejax-0.4.2/sbmltoodejax.egg-info/top_level.txt
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       38 2024-02-26 16:18:13.264850 sbmltoodejax-0.4.2/setup.cfg
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      850 2023-06-06 15:27:10.000000 sbmltoodejax-0.4.2/setup.py
-drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2024-02-26 16:18:13.264850 sbmltoodejax-0.4.2/test/
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     1641 2023-06-06 15:27:10.000000 sbmltoodejax-0.4.2/test/test_jaxfuncs.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2461 2023-06-06 15:27:10.000000 sbmltoodejax-0.4.2/test/test_modulegeneration.py
+drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2024-05-27 09:50:41.933455 sbmltoodejax-0.4.3/
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2760 2023-06-06 15:00:48.000000 sbmltoodejax-0.4.3/LICENSE
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     9498 2024-05-27 09:50:41.933455 sbmltoodejax-0.4.3/PKG-INFO
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     8963 2024-02-26 12:31:44.000000 sbmltoodejax-0.4.3/README.md
+drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2024-05-27 09:50:41.929455 sbmltoodejax-0.4.3/sbmltoodejax/
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      346 2024-05-27 09:50:25.000000 sbmltoodejax-0.4.3/sbmltoodejax/__init__.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     6062 2023-06-06 15:27:10.000000 sbmltoodejax-0.4.3/sbmltoodejax/biomodels_api.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2552 2023-06-06 15:27:10.000000 sbmltoodejax-0.4.3/sbmltoodejax/jaxfuncs.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)    26059 2024-02-26 16:08:36.000000 sbmltoodejax-0.4.3/sbmltoodejax/modulegeneration.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2689 2023-06-06 15:27:10.000000 sbmltoodejax-0.4.3/sbmltoodejax/parse.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     3556 2024-05-27 09:39:49.000000 sbmltoodejax-0.4.3/sbmltoodejax/utils.py
+drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2024-05-27 09:50:41.933455 sbmltoodejax-0.4.3/sbmltoodejax.egg-info/
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     9498 2024-05-27 09:50:41.000000 sbmltoodejax-0.4.3/sbmltoodejax.egg-info/PKG-INFO
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      414 2024-05-27 09:50:41.000000 sbmltoodejax-0.4.3/sbmltoodejax.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)        1 2024-05-27 09:50:41.000000 sbmltoodejax-0.4.3/sbmltoodejax.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       29 2024-05-27 09:50:41.000000 sbmltoodejax-0.4.3/sbmltoodejax.egg-info/requires.txt
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       13 2024-05-27 09:50:41.000000 sbmltoodejax-0.4.3/sbmltoodejax.egg-info/top_level.txt
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       38 2024-05-27 09:50:41.933455 sbmltoodejax-0.4.3/setup.cfg
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      850 2023-06-06 15:27:10.000000 sbmltoodejax-0.4.3/setup.py
+drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2024-05-27 09:50:41.933455 sbmltoodejax-0.4.3/test/
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     1641 2023-06-06 15:27:10.000000 sbmltoodejax-0.4.3/test/test_jaxfuncs.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2461 2023-06-06 15:27:10.000000 sbmltoodejax-0.4.3/test/test_modulegeneration.py
```

### Comparing `sbmltoodejax-0.4.2/LICENSE` & `sbmltoodejax-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.4.2/PKG-INFO` & `sbmltoodejax-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmltoodejax
-Version: 0.4.2
+Version: 0.4.3
 Summary: lightweight library that allows to automatically parse and convert SBML models into python models written end-to-end in JAX
 Home-page: https://github.com/flowersteam/sbmltoodejax
 Author: Mayalen Etcheverry
 Author-email: mayalen.etcheverry@inria.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sbmltoodejax-0.4.2/README.md` & `sbmltoodejax-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.4.2/sbmltoodejax/biomodels_api.py` & `sbmltoodejax-0.4.3/sbmltoodejax/biomodels_api.py`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.4.2/sbmltoodejax/jaxfuncs.py` & `sbmltoodejax-0.4.3/sbmltoodejax/jaxfuncs.py`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.4.2/sbmltoodejax/modulegeneration.py` & `sbmltoodejax-0.4.3/sbmltoodejax/modulegeneration.py`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.4.2/sbmltoodejax/parse.py` & `sbmltoodejax-0.4.3/sbmltoodejax/parse.py`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.4.2/sbmltoodejax/utils.py` & `sbmltoodejax-0.4.3/sbmltoodejax/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     GenerateModel(model_data, model_fp,
                   vary_constant_reactants=vary_constant_reactants, vary_boundary_reactants=vary_boundary_reactants,
                   deltaT=deltaT, atol=atol, rtol=rtol, mxstep=mxstep)
 
     return model_fp
 
 
-def load_biomodel(model_idx, model_fp="jax_model.py", deltaT=0.1, atol=1e-6, rtol=1e-12, mxstep=5000000):
+def load_biomodel(model_idx, model_fp="jax_model.py",
+                  vary_constant_reactants=False, vary_boundary_reactants=False,
+                  deltaT=0.1, atol=1e-6, rtol=1e-12, mxstep=5000000):
     """Calls the generate_biomodel function for a SBML model hosted on the BioModel website and indexed by the provided `model_idx`,
     then loads and returns the generated `model` module and `y0`, `w0`, `c` variables.
 
     Args:
         model_idx: either an integer, or a valid model id
         model_fp (str): filepath for the generated file
         deltaT (float, optional): parameter passed to `generate_biomodel`. Default to 0.1.
@@ -44,15 +46,17 @@
         tuple containing
 
         - model (ModelRollout): generated model rollout module
         - y0 (jax.numpy.Array): default initial state of y variable(as provided in the SBML file)
         - w0 (jax.numpy.Array): default initial state of w variable (as provided in the SBML file)
         - c (jax.numpy.Array): default values of constant kinematic parameters c (as provided in the SBML file)
     """
-    model_fp = generate_biomodel(model_idx, model_fp=model_fp, deltaT=deltaT, atol=atol, rtol=rtol, mxstep=mxstep)
+    model_fp = generate_biomodel(model_idx, model_fp=model_fp,
+                                 vary_constant_reactants=vary_constant_reactants, vary_boundary_reactants=vary_boundary_reactants,
+                                 deltaT=deltaT, atol=atol, rtol=rtol, mxstep=mxstep)
     spec = importlib.util.spec_from_file_location("JaxModelSpec", model_fp)
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     model_cls = getattr(module, "ModelRollout")
     model = model_cls()
     y0 = getattr(module, "y0")
     w0 = getattr(module, "w0")
```

### Comparing `sbmltoodejax-0.4.2/sbmltoodejax.egg-info/PKG-INFO` & `sbmltoodejax-0.4.3/sbmltoodejax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmltoodejax
-Version: 0.4.2
+Version: 0.4.3
 Summary: lightweight library that allows to automatically parse and convert SBML models into python models written end-to-end in JAX
 Home-page: https://github.com/flowersteam/sbmltoodejax
 Author: Mayalen Etcheverry
 Author-email: mayalen.etcheverry@inria.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sbmltoodejax-0.4.2/setup.py` & `sbmltoodejax-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.4.2/test/test_jaxfuncs.py` & `sbmltoodejax-0.4.3/test/test_jaxfuncs.py`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.4.2/test/test_modulegeneration.py` & `sbmltoodejax-0.4.3/test/test_modulegeneration.py`

 * *Files identical despite different names*

