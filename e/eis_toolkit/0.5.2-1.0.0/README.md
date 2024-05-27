# Comparing `tmp/eis_toolkit-0.5.2.tar.gz` & `tmp/eis_toolkit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis_toolkit-0.5.2.tar", max compression
+gzip compressed data, was "eis_toolkit-1.0.0.tar", max compression
```

## Comparing `eis_toolkit-0.5.2.tar` & `eis_toolkit-1.0.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rwxr-xr-x   0        0        0    13827 2024-03-04 07:36:07.783856 eis_toolkit-0.5.2/LICENSE
--rwxr-xr-x   0        0        0     5864 2024-05-13 10:15:39.840704 eis_toolkit-0.5.2/README.md
--rwxr-xr-x   0        0        0       22 2024-02-12 07:36:47.840362 eis_toolkit-0.5.2/eis_toolkit/__init__.py
--rw-r--r--   0        0        0       70 2024-04-04 09:16:19.591131 eis_toolkit-0.5.2/eis_toolkit/__main__.py
--rw-r--r--   0        0        0   116811 2024-05-24 11:29:42.222707 eis_toolkit-0.5.2/eis_toolkit/cli.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/conversions/__init__.py
--rw-r--r--   0        0        0     3840 2024-02-22 09:12:29.156927 eis_toolkit-0.5.2/eis_toolkit/conversions/csv_to_geodataframe.py
--rw-r--r--   0        0        0     2691 2024-04-24 11:26:52.059104 eis_toolkit-0.5.2/eis_toolkit/conversions/raster_to_dataframe.py
--rwxr-xr-x   0        0        0        0 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/__init__.py
--rw-r--r--   0        0        0     4577 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/calculate_base_metrics.py
--rw-r--r--   0        0        0     1233 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/classification_label_evaluation.py
--rw-r--r--   0        0        0     7051 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/classification_probability_evaluation.py
--rw-r--r--   0        0        0     2153 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_confusion_matrix.py
--rw-r--r--   0        0        0     2644 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_nn_model_performance.py
--rw-r--r--   0        0        0     3829 2024-04-25 10:25:47.561371 eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_prediction_area_curves.py
--rw-r--r--   0        0        0     2003 2024-04-25 10:25:47.565371 eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_rate_curve.py
--rw-r--r--   0        0        0     2587 2024-04-25 10:25:47.565371 eis_toolkit-0.5.2/eis_toolkit/evaluation/scoring.py
--rw-r--r--   0        0        0     2739 2024-05-21 06:37:53.189336 eis_toolkit-0.5.2/eis_toolkit/exceptions.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/__init__.py
--rw-r--r--   0        0        0      286 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/basic_plots_seaborn.py
--rw-r--r--   0        0        0     2302 2024-03-06 08:47:28.563567 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/chi_square_test.py
--rw-r--r--   0        0        0     4015 2024-04-15 11:24:32.422063 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/correlation_matrix.py
--rw-r--r--   0        0        0     2416 2024-03-06 08:47:28.563567 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/covariance_matrix.py
--rw-r--r--   0        0        0     6937 2024-04-15 11:24:32.422063 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/dbscan.py
--rw-r--r--   0        0        0     2627 2024-04-02 08:33:51.299185 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/descriptive_statistics.py
--rw-r--r--   0        0        0     2030 2024-03-04 09:08:14.566054 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/feature_importance.py
--rw-r--r--   0        0        0     6361 2024-04-15 11:24:32.422063 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/k_means_cluster.py
--rw-r--r--   0        0        0     2602 2024-03-04 07:36:07.783856 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/local_morans_i.py
--rw-r--r--   0        0        0     4981 2024-03-06 08:47:28.563567 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/normality_test.py
--rw-r--r--   0        0        0     7540 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/parallel_coordinates.py
--rw-r--r--   0        0        0    11017 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/pca.py
--rw-r--r--   0        0        0      445 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/plot_utils.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/prediction/__init__.py
--rw-r--r--   0        0        0     5350 2024-04-30 08:53:14.418579 eis_toolkit-0.5.2/eis_toolkit/prediction/fuzzy_overlay.py
--rw-r--r--   0        0        0    10930 2024-03-12 10:30:37.976282 eis_toolkit-0.5.2/eis_toolkit/prediction/gradient_boosting.py
--rw-r--r--   0        0        0     4424 2024-03-12 10:30:37.976282 eis_toolkit-0.5.2/eis_toolkit/prediction/logistic_regression.py
--rw-r--r--   0        0        0    16273 2024-05-20 10:32:28.957217 eis_toolkit-0.5.2/eis_toolkit/prediction/machine_learning_general.py
--rw-r--r--   0        0        0     3251 2024-05-21 08:40:59.424283 eis_toolkit-0.5.2/eis_toolkit/prediction/machine_learning_predict.py
--rw-r--r--   0        0        0    13658 2024-03-12 10:30:37.976282 eis_toolkit-0.5.2/eis_toolkit/prediction/mlp.py
--rw-r--r--   0        0        0     8686 2024-04-03 07:14:14.999244 eis_toolkit-0.5.2/eis_toolkit/prediction/random_forests.py
--rw-r--r--   0        0        0    17390 2024-04-24 15:28:57.740112 eis_toolkit-0.5.2/eis_toolkit/prediction/weights_of_evidence.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/raster_processing/__init__.py
--rwxr-xr-x   0        0        0     2042 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/clipping.py
--rw-r--r--   0        0        0     6940 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/create_constant_raster.py
--rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/__init__.py
--rw-r--r--   0        0        0     4355 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/classification.py
--rw-r--r--   0        0        0     9871 2024-04-03 09:12:33.201055 eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/parameters.py
--rw-r--r--   0        0        0     6922 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/partial_derivatives.py
--rw-r--r--   0        0        0     1435 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/utilities.py
--rw-r--r--   0        0        0    10388 2024-04-29 09:13:31.923148 eis_toolkit-0.5.2/eis_toolkit/raster_processing/distance_to_anomaly.py
--rw-r--r--   0        0        0     2931 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/extract_values_from_raster.py
--rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/__init__.py
--rw-r--r--   0        0        0     5820 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/focal.py
--rw-r--r--   0        0        0     3521 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/kernels.py
--rw-r--r--   0        0        0    17984 2024-03-06 08:46:24.150688 eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/speckle.py
--rw-r--r--   0        0        0     3656 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/utilities.py
--rw-r--r--   0        0        0    15084 2024-03-04 07:36:07.787855 eis_toolkit-0.5.2/eis_toolkit/raster_processing/reclassify.py
--rw-r--r--   0        0        0     2573 2024-04-03 09:32:00.769041 eis_toolkit-0.5.2/eis_toolkit/raster_processing/reprojecting.py
--rw-r--r--   0        0        0     2745 2024-04-03 09:32:00.769041 eis_toolkit-0.5.2/eis_toolkit/raster_processing/resampling.py
--rw-r--r--   0        0        0     4343 2024-04-03 09:01:39.672155 eis_toolkit-0.5.2/eis_toolkit/raster_processing/snapping.py
--rw-r--r--   0        0        0     4834 2024-04-03 09:32:00.769041 eis_toolkit-0.5.2/eis_toolkit/raster_processing/unifying.py
--rw-r--r--   0        0        0     2050 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/raster_processing/unique_combinations.py
--rw-r--r--   0        0        0     3390 2023-11-10 08:05:31.345266 eis_toolkit-0.5.2/eis_toolkit/raster_processing/windowing.py
--rw-r--r--   0        0        0        0 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/training_data_tools/__init__.py
--rw-r--r--   0        0        0     1840 2024-02-22 09:12:29.160927 eis_toolkit-0.5.2/eis_toolkit/training_data_tools/class_balancing.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/transformations/__init__.py
--rw-r--r--   0        0        0     3639 2024-04-08 06:45:40.454759 eis_toolkit-0.5.2/eis_toolkit/transformations/binarize.py
--rw-r--r--   0        0        0     4696 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/clip.py
--rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/transformations/coda/__init__.py
--rw-r--r--   0        0        0     3054 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/coda/alr.py
--rw-r--r--   0        0        0     2338 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/coda/clr.py
--rw-r--r--   0        0        0     3628 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/coda/ilr.py
--rw-r--r--   0        0        0     2504 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/coda/pairwise.py
--rw-r--r--   0        0        0     4136 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/coda/plr.py
--rw-r--r--   0        0        0     7699 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/linear.py
--rw-r--r--   0        0        0     4883 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/logarithmic.py
--rw-r--r--   0        0        0     5205 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/one_hot_encoding.py
--rw-r--r--   0        0        0     5163 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/transformations/sigmoid.py
--rw-r--r--   0        0        0     6767 2024-04-08 08:42:37.268163 eis_toolkit-0.5.2/eis_toolkit/transformations/winsorize.py
--rw-r--r--   0        0        0        0 2023-12-06 09:22:12.535287 eis_toolkit-0.5.2/eis_toolkit/utilities/__init__.py
--rw-r--r--   0        0        0     1107 2024-04-05 07:27:18.360688 eis_toolkit-0.5.2/eis_toolkit/utilities/aitchison_geometry.py
--rwxr-xr-x   0        0        0        0 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/utilities/checks/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-05 07:27:18.360688 eis_toolkit-0.5.2/eis_toolkit/utilities/checks/compositional.py
--rw-r--r--   0        0        0     1672 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/utilities/checks/dataframe.py
--rwxr-xr-x   0        0        0      599 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/utilities/checks/geometry.py
--rw-r--r--   0        0        0     2353 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/utilities/checks/parameter.py
--rw-r--r--   0        0        0     5837 2024-04-03 09:32:00.769041 eis_toolkit-0.5.2/eis_toolkit/utilities/checks/raster.py
--rw-r--r--   0        0        0     1467 2024-02-22 09:12:29.164927 eis_toolkit-0.5.2/eis_toolkit/utilities/conversions.py
--rw-r--r--   0        0        0     8640 2024-05-03 06:58:41.674662 eis_toolkit-0.5.2/eis_toolkit/utilities/file_io.py
--rw-r--r--   0        0        0    12203 2024-04-24 06:18:14.118407 eis_toolkit-0.5.2/eis_toolkit/utilities/miscellaneous.py
--rw-r--r--   0        0        0     4947 2024-04-24 06:18:14.118407 eis_toolkit-0.5.2/eis_toolkit/utilities/nodata.py
--rw-r--r--   0        0        0     6041 2024-04-24 11:26:53.983156 eis_toolkit-0.5.2/eis_toolkit/utilities/raster.py
--rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-0.5.2/eis_toolkit/vector_processing/__init__.py
--rw-r--r--   0        0        0     1098 2024-02-22 09:12:29.168927 eis_toolkit-0.5.2/eis_toolkit/vector_processing/calculate_geometry.py
--rw-r--r--   0        0        0    22761 2024-05-24 06:00:52.148295 eis_toolkit-0.5.2/eis_toolkit/vector_processing/cell_based_association.py
--rw-r--r--   0        0        0     3240 2024-05-02 10:42:43.425579 eis_toolkit-0.5.2/eis_toolkit/vector_processing/distance_computation.py
--rw-r--r--   0        0        0     1942 2024-02-22 09:12:29.168927 eis_toolkit-0.5.2/eis_toolkit/vector_processing/extract_shared_lines.py
--rw-r--r--   0        0        0     3747 2024-04-25 15:11:32.909910 eis_toolkit-0.5.2/eis_toolkit/vector_processing/idw_interpolation.py
--rw-r--r--   0        0        0     4092 2024-04-24 11:26:53.983156 eis_toolkit-0.5.2/eis_toolkit/vector_processing/kriging_interpolation.py
--rw-r--r--   0        0        0     4827 2024-04-24 14:32:11.183266 eis_toolkit-0.5.2/eis_toolkit/vector_processing/rasterize_vector.py
--rw-r--r--   0        0        0      703 2023-11-10 08:05:31.345266 eis_toolkit-0.5.2/eis_toolkit/vector_processing/reproject_vector.py
--rw-r--r--   0        0        0     1523 2024-04-24 14:32:41.807458 eis_toolkit-0.5.2/eis_toolkit/vector_processing/vector_density.py
--rwxr-xr-x   0        0        0     1778 2024-05-24 11:29:42.222707 eis_toolkit-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 eis_toolkit-0.5.2/PKG-INFO
+-rwxr-xr-x   0        0        0    13827 2024-03-04 07:36:07.783856 eis_toolkit-1.0.0/LICENSE
+-rwxr-xr-x   0        0        0     5883 2024-05-27 13:52:56.128989 eis_toolkit-1.0.0/README.md
+-rwxr-xr-x   0        0        0       22 2024-02-12 07:36:47.840362 eis_toolkit-1.0.0/eis_toolkit/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-04 09:16:19.591131 eis_toolkit-1.0.0/eis_toolkit/__main__.py
+-rw-r--r--   0        0        0   116570 2024-05-27 13:52:54.040969 eis_toolkit-1.0.0/eis_toolkit/cli.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-1.0.0/eis_toolkit/conversions/__init__.py
+-rw-r--r--   0        0        0     3840 2024-02-22 09:12:29.156927 eis_toolkit-1.0.0/eis_toolkit/conversions/csv_to_geodataframe.py
+-rw-r--r--   0        0        0     2691 2024-04-24 11:26:52.059104 eis_toolkit-1.0.0/eis_toolkit/conversions/raster_to_dataframe.py
+-rwxr-xr-x   0        0        0        0 2024-04-25 10:25:47.561371 eis_toolkit-1.0.0/eis_toolkit/evaluation/__init__.py
+-rw-r--r--   0        0        0     4577 2024-04-25 10:25:47.561371 eis_toolkit-1.0.0/eis_toolkit/evaluation/calculate_base_metrics.py
+-rw-r--r--   0        0        0     1233 2024-04-25 10:25:47.561371 eis_toolkit-1.0.0/eis_toolkit/evaluation/classification_label_evaluation.py
+-rw-r--r--   0        0        0     7051 2024-04-25 10:25:47.561371 eis_toolkit-1.0.0/eis_toolkit/evaluation/classification_probability_evaluation.py
+-rw-r--r--   0        0        0     2153 2024-04-25 10:25:47.561371 eis_toolkit-1.0.0/eis_toolkit/evaluation/plot_confusion_matrix.py
+-rw-r--r--   0        0        0     2644 2024-04-25 10:25:47.561371 eis_toolkit-1.0.0/eis_toolkit/evaluation/plot_nn_model_performance.py
+-rw-r--r--   0        0        0     3829 2024-04-25 10:25:47.561371 eis_toolkit-1.0.0/eis_toolkit/evaluation/plot_prediction_area_curves.py
+-rw-r--r--   0        0        0     2003 2024-04-25 10:25:47.565371 eis_toolkit-1.0.0/eis_toolkit/evaluation/plot_rate_curve.py
+-rw-r--r--   0        0        0     2587 2024-04-25 10:25:47.565371 eis_toolkit-1.0.0/eis_toolkit/evaluation/scoring.py
+-rw-r--r--   0        0        0     2739 2024-05-21 06:37:53.189336 eis_toolkit-1.0.0/eis_toolkit/exceptions.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/__init__.py
+-rw-r--r--   0        0        0      286 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/basic_plots_seaborn.py
+-rw-r--r--   0        0        0     2302 2024-03-06 08:47:28.563567 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/chi_square_test.py
+-rw-r--r--   0        0        0     4015 2024-04-15 11:24:32.422063 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/correlation_matrix.py
+-rw-r--r--   0        0        0     2416 2024-03-06 08:47:28.563567 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/covariance_matrix.py
+-rw-r--r--   0        0        0     6937 2024-04-15 11:24:32.422063 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/dbscan.py
+-rw-r--r--   0        0        0     2627 2024-04-02 08:33:51.299185 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/descriptive_statistics.py
+-rw-r--r--   0        0        0     2030 2024-03-04 09:08:14.566054 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/feature_importance.py
+-rw-r--r--   0        0        0     6361 2024-04-15 11:24:32.422063 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/k_means_cluster.py
+-rw-r--r--   0        0        0     2602 2024-03-04 07:36:07.783856 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/local_morans_i.py
+-rw-r--r--   0        0        0     4981 2024-03-06 08:47:28.563567 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/normality_test.py
+-rw-r--r--   0        0        0     7540 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/parallel_coordinates.py
+-rw-r--r--   0        0        0    11017 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/pca.py
+-rw-r--r--   0        0        0      445 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/plot_utils.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-1.0.0/eis_toolkit/prediction/__init__.py
+-rw-r--r--   0        0        0     5350 2024-04-30 08:53:14.418579 eis_toolkit-1.0.0/eis_toolkit/prediction/fuzzy_overlay.py
+-rw-r--r--   0        0        0    10930 2024-03-12 10:30:37.976282 eis_toolkit-1.0.0/eis_toolkit/prediction/gradient_boosting.py
+-rw-r--r--   0        0        0     4424 2024-03-12 10:30:37.976282 eis_toolkit-1.0.0/eis_toolkit/prediction/logistic_regression.py
+-rw-r--r--   0        0        0    16273 2024-05-20 10:32:28.957217 eis_toolkit-1.0.0/eis_toolkit/prediction/machine_learning_general.py
+-rw-r--r--   0        0        0     3251 2024-05-21 08:40:59.424283 eis_toolkit-1.0.0/eis_toolkit/prediction/machine_learning_predict.py
+-rw-r--r--   0        0        0    13658 2024-03-12 10:30:37.976282 eis_toolkit-1.0.0/eis_toolkit/prediction/mlp.py
+-rw-r--r--   0        0        0     8686 2024-04-03 07:14:14.999244 eis_toolkit-1.0.0/eis_toolkit/prediction/random_forests.py
+-rw-r--r--   0        0        0    17390 2024-04-24 15:28:57.740112 eis_toolkit-1.0.0/eis_toolkit/prediction/weights_of_evidence.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-1.0.0/eis_toolkit/raster_processing/__init__.py
+-rwxr-xr-x   0        0        0     2042 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/raster_processing/clipping.py
+-rw-r--r--   0        0        0     6940 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/raster_processing/create_constant_raster.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-1.0.0/eis_toolkit/raster_processing/derivatives/__init__.py
+-rw-r--r--   0        0        0     4355 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/raster_processing/derivatives/classification.py
+-rw-r--r--   0        0        0     9871 2024-04-03 09:12:33.201055 eis_toolkit-1.0.0/eis_toolkit/raster_processing/derivatives/parameters.py
+-rw-r--r--   0        0        0     6922 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/raster_processing/derivatives/partial_derivatives.py
+-rw-r--r--   0        0        0     1435 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/raster_processing/derivatives/utilities.py
+-rw-r--r--   0        0        0    10388 2024-04-29 09:13:31.923148 eis_toolkit-1.0.0/eis_toolkit/raster_processing/distance_to_anomaly.py
+-rw-r--r--   0        0        0     2931 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/raster_processing/extract_values_from_raster.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-1.0.0/eis_toolkit/raster_processing/filters/__init__.py
+-rw-r--r--   0        0        0     5820 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/raster_processing/filters/focal.py
+-rw-r--r--   0        0        0     3521 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/raster_processing/filters/kernels.py
+-rw-r--r--   0        0        0    17984 2024-03-06 08:46:24.150688 eis_toolkit-1.0.0/eis_toolkit/raster_processing/filters/speckle.py
+-rw-r--r--   0        0        0     3656 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/raster_processing/filters/utilities.py
+-rw-r--r--   0        0        0    15084 2024-03-04 07:36:07.787855 eis_toolkit-1.0.0/eis_toolkit/raster_processing/reclassify.py
+-rw-r--r--   0        0        0     2573 2024-04-03 09:32:00.769041 eis_toolkit-1.0.0/eis_toolkit/raster_processing/reprojecting.py
+-rw-r--r--   0        0        0     2745 2024-04-03 09:32:00.769041 eis_toolkit-1.0.0/eis_toolkit/raster_processing/resampling.py
+-rw-r--r--   0        0        0     4343 2024-04-03 09:01:39.672155 eis_toolkit-1.0.0/eis_toolkit/raster_processing/snapping.py
+-rw-r--r--   0        0        0     4834 2024-04-03 09:32:00.769041 eis_toolkit-1.0.0/eis_toolkit/raster_processing/unifying.py
+-rw-r--r--   0        0        0     2050 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/raster_processing/unique_combinations.py
+-rw-r--r--   0        0        0     3390 2023-11-10 08:05:31.345266 eis_toolkit-1.0.0/eis_toolkit/raster_processing/windowing.py
+-rw-r--r--   0        0        0        0 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/training_data_tools/__init__.py
+-rw-r--r--   0        0        0     1840 2024-02-22 09:12:29.160927 eis_toolkit-1.0.0/eis_toolkit/training_data_tools/class_balancing.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-1.0.0/eis_toolkit/transformations/__init__.py
+-rw-r--r--   0        0        0     3639 2024-04-08 06:45:40.454759 eis_toolkit-1.0.0/eis_toolkit/transformations/binarize.py
+-rw-r--r--   0        0        0     4696 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/transformations/clip.py
+-rw-r--r--   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-1.0.0/eis_toolkit/transformations/coda/__init__.py
+-rw-r--r--   0        0        0     3054 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/transformations/coda/alr.py
+-rw-r--r--   0        0        0     2338 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/transformations/coda/clr.py
+-rw-r--r--   0        0        0     3628 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/transformations/coda/ilr.py
+-rw-r--r--   0        0        0     2504 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/transformations/coda/pairwise.py
+-rw-r--r--   0        0        0     4136 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/transformations/coda/plr.py
+-rw-r--r--   0        0        0     7699 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/transformations/linear.py
+-rw-r--r--   0        0        0     4883 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/transformations/logarithmic.py
+-rw-r--r--   0        0        0     5205 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/transformations/one_hot_encoding.py
+-rw-r--r--   0        0        0     5163 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/transformations/sigmoid.py
+-rw-r--r--   0        0        0     6767 2024-04-08 08:42:37.268163 eis_toolkit-1.0.0/eis_toolkit/transformations/winsorize.py
+-rw-r--r--   0        0        0        0 2023-12-06 09:22:12.535287 eis_toolkit-1.0.0/eis_toolkit/utilities/__init__.py
+-rw-r--r--   0        0        0     1107 2024-04-05 07:27:18.360688 eis_toolkit-1.0.0/eis_toolkit/utilities/aitchison_geometry.py
+-rwxr-xr-x   0        0        0        0 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/utilities/checks/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-05 07:27:18.360688 eis_toolkit-1.0.0/eis_toolkit/utilities/checks/compositional.py
+-rw-r--r--   0        0        0     1672 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/utilities/checks/dataframe.py
+-rwxr-xr-x   0        0        0      599 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/utilities/checks/geometry.py
+-rw-r--r--   0        0        0     2353 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/utilities/checks/parameter.py
+-rw-r--r--   0        0        0     5837 2024-04-03 09:32:00.769041 eis_toolkit-1.0.0/eis_toolkit/utilities/checks/raster.py
+-rw-r--r--   0        0        0     1467 2024-02-22 09:12:29.164927 eis_toolkit-1.0.0/eis_toolkit/utilities/conversions.py
+-rw-r--r--   0        0        0     8640 2024-05-03 06:58:41.674662 eis_toolkit-1.0.0/eis_toolkit/utilities/file_io.py
+-rw-r--r--   0        0        0    12203 2024-04-24 06:18:14.118407 eis_toolkit-1.0.0/eis_toolkit/utilities/miscellaneous.py
+-rw-r--r--   0        0        0     4947 2024-04-24 06:18:14.118407 eis_toolkit-1.0.0/eis_toolkit/utilities/nodata.py
+-rw-r--r--   0        0        0     6041 2024-04-24 11:26:53.983156 eis_toolkit-1.0.0/eis_toolkit/utilities/raster.py
+-rwxr-xr-x   0        0        0        0 2024-04-05 07:27:15.808743 eis_toolkit-1.0.0/eis_toolkit/vector_processing/__init__.py
+-rw-r--r--   0        0        0     1098 2024-02-22 09:12:29.168927 eis_toolkit-1.0.0/eis_toolkit/vector_processing/calculate_geometry.py
+-rw-r--r--   0        0        0    22761 2024-05-24 06:00:52.148295 eis_toolkit-1.0.0/eis_toolkit/vector_processing/cell_based_association.py
+-rw-r--r--   0        0        0     3240 2024-05-02 10:42:43.425579 eis_toolkit-1.0.0/eis_toolkit/vector_processing/distance_computation.py
+-rw-r--r--   0        0        0     1942 2024-02-22 09:12:29.168927 eis_toolkit-1.0.0/eis_toolkit/vector_processing/extract_shared_lines.py
+-rw-r--r--   0        0        0     3747 2024-04-25 15:11:32.909910 eis_toolkit-1.0.0/eis_toolkit/vector_processing/idw_interpolation.py
+-rw-r--r--   0        0        0     4092 2024-04-24 11:26:53.983156 eis_toolkit-1.0.0/eis_toolkit/vector_processing/kriging_interpolation.py
+-rw-r--r--   0        0        0     4827 2024-04-24 14:32:11.183266 eis_toolkit-1.0.0/eis_toolkit/vector_processing/rasterize_vector.py
+-rw-r--r--   0        0        0      703 2023-11-10 08:05:31.345266 eis_toolkit-1.0.0/eis_toolkit/vector_processing/reproject_vector.py
+-rw-r--r--   0        0        0     1523 2024-04-24 14:32:41.807458 eis_toolkit-1.0.0/eis_toolkit/vector_processing/vector_density.py
+-rwxr-xr-x   0        0        0     1778 2024-05-27 13:52:56.128989 eis_toolkit-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7544 1970-01-01 00:00:00.000000 eis_toolkit-1.0.0/PKG-INFO
```

### Comparing `eis_toolkit-0.5.2/LICENSE` & `eis_toolkit-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/README.md` & `eis_toolkit-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,61 +46,65 @@
 pip install eis_toolkit
 ```
 
 ```console
 conda install -c conda-forge eis_toolkit
 ```
 
-You can find the latest release of EIS Toolkit also in the [releases page](https://github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository as a Python wheel. Just download the wheel and install with pip
-
-```console
-pip install eis_toolkit-0.4.0-py3-none-any.whl
-```
+A Python wheel can be downloaded also from the [releases page](https://github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository.
 
 > [!TIP]
-> GDAL needs to be installed separately on Windows when using pip / PyPI. If you have trouble installing EIS Toolkit in a venv due to GDAL, you can download a compatible GDAL wheel (for example from [this repository](https://github.com/cgohlke/geospatial-wheels/releases)), install it first, and then attempt to install EIS Toolkit again.
+> GDAL needs to be installed separately on Windows when using pip / PyPI. If you have trouble installing EIS Toolkit due to GDAL, you can download a compatible GDAL wheel (for example from [this repository](https://github.com/cgohlke/geospatial-wheels/releases)), install it first, and then attempt to install EIS Toolkit again.
 
 
 ## Usage
 EIS Toolkit can be used in Python scripts, Jupyter notebooks or via the CLI. At the moment, most tools have their own module and are imported like this:
 ```python
 # In general
 from eis_toolkit.category.module import module_function
 
 # Some examples
 from eis_toolkit.raster_processing.reprojecting import reproject_raster
 from eis_toolkit.exploratory_analyses.pca import compute_pca
 ```
 
-You can find several Jupyter notebooks in this repostiory that demonstrate how tools of EIS Toolkit can be used. The documentation of EIS Toolkit can be read [here](https://gispocoding.github.io/eis_toolkit/).
+The documentation of EIS Toolkit can be read [here](https://gispocoding.github.io/eis_toolkit/). You can find several Jupyter notebooks in this repostiory that demonstrate how tools of EIS Toolkit can be used. 
 
 
 ### EIS QGIS Plugin
 For those that prefer using tools of EIS Toolkit via a graphical user interface, check [EIS QGIS Plugin](https://github.com/GispoCoding/eis_qgis_plugin). The plugin includes the main GUI application called EIS Wizard and all individual EIS Toolkit tools as QGIS processing algorithms.
 
 The plugin is developed by the same core team that develops EIS Toolkit.
 
 ### CLI
-EIS Toolkit includes a [Typer](https://typer.tiangolo.com/) command-line interface that serves as a common interface for integrating the toolkit with external applications, such as QGIS. However, it can be used directly too. To use the CLI, simply use the command
+EIS Toolkit includes a [Typer](https://typer.tiangolo.com/) command-line interface that serves as a common interface for integrating the toolkit with external applications, such as QGIS. The CLI can be used directly too, for example
+
 ```console
