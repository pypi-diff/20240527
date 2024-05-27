# Comparing `tmp/gaitmap-2.5.0.tar.gz` & `tmp/gaitmap-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaitmap-2.5.0.tar", max compression
+gzip compressed data, was "gaitmap-2.5.1.tar", max compression
```

## Comparing `gaitmap-2.5.0.tar` & `gaitmap-2.5.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     2032 2024-05-23 14:22:55.463001 gaitmap-2.5.0/LICENSE
--rw-r--r--   0        0        0    11674 2024-05-23 14:22:55.463001 gaitmap-2.5.0/README.md
--rw-r--r--   0        0        0       69 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/__init__.py
--rw-r--r--   0        0        0      164 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/_event_detection_common/__init__.py
--rw-r--r--   0        0        0     7495 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/_event_detection_common/_event_detection_mixin.py
--rw-r--r--   0        0        0    12515 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/base.py
--rw-r--r--   0        0        0     1317 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/data_transform/__init__.py
--rw-r--r--   0        0        0    15973 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/data_transform/_base.py
--rw-r--r--   0        0        0    12043 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/data_transform/_feature_transform.py
--rw-r--r--   0        0        0     3943 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/data_transform/_filter.py
--rw-r--r--   0        0        0    15601 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/data_transform/_scaler.py
--rw-r--r--   0        0        0      765 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/evaluation_utils/__init__.py
--rw-r--r--   0        0        0     6235 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/evaluation_utils/event_detection.py
--rw-r--r--   0        0        0    28906 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/evaluation_utils/parameter_errors.py
--rw-r--r--   0        0        0    11472 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/evaluation_utils/scores.py
--rw-r--r--   0        0        0    22318 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/evaluation_utils/stride_segmentation.py
--rw-r--r--   0        0        0      703 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/event_detection/__init__.py
--rw-r--r--   0        0        0    19365 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/event_detection/_herzer_event_detection.py
--rw-r--r--   0        0        0     8001 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/example_data.py
--rw-r--r--   0        0        0      543 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/gait_detection/__init__.py
--rw-r--r--   0        0        0      351 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/parameters/__init__.py
--rw-r--r--   0        0        0    22578 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/parameters/_spatial_parameters.py
--rw-r--r--   0        0        0     7833 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/parameters/_temporal_parameters.py
--rw-r--r--   0        0        0      288 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/preprocessing/__init__.py
--rw-r--r--   0        0        0      785 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/__init__.py
--rw-r--r--   0        0        0     5089 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py
--rw-r--r--   0        0        0     3940 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py
--rw-r--r--   0        0        0     6665 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py
--rw-r--r--   0        0        0     1732 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/stride_segmentation/__init__.py
--rw-r--r--   0        0        0    14886 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py
--rw-r--r--   0        0        0     2707 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/stride_segmentation/_utils.py
--rw-r--r--   0        0        0     1181 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/stride_segmentation/hmm.py
--rw-r--r--   0        0        0     1355 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/__init__.py
--rw-r--r--   0        0        0    21027 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py
--rw-r--r--   0        0        0     9356 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py
--rw-r--r--   0        0        0    10514 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py
--rw-r--r--   0        0        0      317 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/orientation_methods/__init__.py
--rw-r--r--   0        0        0     8223 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py
--rw-r--r--   0        0        0     4957 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py
--rw-r--r--   0        0        0      618 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py
--rw-r--r--   0        0        0     7849 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py
--rw-r--r--   0        0        0      243 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/trajectory_methods/__init__.py
--rw-r--r--   0        0        0    13674 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py
--rw-r--r--   0        0        0    16858 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py
--rw-r--r--   0        0        0       41 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/__init__.py
--rw-r--r--   0        0        0     1867 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/_algo_helper.py
--rw-r--r--   0        0        0     4609 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/_datatype_validation_helper.py
--rw-r--r--   0        0        0     1241 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/_gaitmap_mad.py
--rw-r--r--   0        0        0      409 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/_types.py
--rw-r--r--   0        0        0    18375 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/array_handling.py
--rw-r--r--   0        0        0     2556 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/consts.py
--rw-r--r--   0        0        0     6272 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/coordinate_conversion.py
--rw-r--r--   0        0        0    48470 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/datatype_helper.py
--rw-r--r--   0        0        0     1193 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/exceptions.py
--rw-r--r--   0        0        0     1866 2024-05-23 14:22:55.523000 gaitmap-2.5.0/gaitmap/utils/fast_quaternion_math.py
--rw-r--r--   0        0        0    18902 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/utils/rotations.py
--rw-r--r--   0        0        0     2367 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/utils/signal_processing.py
--rw-r--r--   0        0        0    14394 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/utils/static_moment_detection.py
--rw-r--r--   0        0        0     8481 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/utils/stride_list_conversion.py
--rw-r--r--   0        0        0     4124 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/utils/vector_math.py
--rw-r--r--   0        0        0      671 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/zupt_detection/__init__.py
--rw-r--r--   0        0        0     1582 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/zupt_detection/_base.py
--rw-r--r--   0        0        0     3063 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/zupt_detection/_combo_zupt_detector.py
--rw-r--r--   0        0        0    21982 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py
--rw-r--r--   0        0        0     4905 2024-05-23 14:22:55.527000 gaitmap-2.5.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py
--rw-r--r--   0        0        0     3589 2024-05-23 14:22:55.531000 gaitmap-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    13032 1970-01-01 00:00:00.000000 gaitmap-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2032 2024-05-27 12:56:42.712874 gaitmap-2.5.1/LICENSE
+-rw-r--r--   0        0        0    11674 2024-05-27 12:56:42.712874 gaitmap-2.5.1/README.md
+-rw-r--r--   0        0        0       69 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/_event_detection_common/__init__.py
+-rw-r--r--   0        0        0     7495 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/_event_detection_common/_event_detection_mixin.py
+-rw-r--r--   0        0        0    12515 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/base.py
+-rw-r--r--   0        0        0     1317 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/data_transform/__init__.py
+-rw-r--r--   0        0        0    15973 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/data_transform/_base.py
+-rw-r--r--   0        0        0    12043 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/data_transform/_feature_transform.py
+-rw-r--r--   0        0        0     3943 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/data_transform/_filter.py
+-rw-r--r--   0        0        0    15601 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/data_transform/_scaler.py
+-rw-r--r--   0        0        0      765 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/evaluation_utils/__init__.py
+-rw-r--r--   0        0        0     6235 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/evaluation_utils/event_detection.py
+-rw-r--r--   0        0        0    28938 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/evaluation_utils/parameter_errors.py
+-rw-r--r--   0        0        0    11472 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/evaluation_utils/scores.py
+-rw-r--r--   0        0        0    22638 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/evaluation_utils/stride_segmentation.py
+-rw-r--r--   0        0        0      703 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/event_detection/__init__.py
+-rw-r--r--   0        0        0    19365 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/event_detection/_herzer_event_detection.py
+-rw-r--r--   0        0        0     8001 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/example_data.py
+-rw-r--r--   0        0        0      543 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/gait_detection/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/parameters/__init__.py
+-rw-r--r--   0        0        0    22578 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/parameters/_spatial_parameters.py
+-rw-r--r--   0        0        0     7833 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/parameters/_temporal_parameters.py
+-rw-r--r--   0        0        0      288 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/preprocessing/__init__.py
+-rw-r--r--   0        0        0      785 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/preprocessing/sensor_alignment/__init__.py
+-rw-r--r--   0        0        0     5089 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py
+-rw-r--r--   0        0        0     3940 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py
+-rw-r--r--   0        0        0     7713 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py
+-rw-r--r--   0        0        0     1732 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/stride_segmentation/__init__.py
+-rw-r--r--   0        0        0    14886 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/stride_segmentation/_roi_stride_segmentation.py
+-rw-r--r--   0        0        0     2707 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/stride_segmentation/_utils.py
+-rw-r--r--   0        0        0     1181 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/stride_segmentation/hmm.py
+-rw-r--r--   0        0        0     1355 2024-05-27 12:56:42.768874 gaitmap-2.5.1/gaitmap/trajectory_reconstruction/__init__.py
+-rw-r--r--   0        0        0    21027 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/trajectory_reconstruction/_region_level_trajectory.py
+-rw-r--r--   0        0        0     9356 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py
+-rw-r--r--   0        0        0    10514 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py
+-rw-r--r--   0        0        0      317 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/trajectory_reconstruction/orientation_methods/__init__.py
+-rw-r--r--   0        0        0     8223 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py
+-rw-r--r--   0        0        0     4957 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py
+-rw-r--r--   0        0        0      618 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/trajectory_reconstruction/position_methods/__init__.py
+-rw-r--r--   0        0        0     7849 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py
+-rw-r--r--   0        0        0      243 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/trajectory_reconstruction/trajectory_methods/__init__.py
+-rw-r--r--   0        0        0    13674 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py
+-rw-r--r--   0        0        0    16858 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py
+-rw-r--r--   0        0        0       41 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/__init__.py
+-rw-r--r--   0        0        0     1867 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/_algo_helper.py
+-rw-r--r--   0        0        0     4609 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/_datatype_validation_helper.py
+-rw-r--r--   0        0        0     1241 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/_gaitmap_mad.py
+-rw-r--r--   0        0        0      409 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/_types.py
+-rw-r--r--   0        0        0    18375 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/array_handling.py
+-rw-r--r--   0        0        0     2556 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/consts.py
+-rw-r--r--   0        0        0     6272 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/coordinate_conversion.py
+-rw-r--r--   0        0        0    48470 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/datatype_helper.py
+-rw-r--r--   0        0        0     1193 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/exceptions.py
+-rw-r--r--   0        0        0     1866 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/fast_quaternion_math.py
+-rw-r--r--   0        0        0    18902 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/rotations.py
+-rw-r--r--   0        0        0     2367 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/signal_processing.py
+-rw-r--r--   0        0        0    14394 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/static_moment_detection.py
+-rw-r--r--   0        0        0     8481 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/stride_list_conversion.py
+-rw-r--r--   0        0        0     4124 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/utils/vector_math.py
+-rw-r--r--   0        0        0      671 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/zupt_detection/__init__.py
+-rw-r--r--   0        0        0     1582 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/zupt_detection/_base.py
+-rw-r--r--   0        0        0     3063 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/zupt_detection/_combo_zupt_detector.py
+-rw-r--r--   0        0        0    21982 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/zupt_detection/_moving_window_zupt_detector.py
+-rw-r--r--   0        0        0     4905 2024-05-27 12:56:42.772874 gaitmap-2.5.1/gaitmap/zupt_detection/_stride_event_zupt_detector.py
+-rw-r--r--   0        0        0     3589 2024-05-27 12:56:42.776874 gaitmap-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0    13032 1970-01-01 00:00:00.000000 gaitmap-2.5.1/PKG-INFO
```

### Comparing `gaitmap-2.5.0/LICENSE` & `gaitmap-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/README.md` & `gaitmap-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/_event_detection_common/_event_detection_mixin.py` & `gaitmap-2.5.1/gaitmap/_event_detection_common/_event_detection_mixin.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/base.py` & `gaitmap-2.5.1/gaitmap/base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/data_transform/__init__.py` & `gaitmap-2.5.1/gaitmap/data_transform/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/data_transform/_base.py` & `gaitmap-2.5.1/gaitmap/data_transform/_base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/data_transform/_feature_transform.py` & `gaitmap-2.5.1/gaitmap/data_transform/_feature_transform.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/data_transform/_filter.py` & `gaitmap-2.5.1/gaitmap/data_transform/_filter.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/data_transform/_scaler.py` & `gaitmap-2.5.1/gaitmap/data_transform/_scaler.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/evaluation_utils/__init__.py` & `gaitmap-2.5.1/gaitmap/evaluation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/evaluation_utils/event_detection.py` & `gaitmap-2.5.1/gaitmap/evaluation_utils/event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/evaluation_utils/parameter_errors.py` & `gaitmap-2.5.1/gaitmap/evaluation_utils/parameter_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,17 +241,17 @@
     error_loa_upper           6.198064  17.313018
     abs_error_loa_upper       5.030349  17.099293
     rel_error_loa_upper       1.773254   1.678502
     abs_rel_error_loa_upper   1.614135   2.439861
     icc                       0.256198   0.328814
     icc_q05                  -0.710000  -0.670000
     icc_q95                   0.920000   0.940000
