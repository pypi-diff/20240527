# Comparing `tmp/neurocaps-0.9.3.tar.gz` & `tmp/neurocaps-0.9.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.3.tar", last modified: Sun May 26 10:35:13 2024, max compression
+gzip compressed data, was "neurocaps-0.9.3.post1.tar", last modified: Mon May 27 18:21:17 2024, max compression
```

## Comparing `neurocaps-0.9.3.tar` & `neurocaps-0.9.3.post1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 10:35:13.069695 neurocaps-0.9.3/
--rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.3/LICENSE.md
--rw-rw-rw-   0        0        0    16348 2024-05-26 10:35:13.064699 neurocaps-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0    15021 2024-05-26 10:30:02.000000 neurocaps-0.9.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 10:35:12.858389 neurocaps-0.9.3/neurocaps/
--rw-rw-rw-   0        0        0       72 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:35:12.942511 neurocaps-0.9.3/neurocaps/_utils/
--rw-rw-rw-   0        0        0      363 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:35:12.959177 neurocaps-0.9.3/neurocaps/_utils/_cap_internals/
--rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.3/neurocaps/_utils/_cap_internals/__init__.py
--rw-rw-rw-   0        0        0     2531 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-rw-rw-   0        0        0      184 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:35:12.994591 neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/
--rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-rw-rw-   0        0        0     2847 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
--rw-rw-rw-   0        0        0     5777 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-rw-rw-   0        0        0     8190 2024-05-23 03:16:16.000000 neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-rw-rw-   0        0        0     2680 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:35:13.016421 neurocaps-0.9.3/neurocaps/analysis/
--rw-rw-rw-   0        0        0      139 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/analysis/__init__.py
--rw-rw-rw-   0        0        0    69880 2024-05-26 10:33:29.000000 neurocaps-0.9.3/neurocaps/analysis/cap.py
--rw-rw-rw-   0        0        0     4803 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/analysis/merge.py
--rw-rw-rw-   0        0        0     1595 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/analysis/standardize.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:35:13.027554 neurocaps-0.9.3/neurocaps/extraction/
--rw-rw-rw-   0        0        0       87 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/extraction/__init__.py
--rw-rw-rw-   0        0        0    31128 2024-05-26 10:33:29.000000 neurocaps-0.9.3/neurocaps/extraction/timeseriesextractor.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:35:13.060701 neurocaps-0.9.3/neurocaps.egg-info/
--rw-rw-rw-   0        0        0    16348 2024-05-26 10:35:12.000000 neurocaps-0.9.3/neurocaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-05-26 10:35:12.000000 neurocaps-0.9.3/neurocaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 10:35:12.000000 neurocaps-0.9.3/neurocaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2024-05-26 10:35:12.000000 neurocaps-0.9.3/neurocaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-26 10:35:12.000000 neurocaps-0.9.3/neurocaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1499 2024-05-26 10:24:45.000000 neurocaps-0.9.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-26 10:35:13.070444 neurocaps-0.9.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-26 10:35:13.049929 neurocaps-0.9.3/tests/
--rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.3/tests/test_CAP.py
--rw-rw-rw-   0        0        0     4687 2024-05-25 04:47:35.000000 neurocaps-0.9.3/tests/test_TimeseriesExtractor.py
--rw-rw-rw-   0        0        0     1077 2024-05-23 03:16:16.000000 neurocaps-0.9.3/tests/test_TimeseriesExtractor_additional.py
--rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.3/tests/test_merge_dicts.py
--rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.3/tests/test_standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.542630 neurocaps-0.9.3.post1/
+-rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.3.post1/LICENSE.md
+-rw-rw-rw-   0        0        0    16793 2024-05-27 18:21:17.542630 neurocaps-0.9.3.post1/PKG-INFO
+-rw-rw-rw-   0        0        0    15451 2024-05-27 18:12:44.000000 neurocaps-0.9.3.post1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.457019 neurocaps-0.9.3.post1/neurocaps/
+-rw-rw-rw-   0        0        0       72 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.498387 neurocaps-0.9.3.post1/neurocaps/_utils/
+-rw-rw-rw-   0        0        0      363 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.500653 neurocaps-0.9.3.post1/neurocaps/_utils/_cap_internals/
+-rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_cap_internals/__init__.py
+-rw-rw-rw-   0        0        0     2531 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-rw-rw-   0        0        0      184 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.514479 neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-rw-rw-   0        0        0     2187 2024-05-27 16:10:31.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
+-rw-rw-rw-   0        0        0     5777 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-rw-rw-   0        0        0     8190 2024-05-27 16:51:23.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-rw-rw-   0        0        0     2680 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.523140 neurocaps-0.9.3.post1/neurocaps/analysis/
+-rw-rw-rw-   0        0        0      139 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/analysis/__init__.py
+-rw-rw-rw-   0        0        0    72960 2024-05-27 18:18:07.000000 neurocaps-0.9.3.post1/neurocaps/analysis/cap.py
+-rw-rw-rw-   0        0        0     4791 2024-05-27 17:56:51.000000 neurocaps-0.9.3.post1/neurocaps/analysis/merge.py
+-rw-rw-rw-   0        0        0     1626 2024-05-27 17:56:39.000000 neurocaps-0.9.3.post1/neurocaps/analysis/standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.523140 neurocaps-0.9.3.post1/neurocaps/extraction/
+-rw-rw-rw-   0        0        0       87 2024-05-26 10:24:45.000000 neurocaps-0.9.3.post1/neurocaps/extraction/__init__.py
+-rw-rw-rw-   0        0        0    33356 2024-05-27 18:03:42.000000 neurocaps-0.9.3.post1/neurocaps/extraction/timeseriesextractor.py
+drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.542630 neurocaps-0.9.3.post1/neurocaps.egg-info/
+-rw-rw-rw-   0        0        0    16793 2024-05-27 18:21:17.000000 neurocaps-0.9.3.post1/neurocaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-05-27 18:21:17.000000 neurocaps-0.9.3.post1/neurocaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 18:21:17.000000 neurocaps-0.9.3.post1/neurocaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2024-05-27 18:21:17.000000 neurocaps-0.9.3.post1/neurocaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-27 18:21:17.000000 neurocaps-0.9.3.post1/neurocaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1512 2024-05-27 16:09:22.000000 neurocaps-0.9.3.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 18:21:17.542630 neurocaps-0.9.3.post1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 18:21:17.537372 neurocaps-0.9.3.post1/tests/
+-rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.3.post1/tests/test_CAP.py
+-rw-rw-rw-   0        0        0     4687 2024-05-25 04:47:35.000000 neurocaps-0.9.3.post1/tests/test_TimeseriesExtractor.py
+-rw-rw-rw-   0        0        0     1077 2024-05-27 17:22:37.000000 neurocaps-0.9.3.post1/tests/test_TimeseriesExtractor_additional.py
+-rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.3.post1/tests/test_merge_dicts.py
+-rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.3.post1/tests/test_standardize.py
```

### Comparing `neurocaps-0.9.3/LICENSE.md` & `neurocaps-0.9.3.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3/PKG-INFO` & `neurocaps-0.9.3.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.3
-Summary: Co-activation patterns Python package
+Version: 0.9.3.post1
+Summary: Co-activation Patterns (CAPs) Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
@@ -28,25 +28,25 @@
 Requires-Dist: nibabel
 Requires-Dist: nilearn!=0.10.3,>=0.10.1
 Requires-Dist: surfplot
 Requires-Dist: neuromaps
 Requires-Dist: pybids; platform_system != "Windows"
 
 # neurocaps
-This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
+This is a Python package designed to perform Co-activation Patterns (CAPs) analyses. It utilizes k-means clustering to group timepoints (TRs) into brain states, applicable to both resting-state and task-based fMRI data. The package is compatible with data preprocessed using **fMRIPrep** and assumes your directory is BIDS-compliant, containing a derivatives folder with a pipeline folder (such as fMRIPrep) that holds the preprocessed BOLD data.
 
 **Still in beta but stable.**
 
 # Installation
 
-**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
+**Note**: The `get_bold()` method in the `TimeseriesExtractor` class relies on pybids, which is only functional on POSIX operating systems and macOS. If you have a pickled timeseries dictionary in the correct nested form, you can use this package on Windows to visualize the BOLD timeseries, the `CAP` class, as well as the `merge_dicts()` and `standardize()` functions in the in the `neurcaps.analysis` submodule.
 
-To install, using your preferred terminal:
+To install, use your preferred terminal:
 
-**Installation with pip:**
+**Installation using pip:**
 
 ```bash
 
 pip install neurocaps
 
 ```
 
@@ -63,60 +63,77 @@
 git clone https://github.com/donishadsmith/neurocaps/
 cd neurocaps
 pip install -e .
 
 ```
 
 # Usage
-**This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
+**This package contains two main classes: `TimeseriesExtractor` for extracting the timeseries, and `CAP` for performing the CAPs analysis.**
 
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes have a left and right version (bilateral nodes)**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+**Note:** When extracting the timeseries, this package uses either the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes have a left and right version (bilateral nodes). The number of ROIs and networks for the Schaefer atlas can be adjusted with the parcel_approach parameter when initializing the TimeseriesExtractor class.
 
-If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
+To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". For example:
+
+```python
+parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm": 1}}
+```
+
+Similarly, the version of the AAL atlas can be modified using:
+
+```python
+parcel_approach = {"AAL": {"version": "SPM12"}}
+```
+
+If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions (bilateral nodes). 
 
 Custom Key Structure:
-- maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
-- nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+- 'maps': Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+- 'nodes':  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
 Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
 visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
-- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
+- 'regions': Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
         
-Example 
+Example:
 The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
 
 ```Python
 parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
-                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus",
+                              "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                              "regions": {"Vis" : {"lh": [0,1],
                                                   "rh": [3,4]},
                                          "Hippocampus": {"lh": [2],
                                                          "rh": [5]}}}}
  ```
 
 **Main features for `TimeseriesExtractor` includes:**
 
-- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
-- Saving the nested dictionary containing timeseries as a pickle file.
-- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
-- Ability to use parallel processing by specifying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
+- **Timeseries Extraction:** Extract timeseries for resting-state or task data, creating a nested dictionary containing the subject ID, run number, and associated timeseries. This serves as input for the `get_caps()` method in the `CAP` class.
+- **Saving Timeseries:** Save the nested dictionary containing timeseries as a pickle file.
+- **Visualization:** Visualize the timeseries of a Schaefer, AAL, or Custom parcellation node or region/network in a specific subject's run, with options to save the plots.
+- **Parallel Processing:** Use parallel processing by specifying the number of CPU cores in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with TimeseriesExtractor.`get_bold()` to extract session 1 and 2 BOLD timeseries from 105 subjects from resting-state data (single run containing 360 volumes) and two task datasets (three runs containing 200 volumes each and two runs containing 200 volumes) reduced processing time from 5 hours 48 minutes to 1 hour 26 minutes (using 10 cores).
 
 **Main features for `CAP` includes:**
+- **Optimal Cluster Size Identification:** Perform the silhouette or elbow method to identify the optimal cluster size, saving the optimal model as an attribute.
+- **Grouping:** Perform CAPs analysis independently on groups of subject IDs. K-means clustering, silhouette and elbow methods, and plotting are done for each group when specified.
+- **CAP Visualization:** Visualize the CAPs as outer products or heatmaps, with options to use subplots to reduce the number of individual plots. You can save and use the plots. Refer to the docstring for the `caps2plot()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **Surface Plot Visualization:** Convert the atlas used for parcellation to a stat map projected onto a surface plot. Refer to the docstring for the `caps2surf()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **Correlation Matrix Creation:** Create a correlation matrix from CAPs. Refer to the docstring for the `caps2corr()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **CAP Metrics Calculation:** Calculate CAP metrics as described in  [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2]:
+    - *Temporal Fraction:* The proportion of total volumes spent in a single CAP over all volumes in a run.
+    - *Persistence:* The average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time).
+    - *Counts:* The frequency of each CAP observed in a run.
+    - *Transition Frequency:* The number of switches between different CAPs across the entire run.
 
-- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
-- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
-- Visualizing the CAPs identified as an outer product or heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `caps2plot()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
-- Visualizing CAPs as surface plots by converting the atlas used for parcellation to a stat map that gets projected onto a surface plot. Please refer to the docstring for the `caps2surf()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
-- Creating a correlation matrix from CAPs. Please refer to the docstring for the `caps2corr()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
-- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
-different CAPs across the entire run.
+**Additionally, the `neurocaps.analysis` submodule contains two additional functions:**
 
-**Additionally, the `neurocaps.analysis` submodule contains two additional functions**:
-- The `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
+- `merge_dicts`: Merge the subject_timeseries dictionaries for overlapping subjects across tasks to identify similar CAPs across different tasks. The merged dictionary can be saved as a pickle file.
+- `standardize`: Standardizes each run independently for all subjects in the subject timeseries.
 
-Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
+Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) for a more extensive demonstration of the features included in this package.
 
 Quick code example:
 
 ```python
 # Examples use randomized data
 
 from neurocaps.extraction import TimeseriesExtractor
@@ -210,18 +227,27 @@
 # Create correlation matrix
 cap_analysis.caps2corr(annot=True)
 ```
 **Plot Output:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/81620b36-55b0-4c83-be51-95d3f5280fa9)
 
 # Testing 
-This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slightly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+This package was tested using a closed dataset as well as a modified version of a single-subject open dataset to test the TimeseriesExtractor function on GitHub Actions. The open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. was also utilized. This data was obtained from the OpenfMRI database, accession number ds000031. 
 
-Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
+Modifications to the data included:
 
+- Truncating the preprocessed BOLD data and confounds from 448 timepoints to 40 timepoints.
+- Only including session 002 data.
+- Adding a dataset_description.json file to the fmriprep folder.
+- Excluding the nii.gz file in the root BIDS folder.
+- Retaining only the mask, truncated preprocessed BOLD file, and truncated confounds file in the fmriprep folder.
+- Slightly changing the naming style of the mask, preprocessed BOLD file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+- Testing with custom parcellations was done using the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas. This original atlas can be downloaded from.
+
+Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 # References
 [^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
 
 [^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
 
 [^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
```

### Comparing `neurocaps-0.9.3/README.md` & `neurocaps-0.9.3.post1/neurocaps.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,52 @@
+Metadata-Version: 2.1
+Name: neurocaps
+Version: 0.9.3.post1
+Summary: Co-activation Patterns (CAPs) Python package
+Author-email: Donisha Smith <donishasmith@outlook.com>
+Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
+Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: kneed
+Requires-Dist: nibabel
+Requires-Dist: nilearn!=0.10.3,>=0.10.1
+Requires-Dist: surfplot
+Requires-Dist: neuromaps
+Requires-Dist: pybids; platform_system != "Windows"
+
 # neurocaps
-This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
+This is a Python package designed to perform Co-activation Patterns (CAPs) analyses. It utilizes k-means clustering to group timepoints (TRs) into brain states, applicable to both resting-state and task-based fMRI data. The package is compatible with data preprocessed using **fMRIPrep** and assumes your directory is BIDS-compliant, containing a derivatives folder with a pipeline folder (such as fMRIPrep) that holds the preprocessed BOLD data.
 
 **Still in beta but stable.**
 
 # Installation
 
-**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
+**Note**: The `get_bold()` method in the `TimeseriesExtractor` class relies on pybids, which is only functional on POSIX operating systems and macOS. If you have a pickled timeseries dictionary in the correct nested form, you can use this package on Windows to visualize the BOLD timeseries, the `CAP` class, as well as the `merge_dicts()` and `standardize()` functions in the in the `neurcaps.analysis` submodule.
 
-To install, using your preferred terminal:
+To install, use your preferred terminal:
 
-**Installation with pip:**
+**Installation using pip:**
 
 ```bash
 
 pip install neurocaps
 
 ```
 
@@ -30,60 +63,77 @@
 git clone https://github.com/donishadsmith/neurocaps/
 cd neurocaps
 pip install -e .
 
 ```
 
 # Usage
-**This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
+**This package contains two main classes: `TimeseriesExtractor` for extracting the timeseries, and `CAP` for performing the CAPs analysis.**
+
+**Note:** When extracting the timeseries, this package uses either the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes have a left and right version (bilateral nodes). The number of ROIs and networks for the Schaefer atlas can be adjusted with the parcel_approach parameter when initializing the TimeseriesExtractor class.
+
+To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". For example:
+
+```python
+parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm": 1}}
+```
 
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes have a left and right version (bilateral nodes)**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+Similarly, the version of the AAL atlas can be modified using:
 
-If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
+```python
+parcel_approach = {"AAL": {"version": "SPM12"}}
+```
+
+If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions (bilateral nodes). 
 
 Custom Key Structure:
-- maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
-- nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+- 'maps': Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+- 'nodes':  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
 Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
 visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
-- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
+- 'regions': Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
         
-Example 
+Example:
 The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
 
 ```Python
 parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
-                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus",
+                              "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                              "regions": {"Vis" : {"lh": [0,1],
                                                   "rh": [3,4]},
                                          "Hippocampus": {"lh": [2],
                                                          "rh": [5]}}}}
  ```
 
 **Main features for `TimeseriesExtractor` includes:**
 
-- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
-- Saving the nested dictionary containing timeseries as a pickle file.
-- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
-- Ability to use parallel processing by specifying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
+- **Timeseries Extraction:** Extract timeseries for resting-state or task data, creating a nested dictionary containing the subject ID, run number, and associated timeseries. This serves as input for the `get_caps()` method in the `CAP` class.
+- **Saving Timeseries:** Save the nested dictionary containing timeseries as a pickle file.
+- **Visualization:** Visualize the timeseries of a Schaefer, AAL, or Custom parcellation node or region/network in a specific subject's run, with options to save the plots.
+- **Parallel Processing:** Use parallel processing by specifying the number of CPU cores in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with TimeseriesExtractor.`get_bold()` to extract session 1 and 2 BOLD timeseries from 105 subjects from resting-state data (single run containing 360 volumes) and two task datasets (three runs containing 200 volumes each and two runs containing 200 volumes) reduced processing time from 5 hours 48 minutes to 1 hour 26 minutes (using 10 cores).
 
 **Main features for `CAP` includes:**
+- **Optimal Cluster Size Identification:** Perform the silhouette or elbow method to identify the optimal cluster size, saving the optimal model as an attribute.
+- **Grouping:** Perform CAPs analysis independently on groups of subject IDs. K-means clustering, silhouette and elbow methods, and plotting are done for each group when specified.
+- **CAP Visualization:** Visualize the CAPs as outer products or heatmaps, with options to use subplots to reduce the number of individual plots. You can save and use the plots. Refer to the docstring for the `caps2plot()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **Surface Plot Visualization:** Convert the atlas used for parcellation to a stat map projected onto a surface plot. Refer to the docstring for the `caps2surf()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **Correlation Matrix Creation:** Create a correlation matrix from CAPs. Refer to the docstring for the `caps2corr()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **CAP Metrics Calculation:** Calculate CAP metrics as described in  [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2]:
+    - *Temporal Fraction:* The proportion of total volumes spent in a single CAP over all volumes in a run.
+    - *Persistence:* The average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time).
+    - *Counts:* The frequency of each CAP observed in a run.
+    - *Transition Frequency:* The number of switches between different CAPs across the entire run.
 
-- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
-- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
-- Visualizing the CAPs identified as an outer product or heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `caps2plot()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
-- Visualizing CAPs as surface plots by converting the atlas used for parcellation to a stat map that gets projected onto a surface plot. Please refer to the docstring for the `caps2surf()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
-- Creating a correlation matrix from CAPs. Please refer to the docstring for the `caps2corr()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
-- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
-different CAPs across the entire run.
+**Additionally, the `neurocaps.analysis` submodule contains two additional functions:**
 
-**Additionally, the `neurocaps.analysis` submodule contains two additional functions**:
-- The `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
+- `merge_dicts`: Merge the subject_timeseries dictionaries for overlapping subjects across tasks to identify similar CAPs across different tasks. The merged dictionary can be saved as a pickle file.
+- `standardize`: Standardizes each run independently for all subjects in the subject timeseries.
 
-Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
+Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) for a more extensive demonstration of the features included in this package.
 
 Quick code example:
 
 ```python
 # Examples use randomized data
 
 from neurocaps.extraction import TimeseriesExtractor
@@ -177,18 +227,27 @@
 # Create correlation matrix
 cap_analysis.caps2corr(annot=True)
 ```
 **Plot Output:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/81620b36-55b0-4c83-be51-95d3f5280fa9)
 
 # Testing 
-This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slightly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+This package was tested using a closed dataset as well as a modified version of a single-subject open dataset to test the TimeseriesExtractor function on GitHub Actions. The open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. was also utilized. This data was obtained from the OpenfMRI database, accession number ds000031. 
 
-Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
+Modifications to the data included:
+
+- Truncating the preprocessed BOLD data and confounds from 448 timepoints to 40 timepoints.
+- Only including session 002 data.
+- Adding a dataset_description.json file to the fmriprep folder.
+- Excluding the nii.gz file in the root BIDS folder.
+- Retaining only the mask, truncated preprocessed BOLD file, and truncated confounds file in the fmriprep folder.
+- Slightly changing the naming style of the mask, preprocessed BOLD file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+- Testing with custom parcellations was done using the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas. This original atlas can be downloaded from.
 
+Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 # References
 [^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
 
 [^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
 
 [^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
```

### Comparing `neurocaps-0.9.3/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.3.post1/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py` & `neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 import warnings
 def _check_confound_names(high_pass, specified_confound_names, n_acompcor_separate):
     if specified_confound_names == None:
         if high_pass:
-            # Do not use cosine or acompcor regressor if high pass filtering is not None. Acompcor regressors are estimated on high pass filtered version of data form fmriprep
-            confound_names = [
-                "trans_x", "trans_x_derivative1", "trans_x_power2", "trans_x_derivative1_power2",
-                "trans_y", "trans_y_derivative1", "trans_y_derivative1_power2", "trans_y_power2",
-                "trans_z", "trans_z_derivative1", "trans_z_power2", "trans_z_derivative1_power2",
-                "rot_x", "rot_x_derivative1", "rot_x_power2", "rot_x_derivative1_power2",
-                "rot_y", "rot_y_derivative1", "rot_y_power2", "rot_y_derivative1_power2",
-                "rot_z", "rot_z_derivative1", "rot_z_derivative1_power2", "rot_z_power2"
+            # Do not use cosine or acompcor regressor if high-pass filtering is not None. Acompcor regressors are estimated on high pass filtered version of data form fmriprep
+            confound_names = ["trans_x", "trans_x_derivative1","trans_y", "trans_y_derivative1", 
+                              "trans_z", "trans_z_derivative1",  "rot_x", "rot_x_derivative1",
+                              "rot_y", "rot_y_derivative1", "rot_z", "rot_z_derivative1"
             ]
         else:
             confound_names = [
-                "cosine*",
-                "trans_x", "trans_x_derivative1", "trans_x_power2", "trans_x_derivative1_power2",
-                "trans_y", "trans_y_derivative1", "trans_y_derivative1_power2", "trans_y_power2",
-                "trans_z", "trans_z_derivative1", "trans_z_power2", "trans_z_derivative1_power2",
-                "rot_x", "rot_x_derivative1", "rot_x_power2", "rot_x_derivative1_power2",
-                "rot_y", "rot_y_derivative1", "rot_y_power2", "rot_y_derivative1_power2",
-                "rot_z", "rot_z_derivative1", "rot_z_derivative1_power2", "rot_z_power2", 
-                "a_comp_cor_00", "a_comp_cor_01", "a_comp_cor_02", "a_comp_cor_03", "a_comp_cor_04", "a_comp_cor_05"
+                "cosine*","trans_x", "trans_x_derivative1","trans_y", "trans_y_derivative1", 
+                "trans_z", "trans_z_derivative1",  "rot_x", "rot_x_derivative1",
+                "rot_y", "rot_y_derivative1", "rot_z", "rot_z_derivative1", "a_comp_cor_00", 
+                "a_comp_cor_01", "a_comp_cor_02", "a_comp_cor_03", "a_comp_cor_04", "a_comp_cor_05"
             ]
     else:
         assert type(specified_confound_names) == list and len(specified_confound_names) > 0 , "confound_names must be a non-empty list."
         confound_names = specified_confound_names
 
     if n_acompcor_separate:
         check_confounds = [confound for confound in confound_names if "a_comp_cor" not in confound]
```

### Comparing `neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     import copy, json, math, numpy as np, pandas as pd, warnings
 
     # Intitialize subject dictionary
     subject_timeseries = {subj_id: {}}
     
     for run in run_list:
 
-        run_id = "run-1" if run == None else run
+        run_id = "run-0" if run == None else run
         run = run if run != None else ""
 
         # Get files from specific run
         nifti_file = [nifti_file for nifti_file in nifti_files if run in nifti_file.split("/")[-1]]
         if len(mask_files) != 0:
             mask_file = [mask_file for mask_file in mask_files if run in mask_file.split("/")[-1]]
         else:
```

### Comparing `neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.3.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3/neurocaps/analysis/cap.py` & `neurocaps-0.9.3.post1/neurocaps/analysis/cap.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,52 @@
     def __init__(self, parcel_approach: dict[dict], n_clusters: Union[int, list[int]]=5, cluster_selection_method: str=None, groups: dict=None):
         """CAP class
 
         Initializes the CAPs (Co-activation Patterns) class.
 
         Parameters
         ----------
-        node_labels: list[str]
-            Decoded or non-decoded Schaefer Atlas labels for the nodes.
+        parcel_approach: dict[dict]
+           The approach used to parcellate BOLD images. This should be a nested dictionary with the first key being the atlas name. The subkeys should include:
+            - "nodes": A list of node names in the order of the label IDs in the parcellation.
+            - "regions": The regions or networks in the parcellation.
+            - "maps": Directory path to the location of the parcellation file.
+
+          If the "Schaefer" or "AAL" option was used in the `TimeSeriesExtractor` class, you can initialize the `TimeSeriesExtractor` class with the `parcel_approach` 
+          that was initially used, then set this parameter to `TimeSeriesExtractor.parcel_approach`. For this parameter, only "Schaefer", "AAL", and "Custom" are supported.
         n_clusters: int or list[int], default=5
             The number of clusters to use. Can be a single integer or a list of integers.
         cluster_selection_method: str, default=None
             Method to find the optimal number of clusters. Options are "silhouette" or "elbow".
         groups: dict, default=None
-            A mapping of group names to subject IDs. Each group contains subject IDs for
-            separate CAP analysis. If None, CAPs are not separated by group.
+            A mapping of group names to subject IDs. Each group contains subject IDs for separate CAP analysis. If None, CAPs are not separated by group.
 
-        Notes
-        -----
-        The initialization ensures unique values if `n_clusters` is a list and checks for 
-        valid input types and values.
+        Notes for `parcel_approach`
+        ---------------------------
+        If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. This function assumes that the background label is "zero". 
+        Do not add a background label in the "nodes" or "networks" key; the zero index should correspond to the first ID that is not zero.
+
+        Custom Key Structure:
+        - 'maps': Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+        - 'nodes':  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+          Each label should match the parcellation index it represents. For example, if the parcellation label "1" corresponds to the left hemisphere 
+          visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
+          For timeseries extraction, this key is not required.
+        - 'regions': Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
+        
+        Example 
+        The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
+
+        parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "regions": {"Vis" : {"lh": [0,1],
+                                                  "rh": [3,4]},
+                                         "Hippocampus": {"lh": [2],
+                                                         "rh": [5]}}}}
+        
         """
         # Ensure all unique values if n_clusters is a list
         self._n_clusters = n_clusters if type(n_clusters) == int else sorted(list(set(n_clusters)))
         self._cluster_selection_method = cluster_selection_method 
 
         if type(n_clusters) == list:
             self._n_clusters =  self._n_clusters[0] if all([type(self._n_clusters) == list, len(self._n_clusters) == 1]) else self._n_clusters
@@ -64,50 +88,51 @@
 
     def get_caps(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], runs: Union[int, list[int]]=None, random_state: int=None, 
                  init: Union[np.array, Literal["k-means++", "random"]]="k-means++", n_init: Union[Literal["auto"],int]='auto', 
                  max_iter: int=300, tol: float=0.0001, algorithm: Literal["lloyd", "elkan"]="lloyd", show_figs: bool=False, 
                  output_dir: str=None, standardize: bool=True, epsilon: Union[int,float]=0, **kwargs) -> None:
         """""Generate CAPs
 
-        The purpose of this function is to concatenate the timeseries of each subject and perform kmeans clustering on the concatenated data.
+        Concatenates the timeseries of each subject and performs k-means clustering on the concatenated data.
         
         Parameters
         ----------
-        subject_timeseries: dict or str
-            A pickle file containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or
-            the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
-            ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
-            must consist of the timeseries associated with that run.
+        subject_timeseries: dict[dict[np.ndarray]] or str
+            Path of the pickle file containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or
+            the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject ID as a string, 
+            the second level must consist of the run numbers in the form of 'run-#' (where # is the corresponding number of the run), and the last level must consist of the timeseries 
+            (as a numpy array) associated with that run.
         runs: int or list[int], default=None
-            The run numbers to perform the CAPs analysis with. If None, all runs in the subject timeseries will be concatenated into a single dataframe.
+            The run numbers to perform the CAPs analysis with. If None, all runs in the subject timeseries will be concatenated into a single dataframe and subjected to k-means clustering.
         random_state: int, default=None
             The random state to use for scikit's KMeans function.
         init: "k-means++", "random", or array, default="k-means++"
-            Method for choosing initial cluster centroid. Please refer to scikit's KMeans documentation for more information.
+            Method for choosing initial cluster centroid. Refer to scikit's KMeans documentation for more information.
         n_init: "auto" or int, default="auto"
-            Number of times KMeans is ran with different intial clusters. Model with lowest inertia out of the runs will be selected.
-            Please refer to scikit's KMeans documentation for more information.
+            Number of times KMeans is ran with different initial clusters. The model with lowest inertia from these runs will be selected.
+            Refer to scikit's KMeans documentation for more information.
         max_iter: int, default=300
             Maximum number of iterations for a single run of KMeans.
         tol: float, default=1e-4,
-            Stopping criteria if the change of inertia is below value assuming `max_iter` has not been reached.
+            Stopping criterion if the change in inertia is below this value, assuming `max_iter` has not been reached.
         algorithm: "lloyd or "elkan", default="lloyd"
-            The type of algorithm to use. Please refer to scikit's KMeans documentation for more information.
+            The type of algorithm to use. Refer to scikit's KMeans documentation for more information.
         show_figs: bool, default=False
-            Display the plots of inertia scores for all groups if `cluster_selection_method`="elbow".
+            Display the plots of inertia scores for all groups if `cluster_selection_method` is set to "elbow".
         output_dir: str, default=None
-            Directory to save plot in if `cluster_selection_method`="elbow". Will create the directory if it does not exist.
+            Directory to save plot to if `cluster_selection_method` is set to "elbow". The directory will be created if it does not exist.
         standardize: bool, default=True
-            To z-score the features of the concatonated timeseries array.
+            Whether to z-score the features of the concatenated timeseries data.
         epsilon: int or float, default=0
-            Small number to add to the denominator when z-scoring for numerical stabilty.
+            A small number to add to the denominator when z-scoring for numerical stability.
         kwargs: dict
-            Dictionary to adjust certain parameters related to `cluster_selection_method`="elbow". Additional parameters includes "S", which adjust the sensitivity of finding the elbow 
-            (Larger values of `S` are more conservative and less sensitive to small fluctuations; this package uses KneeLocator from the kneed package to identify the elbow), defaults to 1, 
-            "dpi", to adjust the dpi of the elbow plot, defaults to 300, and "figsize", which adjust the size of the elbow plots.
+            Dictionary to adjust certain parameters related to `cluster_selection_method` when set to "elbow". Additional parameters include:
+             - "S": Adjusts the sensitivity of finding the elbow. Larger values are more conservative and less sensitive to small fluctuations. This package uses KneeLocator from the kneed package to identify the elbow. Default is 1.
+             - "dpi": Adjusts the dpi of the elbow plot. Default is 300.
+             - "figsize": Adjusts the size of the elbow plots.
         """
         
         if runs:
             if isinstance(runs,int): runs = list(runs)
     
         self._runs = runs if runs else "all"
         self._standardize = standardize
@@ -254,30 +279,29 @@
         """Generate heatmaps and outer product plots of CAPs
 
         This function produces seaborn heatmaps for each CAP. If groups were given when the CAP class was initialized, plotting will be done for all CAPs for all groups.
 
         Parameters
         ----------
         output_dir: str, default=None
-            Directory to save plots in. Will create the directory if it does not exist. If None, plots will not be saved.
+            Directory to save plots to. The directory will be created if it does not exist. If None, plots will not be saved.
         plot_options: str or list[str], default="outer product"
             Type of plots to create. Options are "outer product" or "heatmap".
         visual_scope: str or list[str], default="regions"
             Determines whether plotting is done at the region level or node level. 
-            For region level, the value of each nodes in the same regions are averaged together them plotted.
+            For region level, the value of each nodes in the same regions are averaged together then plotted.
             Options are "regions" or "nodes".
         task_title: str, default=None
-            Serves as the title of each plot as well as the name of the saved file if output_dir is given.
+            Serves as the title of each plot as well as the name of the saved file if `output_dir` is provided.
         show_figs: bool, default=True
-            Display figures or not to display figures.
+            Whether to display figures.
         subplots: bool, default=True
-            Produce subplots for outer product plots.
+            Whether to produce subplots for outer product plots.
         **kwargs: dict
             Keyword arguments used when saving figures. Valid keywords include:
-
             - "dpi": int, default=300
                 Dots per inch for the figure. Default is 300 if `output_dir` is provided and `dpi` is not specified.
             - "figsize": tuple, default=(8, 6)
                 Size of the figure in inches.
             - "fontsize": int, default=14
                 Font size for the title of individual plots or subplots.
             - "hspace": float, default=0.4
@@ -315,19 +339,20 @@
     
          Notes
         -----
         If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
         the zero index should correspond the first id that is not zero.
 
         Custom Key Structure:
-        - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this label is not required.
-        - nodes: A list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+        - 'maps': Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+        - 'nodes':  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
           Each label should match the parcellation index it represents. For example, if the parcellation label "1" corresponds to the left hemisphere 
           visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
-        - regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes.
+          For timeseries extraction, this key is not required.
+        - 'regions': Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
         
         Example 
         The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
 
         parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
                              "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                              "regions": {"Vis" : {"lh": [0,1],
@@ -634,53 +659,57 @@
         if not show_figs: plt.close()
 
     def calculate_metrics(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], tr: float=None, runs: Union[int]=None, continuous_runs: bool=False, 
                           metrics: Union[str, list[str]]=["temporal fraction", "persistence", "counts", "transition frequency"], return_df: bool=True, 
                           output_dir: str=None, file_name: str=None) -> dict:
         """Get CAPs metrics
 
-        Creates a single pandas Dataframe containing all participants containing CAP metrics as described in Liu et al., 2018 and Yang et al., 2021, 
-        where `temporal fraction` is the proportion of total volumes spent in a single CAP over all volumes in a run, `persistence` is the average 
-        time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and `counts` is the frequency 
-        of each CAP observed in a run, and `transition frequency` is the number of switches between different CAPs across the entire run.
+        Creates a single pandas DataFrame containing CAP metrics for all participants, as described in Liu et al., 2018 and Yang et al., 2021. 
+        The metrics include:
+
+        - 'temporal fraction': The proportion of total volumes spent in a single CAP over all volumes in a run.
+        - 'persistence;: The average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time).
+        - 'counts': The frequency of each CAP observed in a run.
+        - 'transition frequency': The number of switches between different CAPs across the entire run.
+
 
         Parameters
         ----------
-        subject_timeseries: dict or str
-            The absolute path of the pickle file containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or
-            the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
-            ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
-            must consist of the timeseries associated with that run. This should be the same dictionary used for `get_caps()`.
+        subject_timeseries: dict[dict[np.ndarray]] or str
+            Path of the pickle file containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or
+            the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject ID as a string, 
+            the second level must consist of the run numbers in the form of 'run-#' (where # is the corresponding number of the run), and the last level must consist of the timeseries 
+            (as a numpy array) associated with that run.
         tr: float, default=None
-            The repetition time. If given, persistence will be calculate as the average uninterrupted time spent in each CAP. If not give, persistence will be calculate
-            as the average uninterrupted volumes (TRs) spent in each state.
+            The repetition time (TR). If provided, persistence will be calculated as the average uninterrupted time spent in each CAP. 
+            If not provided, persistence will be calculated as the average uninterrupted volumes (TRs) spent in each state.
         runs: int or list[int], default=None
-            The run numbers to calculate cap metrics for. If None, cap metrics will be calculated for each run.
+            The run numbers to calculate CAP metrics for. If None, CAP metrics will be calculated for each run.
         continuous_runs: bool, default=False
             If True, all runs will be treated as a single, uninterrupted run.
         metrics: str or list[str], default=["temporal fraction", "persistence", "counts", "transition frequency"]
             The metrics to calculate. Available options include `temporal fraction`, `persistence`, `counts`, and `transition frequency`.
         return_df: str, default=True
-            If True, dataframe will be returned.
+            If True, returns the dataframe
         output_dir: str, default=None
-            Directory to save dataframe in. Will create the directory if it does not exist. If None, dataframe will not be saved.
+            Directory to save dataframe to. The directory will be created if it does not exist. If None, dataframe will not be saved.
         file_name: str, default=None
-            Name to save dataframe as if output_dir is not None.
+            Will serve as a prefix to append to the saved file names for the dataframes, if `output_dir` is provided.
 
         Returns
         -------
-        Dictionary containing pandas dataframes - one for each metric requested.
+        dict
+            Dictionary containing pandas DataFrames - one for each requested metric.
 
-        Notes
-        -----
-        The presence of 0 for specific CAPs in the "temporal fraction", "persistence", or "counts" dataframes, indicates that the participant had zero instances of 
-        a specific CAP.
+        Note
+        ----
+        The presence of 0 for specific CAPs in the "temporal fraction", "persistence", or "counts" dataframes indicates that the participant had zero instances of a specific CAP.
 
         References
-        -----
+        ----------
         Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
 
         Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. 
         NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
 
         """
         import collections, os, pandas as pd
@@ -814,25 +843,24 @@
 
         if return_df:
             return df_dict
 
     def caps2corr(self, output_dir: str=None, show_figs: bool=True, **kwargs):
         """Generate Correlation Matrix
 
-        This function produces the correlation matrix of all CAPs. If groups were given when the CAP class was initialized, a correlation matrix will be generated for each group. 
+        Produces the correlation matrix of all CAPs. If groups were given when the CAP class was initialized, a correlation matrix will be generated for each group. 
 
         Parameters
         ----------
         output_dir: str, default=None
-            Directory to save plots in. Will create the directory if it does not exist. If None, plots will not be saved.
+            Directory to save plots to. The directory will be created if it does not exist. If None, plots will not be saved.
         show_figs: bool, default=True
-            Display figures or not to display figures.
+            Whether to display figures.
         **kwargs: dict
             Keyword arguments used when saving figures. Valid keywords include:
-
             - "dpi": int, default=300
                 Dots per inch for the figure. Default is 300 if `output_dir` is provided and `dpi` is not specified.
             - "figsize": tuple, default=(8, 6)
                 Size of the figure in inches.
             - "fontsize": int, default=14
                 Font size for the title of individual plots or subplots.
             - "xticklabels_size": int, default=8
@@ -895,38 +923,38 @@
             if not show_figs: plt.close()
             # Save figure
             if output_dir:
                 if not os.path.exists(output_dir): os.makedirs(output_dir)
                 full_filename = f"{group.replace(' ', '_')}_correlation_matrix.png"
                 display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')
 
-    def caps2surf(self, output_dir: str=None, show_figs: bool = True, fwhm: float=None, 
-                  fslr_density: str="32k", save_stat_map: bool=False, method: str="linear",  **kwargs):
-        """Project CAPs onto 
+    def caps2surf(self, output_dir: str=None, show_figs: bool=True, fwhm: float=None, 
+                  fslr_density: str="32k", method: str="linear", save_stat_map: bool=False, **kwargs):
+        """Project CAPs onto surface plots
         
         Converts atlas into a stat map by replacing labels with the corresponding from the cluster centroids then plots on a surface plot.
         This function uses surfplot for surface plotting.
 
         Parameters
         ----------
         output_dir: str, default=None
-            Directory to save plots in. Will create the directory if it does not exist. If None, plots will not be saved. 
+            Directory to save plots to. The directory will be created if it does not exist. If None, plots will not be saved. 
         show_figs: bool, default=True
-            Display figures or not to display figures.
+            Whether to display figures.
         fwhm: float, defualt=None
-            Strength of spatial smoothing to apply in millimeters.
+            Strength of spatial smoothing to apply (in millimeters) to the statistical map prior to interpolating from MNI152 space to fslr surface space. 
+            Note, this can assist with coverage issues in the plot.
         fslr_density: str, default="32k"
-            Density of the fslr surface when converting from mni 152 space to fslr surface. Options are 
-            "32k" or "164k".
+            Density of the fslr surface when converting from MNI152 space to fslr surface. Options are "32k" or "164k".
         method: str, default="linear"
-            Interpolation method to use when converting from mni152 space to fslr surface. Options are "linear"
-            or "nearest".
+            Interpolation method to use when converting from MNI152 space to fslr surface. Options are "linear" or "nearest".
+        save_stat_map: bool, default=False
+            If True, saves the statistical map for each CAP for all groups as a Nifti1Image if `output_dir` is provided.
         **kwargs : dict
             Additional parameters to pass to modify certain plot parameters. Options include:
-
             - "dpi": int, default=300
                 Dots per inch for the plot.
             - "title_pad": int, default=-3
                 Padding for the plot title.
             - "cmap": str, default="cold_hot"
                 Colormap to be used for the plot.
             - "cbar_location": str, default="bottom"
@@ -965,24 +993,22 @@
                 Scale factors for the plot.
 
             Please refer to surfplot's documentation for specifics: 
             https://surfplot.readthedocs.io/en/latest/generated/surfplot.plotting.Plot.html#surfplot.plotting.Plot.
 
         Returns
         -------
-        Nifti Stat map
+        Nifti1Image
+            Nifti statistical map.
 
-        Notes
+        Note
         -----
         Assumes that atlas background label is zero and atlas is in MNI space. Also assumes that the indices from the cluster centroids are related
         to the atlas by an offset of one. For instance, index 0 of the cluster centroid vector is the first nonzero label, which is assumed to be at the 
         first index of the array in sorted(np.unique(atlas_fdata)).
-
-        Using fwhm to adjust smoothing may help coverage issues.
-
         """
 
         import nibabel as nib, numpy as np, os
         from nilearn import image
         from nilearn.plotting.cm import _cmap_d 
         from neuromaps.transforms import mni152_to_fslr
         from neuromaps.datasets import fetch_fslr
```

### Comparing `neurocaps-0.9.3/neurocaps/analysis/merge.py` & `neurocaps-0.9.3.post1/neurocaps/analysis/merge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 import numpy as np
 from typing import Union
 from .._utils import _convert_pickle_to_dict
 
 def merge_dicts(subject_timeseries_list: Union[list[dict], list[str]], return_combined_dict: bool=True, return_reduced_dicts: bool=False, output_dir: str=None, file_name: str=None) -> dict:
     """Merge subject timeseries
 
-    Merge subject timeseries dictionaries or pickle files to the first dictionary or pickle file in the list.
-    Repetition times from the same subject and run are merged together. The combined dicitonary will only include subjects
+    Merge subject timeseries dictionaries or pickle files into the first dictionary or pickle file in the list.
+    Repetition times from the same subject and run are merged together. The combined dictionary will only include subjects
     that are present in all dictionaries.
 
     Parameters
     ----------
-    subject_timeseries_list: list[dict] or list[str]
-        The list of pickle files containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or a liist of the
-        the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
-        ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
-        must consist of the timeseries associated with that run.
+    subject_timeseries_list: list[dict[dict[np.ndarray]]] or list[str]
+        A list of pickle files containing the nested subject timeseries dictionary saved by the `TimeSeriesExtractor` class or a list of nested subject 
+        timeseries dictionaries produced by the `TimeSeriesExtractor` class. The first level of the nested dictionary must consist of the subject ID as a string, 
+        the second level must consist of the run numbers in the form of 'run-#' (where # is the corresponding number of the run), and the last level must consist of the timeseries 
+        (as a numpy array) associated with that run.
     return_combined_dict: bool, default=True,
-        Returns the merged dictionaries if True
+        If True, returns the merged dictionaries.
     return_reduced_dicts: bool, default=False
-        Returns the list of dictionaries provided with only the subjects present in the combined dictionary. Returns dictionaries in the same order
-        they are listed in the `subject_timeseries_list` parameter.
+        If True, returns the list of dictionaries provided with only the subjects present in the combined dictionary. The dictionaries are returned in the same order as listed in 
+        the `subject_timeseries_list` parameter.
     output_dir: str, default=None
-        Directory to save the merged dictionary to. Will be saved as a pickle file.
+        Directory to save the merged dictionary to. Will be saved as a pickle file. The directory will be created if it does not exist.
     file_name: str, default=None
-        Name to save merged dictionary as.
-
-    Raises
-    ------
-    AssertionError
-        If the length of `subject_timeseries_list` is less than two.
+        Name to save the merged dictionary as.
 
     Returns
     -------
     dict
     """
     assert len(subject_timeseries_list) > 1, "Merging cannot be done with less than two dictionaries or files."
```

### Comparing `neurocaps-0.9.3/neurocaps/analysis/standardize.py` & `neurocaps-0.9.3.post1/neurocaps/analysis/standardize.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 def standardize(subject_timeseries: Union[dict,str]) -> dict:
     """Standardize subject timeseries 
     
     Standardizes each run independently for all subjects in the subject timeseries.
 
     Parameters
     ----------
-    subject_timeseries_list: dict or str
-        The list of pickle files containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or a liist of the
-        the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
-        ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
-        must consist of the timeseries associated with that run.
+    subject_timeseries_list: dict[dict[np.ndarray]] or str
+        A list of pickle files containing the nested subject timeseries dictionary saved by the `TimeSeriesExtractor` class or a list of nested subject 
+        timeseries dictionaries produced by the `TimeSeriesExtractor` class. The first level of the nested dictionary must consist of the subject ID as a string, 
+        the second level must consist of the run numbers in the form of 'run-#' (where # is the corresponding number of the run), and the last level must consist of the timeseries 
+        (as a numpy array) associated with that run.
 
     Returns
     -------
     dict
     """
 
     if ".pkl" in subject_timeseries:
```

### Comparing `neurocaps-0.9.3/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.3.post1/neurocaps/extraction/timeseriesextractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,73 +1,90 @@
 import json, os, re, sys, warnings
 from typing import Union
 from .._utils import _TimeseriesExtractorGetter, _check_confound_names, _check_parcel_approach, _extract_timeseries
 
 class TimeseriesExtractor(_TimeseriesExtractorGetter):
-    def __init__(self, space: str="MNI152NLin2009cAsym", standardize: Union[bool,str]="zscore_sample", detrend: bool=False , low_pass: float=None, high_pass: float=None, 
-                 parcel_approach : dict={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}, use_confounds: bool=True, confound_names: list[str]=None, 
+    def __init__(self, space: str="MNI152NLin2009cAsym", standardize: Union[bool,str]="zscore_sample", detrend: bool=True , low_pass: float=None, high_pass: float=None, 
+                 parcel_approach : dict[dict]={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}, use_confounds: bool=True, confound_names: list[str]=None, 
                  fwhm: float=None, fd_threshold: float=None, n_acompcor_separate: int=None, dummy_scans: int=None):
         """Timeseries Extractor Class
         
-        Initializes the TimeseriesExtractor class to prepare for Co-activation Patterns (CAPs) analysis.
+        Initializes the TimeseriesExtractor class.
 
         Parameters
         ----------
         space: str, default="MNI152NLin2009cAsym"
-            The brain template space data is in. 
-        standardize: bool, default=True
+            The standard template space that the preprocessed bold data is registered to. 
+        standardize: bool, default="zscore_sample"
             Determines whether to standardize the timeseries. Refer to Nilearn's NiftiLabelsMasker for available options. 
         detrend: bool, default=True
-            Detrends timeseries during extraction.
+            Detrends the timeseries during extraction.
         low_pass: bool, default=None
-            Signals above cutoff frequency will be filtered out.
+            Filters out signals above the specified cutoff frequency.
         high_pass: float, default=None
-            Signals below cutoff frequency will be filtered out.
-        parcel_approach: dict, default={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}
-            Approach to use to parcellate bold images. Should be in the form of a nested dictionary where the first key is the atlas.
-            Currently only "Schaefer", "AAL", and "Custom" is supported. For the sub-dictionary for "Schaefer", available options includes "n_rois", "yeo_networks", and "resolution_mm".
-            Please refer to the documentation for Nilearn's `datasets.fetch_atlas_schaefer_2018` for valid inputs. For the subdictionary for "AAL" only "version"
-            is an option. Please refer to the documentation for Nilearn's `datasets.fetch_atlas_aal` for valid inputs. As of version 0.8.9, you can replace "Schaefer"
-            and "AAL" with "Custom". At minimum, if "Custom" is specified, a subkey, called "maps" specifying the directory location of the parcellation as a Nifti (e.g .nii or .nii.gz)
-            - {"Custom": {"maps": "/location/to/parcellation.nii.gz"}}.
+            Filters out signals below the specified cutoff frequency.
+        parcel_approach: dict[dict], default={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}
+            The approach to parcellate BOLD images. This should be a nested dictionary with the first key being the atlas name. Currently, only "Schaefer", "AAL", and "Custom" are supported.
+            - For "Schaefer", available options include n_rois, yeo_networks, and resolution_mm. Refer to Nilearn's datasets.fetch_atlas_schaefer_2018 for valid inputs.
+            - For "AAL", the only option is version. Refer to Nilearn's datasets.fetch_atlas_aal for valid inputs.
+            - For "Custom", the key must include a subkey called maps specifying the directory location of the parcellation Nifti file (e.g., {"Custom": {"maps": "/location/to/parcellation.nii.gz"}}).
         use_confounds: bool, default=True
-            To use confounds when extracting timeseries.
-        confound_names: List[str], default=None
-            Names of confounds to use in confound files. If None, default confounds are used.
+            Determines whether to use confounds when extracting timeseries.
+        confound_names: list[str], default=None
+            Specifies the names of confounds to use from confound files. If None, default confounds are used. Note, an asterisk ("*") can be used to find confound names that start with the term preceding the asterisk. 
+            For instance, "cosine*" will find all confound names in the confound files starting with "cosine".
         fwhm: float, default=None
-            Parameter for spatial smoothing.
+            Applies spatial smoothing to data (in millimeters). Note that using parcellations already averages voxels within parcel boundaries, which can improve signal-to-noise ratio (SNR) assuming Gaussian noise distribution. 
+            However, smoothing may also blur parcel boundaries.
         fd_threshold: float, default=None
-            Threshold criteria to remove frames after nuisance regression and timeseries extraction. For this to work, a column named "framewise_displacement" must be
-            in the confounds dataframe and `use_confounds` must be true. Additionally, 'framewise_displacemnt' does not need to be specified in the `confound_names` for this to work.
+            Sets a threshold to remove frames after nuisance regression and timeseries extraction. This requires a column named framewise_displacement in the confounds dataframe and use_confounds set to True. 
+            Additionally, `framewise_displacement` should not need be specified in confound_names is using this parameter.
         n_acompcor_separate: int, default = None
-            The number of separate acompcor components derived from the white-matter (WM) and cerebrospinal (CSF) masks to use. For instance if '5' is assigned to this parameter
-            then the first five components derived from the WM mask and the first five components derived from the CSF mask will be used, resulting in ten acompcor components being
-            used. If this parameter is not none any acompcor components listed in the confound names will be disregarded in order to locate the first 'n' components derived from the 
-            masks. To use the acompcor components derived from the combined masks (WM & CSF) leave this parameter as 'None' and list the specific acompcors of interest in the 
-            `confound_names` parameter.
+            Specifies the number of separate acompcor components derived from white-matter (WM) and cerebrospinal fluid (CSF) masks to use. For example, if set to 5, the first five components from the WM mask 
+            and the first five from the CSF mask will be used, totaling ten acompcor components. If this parameter is not None, any acompcor components listed in confound_names will be disregarded. To use acompcor 
+            components derived from combined masks (WM & CSF), leave this parameter as None and list the specific acompcors of interest in confound_names..
         dummy_scans: float, default=None
-            Removes the first `n` number of volumes before extracting the timeseries.
+            Removes the first n volumes before extracting the timeseries.
         
         Notes for `confounds_names`
         --------------------------
-        For the `confound_names` parameter, an asterisk ("*") can be used to find the name of confounds that starts with the term preceding the asterisk.
-        For instance, "cosine*" will find all confound names in the confound files starting with "cosine".
+        Additionally, default `confound_names` changes if `high_pass` is not None.
+
+        If `high_pass` is not None, then the cosine parameters and acompcor parameters are not used because the cosine parameters are high-pass filters
+        and the acompcor regressors are estimated on the high-pass filtered version of the data:
+        confound_names = ["trans_x", "trans_x_derivative1","trans_y", "trans_y_derivative1", 
+                              "trans_z", "trans_z_derivative1",  "rot_x", "rot_x_derivative1",
+                              "rot_y", "rot_y_derivative1", "rot_z", "rot_z_derivative1"
+            ]
+
+        If `high_pass` is None, then:
+            confound_names = ["trans_x", "trans_x_derivative1","trans_y", "trans_y_derivative1", 
+                              "trans_z", "trans_z_derivative1",  "rot_x", "rot_x_derivative1",
+                              "rot_y", "rot_y_derivative1", "rot_z", "rot_z_derivative1"
+            ]
+        else:
+            confound_names = [
+                "cosine*","trans_x", "trans_x_derivative1","trans_y", "trans_y_derivative1", 
+                "trans_z", "trans_z_derivative1",  "rot_x", "rot_x_derivative1",
+                "rot_y", "rot_y_derivative1", "rot_z", "rot_z_derivative1", "a_comp_cor_00", 
+                "a_comp_cor_01", "a_comp_cor_02", "a_comp_cor_03", "a_comp_cor_04", "a_comp_cor_05"
+            ]
 
         Notes for `parcel_approach`
         ---------------------------
-        If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
-        the zero index should correspond the first id that is not zero.
+        If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. This function assumes that the background label is "zero". 
+        Do not add a background label in the "nodes" or "networks" key; the zero index should correspond to the first ID that is not zero.
 
         Custom Key Structure:
-        - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
-        - nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+        - 'maps': Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+        - 'nodes':  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
           Each label should match the parcellation index it represents. For example, if the parcellation label "1" corresponds to the left hemisphere 
           visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
           For timeseries extraction, this key is not required.
-        - regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
+        - 'regions': Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
         
         Example 
         The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
 
         parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
                              "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                              "regions": {"Vis" : {"lh": [0,1],
@@ -88,46 +105,56 @@
             self._signal_clean_info["fd_threshold"] = fd_threshold
 
     def get_bold(self, bids_dir: str, task: str, session: Union[int,str]=None, runs: list[int]=None, condition: str=None, tr: Union[int, float]=None, 
                  run_subjects: list[str]=None, exclude_subjects: list[str]= None, pipeline_name: str=None, n_cores: Union[bool, int]=None, verbose: bool=True, flush_print: bool=False,
                  exclude_niftis: list[str]=None) -> None: 
         """Get Bold Data
 
-        Collects files needed to extract timeseries data from NIfTI files for BIDS-compliant datasets.
+        Collects files needed to extract timeseries data from NIfTI files for BIDS-compliant datasets containing a derivatives folder. This function assumes that your BOLD data was preprocessed using a standard 
+        preprocessing pipeline such as fMRIPrep.
 
         Parameters
         ----------
         bids_dir: str
             Path to a BIDS compliant directory. 
         task: str
             Name of task to process.
         session: int, default=None
             Session to extract timeseries from. Only a single session can be extracted at a time. 
         runs: list[int], default=None
-            Run number to extract timeseries data from. Extracts all runs if unspecified.
+            List of run numbers to extract timeseries data from. Extracts all runs if unspecified. For instance, if only "run-0" and "run-1" should be extracted, then 
+            `runs=[0,1]`.
         condition: str, default=None
             Specific condition in the task to extract from. Only a single condition can be extracted at a time.
         tr: int or float, default=None
             Repetition time for task.
         run_subjects: list[str], default=None
             List of subject IDs to process. Processes all subjects if None.
         exclude_subjects: list[str], default=None
             List of subject IDs to exclude.  
         pipeline_name: str, default=None
             The name of the pipeline folder in the derivatives folder containing the preprocessed data. If None, BIDSLayout will use the name of dset_dir with derivatives=True. This parameter
-            should be used if their are multiple pipelines in the derivatives folder.
+            should be used if there are multiple pipelines in the derivatives folder.
         n_cores: bool or int, default=None
             The number of CPU cores to use for multiprocessing. If true, all available cores will be used.
         verbose: bool, default=True
-            Print subject specific information such as confounds being extracted and id and run of subject being processed during timeseries extraction.
+            Print subject-specific information such as confounds being extracted, and id and run of subject being processed during timeseries extraction.
         flush_print: bool, default=False
-            Flush the printed subject specific infomation produced during the timeseries extraction process.
+            Flush the printed subject-specific infomation produced during the timeseries extraction process.
         exclude_niftis: list[str], default=None
-            Exclude certain preprocessed nifti files to prevent the timeseries of that file from being extracted. Used if there are specific runs across differnt participants that need to be
+            List of specific preprocessed NIfTI files to exclude, preventing their timeseries from being extracted. Used if there are specific runs across differnt participants that need to be
             excluded.
+
+        Note
+        ----
+        This function stores the extracted timeseries as a nested dictionary and stores it in `self.subject_timeseres`. The first level of the nested dictionary consists of the subject ID as a string, 
+        the second level consists of the run numbers in the form of 'run-#' (where # is the corresponding number of the run), and the last level must consist of the timeseries 
+        (as a numpy array) associated with that run.
+
+        Additionally, if your files do not specify a run number due to your subjects only having a single run, the run id key for the second level of the nested dictionary defaults to "run-0".
         """
         import bids, multiprocessing
 
         if sys.platform == "win32":
             raise SystemError("Cannot use this method on Windows devices since it relies on the `pybids` module which is only compatable with POSIX systems.")
 
         # Update attributes
@@ -294,17 +321,17 @@
         """Save Bold Data
 
         Saves the timeseries dictionary obtained from running `get_bold()` as a pickle file.
 
         Parameters
         ----------
         output_dir: str
-            Directory to save the file to. Will create the directory if it does not exist.
+            Directory to save to. The directory will be created if it does not exist.
         file_name: str, default=None
-            Name of the file without or without the "pkl" extension.
+            Name of the file with or without the "pkl" extension.
         """
         import pickle
 
         if not hasattr(self, "_subject_timeseries"):
             raise AttributeError("Cannot save pickle file since `self._subject_timeseries` does not exist, either run `self.get_bold()` or assign a valid timeseries dictionary to `self.subject_timeseries`.")
 
         if output_dir:
@@ -320,47 +347,47 @@
         """Plot Bold Data
 
         Collects files needed to extract timeseries data from NIfTI files for BIDS-compliant datasets.
 
         Parameters
         ----------
         subj_id: str
-            Subject ID, as a string, to plot.
+            The subject ID.
         run: int
             The run to plot.
         roi_indx: int or list[int], default=None
-            The indices of the Schaefer nodes to plot. See self.node_indices for valid node names and indices.
+            The indices of the parcellation nodes to plot. See self.node_indices for valid node names and indices.
         region: str, default=None
             The region of the parcellation to plot. If not None, all nodes in the specified region will be averaged then plotted. See `regions` in self.parcel_approach 
             for valid regions names.
         show_figs: bool, default=True
-            Whether to show figires or not to show figures
+            Whether to show the figures.
         output_dir: str, default=None
-            Directory to save the file to. Will create the directory if it does not exist.
+            Directory to save to. The directory will be created if it does not exist.
         file_name: str, default=None
             Name of the file without the extension.
         **kwargs: dict
             Keyword arguments used when saving figures. Valid keywords include:
-        
             - "dpi": int, default=300
                 Dots per inch for the figure. Default is 300 if `output_dir` is provided and `dpi` is not specified.
             - "figsize": tuple, default=(11, 5)
                 Size of the figure in inches. Default is (11, 5) if "figsize" is not specified.
 
         Notes
         -----
         If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
         the zero index should correspond the first id that is not zero.
 
         Custom Key Structure:
-        - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this label is not required.
-        - nodes: A list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+        - 'maps': Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+        - 'nodes':  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
           Each label should match the parcellation index it represents. For example, if the parcellation label "1" corresponds to the left hemisphere 
           visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
-        - regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes.
+          For timeseries extraction, this key is not required.
+        - 'regions': Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
         
         Example 
         The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
 
         parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
                              "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                              "regions": {"Vis" : {"lh": [0,1],
@@ -370,15 +397,15 @@
         """
     
         import matplotlib.pyplot as plt, numpy as np
 
         if not hasattr(self, "_subject_timeseries"):
             raise AttributeError("Cannot plot bold data since `self._subject_timeseries` does not exist, either run `self.get_bold()` or assign a valid timeseries structure to self.subject_timeseries.")
 
-        if isinstance(subj_id,int): subj_id = str(subj_id)
+        if isinstance(subj_id, int): subj_id = str(subj_id)
 
         if roi_indx !=None and region != None:
             raise ValueError("`roi_indx` and `region` can not be used simultaneously.")
         
         if file_name != None and output_dir == None: warnings.warn("`file_name` supplied but no `output_dir` specified. Files will not be saved.")
         
         if output_dir:
```

### Comparing `neurocaps-0.9.3/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.3.post1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,19 @@
-Metadata-Version: 2.1
-Name: neurocaps
-Version: 0.9.3
-Summary: Co-activation patterns Python package
-Author-email: Donisha Smith <donishasmith@outlook.com>
-Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
-Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: matplotlib
-Requires-Dist: seaborn
-Requires-Dist: kneed
-Requires-Dist: nibabel
-Requires-Dist: nilearn!=0.10.3,>=0.10.1
-Requires-Dist: surfplot
-Requires-Dist: neuromaps
-Requires-Dist: pybids; platform_system != "Windows"
-
 # neurocaps
-This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
+This is a Python package designed to perform Co-activation Patterns (CAPs) analyses. It utilizes k-means clustering to group timepoints (TRs) into brain states, applicable to both resting-state and task-based fMRI data. The package is compatible with data preprocessed using **fMRIPrep** and assumes your directory is BIDS-compliant, containing a derivatives folder with a pipeline folder (such as fMRIPrep) that holds the preprocessed BOLD data.
 
 **Still in beta but stable.**
 
 # Installation
 
-**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
+**Note**: The `get_bold()` method in the `TimeseriesExtractor` class relies on pybids, which is only functional on POSIX operating systems and macOS. If you have a pickled timeseries dictionary in the correct nested form, you can use this package on Windows to visualize the BOLD timeseries, the `CAP` class, as well as the `merge_dicts()` and `standardize()` functions in the in the `neurcaps.analysis` submodule.
 
-To install, using your preferred terminal:
+To install, use your preferred terminal:
 
-**Installation with pip:**
+**Installation using pip:**
 
 ```bash
 
 pip install neurocaps
 
 ```
 
@@ -63,60 +30,77 @@
 git clone https://github.com/donishadsmith/neurocaps/
 cd neurocaps
 pip install -e .
 
 ```
 
 # Usage
-**This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
+**This package contains two main classes: `TimeseriesExtractor` for extracting the timeseries, and `CAP` for performing the CAPs analysis.**
+
+**Note:** When extracting the timeseries, this package uses either the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes have a left and right version (bilateral nodes). The number of ROIs and networks for the Schaefer atlas can be adjusted with the parcel_approach parameter when initializing the TimeseriesExtractor class.
+
+To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". For example:
+
+```python
+parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm": 1}}
+```
 
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes have a left and right version (bilateral nodes)**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+Similarly, the version of the AAL atlas can be modified using:
 
-If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
+```python
+parcel_approach = {"AAL": {"version": "SPM12"}}
+```
+
+If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions (bilateral nodes). 
 
 Custom Key Structure:
-- maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
-- nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+- 'maps': Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+- 'nodes':  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
 Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
 visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
-- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
+- 'regions': Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
         
-Example 
+Example:
 The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
 
 ```Python
 parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
-                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus",
+                              "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                              "regions": {"Vis" : {"lh": [0,1],
                                                   "rh": [3,4]},
                                          "Hippocampus": {"lh": [2],
                                                          "rh": [5]}}}}
  ```
 
 **Main features for `TimeseriesExtractor` includes:**
 
-- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
-- Saving the nested dictionary containing timeseries as a pickle file.
-- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
-- Ability to use parallel processing by specifying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
+- **Timeseries Extraction:** Extract timeseries for resting-state or task data, creating a nested dictionary containing the subject ID, run number, and associated timeseries. This serves as input for the `get_caps()` method in the `CAP` class.
+- **Saving Timeseries:** Save the nested dictionary containing timeseries as a pickle file.
+- **Visualization:** Visualize the timeseries of a Schaefer, AAL, or Custom parcellation node or region/network in a specific subject's run, with options to save the plots.
+- **Parallel Processing:** Use parallel processing by specifying the number of CPU cores in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with TimeseriesExtractor.`get_bold()` to extract session 1 and 2 BOLD timeseries from 105 subjects from resting-state data (single run containing 360 volumes) and two task datasets (three runs containing 200 volumes each and two runs containing 200 volumes) reduced processing time from 5 hours 48 minutes to 1 hour 26 minutes (using 10 cores).
 
 **Main features for `CAP` includes:**
+- **Optimal Cluster Size Identification:** Perform the silhouette or elbow method to identify the optimal cluster size, saving the optimal model as an attribute.
+- **Grouping:** Perform CAPs analysis independently on groups of subject IDs. K-means clustering, silhouette and elbow methods, and plotting are done for each group when specified.
+- **CAP Visualization:** Visualize the CAPs as outer products or heatmaps, with options to use subplots to reduce the number of individual plots. You can save and use the plots. Refer to the docstring for the `caps2plot()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **Surface Plot Visualization:** Convert the atlas used for parcellation to a stat map projected onto a surface plot. Refer to the docstring for the `caps2surf()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **Correlation Matrix Creation:** Create a correlation matrix from CAPs. Refer to the docstring for the `caps2corr()` method in the `CAP` class for available **kwargs arguments and parameters to modify plots.
+- **CAP Metrics Calculation:** Calculate CAP metrics as described in  [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2]:
+    - *Temporal Fraction:* The proportion of total volumes spent in a single CAP over all volumes in a run.
+    - *Persistence:* The average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time).
+    - *Counts:* The frequency of each CAP observed in a run.
+    - *Transition Frequency:* The number of switches between different CAPs across the entire run.
 
-- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
-- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
-- Visualizing the CAPs identified as an outer product or heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `caps2plot()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
-- Visualizing CAPs as surface plots by converting the atlas used for parcellation to a stat map that gets projected onto a surface plot. Please refer to the docstring for the `caps2surf()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
-- Creating a correlation matrix from CAPs. Please refer to the docstring for the `caps2corr()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
-- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
-different CAPs across the entire run.
+**Additionally, the `neurocaps.analysis` submodule contains two additional functions:**
 
-**Additionally, the `neurocaps.analysis` submodule contains two additional functions**:
-- The `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
+- `merge_dicts`: Merge the subject_timeseries dictionaries for overlapping subjects across tasks to identify similar CAPs across different tasks. The merged dictionary can be saved as a pickle file.
+- `standardize`: Standardizes each run independently for all subjects in the subject timeseries.
 
-Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
+Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) for a more extensive demonstration of the features included in this package.
 
 Quick code example:
 
 ```python
 # Examples use randomized data
 
 from neurocaps.extraction import TimeseriesExtractor
@@ -210,24 +194,33 @@
 # Create correlation matrix
 cap_analysis.caps2corr(annot=True)
 ```
 **Plot Output:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/81620b36-55b0-4c83-be51-95d3f5280fa9)
 
 # Testing 
-This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slightly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+This package was tested using a closed dataset as well as a modified version of a single-subject open dataset to test the TimeseriesExtractor function on GitHub Actions. The open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. was also utilized. This data was obtained from the OpenfMRI database, accession number ds000031. 
 
-Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
+Modifications to the data included:
+
+- Truncating the preprocessed BOLD data and confounds from 448 timepoints to 40 timepoints.
+- Only including session 002 data.
+- Adding a dataset_description.json file to the fmriprep folder.
+- Excluding the nii.gz file in the root BIDS folder.
+- Retaining only the mask, truncated preprocessed BOLD file, and truncated confounds file in the fmriprep folder.
+- Slightly changing the naming style of the mask, preprocessed BOLD file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+- Testing with custom parcellations was done using the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas. This original atlas can be downloaded from.
 
+Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 # References
 [^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
 
 [^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
 
 [^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
 
 [^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
 
 [^5]: Huang CC, Rolls ET, Feng J, Lin CP. An extended Human Connectome Project multimodal parcellation atlas of the human cortex and subcortical areas. Brain Struct Funct. 2022 Apr;227(3):763-778. Epub 2021 Nov 17. doi: 10.1007/s00429-021-02421-6
 
-[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
+[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
```

### Comparing `neurocaps-0.9.3/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.3.post1/neurocaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3/pyproject.toml` & `neurocaps-0.9.3.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,93 +2,94 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6e65 7572 6f63 6170 7322 0d0a 7665   "neurocaps"..ve
-00000080: 7273 696f 6e20 3d20 2230 2e39 2e33 220d  rsion = "0.9.3".
-00000090: 0a61 7574 686f 7273 203d 205b 7b6e 616d  .authors = [{nam
-000000a0: 6520 3d20 2244 6f6e 6973 6861 2053 6d69  e = "Donisha Smi
-000000b0: 7468 222c 2065 6d61 696c 203d 2022 646f  th", email = "do
-000000c0: 6e69 7368 6173 6d69 7468 406f 7574 6c6f  nishasmith@outlo
-000000d0: 6f6b 2e63 6f6d 227d 5d0d 0a64 6573 6372  ok.com"}]..descr
-000000e0: 6970 7469 6f6e 203d 2022 436f 2d61 6374  iption = "Co-act
-000000f0: 6976 6174 696f 6e20 7061 7474 6572 6e73  ivation patterns
-00000100: 2050 7974 686f 6e20 7061 636b 6167 6522   Python package"
-00000110: 0d0a 7265 6164 6d65 203d 2022 5245 4144  ..readme = "READ
-00000120: 4d45 2e6d 6422 0d0a 7265 7175 6972 6573  ME.md"..requires
-00000130: 2d70 7974 686f 6e20 3d20 223e 3d33 2e39  -python = ">=3.9
-00000140: 2e30 220d 0a6b 6579 776f 7264 7320 3d20  .0"..keywords = 
-00000150: 5b22 7079 7468 6f6e 222c 2022 436f 2d41  ["python", "Co-A
-00000160: 6374 6976 6174 696f 6e20 5061 7474 6572  ctivation Patter
-00000170: 6e73 222c 2022 4341 5073 222c 2022 6e65  ns", "CAPs", "ne
-00000180: 7572 6f69 6d61 6769 6e67 222c 2022 666d  uroimaging", "fm
-00000190: 7269 222c 2022 6466 6322 2c20 2264 796e  ri", "dfc", "dyn
-000001a0: 616d 6963 2066 756e 6374 696f 6e61 6c20  amic functional 
-000001b0: 636f 6e6e 6563 7469 7669 7479 222c 2022  connectivity", "
-000001c0: 664d 5249 5072 6570 225d 0d0a 636c 6173  fMRIPrep"]..clas
-000001d0: 7369 6669 6572 7320 3d20 5b0d 0a20 2020  sifiers = [..   
-000001e0: 2022 496e 7465 6e64 6564 2041 7564 6965   "Intended Audie
-000001f0: 6e63 6520 3a3a 2045 6475 6361 7469 6f6e  nce :: Education
-00000200: 222c 0d0a 2020 2020 2249 6e74 656e 6465  ",..    "Intende
-00000210: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
-00000220: 6965 6e63 652f 5265 7365 6172 6368 222c  ience/Research",
-00000230: 0d0a 2020 2020 2254 6f70 6963 203a 3a20  ..    "Topic :: 
-00000240: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
-00000250: 6565 7269 6e67 222c 0d0a 2020 2020 224c  eering",..    "L
-00000260: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-00000270: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-00000280: 6365 6e73 6522 2c0d 0a20 2020 2022 5072  cense",..    "Pr
-00000290: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000002a0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000002b0: 332e 3922 2c0d 0a20 2020 2022 5072 6f67  3.9",..    "Prog
-000002c0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000002d0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000002e0: 3130 222c 0d0a 2020 2020 2250 726f 6772  10",..    "Progr
-000002f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000300: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000310: 3122 2c0d 0a20 2020 2022 5072 6f67 7261  1",..    "Progra
-00000320: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000330: 3a20 5079 7468 6f6e 203a 3a20 332e 3132  : Python :: 3.12
-00000340: 222c 0d0a 2020 2020 224f 7065 7261 7469  ",..    "Operati
-00000350: 6e67 2053 7973 7465 6d20 3a3a 204d 6163  ng System :: Mac
-00000360: 4f53 203a 3a20 4d61 634f 5320 5822 2c0d  OS :: MacOS X",.
-00000370: 0a20 2020 2022 4f70 6572 6174 696e 6720  .    "Operating 
-00000380: 5379 7374 656d 203a 3a20 504f 5349 5820  System :: POSIX 
-00000390: 3a3a 204c 696e 7578 222c 0d0a 2020 2020  :: Linux",..    
-000003a0: 224f 7065 7261 7469 6e67 2053 7973 7465  "Operating Syste
-000003b0: 6d20 3a3a 204d 6963 726f 736f 6674 203a  m :: Microsoft :
-000003c0: 3a20 5769 6e64 6f77 7320 3a3a 2057 696e  : Windows :: Win
-000003d0: 646f 7773 2031 3122 2c0d 0a20 2020 2022  dows 11",..    "
-000003e0: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-000003f0: 7573 203a 3a20 3420 2d20 4265 7461 220d  us :: 4 - Beta".
-00000400: 0a5d 0d0a 6465 7065 6e64 656e 6369 6573  .]..dependencies
-00000410: 203d 205b 226e 756d 7079 222c 0d0a 2020   = ["numpy",..  
-00000420: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00000430: 616e 6461 7322 2c0d 0a20 2020 2020 2020  andas",..       
-00000440: 2020 2020 2020 2020 2022 6d61 7470 6c6f           "matplo
-00000450: 746c 6962 222c 0d0a 2020 2020 2020 2020  tlib",..        
-00000460: 2020 2020 2020 2020 2273 6561 626f 726e          "seaborn
-00000470: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000480: 2020 2020 226b 6e65 6564 222c 0d0a 2020      "kneed",..  
-00000490: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-000004a0: 6962 6162 656c 222c 0d0a 2020 2020 2020  ibabel",..      
-000004b0: 2020 2020 2020 2020 2020 226e 696c 6561            "nilea
-000004c0: 726e 3e3d 302e 3130 2e31 2c20 213d 302e  rn>=0.10.1, !=0.
-000004d0: 3130 2e33 222c 0d0a 2020 2020 2020 2020  10.3",..        
-000004e0: 2020 2020 2020 2020 2273 7572 6670 6c6f          "surfplo
-000004f0: 7422 2c0d 0a20 2020 2020 2020 2020 2020  t",..           
-00000500: 2020 2020 2022 6e65 7572 6f6d 6170 7322       "neuromaps"
-00000510: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000520: 2020 2022 7079 6269 6473 3b20 706c 6174     "pybids; plat
-00000530: 666f 726d 5f73 7973 7465 6d20 213d 2027  form_system != '
-00000540: 5769 6e64 6f77 7327 220d 0a20 2020 2020  Windows'"..     
-00000550: 2020 2020 2020 2020 2020 205d 0d0a 0d0a             ]....
-00000560: 5b70 726f 6a65 6374 2e75 726c 735d 0d0a  [project.urls]..
-00000570: 486f 6d65 7061 6765 203d 2022 6874 7470  Homepage = "http
-00000580: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
-00000590: 6f6e 6973 6861 6473 6d69 7468 2f6e 6575  onishadsmith/neu
-000005a0: 726f 6361 7073 2220 200d 0a0d 0a5b 746f  rocaps"  ....[to
-000005b0: 6f6c 2e64 6973 7475 7469 6c73 2e62 6469  ol.distutils.bdi
-000005c0: 7374 5f77 6865 656c 5d0d 0a75 6e69 7665  st_wheel]..unive
-000005d0: 7273 616c 203d 2074 7275 65              rsal = true
+00000080: 7273 696f 6e20 3d20 2230 2e39 2e33 2e70  rsion = "0.9.3.p
+00000090: 6f73 7431 220d 0a61 7574 686f 7273 203d  ost1"..authors =
+000000a0: 205b 7b6e 616d 6520 3d20 2244 6f6e 6973   [{name = "Donis
+000000b0: 6861 2053 6d69 7468 222c 2065 6d61 696c  ha Smith", email
+000000c0: 203d 2022 646f 6e69 7368 6173 6d69 7468   = "donishasmith
+000000d0: 406f 7574 6c6f 6f6b 2e63 6f6d 227d 5d0d  @outlook.com"}].
+000000e0: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
+000000f0: 436f 2d61 6374 6976 6174 696f 6e20 5061  Co-activation Pa
+00000100: 7474 6572 6e73 2028 4341 5073 2920 5079  tterns (CAPs) Py
+00000110: 7468 6f6e 2070 6163 6b61 6765 220d 0a72  thon package"..r
+00000120: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
+00000130: 6d64 220d 0a72 6571 7569 7265 732d 7079  md"..requires-py
+00000140: 7468 6f6e 203d 2022 3e3d 332e 392e 3022  thon = ">=3.9.0"
+00000150: 0d0a 6b65 7977 6f72 6473 203d 205b 2270  ..keywords = ["p
+00000160: 7974 686f 6e22 2c20 2243 6f2d 4163 7469  ython", "Co-Acti
+00000170: 7661 7469 6f6e 2050 6174 7465 726e 7322  vation Patterns"
+00000180: 2c20 2243 4150 7322 2c20 226e 6575 726f  , "CAPs", "neuro
+00000190: 696d 6167 696e 6722 2c20 2266 6d72 6922  imaging", "fmri"
+000001a0: 2c20 2264 6663 222c 2022 6479 6e61 6d69  , "dfc", "dynami
+000001b0: 6320 6675 6e63 7469 6f6e 616c 2063 6f6e  c functional con
+000001c0: 6e65 6374 6976 6974 7922 2c20 2266 4d52  nectivity", "fMR
+000001d0: 4950 7265 7022 5d0d 0a63 6c61 7373 6966  IPrep"]..classif
+000001e0: 6965 7273 203d 205b 0d0a 2020 2020 2249  iers = [..    "I
+000001f0: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000200: 203a 3a20 4564 7563 6174 696f 6e22 2c0d   :: Education",.
+00000210: 0a20 2020 2022 496e 7465 6e64 6564 2041  .    "Intended A
+00000220: 7564 6965 6e63 6520 3a3a 2053 6369 656e  udience :: Scien
+00000230: 6365 2f52 6573 6561 7263 6822 2c0d 0a20  ce/Research",.. 
+00000240: 2020 2022 546f 7069 6320 3a3a 2053 6369     "Topic :: Sci
+00000250: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
+00000260: 696e 6722 2c0d 0a20 2020 2022 4c69 6365  ing",..    "Lice
+00000270: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000280: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000290: 7365 222c 0d0a 2020 2020 2250 726f 6772  se",..    "Progr
+000002a0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000002b0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+000002c0: 222c 0d0a 2020 2020 2250 726f 6772 616d  ",..    "Program
+000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002e0: 2050 7974 686f 6e20 3a3a 2033 2e31 3022   Python :: 3.10"
+000002f0: 2c0d 0a20 2020 2022 5072 6f67 7261 6d6d  ,..    "Programm
+00000300: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000310: 5079 7468 6f6e 203a 3a20 332e 3131 222c  Python :: 3.11",
+00000320: 0d0a 2020 2020 2250 726f 6772 616d 6d69  ..    "Programmi
+00000330: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000340: 7974 686f 6e20 3a3a 2033 2e31 3222 2c0d  ython :: 3.12",.
+00000350: 0a20 2020 2022 4f70 6572 6174 696e 6720  .    "Operating 
+00000360: 5379 7374 656d 203a 3a20 4d61 634f 5320  System :: MacOS 
+00000370: 3a3a 204d 6163 4f53 2058 222c 0d0a 2020  :: MacOS X",..  
+00000380: 2020 224f 7065 7261 7469 6e67 2053 7973    "Operating Sys
+00000390: 7465 6d20 3a3a 2050 4f53 4958 203a 3a20  tem :: POSIX :: 
+000003a0: 4c69 6e75 7822 2c0d 0a20 2020 2022 4f70  Linux",..    "Op
+000003b0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+000003c0: 3a20 4d69 6372 6f73 6f66 7420 3a3a 2057  : Microsoft :: W
+000003d0: 696e 646f 7773 203a 3a20 5769 6e64 6f77  indows :: Window
+000003e0: 7320 3131 222c 0d0a 2020 2020 2244 6576  s 11",..    "Dev
+000003f0: 656c 6f70 6d65 6e74 2053 7461 7475 7320  elopment Status 
+00000400: 3a3a 2034 202d 2042 6574 6122 0d0a 5d0d  :: 4 - Beta"..].
+00000410: 0a64 6570 656e 6465 6e63 6965 7320 3d20  .dependencies = 
+00000420: 5b22 6e75 6d70 7922 2c0d 0a20 2020 2020  ["numpy",..     
+00000430: 2020 2020 2020 2020 2020 2022 7061 6e64             "pand
+00000440: 6173 222c 0d0a 2020 2020 2020 2020 2020  as",..          
+00000450: 2020 2020 2020 226d 6174 706c 6f74 6c69        "matplotli
+00000460: 6222 2c0d 0a20 2020 2020 2020 2020 2020  b",..           
+00000470: 2020 2020 2022 7365 6162 6f72 6e22 2c0d       "seaborn",.
+00000480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000490: 2022 6b6e 6565 6422 2c0d 0a20 2020 2020   "kneed",..     
+000004a0: 2020 2020 2020 2020 2020 2022 6e69 6261             "niba
+000004b0: 6265 6c22 2c0d 0a20 2020 2020 2020 2020  bel",..         
+000004c0: 2020 2020 2020 2022 6e69 6c65 6172 6e3e         "nilearn>
+000004d0: 3d30 2e31 302e 312c 2021 3d30 2e31 302e  =0.10.1, !=0.10.
+000004e0: 3322 2c0d 0a20 2020 2020 2020 2020 2020  3",..           
+000004f0: 2020 2020 2022 7375 7266 706c 6f74 222c       "surfplot",
+00000500: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000510: 2020 226e 6575 726f 6d61 7073 222c 0d0a    "neuromaps",..
+00000520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000530: 2270 7962 6964 733b 2070 6c61 7466 6f72  "pybids; platfor
+00000540: 6d5f 7379 7374 656d 2021 3d20 2757 696e  m_system != 'Win
+00000550: 646f 7773 2722 0d0a 2020 2020 2020 2020  dows'"..        
+00000560: 2020 2020 2020 2020 5d0d 0a0d 0a5b 7072          ]....[pr
+00000570: 6f6a 6563 742e 7572 6c73 5d0d 0a48 6f6d  oject.urls]..Hom
+00000580: 6570 6167 6520 3d20 2268 7474 7073 3a2f  epage = "https:/
+00000590: 2f67 6974 6875 622e 636f 6d2f 646f 6e69  /github.com/doni
+000005a0: 7368 6164 736d 6974 682f 6e65 7572 6f63  shadsmith/neuroc
+000005b0: 6170 7322 2020 0d0a 0d0a 5b74 6f6f 6c2e  aps"  ....[tool.
+000005c0: 6469 7374 7574 696c 732e 6264 6973 745f  distutils.bdist_
+000005d0: 7768 6565 6c5d 0d0a 756e 6976 6572 7361  wheel]..universa
+000005e0: 6c20 3d20 7472 7565                      l = true
```

### Comparing `neurocaps-0.9.3/tests/test_CAP.py` & `neurocaps-0.9.3.post1/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3/tests/test_TimeseriesExtractor.py` & `neurocaps-0.9.3.post1/tests/test_TimeseriesExtractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3/tests/test_TimeseriesExtractor_additional.py` & `neurocaps-0.9.3.post1/tests/test_TimeseriesExtractor_additional.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
     bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
 
     pipeline_name = "fmriprep_1.0.0/fmriprep"
     extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2)
     
     print(extractor.subject_timeseries, flush=True)
 
-    assert extractor.subject_timeseries["01"]["run-1"].shape[-1] == 100
-    assert extractor.subject_timeseries["01"]["run-1"].shape[0] == 40
+    assert extractor.subject_timeseries["01"]["run-0"].shape[-1] == 100
+    assert extractor.subject_timeseries["01"]["run-0"].shape[0] == 40
```

### Comparing `neurocaps-0.9.3/tests/test_merge_dicts.py` & `neurocaps-0.9.3.post1/tests/test_merge_dicts.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.3/tests/test_standardize.py` & `neurocaps-0.9.3.post1/tests/test_standardize.py`

 * *Files identical despite different names*