-eis
+eis resample-raster-cli --input-raster path/to/raster.tif --output-raster path/to/output.tif --resolution 50 --resampling-method bilinear
 ```
 
-or
+For general help, use
 
 ```console
 eis --help
 ```
 
-to get started. However, please note that the CLI has been primarily designed to communicate with external programs and may feel clunky in direct use.
+or help for a tool
+
+```console
+eis <tool-name> --help
+```
+
+> [!NOTE] 
+> Please note that the CLI has been primarily designed to communicate with external programs and may be clunky in direct use.
 
 ## Roadmap
 
 - Milestone 1: **Beta release 0.1** (November 2023). The toolkit should have the basic funtionalities required for a full MPM workflow. Official testing phase begins. The plugin will be still under active development.
-- Milestone 2: **Release 1.0** (April 2024). All features should be incorporated at this time and the toolkit useful for actual MPM work. Testing will continue, potential bugs will be fixed and the user experience refined.
+- Milestone 2: **Release 1.0** (May 2024). Most features should be incorporated at this time and the toolkit useful for actual MPM work. Testing will continue, more advanced methods added and the user experience refined.
 
 ## Contributing
 
 We welcome contributions to EIS Toolkit in various forms:
 - ✨ Developing new tools
 - 🐞 Fixing bugs in the code
 - 📝 Bug and other reporting
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_11gsdi_v_/tmp9e08m1v9_TarContainer/0/1.md", line 6, column 35: Levels of opening and closing headings don't match*

```diff
@@ -15,59 +15,58 @@
 (https://github.com/GispoCoding/eis_qgis_plugin). > [!NOTE] > This repository
 is still in development. Check the [wiki page of EIS Toolkit](https://
 github.com/GispoCoding/eis_toolkit/wiki) for list of tools and [roadmap]
 (#roadmap) for more details about the project. ## Installation We recommend
 installing EIS Toolkit in an empty virtual environment to ensure compatibility
 between package versions. EIS Toolkit is available in conda-forge and PyPI and
 can be installed with one of the following commands. ```console pip install
-eis_toolkit ``` ```console conda install -c conda-forge eis_toolkit ``` You can
-find the latest release of EIS Toolkit also in the [releases page](https://
-github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository as a
-Python wheel. Just download the wheel and install with pip ```console pip
-install eis_toolkit-0.4.0-py3-none-any.whl ``` > [!TIP] > GDAL needs to be
-installed separately on Windows when using pip / PyPI. If you have trouble
-installing EIS Toolkit in a venv due to GDAL, you can download a compatible
-GDAL wheel (for example from [this repository](https://github.com/cgohlke/
-geospatial-wheels/releases)), install it first, and then attempt to install EIS
-Toolkit again. ## Usage EIS Toolkit can be used in Python scripts, Jupyter
-notebooks or via the CLI. At the moment, most tools have their own module and
-are imported like this: ```python # In general from eis_toolkit.category.module
-import module_function # Some examples from
+eis_toolkit ``` ```console conda install -c conda-forge eis_toolkit ``` A
+Python wheel can be downloaded also from the [releases page](https://
+github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository. >
+[!TIP] > GDAL needs to be installed separately on Windows when using pip /
+PyPI. If you have trouble installing EIS Toolkit due to GDAL, you can download
+a compatible GDAL wheel (for example from [this repository](https://github.com/
+cgohlke/geospatial-wheels/releases)), install it first, and then attempt to
+install EIS Toolkit again. ## Usage EIS Toolkit can be used in Python scripts,
+Jupyter notebooks or via the CLI. At the moment, most tools have their own
+module and are imported like this: ```python # In general from
+eis_toolkit.category.module import module_function # Some examples from
 eis_toolkit.raster_processing.reprojecting import reproject_raster from
-eis_toolkit.exploratory_analyses.pca import compute_pca ``` You can find
-several Jupyter notebooks in this repostiory that demonstrate how tools of EIS
-Toolkit can be used. The documentation of EIS Toolkit can be read [here](https:
-//gispocoding.github.io/eis_toolkit/). ### EIS QGIS Plugin For those that
-prefer using tools of EIS Toolkit via a graphical user interface, check [EIS
-QGIS Plugin](https://github.com/GispoCoding/eis_qgis_plugin). The plugin
-includes the main GUI application called EIS Wizard and all individual EIS
-Toolkit tools as QGIS processing algorithms. The plugin is developed by the
-same core team that develops EIS Toolkit. ### CLI EIS Toolkit includes a
-[Typer](https://typer.tiangolo.com/) command-line interface that serves as a
-common interface for integrating the toolkit with external applications, such
-as QGIS. However, it can be used directly too. To use the CLI, simply use the
-command ```console eis ``` or ```console eis --help ``` to get started.
-However, please note that the CLI has been primarily designed to communicate
-with external programs and may feel clunky in direct use. ## Roadmap -
-Milestone 1: **Beta release 0.1** (November 2023). The toolkit should have the
-basic funtionalities required for a full MPM workflow. Official testing phase
-begins. The plugin will be still under active development. - Milestone 2:
-**Release 1.0** (April 2024). All features should be incorporated at this time
-and the toolkit useful for actual MPM work. Testing will continue, potential
-bugs will be fixed and the user experience refined. ## Contributing We welcome
-contributions to EIS Toolkit in various forms: - â¨ Developing new tools -
-ð Fixing bugs in the code - ð Bug and other reporting - ð¡ Feature
-suggestions To contribute with code or documentation, you'll need a local
-development environment and a copy of the repository. Please refer to the **For
-developers** section below for detailed setup instructions. If you're
-interested in bug reporting or making feature suggestions, you can familiarize
-yourself with the toolkit and test it as described in the **Usage** section.
-When you encounter bugs or have ideas for new features, you can create an issue
-in this repository. ### For developers All contributing developers need Git and
-a copy of the repository. ```console git clone https://github.com/GispoCoding/
-eis_toolkit.git ``` After this you have three options for setting up your local
-development environment. 1. Docker - [instructions](./instructions/
-dev_setup_with_docker.md) 2. Poetry - [instructions](./instructions/
-dev_setup_without_docker.md) 3. Conda - [instructions](./instructions/
-dev_setup_without_docker_with_conda.md) *For general contributing guidelines,
-see [CONTRIBUTING](./CONTRIBUTING.md).* ## License Licensed under the EUPL-1.2
-or later.
+eis_toolkit.exploratory_analyses.pca import compute_pca ``` The documentation
+of EIS Toolkit can be read [here](https://gispocoding.github.io/eis_toolkit/).
+You can find several Jupyter notebooks in this repostiory that demonstrate how
+tools of EIS Toolkit can be used. ### EIS QGIS Plugin For those that prefer
+using tools of EIS Toolkit via a graphical user interface, check [EIS QGIS
+Plugin](https://github.com/GispoCoding/eis_qgis_plugin). The plugin includes
+the main GUI application called EIS Wizard and all individual EIS Toolkit tools
+as QGIS processing algorithms. The plugin is developed by the same core team
+that develops EIS Toolkit. ### CLI EIS Toolkit includes a [Typer](https://
+typer.tiangolo.com/) command-line interface that serves as a common interface
+for integrating the toolkit with external applications, such as QGIS. The CLI
+can be used directly too, for example ```console eis resample-raster-cli --
+input-raster path/to/raster.tif --output-raster path/to/output.tif --resolution
+50 --resampling-method bilinear ``` For general help, use ```console eis --help
+``` or help for a tool ```console eis --help ``` > [!NOTE] > Please note that
+the CLI has been primarily designed to communicate with external programs and
+may be clunky in direct use. ## Roadmap - Milestone 1: **Beta release 0.1**
+(November 2023). The toolkit should have the basic funtionalities required for
+a full MPM workflow. Official testing phase begins. The plugin will be still
+under active development. - Milestone 2: **Release 1.0** (May 2024). Most
+features should be incorporated at this time and the toolkit useful for actual
+MPM work. Testing will continue, more advanced methods added and the user
+experience refined. ## Contributing We welcome contributions to EIS Toolkit in
+various forms: - â¨ Developing new tools - ð Fixing bugs in the code - ð
+Bug and other reporting - ð¡ Feature suggestions To contribute with code or
+documentation, you'll need a local development environment and a copy of the
+repository. Please refer to the **For developers** section below for detailed
+setup instructions. If you're interested in bug reporting or making feature
+suggestions, you can familiarize yourself with the toolkit and test it as
+described in the **Usage** section. When you encounter bugs or have ideas for
+new features, you can create an issue in this repository. ### For developers
+All contributing developers need Git and a copy of the repository. ```console
+git clone https://github.com/GispoCoding/eis_toolkit.git ``` After this you
+have three options for setting up your local development environment. 1. Docker
+- [instructions](./instructions/dev_setup_with_docker.md) 2. Poetry -
+[instructions](./instructions/dev_setup_without_docker.md) 3. Conda -
+[instructions](./instructions/dev_setup_without_docker_with_conda.md) *For
+general contributing guidelines, see [CONTRIBUTING](./CONTRIBUTING.md).* ##
+License Licensed under the EUPL-1.2 or later.
```

### Comparing `eis_toolkit-0.5.2/eis_toolkit/cli.py` & `eis_toolkit-1.0.0/eis_toolkit/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -722,18 +722,17 @@
     typer.echo("Progress: 10%")
 
     with rasterio.open(input_file) as raster:
         typer.echo("Progress: 25%")
         results_dict = descriptive_statistics_raster(raster)
     typer.echo("Progress: 75%")
 
-    json_str = json.dumps(results_dict)
-    typer.echo("Progress: 100%\n")
+    typer.echo("Progress: 100% \n")
 
-    typer.echo(f"Results: {json_str}")
+    typer.echo(f"Results: {str(results_dict)}")
     typer.echo("\nDescriptive statistics (raster) completed")
 
 
 # DESCRIPTIVE STATISTICS (VECTOR)
 @app.command()
 def descriptive_statistics_vector_cli(input_file: INPUT_FILE_OPTION, column: str = None):
     """Generate descriptive statistics from vector or tabular data."""
@@ -751,19 +750,18 @@
             df = pd.read_csv(input_file)
             typer.echo("Progress: 25%")
             results_dict = descriptive_statistics_dataframe(df, column)
         except:  # noqa: E722
             raise Exception("Could not read input file as raster or dataframe")
     typer.echo("Progress: 75%")
 
-    json_str = json.dumps(results_dict)
     typer.echo("Progress: 100%")
 
-    typer.echo(f"Results: {json_str}")
-    typer.echo("Descriptive statistics (vector) completed")
+    typer.echo(f"Results: {str(results_dict)}")
+    typer.echo("\nDescriptive statistics (vector) completed")
 
 
 # LOCAL MORAN'S I
 @app.command()
 def local_morans_i_cli(
     input_vector: INPUT_FILE_OPTION,
     output_vector: OUTPUT_FILE_OPTION,
@@ -1362,15 +1360,15 @@
             same_extent=same_extent,
         )
         [rstr.close() for rstr in to_unify]  # Close all rasters
     typer.echo("Progress: 75%")
 
     out_rasters_dict = {}
     for i, (out_image, out_meta) in enumerate(unified[1:]):  # Skip writing base raster
-        in_raster_name = os.path.splitext(os.path.split(rasters_to_unify[i - 1])[1])[0]
+        in_raster_name = os.path.splitext(os.path.split(rasters_to_unify[i])[1])[0]
         output_raster_name = f"{in_raster_name}_unified"
         output_raster_path = output_directory.joinpath(output_raster_name + ".tif")
         with rasterio.open(output_raster_path, "w", **out_meta) as dst:
             dst.write(out_image)
         out_rasters_dict[output_raster_name] = str(output_raster_path)
     typer.echo("Progress: 100%")
 
@@ -3111,18 +3109,17 @@
     (y_prob, y_true), _, _ = read_data_for_evaluation([probabilities, true_labels])
     typer.echo("Progress: 25%")
 
     results_dict = summarize_probability_metrics(y_true=y_true, y_prob=y_prob)
 
     typer.echo("Progress: 75%")
 
-    json_str = json.dumps(results_dict)
     typer.echo("Progress: 100% \n")
 
-    typer.echo(f"Results: {json_str}")
+    typer.echo(f"Results: {str(results_dict)}")
     typer.echo("\nGenerating probability metrics summary completed.")
 
 
 @app.command()
 def summarize_label_metrics_binary_cli(true_labels: INPUT_FILE_OPTION, predictions: INPUT_FILE_OPTION):
     """
     Generate a comprehensive report of various evaluation metrics for binary classification results.
@@ -3137,19 +3134,18 @@
 
     (y_pred, y_true), _, _ = read_data_for_evaluation([predictions, true_labels])
     typer.echo("Progress: 25%")
 
     results_dict = summarize_label_metrics_binary(y_true=y_true, y_pred=y_pred)
     typer.echo("Progress: 75%")
 
-    json_str = json.dumps(results_dict)
     typer.echo("Progress: 100% \n")
 
-    typer.echo(f"Results: {json_str}")
-    typer.echo("\n Generating prediction label metrics summary completed.")
+    typer.echo(f"Results: {str(results_dict)}")
+    typer.echo("\nGenerating prediction label metrics summary completed.")
 
 
 @app.command()
 def plot_roc_curve_cli(
     true_labels: INPUT_FILE_OPTION,
     probabilities: INPUT_FILE_OPTION,
     output_file: OUTPUT_FILE_OPTION,
@@ -3353,20 +3349,15 @@
 
     (y_pred, y_true), _, _ = read_data_for_evaluation([predictions, true_labels])
     typer.echo("Progress: 25%")
 
     outputs = score_predictions(y_true, y_pred, metrics)
     typer.echo("Progress: 100% \n")
 
-    if isinstance(outputs, dict):
-        for key, value in outputs.items():
-            typer.echo(f"{key}: {value}")
-    else:
-        typer.echo(outputs)
-
+    typer.echo(f"Results: {str(outputs)}")
     typer.echo("\nScoring predictions completed.")
 
 
 # --- UTILITIES ---
 @app.command()
 def split_raster_bands_cli(input_raster: INPUT_FILE_OPTION, output_dir: OUTPUT_DIR_OPTION):  # CHECK
     """Split multiband raster into singleband rasters."""
```

### Comparing `eis_toolkit-0.5.2/eis_toolkit/conversions/csv_to_geodataframe.py` & `eis_toolkit-1.0.0/eis_toolkit/conversions/csv_to_geodataframe.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/conversions/raster_to_dataframe.py` & `eis_toolkit-1.0.0/eis_toolkit/conversions/raster_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/evaluation/calculate_base_metrics.py` & `eis_toolkit-1.0.0/eis_toolkit/evaluation/calculate_base_metrics.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/evaluation/classification_label_evaluation.py` & `eis_toolkit-1.0.0/eis_toolkit/evaluation/classification_label_evaluation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/evaluation/classification_probability_evaluation.py` & `eis_toolkit-1.0.0/eis_toolkit/evaluation/classification_probability_evaluation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_confusion_matrix.py` & `eis_toolkit-1.0.0/eis_toolkit/evaluation/plot_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_nn_model_performance.py` & `eis_toolkit-1.0.0/eis_toolkit/evaluation/plot_nn_model_performance.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_prediction_area_curves.py` & `eis_toolkit-1.0.0/eis_toolkit/evaluation/plot_prediction_area_curves.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/evaluation/plot_rate_curve.py` & `eis_toolkit-1.0.0/eis_toolkit/evaluation/plot_rate_curve.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/evaluation/scoring.py` & `eis_toolkit-1.0.0/eis_toolkit/evaluation/scoring.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/exceptions.py` & `eis_toolkit-1.0.0/eis_toolkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/chi_square_test.py` & `eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/chi_square_test.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/correlation_matrix.py` & `eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/covariance_matrix.py` & `eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/covariance_matrix.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/dbscan.py` & `eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/dbscan.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/descriptive_statistics.py` & `eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/descriptive_statistics.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/feature_importance.py` & `eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/feature_importance.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/k_means_cluster.py` & `eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/k_means_cluster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/local_morans_i.py` & `eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/local_morans_i.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/normality_test.py` & `eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/normality_test.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/parallel_coordinates.py` & `eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/exploratory_analyses/pca.py` & `eis_toolkit-1.0.0/eis_toolkit/exploratory_analyses/pca.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/prediction/fuzzy_overlay.py` & `eis_toolkit-1.0.0/eis_toolkit/prediction/fuzzy_overlay.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/prediction/gradient_boosting.py` & `eis_toolkit-1.0.0/eis_toolkit/prediction/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/prediction/logistic_regression.py` & `eis_toolkit-1.0.0/eis_toolkit/prediction/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/prediction/machine_learning_general.py` & `eis_toolkit-1.0.0/eis_toolkit/prediction/machine_learning_general.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/prediction/machine_learning_predict.py` & `eis_toolkit-1.0.0/eis_toolkit/prediction/machine_learning_predict.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/prediction/mlp.py` & `eis_toolkit-1.0.0/eis_toolkit/prediction/mlp.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/prediction/random_forests.py` & `eis_toolkit-1.0.0/eis_toolkit/prediction/random_forests.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/prediction/weights_of_evidence.py` & `eis_toolkit-1.0.0/eis_toolkit/prediction/weights_of_evidence.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/clipping.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/clipping.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/create_constant_raster.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/create_constant_raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/classification.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/derivatives/classification.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/parameters.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/derivatives/parameters.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/partial_derivatives.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/derivatives/partial_derivatives.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/derivatives/utilities.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/derivatives/utilities.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/distance_to_anomaly.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/distance_to_anomaly.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/extract_values_from_raster.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/extract_values_from_raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/focal.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/filters/focal.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/kernels.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/filters/kernels.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/speckle.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/filters/speckle.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/filters/utilities.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/filters/utilities.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/reclassify.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/reclassify.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/reprojecting.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/reprojecting.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/resampling.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/resampling.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/snapping.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/snapping.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/unifying.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/unifying.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/unique_combinations.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/unique_combinations.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/raster_processing/windowing.py` & `eis_toolkit-1.0.0/eis_toolkit/raster_processing/windowing.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/training_data_tools/class_balancing.py` & `eis_toolkit-1.0.0/eis_toolkit/training_data_tools/class_balancing.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/transformations/binarize.py` & `eis_toolkit-1.0.0/eis_toolkit/transformations/binarize.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/transformations/clip.py` & `eis_toolkit-1.0.0/eis_toolkit/transformations/clip.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/transformations/coda/alr.py` & `eis_toolkit-1.0.0/eis_toolkit/transformations/coda/alr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/transformations/coda/clr.py` & `eis_toolkit-1.0.0/eis_toolkit/transformations/coda/clr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/transformations/coda/ilr.py` & `eis_toolkit-1.0.0/eis_toolkit/transformations/coda/ilr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/transformations/coda/pairwise.py` & `eis_toolkit-1.0.0/eis_toolkit/transformations/coda/pairwise.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/transformations/coda/plr.py` & `eis_toolkit-1.0.0/eis_toolkit/transformations/coda/plr.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/transformations/linear.py` & `eis_toolkit-1.0.0/eis_toolkit/transformations/linear.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/transformations/logarithmic.py` & `eis_toolkit-1.0.0/eis_toolkit/transformations/logarithmic.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/transformations/one_hot_encoding.py` & `eis_toolkit-1.0.0/eis_toolkit/transformations/one_hot_encoding.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/transformations/sigmoid.py` & `eis_toolkit-1.0.0/eis_toolkit/transformations/sigmoid.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/transformations/winsorize.py` & `eis_toolkit-1.0.0/eis_toolkit/transformations/winsorize.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/utilities/aitchison_geometry.py` & `eis_toolkit-1.0.0/eis_toolkit/utilities/aitchison_geometry.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/utilities/checks/compositional.py` & `eis_toolkit-1.0.0/eis_toolkit/utilities/checks/compositional.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/utilities/checks/dataframe.py` & `eis_toolkit-1.0.0/eis_toolkit/utilities/checks/dataframe.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/utilities/checks/geometry.py` & `eis_toolkit-1.0.0/eis_toolkit/utilities/checks/geometry.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/utilities/checks/parameter.py` & `eis_toolkit-1.0.0/eis_toolkit/utilities/checks/parameter.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/utilities/checks/raster.py` & `eis_toolkit-1.0.0/eis_toolkit/utilities/checks/raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/utilities/conversions.py` & `eis_toolkit-1.0.0/eis_toolkit/utilities/conversions.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/utilities/file_io.py` & `eis_toolkit-1.0.0/eis_toolkit/utilities/file_io.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/utilities/miscellaneous.py` & `eis_toolkit-1.0.0/eis_toolkit/utilities/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/utilities/nodata.py` & `eis_toolkit-1.0.0/eis_toolkit/utilities/nodata.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/utilities/raster.py` & `eis_toolkit-1.0.0/eis_toolkit/utilities/raster.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/vector_processing/calculate_geometry.py` & `eis_toolkit-1.0.0/eis_toolkit/vector_processing/calculate_geometry.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/vector_processing/cell_based_association.py` & `eis_toolkit-1.0.0/eis_toolkit/vector_processing/cell_based_association.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/vector_processing/distance_computation.py` & `eis_toolkit-1.0.0/eis_toolkit/vector_processing/distance_computation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/vector_processing/extract_shared_lines.py` & `eis_toolkit-1.0.0/eis_toolkit/vector_processing/extract_shared_lines.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/vector_processing/idw_interpolation.py` & `eis_toolkit-1.0.0/eis_toolkit/vector_processing/idw_interpolation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/vector_processing/kriging_interpolation.py` & `eis_toolkit-1.0.0/eis_toolkit/vector_processing/kriging_interpolation.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/vector_processing/rasterize_vector.py` & `eis_toolkit-1.0.0/eis_toolkit/vector_processing/rasterize_vector.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/vector_processing/reproject_vector.py` & `eis_toolkit-1.0.0/eis_toolkit/vector_processing/reproject_vector.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/eis_toolkit/vector_processing/vector_density.py` & `eis_toolkit-1.0.0/eis_toolkit/vector_processing/vector_density.py`

 * *Files identical despite different names*

### Comparing `eis_toolkit-0.5.2/pyproject.toml` & `eis_toolkit-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eis_toolkit"
-version = "0.5.2"
+version = "1.0.0"
 description = "EIS Toolkit is a comprehensive collection of tools suitable for mineral prospectivity mapping. This toolkit has been developed as part of the Exploration Information System project which has been funded by European Union."
 authors = []
 maintainers = ["Gispo Ltd. <info@gispo.fi>"]
 license = "EUPL-1.2"
 readme = "README.md"
 homepage = "https://eis-he.eu"
 repository = "https://github.com/GispoCoding/eis_toolkit"
```

### Comparing `eis_toolkit-0.5.2/PKG-INFO` & `eis_toolkit-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis_toolkit
-Version: 0.5.2
+Version: 1.0.0
 Summary: EIS Toolkit is a comprehensive collection of tools suitable for mineral prospectivity mapping. This toolkit has been developed as part of the Exploration Information System project which has been funded by European Union.
 Home-page: https://eis-he.eu
 License: EUPL-1.2
 Keywords: Development Status :: 4 - Beta,Topic :: Scientific/Engineering :: GIS,Programming Language :: Python :: 3 :: Only
 Maintainer: Gispo Ltd.
 Maintainer-email: info@gispo.fi
 Requires-Python: >=3.9,<3.11
@@ -81,61 +81,65 @@
 pip install eis_toolkit
 ```
 
 ```console
 conda install -c conda-forge eis_toolkit
 ```
 
-You can find the latest release of EIS Toolkit also in the [releases page](https://github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository as a Python wheel. Just download the wheel and install with pip
-
-```console
-pip install eis_toolkit-0.4.0-py3-none-any.whl
-```
+A Python wheel can be downloaded also from the [releases page](https://github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository.
 
 > [!TIP]
-> GDAL needs to be installed separately on Windows when using pip / PyPI. If you have trouble installing EIS Toolkit in a venv due to GDAL, you can download a compatible GDAL wheel (for example from [this repository](https://github.com/cgohlke/geospatial-wheels/releases)), install it first, and then attempt to install EIS Toolkit again.
+> GDAL needs to be installed separately on Windows when using pip / PyPI. If you have trouble installing EIS Toolkit due to GDAL, you can download a compatible GDAL wheel (for example from [this repository](https://github.com/cgohlke/geospatial-wheels/releases)), install it first, and then attempt to install EIS Toolkit again.
 
 
 ## Usage
 EIS Toolkit can be used in Python scripts, Jupyter notebooks or via the CLI. At the moment, most tools have their own module and are imported like this:
 ```python
 # In general
 from eis_toolkit.category.module import module_function
 
 # Some examples
 from eis_toolkit.raster_processing.reprojecting import reproject_raster
 from eis_toolkit.exploratory_analyses.pca import compute_pca
 ```
 
-You can find several Jupyter notebooks in this repostiory that demonstrate how tools of EIS Toolkit can be used. The documentation of EIS Toolkit can be read [here](https://gispocoding.github.io/eis_toolkit/).
+The documentation of EIS Toolkit can be read [here](https://gispocoding.github.io/eis_toolkit/). You can find several Jupyter notebooks in this repostiory that demonstrate how tools of EIS Toolkit can be used. 
 
 
 ### EIS QGIS Plugin
 For those that prefer using tools of EIS Toolkit via a graphical user interface, check [EIS QGIS Plugin](https://github.com/GispoCoding/eis_qgis_plugin). The plugin includes the main GUI application called EIS Wizard and all individual EIS Toolkit tools as QGIS processing algorithms.
 
 The plugin is developed by the same core team that develops EIS Toolkit.
 
 ### CLI
-EIS Toolkit includes a [Typer](https://typer.tiangolo.com/) command-line interface that serves as a common interface for integrating the toolkit with external applications, such as QGIS. However, it can be used directly too. To use the CLI, simply use the command
+EIS Toolkit includes a [Typer](https://typer.tiangolo.com/) command-line interface that serves as a common interface for integrating the toolkit with external applications, such as QGIS. The CLI can be used directly too, for example
+
 ```console
-eis
+eis resample-raster-cli --input-raster path/to/raster.tif --output-raster path/to/output.tif --resolution 50 --resampling-method bilinear
 ```
 
-or
+For general help, use
 
 ```console
 eis --help
 ```
 
-to get started. However, please note that the CLI has been primarily designed to communicate with external programs and may feel clunky in direct use.
+or help for a tool
+
+```console
+eis <tool-name> --help
+```
+
+> [!NOTE] 
+> Please note that the CLI has been primarily designed to communicate with external programs and may be clunky in direct use.
 
 ## Roadmap
 
 - Milestone 1: **Beta release 0.1** (November 2023). The toolkit should have the basic funtionalities required for a full MPM workflow. Official testing phase begins. The plugin will be still under active development.
-- Milestone 2: **Release 1.0** (April 2024). All features should be incorporated at this time and the toolkit useful for actual MPM work. Testing will continue, potential bugs will be fixed and the user experience refined.
+- Milestone 2: **Release 1.0** (May 2024). Most features should be incorporated at this time and the toolkit useful for actual MPM work. Testing will continue, more advanced methods added and the user experience refined.
 
 ## Contributing
 
 We welcome contributions to EIS Toolkit in various forms:
 - ✨ Developing new tools
 - 🐞 Fixing bugs in the code
 - 📝 Bug and other reporting
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_11gsdi_v_/tmp9e08m1v9_TarContainer/0/103", line 41, column 35: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eis_toolkit Version: 0.5.2 Summary: EIS Toolkit is
+Metadata-Version: 2.1 Name: eis_toolkit Version: 1.0.0 Summary: EIS Toolkit is
 a comprehensive collection of tools suitable for mineral prospectivity mapping.
 This toolkit has been developed as part of the Exploration Information System
 project which has been funded by European Union. Home-page: https://eis-he.eu
 License: EUPL-1.2 Keywords: Development Status :: 4 - Beta,Topic :: Scientific/
 Engineering :: GIS,Programming Language :: Python :: 3 :: Only Maintainer:
 Gispo Ltd. Maintainer-email: info@gispo.fi Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL
@@ -37,59 +37,58 @@
 (https://github.com/GispoCoding/eis_qgis_plugin). > [!NOTE] > This repository
 is still in development. Check the [wiki page of EIS Toolkit](https://
 github.com/GispoCoding/eis_toolkit/wiki) for list of tools and [roadmap]
 (#roadmap) for more details about the project. ## Installation We recommend
 installing EIS Toolkit in an empty virtual environment to ensure compatibility
 between package versions. EIS Toolkit is available in conda-forge and PyPI and
 can be installed with one of the following commands. ```console pip install
-eis_toolkit ``` ```console conda install -c conda-forge eis_toolkit ``` You can
-find the latest release of EIS Toolkit also in the [releases page](https://
-github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository as a
-Python wheel. Just download the wheel and install with pip ```console pip
-install eis_toolkit-0.4.0-py3-none-any.whl ``` > [!TIP] > GDAL needs to be
-installed separately on Windows when using pip / PyPI. If you have trouble
-installing EIS Toolkit in a venv due to GDAL, you can download a compatible
-GDAL wheel (for example from [this repository](https://github.com/cgohlke/
-geospatial-wheels/releases)), install it first, and then attempt to install EIS
-Toolkit again. ## Usage EIS Toolkit can be used in Python scripts, Jupyter
-notebooks or via the CLI. At the moment, most tools have their own module and
-are imported like this: ```python # In general from eis_toolkit.category.module
-import module_function # Some examples from
+eis_toolkit ``` ```console conda install -c conda-forge eis_toolkit ``` A
+Python wheel can be downloaded also from the [releases page](https://
+github.com/GispoCoding/eis_toolkit/releases) of this GitHub repository. >
+[!TIP] > GDAL needs to be installed separately on Windows when using pip /
+PyPI. If you have trouble installing EIS Toolkit due to GDAL, you can download
+a compatible GDAL wheel (for example from [this repository](https://github.com/
+cgohlke/geospatial-wheels/releases)), install it first, and then attempt to
+install EIS Toolkit again. ## Usage EIS Toolkit can be used in Python scripts,
+Jupyter notebooks or via the CLI. At the moment, most tools have their own
+module and are imported like this: ```python # In general from
+eis_toolkit.category.module import module_function # Some examples from
 eis_toolkit.raster_processing.reprojecting import reproject_raster from
-eis_toolkit.exploratory_analyses.pca import compute_pca ``` You can find
-several Jupyter notebooks in this repostiory that demonstrate how tools of EIS
-Toolkit can be used. The documentation of EIS Toolkit can be read [here](https:
-//gispocoding.github.io/eis_toolkit/). ### EIS QGIS Plugin For those that
-prefer using tools of EIS Toolkit via a graphical user interface, check [EIS
-QGIS Plugin](https://github.com/GispoCoding/eis_qgis_plugin). The plugin
-includes the main GUI application called EIS Wizard and all individual EIS
-Toolkit tools as QGIS processing algorithms. The plugin is developed by the
-same core team that develops EIS Toolkit. ### CLI EIS Toolkit includes a
-[Typer](https://typer.tiangolo.com/) command-line interface that serves as a
-common interface for integrating the toolkit with external applications, such
-as QGIS. However, it can be used directly too. To use the CLI, simply use the
-command ```console eis ``` or ```console eis --help ``` to get started.
-However, please note that the CLI has been primarily designed to communicate
-with external programs and may feel clunky in direct use. ## Roadmap -
-Milestone 1: **Beta release 0.1** (November 2023). The toolkit should have the
-basic funtionalities required for a full MPM workflow. Official testing phase
-begins. The plugin will be still under active development. - Milestone 2:
-**Release 1.0** (April 2024). All features should be incorporated at this time
-and the toolkit useful for actual MPM work. Testing will continue, potential
-bugs will be fixed and the user experience refined. ## Contributing We welcome
-contributions to EIS Toolkit in various forms: - â¨ Developing new tools -
-ð Fixing bugs in the code - ð Bug and other reporting - ð¡ Feature
-suggestions To contribute with code or documentation, you'll need a local
-development environment and a copy of the repository. Please refer to the **For
-developers** section below for detailed setup instructions. If you're
-interested in bug reporting or making feature suggestions, you can familiarize
-yourself with the toolkit and test it as described in the **Usage** section.
-When you encounter bugs or have ideas for new features, you can create an issue
-in this repository. ### For developers All contributing developers need Git and
-a copy of the repository. ```console git clone https://github.com/GispoCoding/
-eis_toolkit.git ``` After this you have three options for setting up your local
-development environment. 1. Docker - [instructions](./instructions/
-dev_setup_with_docker.md) 2. Poetry - [instructions](./instructions/
-dev_setup_without_docker.md) 3. Conda - [instructions](./instructions/
-dev_setup_without_docker_with_conda.md) *For general contributing guidelines,
-see [CONTRIBUTING](./CONTRIBUTING.md).* ## License Licensed under the EUPL-1.2
-or later.
+eis_toolkit.exploratory_analyses.pca import compute_pca ``` The documentation
+of EIS Toolkit can be read [here](https://gispocoding.github.io/eis_toolkit/).
+You can find several Jupyter notebooks in this repostiory that demonstrate how
+tools of EIS Toolkit can be used. ### EIS QGIS Plugin For those that prefer
+using tools of EIS Toolkit via a graphical user interface, check [EIS QGIS
+Plugin](https://github.com/GispoCoding/eis_qgis_plugin). The plugin includes
+the main GUI application called EIS Wizard and all individual EIS Toolkit tools
+as QGIS processing algorithms. The plugin is developed by the same core team
+that develops EIS Toolkit. ### CLI EIS Toolkit includes a [Typer](https://
+typer.tiangolo.com/) command-line interface that serves as a common interface
+for integrating the toolkit with external applications, such as QGIS. The CLI
+can be used directly too, for example ```console eis resample-raster-cli --
+input-raster path/to/raster.tif --output-raster path/to/output.tif --resolution
+50 --resampling-method bilinear ``` For general help, use ```console eis --help
+``` or help for a tool ```console eis --help ``` > [!NOTE] > Please note that
+the CLI has been primarily designed to communicate with external programs and
+may be clunky in direct use. ## Roadmap - Milestone 1: **Beta release 0.1**
+(November 2023). The toolkit should have the basic funtionalities required for
+a full MPM workflow. Official testing phase begins. The plugin will be still
+under active development. - Milestone 2: **Release 1.0** (May 2024). Most
+features should be incorporated at this time and the toolkit useful for actual
+MPM work. Testing will continue, more advanced methods added and the user
+experience refined. ## Contributing We welcome contributions to EIS Toolkit in
+various forms: - â¨ Developing new tools - ð Fixing bugs in the code - ð
+Bug and other reporting - ð¡ Feature suggestions To contribute with code or
+documentation, you'll need a local development environment and a copy of the
+repository. Please refer to the **For developers** section below for detailed
+setup instructions. If you're interested in bug reporting or making feature
+suggestions, you can familiarize yourself with the toolkit and test it as
+described in the **Usage** section. When you encounter bugs or have ideas for
+new features, you can create an issue in this repository. ### For developers
+All contributing developers need Git and a copy of the repository. ```console
+git clone https://github.com/GispoCoding/eis_toolkit.git ``` After this you
+have three options for setting up your local development environment. 1. Docker
+- [instructions](./instructions/dev_setup_with_docker.md) 2. Poetry -
+[instructions](./instructions/dev_setup_without_docker.md) 3. Conda -
+[instructions](./instructions/dev_setup_without_docker_with_conda.md) *For
+general contributing guidelines, see [CONTRIBUTING](./CONTRIBUTING.md).* ##
+License Licensed under the EUPL-1.2 or later.
```