-    n_common                  4.000000   4.000000
-    n_additional_reference    0.000000   0.000000
     n_additional_predicted    0.000000   0.000000
+    n_additional_reference    0.000000   0.000000
+    n_common                  4.000000   4.000000
 
     >>> pd.set_option("display.max_columns", None)
     >>> pd.set_option("display.width", 0)
     >>> predicted_sensor_left = pd.DataFrame(columns=["para"], data=[23, 82, 42]).rename_axis("s_id")
     >>> reference_sensor_left = pd.DataFrame(columns=["para"], data=[21, 86, 65]).rename_axis("s_id")
     >>> predicted_sensor_right = pd.DataFrame(columns=["para"], data=[26, -58, -3]).rename_axis("s_id")
     >>> reference_sensor_right = pd.DataFrame(columns=["para"], data=[96, -78, 86]).rename_axis("s_id")
@@ -482,15 +482,15 @@
             common = len(aligned.loc[:, pd.IndexSlice[:, para]].dropna(how="any"))
             max_common = max(common, max_common)
             common_rows_per_parameter[para] = {
                 "n_common": common,
                 "n_additional_reference": len(reference_parameter_correct[para].dropna()) - common,
                 "n_additional_predicted": len(predicted_parameter_correct[para].dropna()) - common,
             }
