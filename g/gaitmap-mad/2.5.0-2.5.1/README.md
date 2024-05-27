# Comparing `tmp/gaitmap_mad-2.5.0.tar.gz` & `tmp/gaitmap_mad-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitmap_mad-2.5.0.tar", max compression
+gzip compressed data, was "gaitmap_mad-2.5.1.tar", max compression
```

## Comparing `gaitmap_mad-2.5.0.tar` & `gaitmap_mad-2.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      734 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/LICENSE
--rw-r--r--   0        0        0      597 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/README.md
--rw-r--r--   0        0        0      482 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/__init__.py
--rw-r--r--   0        0        0      442 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/event_detection/__init__.py
--rw-r--r--   0        0        0     6009 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py
--rw-r--r--   0        0        0    14314 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/event_detection/_rampp_event_detection.py
--rw-r--r--   0        0        0      340 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/gait_detection/__init__.py
--rw-r--r--   0        0        0    24803 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py
--rw-r--r--   0        0        0      117 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/preprocessing/__init__.py
--rw-r--r--   0        0        0      234 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/preprocessing/sensor_alignment/__init__.py
--rw-r--r--   0        0        0    12668 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py
--rw-r--r--   0        0        0     1115 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/__init__.py
--rw-r--r--   0        0        0      814 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/__init__.py
--rw-r--r--   0        0        0    15231 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py
--rw-r--r--   0        0        0    36710 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py
--rw-r--r--   0        0        0     8812 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py
--rw-r--r--   0        0        0      436 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/__init__.py
--rw-r--r--   0        0        0     7513 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv
--rw-r--r--   0        0        0    16016 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py
--rw-r--r--   0        0        0     3563 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py
--rw-r--r--   0        0        0     1185 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/__init__.py
--rw-r--r--   0        0        0    11514 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py
--rw-r--r--   0        0        0    12637 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py
--rw-r--r--   0        0        0        0 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/__init__.py
--rw-r--r--   0        0        0   397824 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json
--rw-r--r--   0        0        0    27238 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py
--rw-r--r--   0        0        0    19115 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_simple_model.py
--rw-r--r--   0        0        0    26896 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_utils.py
--rw-r--r--   0        0        0      265 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/trajectory_reconstruction/__init__.py
--rw-r--r--   0        0        0      263 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/trajectory_reconstruction/position_methods/__init__.py
--rw-r--r--   0        0        0    10706 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py
--rw-r--r--   0        0        0      589 2024-05-23 14:22:53.681208 gaitmap_mad-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 gaitmap_mad-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0      734 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/LICENSE
+-rw-r--r--   0        0        0      597 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/README.md
+-rw-r--r--   0        0        0      482 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/gaitmap_mad/__init__.py
+-rw-r--r--   0        0        0      442 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/gaitmap_mad/event_detection/__init__.py
+-rw-r--r--   0        0        0     6009 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py
+-rw-r--r--   0        0        0    14314 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/gaitmap_mad/event_detection/_rampp_event_detection.py
+-rw-r--r--   0        0        0      340 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/gaitmap_mad/gait_detection/__init__.py
+-rw-r--r--   0        0        0    24803 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py
+-rw-r--r--   0        0        0      117 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/gaitmap_mad/preprocessing/__init__.py
+-rw-r--r--   0        0        0      234 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/gaitmap_mad/preprocessing/sensor_alignment/__init__.py
+-rw-r--r--   0        0        0    12668 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py
+-rw-r--r--   0        0        0     1115 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/__init__.py
+-rw-r--r--   0        0        0      814 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/__init__.py
+-rw-r--r--   0        0        0    15231 2024-05-27 12:56:42.379045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py
+-rw-r--r--   0        0        0    36710 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py
+-rw-r--r--   0        0        0     8812 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py
+-rw-r--r--   0        0        0      436 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/__init__.py
+-rw-r--r--   0        0        0     7513 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv
+-rw-r--r--   0        0        0    16016 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py
+-rw-r--r--   0        0        0     3563 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py
+-rw-r--r--   0        0        0     1185 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/__init__.py
+-rw-r--r--   0        0        0    11514 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py
+-rw-r--r--   0        0        0    12637 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/__init__.py
+-rw-r--r--   0        0        0   397824 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json
+-rw-r--r--   0        0        0    27238 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py
+-rw-r--r--   0        0        0    19115 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_simple_model.py
+-rw-r--r--   0        0        0    26896 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_utils.py
+-rw-r--r--   0        0        0      265 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/trajectory_reconstruction/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/trajectory_reconstruction/position_methods/__init__.py
+-rw-r--r--   0        0        0    10706 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py
+-rw-r--r--   0        0        0      589 2024-05-27 12:56:42.383045 gaitmap_mad-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 gaitmap_mad-2.5.1/PKG-INFO
```

### Comparing `gaitmap_mad-2.5.0/LICENSE` & `gaitmap_mad-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/README.md` & `gaitmap_mad-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py` & `gaitmap_mad-2.5.1/gaitmap_mad/event_detection/_filtered_rampp_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/event_detection/_rampp_event_detection.py` & `gaitmap_mad-2.5.1/gaitmap_mad/event_detection/_rampp_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py` & `gaitmap_mad-2.5.1/gaitmap_mad/gait_detection/_ullrich_gait_sequence_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py` & `gaitmap_mad-2.5.1/gaitmap_mad/preprocessing/sensor_alignment/_forward_direction_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/__init__.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/__init__.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_barth_dtw.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_base_dtw.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_constrained_barth_dtw.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/barth_original_template.csv`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_dtw_templates/templates.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/dtw/_vendored_tslearn.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/__init__.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_hmm_feature_transform.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_hmm_stride_segmentation.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_pre_trained_models/fallriskpd_at_lab_model.json`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_segmentation_model.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_simple_model.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_simple_model.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/stride_segmentation/hmm/_utils.py` & `gaitmap_mad-2.5.1/gaitmap_mad/stride_segmentation/hmm/_utils.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py` & `gaitmap_mad-2.5.1/gaitmap_mad/trajectory_reconstruction/position_methods/_piece_wise_linear_dedrifted_integration.py`

 * *Files identical despite different names*

### Comparing `gaitmap_mad-2.5.0/pyproject.toml` & `gaitmap_mad-2.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gaitmap_mad"
-version = "2.5.0"
+version = "2.5.1"
 description = "Specific algorithm implementaions by the mad_lab"
 license = "AGPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/gaitmap"
 repository = "https://github.com/mad-lab-fau/gaitmap"
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
```

### Comparing `gaitmap_mad-2.5.0/PKG-INFO` & `gaitmap_mad-2.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitmap_mad
-Version: 2.5.0
+Version: 2.5.1
 Summary: Specific algorithm implementaions by the mad_lab
 Home-page: https://github.com/mad-lab-fau/gaitmap
 License: AGPL-3.0
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