-        meta_error_dict[sensor] = pd.DataFrame(common_rows_per_parameter)
+        meta_error_dict[sensor] = pd.DataFrame(common_rows_per_parameter).sort_index()
 
         if max_common == 0:
             raise ValidationError(err_msg_start + "common entries are found between predicted and reference!")
 
         aligned_dict[sensor] = aligned
 
     return aligned_dict, meta_error_dict
@@ -563,15 +563,15 @@
         return None
 
     assert set(data.columns.get_level_values("error_type")) == {"predicted", "reference"}
     # If it is not unique, the ICC calculation will fail.
     assert data.index.is_unique
 
     paras = data.columns.get_level_values("parameter").unique()
-    data = data.stack("error_type").reset_index()
+    data = data.stack("error_type", future_stack=True).reset_index()
     coefs: dict[str, pd.Series] = {}
     for para in paras:
         try:
             # If handle error is ignore, we also ignore all warnings here.
             with warnings.catch_warnings():
                 if scoring_errors == "ignore":
                     warnings.simplefilter("ignore")
```

### Comparing `gaitmap-2.5.0/gaitmap/evaluation_utils/scores.py` & `gaitmap-2.5.1/gaitmap/evaluation_utils/scores.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/evaluation_utils/stride_segmentation.py` & `gaitmap-2.5.1/gaitmap/evaluation_utils/stride_segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,15 +478,24 @@
         return np.array([]), np.array([])
 
     right_tree = KDTree(list_right)
     left_tree = KDTree(list_left)
 
     if one_to_one is False:
         # p = np.inf is used to select the Chebyshev distance
-        keys = list(zip(*right_tree.sparse_distance_matrix(left_tree, tolerance, p=np.inf).keys()))
+        keys = list(
+            zip(
+                # We force sort the keys here to make sure the order is deterministic, even if the storage order of
+                # sparse array might not be.
+                *sorted(
+                    right_tree.sparse_distance_matrix(left_tree, tolerance, p=np.inf, output_type="dict").keys(),
+                    key=lambda x: x[1],
+                )
+            )
+        )
         # All values are returned that have a valid match
         return (np.array([]), np.array([])) if len(keys) == 0 else (np.array(keys[1]), np.array(keys[0]))
 
     # one_to_one is True
     # We calculate the closest neighbor based on the Manhatten distance in both directions and then find only the cases
     # were the right side closest neighbor resulted in the same pairing as the left side closest neighbor ensuring
     # that we have true one-to-one-matches and we have already the closest match based on our final criteria.
```

### Comparing `gaitmap-2.5.0/gaitmap/event_detection/__init__.py` & `gaitmap-2.5.1/gaitmap/event_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/event_detection/_herzer_event_detection.py` & `gaitmap-2.5.1/gaitmap/event_detection/_herzer_event_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/example_data.py` & `gaitmap-2.5.1/gaitmap/example_data.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/gait_detection/__init__.py` & `gaitmap-2.5.1/gaitmap/gait_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/parameters/_spatial_parameters.py` & `gaitmap-2.5.1/gaitmap/parameters/_spatial_parameters.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/parameters/_temporal_parameters.py` & `gaitmap-2.5.1/gaitmap/parameters/_temporal_parameters.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/__init__.py` & `gaitmap-2.5.1/gaitmap/preprocessing/sensor_alignment/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py` & `gaitmap-2.5.1/gaitmap/preprocessing/sensor_alignment/_gravity_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py` & `gaitmap-2.5.1/gaitmap/preprocessing/sensor_alignment/_mulisensor_alignment.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py` & `gaitmap-2.5.1/gaitmap/preprocessing/sensor_alignment/_pca_alignment.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing_extensions import Self
 
 from gaitmap.base import BaseSensorAlignment
 from gaitmap.utils._algo_helper import invert_result_dictionary, set_params_from_dict
 from gaitmap.utils._types import _Hashable
 from gaitmap.utils.consts import SF_ACC, SF_GYR
 from gaitmap.utils.datatype_helper import SensorData, get_multi_sensor_names, is_sensor_data
-from gaitmap.utils.rotations import rotate_dataset
+from gaitmap.utils.rotations import find_signed_3d_angle, rotate_dataset
 
 # TODO: Move `right_handed_cord` to general utils package
 
 
 def right_handed_cord(x: Optional[np.ndarray], y: Optional[np.ndarray], z: Optional[np.ndarray]) -> np.ndarray:
     """Create right handed coordinate system, with two axis provided."""
     if x is None:
@@ -39,34 +39,45 @@
         raise ValueError('Invalid axis for pca plane! Valid axis would be e.g. ("gyr_x", "gyr_y").')
 
     # find dominant movement axis by PCA only search in 2D plane assuming that the dataset is already roughly aligned in
     # the third direction
     pca = PCA(n_components=2)
     pca = pca.fit(dataset[pca_plane_axis])
 
+    pca_components = pca.components_.copy()
+    # To follow the coordinate system convention, we ensure that the second component is positive 90 deg rotation from
+    # the first component
+    angle = np.rad2deg(find_signed_3d_angle(pca_components[1], pca_components[0], [0, 0, 1]))
+    if angle < 0:
+        pca_components[1] *= -1
+    # To make the output of this alignment deteministic, we always ensure that the first component is positive
+    if pca_components[0, 0] < 0:
+        pca_components *= -1
+
     # define new coordinate system
     # target axis will correspond to the pca component with highest explained_variance_
-    pca_main_component_axis = np.array([pca.components_[0][0], pca.components_[0][1], 0])
+    pca_main_component_axis = np.array([pca_components[0, 0], pca_components[0, 1], 0])
 
     target_axis_helper = {"x": None, "y": None}
 
     if target_axis.lower() not in target_axis_helper:
-        raise ValueError(f"Invalid target aixs! Axis must be one of {target_axis_helper.keys()}")
+        raise ValueError(f"Invalid target axis! Axis must be one of {target_axis_helper.keys()}")
 
     target_axis_helper[target_axis.lower()] = pca_main_component_axis
 
     rotation_matrix = right_handed_cord(**target_axis_helper, z=np.array([0, 0, 1]))
 
     r = Rotation.from_matrix(rotation_matrix)
 
     # apply rotation to dataset
     return {
         "aligned_data": rotate_dataset(dataset, r),
         "rotation": r,
         "pca": pca,
+        "normalized_pca_components": pca_components,
     }
 
 
 class PcaAlignment(BaseSensorAlignment):
     """Align dataset target axis, to the main foot rotation plane, which is usually the medio-lateral plane.
 
     The Principle Component Analysis (PCA) can be used to determin the coordinate plane where the main movement
@@ -90,14 +101,19 @@
     ----------
     aligned_data_
         The rotated sensor data after alignment
     rotation_
         The :class:`~scipy.spatial.transform.Rotation` object tranforming the original data to the aligned data
     pca_
         :class:`~sklearn.decomposition.PCA` object after fitting
+    normalized_pca_components_
+        These are the PCA componts, but aligned to the coordinate system convention.
+        I.e. the first component is always positive and the second component is positive 90 deg rotation from the first
+        (i.e. they form a right handed coordinate system).
+        These normalized components can be used to estimate the rotation of the sensor frame.
 
     Other Parameters
     ----------------
     data
         The data passed to the `align` method.
 
 
@@ -128,14 +144,15 @@
     gaitmap.preprocessing.sensor_alignment.ForwardDirectionSignAlignment: Alignment of the forward direction after
                                                                           PCA Alignment
 
     """
 
     rotation_: Union[Rotation, dict[_Hashable, Rotation]]
     pca_: Union[PCA, dict[_Hashable, PCA]]
+    normalized_pca_components_: Union[np.ndarray, dict[_Hashable, np.ndarray]]
 
     target_axis: str
     pca_plane_axis: Sequence[str]
 
     data: SensorData
 
     def __init__(self, target_axis: str = "y", pca_plane_axis: Sequence[str] = ("gyr_x", "gyr_y")) -> None:
```

### Comparing `gaitmap-2.5.0/gaitmap/stride_segmentation/__init__.py` & `gaitmap-2.5.1/gaitmap/stride_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/stride_segmentation/_roi_stride_segmentation.py` & `gaitmap-2.5.1/gaitmap/stride_segmentation/_roi_stride_segmentation.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/stride_segmentation/_utils.py` & `gaitmap-2.5.1/gaitmap/stride_segmentation/_utils.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/stride_segmentation/hmm.py` & `gaitmap-2.5.1/gaitmap/stride_segmentation/hmm.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/__init__.py` & `gaitmap-2.5.1/gaitmap/trajectory_reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/_region_level_trajectory.py` & `gaitmap-2.5.1/gaitmap/trajectory_reconstruction/_region_level_trajectory.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py` & `gaitmap-2.5.1/gaitmap/trajectory_reconstruction/_stride_level_trajectory.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py` & `gaitmap-2.5.1/gaitmap/trajectory_reconstruction/_trajectory_wrapper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py` & `gaitmap-2.5.1/gaitmap/trajectory_reconstruction/orientation_methods/_madgwick.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py` & `gaitmap-2.5.1/gaitmap/trajectory_reconstruction/orientation_methods/_simple_gyro_integration.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/position_methods/__init__.py` & `gaitmap-2.5.1/gaitmap/trajectory_reconstruction/position_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py` & `gaitmap-2.5.1/gaitmap/trajectory_reconstruction/position_methods/_forward_backwards_integration.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py` & `gaitmap-2.5.1/gaitmap/trajectory_reconstruction/trajectory_methods/_kalman_numba_funcs.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py` & `gaitmap-2.5.1/gaitmap/trajectory_reconstruction/trajectory_methods/_rts_kalman.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/_algo_helper.py` & `gaitmap-2.5.1/gaitmap/utils/_algo_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/_datatype_validation_helper.py` & `gaitmap-2.5.1/gaitmap/utils/_datatype_validation_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/_gaitmap_mad.py` & `gaitmap-2.5.1/gaitmap/utils/_gaitmap_mad.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/array_handling.py` & `gaitmap-2.5.1/gaitmap/utils/array_handling.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/consts.py` & `gaitmap-2.5.1/gaitmap/utils/consts.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/coordinate_conversion.py` & `gaitmap-2.5.1/gaitmap/utils/coordinate_conversion.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/datatype_helper.py` & `gaitmap-2.5.1/gaitmap/utils/datatype_helper.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/exceptions.py` & `gaitmap-2.5.1/gaitmap/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/fast_quaternion_math.py` & `gaitmap-2.5.1/gaitmap/utils/fast_quaternion_math.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/rotations.py` & `gaitmap-2.5.1/gaitmap/utils/rotations.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/signal_processing.py` & `gaitmap-2.5.1/gaitmap/utils/signal_processing.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/static_moment_detection.py` & `gaitmap-2.5.1/gaitmap/utils/static_moment_detection.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/stride_list_conversion.py` & `gaitmap-2.5.1/gaitmap/utils/stride_list_conversion.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/utils/vector_math.py` & `gaitmap-2.5.1/gaitmap/utils/vector_math.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/zupt_detection/__init__.py` & `gaitmap-2.5.1/gaitmap/zupt_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/zupt_detection/_base.py` & `gaitmap-2.5.1/gaitmap/zupt_detection/_base.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/zupt_detection/_combo_zupt_detector.py` & `gaitmap-2.5.1/gaitmap/zupt_detection/_combo_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/zupt_detection/_moving_window_zupt_detector.py` & `gaitmap-2.5.1/gaitmap/zupt_detection/_moving_window_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/gaitmap/zupt_detection/_stride_event_zupt_detector.py` & `gaitmap-2.5.1/gaitmap/zupt_detection/_stride_event_zupt_detector.py`

 * *Files identical despite different names*

### Comparing `gaitmap-2.5.0/pyproject.toml` & `gaitmap-2.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gaitmap"
-version = "2.5.0"
+version = "2.5.1"
 description = "The Gait and Movement Analysis Package - Your definite guide to reliable IMU based human movement analysis."
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mad-lab-fau/gaitmap"
 repository = "https://github.com/mad-lab-fau/gaitmap"
 authors = [
     "Arne Küderle <arne.kuederle@fau.de>",
```

### Comparing `gaitmap-2.5.0/PKG-INFO` & `gaitmap-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaitmap
-Version: 2.5.0
+Version: 2.5.1
 Summary: The Gait and Movement Analysis Package - Your definite guide to reliable IMU based human movement analysis.
 Home-page: https://github.com/mad-lab-fau/gaitmap
 License: MIT
 Author: Arne Küderle
 Author-email: arne.kuederle@fau.de
 Requires-Python: >=3.9.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

