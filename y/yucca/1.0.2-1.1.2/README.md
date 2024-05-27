# Comparing `tmp/yucca-1.0.2.tar.gz` & `tmp/yucca-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yucca-1.0.2.tar", last modified: Fri Mar 22 18:08:57 2024, max compression
+gzip compressed data, was "yucca-1.1.2.tar", last modified: Mon May 27 09:37:22 2024, max compression
```

## Comparing `yucca-1.0.2.tar` & `yucca-1.1.2.tar`

### file list

```diff
@@ -1,244 +1,303 @@
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.574204 yucca-1.0.2/
--rw-r--r--   0 zcr545     (501) staff       (20)    11357 2023-10-26 08:30:20.000000 yucca-1.0.2/LICENSE
--rw-r--r--   0 zcr545     (501) staff       (20)    16019 2024-03-22 18:08:57.573894 yucca-1.0.2/PKG-INFO
--rw-r--r--   0 zcr545     (501) staff       (20)    14366 2024-03-22 17:22:59.000000 yucca-1.0.2/README.md
--rw-r--r--   0 zcr545     (501) staff       (20)     1975 2024-03-22 18:08:35.000000 yucca-1.0.2/pyproject.toml
--rw-r--r--   0 zcr545     (501) staff       (20)       91 2024-03-22 18:08:57.575194 yucca-1.0.2/setup.cfg
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:56.811253 yucca-1.0.2/tests/
--rw-r--r--   0 zcr545     (501) staff       (20)     2552 2024-02-06 14:22:56.000000 yucca-1.0.2/tests/test_configurations.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4312 2024-03-21 12:23:07.000000 yucca-1.0.2/tests/test_end_to_end.py
--rw-r--r--   0 zcr545     (501) staff       (20)      359 2023-12-18 12:58:40.000000 yucca-1.0.2/tests/test_infinite_random_batch_sampler.py
--rw-r--r--   0 zcr545     (501) staff       (20)      188 2024-01-03 09:48:17.000000 yucca-1.0.2/tests/test_manager.py
--rw-r--r--   0 zcr545     (501) staff       (20)      108 2023-11-15 09:40:14.000000 yucca-1.0.2/tests/test_paths.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:56.822481 yucca-1.0.2/yucca/
--rw-r--r--   0 zcr545     (501) staff       (20)       59 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:56.849528 yucca-1.0.2/yucca/deprecated/
--rw-r--r--   0 zcr545     (501) staff       (20)    16113 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/deprecated/YuccaLoader.py
--rw-r--r--   0 zcr545     (501) staff       (20)    13769 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/deprecated/YuccaManager.py
--rw-r--r--   0 zcr545     (501) staff       (20)    33216 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/deprecated/base_manager.py
--rw-r--r--   0 zcr545     (501) staff       (20)     5672 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/deprecated/run_training_OLD.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:56.878953 yucca-1.0.2/yucca/evaluation/
--rw-r--r--   0 zcr545     (501) staff       (20)    14196 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/evaluation/YuccaEvaluator.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-10-26 08:38:45.000000 yucca-1.0.2/yucca/evaluation/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:56.885980 yucca-1.0.2/yucca/evaluation/challenge_evaluation_scripts/
--rw-r--r--   0 zcr545     (501) staff       (20)    10279 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/evaluation/challenge_evaluation_scripts/isles_eval.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:56.889534 yucca-1.0.2/yucca/evaluation/challenge_preparation_scripts/
--rw-r--r--   0 zcr545     (501) staff       (20)     3090 2023-11-25 21:17:51.000000 yucca-1.0.2/yucca/evaluation/challenge_preparation_scripts/prepare_decathlon.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1028 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/evaluation/confusion_matrix.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:56.899222 yucca-1.0.2/yucca/evaluation/deepmind_surface_distance/
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-03-18 17:16:20.000000 yucca-1.0.2/yucca/evaluation/deepmind_surface_distance/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)    22423 2024-03-18 17:16:20.000000 yucca-1.0.2/yucca/evaluation/deepmind_surface_distance/lookup_tables.py
--rw-r--r--   0 zcr545     (501) staff       (20)    18475 2024-03-18 17:16:20.000000 yucca-1.0.2/yucca/evaluation/deepmind_surface_distance/metrics.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4894 2024-02-19 12:41:30.000000 yucca-1.0.2/yucca/evaluation/loggers.py
--rw-r--r--   0 zcr545     (501) staff       (20)     3619 2024-02-19 12:41:30.000000 yucca-1.0.2/yucca/evaluation/metrics.py
--rw-r--r--   0 zcr545     (501) staff       (20)     3026 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/evaluation/obj_metrics.py
--rw-r--r--   0 zcr545     (501) staff       (20)      928 2024-03-18 17:16:55.000000 yucca-1.0.2/yucca/evaluation/surface_metrics.py
--rw-r--r--   0 zcr545     (501) staff       (20)      348 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/evaluation/training_metrics.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:56.906123 yucca-1.0.2/yucca/image_processing/
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/image_processing/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2300 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/image_processing/cropping_and_padding.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2287 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/image_processing/matrix_ops.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:56.915763 yucca-1.0.2/yucca/image_processing/objects/
--rw-r--r--   0 zcr545     (501) staff       (20)     2739 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/image_processing/objects/BoundingBox.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/image_processing/objects/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)      583 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/image_processing/objects/filtering.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:56.975341 yucca-1.0.2/yucca/image_processing/transforms/
--rw-r--r--   0 zcr545     (501) staff       (20)     2132 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/image_processing/transforms/BiasField.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1506 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/image_processing/transforms/Blur.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1004 2024-03-21 12:23:07.000000 yucca-1.0.2/yucca/image_processing/transforms/CopyImageToSeg.py
--rw-r--r--   0 zcr545     (501) staff       (20)     5042 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/image_processing/transforms/Gamma.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2940 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/image_processing/transforms/Ghosting.py
--rw-r--r--   0 zcr545     (501) staff       (20)     6012 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/image_processing/transforms/Masking.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2425 2024-03-21 12:23:07.000000 yucca-1.0.2/yucca/image_processing/transforms/Mirror.py
--rw-r--r--   0 zcr545     (501) staff       (20)     3286 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/image_processing/transforms/Noise.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4004 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/image_processing/transforms/Ringing.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2440 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/image_processing/transforms/SimulateLowres.py
--rw-r--r--   0 zcr545     (501) staff       (20)     7437 2024-03-21 12:23:07.000000 yucca-1.0.2/yucca/image_processing/transforms/Spatial.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1577 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/image_processing/transforms/YuccaTransform.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/image_processing/transforms/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)    12639 2024-03-21 12:23:07.000000 yucca-1.0.2/yucca/image_processing/transforms/cropping_and_padding.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4636 2024-03-21 12:23:07.000000 yucca-1.0.2/yucca/image_processing/transforms/formatting.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1849 2024-01-19 08:47:55.000000 yucca-1.0.2/yucca/image_processing/transforms/sampling.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:56.975906 yucca-1.0.2/yucca/network_architectures/
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/network_architectures/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:56.990198 yucca-1.0.2/yucca/network_architectures/blocks_and_layers/
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/network_architectures/blocks_and_layers/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)    23680 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/network_architectures/blocks_and_layers/conv_blocks.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4875 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/network_architectures/blocks_and_layers/conv_layers.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1243 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/network_architectures/blocks_and_layers/norm.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.029317 yucca-1.0.2/yucca/network_architectures/networks/
--rw-r--r--   0 zcr545     (501) staff       (20)     3638 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/network_architectures/networks/DeepLabHeadV3Plus.py
--rw-r--r--   0 zcr545     (501) staff       (20)    30850 2024-02-19 12:41:30.000000 yucca-1.0.2/yucca/network_architectures/networks/MedNeXt.py
--rw-r--r--   0 zcr545     (501) staff       (20)    11368 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/network_architectures/networks/MultiResUNet.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4920 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/network_architectures/networks/TinyUNet.py
--rw-r--r--   0 zcr545     (501) staff       (20)     7872 2024-01-19 08:47:55.000000 yucca-1.0.2/yucca/network_architectures/networks/UNet.py
--rw-r--r--   0 zcr545     (501) staff       (20)     9326 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/network_architectures/networks/UNetR.py
--rw-r--r--   0 zcr545     (501) staff       (20)     7580 2024-01-03 09:48:17.000000 yucca-1.0.2/yucca/network_architectures/networks/UNetRE.py
--rw-r--r--   0 zcr545     (501) staff       (20)     6801 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/network_architectures/networks/UXNet.py
--rw-r--r--   0 zcr545     (501) staff       (20)     5285 2024-03-11 14:50:22.000000 yucca-1.0.2/yucca/network_architectures/networks/YuccaNet.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/network_architectures/networks/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4874 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/network_architectures/networks/resnet.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.036516 yucca-1.0.2/yucca/network_architectures/utils/
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/network_architectures/utils/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1068 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/network_architectures/utils/get_steps_for_sliding_window.py
--rw-r--r--   0 zcr545     (501) staff       (20)     9279 2024-03-11 14:50:22.000000 yucca-1.0.2/yucca/network_architectures/utils/model_memory_estimation.py
--rw-r--r--   0 zcr545     (501) staff       (20)      946 2024-03-22 16:50:24.000000 yucca-1.0.2/yucca/paths.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.046520 yucca-1.0.2/yucca/planning/
--rw-r--r--   0 zcr545     (501) staff       (20)      400 2024-02-21 14:52:45.000000 yucca-1.0.2/yucca/planning/ClassificationPlanner.py
--rw-r--r--   0 zcr545     (501) staff       (20)    12565 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/planning/YuccaPlanner.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-10-25 15:18:27.000000 yucca-1.0.2/yucca/planning/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)     6406 2024-03-11 14:50:22.000000 yucca-1.0.2/yucca/planning/dataset_properties.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.065341 yucca-1.0.2/yucca/planning/resampling/
--rw-r--r--   0 zcr545     (501) staff       (20)      646 2024-02-21 14:52:45.000000 yucca-1.0.2/yucca/planning/resampling/UnsupervisedPlannerUnitSpacing.py
--rw-r--r--   0 zcr545     (501) staff       (20)      650 2024-02-29 09:54:15.000000 yucca-1.0.2/yucca/planning/resampling/YuccaPlanner_1_1_1.py
--rw-r--r--   0 zcr545     (501) staff       (20)      612 2024-02-21 14:52:45.000000 yucca-1.0.2/yucca/planning/resampling/YuccaPlanner_1_1_125.py
--rw-r--r--   0 zcr545     (501) staff       (20)      586 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/planning/resampling/YuccaPlanner_224x224.py
--rw-r--r--   0 zcr545     (501) staff       (20)      659 2024-03-11 14:50:22.000000 yucca-1.0.2/yucca/planning/resampling/YuccaPlanner_MaxSize.py
--rw-r--r--   0 zcr545     (501) staff       (20)      395 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/planning/resampling/YuccaPlanner_NoResample.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/planning/resampling/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.078775 yucca-1.0.2/yucca/preprocessing/
--rw-r--r--   0 zcr545     (501) staff       (20)     1896 2024-03-05 12:40:35.000000 yucca-1.0.2/yucca/preprocessing/ClassificationPreprocessor.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2282 2024-02-19 12:41:30.000000 yucca-1.0.2/yucca/preprocessing/UnsupervisedPreprocessor.py
--rw-r--r--   0 zcr545     (501) staff       (20)    31622 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/preprocessing/YuccaPreprocessor.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-10-26 08:42:49.000000 yucca-1.0.2/yucca/preprocessing/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2533 2024-02-19 13:22:39.000000 yucca-1.0.2/yucca/preprocessing/normalization.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.111336 yucca-1.0.2/yucca/run/
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-10-25 15:18:27.000000 yucca-1.0.2/yucca/run/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1026 2024-02-29 09:54:15.000000 yucca-1.0.2/yucca/run/run_ensemble.py
--rw-r--r--   0 zcr545     (501) staff       (20)     5678 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/run/run_evaluation.py
--rw-r--r--   0 zcr545     (501) staff       (20)     6420 2024-03-05 10:59:10.000000 yucca-1.0.2/yucca/run/run_finetune.py
--rw-r--r--   0 zcr545     (501) staff       (20)     8068 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/run/run_inference.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2606 2024-02-21 14:52:45.000000 yucca-1.0.2/yucca/run/run_preprocessing.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1061 2023-12-04 09:50:07.000000 yucca-1.0.2/yucca/run/run_task_conversion.py
--rw-r--r--   0 zcr545     (501) staff       (20)     6652 2024-03-05 10:59:10.000000 yucca-1.0.2/yucca/run/run_training.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.268923 yucca-1.0.2/yucca/task_conversion/
--rw-r--r--   0 zcr545     (501) staff       (20)     2667 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/task_conversion/Task000_TEST_CLASSIFICATION.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2897 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/task_conversion/Task000_TEST_SEGMENTATION.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2327 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/task_conversion/Task000_TEST_UNSUPERVISED.py
--rw-r--r--   0 zcr545     (501) staff       (20)     3714 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/task_conversion/Task001_OASIS.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2764 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/task_conversion/Task002_LPBA40.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2841 2024-01-05 15:33:05.000000 yucca-1.0.2/yucca/task_conversion/Task003_Hammers.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2711 2024-02-19 12:41:30.000000 yucca-1.0.2/yucca/task_conversion/Task004_HarP.py
--rw-r--r--   0 zcr545     (501) staff       (20)     3711 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/task_conversion/Task005_ISLES22.py
--rw-r--r--   0 zcr545     (501) staff       (20)     5357 2024-01-26 09:22:50.000000 yucca-1.0.2/yucca/task_conversion/Task006_WMH_Flair.py
--rw-r--r--   0 zcr545     (501) staff       (20)     5334 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/task_conversion/Task007_WMH_T1.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4463 2024-02-29 09:54:15.000000 yucca-1.0.2/yucca/task_conversion/Task008_WMH.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2718 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/task_conversion/Task010_AMOS22.py
--rw-r--r--   0 zcr545     (501) staff       (20)     5369 2024-03-11 14:50:22.000000 yucca-1.0.2/yucca/task_conversion/Task011_MSSEG1.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4585 2024-03-11 14:50:22.000000 yucca-1.0.2/yucca/task_conversion/Task012_BraTS21.py
--rw-r--r--   0 zcr545     (501) staff       (20)     5366 2024-02-21 14:52:45.000000 yucca-1.0.2/yucca/task_conversion/Task021_Decathlon_BrainTumour.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4582 2024-02-21 14:52:45.000000 yucca-1.0.2/yucca/task_conversion/Task023_Decathlon_Liver.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4616 2024-03-11 14:50:22.000000 yucca-1.0.2/yucca/task_conversion/Task028_Decathlon_HepaticVessel.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1570 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/task_conversion/Task100_combine_001_002.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2951 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/task_conversion/Task201_PPMI.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2099 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/task_conversion/Task202_ISLES22.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2811 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/task_conversion/Task203_OASIS3.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2631 2024-02-15 09:14:02.000000 yucca-1.0.2/yucca/task_conversion/Task204_OASIS4.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2046 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/task_conversion/Task205_Hippocampus.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2312 2024-02-21 14:52:45.000000 yucca-1.0.2/yucca/task_conversion/Task206_BrainTumour.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2899 2024-02-19 12:41:30.000000 yucca-1.0.2/yucca/task_conversion/Task207_ADNI.py
--rw-r--r--   0 zcr545     (501) staff       (20)     3659 2024-02-15 09:14:04.000000 yucca-1.0.2/yucca/task_conversion/Task208_WMH.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1877 2024-03-13 08:34:20.000000 yucca-1.0.2/yucca/task_conversion/Task209_BraTS21.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2081 2024-03-13 08:34:20.000000 yucca-1.0.2/yucca/task_conversion/Task210_MSSEG1.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1383 2024-02-19 12:41:30.000000 yucca-1.0.2/yucca/task_conversion/Task241_BR41NS.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1446 2024-03-13 08:34:20.000000 yucca-1.0.2/yucca/task_conversion/Task245_BRAINS-45K.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1231 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/task_conversion/Task298_Combine_supervised.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1295 2024-02-19 12:41:30.000000 yucca-1.0.2/yucca/task_conversion/Task299_Combine.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2748 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/task_conversion/Task501_FetalPlanesDB.py
--rw-r--r--   0 zcr545     (501) staff       (20)     3599 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/task_conversion/Task502_tiny_imagenet_200.py
--rw-r--r--   0 zcr545     (501) staff       (20)     3245 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/task_conversion/Task701_OASIS_NoLabel.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2447 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/task_conversion/Task901_SONAI_NoLabel.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2476 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/task_conversion/Task902_SONAI100k_NoLabel.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-10-26 08:07:59.000000 yucca-1.0.2/yucca/task_conversion/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)     3396 2023-11-25 21:17:51.000000 yucca-1.0.2/yucca/task_conversion/template.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1413 2023-11-25 21:17:51.000000 yucca-1.0.2/yucca/task_conversion/template_combine_imagesTr.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2709 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/task_conversion/template_multiprocessing.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4763 2024-02-21 14:52:58.000000 yucca-1.0.2/yucca/task_conversion/utils.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.269443 yucca-1.0.2/yucca/training/
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/training/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.275881 yucca-1.0.2/yucca/training/augmentation/
--rw-r--r--   0 zcr545     (501) staff       (20)    13278 2024-03-22 17:22:59.000000 yucca-1.0.2/yucca/training/augmentation/YuccaAugmentationComposer.py
--rw-r--r--   0 zcr545     (501) staff       (20)        1 2024-03-05 10:59:10.000000 yucca-1.0.2/yucca/training/augmentation/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1692 2024-03-22 17:22:59.000000 yucca-1.0.2/yucca/training/augmentation/augmentation_presets.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.303387 yucca-1.0.2/yucca/training/configuration/
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:07:31.000000 yucca-1.0.2/yucca/training/configuration/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)     6618 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/training/configuration/configure_callbacks.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4960 2024-03-05 10:59:10.000000 yucca-1.0.2/yucca/training/configuration/configure_checkpoint.py
--rw-r--r--   0 zcr545     (501) staff       (20)     5782 2024-03-12 12:24:34.000000 yucca-1.0.2/yucca/training/configuration/configure_input_dims.py
--rw-r--r--   0 zcr545     (501) staff       (20)     2444 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/training/configuration/configure_paths.py
--rw-r--r--   0 zcr545     (501) staff       (20)     3109 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/training/configuration/configure_plans.py
--rw-r--r--   0 zcr545     (501) staff       (20)      933 2024-02-29 09:54:15.000000 yucca-1.0.2/yucca/training/configuration/configure_seed.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1847 2024-02-06 14:53:36.000000 yucca-1.0.2/yucca/training/configuration/configure_task.py
--rw-r--r--   0 zcr545     (501) staff       (20)     3570 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/training/configuration/split_data.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.316796 yucca-1.0.2/yucca/training/data_loading/
--rw-r--r--   0 zcr545     (501) staff       (20)     8094 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/training/data_loading/YuccaDataModule.py
--rw-r--r--   0 zcr545     (501) staff       (20)     7139 2024-03-21 12:23:07.000000 yucca-1.0.2/yucca/training/data_loading/YuccaDataset.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/training/data_loading/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1174 2023-11-15 09:40:14.000000 yucca-1.0.2/yucca/training/data_loading/samplers.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.321283 yucca-1.0.2/yucca/training/lightning_modules/
--rw-r--r--   0 zcr545     (501) staff       (20)    18128 2024-03-21 12:23:07.000000 yucca-1.0.2/yucca/training/lightning_modules/YuccaLightningModule.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-18 12:58:40.000000 yucca-1.0.2/yucca/training/lightning_modules/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.321825 yucca-1.0.2/yucca/training/loss_and_optim/
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/training/loss_and_optim/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.494283 yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/
--rw-r--r--   0 zcr545     (501) staff       (20)      419 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/CE.py
--rw-r--r--   0 zcr545     (501) staff       (20)      327 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/MSE.py
--rw-r--r--   0 zcr545     (501) staff       (20)      585 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/NLL.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)      886 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/deep_supervision.py
--rw-r--r--   0 zcr545     (501) staff       (20)     5682 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/hierarchical_losses.py
--rw-r--r--   0 zcr545     (501) staff       (20)     5594 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/nnUNet_losses.py
--rw-r--r--   0 zcr545     (501) staff       (20)     9620 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/unified_focal_loss.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.494960 yucca-1.0.2/yucca/training/loss_and_optim/optimizers/
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/training/loss_and_optim/optimizers/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.495465 yucca-1.0.2/yucca/training/loss_and_optim/schedulers/
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/training/loss_and_optim/schedulers/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.500319 yucca-1.0.2/yucca/training/loss_and_optim/utils/
--rw-r--r--   0 zcr545     (501) staff       (20)     2434 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/training/loss_and_optim/utils/LossTree.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/training/loss_and_optim/utils/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.505980 yucca-1.0.2/yucca/training/managers/
--rw-r--r--   0 zcr545     (501) staff       (20)    14557 2024-03-22 17:22:59.000000 yucca-1.0.2/yucca/training/managers/YuccaManager.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-18 12:58:40.000000 yucca-1.0.2/yucca/training/managers/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.513221 yucca-1.0.2/yucca/training/managers/alternative_managers/
--rw-r--r--   0 zcr545     (501) staff       (20)      309 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/training/managers/alternative_managers/YuccaManager_NoPatches.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1377 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/training/managers/alternative_managers/YuccaManager_PatchSizeMax.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/training/managers/alternative_managers/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.528253 yucca-1.0.2/yucca/training/managers/augmentation/
--rw-r--r--   0 zcr545     (501) staff       (20)      309 2024-03-21 12:23:07.000000 yucca-1.0.2/yucca/training/managers/augmentation/YuccaManager_AllAlways.py
--rw-r--r--   0 zcr545     (501) staff       (20)      366 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/training/managers/augmentation/YuccaManager_BiasField.py
--rw-r--r--   0 zcr545     (501) staff       (20)      371 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/training/managers/augmentation/YuccaManager_Ghosting.py
--rw-r--r--   0 zcr545     (501) staff       (20)      368 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/training/managers/augmentation/YuccaManager_Ringing.py
--rw-r--r--   0 zcr545     (501) staff       (20)      651 2024-01-26 09:22:50.000000 yucca-1.0.2/yucca/training/managers/augmentation/YuccaManager_SpatialOnly.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-18 12:58:40.000000 yucca-1.0.2/yucca/training/managers/augmentation/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.533243 yucca-1.0.2/yucca/training/managers/epochs/
--rw-r--r--   0 zcr545     (501) staff       (20)      839 2023-12-18 12:58:40.000000 yucca-1.0.2/yucca/training/managers/epochs/YuccaManager_1epoch.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-18 12:58:40.000000 yucca-1.0.2/yucca/training/managers/epochs/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.538291 yucca-1.0.2/yucca/training/managers/losses/
--rw-r--r--   0 zcr545     (501) staff       (20)      608 2023-12-18 12:58:40.000000 yucca-1.0.2/yucca/training/managers/losses/YuccaManager_CE.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1722 2023-12-18 12:58:40.000000 yucca-1.0.2/yucca/training/managers/losses/YuccaManager_DS.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-18 12:58:40.000000 yucca-1.0.2/yucca/training/managers/losses/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.542156 yucca-1.0.2/yucca/training/managers/lr/
--rw-r--r--   0 zcr545     (501) staff       (20)      219 2024-02-06 14:22:56.000000 yucca-1.0.2/yucca/training/managers/lr/YuccaManager_1e5.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-18 12:58:40.000000 yucca-1.0.2/yucca/training/managers/lr/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.544836 yucca-1.0.2/yucca/training/managers/optimizers/
--rw-r--r--   0 zcr545     (501) staff       (20)      244 2023-12-18 12:58:40.000000 yucca-1.0.2/yucca/training/managers/optimizers/YuccaManager_AdamW.py
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-12-18 12:58:40.000000 yucca-1.0.2/yucca/training/managers/optimizers/__init__.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.571936 yucca-1.0.2/yucca/utils/
--rw-r--r--   0 zcr545     (501) staff       (20)        0 2023-10-26 08:06:57.000000 yucca-1.0.2/yucca/utils/__init__.py
--rw-r--r--   0 zcr545     (501) staff       (20)      159 2024-01-04 14:18:49.000000 yucca-1.0.2/yucca/utils/dict.py
--rw-r--r--   0 zcr545     (501) staff       (20)     4525 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/utils/files_and_folders.py
--rw-r--r--   0 zcr545     (501) staff       (20)      281 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/utils/kwargs.py
--rw-r--r--   0 zcr545     (501) staff       (20)      735 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/utils/loading.py
--rw-r--r--   0 zcr545     (501) staff       (20)      967 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/utils/nib_utils.py
--rw-r--r--   0 zcr545     (501) staff       (20)     3742 2024-03-12 09:16:24.000000 yucca-1.0.2/yucca/utils/saving.py
--rw-r--r--   0 zcr545     (501) staff       (20)      222 2023-12-14 13:38:41.000000 yucca-1.0.2/yucca/utils/softmax.py
--rw-r--r--   0 zcr545     (501) staff       (20)      877 2023-12-04 09:50:07.000000 yucca-1.0.2/yucca/utils/task_ids.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1114 2024-03-18 17:16:12.000000 yucca-1.0.2/yucca/utils/torch_utils.py
--rw-r--r--   0 zcr545     (501) staff       (20)     1927 2024-01-23 10:04:44.000000 yucca-1.0.2/yucca/utils/type_conversions.py
-drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-03-22 18:08:57.572705 yucca-1.0.2/yucca.egg-info/
--rw-r--r--   0 zcr545     (501) staff       (20)    16019 2024-03-22 18:08:56.000000 yucca-1.0.2/yucca.egg-info/PKG-INFO
--rw-r--r--   0 zcr545     (501) staff       (20)     8761 2024-03-22 18:08:56.000000 yucca-1.0.2/yucca.egg-info/SOURCES.txt
--rw-r--r--   0 zcr545     (501) staff       (20)        1 2024-03-22 18:08:56.000000 yucca-1.0.2/yucca.egg-info/dependency_links.txt
--rw-r--r--   0 zcr545     (501) staff       (20)      354 2024-03-22 18:08:56.000000 yucca-1.0.2/yucca.egg-info/entry_points.txt
--rw-r--r--   0 zcr545     (501) staff       (20)      426 2024-03-22 18:08:56.000000 yucca-1.0.2/yucca.egg-info/requires.txt
--rw-r--r--   0 zcr545     (501) staff       (20)        6 2024-03-22 18:08:56.000000 yucca-1.0.2/yucca.egg-info/top_level.txt
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.410392 yucca-1.1.2/
+-rw-r--r--   0 zcr545     (501) staff       (20)    11357 2023-10-26 08:30:20.000000 yucca-1.1.2/LICENSE
+-rw-r--r--   0 zcr545     (501) staff       (20)    16020 2024-05-27 09:37:22.410191 yucca-1.1.2/PKG-INFO
+-rw-r--r--   0 zcr545     (501) staff       (20)    14366 2024-03-22 17:22:59.000000 yucca-1.1.2/README.md
+-rw-r--r--   0 zcr545     (501) staff       (20)     2039 2024-05-12 17:17:16.000000 yucca-1.1.2/pyproject.toml
+-rw-r--r--   0 zcr545     (501) staff       (20)      127 2024-05-27 09:37:22.411307 yucca-1.1.2/setup.cfg
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.274402 yucca-1.1.2/tests/
+-rw-r--r--   0 zcr545     (501) staff       (20)     2570 2024-05-07 13:44:52.000000 yucca-1.1.2/tests/test_configurations.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     4314 2024-05-07 13:44:48.000000 yucca-1.1.2/tests/test_end_to_end.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      342 2024-05-07 13:44:52.000000 yucca-1.1.2/tests/test_infinite_random_batch_sampler.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      188 2024-05-07 13:44:52.000000 yucca-1.1.2/tests/test_manager.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      108 2023-11-15 09:40:14.000000 yucca-1.1.2/tests/test_paths.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.276749 yucca-1.1.2/yucca/
+-rw-r--r--   0 zcr545     (501) staff       (20)       59 2024-02-06 14:22:56.000000 yucca-1.1.2/yucca/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.283175 yucca-1.1.2/yucca/callbacks/
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/callbacks/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     4894 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/callbacks/loggers.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1063 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/callbacks/prediction_writer.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.284197 yucca-1.1.2/yucca/data/
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.285556 yucca-1.1.2/yucca/data/augmentation/
+-rw-r--r--   0 zcr545     (501) staff       (20)    15393 2024-05-23 13:54:58.000000 yucca-1.1.2/yucca/data/augmentation/YuccaAugmentationComposer.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        1 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2887 2024-05-23 13:54:58.000000 yucca-1.1.2/yucca/data/augmentation/augmentation_presets.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.295090 yucca-1.1.2/yucca/data/augmentation/transforms/
+-rw-r--r--   0 zcr545     (501) staff       (20)     1400 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/BiasField.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1663 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/Blur.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3071 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/Gamma.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2063 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/Ghosting.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5309 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/Masking.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2437 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/Mirror.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3670 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/Noise.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1748 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/Ringing.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2369 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/SimulateLowres.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     4951 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/Spatial.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1577 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/YuccaTransform.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1007 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/copy_image_to_label.py
+-rw-r--r--   0 zcr545     (501) staff       (20)    12640 2024-05-13 14:37:06.000000 yucca-1.1.2/yucca/data/augmentation/transforms/cropping_and_padding.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5464 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/formatting.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1731 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/normalize.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      964 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/augmentation/transforms/sampling.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.296309 yucca-1.1.2/yucca/data/data_modules/
+-rw-r--r--   0 zcr545     (501) staff       (20)     8994 2024-05-15 17:06:10.000000 yucca-1.1.2/yucca/data/data_modules/YuccaDataModule.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        1 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/data_modules/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.297798 yucca-1.1.2/yucca/data/datasets/
+-rw-r--r--   0 zcr545     (501) staff       (20)      541 2024-05-12 17:17:16.000000 yucca-1.1.2/yucca/data/datasets/YuccaCompressedDataset.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     8089 2024-05-13 13:26:56.000000 yucca-1.1.2/yucca/data/datasets/YuccaDataset.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        1 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/data/datasets/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.298704 yucca-1.1.2/yucca/data/datasets/alternative_datasets/
+-rw-r--r--   0 zcr545     (501) staff       (20)     1114 2024-05-12 17:17:16.000000 yucca-1.1.2/yucca/data/datasets/alternative_datasets/YuccaDataset_1modality.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-12 17:17:16.000000 yucca-1.1.2/yucca/data/datasets/alternative_datasets/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1174 2024-05-13 14:37:06.000000 yucca-1.1.2/yucca/data/samplers.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.300941 yucca-1.1.2/yucca/functional/
+-rw-r--r--   0 zcr545     (501) staff       (20)      749 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.304991 yucca-1.1.2/yucca/functional/array_operations/
+-rw-r--r--   0 zcr545     (501) staff       (20)      665 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/array_operations/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      773 2024-05-13 14:37:06.000000 yucca-1.1.2/yucca/functional/array_operations/bounding_boxes.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2300 2024-05-13 14:37:06.000000 yucca-1.1.2/yucca/functional/array_operations/cropping_and_padding.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      583 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/array_operations/filtering.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2287 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/array_operations/matrix_ops.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2845 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/array_operations/normalization.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      563 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/array_operations/transpose.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.307850 yucca-1.1.2/yucca/functional/evaluation/
+-rw-r--r--   0 zcr545     (501) staff       (20)      488 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/evaluation/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1028 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/evaluation/confusion_matrix.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.309009 yucca-1.1.2/yucca/functional/evaluation/deepmind_surface_distance/
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/evaluation/deepmind_surface_distance/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)    22423 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/evaluation/deepmind_surface_distance/lookup_tables.py
+-rw-r--r--   0 zcr545     (501) staff       (20)    18475 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/evaluation/deepmind_surface_distance/metrics.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3619 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/evaluation/metrics.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3048 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/evaluation/obj_metrics.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      950 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/evaluation/surface_metrics.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3535 2024-05-13 14:37:06.000000 yucca-1.1.2/yucca/functional/planning.py
+-rw-r--r--   0 zcr545     (501) staff       (20)    21141 2024-05-16 07:43:47.000000 yucca-1.1.2/yucca/functional/preprocessing.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.309429 yucca-1.1.2/yucca/functional/testing/
+-rw-r--r--   0 zcr545     (501) staff       (20)      184 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/testing/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.311391 yucca-1.1.2/yucca/functional/testing/data/
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/testing/data/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      986 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/testing/data/array.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      958 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/testing/data/nifti.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/testing/data/tensor.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.315988 yucca-1.1.2/yucca/functional/transforms/
+-rw-r--r--   0 zcr545     (501) staff       (20)      587 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/transforms/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1134 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/transforms/bias_field.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      319 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/transforms/blur.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1721 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/transforms/gamma.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      860 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/transforms/masking.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1210 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/transforms/motion_ghosting.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      665 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/transforms/noise.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2390 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/transforms/ringing.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1466 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/transforms/sampling.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3739 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/transforms/spatial.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.321740 yucca-1.1.2/yucca/functional/utils/
+-rw-r--r--   0 zcr545     (501) staff       (20)      787 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/utils/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      159 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/utils/dict.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5588 2024-05-12 17:17:16.000000 yucca-1.1.2/yucca/functional/utils/files_and_folders.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      281 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/utils/kwargs.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      735 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/utils/loading.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      967 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/utils/nib_utils.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2841 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/utils/saving.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      222 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/utils/softmax.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1114 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/utils/torch_utils.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1927 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/utils/type_conversions.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.323075 yucca-1.1.2/yucca/functional/visualization/
+-rw-r--r--   0 zcr545     (501) staff       (20)       81 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/visualization/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2504 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/functional/visualization/imshow.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.324048 yucca-1.1.2/yucca/lightning_modules/
+-rw-r--r--   0 zcr545     (501) staff       (20)    16486 2024-05-23 13:54:58.000000 yucca-1.1.2/yucca/lightning_modules/YuccaLightningModule.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/lightning_modules/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.325362 yucca-1.1.2/yucca/metrics/
+-rw-r--r--   0 zcr545     (501) staff       (20)     2046 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/metrics/BoundingBox.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/metrics/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1416 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/metrics/training_metrics.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.325931 yucca-1.1.2/yucca/networks/
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.327833 yucca-1.1.2/yucca/networks/blocks_and_layers/
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/blocks_and_layers/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)    23654 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/blocks_and_layers/conv_blocks.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     4875 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/blocks_and_layers/conv_layers.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1243 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/blocks_and_layers/norm.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.333986 yucca-1.1.2/yucca/networks/networks/
+-rw-r--r--   0 zcr545     (501) staff       (20)     3638 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/networks/DeepLabHeadV3Plus.py
+-rw-r--r--   0 zcr545     (501) staff       (20)    30823 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/networks/MedNeXt.py
+-rw-r--r--   0 zcr545     (501) staff       (20)    11329 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/networks/MultiResUNet.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     4894 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/networks/TinyUNet.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     7846 2024-05-21 11:49:30.000000 yucca-1.1.2/yucca/networks/networks/UNet.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     9313 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/networks/UNetR.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     7554 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/networks/UNetRE.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     6762 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/networks/UXNet.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5283 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/networks/YuccaNet.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/networks/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     4848 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/networks/resnet.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.335453 yucca-1.1.2/yucca/networks/utils/
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/utils/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1068 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/networks/utils/get_steps_for_sliding_window.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     9416 2024-05-10 09:16:43.000000 yucca-1.1.2/yucca/networks/utils/model_memory_estimation.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.337042 yucca-1.1.2/yucca/optimization/
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/optimization/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5649 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/optimization/hierarchical_losses.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.340710 yucca-1.1.2/yucca/optimization/loss_functions/
+-rw-r--r--   0 zcr545     (501) staff       (20)      419 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/optimization/loss_functions/CE.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      327 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/optimization/loss_functions/MSE.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      585 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/optimization/loss_functions/NLL.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/optimization/loss_functions/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      888 2024-05-23 13:54:58.000000 yucca-1.1.2/yucca/optimization/loss_functions/deep_supervision.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5649 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/optimization/loss_functions/hierarchical_losses.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5582 2024-05-23 13:54:58.000000 yucca-1.1.2/yucca/optimization/loss_functions/nnUNet_losses.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     9620 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/optimization/loss_functions/unified_focal_loss.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.341539 yucca-1.1.2/yucca/optimization/optimizers/
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/optimization/optimizers/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.342034 yucca-1.1.2/yucca/optimization/schedulers/
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/optimization/schedulers/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.343263 yucca-1.1.2/yucca/optimization/utils/
+-rw-r--r--   0 zcr545     (501) staff       (20)     2434 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/optimization/utils/LossTree.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/optimization/utils/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      946 2024-03-22 16:50:24.000000 yucca-1.1.2/yucca/paths.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.343871 yucca-1.1.2/yucca/pipeline/
+-rw-r--r--   0 zcr545     (501) staff       (20)      263 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.347948 yucca-1.1.2/yucca/pipeline/configuration/
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/configuration/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     6632 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/configuration/configure_callbacks.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     4971 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/configuration/configure_checkpoint.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5769 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/configuration/configure_input_dims.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2444 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/configuration/configure_paths.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3775 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/configuration/configure_plans.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      933 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/configuration/configure_seed.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1847 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/configuration/configure_task.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3668 2024-05-12 17:17:16.000000 yucca-1.1.2/yucca/pipeline/configuration/split_data.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.348710 yucca-1.1.2/yucca/pipeline/evaluation/
+-rw-r--r--   0 zcr545     (501) staff       (20)    14229 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/evaluation/YuccaEvaluator.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/evaluation/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.349003 yucca-1.1.2/yucca/pipeline/evaluation/challenge_evaluation_scripts/
+-rw-r--r--   0 zcr545     (501) staff       (20)    10279 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/evaluation/challenge_evaluation_scripts/isles_eval.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.349433 yucca-1.1.2/yucca/pipeline/evaluation/challenge_preparation_scripts/
+-rw-r--r--   0 zcr545     (501) staff       (20)     3090 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/evaluation/challenge_preparation_scripts/prepare_decathlon.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.351015 yucca-1.1.2/yucca/pipeline/managers/
+-rw-r--r--   0 zcr545     (501) staff       (20)    15564 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/YuccaManager.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      328 2024-05-23 13:54:58.000000 yucca-1.1.2/yucca/pipeline/managers/YuccaManagerV2.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.352845 yucca-1.1.2/yucca/pipeline/managers/alternative_managers/
+-rw-r--r--   0 zcr545     (501) staff       (20)      297 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/alternative_managers/YuccaManager_NoPatches.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1377 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/alternative_managers/YuccaManager_PatchSizeMax.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/alternative_managers/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.358622 yucca-1.1.2/yucca/pipeline/managers/augmentation/
+-rw-r--r--   0 zcr545     (501) staff       (20)      305 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/augmentation/YuccaManager_AllAlways.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      362 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/augmentation/YuccaManager_BiasField.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      282 2024-05-12 17:17:16.000000 yucca-1.1.2/yucca/pipeline/managers/augmentation/YuccaManager_CT.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      367 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/augmentation/YuccaManager_Ghosting.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1029 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/augmentation/YuccaManager_PreserveRange.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      364 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/augmentation/YuccaManager_Ringing.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      651 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/augmentation/YuccaManager_SpatialOnly.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      760 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/augmentation/YuccaManager_Tester.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/augmentation/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.359931 yucca-1.1.2/yucca/pipeline/managers/dataloading/
+-rw-r--r--   0 zcr545     (501) staff       (20)      402 2024-05-12 17:17:16.000000 yucca-1.1.2/yucca/pipeline/managers/dataloading/YuccaManager_Compress.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      651 2024-05-12 17:17:16.000000 yucca-1.1.2/yucca/pipeline/managers/dataloading/YuccaManager_Only1Modality.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/dataloading/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.360600 yucca-1.1.2/yucca/pipeline/managers/epochs/
+-rw-r--r--   0 zcr545     (501) staff       (20)      839 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/epochs/YuccaManager_1epoch.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/epochs/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.361807 yucca-1.1.2/yucca/pipeline/managers/losses/
+-rw-r--r--   0 zcr545     (501) staff       (20)      597 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/losses/YuccaManager_CE.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1711 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/losses/YuccaManager_DS.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/losses/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.362903 yucca-1.1.2/yucca/pipeline/managers/lr/
+-rw-r--r--   0 zcr545     (501) staff       (20)      219 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/lr/YuccaManager_1e5.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/lr/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.363942 yucca-1.1.2/yucca/pipeline/managers/optimizers/
+-rw-r--r--   0 zcr545     (501) staff       (20)      244 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/optimizers/YuccaManager_AdamW.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/managers/optimizers/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.365831 yucca-1.1.2/yucca/pipeline/planning/
+-rw-r--r--   0 zcr545     (501) staff       (20)      409 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/planning/ClassificationPlanner.py
+-rw-r--r--   0 zcr545     (501) staff       (20)    12208 2024-05-12 17:17:16.000000 yucca-1.1.2/yucca/pipeline/planning/YuccaPlanner.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      263 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/planning/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.367565 yucca-1.1.2/yucca/pipeline/planning/alternative_planners/
+-rw-r--r--   0 zcr545     (501) staff       (20)      490 2024-05-12 17:17:16.000000 yucca-1.1.2/yucca/pipeline/planning/alternative_planners/YuccaPlanner_Compress.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      515 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/planning/alternative_planners/YuccaPlanner_MissingModalities.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      263 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/planning/alternative_planners/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     6439 2024-05-13 14:37:06.000000 yucca-1.1.2/yucca/pipeline/planning/dataset_properties.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.371369 yucca-1.1.2/yucca/pipeline/planning/resampling/
+-rw-r--r--   0 zcr545     (501) staff       (20)      655 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/planning/resampling/UnsupervisedPlannerUnitSpacing.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      659 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/planning/resampling/YuccaPlanner_1_1_1.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      621 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/planning/resampling/YuccaPlanner_1_1_125.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      594 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/planning/resampling/YuccaPlanner_224x224.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      668 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/planning/resampling/YuccaPlanner_MaxSize.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      591 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/planning/resampling/YuccaPlanner_NoResample.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/planning/resampling/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.373541 yucca-1.1.2/yucca/pipeline/preprocessing/
+-rw-r--r--   0 zcr545     (501) staff       (20)      636 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/preprocessing/ClassificationPreprocessor.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1179 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/preprocessing/UnsupervisedPreprocessor.py
+-rw-r--r--   0 zcr545     (501) staff       (20)    20246 2024-05-13 14:37:06.000000 yucca-1.1.2/yucca/pipeline/preprocessing/YuccaPreprocessor.py
+-rw-r--r--   0 zcr545     (501) staff       (20)      263 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/preprocessing/__init__.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.376962 yucca-1.1.2/yucca/pipeline/run/
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/run/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1037 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/run/run_ensemble.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5760 2024-05-10 09:16:43.000000 yucca-1.1.2/yucca/pipeline/run/run_evaluation.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     6447 2024-05-13 14:41:14.000000 yucca-1.1.2/yucca/pipeline/run/run_finetune.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     8159 2024-05-10 09:16:43.000000 yucca-1.1.2/yucca/pipeline/run/run_inference.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2754 2024-05-12 17:17:16.000000 yucca-1.1.2/yucca/pipeline/run/run_preprocessing.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1070 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/run/run_task_conversion.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     6957 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/run/run_training.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.408416 yucca-1.1.2/yucca/pipeline/task_conversion/
+-rw-r--r--   0 zcr545     (501) staff       (20)     2676 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task000_TEST_CLASSIFICATION.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2906 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task000_TEST_SEGMENTATION.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2336 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task000_TEST_UNSUPERVISED.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3723 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task001_OASIS.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2773 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task002_LPBA40.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2850 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task003_Hammers.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2720 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task004_HarP.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3720 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task005_ISLES22.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5366 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task006_WMH_Flair.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5343 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task007_WMH_T1.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     4472 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task008_WMH.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2727 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task010_AMOS22.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1765 2024-05-23 13:54:58.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task010_AMOS22TEST.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5378 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task011_MSSEG1.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     4630 2024-05-14 12:18:54.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task012_BraTS21.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3362 2024-05-12 17:17:16.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task013_AutoPET3.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2563 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task014_MBAS24.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2927 2024-05-10 09:16:43.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task015_AIMS-TBI24.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3775 2024-05-23 13:54:58.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task016_ACDC.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3266 2024-05-27 09:37:15.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task017_BTCV.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5380 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task021_Decathlon_BrainTumour.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     4594 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task023_Decathlon_Liver.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     4628 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task028_Decathlon_HepaticVessel.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3326 2024-05-14 12:18:54.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task040_BraTS21_flair.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3314 2024-05-14 12:18:54.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task041_BraTS21_t1.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3322 2024-05-14 12:18:54.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task042_BraTS21_t1ce.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3314 2024-05-14 12:18:54.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task043_BraTS21_t2.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1579 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task100_combine_001_002.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3415 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task201_PPMI.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2205 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task202_ISLES22.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2886 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task203_OASIS3.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2757 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task204_OASIS4.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2055 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task205_Hippocampus.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2375 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task206_BrainTumour.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3082 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task207_ADNI.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3668 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task208_WMH.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1886 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task209_BraTS21.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2090 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task210_MSSEG1.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1392 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task241_BR41NS.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1455 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task245_BRAINS-45K.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1240 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task298_Combine_supervised.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1304 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task299_Combine.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2757 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task501_FetalPlanesDB.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3608 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task502_tiny_imagenet_200.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3254 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task701_OASIS_NoLabel.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2456 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task901_SONAI_NoLabel.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2485 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task902_SONAI100k_NoLabel.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     4750 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/Task998_WMH_Dummy_Missing_Modalities.py
+-rw-r--r--   0 zcr545     (501) staff       (20)        0 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/__init__.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     3405 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/template.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     1422 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/template_combine_imagesTr.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     2718 2024-05-07 13:44:52.000000 yucca-1.1.2/yucca/pipeline/task_conversion/template_multiprocessing.py
+-rw-r--r--   0 zcr545     (501) staff       (20)     5671 2024-05-27 09:37:15.000000 yucca-1.1.2/yucca/pipeline/task_conversion/utils.py
+drwxr-xr-x   0 zcr545     (501) staff       (20)        0 2024-05-27 09:37:22.409066 yucca-1.1.2/yucca.egg-info/
+-rw-r--r--   0 zcr545     (501) staff       (20)    16020 2024-05-27 09:37:22.000000 yucca-1.1.2/yucca.egg-info/PKG-INFO
+-rw-r--r--   0 zcr545     (501) staff       (20)    11468 2024-05-27 09:37:22.000000 yucca-1.1.2/yucca.egg-info/SOURCES.txt
+-rw-r--r--   0 zcr545     (501) staff       (20)        1 2024-05-27 09:37:22.000000 yucca-1.1.2/yucca.egg-info/dependency_links.txt
+-rw-r--r--   0 zcr545     (501) staff       (20)      417 2024-05-27 09:37:22.000000 yucca-1.1.2/yucca.egg-info/entry_points.txt
+-rw-r--r--   0 zcr545     (501) staff       (20)      426 2024-05-27 09:37:22.000000 yucca-1.1.2/yucca.egg-info/requires.txt
+-rw-r--r--   0 zcr545     (501) staff       (20)        6 2024-05-27 09:37:22.000000 yucca-1.1.2/yucca.egg-info/top_level.txt
```

### Comparing `yucca-1.0.2/LICENSE` & `yucca-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/PKG-INFO` & `yucca-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: yucca
-Version: 1.0.2
+Version: 1.1.2
 Summary: The modern framework for sandbox experimentation and out-of-the box machine learning on medical data.
-Author-email: Sebastian Llambias <llambias@live.dk>, Asbjørn Munk <9844416+asbjrnmunk@users.noreply.github.com>, Jakob Ambsdorf <20045425+jakobamb@users.noreply.github.com>
+Author-email: Sebastian Llambias <llambias@live.com>, Asbjørn Munk <9844416+asbjrnmunk@users.noreply.github.com>, Jakob Ambsdorf <20045425+jakobamb@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/sllambias/yucca
 Project-URL: Bug Tracker, https://github.com/sllambias/yucca/issues
 Keywords: deep learning,image segmentation,medical image analysis,medical image segmentation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `yucca-1.0.2/README.md` & `yucca-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/pyproject.toml` & `yucca-1.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "yucca"
-version = "1.0.2"
+version = "1.1.2"
 authors = [
-  { name="Sebastian Llambias", email="llambias@live.dk" },
+  { name="Sebastian Llambias", email="llambias@live.com" },
   { name="Asbjørn Munk", email="9844416+asbjrnmunk@users.noreply.github.com" },
   { name="Jakob Ambsdorf", email="20045425+jakobamb@users.noreply.github.com" },
 ]
 description = "The modern framework for sandbox experimentation and out-of-the box machine learning on medical data."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -45,21 +45,21 @@
     'pytest>=7.3',
     'flake8>=6.1.0',
     'black>=23.10.1',
     'mypy>=1.6.0',
 ]
 
 [project.scripts]
-yucca_preprocess = 'yucca.run.run_preprocessing:main'
-yucca_train = 'yucca.run.run_training:main'
-yucca_inference = 'yucca.run.run_inference:main'
-yucca_evaluation = 'yucca.run.run_evaluation:main'
-yucca_finetune = 'yucca.run.run_finetune:main'
-yucca_convert_task = 'yucca.run.run_task_conversion:main'
-yucca_ensemble = 'yucca.run.run_ensemble:main'
+yucca_preprocess = 'yucca.pipeline.run.run_preprocessing:main'
+yucca_train = 'yucca.pipeline.run.run_training:main'
+yucca_inference = 'yucca.pipeline.run.run_inference:main'
+yucca_evaluation = 'yucca.pipeline.run.run_evaluation:main'
+yucca_finetune = 'yucca.pipeline.run.run_finetune:main'
+yucca_convert_task = 'yucca.pipeline.run.run_task_conversion:main'
+yucca_ensemble = 'yucca.pipeline.run.run_ensemble:main'
 
 [project.urls]
 "Homepage" = "https://github.com/sllambias/yucca"
 "Bug Tracker" = "https://github.com/sllambias/yucca/issues"
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
```

### Comparing `yucca-1.0.2/tests/test_configurations.py` & `yucca-1.1.2/tests/test_configurations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 def test_configurations(setup_preprocessed_segmentation_data):
-    from yucca.training.configuration.configure_callbacks import get_callback_config
-    from yucca.training.configuration.configure_paths import get_path_config
-    from yucca.training.configuration.configure_plans import get_plan_config
-    from yucca.training.configuration.configure_task import get_task_config
-    from yucca.training.configuration.configure_input_dims import get_input_dims_config
-    from yucca.training.configuration.split_data import get_split_config
-    from yucca.training.configuration.configure_checkpoint import get_checkpoint_config
-    from yucca.training.configuration.configure_seed import seed_everything_and_get_seed_config
+    from yucca.pipeline.configuration.configure_callbacks import get_callback_config
+    from yucca.pipeline.configuration.configure_paths import get_path_config
+    from yucca.pipeline.configuration.configure_plans import get_plan_config
+    from yucca.pipeline.configuration.configure_task import get_task_config
+    from yucca.pipeline.configuration.configure_input_dims import get_input_dims_config
+    from yucca.pipeline.configuration.split_data import get_split_config
+    from yucca.pipeline.configuration.configure_checkpoint import get_checkpoint_config
+    from yucca.pipeline.configuration.configure_seed import seed_everything_and_get_seed_config
 
+    # Random test
     task_config = get_task_config(task="Task000_TEST_SEGMENTATION")
     assert task_config is not None and isinstance(task_config.continue_from_most_recent, bool)
 
     path_config = get_path_config(task_config=task_config)
     assert path_config is not None and isinstance(path_config.version, int)
 
     ckpt_config = get_checkpoint_config(
```

### Comparing `yucca-1.0.2/tests/test_end_to_end.py` & `yucca-1.1.2/tests/test_end_to_end.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,16 @@
             "--train_batches_per_step",
             "1",
             "--val_batches_per_step",
             "1",
         ],
         check=True,
     )
+
+
 def test_finetune():
     from yucca.paths import yucca_models
 
     chk = os.path.join(
         yucca_models,
         "Task000_TEST_SEGMENTATION",
         "TinyUNet__3D",
```

### Comparing `yucca-1.0.2/yucca/deprecated/YuccaManager.py` & `yucca-1.1.2/yucca/pipeline/managers/YuccaManager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,351 +1,372 @@
+import lightning as L
 import torch
-import numpy as np
-import yucca
 import wandb
-from sklearn.model_selection import KFold
-from torch import optim
-from torch.cuda.amp import GradScaler
-from batchgenerators.utilities.file_and_folder_operations import (
-    join,
-    subfiles,
-    save_pickle,
-)
-from yucca.paths import yucca_preprocessed_data
-from yucca.training.trainers.base_manager import base_manager
-from yucca.evaluation.confusion_matrix import (
-    torch_confusion_matrix_from_logits,
-    torch_get_tp_fp_tn_fn,
-)
-from yucca.evaluation.metrics import dice_per_label
-from yucca.loss_and_optim.loss_functions.nnUNet_losses import DiceCE
-from yucca.utils.files_and_folders import recursive_find_python_class
-from yucca.utils.kwargs import filter_kwargs
+import logging
+from typing import Literal, Union, Optional
+from yucca.data.augmentation.YuccaAugmentationComposer import YuccaAugmentationComposer
+from yucca.pipeline.configuration.split_data import get_split_config, SplitConfig
+from yucca.pipeline.configuration.configure_task import get_task_config
+from yucca.pipeline.configuration.configure_callbacks import get_callback_config
+from yucca.pipeline.configuration.configure_checkpoint import get_checkpoint_config
+from yucca.pipeline.configuration.configure_seed import seed_everything_and_get_seed_config
+from yucca.pipeline.configuration.configure_paths import get_path_config
+from yucca.pipeline.configuration.configure_plans import get_plan_config
+from yucca.pipeline.configuration.configure_input_dims import get_input_dims_config
+from yucca.data.data_modules.YuccaDataModule import YuccaDataModule
+from yucca.data.datasets.YuccaDataset import YuccaTrainDataset, YuccaTestDataset
+from yucca.data.samplers import InfiniteRandomSampler
+from yucca.lightning_modules.YuccaLightningModule import YuccaLightningModule
+from yucca.paths import yucca_results
+from yucca.functional.utils.torch_utils import measure_FLOPs
+from fvcore.nn import flop_count_table
 
 
-class YuccaManager(base_manager):
+class YuccaManager:
     """
-    This is the barebone functional trainer of the pipeline.
+    The YuccaLightningManager class provides a convenient way to manage the training and inference processes in the Yucca project.
+    It encapsulates the configuration, setup, and execution steps, making it easier to conduct experiments and predictions with consistent settings.
 
-    When training is started it will call self.initialize(). This carries out the following steps:
-        - Loads the plans in the folder of the preprocessed training data
-        - Sets the required outpaths for saving model weights, training parameters and logs
-        - Sets the # epochs and # batches pr. epoch
-            - By default 1000 epochs of 250/50 train/val batches pr. epoch
-        - Sets the batch size and patch size
-          - Patch Size is automatically set based on the dataset.
-        - Defines the Data Augmentation scheme
-        - Initializes the network
-            - Input and output channels are derived from the # modalities and
-            # classes stored in the plans file of the dataset.
-        - Loads the data
-            - If no splits are provided it will automatically split the data.
-            - This initializes the data loaders and feeds them to the YuccaAugmenter
-        - Initializes the loss function, optimizer, learning rate, scheduler and scaler.
-        - Saves all these parameters in the defined outpath
-        - Initializes weights & biases
-    Then it starts training
-        - Using mixed precision
-        - Gradients are scaled and clipped.
-        - Augmentations are applied using the CPU while the forward - backward pass is handled
-        by the GPU to avoid IO bottlenecks
-        - On epoch start the start time is recorded and lists for losses etc. are created
-        - On epoch finish the end time is recorded and validation results are evaluated and uploaded
-        to both WANDB and the local training log. Finally the LR is updated according to any
-        scheduler.
-        - Model weights are stored every Xth (default 300) epoch AND whenever the model improves its historically
-        best Dice on the validation set.
-    After the last epoch the final model weights are saved and training is concluded.
+    The initialize method of the YuccaLightningManager class is responsible for setting up the necessary components for either training or inference.
+    This method performs the configuration of paths, creates data augmentation objects, and sets up the PyTorch Lightning modules (model and data module)
+    based on the specified stage in the pipeline. The stages can be "fit" (training), "test" (testing), or "predict" (inference).
+
+    It performs the following steps:
+        (1) Configure Paths: The YuccaConfigurator class is used to set up paths for training,
+        including the training data directory, output path, and plans file path.
+
+        (2) Create Augmentation Objects: The YuccaAugmentationComposer class is used to create data augmentation objects
+        (augmenter.train_transforms and augmenter.val_transforms) based on the specified patch size and model dimensionality.
+
+        (3) Set Up PyTorch Lightning Modules: The YuccaLightningModule class is initialized with the appropriate configuration
+        using the YuccaConfigurator object. This module is responsible for defining the neural network architecture, loss functions,
+        and optimization strategies.
+
+        (4) Set Up PyTorch Lightning Data Module: The YuccaDataModule class is initialized with the composed training and validation transforms,
+        along with the YuccaConfigurator object. This module handles the loading and preprocessing of the training, validation, and prediction datasets.
+
+        (5) Initialize PyTorch Lightning Trainer: The PyTorch Lightning Trainer is configured with the necessary settings, including callbacks,
+        output directory, precision, and other specified parameters.
     """
 
     def __init__(
         self,
-        model,
-        model_dimensions: str,
-        task: str,
-        folds: str | int,
-        planner: str,
-        starting_lr: float = None,
-        loss_fn: str = None,
-        momentum: float = None,
-        continue_training: bool = False,
-        checkpoint: str = None,
-        finetune: bool = False,
-        fast_training: bool = False,
+        ckpt_path: str = None,
+        continue_from_most_recent: bool = True,
+        deep_supervision: bool = False,
+        enable_logging: bool = True,
+        learning_rate: float = 1e-3,
+        loss: str = None,
+        max_epochs: int = 1000,
+        max_vram: int = 12,
+        model_dimensions: str = "3D",
+        model_name: str = "TinyUNet",
+        momentum: float = 0.9,
+        num_workers: Optional[int] = None,
+        batch_size: Union[int, Literal["tiny"]] = None,
+        patch_based_training: bool = True,
+        patch_size: Union[tuple, Literal["max", "min", "mean"]] = None,
+        augmentation_params: dict = {},
+        planner: str = "YuccaPlanner",
+        precision: str = "bf16-mixed",
+        profile: bool = False,
+        split_idx: int = 0,
+        split_data_method: str = "kfold",
+        split_data_param: int = 5,
+        step_logging: bool = False,
+        task: str = None,
+        experiment: str = "default",
+        train_batches_per_step: int = 250,
+        val_batches_per_step: int = 50,
+        **kwargs,
     ):
-        super().__init__()
-
-        # Trainer specific parameters
-        self._DEFAULT_STARTING_LR = 1e-3
-        self._DEFAULT_LOSS = DiceCE
-        self._DEFAULT_MOMENTUM = 0.9
-        self.batch_size_3D = 2
-        self.batch_size_2D = 64
-        self.train_batches_per_epoch = 250
-        self.val_batches_per_epoch = 50
-        self.name = self.__class__.__name__
-        self.optim = optim.SGD
-        self.lr_scheduler = optim.lr_scheduler.CosineAnnealingLR
-        self.final_epoch = 1000
-        self.p_force_foreground = 0.33
-        self.fast_final_epoch = 500
-        self.fast_train_batches_per_epoch = 100
-        self.fast_val_batches_per_epoch = 20
-        self.max_vram = 12
-
-        # REQUIRED:
-        # These must be defined in run_training
-        self.model_name = model
+        self.ckpt_path = ckpt_path
+        self.continue_from_most_recent = continue_from_most_recent
+        self.deep_supervision = deep_supervision
+        self.enable_logging = enable_logging
+        self.experiment = experiment
+        self.learning_rate = float(learning_rate)
+        self.loss = loss
+        self.max_epochs = max_epochs
+        self.max_vram = max_vram
         self.model_dimensions = model_dimensions
+        self.model_name = model_name
+        self.momentum = float(momentum)
+        self.name = self.__class__.__name__
+        self.num_workers = num_workers
+        self.augmentation_params = augmentation_params
+        self.batch_size = batch_size
+        self.patch_based_training = patch_based_training
+        self.patch_size = patch_size
+        self.planner = planner
+        self.precision = precision
+        self.profile = profile
+        self.split_idx = split_idx
+        self.split_data_method = split_data_method
+        self.split_data_param = split_data_param
+        self.step_logging = step_logging
         self.task = task
-        self.folds = int(folds)
-        self.plan_id = planner
-        self.continue_training = continue_training
-        self.checkpoint = checkpoint
-        self.fast_training = fast_training
-        self.finetune = finetune
-
-        # OPTIONALS:
-        # These can be defined in run_training
-        self.starting_lr = starting_lr
-        self.loss_fn = loss_fn
-        self.momentum = momentum
-
-        # The default is for the basic UNet.
-        self.patch_size_3D = (96, 96, 96)
-        self.patch_size_2D = (160, 160)
-        if self.model_name == "MultiResUNet":
-            self.patch_size_3D = (96, 96, 80)
-            self.patch_size_2D = (144, 144)
-
-        # kwargs that we set when params such as LR has been settled (do we use default or is it
-        # specified?)
-        self.loss_fn_kwargs = {}
-        self.optim_kwargs = {}
-        self.lr_scheduler_kwargs = {}
-
-    def comprehensive_eval(self, pred, seg):
-        if not self.epoch_eval_dict:
-            self.epoch_eval_dict = {
-                stat: []
-                for stat in [
-                    "Dice           :",
-                    "True Positives :",
-                    "False Positives:",
-                    "False Negatives:",
-                ]
-            }
-
-        confusion_matrix = torch_confusion_matrix_from_logits(pred, seg)
-        tp, fp, _, fn = torch_get_tp_fp_tn_fn(confusion_matrix, ignore_label=0)
-        self.epoch_eval_dict["Dice           :"].append(dice_per_label(tp, fp, _, fn))
-        self.epoch_eval_dict["True Positives :"].append(tp)
-        self.epoch_eval_dict["False Positives:"].append(fp)
-        self.epoch_eval_dict["False Negatives:"].append(fn)
-
-    def initialize(self):
-        if not self.is_initialized:
-            # Then we load the plans and set modalities and classes etc.
-            self.load_plans_from_path(
-                join(
-                    yucca_preprocessed_data,
-                    self.task,
-                    self.plan_id,
-                    self.plan_id + "_plans.json",
-                )
-            )
+        self.train_batches_per_step = train_batches_per_step
+        self.val_batches_per_step = val_batches_per_step
+        self.kwargs = kwargs
+
+        # Automatically changes bfloat training if we're running on a GPU
+        # that doesn't support it (otherwise it just crashes.)
+        if "bf" in self.precision and torch.cuda.is_available():
+            if not torch.cuda.is_bf16_supported():
+                self.precision = self.precision.replace("bf", "")
+
+        if self.kwargs.get("fast_dev_run"):
+            self.setup_fast_dev_run()
+
+        # defaults
+        self.trainer = L.Trainer
+        self.train_dataset_class = YuccaTrainDataset
+        self.test_dataset_class = YuccaTestDataset
 
-            # First we set the path based on the supplied parameters
-            self.set_outpath()
+    def initialize(
+        self,
+        stage: Literal["fit", "test", "predict"],
+        disable_tta: bool = False,
+        overwrite_predictions: bool = False,
+        pred_data_dir: str = None,
+        save_softmax: bool = False,
+        prediction_output_dir: str = "./",
+    ):
+        # Here we configure the outpath we will use to store model files and metadata
+        # along with the path to plans file which will also be loaded.
+        task_config = get_task_config(
+            task=self.task,
+            continue_from_most_recent=self.continue_from_most_recent,
+            manager_name=self.name,
+            model_dimensions=self.model_dimensions,
+            model_name=self.model_name,
+            patch_based_training=self.patch_based_training,
+            planner_name=self.planner,
+            experiment=self.experiment,
+            split_idx=self.split_idx,
+            split_data_method=self.split_data_method,
+            split_data_param=self.split_data_param,
+        )
 
-            # Now we can log the plan file, after the outpath has been created
-            self.log(f'{"plan file:":20}', self.plans_path, time=False)
+        path_config = get_path_config(task_config=task_config)
 
-            # Now we set up parameters for the data and the data augmentations
-            self.set_train_length()
-            self.set_batch_and_patch_sizes()
-            self.setup_DA()
-
-            # Load self.network based on the
-            # dimensions (2D or 3D) and classes (number of output channels)
-            self.initialize_network()
-            self.log(
-                f'{"network:":20}',
-                self.model_dimensions,
-                self.network.__class__.__name__,
-                time=False,
-            )
+        self.ckpt_config = get_checkpoint_config(
+            ckpt_path=self.ckpt_path,
+            continue_from_most_recent=task_config.continue_from_most_recent,
+            current_experiment=task_config.experiment,
+            path_config=path_config,
+        )
 
-            # Load the data (and if necessary split it)
-            # Before loading data, we set random seeds for reproducibility
-            self.load_data()
-
-            # Setup optimizer, learning rate, momentum etc.
-            self.initialize_loss_optim_lr()
-
-            # Before saving parameters and moving on to training
-            # check if we are using pretrained weights/continuing training
-            if self.continue_training:
-                if self.checkpoint:
-                    self.load_checkpoint(self.checkpoint, train=True)
-                else:
-                    latest = subfiles(self.outpath, suffix="latest.model", join=False)[0]
-                    assert latest, "Can not continue training. No latest checkpoint found."
-
-                    self.load_checkpoint(join(self.outpath, latest), train=True)
-
-            # And finally save a json with arguments and parameters
-            self.save_parameter_json()
-            self.initialize_wandb()
+        seed_config = seed_everything_and_get_seed_config(ckpt_seed=self.ckpt_config.ckpt_seed)
+
+        plan_config = self.get_plan_config(
+            ckpt_plans=self.ckpt_config.ckpt_plans,
+            plans_path=path_config.plans_path,
+            stage=stage,
+        )
 
-            self.log("initialization done, printing network", "\n", time=False)
-            self.log(self.network, time=False)
+        callback_config = get_callback_config(
+            save_dir=path_config.save_dir,
+            version_dir=path_config.version_dir,
+            ckpt_version_dir=self.ckpt_config.ckpt_version_dir,
+            ckpt_wandb_id=self.ckpt_config.ckpt_wandb_id,
+            experiment=task_config.experiment,
+            version=path_config.version,
+            enable_logging=self.enable_logging,
+            log_lr=True,
+            prediction_output_dir=prediction_output_dir,
+            profile=self.profile,
+            save_softmax=save_softmax,
+        )
 
-            self.is_initialized = True
+        if stage == "fit":
+            splits_config = get_split_config(task_config.split_method, task_config.split_param, path_config)
         else:
-            print(
-                "Network is already initialized. \
-                  Calling initialize repeatedly should be avoided."
-            )
+            splits_config = SplitConfig()
 
-    def initialize_loss_optim_lr(self):
-        # Define the gradscaler
-        self.grad_scaler = GradScaler(enabled=True)
-
-        # Defining the loss
-        if not self.loss_fn:
-            self.loss_fn = self._DEFAULT_LOSS
-
-        elif self.loss_fn:
-            self.loss_fn = recursive_find_python_class(
-                folder=[join(yucca.__path__[0], "training", "loss_functions")],
-                class_name=self.loss_fn,
-                current_module="yucca.training.loss_functions",
-            )
+        input_dims_config = get_input_dims_config(
+            plan=plan_config.plans,
+            model_dimensions=task_config.model_dimensions,
+            num_classes=plan_config.num_classes,
+            ckpt_patch_size=self.ckpt_config.ckpt_patch_size,
+            model_name=task_config.model_name,
+            max_vram=self.max_vram,
+            batch_size=self.batch_size,
+            patch_based_training=task_config.patch_based_training,
+            patch_size=self.patch_size,
+        )
+
+        augmenter = YuccaAugmentationComposer(
+            deep_supervision=self.deep_supervision,
+            patch_size=input_dims_config.patch_size,
+            is_2D=True if self.model_dimensions == "2D" else False,
+            parameter_dict=self.augmentation_params,
+            task_type_preset=plan_config.task_type,
+        )
+
+        self.model_module = YuccaLightningModule(
+            config=task_config.lm_hparams()
+            | path_config.lm_hparams()
+            | self.ckpt_config.lm_hparams()
+            | seed_config.lm_hparams()
+            | splits_config.lm_hparams()
+            | plan_config.lm_hparams()
+            | input_dims_config.lm_hparams()
+            | callback_config.lm_hparams()
+            | augmenter.lm_hparams(),
+            deep_supervision=self.deep_supervision,
+            learning_rate=self.learning_rate,
+            loss_fn=self.loss,
+            momentum=self.momentum,
+            step_logging=self.step_logging,
+            test_time_augmentation=not disable_tta if disable_tta is True else augmenter.mirror_p_per_sample > 0,
+        )
 
-        self.loss_fn_kwargs = {
-            "soft_dice_kwargs": {"apply_softmax": True},  # DCE
-            "hierarchical_kwargs": {"rootdict": self.plans["dataset_properties"]["label_hierarchy"]},  # Hierarchical Loss
-        }
-        self.loss_fn_kwargs = filter_kwargs(self.loss_fn, self.loss_fn_kwargs)
-        self.loss_fn = self.loss_fn(**self.loss_fn_kwargs)
-        assert isinstance(self.loss_fn, torch.nn.Module), (
-            "Loss is not a torch.nn.Module. " "Make sure the correct loss was found (check spelling)"
-        )
-
-        self.log(f'{"loss function":20}', self.loss_fn.__class__.__name__, time=False)
-
-        # Defining the learning rate
-        if not self.starting_lr:
-            self.starting_lr = self._DEFAULT_STARTING_LR
-        if self.finetune:
-            self.starting_lr /= 10
-        self.log(f'{"learning rate:":20}', self.starting_lr, time=False)
-
-        # Defining the momentum
-        if not self.momentum:
-            self.momentum = self._DEFAULT_MOMENTUM
-        self.log(f'{"momentum":20}', self.momentum, time=False)
-
-        # And constructing the optimizer
-        # Set kwargs for all optimizers and then filter relevant ones based on optimizer class
-
-        self.optim_kwargs = {
-            "lr": float(self.starting_lr),  # all
-            "momentum": float(self.momentum),  # SGD
-            "eps": 1e-4,
-            "weight_decay": 3e-5,
-        }
-        self.optim_kwargs = filter_kwargs(self.optim, self.optim_kwargs)
-        self.optim = self.optim(self.network.parameters(), **self.optim_kwargs)
-        self.log(f'{"optimizer":20}', self.optim.__class__.__name__, time=False)
-
-        # Set kwargs for all schedulers and then filter relevant ones based on scheduler class
-        self.lr_scheduler_kwargs = {
-            "T_max": self.final_epoch,
-            "eta_min": 1e-9,  # Cosine Annealing
-        }
-        self.lr_scheduler_kwargs = filter_kwargs(self.lr_scheduler, self.lr_scheduler_kwargs)
-        self.lr_scheduler = self.lr_scheduler(self.optim, **self.lr_scheduler_kwargs)
-        self.log(f'{"LR scheduler":20}', self.lr_scheduler.__class__.__name__, time=False)
+        self.data_module = YuccaDataModule(
+            allow_missing_modalities=plan_config.allow_missing_modalities,
+            composed_train_transforms=augmenter.train_transforms,
+            composed_val_transforms=augmenter.val_transforms,
+            image_extension=plan_config.image_extension,
+            input_dims_config=input_dims_config,
+            overwrite_predictions=overwrite_predictions,
+            num_workers=self.num_workers,
+            pred_data_dir=pred_data_dir,
+            pred_save_dir=prediction_output_dir,
+            pre_aug_patch_size=augmenter.pre_aug_patch_size,
+            splits_config=splits_config,
+            split_idx=task_config.split_idx,
+            task_type=plan_config.task_type,
+            test_dataset_class=self.test_dataset_class,
+            train_data_dir=path_config.train_data_dir,
+            train_dataset_class=self.train_dataset_class,
+        )
+
+        self.verify_modules_are_valid()
+        self.visualize_model_with_FLOPs(self.model_module, input_dims_config)
+
+        self.trainer = L.Trainer(
+            callbacks=callback_config.callbacks,
+            default_root_dir=path_config.save_dir,
+            limit_train_batches=self.train_batches_per_step,
+            limit_val_batches=self.val_batches_per_step,
+            log_every_n_steps=min(self.train_batches_per_step, 50),
+            logger=callback_config.loggers,
+            precision=self.precision,
+            profiler=callback_config.profiler,
+            enable_progress_bar=not self.enable_logging,
+            max_epochs=self.max_epochs,
+            **self.kwargs,
+        )
 
     def run_training(self):
-        self.initialize()
+        self.initialize(stage="fit")
+        self.trainer.fit(
+            model=self.model_module,
+            datamodule=self.data_module,
+            ckpt_path="last",
+        )
+        self.finish()
 
-        _ = self.tr_gen.next()
-        _ = self.val_gen.next()
+    def run_finetuning(self):
+        self.initialize(stage="fit")
+        self.model_module.load_state_dict(
+            state_dict=torch.load(self.ckpt_config.ckpt_path, map_location=torch.device("cpu"))["state_dict"], strict=False
+        )
+        self.trainer.fit(
+            model=self.model_module,
+            datamodule=self.data_module,
+        )
+        self.finish()
 
-        if torch.cuda.is_available():
-            torch.cuda.empty_cache()
-        else:
-            self.log(
-                "CUDA NOT AVAILABLE. YOU SHOULD REALLY NOT TRAIN WITHOUT CUDA!",
-                time=False,
-            )
+    def predict_folder(
+        self,
+        input_folder,
+        disable_tta: bool = False,
+        overwrite_predictions: bool = False,
+        output_folder: str = yucca_results,
+        save_softmax=False,
+    ):
+        self.batch_size = 1
+        self.initialize(
+            stage="predict",
+            disable_tta=disable_tta,
+            overwrite_predictions=overwrite_predictions,
+            pred_data_dir=input_folder,
+            prediction_output_dir=output_folder,
+            save_softmax=save_softmax,
+        )
+
+        self.trainer.predict(
+            model=self.model_module,
+            dataloaders=self.data_module,
+            ckpt_path=self.ckpt_config.ckpt_path,
+            return_predictions=False,
+        )
+        self.finish()
 
-        wandb.watch(self.network)
+    @staticmethod
+    def get_plan_config(ckpt_plans, plans_path, stage):
+        plan_config = get_plan_config(
+            ckpt_plans=ckpt_plans,
+            plans_path=plans_path,
+            stage=stage,
+        )
+        return plan_config
 
-        while self.current_epoch < self.final_epoch:
-            self.epoch_start()
+    def finish(self):
+        wandb.finish()
 
-            self.network.train()
-            for _ in range(self.train_batches_per_epoch):
-                batch_loss = self.run_batch(next(self.tr_gen))
-                self.epoch_tr_loss.append(batch_loss)
-
-            self.network.eval()
-            with torch.no_grad():
-                for _ in range(self.val_batches_per_epoch):
-                    batch_loss = self.run_batch(next(self.val_gen), train=False, comprehensive_eval=True)
-                    self.epoch_val_loss.append(batch_loss)
-
-            self.tr_losses.append(np.mean(self.epoch_tr_loss))
-            self.val_losses.append(np.mean(self.epoch_val_loss))
-
-            if self.lr_scheduler:
-                self.lr_scheduler.step()
-
-            self.epoch_finish()
-
-        if self.current_epoch == self.final_epoch:
-            self.save_checkpoint("checkpoint_final.model")
-            wandb.finish()
-
-    def setup_DA(self):
-        super().setup_DA()
-        self.AdditiveNoise_p_per_sample = 0.2
-        self.BiasField_p_per_sample = 0.33
-        self.Blurring_p_per_sample = 0.2
-        self.ElasticDeform_p_per_sample = 0.33
-        self.Gamma_p_per_sample = 0.2
-        self.GibbsRinging_p_per_sample = 0.2
-        self.Mirror_p_per_sample = 0.2
-        self.MotionGhosting_p_per_sample = 0.2
-        self.MultiplicativeNoise_p_per_sample = 0.2
-        self.Rotation_p_per_sample = 0.33
-        self.Scale_p_per_sample = 0.33
-        self.SimulateLowres_p_per_sample = 0.2
-
-    def split_data(self):
-        splits = []
-
-        files = subfiles(self.folder_with_preprocessed_data, join=False, suffix=".npy")
-        if not files:
-            files = subfiles(self.folder_with_preprocessed_data, join=False, suffix=".npz")
-            if files:
-                self.log(
-                    "Only found compressed (.npz) files. This might increase runtime.",
-                    time=False,
-                )
-
-        assert files, f"Couldn't find any .npy or .npz files in {self.folder_with_preprocessed_data}"
-
-        files = np.array(files)
-        # We set this seed manually as multiple trainers might use this split,
-        # And we may not know which individual seed dictated the data splits
-        # Therefore for reproducibility this is fixed.
-
-        kf = KFold(n_splits=5, shuffle=True, random_state=52189)
-        for train, val in kf.split(files):
-            splits.append({"train": list(files[train]), "val": list(files[val])})
+    def verify_modules_are_valid(self):
+        # Method to expand for additional verifications
+        self.verify_samplers_are_valid()
+
+    def verify_samplers_are_valid(self):
+        if (
+            not issubclass(self.data_module.train_sampler, InfiniteRandomSampler) and self.train_batches_per_step is not None
+        ) or (not issubclass(self.data_module.val_sampler, InfiniteRandomSampler) and self.val_batches_per_step is not None):
+            logging.info(
+                "Warning: you are limiting the amount of batches pr. step, but not sampling using InfiniteRandomSampler."
+            )
+
+    def visualize_model_with_FLOPs(self, lightning_module, input_dims_config):
+        flops = self.get_flops(
+            lightning_module, input_dims_config.batch_size, input_dims_config.num_modalities, input_dims_config.patch_size
+        )
+        logging.info("\n" + flop_count_table(flops))
 
-        save_pickle(splits, self.splits_file)
+    @staticmethod
+    def get_flops(lightning_module, batch_size, modalities, patch_size):
+        data = torch.randn((batch_size, modalities, *patch_size))
+        flops = measure_FLOPs(lightning_module.model, data)
+        return flops
+
+    def setup_fast_dev_run(self):
+        self.batch_size = 2
+        self.patch_size = (32, 32)
+        self.enable_logging = False
+        self.model_dimensions = "2D"
+        self.precision = 32
+        self.kwargs["accelerator"] = "cpu"
+        self.train_batches_per_step = 10
+        self.val_batches_per_step = 5
+
+
+if __name__ == "__main__":
+    # path = "/home/zcr545/YuccaData/yucca_models/Task001_OASIS/UNet__3D/YuccaPlanner/YuccaLightningManager/0/2023_11_08_15_19_14/checkpoints/test_ckpt.ckpt"
+    path = None
+    Manager = YuccaManager(
+        disable_logging=False,
+        ckpt_path=path,
+        model_name="TinyUNet",
+        model_dimensions="2D",
+        num_workers=0,
+        split_idx=0,
+        step_logging=True,
+        task="Task001_OASIS",
+    )
+    Manager.initialize("fit")
+    # Manager.run_training()
+    # Manager.predict_folder(
+    #    input_folder="/home/zcr545/YuccaData/yucca_raw_data/Task001_OASIS/imagesTs",
+    #    output_folder="/home/zcr545/YuccaData/yucca_predictions",
+    # )
```

### Comparing `yucca-1.0.2/yucca/deprecated/run_training_OLD.py` & `yucca-1.1.2/yucca/pipeline/run/run_evaluation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,159 +1,149 @@
+"""
+This script can be used in two ways:
+1. You can specify the paths to the folder containing predictions and labels/ground truth
+using "--pred" and "--gt" and define the labels of interest using e.g. "-c 0 1"
+
+2. You can specify the task, trainer and planner like it's also done in other yucca_ scripts.
+if "-t" for target task is left blank, we assume you are predicting and evaluating data
+from the same task as the one the model is trained on.
+"""
+
 import argparse
-import yucca
-from yucca.utils.task_ids import maybe_get_task_from_task_id
-from yucca.utils.files_and_folders import recursive_find_python_class
-from batchgenerators.utilities.file_and_folder_operations import join
+from batchgenerators.utilities.file_and_folder_operations import load_json, join
+from yucca.pipeline.evaluation.YuccaEvaluator import YuccaEvaluator
+from yucca.pipeline.task_conversion.utils import maybe_get_task_from_task_id
+from yucca.paths import yucca_raw_data, yucca_results
 
 
 def main():
     parser = argparse.ArgumentParser()
 
-    # Required Arguments #
+    parser.add_argument(
+        "-s",
+        help="Name of the source task i.e. what the model is trained on. " "Should be of format: TaskXXX_MYTASK",
+        required=False,
+    )
     parser.add_argument(
         "-t",
-        "--task",
-        help="Name of the task used for training. "
-        "The data should already be preprocessed using yucca_preprocess"
-        "Argument should be of format: TaskXXX_MYTASK",
+        help="Name of the target task i.e. the data to be predicted. " "Should be of format: TaskXXX_MYTASK",
+        required=False,
+    )
+    parser.add_argument("-m", help="Model Architecture. Defaults to UNet.", default="UNet")
+    parser.add_argument("-d", help="2D, 25D or 3D model. Defaults to 3D.", default="3D")
+    parser.add_argument(
+        "-man",
+        help="Full name of Manager Class. \n" "e.g. 'YuccaTrainer_DCE' or 'YuccaTrainer'. Defaults to YuccaTrainer.",
+        default="YuccaManager",
     )
+    parser.add_argument("-pl", help="Plan ID. Defaults to YuccaPlanner", default="YuccaPlanner")
+    parser.add_argument("-chk", help="Checkpoint used for inference. Defaults to best.", default="best")
+    parser.add_argument("-c", nargs="*", help="Classes to include for evaluation", type=str)
+
+    # Alternatively, these can be used to manually specify paths
+    parser.add_argument("--pred", help="manually specify path to predicted segmentations", default=None, required=False)
+    parser.add_argument("--gt", help="manually specify path to ground truth", default=None, required=False)
 
-    # Optional arguments with default values #
+    # Optionals (infrequently changed)
     parser.add_argument(
-        "-m",
-        help="Model Architecture. Should be one of MultiResUNet or UNet"
-        " Note that this is case sensitive. "
-        "Defaults to the standard UNet.",
-        default="UNet",
+        "--task_type",
+        default="segmentation",
+        type=str,
+        required=False,
+        help="Defaults to segmentation. Set to 'classification' for classification tasks.",
     )
     parser.add_argument(
-        "-d",
-        help="Dimensionality of the Model. Can be 3D or 2D. "
-        "Defaults to 3D. Note that this will always be 2D if ensemble is enabled.",
+        "--as_binary", help="run evaluation as if data was binary", action="store_true", default=None, required=False
     )
-    parser.add_argument("-tr", help="Trainer Class to be used. " "Defaults to the basic YuccaTrainer", default="YuccaTrainer")
     parser.add_argument(
-        "-pl",
-        help="Plan ID to be used. "
-        "This specifies which plan and preprocessed data to use for training "
-        "on the given task. Defaults to the YuccaPlanne folder",
-        default="YuccaPlanner",
+        "--experiment",
+        help="A name for the experiment being performed, with no spaces.",
+        default="default",
     )
     parser.add_argument(
-        "-f",
-        help="Fold to use for training. Unless manually assigned, "
-        "folds [0,1,2,3,4] will be created automatically. "
-        "Defaults to training on fold 0",
-        default=0,
+        "--no_wandb",
+        help="Disable logging of evaluation results to wandb",
+        default=False,
+        action="store_true",
+        required=False,
     )
+    parser.add_argument("--obj_eval", help="enable object evaluation", action="store_true", default=None, required=False)
     parser.add_argument(
-        "--ensemble",
-        help="Used to train ensemble/2.5D models. Will run 3 consecutive trainings.",
+        "--overwrite",
         default=False,
         action="store_true",
+        required=False,
+        help="Overwrite existing predictions",
     )
+    parser.add_argument("--split_idx", type=int, help="idx of splits to use for training.", default=0)
     parser.add_argument(
-        "--fast", help="Used to speed up training, possibly at the expense of performance", default=False, action="store_true"
+        "--split_data_method", help="Specify splitting method. Either kfold, simple_train_val_split", default="kfold"
     )
-
-    # The following can be changed to run training with alternative LR, Loss and/or Momentum ###
     parser.add_argument(
-        "--lr",
-        help="Should only be used to employ alternative Learning Rate. " "Format should be scientific notation e.g. 1e-4.",
-        default=None,
+        "--split_data_param",
+        help="Specify the parameter for the selected split method. For KFold use an int, for simple_split use a float between 0.0-1.0.",
+        default=5,
     )
-    parser.add_argument("--loss", help="Should only be used to employ alternative Loss Function", default=None)
-    parser.add_argument("--mom", help="Should only be used to employ alternative Momentum.", default=None)
+    parser.add_argument("--surface_eval", help="enable surface evaluation", action="store_true", default=None, required=False)
 
-    # Only touch the following if you know what you're doing #
     parser.add_argument(
-        "--continue_train", help="continue training a previously saved checkpoint. ", action="store_true", default=False
+        "--version", "-v", help="version number of the model. Defaults to 0.", default=0, type=int, required=False
     )
-    # parser.add_argument("--chk", help="used to specify checkpoint to continue training from "
-    #                    "when --continue_train is supplied. "
-    #                    "The default is the latest model.", default='latest')
-    # parser.add_argument("--threads", help="number of threads/processes", default=2)
-
     args = parser.parse_args()
 
-    task = maybe_get_task_from_task_id(args.task)
+    source_task = maybe_get_task_from_task_id(args.s)
+    target_task = maybe_get_task_from_task_id(args.t)
+    manager_name = args.man
     model = args.m
     dimensions = args.d
-    trainer_name = args.tr
-    plans = args.pl
-    split_idx = args.f
-    ensemble = args.ensemble
-    fast_training = args.fast
-    lr = args.lr
-    loss = args.loss
-    momentum = args.mom
-    continue_training = args.continue_train
-    # threads = args.threads
-    # checkpoint = args.chk
-
-    assert model in [
-        "MedNeXt",
-        "MultiResUNet",
-        "UNet",
-        "UNetR",
-        "UXNet",
-        "ResNet50",
-    ], f"{model} is an invalid model name. This is case sensitive."
-
-    if lr:
-        assert "e" in lr, f"Learning Rate should be in scientific notation e.g. 1e-4, but is {lr}"
-
-    if not ensemble:
-        trainer = recursive_find_python_class(
-            folder=[join(yucca.__path__[0], "training", "trainers")],
-            class_name=trainer_name,
-            current_module="yucca.training.trainers",
+    plan_id = args.pl
+    checkpoint = args.chk
+    obj = args.obj_eval
+    overwrite = args.overwrite
+    as_binary = args.as_binary
+    classes = args.c
+    predpath = args.pred
+    gtpath = args.gt
+    experiment = args.experiment
+    num_version = args.version
+    task_type = args.task_type
+    use_wandb = not args.no_wandb
+    split_idx = args.split_idx
+    split_data_method = args.split_data_method
+    split_data_param = args.split_data_param
+    surface_eval = args.surface_eval
+    assert (predpath and gtpath) or source_task, "Either supply BOTH paths or the source task"
+
+    if not predpath:
+        if not target_task:
+            target_task = source_task
+
+        predpath = join(  # TODO: Extract this into a function
+            yucca_results,
+            target_task,
+            source_task,
+            model + "__" + dimensions,
+            manager_name + "__" + plan_id,
+            experiment,
+            f"{split_data_method}_{split_data_param}_fold_{split_idx}",
+            "version_" + str(num_version),
+            checkpoint,
         )
-        trainer = trainer(
-            model=model,
-            model_dimensions=dimensions,
-            task=task,
-            split_idx=split_idx,
-            plan_id=plans,
-            starting_lr=lr,
-            loss_fn=loss,
-            momentum=momentum,
-            continue_training=continue_training,
-            fast_training=fast_training,
-        )
-
-        command_used = "yucca_train " + " ".join(f"-{k} {v}" for k, v in vars(args).items())
-        trainer.set_train_command(command_used)
+        gtpath = join(yucca_raw_data, target_task, "labelsTs")
+        classes = list(load_json(join(yucca_raw_data, target_task, "dataset.json"))["labels"].keys())
 
-        trainer.run_training()
-    if ensemble:
-        print("Starting ensemble training. Model dimensions will automatically be set to 2D.")
-        dimensions = "2D"
-        views = ["X", "Y", "Z"]
-        for view in views:
-            trainer = recursive_find_python_class(
-                split_idx=[join(yucca.__path__[0], "training", "trainers")],
-                class_name=trainer_name,
-                current_module="yucca.training.trainers",
-            )
-            plan_and_view = plans + view
-            trainer = trainer(
-                model=model,
-                model_dimensions=dimensions,
-                task=task,
-                split_idx=split_idx,
-                plan_id=plan_and_view,
-                starting_lr=lr,
-                loss_fn=loss,
-                momentum=momentum,
-                continue_training=continue_training,
-                fast_training=fast_training,
-            )
-
-            command_used = "yucca_train " + " ".join(f"-{k} {v}" for k, v in vars(args).items())
-            trainer.set_train_command(command_used)
-
-            trainer.run_training()
+    evaluator = YuccaEvaluator(
+        classes,
+        folder_with_predictions=predpath,
+        folder_with_ground_truth=gtpath,
+        do_object_eval=obj,
+        do_surface_eval=surface_eval,
+        overwrite=overwrite,
+        as_binary=as_binary,
+        task_type=task_type,
+        use_wandb=use_wandb,
+    )
+    evaluator.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `yucca-1.0.2/yucca/evaluation/YuccaEvaluator.py` & `yucca-1.1.2/yucca/pipeline/evaluation/YuccaEvaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import numpy as np
 import nibabel as nib
 import json
 import sys
 import wandb
 from batchgenerators.utilities.file_and_folder_operations import subfiles, join, load_json, isfile
 from sklearn.metrics import confusion_matrix
-from yucca.evaluation.metrics import (
+from yucca.functional.evaluation.metrics import (
     dice,
     jaccard,
     sensitivity,
     precision,
     TP,
     FP,
     FN,
     total_pos_gt,
     total_pos_pred,
     volume_similarity,
     accuracy,
     auroc,
 )
-from yucca.evaluation.obj_metrics import get_obj_stats_for_label
-from yucca.evaluation.surface_metrics import get_surface_metrics_for_label
+from yucca.functional.evaluation.obj_metrics import get_obj_stats_for_label
+from yucca.functional.evaluation.surface_metrics import get_surface_metrics_for_label
 from yucca.paths import yucca_raw_data
 from weave.monitoring import StreamTable
 from tqdm import tqdm
 
 
 class YuccaEvaluator(object):
     def __init__(
```

### Comparing `yucca-1.0.2/yucca/evaluation/challenge_evaluation_scripts/isles_eval.py` & `yucca-1.1.2/yucca/pipeline/evaluation/challenge_evaluation_scripts/isles_eval.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/evaluation/challenge_preparation_scripts/prepare_decathlon.py` & `yucca-1.1.2/yucca/pipeline/evaluation/challenge_preparation_scripts/prepare_decathlon.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/evaluation/confusion_matrix.py` & `yucca-1.1.2/yucca/functional/evaluation/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/evaluation/deepmind_surface_distance/lookup_tables.py` & `yucca-1.1.2/yucca/functional/evaluation/deepmind_surface_distance/lookup_tables.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/evaluation/deepmind_surface_distance/metrics.py` & `yucca-1.1.2/yucca/functional/evaluation/deepmind_surface_distance/metrics.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/evaluation/loggers.py` & `yucca-1.1.2/yucca/callbacks/loggers.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/evaluation/metrics.py` & `yucca-1.1.2/yucca/functional/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/evaluation/obj_metrics.py` & `yucca-1.1.2/yucca/functional/evaluation/obj_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import cc3d
-from yucca.utils.nib_utils import get_nib_spacing
-from yucca.evaluation.metrics import sensitivity, precision, f1
+from yucca.functional.utils.nib_utils import get_nib_spacing
+from yucca.functional.evaluation.metrics import sensitivity, precision, f1
 
 
 def get_obj_stats_for_label(gt, pred, label, as_binary=False):
     spacing = get_nib_spacing(gt)
     gt = np.around(gt.get_fdata())
     pred = np.around(pred.get_fdata())
     if as_binary:
```

### Comparing `yucca-1.0.2/yucca/evaluation/surface_metrics.py` & `yucca-1.1.2/yucca/functional/evaluation/surface_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-from yucca.utils.nib_utils import get_nib_spacing
-from yucca.evaluation.deepmind_surface_distance import metrics
+from yucca.functional.utils.nib_utils import get_nib_spacing
+from yucca.functional.evaluation.deepmind_surface_distance import metrics
 
 
 def get_surface_metrics_for_label(gt, pred, label, as_binary: bool = False):
     spacing = get_nib_spacing(pred)
     pred = pred.get_fdata()
     gt = gt.get_fdata()
     labeldict = {}
```

### Comparing `yucca-1.0.2/yucca/image_processing/cropping_and_padding.py` & `yucca-1.1.2/yucca/functional/array_operations/cropping_and_padding.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/image_processing/matrix_ops.py` & `yucca-1.1.2/yucca/functional/array_operations/matrix_ops.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/image_processing/objects/BoundingBox.py` & `yucca-1.1.2/yucca/metrics/BoundingBox.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Fri Dec 16 13:25:09 2022
 
 @author: zcr545
 """
-from copy import deepcopy
-import numpy as np
-
-
-def get_bbox_for_foreground(array, background_label=0):
-    array = deepcopy(array)
-    array[array != background_label] = 1
-    return get_bbox_for_label(array, label=1)
-
-
-def get_bbox_for_label(array, label, padding=0):
-    a = np.where(array == label)
-
-    x1, x2, y1, y2 = np.min(a[0]), np.max(a[0]), np.min(a[1]), np.max(a[1])
-
-    xmin = min(x1, x2) - padding
-    xmax = max(x1, x2) + padding
-
-    ymin = min(y1, y2) - padding
-    ymax = max(y1, y2) + padding
-
-    if len(array.shape) == 3:
-        z1, z2 = np.min(a[2]), np.max(a[2])
-
-        zmin = min(z1, z2) - padding
-        zmax = max(z1, z2) + padding
-
-        return [xmin, xmax + 1, ymin, ymax + 1, zmin, zmax + 1]
-
-    return [xmin, xmax + 1, ymin, ymax + 1]
+from yucca.functional.array_operations.bounding_boxes import get_bbox_for_label
 
 
 class Box(object):
     def __init__(self, array, label, padding):
         # Create bounding box for the object.
         self.array = array
         self.label = label
```

### Comparing `yucca-1.0.2/yucca/image_processing/objects/filtering.py` & `yucca-1.1.2/yucca/functional/array_operations/filtering.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/image_processing/transforms/Blur.py` & `yucca-1.1.2/yucca/data/augmentation/transforms/SimulateLowres.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,57 @@
-from yucca.image_processing.transforms.YuccaTransform import YuccaTransform
+from yucca.data.augmentation.transforms.YuccaTransform import YuccaTransform
+from yucca.functional.transforms import simulate_lowres
 import numpy as np
-from typing import Tuple
-from scipy.ndimage import gaussian_filter
 
 
-class Blur(YuccaTransform):
-    def __init__(self, data_key="image", p_per_sample=1, p_per_channel=0.5, sigma=(0.5, 1.0)):
+class SimulateLowres(YuccaTransform):
+    def __init__(
+        self,
+        data_key="image",
+        p_per_sample: float = 1.0,
+        p_per_channel: float = 0.5,
+        p_per_axis: float = 0.33,
+        zoom_range=(0.5, 1.0),
+        clip_to_input_range=False,
+    ):
         self.data_key = data_key
         self.p_per_sample = p_per_sample
         self.p_per_channel = p_per_channel
-        self.sigma = sigma
+        self.p_per_axis = p_per_axis
+        self.zoom_range = zoom_range
+        self.clip_to_input_range = clip_to_input_range
 
     @staticmethod
-    def get_params(sigma: Tuple[float]):
-        sigma = np.random.uniform(*sigma)
-        return sigma
-
-    def __blur__(self, imageVolume, sigma):
-        for c in range(imageVolume.shape[0]):
-            if np.random.uniform() < self.p_per_channel:
-                imageVolume[c] = gaussian_filter(imageVolume[c], sigma, order=0)
-        return imageVolume
+    def get_params(zoom_range, shape, p_per_axis):
+        # No parameters to retrieve
+        if isinstance(shape, (list, tuple)):
+            shape = np.array(shape)
+        zoom = np.random.uniform(*zoom_range)
+        dim = len(shape)
+        zoomed_shape = np.round(shape * zoom).astype(int)
+        for i in range(dim):
+            if np.random.uniform() < p_per_axis:
+                shape[i] = zoomed_shape[i]
+        return shape
+
+    def __simulatelowres__(self, image, target_shape):
+        image = simulate_lowres(image, target_shape=target_shape, clip_to_input_range=self.clip_to_input_range)
+        return image
 
     def __call__(self, packed_data_dict=None, **unpacked_data_dict):
         data_dict = packed_data_dict if packed_data_dict else unpacked_data_dict
         assert (
             len(data_dict[self.data_key].shape) == 5 or len(data_dict[self.data_key].shape) == 4
         ), f"Incorrect data size or shape.\
             \nShould be (b, c, x, y, z) or (b, c, x, y) and is: {data_dict[self.data_key].shape}"
 
         for b in range(data_dict[self.data_key].shape[0]):
             if np.random.uniform() < self.p_per_sample:
-                sigma = self.get_params(self.sigma)
-                data_dict[self.data_key][b] = self.__blur__(data_dict[self.data_key][b], sigma)
+                for c in range(data_dict[self.data_key][b].shape[0]):
+                    if np.random.uniform() < self.p_per_channel:
+                        target_shape = self.get_params(
+                            self.zoom_range,
+                            data_dict[self.data_key][b, c].shape,
+                            self.p_per_axis,
+                        )
+                        data_dict[self.data_key][b, c] = self.__simulatelowres__(data_dict[self.data_key][b, c], target_shape)
         return data_dict
```

### Comparing `yucca-1.0.2/yucca/image_processing/transforms/CopyImageToSeg.py` & `yucca-1.1.2/yucca/data/augmentation/transforms/copy_image_to_label.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from yucca.image_processing.transforms.YuccaTransform import YuccaTransform
+from yucca.data.augmentation.transforms.YuccaTransform import YuccaTransform
 
 
-class CopyImageToSeg(YuccaTransform):
+class CopyImageToLabel(YuccaTransform):
     def __init__(self, copy=False, data_key="image", label_key="label"):
         self.copy = copy
         self.data_key = data_key
         self.label_key = label_key
 
     @staticmethod
     def get_params():
```

### Comparing `yucca-1.0.2/yucca/image_processing/transforms/Ghosting.py` & `yucca-1.1.2/yucca/data/augmentation/transforms/Ghosting.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,51 @@
-from yucca.image_processing.transforms.YuccaTransform import YuccaTransform
+from yucca.data.augmentation.transforms.YuccaTransform import YuccaTransform
+from yucca.functional.transforms import motion_ghosting
 import numpy as np
 from typing import Tuple
 
 
 class MotionGhosting(YuccaTransform):
     def __init__(
         self,
         data_key="image",
-        p_per_sample=1,
+        p_per_sample: float = 1.0,
         alpha=(0.85, 0.95),
-        numReps=(2, 5),
+        num_reps=(2, 5),
         axes=(0, 3),
+        clip_to_input_range=False,
     ):
         self.data_key = data_key
         self.p_per_sample = p_per_sample
         self.alpha = alpha
-        self.numReps = numReps
+        self.num_reps = num_reps
         self.axes = axes
+        self.clip_to_input_range = clip_to_input_range
 
     @staticmethod
-    def get_params(alpha: Tuple[float], numReps: Tuple[float], axes: Tuple[float]) -> Tuple[float]:
+    def get_params(alpha: Tuple[float], num_reps: Tuple[float], axes: Tuple[float]) -> Tuple[float]:
         alpha = np.random.uniform(*alpha)
-        numReps = np.random.randint(*numReps)
+        num_reps = np.random.randint(*num_reps)
         axis = np.random.randint(*axes)
-        return alpha, numReps, axis
+        return alpha, num_reps, axis
 
-    def __motionGhosting__(self, imageVolume, alpha, numReps, axis):
-        m = min(0, imageVolume.min())
-        imageVolume += abs(m)
-        if len(imageVolume.shape) == 3:
-            assert axis in [0, 1, 2], "Incorrect or no axis"
-
-            h, w, d = imageVolume.shape
-
-            imageVolume = np.fft.fftn(imageVolume, s=[h, w, d])
-
-            if axis == 0:
-                imageVolume[0:-1:numReps, :, :] = alpha * imageVolume[0:-1:numReps, :, :]
-            elif axis == 1:
-                imageVolume[:, 0:-1:numReps, :] = alpha * imageVolume[:, 0:-1:numReps, :]
-            else:
-                imageVolume[:, :, 0:-1:numReps] = alpha * imageVolume[:, :, 0:-1:numReps]
-
-            imageVolume = abs(np.fft.ifftn(imageVolume, s=[h, w, d]))
-        if len(imageVolume.shape) == 2:
-            assert axis in [0, 1], "Incorrect or no axis"
-            h, w = imageVolume.shape
-            imageVolume = np.fft.fftn(imageVolume, s=[h, w])
-
-            if axis == 0:
-                imageVolume[0:-1:numReps, :] = alpha * imageVolume[0:-1:numReps, :]
-            else:
-                imageVolume[:, 0:-1:numReps] = alpha * imageVolume[:, 0:-1:numReps]
-            imageVolume = abs(np.fft.ifftn(imageVolume, s=[h, w]))
-        imageVolume -= m
-        return imageVolume
+    def __motionGhosting__(self, image, alpha, num_reps, axis):
+        image = motion_ghosting(
+            image=image, alpha=alpha, num_reps=num_reps, axis=axis, clip_to_input_range=self.clip_to_input_range
+        )
+        return image
 
     def __call__(self, packed_data_dict=None, **unpacked_data_dict):
         data_dict = packed_data_dict if packed_data_dict else unpacked_data_dict
         assert (
             len(data_dict[self.data_key].shape) == 5 or len(data_dict[self.data_key].shape) == 4
         ), f"Incorrect data size or shape.\
             \nShould be (b, c, x, y, z) or (b, c, x, y) and is: {data_dict[self.data_key].shape}"
 
         for b in range(data_dict[self.data_key].shape[0]):
             for c in range(data_dict[self.data_key][b].shape[0]):
                 if np.random.uniform() < self.p_per_sample:
-                    alpha, numReps, axis = self.get_params(self.alpha, self.numReps, self.axes)
+                    alpha, num_reps, axis = self.get_params(self.alpha, self.num_reps, self.axes)
                     data_dict[self.data_key][b, c] = self.__motionGhosting__(
-                        data_dict[self.data_key][b, c], alpha, numReps, axis
+                        data_dict[self.data_key][b, c], alpha, num_reps, axis
                     )
         return data_dict
```

### Comparing `yucca-1.0.2/yucca/image_processing/transforms/Masking.py` & `yucca-1.1.2/yucca/data/augmentation/transforms/Masking.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import logging
-from yucca.image_processing.transforms.YuccaTransform import YuccaTransform
+from yucca.data.augmentation.transforms.YuccaTransform import YuccaTransform
 from typing import Union, Iterable
+from yucca.functional.transforms import mask_batch
 
 
 class Masking(YuccaTransform):
     """
     A Yucca transform class for applying masking to input images or image volumes.
 
     It can be used for masking with a fixed ratio and fixed token size but it can also be used
@@ -72,31 +73,15 @@
                 logging.warn(
                     "token_size is set to a ratio over 0.25 of the image. " "This is not intended and should be reconsidered."
                 )
             token_size = [int(i * np.random.uniform(*token_size)) for i in input_shape]
         return pixel_value, ratio, token_size
 
     def __mask__(self, image_volume, pixel_value, ratio, token_size):
-        assert len(image_volume.shape[2:]) == len(token_size), (
-            "mask token size not compatible with input data"
-            f"mask token is: {token_size} and image is shape: {image_volume.shape[2:]}"
-        )
-        # np.ceil to get a grid with exact or larger dims than the input image
-        # later we will crop it to the desired dims
-        slices = [slice(0, shape) for shape in image_volume.shape[2:]]
-        grid_dims = np.ceil(image_volume.shape[2:] / np.array(token_size)).astype(np.uint8)
-
-        grid_flat = np.ones(np.prod(grid_dims))
-        grid_flat[: int(len(grid_flat) * ratio)] = 0
-        np.random.shuffle(grid_flat)
-        grid = grid_flat.reshape(grid_dims)
-        for idx, size in enumerate(token_size):
-            grid = np.repeat(grid, repeats=size, axis=idx)
-
-        image_volume[:, :, grid[*slices] == 0] = pixel_value
+        image_volume = mask_batch(batch=image_volume, pixel_value=pixel_value, ratio=ratio, token_size=token_size)
         return image_volume
 
     def __call__(self, packed_data_dict=None, **unpacked_data_dict):
         data_dict = packed_data_dict if packed_data_dict else unpacked_data_dict
         assert (
             len(data_dict[self.data_key].shape) == 5 or len(data_dict[self.data_key].shape) == 4
         ), f"Incorrect data size or shape.\
```

### Comparing `yucca-1.0.2/yucca/image_processing/transforms/Mirror.py` & `yucca-1.1.2/yucca/data/augmentation/transforms/Mirror.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from yucca.image_processing.transforms.YuccaTransform import YuccaTransform
+from yucca.data.augmentation.transforms.YuccaTransform import YuccaTransform
 import numpy as np
 
 
 class Mirror(YuccaTransform):
     def __init__(
         self,
         data_key="image",
         label_key="label",
-        p_per_sample=1,
+        p_per_sample: float = 1.0,
         axes=(0, 1, 2),
         p_mirror_per_axis=0.33,
         skip_label=False,
     ):
         self.data_key = data_key
         self.label_key = label_key
         self.p_per_sample = p_per_sample
```

### Comparing `yucca-1.0.2/yucca/image_processing/transforms/Noise.py` & `yucca-1.1.2/yucca/data/augmentation/transforms/Noise.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-from yucca.image_processing.transforms.YuccaTransform import YuccaTransform
+from yucca.data.augmentation.transforms.YuccaTransform import YuccaTransform
+from yucca.functional.transforms import additive_noise, multiplicative_noise
 import numpy as np
 from typing import Tuple
 
 
 class AdditiveNoise(YuccaTransform):
-    def __init__(self, data_key="image", p_per_sample=1, mean=(0.0, 0.0), sigma=(1e-3, 1e-4)):
+    def __init__(
+        self,
+        data_key="image",
+        p_per_sample: float = 1.0,
+        mean=(0.0, 0.0),
+        sigma=(1e-3, 1e-4),
+        clip_to_input_range=False,
+    ):
         self.data_key = data_key
         self.p_per_sample = p_per_sample
         self.mean = mean
         self.sigma = sigma
+        self.clip_to_input_range = clip_to_input_range
 
     @staticmethod
     def get_params(mean: Tuple[float], sigma: Tuple[float]) -> Tuple[float]:
         mean = float(np.random.uniform(*mean))
         sigma = float(np.random.uniform(*sigma))
         return mean, sigma
 
-    def __additiveNoise__(self, imageVolume, mean, sigma):
-        # J = I+n
-        gauss = np.random.normal(mean, sigma, imageVolume.shape)
-        return imageVolume + gauss
+    def __additiveNoise__(self, image, mean, sigma):
+        image = additive_noise(image=image, mean=mean, sigma=sigma, clip_to_input_range=self.clip_to_input_range)
+        return image
 
     def __call__(self, packed_data_dict=None, **unpacked_data_dict):
         data_dict = packed_data_dict if packed_data_dict else unpacked_data_dict
         assert (
             len(data_dict[self.data_key].shape) == 5 or len(data_dict[self.data_key].shape) == 4
         ), f"Incorrect data size or shape.\
             \nShould be (c, x, y, z) or (c, x, y) and is: {data_dict[self.data_key].shape}"
@@ -41,30 +49,37 @@
     variables in DIKU_3D_augmentation_params:
         do_multiplicativeNoise
         multiplicativeNoise_p_per_sample
         multiplicativeNoise_mean
         multiplicativeNoise_sigma
     """
 
-    def __init__(self, data_key="image", p_per_sample=1, mean=(0.0, 0.0), sigma=(1e-3, 1e-4)):
+    def __init__(
+        self,
+        data_key="image",
+        p_per_sample: float = 1.0,
+        mean=(0.0, 0.0),
+        sigma=(1e-3, 1e-4),
+        clip_to_input_range=False,
+    ):
         self.data_key = data_key
         self.p_per_sample = p_per_sample
         self.mean = mean
         self.sigma = sigma
+        self.clip_to_input_range = clip_to_input_range
 
     @staticmethod
     def get_params(mean: Tuple[float], sigma: Tuple[float]) -> Tuple[float]:
         mean = float(np.random.uniform(*mean))
         sigma = float(np.random.uniform(*sigma))
         return mean, sigma
 
-    def __multiplicativeNoise__(self, imageVolume, mean, sigma):
-        # J = I + I*n
-        gauss = np.random.normal(mean, sigma, imageVolume.shape)
-        return imageVolume + imageVolume * gauss
+    def __multiplicativeNoise__(self, image, mean, sigma):
+        image = multiplicative_noise(image=image, mean=mean, sigma=sigma, clip_to_input_range=self.clip_to_input_range)
+        return image
 
     def __call__(self, packed_data_dict=None, **unpacked_data_dict):
         data_dict = packed_data_dict if packed_data_dict else unpacked_data_dict
         assert (
             len(data_dict[self.data_key].shape) == 5 or len(data_dict[self.data_key].shape) == 4
         ), f"Incorrect data size or shape.\
             \nShould be (b, c, x, y, z) or (b, c, x, y) and is: {data_dict[self.data_key].shape}"
```

### Comparing `yucca-1.0.2/yucca/image_processing/transforms/SimulateLowres.py` & `yucca-1.1.2/yucca/data/augmentation/transforms/Gamma.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,71 @@
-from yucca.image_processing.transforms.YuccaTransform import YuccaTransform
+from yucca.data.augmentation.transforms.YuccaTransform import YuccaTransform
+from yucca.functional.transforms import augment_gamma
 import numpy as np
-from skimage.transform import resize
 
 
-class SimulateLowres(YuccaTransform):
+class Gamma(YuccaTransform):
+    """
+    WRAPPER FOR NNUNET AUGMENT GAMMA: https://github.com/MIC-DKFZ/batchgenerators/blob/8822a08a7dbfa4986db014e6a74b040778164ca6/batchgenerators/augmentations/color_augmentations.py
+
+    Augments by changing 'gamma' of the image (same as gamma correction in photos or computer monitors
+
+    :param gamma_range: range to sample gamma from. If one value is smaller than 1 and the other one is
+    larger then half the samples will have gamma <1 and the other >1 (in the inverval that was specified).
+    Tuple of float. If one value is < 1 and the other > 1 then half the images will be augmented with gamma values
+    smaller than 1 and the other half with > 1
+    :param invert_image: whether to invert the image before applying gamma augmentation
+    :param retain_stats: Gamma transformation will alter the mean and std of the data in the patch. If retain_stats=True,
+    the data will be transformed to match the mean and standard deviation before gamma augmentation. retain_stats
+    can also be callable (signature retain_stats() -> bool)
+    """
+
     def __init__(
         self,
         data_key="image",
-        p_per_sample=1,
-        p_per_channel=0.5,
-        p_per_axis=0.33,
-        zoom_range=(0.5, 1.0),
+        p_per_sample: float = 1.0,
+        p_invert_image: float = 0.05,
+        gamma_range=(0.5, 2.0),
+        per_channel=True,
+        clip_to_input_range=False,
     ):
         self.data_key = data_key
         self.p_per_sample = p_per_sample
-        self.p_per_channel = p_per_channel
-        self.p_per_axis = p_per_axis
-        self.zoom_range = zoom_range
+        self.gamma_range = gamma_range
+        self.p_invert_image = p_invert_image
+        self.per_channel = per_channel
+        self.clip_to_input_range = clip_to_input_range
 
     @staticmethod
-    def get_params(zoom_range, shape, p_per_axis):
+    def get_params(p_invert_image):
         # No parameters to retrieve
-        if isinstance(shape, (list, tuple)):
-            shape = np.array(shape)
-        zoom = np.random.uniform(*zoom_range)
-        dim = len(shape)
-        zoomed_shape = np.round(shape * zoom).astype(int)
-        for i in range(dim):
-            if np.random.uniform() < p_per_axis:
-                shape[i] = zoomed_shape[i]
-        return shape
-
-    def __simulatelowres__(self, imageVolume, target_shape):
-        shape = imageVolume.shape
-        downsampled = resize(
-            imageVolume.astype(float),
-            target_shape,
-            order=0,
-            mode="edge",
-            anti_aliasing=False,
+        do_invert = False
+        if np.random.uniform() < p_invert_image:
+            do_invert = True
+        return do_invert
+
+    def __gamma__(self, image, gamma_range, invert_image, per_channel):
+        return augment_gamma(
+            image,
+            gamma_range,
+            invert_image,
+            per_channel,
+            clip_to_input_range=self.clip_to_input_range,
         )
-        imageVolume = resize(downsampled, shape, order=3, mode="edge", anti_aliasing=False)
-        return imageVolume
 
     def __call__(self, packed_data_dict=None, **unpacked_data_dict):
         data_dict = packed_data_dict if packed_data_dict else unpacked_data_dict
         assert (
             len(data_dict[self.data_key].shape) == 5 or len(data_dict[self.data_key].shape) == 4
         ), f"Incorrect data size or shape.\
             \nShould be (b, c, x, y, z) or (b, c, x, y) and is: {data_dict[self.data_key].shape}"
 
         for b in range(data_dict[self.data_key].shape[0]):
             if np.random.uniform() < self.p_per_sample:
-                for c in range(data_dict[self.data_key][b].shape[0]):
-                    if np.random.uniform() < self.p_per_channel:
-                        target_shape = self.get_params(
-                            self.zoom_range,
-                            data_dict[self.data_key][b, c].shape,
-                            self.p_per_axis,
-                        )
-                        data_dict[self.data_key][b, c] = self.__simulatelowres__(data_dict[self.data_key][b, c], target_shape)
+                do_invert = self.get_params(self.p_invert_image)
+                data_dict[self.data_key][b] = self.__gamma__(
+                    data_dict[self.data_key][b],
+                    self.gamma_range,
+                    do_invert,
+                    per_channel=self.per_channel,
+                )
         return data_dict
```

### Comparing `yucca-1.0.2/yucca/image_processing/transforms/YuccaTransform.py` & `yucca-1.1.2/yucca/data/augmentation/transforms/YuccaTransform.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/image_processing/transforms/cropping_and_padding.py` & `yucca-1.1.2/yucca/data/augmentation/transforms/cropping_and_padding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from yucca.image_processing.transforms.YuccaTransform import YuccaTransform
+from yucca.data.augmentation.transforms.YuccaTransform import YuccaTransform
 from typing import Literal, Union
 
 
 class CropPad(YuccaTransform):
     def __init__(
         self,
         data_key="image",
```

### Comparing `yucca-1.0.2/yucca/image_processing/transforms/formatting.py` & `yucca-1.1.2/yucca/data/augmentation/transforms/formatting.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import torch
-from yucca.image_processing.transforms.YuccaTransform import YuccaTransform
+from yucca.data.augmentation.transforms.YuccaTransform import YuccaTransform
 from typing import Optional
 
 
 class RemoveSegChannelAxis(YuccaTransform):
     def __init__(self, label_key="label", channel_to_remove=1):
         self.label_key = label_key
         self.channel = channel_to_remove
@@ -117,7 +117,32 @@
             data_dict[self.label_key] = label
         return data_dict
 
     def __call__(self, packed_data_dict=None, **unpacked_data_dict):
         data_dict = packed_data_dict if packed_data_dict else unpacked_data_dict
         data_dict = self.__squeeze__(data_dict)
         return data_dict
+
+
+class CollectMetadata(YuccaTransform):
+    # Class to collect arbitrary metadata used in later transforms.
+    # Values here are collected BEFORE ANY augmentations are applied.
+    def __init__(self, data_key="image", label_key="label"):
+        self.data_key = data_key
+        self.label_key = label_key
+
+    @staticmethod
+    def get_params():
+        pass
+
+    def __collect__(self, data_dict):
+        metadata = {}
+        data = data_dict[self.data_key]
+        metadata["min"] = data.min()
+        metadata["max"] = data.max()
+        data_dict["metadata"] = metadata
+        return data_dict
+
+    def __call__(self, packed_data_dict=None, **unpacked_data_dict):
+        data_dict = packed_data_dict if packed_data_dict else unpacked_data_dict
+        data_dict = self.__collect__(data_dict)
+        return data_dict
```

### Comparing `yucca-1.0.2/yucca/image_processing/transforms/sampling.py` & `yucca-1.1.2/yucca/functional/transforms/sampling.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,45 @@
-from yucca.image_processing.transforms.YuccaTransform import YuccaTransform
 import numpy as np
 from skimage.transform import resize
 
 
-class DownsampleSegForDS(YuccaTransform):
-    """ """
-
-    def __init__(self, deep_supervision: bool = False, label_key="label", factors=(1, 0.5, 0.25, 0.125, 0.0625)):
-        self.deep_supervision = deep_supervision
-        self.label_key = label_key
-        self.factors = factors
-
-    @staticmethod
-    def get_params():
-        # No parameters to retrieve
-        pass
-
-    def __downsample__(self, label, factors):
-        orig_type = label.dtype
-        orig_shape = label.shape
-        downsampled_labels = []
-        for factor in factors:
-            target_shape = np.array(orig_shape).astype(int)
-            for i in range(2, len(orig_shape)):
-                target_shape[i] *= factor
-            if np.all(target_shape == orig_shape):
-                downsampled_labels.append(label)
-            else:
-                canvas = np.zeros(target_shape)
-                for b in range(label.shape[0]):
-                    for c in range(label[b].shape[0]):
-                        canvas[b, c] = resize(
-                            label[b, c].astype(float),
-                            target_shape[2:],
-                            0,
-                            mode="edge",
-                            clip=True,
-                            anti_aliasing=False,
-                        ).astype(orig_type)
-                downsampled_labels.append(canvas)
-        return downsampled_labels
-
-    def __call__(self, packed_data_dict=None, **unpacked_data_dict):
-        data_dict = packed_data_dict if packed_data_dict else unpacked_data_dict
-        if self.deep_supervision:
-            data_dict[self.label_key] = self.__downsample__(data_dict[self.label_key], self.factors)
-        return data_dict
+def downsample_label(label, factors):
+    orig_type = label.dtype
+    orig_shape = label.shape
+    downsampled_labels = []
+    for factor in factors:
+        target_shape = np.array(orig_shape).astype(int)
+        for i in range(2, len(orig_shape)):
+            target_shape[i] *= factor
+        if np.all(target_shape == orig_shape):
+            downsampled_labels.append(label)
+        else:
+            canvas = np.zeros(target_shape)
+            for b in range(label.shape[0]):
+                for c in range(label[b].shape[0]):
+                    canvas[b, c] = resize(
+                        label[b, c].astype(float),
+                        target_shape[2:],
+                        0,
+                        mode="edge",
+                        clip=True,
+                        anti_aliasing=False,
+                    ).astype(orig_type)
+            downsampled_labels.append(canvas)
+    return downsampled_labels
+
+
+def simulate_lowres(image, target_shape, clip_to_input_range):
+    img_min = image.min()
+    img_max = image.max()
+    shape = image.shape
+    downsampled = resize(
+        image.astype(float),
+        target_shape,
+        order=0,
+        mode="edge",
+        anti_aliasing=False,
+    )
+    image = resize(downsampled, shape, order=3, mode="edge", anti_aliasing=False)
+    if clip_to_input_range:
+        image = np.clip(image, a_min=img_min, a_max=img_max)
+    return image
```

### Comparing `yucca-1.0.2/yucca/network_architectures/blocks_and_layers/conv_blocks.py` & `yucca-1.1.2/yucca/networks/blocks_and_layers/conv_blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
-from yucca.network_architectures.blocks_and_layers.conv_layers import (
+from yucca.networks.blocks_and_layers.conv_layers import (
     ConvDropoutNormNonlin,
     ConvDropoutNorm,
 )
-from yucca.network_architectures.blocks_and_layers.norm import LayerNorm3d
+from yucca.networks.blocks_and_layers.norm import LayerNorm3d
 from timm.layers import DropPath
 from functools import partial
 from typing import Callable, Optional
 
 
 class Bottleneck(nn.Module):
     # Bottleneck in torchvision places the stride for downsampling at 3x3 convolution(self.conv2)
```

### Comparing `yucca-1.0.2/yucca/network_architectures/blocks_and_layers/conv_layers.py` & `yucca-1.1.2/yucca/networks/blocks_and_layers/conv_layers.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/network_architectures/blocks_and_layers/norm.py` & `yucca-1.1.2/yucca/networks/blocks_and_layers/norm.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/network_architectures/networks/DeepLabHeadV3Plus.py` & `yucca-1.1.2/yucca/networks/networks/DeepLabHeadV3Plus.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/network_architectures/networks/MedNeXt.py` & `yucca-1.1.2/yucca/networks/networks/MedNeXt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import torch
 import torch.nn as nn
 import torch.utils.checkpoint as checkpoint
-from yucca.network_architectures.blocks_and_layers.conv_blocks import (
+from yucca.networks.blocks_and_layers.conv_blocks import (
     MedNeXtBlock,
     MedNeXtDownBlock,
     MedNeXtUpBlock,
     OutBlock,
 )
-from yucca.network_architectures.networks.YuccaNet import YuccaNet
+from yucca.networks.networks.YuccaNet import YuccaNet
 
 
 class MedNeXt(YuccaNet):
     """
     From the paper: https://arxiv.org/pdf/2303.09975.pdf
     code source: https://github.com/MIC-DKFZ/MedNeXt/tree/main
     Using the 5-kernel L version presented in the paper.
@@ -871,15 +871,14 @@
             x = checkpoint.checkpoint(l, x, self.dummy_tensor)
         return x
 
     def forward(self, xs: list):
         # unpack the output of the encoder
         x_res_0, x_res_1, x_res_2, x_res_3, x = xs
         if self.outside_block_checkpointing:
-
             x_up_3 = checkpoint.checkpoint(self.up_3, x, self.dummy_tensor)
             dec_x = x_res_3 + x_up_3
             x = self.iterative_checkpoint(self.dec_block_3, dec_x)
 
             del x_res_3, x_up_3
 
             x_up_2 = checkpoint.checkpoint(self.up_2, x, self.dummy_tensor)
```

### Comparing `yucca-1.0.2/yucca/network_architectures/networks/MultiResUNet.py` & `yucca-1.1.2/yucca/networks/networks/MultiResUNet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 FROM: https://github.com/j-sripad/mulitresunet-pytorch/blob/main/multiresunet.py
 """
 
 import torch
 import torch.nn as nn
-from yucca.network_architectures.networks.YuccaNet import YuccaNet
-from yucca.network_architectures.blocks_and_layers.conv_blocks import (
+from yucca.networks.networks.YuccaNet import YuccaNet
+from yucca.networks.blocks_and_layers.conv_blocks import (
     Multiresblock,
     Respath,
 )
-from yucca.network_architectures.blocks_and_layers.conv_layers import (
+from yucca.networks.blocks_and_layers.conv_layers import (
     ConvDropoutNormNonlin,
 )
 
 
 class MultiResUNet(YuccaNet):
     """
     Arguments:
```

### Comparing `yucca-1.0.2/yucca/network_architectures/networks/TinyUNet.py` & `yucca-1.1.2/yucca/networks/networks/TinyUNet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
-from yucca.network_architectures.networks.YuccaNet import YuccaNet
-from yucca.network_architectures.blocks_and_layers.conv_layers import (
+from yucca.networks.networks.YuccaNet import YuccaNet
+from yucca.networks.blocks_and_layers.conv_layers import (
     DoubleConvDropoutNormNonlin,
 )
 
 
 class TinyUNet(YuccaNet):
     def __init__(
         self,
```

### Comparing `yucca-1.0.2/yucca/network_architectures/networks/UNet.py` & `yucca-1.1.2/yucca/networks/networks/UNet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
-from yucca.network_architectures.networks.YuccaNet import YuccaNet
-from yucca.network_architectures.blocks_and_layers.conv_layers import (
+from yucca.networks.networks.YuccaNet import YuccaNet
+from yucca.networks.blocks_and_layers.conv_layers import (
     DoubleConvDropoutNormNonlin,
 )
 
 
 class UNet(YuccaNet):
     def __init__(
         self,
```

### Comparing `yucca-1.0.2/yucca/network_architectures/networks/UNetR.py` & `yucca-1.1.2/yucca/networks/networks/UNetR.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 from typing import Tuple
 import torch
 from monai.networks.blocks import UnetrBasicBlock, UnetrPrUpBlock, UnetrUpBlock
 from monai.networks.blocks.dynunet_block import UnetOutBlock
 from monai.networks.nets import ViT
-from yucca.network_architectures.networks.YuccaNet import YuccaNet
+from yucca.networks.networks.YuccaNet import YuccaNet
 
 
 class UNetR(YuccaNet):
     def __init__(
         self,
         input_channels: int,
         patch_size: list | Tuple,
```

### Comparing `yucca-1.0.2/yucca/network_architectures/networks/UNetRE.py` & `yucca-1.1.2/yucca/networks/networks/UNetRE.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
-from yucca.network_architectures.networks.YuccaNet import YuccaNet
-from yucca.network_architectures.blocks_and_layers.conv_layers import (
+from yucca.networks.networks.YuccaNet import YuccaNet
+from yucca.networks.blocks_and_layers.conv_layers import (
     DoubleConvDropoutNormNonlin,
 )
 
 
 class UNetRE(YuccaNet):
     def __init__(
         self,
```

### Comparing `yucca-1.0.2/yucca/network_architectures/networks/UXNet.py` & `yucca-1.1.2/yucca/networks/networks/UXNet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch.nn as nn
 from monai.networks.blocks import UnetrBasicBlock, UnetrUpBlock
 from monai.networks.blocks.dynunet_block import UnetOutBlock
-from yucca.network_architectures.networks.YuccaNet import YuccaNet
-from yucca.network_architectures.blocks_and_layers.conv_blocks import UXNet_encoder
-from yucca.network_architectures.blocks_and_layers.norm import (
+from yucca.networks.networks.YuccaNet import YuccaNet
+from yucca.networks.blocks_and_layers.conv_blocks import UXNet_encoder
+from yucca.networks.blocks_and_layers.norm import (
     LayerNorm2d,
     LayerNorm3d,
 )
 
 
 class UXNet(YuccaNet):
     "https://github.com/MASILab/3DUX-Net/blob/main/networks/UXNet_3D/uxnet_encoder.py"
```

### Comparing `yucca-1.0.2/yucca/network_architectures/networks/YuccaNet.py` & `yucca-1.1.2/yucca/networks/networks/YuccaNet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 from torch import nn
-from yucca.utils.torch_utils import get_available_device
-from yucca.network_architectures.utils.get_steps_for_sliding_window import (
+from yucca.functional.utils.torch_utils import get_available_device
+from yucca.networks.utils.get_steps_for_sliding_window import (
     get_steps_for_sliding_window,
 )
 
 
 class YuccaNet(nn.Module):
     def __init__(self):
         super(YuccaNet, self).__init__()
```

### Comparing `yucca-1.0.2/yucca/network_architectures/networks/resnet.py` & `yucca-1.1.2/yucca/networks/networks/resnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
-from yucca.network_architectures.networks.YuccaNet import YuccaNet
-from yucca.network_architectures.blocks_and_layers.conv_blocks import Bottleneck
+from yucca.networks.networks.YuccaNet import YuccaNet
+from yucca.networks.blocks_and_layers.conv_blocks import Bottleneck
 from torch import Tensor
 
 
 class ResNet50(YuccaNet):
     """ """
 
     def __init__(
```

### Comparing `yucca-1.0.2/yucca/network_architectures/utils/get_steps_for_sliding_window.py` & `yucca-1.1.2/yucca/networks/utils/get_steps_for_sliding_window.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/network_architectures/utils/model_memory_estimation.py` & `yucca-1.1.2/yucca/networks/utils/model_memory_estimation.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 """
 
 import torch
 import numpy as np
 import yucca
 import math
 import logging
-from yucca.utils.torch_utils import get_available_device, flush_and_get_torch_memory_allocated
-from yucca.utils.files_and_folders import recursive_find_python_class
-from yucca.utils.kwargs import filter_kwargs
+from yucca.functional.utils.torch_utils import get_available_device, flush_and_get_torch_memory_allocated
+from yucca.functional.utils.files_and_folders import recursive_find_python_class
+from yucca.functional.utils.kwargs import filter_kwargs
 
 from batchgenerators.utilities.file_and_folder_operations import join
 from torch import nn
 
 
 def estimate_memory_training(model, model_input, optimizer_type=torch.optim.Adam, use_amp=True, device=None):
     """Predict the maximum memory usage of the model.
@@ -41,15 +41,16 @@
         model (nn.Module): the neural network model
         sample_input (torch.Tensor): A sample input to the network. It should be
             a single item, not a batch, and it will be replicated batch_size times.
         batch_size (int): the batch size
         use_amp (bool): whether to estimate based on using mixed precision
         device (torch.device): the device to use
     """
-    device = torch.device(get_available_device())
+    if device is None:
+        device = torch.device(get_available_device())
     # Reset model and optimizer
     model.cpu()
     optimizer = optimizer_type(model.parameters(), lr=0.001)
 
     a = flush_and_get_torch_memory_allocated(device)
     model.to(device)
     b = flush_and_get_torch_memory_allocated(device)
@@ -88,18 +89,21 @@
     model_name,
     max_patch_size,
     fixed_patch_size: tuple | list = None,
     fixed_batch_size: tuple | list = None,
     max_memory_usage_in_gb=None,
 ):
     if max_memory_usage_in_gb is None:
-        try:
-            gpu_vram_in_gb = int(torch.cuda.get_device_properties(0).total_memory / 1024**2 * 0.001)
-        except RuntimeError:
-            gpu_vram_in_gb = 12
+        if not torch.cuda.is_available():
+            gpu_vram_in_gb = 6
+        else:
+            try:
+                gpu_vram_in_gb = int(torch.cuda.get_device_properties(0).total_memory / 1024**2 * 0.001)
+            except RuntimeError:
+                gpu_vram_in_gb = 12
         # Don't wanna utilize more than 8/12GB, to ensure epoch times are kept relatively low
         if dimensionality == "2D":
             max_memory_usage_in_gb = min(8, gpu_vram_in_gb)
         if dimensionality == "3D":
             max_memory_usage_in_gb = min(12, gpu_vram_in_gb)
 
     # Use this offset to factor the overhead from CUDA and other libraries taking a substantial amount of VRAM
@@ -114,15 +118,15 @@
             max_patch_size = max_patch_size[1:]
         conv = nn.Conv2d
         dropout = nn.Dropout2d
         norm = nn.InstanceNorm2d
         batch_size = 8
         max_batch_size = 512
         patch_size = [32, 32]
-        absolute_max = 384**2
+        absolute_max = 224**2
     if dimensionality == "3D":
         conv = nn.Conv3d
         dropout = nn.Dropout3d
         norm = nn.InstanceNorm3d
         batch_size = 2
         max_batch_size = 2
         patch_size = [32, 32, 32]
@@ -137,17 +141,17 @@
         # first fix dimensions so they are divisible by 16 (otherwise issues with standard pools and strides)
         patch_size = [math.ceil(i / 16) * 16 for i in patch_size]
         max_patch_size = patch_size
         if fixed_batch_size:  # In this case we just instantly return after dims are fixed
             return batch_size, tuple(patch_size)
 
     model = recursive_find_python_class(
-        folder=[join(yucca.__path__[0], "network_architectures")],
+        folder=[join(yucca.__path__[0], "networks")],
         class_name=model_name,
-        current_module="yucca.network_architectures",
+        current_module="yucca.networks",
     )
     model_kwargs = {
         "input_channels": modalities,
         "num_classes": num_classes,
         "conv_op": conv,
         "patch_size": patch_size,
         "dropout_op": dropout,
```

### Comparing `yucca-1.0.2/yucca/paths.py` & `yucca-1.1.2/yucca/paths.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/planning/YuccaPlanner.py` & `yucca-1.1.2/yucca/pipeline/planning/YuccaPlanner.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from yucca.pipeline.preprocessing import ClassificationPreprocessor
 import yucca
 import numpy as np
 from yucca.paths import yucca_preprocessed_data, yucca_raw_data
-from yucca.planning.dataset_properties import create_dataset_properties
-from yucca.utils.files_and_folders import recursive_find_python_class
-from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, isfile, load_pickle, save_json, subfiles
+from yucca.pipeline.planning.dataset_properties import create_dataset_properties
+from yucca.functional.utils.files_and_folders import recursive_find_python_class
+from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, isfile, load_pickle, save_json
+from yucca.functional.planning import make_plans_file, add_stats_to_plans_post_preprocessing
+from yucca.pipeline.preprocessing import UnsupervisedPreprocessor
 
 
 class YuccaPlanner(object):
     """
     For subclasses changing parameters: remember to also change the name.
     otherwise different planners will save files with identical names and override eachother.
 
@@ -40,17 +43,19 @@
         view=None,
     ):
         # Required arguments
         self.task = task
 
         # Planner Specific settings
         self.name = str(self.__class__.__name__) + str(view or "")
+        self.compress = False
         self.target_coordinate_system = "RAS"
         self.crop_to_nonzero = True
         self.norm_op = "standardize"
+        self.allow_missing_modalities = False
 
         # This is only relevant for planners with fixed sizes.
         self.keep_aspect_ratio_when_using_target_size = True
 
         # Don't change the remaining variables unless you know what you're doing
         # Threading speeds up the process. Unittests should by default be enabled.
         self.preprocessor = preprocessor
@@ -68,14 +73,15 @@
         if not isfile(join(self.target_dir, "dataset_properties.pkl")):
             print("Properties file not found. Creating one now - this might take a few minutes")
             create_dataset_properties(data_dir=self.in_dir, save_dir=self.target_dir, num_workers=self.threads)
         self.dataset_properties = load_pickle(join(self.target_dir, "dataset_properties.pkl"))
 
         self.determine_transpose()
         self.determine_target_size_from_fixed_size_or_spacing()
+        self.determine_task_type()
         self.validate_target_size()
         self.drop_keys_from_dict(dict=self.dataset_properties, keys=[])
         self.populate_plans_file()
 
         save_json(self.plans, self.plans_path, sort_keys=False)
 
     def determine_transpose(self):
@@ -129,95 +135,79 @@
 
     def drop_keys_from_dict(self, dict, keys):
         for key in keys:
             dict.pop(key)
 
     def preprocess(self):
         preprocessor = recursive_find_python_class(
-            folder=[join(yucca.__path__[0], "preprocessing")],
+            folder=[join(yucca.__path__[0], "pipeline", "preprocessing")],
             class_name=self.preprocessor,
-            current_module="yucca.preprocessing",
+            current_module="yucca.pipeline.preprocessing",
         )
 
-        preprocessor = preprocessor(self.plans_path, self.task, self.threads, self.disable_sanity_checks)
+        preprocessor = preprocessor(
+            plans_path=self.plans_path,
+            task=self.task,
+            threads=self.threads,
+            disable_sanity_checks=self.disable_sanity_checks,
+            allow_missing_modalities=self.allow_missing_modalities,
+            compress=self.compress,
+        )
         preprocessor.run()
         self.postprocess()
 
     def populate_plans_file(self):
-        self.plans["target_coordinate_system"] = self.target_coordinate_system
-        # When True all the background between the volumes and the edges of the image is removed
-        self.plans["crop_to_nonzero"] = self.crop_to_nonzero
-
-        # Change this to have different normalization schemes for all or some modalities
-        self.plans["normalization_scheme"] = [self.norm_op for _ in self.dataset_properties["modalities"]]
-
-        self.plans["transpose_forward"] = self.transpose_fw
-        self.plans["transpose_backward"] = self.transpose_bw
-
-        # Defaults to the median spacing of the training data.
-        # Change the determine_spacing() function to use different spacings
-        self.plans["keep_aspect_ratio_when_using_target_size"] = self.keep_aspect_ratio_when_using_target_size
-        self.plans["target_size"] = self.fixed_target_size
-        self.plans["target_spacing"] = self.fixed_target_spacing
-        self.plans["preprocessor"] = self.preprocessor
-        self.plans["dataset_properties"] = self.dataset_properties
-        self.plans["plans_name"] = self.name
-        self.plans["suggested_dimensionality"] = self.suggested_dimensionality
+        self.plans = make_plans_file(
+            allow_missing_modalities=self.allow_missing_modalities,
+            crop_to_nonzero=self.crop_to_nonzero,
+            classes=self.dataset_properties["classes"],
+            norm_op=self.norm_op,
+            modalities=self.dataset_properties["modalities"],
+            plans_name=self.name,
+            preprocessor=self.preprocessor,
+            dataset_properties=self.dataset_properties,
+            keep_aspect_ratio_when_using_target_size=self.keep_aspect_ratio_when_using_target_size,
+            task_type=self.task_type,
+            target_coordinate_system=self.target_coordinate_system,
+            target_spacing=self.fixed_target_spacing,
+            target_size=self.fixed_target_size,
+            transpose_forward=self.transpose_fw,
+            transpose_backward=self.transpose_bw,
+            suggested_dimensionality=self.suggested_dimensionality,
+        )
 
     def postprocess(self):
-        pkl_files = subfiles(self.plans_folder, suffix=".pkl")
-
-        new_spacings = []
-        new_sizes = []
-        n_cc = []
-        size_cc = []
-        for pkl_file in pkl_files:
-            pkl_file = load_pickle(pkl_file)
-            new_spacings.append(pkl_file["new_spacing"])
-            new_sizes.append(pkl_file["new_size"])
-            n_cc.append(pkl_file["label_cc_n"])
-            if np.mean(pkl_file["label_cc_sizes"]) > 0:
-                size_cc.append(np.mean(pkl_file["label_cc_sizes"], dtype=int))
-
-        mean_size = np.mean(new_sizes, 0, dtype=int).tolist()
-        min_size = np.min(new_sizes, 0).tolist()
-        max_size = np.max(new_sizes, 0).tolist()
-
-        if len(size_cc) > 0:
-            mean_cc = np.mean(size_cc, dtype=int).tolist()
-            min_cc = np.min(size_cc).tolist()
-            max_cc = np.max(size_cc).tolist()
-            mean_n_cc = np.mean(n_cc, dtype=int).tolist()
-            min_n_cc = np.min(n_cc, initial=-1).tolist()
-            max_n_cc = np.max(n_cc, initial=-1).tolist()
-        else:
-            mean_cc = min_cc = max_cc = mean_n_cc = min_n_cc = max_n_cc = 0
-
-        self.plans["new_sizes"] = new_sizes
-        self.plans["new_spacings"] = new_spacings
-        self.plans["new_mean_size"] = mean_size
-        self.plans["new_min_size"] = min_size
-        self.plans["new_max_size"] = max_size
-        self.plans["mean_cc_size"] = mean_cc
-        self.plans["max_cc_size"] = max_cc
-        self.plans["min_cc_size"] = min_cc
-        self.plans["mean_n_cc"] = mean_n_cc
-        self.plans["max_n_cc"] = max_n_cc
-        self.plans["min_n_cc"] = min_n_cc
-
+        self.plans = add_stats_to_plans_post_preprocessing(plans=self.plans, directory=self.plans_folder)
         save_json(self.plans, self.plans_path, sort_keys=False)
 
     def set_paths(self):
         # Setting up paths
         self.in_dir = join(yucca_raw_data, self.task)
         self.target_dir = join(yucca_preprocessed_data, self.task)
         self.plans_folder = join(self.target_dir, self.name)
         self.plans_path = join(self.plans_folder, self.name + "_plans.json")
         maybe_mkdir_p(join(self.target_dir, self.name))
 
+    def determine_task_type(self):
+        preprocessor_class = recursive_find_python_class(
+            folder=[join(yucca.__path__[0], "pipeline", "preprocessing")],
+            class_name=self.preprocessor,
+            current_module="yucca.pipeline.preprocessing",
+        )
+        # If key is not present in plan then we try to infer the task_type from the Type of Preprocessor
+        assert (
+            preprocessor_class
+        ), f"{self.preprocessor} was found in plans, but no class with the corresponding name was found"
+        if issubclass(preprocessor_class, ClassificationPreprocessor):
+            self.task_type = "classification"
+        elif issubclass(preprocessor_class, UnsupervisedPreprocessor):
+            self.task_type = "self-supervised"
+        else:
+            self.task_type = "segmentation"
+
 
 class YuccaPlannerX(YuccaPlanner):
     """
     Used to train (mostly 2D) models on the Coronal view of 3D volumes.
     """
 
     def __init__(
```

### Comparing `yucca-1.0.2/yucca/planning/dataset_properties.py` & `yucca-1.1.2/yucca/pipeline/planning/dataset_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Dict, List
 from batchgenerators.utilities.file_and_folder_operations import subfiles, join, load_json, save_pickle
-from yucca.utils.nib_utils import get_nib_spacing
-from yucca.utils.type_conversions import nifti_or_np_to_np
-from yucca.utils.loading import read_file_to_nifti_or_np
+from yucca.functional.utils.nib_utils import get_nib_spacing
+from yucca.functional.utils.type_conversions import nifti_or_np_to_np
+from yucca.functional.utils.loading import read_file_to_nifti_or_np
 import nibabel as nib
 import numpy as np
 from tqdm.contrib.concurrent import process_map
 from tqdm import tqdm
 from functools import partial
```

### Comparing `yucca-1.0.2/yucca/planning/resampling/UnsupervisedPlannerUnitSpacing.py` & `yucca-1.1.2/yucca/pipeline/planning/resampling/UnsupervisedPlannerUnitSpacing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from yucca.planning.YuccaPlanner import UnsupervisedPlanner
+from yucca.pipeline.planning.YuccaPlanner import UnsupervisedPlanner
 
 
 class UnsupervisedPlannerUnitSpacing(UnsupervisedPlanner):
     def __init__(self, task, preprocessor="UnsupervisedPreprocessor", threads=None, disable_sanity_checks=False, view=None):
         super().__init__(
             task, preprocessor=preprocessor, threads=threads, disable_sanity_checks=disable_sanity_checks, view=view
         )
```

### Comparing `yucca-1.0.2/yucca/planning/resampling/YuccaPlanner_1_1_1.py` & `yucca-1.1.2/yucca/pipeline/planning/resampling/YuccaPlanner_224x224.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from yucca.planning.YuccaPlanner import YuccaPlanner
+from yucca.pipeline.planning.YuccaPlanner import YuccaPlanner
 
 
-class YuccaPlanner_1_1_1(YuccaPlanner):
+class YuccaPlanner_224x224(YuccaPlanner):
     def __init__(self, task, preprocessor="YuccaPreprocessor", threads=None, disable_sanity_checks=False, view=None):
         super().__init__(
             task, preprocessor=preprocessor, threads=threads, disable_sanity_checks=disable_sanity_checks, view=view
         )
         self.name = str(self.__class__.__name__) + str(view or "")
-        self.view = view
-        self.norm_op = "volume_wise_znorm"
 
     def determine_target_size_from_fixed_size_or_spacing(self):
-        self.fixed_target_spacing = [1, 1, 1]
-        self.fixed_target_size = None
+        self.fixed_target_size = [224, 224]
+        self.fixed_target_spacing = None
```

### Comparing `yucca-1.0.2/yucca/planning/resampling/YuccaPlanner_1_1_125.py` & `yucca-1.1.2/yucca/pipeline/planning/resampling/YuccaPlanner_NoResample.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from yucca.planning.YuccaPlanner import YuccaPlanner
+from yucca.pipeline.planning.YuccaPlanner import YuccaPlanner
 
 
-class YuccaPlanner_1_1_125(YuccaPlanner):
+class YuccaPlanner_NoResample(YuccaPlanner):
     def __init__(self, task, preprocessor="YuccaPreprocessor", threads=None, disable_sanity_checks=False, view=None):
         super().__init__(
             task, preprocessor=preprocessor, threads=threads, disable_sanity_checks=disable_sanity_checks, view=view
         )
         self.name = str(self.__class__.__name__) + str(view or "")
-        self.view = view
 
     def determine_target_size_from_fixed_size_or_spacing(self):
-        self.fixed_target_spacing = [1, 1, 1.25]
+        self.fixed_target_spacing = None
         self.fixed_target_size = None
```

### Comparing `yucca-1.0.2/yucca/planning/resampling/YuccaPlanner_224x224.py` & `yucca-1.1.2/yucca/pipeline/planning/resampling/YuccaPlanner_1_1_125.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from yucca.planning.YuccaPlanner import YuccaPlanner
+from yucca.pipeline.planning.YuccaPlanner import YuccaPlanner
 
 
-class YuccaPlanner_224x224(YuccaPlanner):
-
+class YuccaPlanner_1_1_125(YuccaPlanner):
     def __init__(self, task, preprocessor="YuccaPreprocessor", threads=None, disable_sanity_checks=False, view=None):
         super().__init__(
             task, preprocessor=preprocessor, threads=threads, disable_sanity_checks=disable_sanity_checks, view=view
         )
         self.name = str(self.__class__.__name__) + str(view or "")
+        self.view = view
 
     def determine_target_size_from_fixed_size_or_spacing(self):
-        self.fixed_target_size = [224, 224]
-        self.fixed_target_spacing = None
+        self.fixed_target_spacing = [1, 1, 1.25]
+        self.fixed_target_size = None
```

### Comparing `yucca-1.0.2/yucca/preprocessing/normalization.py` & `yucca-1.1.2/yucca/functional/array_operations/normalization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 import warnings
 from skimage import exposure
 import numpy as np
+from typing import Optional
 
 
-def normalizer(array: np.ndarray, scheme: str, intensities: {}):
+def normalizer(array: np.ndarray, scheme: str, intensities: Optional[dict] = None):
     """
     Normalizing function for preprocessing and inference.
 
     supported schemes can be either:
     None = for no normalization. Generally not recommended.
     MinMax = for 0-1 or Min-Max normalization.
     255to1 = for 0-1 normalization of 8 bit images.
     Standardize = (array - mean) / std. Based on modality wide stats.
     Clip = for contrast clipping. This will clip values to the 0.01 and 99.99th percentiles
         and then perform 0-1 normalization.
     """
-    accepted_schemes = ["clipping", "minmax", "no_norm", "standardize", "volume_wise_znorm", "255to1"]
+    accepted_schemes = ["clipping", "minmax", "range", "no_norm", "standardize", "volume_wise_znorm", "255to1"]
 
     assert scheme in accepted_schemes, "invalid normalization scheme inserted" f"attempted scheme: {scheme}"
     assert array is not None
 
     if scheme == "no_norm":
         return array
 
     elif scheme == "minmax":
         assert intensities is not None, "ERROR: dataset wide stats are required for minmax"
-        return (array - intensities["min"]) / (intensities["max"] - intensities["min"])
+        return (array - intensities["min"]) / (intensities["max"] - intensities["min"] + 1e-9)
 
     elif scheme == "255to1":
         return array / 255
 
+    elif scheme == "range":
+        print(array.max(), array.min(), intensities)
+        return (array - array.min()) / (array.max() - array.min() + 1e-9) * (
+            intensities["max"] - intensities["min"] + 1e-9
+        ) + intensities["min"]
+
     elif scheme == "standardize":
         assert intensities is not None, "ERROR: dataset wide stats are required for standardize"
         return (array - float(intensities["mean"])) / float(intensities["std"])
 
     elif scheme == "clip":
         lower_bound, upper_bound = np.percentile(array, (0.01, 99.99))
         array = exposure.rescale_intensity(array, in_range=(lower_bound, upper_bound), out_range=(0, 1))
         return array
 
     elif scheme == "volume_wise_znorm":
         empty_val = array.min()  # We assume the background is the minimum value
-
         if empty_val != array[0, 0, 0]:
             warnings.warn(
                 "Tried to normalize an array where the top right value was not the same as the minimum value."
                 f"empty_val: {empty_val}, top right: {array[0, 0, 0]}"
             )
         mask = array != empty_val
         array = clamp(array, mask=mask)
```

### Comparing `yucca-1.0.2/yucca/run/run_ensemble.py` & `yucca-1.1.2/yucca/pipeline/run/run_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 2. You can specify the task, trainer and planner like it's also done in other yucca_ scripts.
 if "-t" for target task is left blank, we assume you are predicting and evaluating data
 from the same task as the one the model is trained on.
 """
 
 import argparse
-from yucca.utils.saving import merge_softmax_from_folders
+from yucca.functional.utils.saving import merge_softmax_from_folders
 
 
 def main():
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "--in_dirs",
```

### Comparing `yucca-1.0.2/yucca/run/run_finetune.py` & `yucca-1.1.2/yucca/pipeline/run/run_finetune.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import yucca
-from yucca.utils.task_ids import maybe_get_task_from_task_id
-from yucca.utils.files_and_folders import recursive_find_python_class
+from yucca.pipeline.task_conversion.utils import maybe_get_task_from_task_id
+from yucca.functional.utils.files_and_folders import recursive_find_python_class
 from batchgenerators.utilities.file_and_folder_operations import join
 
 
 def main():
     parser = argparse.ArgumentParser()
 
     # Required Arguments #
@@ -127,17 +127,17 @@
     split_data_param = args.split_data_param
     train_batches_per_step = args.train_batches_per_step
     val_batches_per_step = args.val_batches_per_step
 
     kwargs = {}
 
     manager = recursive_find_python_class(
-        folder=[join(yucca.__path__[0], "training", "managers")],
+        folder=[join(yucca.__path__[0], "pipeline", "managers")],
         class_name=manager_name,
-        current_module="yucca.training.managers",
+        current_module="yucca.pipeline.managers",
     )
 
     manager = manager(
         batch_size=batch_size,
         ckpt_path=checkpoint,
         continue_from_most_recent=not new_version,
         deep_supervision=deep_supervision,
```

### Comparing `yucca-1.0.2/yucca/run/run_inference.py` & `yucca-1.1.2/yucca/pipeline/run/run_inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import yucca
-from yucca.utils.task_ids import maybe_get_task_from_task_id
+from yucca.pipeline.task_conversion.utils import maybe_get_task_from_task_id
 from yucca.paths import yucca_raw_data, yucca_results, yucca_models
-from yucca.evaluation.YuccaEvaluator import YuccaEvaluator
-from yucca.training.managers.YuccaManager import YuccaManager
-from yucca.utils.files_and_folders import recursive_find_python_class
+from yucca.pipeline.evaluation.YuccaEvaluator import YuccaEvaluator
+from yucca.pipeline.managers.YuccaManager import YuccaManager
+from yucca.functional.utils.files_and_folders import recursive_find_python_class
 from batchgenerators.utilities.file_and_folder_operations import (
     join,
     isfile,
     maybe_mkdir_p,
     isdir,
     subdirs,
 )
@@ -151,14 +151,16 @@
     no_eval = args.no_eval
     overwrite = args.overwrite
     predict_train = args.predict_train
     profile = args.profile
     save_softmax = args.save_softmax
     use_wandb = not args.no_wandb
 
+    kwargs = {}
+
     path_to_versions = join(
         yucca_models,
         source_task,
         model + "__" + dimensions,
         manager_name + "__" + planner,
         experiment,
         f"{split_data_method}_{split_data_param}_fold_{split_idx}",
@@ -179,17 +181,17 @@
         checkpoint + ".ckpt",
     )
 
     assert isfile(modelfile), "Can't find .cpkt file with trained model weights. " f"Should be located at: {modelfile}"
     print(f"######################################################################## \n" f"{'Using model: ':25} {modelfile}")
 
     manager = recursive_find_python_class(
-        folder=[join(yucca.__path__[0], "training", "managers")],
+        folder=[join(yucca.__path__[0], "pipeline", "managers")],
         class_name=manager_name,
-        current_module="yucca.training.managers",
+        current_module="yucca.pipeline.managers",
     )
 
     assert manager, f"searching for {manager_name} " f"but found: {manager}"
     assert issubclass(manager, (YuccaManager, YuccaManager)), "Trainer is not a subclass of YuccaTrainer."
 
     print(f"{'Using manager: ':25} {manager_name}")
     manager = manager(
@@ -200,26 +202,28 @@
         model_dimensions=dimensions,
         task=source_task,
         split_idx=split_idx,
         split_data_method=split_data_method,
         split_data_param=split_data_param,
         planner=planner,
         profile=profile,
+        **kwargs,
     )
 
     # Setting up input paths and output paths
     inpath = join(yucca_raw_data, target_task, "imagesTs")
     ground_truth = join(yucca_raw_data, target_task, "labelsTs")
 
     outpath = join(
         yucca_results,
         target_task,
         source_task,
         model + "__" + dimensions,
         manager_name + "__" + planner,
+        experiment,
         f"{split_data_method}_{split_data_param}_fold_{split_idx}",
         f"version_{version}",
         checkpoint,
     )
 
     if predict_train:
         inpath = join(yucca_raw_data, target_task, "imagesTr")
```

### Comparing `yucca-1.0.2/yucca/run/run_preprocessing.py` & `yucca-1.1.2/yucca/pipeline/run/run_preprocessing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import yucca
-from yucca.utils.task_ids import maybe_get_task_from_task_id
-from yucca.utils.files_and_folders import recursive_find_python_class
+from yucca.pipeline.task_conversion.utils import maybe_get_task_from_task_id
+from yucca.functional.utils.files_and_folders import recursive_find_python_class
 from batchgenerators.utilities.file_and_folder_operations import join
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-t", "--task", help="Name of the task to preprocess. " "Should be of format: TaskXXX_MYTASK", required=True
@@ -27,38 +27,42 @@
     )
     parser.add_argument(
         "--ensemble",
         help="Used to initialize data preprocessing for ensemble/2.5D training",
         default=False,
         action="store_true",
     )
-    parser.add_argument("--disable_sanity_checks", help="Enable or disable sanity checks", default=False)
+    parser.add_argument("--disable_sanity_checks", help="Enable or disable sanity checks", action="store_true", default=False)
     parser.add_argument("--threads", help="Used to specify the number of processes to use for preprocessing", default=2)
     args = parser.parse_args()
 
     task = maybe_get_task_from_task_id(args.task)
     planner_name = args.pl
     preprocessor_name = args.pr
     view = args.v
     disable_sanity_checks = args.disable_sanity_checks
     ensemble = args.ensemble
     threads = args.threads
 
     if not ensemble:
         planner = recursive_find_python_class(
-            folder=[join(yucca.__path__[0], "planning")], class_name=planner_name, current_module="yucca.planning"
+            folder=[join(yucca.__path__[0], "pipeline", "planning")],
+            class_name=planner_name,
+            current_module="yucca.pipeline.planning",
         )
         planner = planner(task, preprocessor_name, threads=threads, disable_sanity_checks=disable_sanity_checks, view=view)
         planner.plan()
         planner.preprocess()
     if ensemble:
         views = ["X", "Y", "Z"]
         for view in views:
             planner = recursive_find_python_class(
-                folder=[join(yucca.__path__[0], "planning")], class_name=planner_name, current_module="yucca.planning"
+                folder=[join(yucca.__path__[0], "pipeline", "planning")],
+                class_name=planner_name,
+                current_module="yucca.pipeline.planning",
             )
             planner = planner(task, preprocessor_name, threads=threads, disable_sanity_checks=disable_sanity_checks, view=view)
             planner.plan()
             planner.preprocess()
 
 
 if __name__ == "__main__":
```

### Comparing `yucca-1.0.2/yucca/run/run_task_conversion.py` & `yucca-1.1.2/yucca/pipeline/run/run_task_conversion.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     parser.add_argument(
         "-t", "--task", help="Name of the task to preprocess. " "Should be of format: TaskXXX_MYTASK", required=True
     )
     parser.add_argument("-p", "--path", help="Path to source data", default=yucca_source)
     parser.add_argument("-d", "--subdir", help="Directory of data inside source data")
 
     args = parser.parse_args()
-    task_converter = importlib.import_module(f"yucca.task_conversion.{args.task}")
+    task_converter = importlib.import_module(f"yucca.pipeline.task_conversion.{args.task}")
 
     if args.subdir is None:
         task_converter.convert(args.path)
     else:
         task_converter.convert(args.path, args.subdir)
```

### Comparing `yucca-1.0.2/yucca/run/run_training.py` & `yucca-1.1.2/yucca/pipeline/run/run_training.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import yucca
-from yucca.utils.task_ids import maybe_get_task_from_task_id
-from yucca.utils.files_and_folders import recursive_find_python_class
+from yucca.pipeline.task_conversion.utils import maybe_get_task_from_task_id
+from yucca.functional.utils.files_and_folders import recursive_find_python_class
 from batchgenerators.utilities.file_and_folder_operations import join
 
 
 def main():
     parser = argparse.ArgumentParser()
 
     # Required Arguments #
@@ -93,15 +93,16 @@
     parser.add_argument(
         "--split_data_param",
         help="Specify the parameter for the selected split method. For KFold use an int, for simple_split use a float between 0.0-1.0.",
         default=5,
     )
     parser.add_argument("--train_batches_per_step", type=int, default=250)
     parser.add_argument("--val_batches_per_step", type=int, default=50)
-
+    parser.add_argument("--fast_dev_run", action="store_true")
+    parser.add_argument("--accelerator", type=str, default=None)
     args = parser.parse_args()
 
     # Required
     task = maybe_get_task_from_task_id(args.task)
 
     # Optionals (frequently changed)
     dimensions = args.d
@@ -111,14 +112,15 @@
 
     # Optionals (occasionally changed)
     log = not args.disable_logging
     batch_size = args.batch_size
     deep_supervision = args.ds
     epochs = args.epochs
     experiment = args.experiment
+    fast_dev_run = args.fast_dev_run
     loss = args.loss
     lr = args.lr
     max_vram = args.max_vram
     momentum = args.mom
     new_version = args.new_version
     num_workers = args.num_workers
     patch_size = args.patch_size
@@ -126,32 +128,34 @@
     profile = args.profile
     split_idx = args.split_idx
     split_data_method = args.split_data_method
     split_data_param = args.split_data_param
     train_batches_per_step = args.train_batches_per_step
     val_batches_per_step = args.val_batches_per_step
 
-    kwargs = {}
+    kwargs = {"fast_dev_run": fast_dev_run}
+    if args.accelerator is not None:
+        kwargs["accelerator"] = args.accelerator
 
     assert model_name in [
         "MedNeXt",
         "MultiResUNet",
         "UNet",
         "UNetR",
         "UNetRE",
         "UXNet",
         "ResNet50",
         "TinyUNet",
     ], f"{model_name} is an invalid model name. This is case sensitive."
 
     print(f"{'Using manager: ':25} {manager_name}")
     manager = recursive_find_python_class(
-        folder=[join(yucca.__path__[0], "training", "managers")],
+        folder=[join(yucca.__path__[0], "pipeline", "managers")],
         class_name=manager_name,
-        current_module="yucca.training.managers",
+        current_module="yucca.pipeline.managers",
     )
 
     manager = manager(
         ckpt_path=None,
         continue_from_most_recent=not new_version,
         deep_supervision=deep_supervision,
         enable_logging=log,
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task000_TEST_CLASSIFICATION.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task000_TEST_CLASSIFICATION.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ONLY used to run tests
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 import shutil
 from yucca.paths import yucca_raw_data
 from tqdm import tqdm
 from sklearn.model_selection import train_test_split
 
 
 def convert(path: str, subdir: str = "dataset_test0_classification"):
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task000_TEST_SEGMENTATION.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task000_TEST_SEGMENTATION.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     lab = np.random.randint(0, 2, (32, 32, 32)).astype(float)
     ims.append(nib.Nifti1Image(arr, affine=np.eye(4)))
     labs.append(nib.Nifti1Image(lab, affine=np.eye(4)))
 
 """
 
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 import shutil
 from yucca.paths import yucca_raw_data
 from tqdm import tqdm
 from sklearn.model_selection import train_test_split
 
 
 def convert(path: str, subdir: str = "dataset_test0"):
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task000_TEST_UNSUPERVISED.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task000_TEST_UNSUPERVISED.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     lab = np.random.randint(0, 2, (32, 32, 32)).astype(float)
     ims.append(nib.Nifti1Image(arr, affine=np.eye(4)))
     labs.append(nib.Nifti1Image(lab, affine=np.eye(4)))
 
 """
 
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 import shutil
 from yucca.paths import yucca_raw_data
 from tqdm import tqdm
 from sklearn.model_selection import train_test_split
 
 
 def convert(path: str, subdir: str = "dataset_test0"):
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task001_OASIS.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task001_OASIS.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, save_pickle
 
     maybe_mkdir_p(join(yucca_preprocessing_dir, task_name))
     save_pickle(splits, join(yucca_preprocessing_dir, task_name, 'splits.pkl'))
 """
 
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 import shutil
 import gzip
 from yucca.paths import yucca_raw_data
 from tqdm import tqdm
 
 
 def convert(path: str, subdir: str = "OASIS"):
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task002_LPBA40.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task002_LPBA40.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 import shutil
 import gzip
 from yucca.paths import yucca_raw_data
 from tqdm import tqdm
 
 
 def convert(path: str, subdir: str = "LPBA40"):
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task003_Hammers.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task003_Hammers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 import shutil
 import gzip
 from yucca.paths import yucca_raw_data
 from tqdm import tqdm
 
 
 def convert(path: str, subdir: str = "Hammers"):
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task004_HarP.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task004_HarP.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 import shutil
 import gzip
 from yucca.paths import yucca_raw_data
 
 
 def convert(path: str, subdir: str = "HarP"):
     # INPUT DATA
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task005_ISLES22.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task005_ISLES22.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import nibabel as nib
 import nibabel.processing as nibpro
 from tqdm import tqdm
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subdirs
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
 from sklearn.model_selection import train_test_split
 
 
 def convert(path: str, subdir: str = "ISLES-2022"):
     # INPUT DATA
     path = f"{path}/{subdir}"
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task006_WMH_Flair.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task006_WMH_Flair.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import shutil
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfolders
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
 
 
 def convert(path: str, subdir: str = "WMH"):
     """INPUT DATA - Define input path and suffixes"""
     path = join(path, subdir)
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task007_WMH_T1.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task007_WMH_T1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import shutil
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfolders
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
 
 
 def convert(path: str, subdir: str = "WMH"):
     """INPUT DATA - Define input path and suffixes"""
     path = join(path, subdir)
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task008_WMH.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task008_WMH.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import shutil
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfolders
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
 
 
 def convert(path: str, subdir: str = "WMH"):
     """INPUT DATA - Define input path and suffixes"""
     path = join(path, subdir)
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task010_AMOS22.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task010_AMOS22.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 import shutil
 from yucca.paths import yucca_raw_data
 
 
 def convert(path: str, subdir: str = "amos22"):
     # INPUT DATA
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task011_MSSEG1.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task011_MSSEG1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subdirs
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
 import shutil
 
 
 def convert(path: str, subdir: str = "MSSEG1_2016"):
     # Target names
     task_name = "Task011_MSSEG1"
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task012_BraTS21.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task012_BraTS21.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subdirs
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
 from sklearn.model_selection import train_test_split
 import nibabel as nib
 import numpy as np
 import shutil
 
 
@@ -49,15 +49,15 @@
         dst_image_file_path4 = f"{target_imagesTr}/{task_prefix}_{sTr}_003.nii.gz"
 
         dst_label_path = f"{target_labelsTr}/{task_prefix}_{sTr}.nii.gz"
         label = nib.load(join(base_in, sTr, sTr + "_seg" + file_suffix))
         labelarr = label.get_fdata()
         labelarr[labelarr == 4.0] = 3.0
         assert np.all(np.isin(np.unique(labelarr), np.array([0, 1, 2, 3])))
-        labelnew = nib.Nifti1Image(labelarr, label.affine, label.header)
+        labelnew = nib.Nifti1Image(labelarr, label.affine, label.header, dtype=np.float32)
         nib.save(labelnew, dst_label_path)
 
         shutil.copy2(src_image_file_path1, dst_image_file_path1)
         shutil.copy2(src_image_file_path2, dst_image_file_path2)
         shutil.copy2(src_image_file_path3, dst_image_file_path3)
         shutil.copy2(src_image_file_path4, dst_image_file_path4)
 
@@ -72,15 +72,15 @@
         dst_image_file_path4 = f"{target_imagesTs}/{task_prefix}_{sTs}_003.nii.gz"
 
         dst_label_path = f"{target_labelsTs}/{task_prefix}_{sTs}.nii.gz"
         label = nib.load(join(base_in, sTs, sTs + "_seg" + file_suffix))
         labelarr = label.get_fdata()
         labelarr[labelarr == 4.0] = 3.0
         assert np.all(np.isin(np.unique(labelarr), np.array([0, 1, 2, 3])))
-        labelnew = nib.Nifti1Image(labelarr, label.affine, label.header)
+        labelnew = nib.Nifti1Image(labelarr, label.affine, label.header, dtype=np.float32)
         nib.save(labelnew, dst_label_path)
 
         shutil.copy2(src_image_file_path1, dst_image_file_path1)
         shutil.copy2(src_image_file_path2, dst_image_file_path2)
         shutil.copy2(src_image_file_path3, dst_image_file_path3)
         shutil.copy2(src_image_file_path4, dst_image_file_path4)
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task021_Decathlon_BrainTumour.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task021_Decathlon_BrainTumour.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import nibabel as nib
 import numpy as np
 from sklearn.model_selection import train_test_split
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data, yucca_source
-from yucca.utils.nib_utils import get_nib_orientation, get_nib_spacing
+from yucca.functional.utils.nib_utils import get_nib_orientation, get_nib_spacing
 
 
 def convert(path: str = yucca_source, subdir: str = "decathlon", subsubdir: str = "Task01_BrainTumour"):
     # INPUT DATA
     path = f"{path}/{subdir}/{subsubdir}"
 
     file_suffix = ".nii.gz"
@@ -53,23 +53,20 @@
         t1w = image.slicer[:, :, :, 1]
         t1gd = image.slicer[:, :, :, 2]
         t2w = image.slicer[:, :, :, 3]
 
         orig_ornt = get_nib_orientation(flair)
         label_ornt = get_nib_orientation(label)
         if orig_ornt == label_ornt:
-
             orig_spacing = get_nib_spacing(flair)
             label_spacing = get_nib_spacing(label)
             if orig_spacing.all() == label_spacing.all():
-
                 orig_shape = np.shape(flair)
                 label_shape = np.shape(label)
                 if orig_shape == label_shape:
-
                     nib.save(flair, f"{target_imagesTr}/{task_prefix}_{sTr}_000.nii.gz")
                     nib.save(t1w, f"{target_imagesTr}/{task_prefix}_{sTr}_001.nii.gz")
                     nib.save(t1gd, f"{target_imagesTr}/{task_prefix}_{sTr}_002.nii.gz")
                     nib.save(t2w, f"{target_imagesTr}/{task_prefix}_{sTr}_003.nii.gz")
 
                     nib.save(label, f"{target_labelsTr}/{task_prefix}_{sTr}.nii.gz")
 
@@ -93,22 +90,20 @@
         t1gd = image.slicer[:, :, :, 2]
         t2w = image.slicer[:, :, :, 3]
 
         orig_ornt = get_nib_orientation(flair)
         label_ornt = get_nib_orientation(label)
 
         if orig_ornt == label_ornt:
-
             print("same orientation")
 
             orig_spacing = get_nib_spacing(flair)
             label_spacing = get_nib_spacing(label)
 
             if orig_spacing.all() == label_spacing.all():
-
                 print("same spacing")
 
                 orig_shape = np.shape(flair)
                 label_shape = np.shape(label)
 
                 if orig_shape == label_shape:
                     nib.save(flair, f"{target_imagesTs}/{task_prefix}_{sTs}_000.nii.gz")
@@ -119,15 +114,14 @@
                     nib.save(label, f"{target_labelsTs}/{task_prefix}_{sTs}.nii.gz")
 
                 else:
                     print("shape not matching, file not saved")
                     skipped.append(join(images_dir_ts, sTs))
 
             else:
-
                 print("Spacing not matching")
                 skipped.append(join(images_dir_ts, sTs))
 
         else:
             print("Orientation not matching")
             skipped.append(join(images_dir_ts, sTs))
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task023_Decathlon_Liver.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task023_Decathlon_Liver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import nibabel as nib
 import numpy as np
 from sklearn.model_selection import train_test_split
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
-from yucca.utils.nib_utils import get_nib_orientation, get_nib_spacing
+from yucca.functional.utils.nib_utils import get_nib_orientation, get_nib_spacing
 
 
 def convert(path: str, subdir: str = "decathlon", subsubdir: str = "Task03_Liver"):
     # INPUT DATA
     path = f"{path}/{subdir}/{subsubdir}"
 
     file_suffix = ".nii.gz"
@@ -48,39 +48,35 @@
         sTr = sTr[: -len(file_suffix)]
 
         # Orient to RAS and register image-label, using the image as reference.
         orig_ornt = get_nib_orientation(image)
         label_ornt = get_nib_orientation(label)
 
         if orig_ornt == label_ornt:
-
             print("same orientation")
 
             orig_spacing = get_nib_spacing(image)
             label_spacing = get_nib_spacing(label)
 
             if orig_spacing.all() == label_spacing.all():
-
                 print("same spacing")
 
                 orig_shape = np.shape(image)
                 label_shape = np.shape(label)
 
                 if orig_shape == label_shape:
-
                     nib.save(image, filename=f"{target_imagesTr}/{task_prefix}_{sTr}_000.nii.gz")
                     nib.save(label, filename=f"{target_labelsTr}/{task_prefix}_{sTr}.nii.gz")
                     print("same shape, file saved")
 
                 else:
                     print("shape not matching, file not saved")
                     skipped.append(join(images_dir_tr, sTr))
 
             else:
-
                 print("Spacing not matching")
                 skipped.append(join(images_dir_tr, sTr))
 
         else:
             print("Orientation not matching")
             skipped.append(join(images_dir_tr, sTr))
 
@@ -90,39 +86,35 @@
         sTs = sTs[: -len(file_suffix)]
 
         # Orient to RAS and register image-label, using the image as reference.
         orig_ornt = get_nib_orientation(image)
         label_ornt = get_nib_orientation(label)
 
         if orig_ornt == label_ornt:
-
             print("same orientation")
 
             orig_spacing = get_nib_spacing(image)
             label_spacing = get_nib_spacing(label)
 
             if orig_spacing.all() == label_spacing.all():
-
                 print("same spacing")
 
                 orig_shape = np.shape(image)
                 label_shape = np.shape(label)
 
                 if orig_shape == label_shape:
-
                     nib.save(image, filename=f"{target_imagesTs}/{task_prefix}_{sTs}_000.nii.gz")
                     nib.save(label, filename=f"{target_labelsTs}/{task_prefix}_{sTs}.nii.gz")
                     print("same shape, file saved")
 
                 else:
                     print("shape not matching, file not saved")
                     skipped.append(join(images_dir_ts, sTs))
 
             else:
-
                 print("Spacing not matching")
                 skipped.append(join(images_dir_ts, sTs))
 
         else:
             print("Orientation not matching")
             skipped.append(join(images_dir_ts, sTs))
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task028_Decathlon_HepaticVessel.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task028_Decathlon_HepaticVessel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import nibabel as nib
 import numpy as np
 from sklearn.model_selection import train_test_split
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
-from yucca.utils.nib_utils import get_nib_orientation, get_nib_spacing
+from yucca.functional.utils.nib_utils import get_nib_orientation, get_nib_spacing
 
 
 def convert(path: str, subdir: str = "decathlon", subsubdir: str = "Task08_HepaticVessel"):
     # INPUT DATA
     path = f"{path}/{subdir}/{subsubdir}"
 
     file_suffix = ".nii.gz"
@@ -48,39 +48,35 @@
         sTr = sTr[: -len(file_suffix)]
 
         # Orient to RAS and register image-label, using the image as reference.
         orig_ornt = get_nib_orientation(image)
         label_ornt = get_nib_orientation(label)
 
         if orig_ornt == label_ornt:
-
             print("same orientation")
 
             orig_spacing = get_nib_spacing(image)
             label_spacing = get_nib_spacing(label)
 
             if orig_spacing.all() == label_spacing.all():
-
                 print("same spacing")
 
                 orig_shape = np.shape(image)
                 label_shape = np.shape(label)
 
                 if orig_shape == label_shape:
-
                     nib.save(image, filename=f"{target_imagesTr}/{task_prefix}_{sTr}_000.nii.gz")
                     nib.save(label, filename=f"{target_labelsTr}/{task_prefix}_{sTr}.nii.gz")
                     print("same shape, file saved")
 
                 else:
                     print("shape not matching, file not saved")
                     skipped.append(join(images_dir_tr, sTr))
 
             else:
-
                 print("Spacing not matching")
                 skipped.append(join(images_dir_tr, sTr))
 
         else:
             print("Orientation not matching")
             skipped.append(join(images_dir_tr, sTr))
 
@@ -90,39 +86,35 @@
         sTs = sTs[: -len(file_suffix)]
 
         # Orient to RAS and register image-label, using the image as reference.
         orig_ornt = get_nib_orientation(image)
         label_ornt = get_nib_orientation(label)
 
         if orig_ornt == label_ornt:
-
             print("same orientation")
 
             orig_spacing = get_nib_spacing(image)
             label_spacing = get_nib_spacing(label)
 
             if orig_spacing.all() == label_spacing.all():
-
                 print("same spacing")
 
                 orig_shape = np.shape(image)
                 label_shape = np.shape(label)
 
                 if orig_shape == label_shape:
-
                     nib.save(image, filename=f"{target_imagesTs}/{task_prefix}_{sTs}_000.nii.gz")
                     nib.save(label, filename=f"{target_labelsTs}/{task_prefix}_{sTs}.nii.gz")
                     print("same shape, file saved")
 
                 else:
                     print("shape not matching, file not saved")
                     skipped.append(join(images_dir_ts, sTs))
 
             else:
-
                 print("Spacing not matching")
                 skipped.append(join(images_dir_ts, sTs))
 
         else:
             print("Orientation not matching")
             skipped.append(join(images_dir_ts, sTs))
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task100_combine_001_002.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task100_combine_001_002.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from yucca.task_conversion.utils import combine_imagesTr_from_tasks, generate_dataset_json
+from yucca.pipeline.task_conversion.utils import combine_imagesTr_from_tasks, generate_dataset_json
 from yucca.paths import yucca_raw_data
 
 
 def convert(_path: str, _subdir: str = ""):
     # Define the name of the new task
     task_name = "Task100_combine_001_002"
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task201_PPMI.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task201_PPMI.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json, dirs_in_dir, should_use_volume
+from yucca.pipeline.task_conversion.utils import generate_dataset_json, dirs_in_dir, should_use_volume
 from yucca.paths import yucca_raw_data
 from datetime import datetime
 from tqdm import tqdm
 import nibabel as nib
 
 
 accept_modalities = ["t1", "t2", "mprage", "flair", "gre", "dwi", "swi", "grappa"]
@@ -55,18 +55,28 @@
                 parsed_date = datetime.strptime(date, "%Y-%m-%d_%H_%M_%S.%f")
                 date_simple = parsed_date.strftime("%Y%m%d")
                 for image in dirs_in_dir(date_dir):
                     image_dir = join(date_dir, image)
                     if "nifti" and "dicom" in dirs_in_dir(image_dir):
                         image_dir = join(image_dir, "nifti")
                     for file in subfiles(image_dir, join=False, suffix=".nii"):
+                        other_info = (
+                            file.replace(subject, "")
+                            .replace(modality, "")
+                            .replace(date_simple, "")
+                            .replace(image, "")
+                            .replace(".nii", "")
+                            .replace(".", "_")
+                        )
                         image_path = join(image_dir, file)
                         vol = nib.load(image_path)
                         if should_use_volume(vol):
-                            output_name = f"{task_prefix}_{subject}_{modality}_{date_simple}_{image}_000.nii.gz"
+                            output_name = (
+                                f"{task_prefix}_#_{subject}_#_{modality}_#_{date_simple}_#_{image}_#_{other_info}_000.nii.gz"
+                            )
                             output_path = join(target_imagesTr, output_name)
                             nib.save(vol, filename=output_path)
 
     generate_dataset_json(
         join(target_base, "dataset.json"),
         target_imagesTr,
         imagesTs_dir=None,
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task202_ISLES22.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task202_ISLES22.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json, dirs_in_dir
+from yucca.pipeline.task_conversion.utils import generate_dataset_json, dirs_in_dir
 from yucca.paths import yucca_raw_data
 from tqdm import tqdm
 import shutil
 
 
 def convert(path: str, subdir: str = "ISLES-2022"):
     """INPUT DATA - Define input path and suffixes"""
@@ -30,16 +30,16 @@
         subject_dir = join(subjects_dir, subject)
         for session in dirs_in_dir(subject_dir):
             session_dir = join(subject_dir, session)
             for modality in dirs_in_dir(session_dir):
                 modality_dir = join(session_dir, modality)
                 for file in subfiles(modality_dir, join=False, suffix=ext):
                     image_path = join(modality_dir, file)
-                    file_name = file[: -len(ext)]
-                    output_name = f"{task_prefix}_{file_name}_000.nii.gz"
+                    other_info = file[: -len(ext)].replace(subject, "").replace(session, "").replace(modality, "")
+                    output_name = f"{task_prefix}_{subject}_{modality}_{session}_{other_info}_000.nii.gz"
                     output_path = join(target_imagesTr, output_name)
                     shutil.copy2(image_path, output_path)
 
     generate_dataset_json(
         join(target_base, "dataset.json"),
         target_imagesTr,
         imagesTs_dir=None,
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task203_OASIS3.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task204_OASIS4.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,76 @@
 import shutil
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json, dirs_in_dir, should_use_volume
+from yucca.pipeline.task_conversion.utils import generate_dataset_json, should_use_volume, dirs_in_dir
 from yucca.paths import yucca_raw_data
 from tqdm import tqdm
 import nibabel as nib
 
 
-accept_modalities = ["t1", "t2", "mprage", "flair", "gre", "dwi", "swi", "grappa", "anat"]
 rejec_modalities = ["fmri", "func"]  # TODO: Might need to skip GRE
 
 
 def should_skip(modality: str):
     modality = modality.lower()
     for reject in rejec_modalities:
         if reject in modality:
             return True
-    for accept in accept_modalities:
-        if accept in modality:
-            return False
-    return True
+    return False
 
 
-def convert(path: str, subdir: str = "OASIS3"):
+def convert(path: str, subdir: str = "OASIS4"):
     """INPUT DATA - Define input path and suffixes"""
     path = join(path, subdir)
 
     """ OUTPUT DATA - Define the task name and prefix """
-    task_name = "Task203_OASIS3"
-    task_prefix = "OASIS3"
+    task_name = "Task204_OASIS4"
+    task_prefix = "OASIS4"
 
-    subjects_dir = join(path, "DATA")
+    subjects_dir = join(path, "OASIS4_images")
     target_base = join(yucca_raw_data, task_name)
     target_imagesTr = join(target_base, "imagesTr")
 
     maybe_mkdir_p(target_imagesTr)
 
     """Populate Target Directory"""
 
     ext = ".nii.gz"
 
     skipped_volumes = []
     skipped_modalities = []
-
     for subject in tqdm(dirs_in_dir(subjects_dir), desc="Subjects"):
         if "mr" not in subject.lower():
             continue  # skip this subject
 
         subject_dir = join(subjects_dir, subject)
         for modality in dirs_in_dir(subject_dir):
-            modality_dir = join(subject_dir, modality)
             if should_skip(modality):
                 skipped_modalities.append(modality)
                 continue  # skip this modality
+            modality_dir = join(subject_dir, modality, "NIFTI")
             for file in subfiles(modality_dir, join=False, suffix=ext):
                 image_path = join(modality_dir, file)
-                file_name = file[: -len(ext)]
+                other_info = file[: -len(ext)].replace(subject, "").replace(modality, "")
                 vol = nib.load(image_path)
                 if should_use_volume(vol):
-                    output_name = f"{task_prefix}_{file_name}_000.nii.gz"
+                    output_name = f"{task_prefix}_{subject}_{modality}_{other_info}_000.nii.gz"
+                    print(output_name)
                     output_path = join(target_imagesTr, output_name)
                     shutil.copy2(image_path, output_path)
                 else:
                     skipped_volumes.append(image_path)
 
     print(f"Skipped {len(skipped_volumes)} and {len(skipped_modalities)}")
     print("Skipped workers", skipped_volumes)
     print("Skipped modalities", skipped_modalities)
 
     generate_dataset_json(
         join(target_base, "dataset.json"),
         target_imagesTr,
         imagesTs_dir=None,
         modalities=["MRI"],
-        labels=None,
+        labels={},
         dataset_name=task_name,
         license="https://www.oasis-brains.org/#access",
         dataset_description="Open Access Series of Imaging Studies (OASIS)",
         dataset_reference="https://www.oasis-brains.org",
     )
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task204_OASIS4.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task203_OASIS3.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,80 @@
 import shutil
-from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles, subdirs
-from yucca.task_conversion.utils import generate_dataset_json, should_use_volume
+from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
+from yucca.pipeline.task_conversion.utils import generate_dataset_json, dirs_in_dir, should_use_volume
 from yucca.paths import yucca_raw_data
 from tqdm import tqdm
 import nibabel as nib
 
 
+accept_modalities = ["t1", "t2", "mprage", "flair", "gre", "dwi", "swi", "grappa", "anat"]
 rejec_modalities = ["fmri", "func"]  # TODO: Might need to skip GRE
 
 
 def should_skip(modality: str):
     modality = modality.lower()
     for reject in rejec_modalities:
         if reject in modality:
             return True
-    return False
+    for accept in accept_modalities:
+        if accept in modality:
+            return False
+    return True
 
 
-def convert(path: str, subdir: str = "OASIS4"):
+def convert(path: str, subdir: str = "OASIS3"):
     """INPUT DATA - Define input path and suffixes"""
     path = join(path, subdir)
 
     """ OUTPUT DATA - Define the task name and prefix """
-    task_name = "Task204_OASIS4"
-    task_prefix = "OASIS4"
+    task_name = "Task203_OASIS3"
+    task_prefix = "OASIS3"
 
-    subjects_dir = join(path, "OASIS4_images")
+    subjects_dir = join(path, "DATA")
     target_base = join(yucca_raw_data, task_name)
     target_imagesTr = join(target_base, "imagesTr")
 
     maybe_mkdir_p(target_imagesTr)
 
     """Populate Target Directory"""
 
     ext = ".nii.gz"
 
     skipped_volumes = []
     skipped_modalities = []
-    for subject in tqdm(subdirs(subjects_dir), desc="Subjects"):
+
+    for subject in tqdm(dirs_in_dir(subjects_dir), desc="Subjects"):
         if "mr" not in subject.lower():
             continue  # skip this subject
 
         subject_dir = join(subjects_dir, subject)
-        for modality in subdirs(subject_dir):
+        for modality in dirs_in_dir(subject_dir):
+            modality_dir = join(subject_dir, modality)
             if should_skip(modality):
                 skipped_modalities.append(modality)
                 continue  # skip this modality
-            modality_dir = join(subject_dir, modality, "NIFTI")
             for file in subfiles(modality_dir, join=False, suffix=ext):
                 image_path = join(modality_dir, file)
-                file_name = file[: -len(ext)]
+                other_info = file[: -len(ext)].replace(subject, "").replace(modality, "")
                 vol = nib.load(image_path)
                 if should_use_volume(vol):
-                    output_name = f"{task_prefix}_{file_name}_000.nii.gz"
+                    output_name = f"{task_prefix}_{subject}_{modality}_{other_info}_000.nii.gz"
                     output_path = join(target_imagesTr, output_name)
                     shutil.copy2(image_path, output_path)
                 else:
                     skipped_volumes.append(image_path)
 
     print(f"Skipped {len(skipped_volumes)} and {len(skipped_modalities)}")
     print("Skipped workers", skipped_volumes)
     print("Skipped modalities", skipped_modalities)
 
     generate_dataset_json(
         join(target_base, "dataset.json"),
         target_imagesTr,
         imagesTs_dir=None,
         modalities=["MRI"],
-        labels={},
+        labels=None,
         dataset_name=task_name,
         license="https://www.oasis-brains.org/#access",
         dataset_description="Open Access Series of Imaging Studies (OASIS)",
         dataset_reference="https://www.oasis-brains.org",
     )
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task205_Hippocampus.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task205_Hippocampus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import shutil
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json, should_use_volume
+from yucca.pipeline.task_conversion.utils import generate_dataset_json, should_use_volume
 from yucca.paths import yucca_raw_data
 from tqdm import tqdm
 
 import nibabel as nib
 
 
 def convert(path: str, subdir: str = "decathlon/Task04_Hippocampus"):
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task206_BrainTumour.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task040_BraTS21_flair.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,84 @@
-from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subdirs
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
-from tqdm import tqdm
+from sklearn.model_selection import train_test_split
 import nibabel as nib
+import numpy as np
+import shutil
+from tqdm import tqdm
 
 
-def convert(path: str, subdir: str = "decathlon/Task01_BrainTumour"):
-    """INPUT DATA - Define input path and suffixes"""
-    path = join(path, subdir)
-    ext = ".nii.gz"
-
-    """ OUTPUT DATA - Define the task name and prefix """
-    task_name = "Task206_BrainTumour"
-    task_prefix = "BrainTumour"
-
-    """ Access the input data. If images are not split into train/test, and you wish to randomly
-    split the data, uncomment and adapt the following lines to fit your local path. """
+def convert(path: str, subdir: str = "brats21/training_data"):
+    # Target names
+    task_name = "Task040_BraTS21_flair"
+    task_prefix = "BraTS21"
 
-    # NOTE: We use the test set for pre-training, as the labels are no longer available, and we thus cannot use it for evaluation!
-    subjects_dir = join(path, "imagesTs")
+    ###OUTPUT DATA
+    # Target paths
     target_base = join(yucca_raw_data, task_name)
+
     target_imagesTr = join(target_base, "imagesTr")
+    target_labelsTr = join(target_base, "labelsTr")
 
-    maybe_mkdir_p(target_imagesTr)
+    target_imagesTs = join(target_base, "imagesTs")
+    target_labelsTs = join(target_base, "labelsTs")
 
-    """Populate Target Directory
-    This is also the place to apply any re-orientation, resampling and/or label correction."""
+    maybe_mkdir_p(target_imagesTr)
+    maybe_mkdir_p(target_labelsTs)
+    maybe_mkdir_p(target_imagesTs)
+    maybe_mkdir_p(target_labelsTr)
+
+    # INPUT DATA
+    # Input path and names
+    base_in = join(path, subdir)
+    file_suffix = ".nii.gz"
+
+    # Train/Test Splits
+    # We only use the train folder, as the test folder does not contain segmentations
+    # to obtain those, submission to the challenge is required (it's from 2008, forget it)
+    training_samples, test_samples = train_test_split(subdirs(base_in, join=False), random_state=4215532)
+
+    ###Populate Target Directory###
+    for sTr in tqdm(training_samples, desc="training"):
+        src_image_file_path1 = join(base_in, sTr, sTr + "_flair" + file_suffix)
+        dst_image_file_path1 = f"{target_imagesTr}/{task_prefix}_{sTr}_000.nii.gz"
+
+        dst_label_path = f"{target_labelsTr}/{task_prefix}_{sTr}.nii.gz"
+        label = nib.load(join(base_in, sTr, sTr + "_seg" + file_suffix))
+        labelarr = label.get_fdata()
+        labelarr[labelarr == 4.0] = 3.0
+        assert np.all(np.isin(np.unique(labelarr), np.array([0, 1, 2, 3])))
+        labelnew = nib.Nifti1Image(labelarr, label.affine, label.header, dtype=np.float32)
+        nib.save(labelnew, dst_label_path)
+
+        shutil.copy2(src_image_file_path1, dst_image_file_path1)
+
+    for sTs in tqdm(test_samples, desc="test"):
+        src_image_file_path1 = join(base_in, sTs, sTs + "_flair" + file_suffix)
+        dst_image_file_path1 = f"{target_imagesTs}/{task_prefix}_{sTs}_000.nii.gz"
+
+        dst_label_path = f"{target_labelsTs}/{task_prefix}_{sTs}.nii.gz"
+        label = nib.load(join(base_in, sTs, sTs + "_seg" + file_suffix))
+        labelarr = label.get_fdata()
+        labelarr[labelarr == 4.0] = 3.0
+        assert np.all(np.isin(np.unique(labelarr), np.array([0, 1, 2, 3])))
+        labelnew = nib.Nifti1Image(labelarr, label.affine, label.header, dtype=np.float32)
+        nib.save(labelnew, dst_label_path)
 
-    for file in tqdm(subfiles(subjects_dir, join=False, suffix=ext)):
-        image_path = join(subjects_dir, file)
-        file_name = file[6 : -len(ext)]  # remove the prefix BRATS_ and the suffix .nii.gz
-
-        vol = nib.load(image_path)
-
-        flair = vol.slicer[:, :, :, 0]
-        t1w = vol.slicer[:, :, :, 1]
-        t1gd = vol.slicer[:, :, :, 2]
-        t2w = vol.slicer[:, :, :, 3]
-
-        nib.save(flair, filename=f"{target_imagesTr}/{task_prefix}_{file_name}_flair_000.nii.gz")
-        nib.save(t1w, filename=f"{target_imagesTr}/{task_prefix}_{file_name}_t1w_000.nii.gz")
-        nib.save(t1gd, filename=f"{target_imagesTr}/{task_prefix}_{file_name}_t1gd_000.nii.gz")
-        nib.save(t2w, filename=f"{target_imagesTr}/{task_prefix}_{file_name}_t2w_000.nii.gz")
+        shutil.copy2(src_image_file_path1, dst_image_file_path1)
 
     generate_dataset_json(
         join(target_base, "dataset.json"),
         target_imagesTr,
-        imagesTs_dir=None,
-        modalities=["MRI"],
-        labels=None,
+        target_imagesTs,
+        ["FLAIR"],
+        labels={0: "background", 1: "necrotic tumor core", 2: "peritumoral edematous/invaded tissue", 3: "GD-enhancing tumor"},
         dataset_name=task_name,
-        license="CC-BY-SA 4.0",
-        dataset_description="Decathlon: Brain Tumour Segmentation",
-        dataset_reference="King's College London",
+        license="hands off!",
+        dataset_description="BraTS21",
+        dataset_reference="https://www.nitrc.org/projects/msseg, https://arxiv.org/abs/2206.06694",
     )
+
+
+if __name__ == "__main__":
+    convert()
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task207_ADNI.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task207_ADNI.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import gzip
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json, dirs_in_dir, should_use_volume
+from yucca.pipeline.task_conversion.utils import generate_dataset_json, dirs_in_dir, should_use_volume
 from yucca.paths import yucca_raw_data
 from tqdm import tqdm
 import shutil
 
 import nibabel as nib
 
 
@@ -41,19 +41,21 @@
             modality_dir = join(subject_dir, modality)
             for session in dirs_in_dir(modality_dir):
                 session_dir = join(modality_dir, session)
                 for id in dirs_in_dir(session_dir):
                     id_dir = join(session_dir, id)
                     for file in subfiles(id_dir, join=False, suffix=ext):
                         image_path = join(id_dir, file)
-                        file_name = file[: -len(ext)]
+                        other_info = (
+                            file[: -len(ext)].replace(subject, "").replace(modality, "").replace(session, "").replace(id, "")
+                        )
                         try:
                             vol = nib.load(image_path)
                             if should_use_volume(vol):
-                                output_name = f"{task_prefix}_{file_name}_000.nii.gz"
+                                output_name = f"{task_prefix}_{subject}_{modality}_{session}_{id}_{other_info}_000.nii.gz"
                                 output_path = join(target_imagesTr, output_name)
                                 image_file = open(image_path, "rb")
                                 shutil.copyfileobj(image_file, gzip.open(output_path, "wb"))
                             else:
                                 skipped.append(image_path)
                         except:
                             errors.append(image_path)
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task208_WMH.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task208_WMH.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import shutil
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfolders
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
 
 
 def convert(path: str, subdir: str = "WMH"):
     """INPUT DATA - Define input path and suffixes"""
     path = join(path, subdir)
 
@@ -37,16 +37,16 @@
         # test_samples = subfolders(test_folder, join=False)
 
         # First we add the data from the training folders
         for sTr in training_samples:
             # Loading relevant modalities and the ground truth
             src_flair_file_path = join(train_folder, sTr, "pre", "FLAIR.nii.gz")
             src_t1_file_path = join(train_folder, sTr, "pre", "T1.nii.gz")
-            dst_flair_file_path = f"{target_imagesTr}/{task_prefix}_flair_{sTr}_000.nii.gz"
-            dst_t1_file_path = f"{target_imagesTr}/{task_prefix}_t1_{sTr}_000.nii.gz"
+            dst_flair_file_path = f"{target_imagesTr}/{task_prefix}_{sTr}_flair_000.nii.gz"
+            dst_t1_file_path = f"{target_imagesTr}/{task_prefix}_{sTr}_t1_000.nii.gz"
             shutil.copy2(src_flair_file_path, dst_flair_file_path)
             shutil.copy2(src_t1_file_path, dst_t1_file_path)
 
         # Then we add the data from the original testing folders
         # if dataset == "Amsterdam":
         #   for site in test_samples:
         #       samples = subfolders(join(test_folder, site), join=False)
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task209_BraTS21.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task209_BraTS21.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
 import shutil
 from tqdm import tqdm
 from os.path import basename
 
 
 def convert(_path: str):
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task210_MSSEG1.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task210_MSSEG1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
 import shutil
 from tqdm import tqdm
 from os.path import basename
 
 
 def convert(_path: str):
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task241_BR41NS.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task241_BR41NS.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from yucca.task_conversion.utils import combine_images_from_tasks, generate_dataset_json
+from yucca.pipeline.task_conversion.utils import combine_images_from_tasks, generate_dataset_json
 from yucca.paths import yucca_raw_data
 
 
 def convert(_path: str, _subdir: str = None):
     # Define the name of the new task
     task_name = "Task241_BR41NS"
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task245_BRAINS-45K.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task245_BRAINS-45K.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from yucca.task_conversion.utils import combine_images_from_tasks, generate_dataset_json
+from yucca.pipeline.task_conversion.utils import combine_images_from_tasks, generate_dataset_json
 from yucca.paths import yucca_raw_data
 
 
 def convert(_path: str, _subdir: str = None):
     # Define the name of the new task
     task_name = "Task245_BRAINS-45K"
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task298_Combine_supervised.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task298_Combine_supervised.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from yucca.task_conversion.utils import combine_images_from_tasks, generate_dataset_json
+from yucca.pipeline.task_conversion.utils import combine_images_from_tasks, generate_dataset_json
 from yucca.paths import yucca_raw_data
 
 
 def convert(_path: str, _subdir: str = None):
     # Define the name of the new task
     task_name = "Task213_OASIS_Hammers"
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task299_Combine.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task299_Combine.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from yucca.task_conversion.utils import combine_images_from_tasks, generate_dataset_json
+from yucca.pipeline.task_conversion.utils import combine_images_from_tasks, generate_dataset_json
 from yucca.paths import yucca_raw_data
 
 
 def convert(_path: str, _subdir: str = None):
     # Define the name of the new task
     task_name = "Task299_Combine"
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task501_FetalPlanesDB.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task501_FetalPlanesDB.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p
 from yucca.paths import yucca_raw_data
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 
 
 def convert(path: str, subdir: str = "FETAL_PLANES_DB"):
     # INPUT DATA
 
     path = f"{path}/{subdir}"
     # file_suffix = ".png"
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task502_tiny_imagenet_200.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task502_tiny_imagenet_200.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 import pandas as pd
 import shutil
 from tqdm import tqdm
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subdirs, subfiles
 from yucca.paths import yucca_raw_data
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 
 
 def convert(path: str, subdir: str = "tiny-imagenet-200"):
     # INPUT DATA
 
     path = f"{path}/{subdir}"
     # file_suffix = ".png"
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task701_OASIS_NoLabel.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task701_OASIS_NoLabel.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, save_pickle
 
     maybe_mkdir_p(join(yucca_preprocessing_dir, task_name))
     save_pickle(splits, join(yucca_preprocessing_dir, task_name, 'splits.pkl'))
 """
 
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 import shutil
 import gzip
 from yucca.paths import yucca_raw_data
 from tqdm import tqdm
 
 
 def convert(path: str, subdir: str = "OASIS"):
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task901_SONAI_NoLabel.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task901_SONAI_NoLabel.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Task_conversion file for the SONAI data, without labels and with 2D jpg images (cache).
 """
 
 import shutil
 from tqdm import tqdm
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p
 from yucca.paths import yucca_raw_data
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 
 
 def convert(path: str, txt_file_prefix: str = "data"):
     """
     Converts the SONAI image chache to the Yucca format.
 
     We are abusing the subdir argument to specify a file with the label paths.
```

### Comparing `yucca-1.0.2/yucca/task_conversion/Task902_SONAI100k_NoLabel.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/Task902_SONAI100k_NoLabel.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Task_conversion file for the SONAI data, without labels and with 2D jpg images (cache).
 """
 
 import shutil
 from tqdm import tqdm
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p
 from yucca.paths import yucca_raw_data
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 
 
 def convert(path: str, txt_file_prefix: str = "sonai_100k"):
     """
     Converts the SONAI image chache to the Yucca format.
 
     We are abusing the subdir argument to specify a file with the label paths.
```

### Comparing `yucca-1.0.2/yucca/task_conversion/template.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import shutil
 import gzip
 from sklearn.model_selection import train_test_split
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 from yucca.paths import yucca_raw_data
 
 
 def convert(path: str, subdir: str = "MyDataset"):
     """INPUT DATA - Define input path and suffixes"""
     path = join(path, subdir)
     file_suffix = ".nii"
```

### Comparing `yucca-1.0.2/yucca/task_conversion/template_combine_imagesTr.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/template_combine_imagesTr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from yucca.task_conversion.utils import combine_imagesTr_from_tasks, generate_dataset_json
+from yucca.pipeline.task_conversion.utils import combine_imagesTr_from_tasks, generate_dataset_json
 from yucca.paths import yucca_raw_data
 
 
 # Define the name of the new task
 task_name = "TaskXXX_MyCombinedTask"
 
 # Define the expected labels (leave empty for no labels)
```

### Comparing `yucca-1.0.2/yucca/task_conversion/template_multiprocessing.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/template_multiprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from batchgenerators.utilities.file_and_folder_operations import join, maybe_mkdir_p, subfiles
-from yucca.task_conversion.utils import generate_dataset_json
+from yucca.pipeline.task_conversion.utils import generate_dataset_json
 import shutil
 import gzip
 from yucca.paths import yucca_raw_data
 from multiprocessing import Pool
 
 
 def convert_case(sample, input_image_dir, input_label_dir, target_image_dir, target_label_dir, prefix, suffix):
```

### Comparing `yucca-1.0.2/yucca/task_conversion/utils.py` & `yucca-1.1.2/yucca/pipeline/task_conversion/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import os
 import shutil
+import nibabel as nib
 from yucca.paths import yucca_raw_data
 from typing import Literal
-from batchgenerators.utilities.file_and_folder_operations import save_json, subfiles, join
+from batchgenerators.utilities.file_and_folder_operations import save_json, subfiles, join, subdirs
 from tqdm import tqdm
-import nibabel as nib
 from pathlib import Path
 
 
 def combine_images_from_tasks(tasks: list, target_base: str, run_type: Literal["supervised", "unsupervised"]):
     assert len(tasks) > 0, "list of tasks empty"
     for task in tqdm(tasks):
         folders = ["imagesTr", "imagesTs", "labelsTr", "labelsTs"] if run_type == "supervised" else ["imagesTr"]
@@ -48,14 +48,19 @@
     return [f.name for f in p.iterdir() if f.is_file() and f.name[0] not in [".", "_"]]
 
 
 def should_use_volume(vol: nib.Nifti1Image):
     return not (np.any(np.array(vol.shape) < 15) or len(vol.shape) != 3 or np.array(vol.dataobj).min() < 0)
 
 
+def remove_punctuation_and_spaces(data: str):
+    data = data.replace(" ", "-").replace(",", "-").replace(".", "-")
+    return data
+
+
 def generate_dataset_json(
     output_file: str,
     imagesTr_dir: str,
     imagesTs_dir: str,
     modalities: dict,
     labels: dict,
     dataset_name: str,
@@ -111,7 +116,28 @@
 
     if not output_file.endswith("dataset.json"):
         print(
             "WARNING: output file name is not dataset.json! This may be intentional or not. You decide. "
             "Proceeding anyways..."
         )
     save_json(json_dict, os.path.join(output_file))
+
+
+def maybe_get_task_from_task_id(task_id: str | int):
+    task_id = str(task_id)
+    tasks = subdirs(yucca_raw_data, join=False)
+
+    # Check if name is already complete
+    if task_id in tasks:
+        return task_id
+
+    # If not, we try to recreate the name
+    # We use the raw_data folder as reference
+    for task in tasks:
+        if task_id.lower() in task.lower():
+            return task
+
+    # If we can't find anything we just return the original, on the offchance that the task does not exist in Raw Data while existing in e.g. Preprocessed
+    print(
+        f"Couldn't find a task called: {task_id} in the raw data folder: {yucca_raw_data}. If your task only exists in e.g. the Preprocessed folder things might still work."
+    )
+    return task_id
```

### Comparing `yucca-1.0.2/yucca/training/augmentation/YuccaAugmentationComposer.py` & `yucca-1.1.2/yucca/data/augmentation/YuccaAugmentationComposer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 from torchvision import transforms
-from yucca.image_processing.matrix_ops import get_max_rotated_size
-from yucca.image_processing.transforms.formatting import (
-    AddBatchDimension,
-    RemoveBatchDimension,
-)
-from yucca.image_processing.transforms.BiasField import BiasField
-from yucca.image_processing.transforms.Blur import Blur
-from yucca.image_processing.transforms.CopyImageToSeg import CopyImageToSeg
-from yucca.image_processing.transforms.Gamma import Gamma
-from yucca.image_processing.transforms.Ghosting import MotionGhosting
-from yucca.image_processing.transforms.Masking import Masking
-from yucca.image_processing.transforms.Mirror import Mirror
-from yucca.image_processing.transforms.Noise import (
-    AdditiveNoise,
-    MultiplicativeNoise,
-)
-from yucca.image_processing.transforms.Ringing import GibbsRinging
-from yucca.image_processing.transforms.sampling import DownsampleSegForDS
-from yucca.image_processing.transforms.SimulateLowres import SimulateLowres
-from yucca.image_processing.transforms.Spatial import Spatial
+from yucca.functional.array_operations.matrix_ops import get_max_rotated_size
+from yucca.data.augmentation.transforms.normalize import Normalize
+from yucca.data.augmentation.transforms.formatting import AddBatchDimension, RemoveBatchDimension, CollectMetadata
+from yucca.data.augmentation.transforms.BiasField import BiasField
+from yucca.data.augmentation.transforms.Blur import Blur
+from yucca.data.augmentation.transforms.copy_image_to_label import CopyImageToLabel
+from yucca.data.augmentation.transforms.Gamma import Gamma
+from yucca.data.augmentation.transforms.Ghosting import MotionGhosting
+from yucca.data.augmentation.transforms.Masking import Masking
+from yucca.data.augmentation.transforms.Mirror import Mirror
+from yucca.data.augmentation.transforms.Noise import AdditiveNoise, MultiplicativeNoise
+from yucca.data.augmentation.transforms.Ringing import GibbsRinging
+from yucca.data.augmentation.transforms.sampling import DownsampleSegForDS
+from yucca.data.augmentation.transforms.SimulateLowres import SimulateLowres
+from yucca.data.augmentation.transforms.Spatial import Spatial
 
 
 class YuccaAugmentationComposer:
     def __init__(
         self,
         patch_size: list | tuple,
         deep_supervision: bool = False,
@@ -35,41 +30,44 @@
         self.setup_default_params(is_2D, patch_size)
         self.apply_task_type_specific_preset(task_type_preset)
         self.overwrite_params(parameter_dict)
         self.train_transforms = self.compose_train_transforms()
         self.val_transforms = self.compose_val_transforms()
 
     def setup_default_params(self, is_2D, patch_size):
+        """
+        Default probabilities (all ON by default)
+        For augmentations with AUG_P_PER_SAMPLE, AUG_P_PER_CHANNEL and AUG_P_PER_AXIS they are applied in the following order:
+                for sample in dataset: # iterate over the batch
+         if p_per_sample > np.random.uniform():
+           for channel in sample: # iterate over the channel/modalities
+             if p_per_channel > np.random.uniform():
+               for axis in channel: # iterate over the h,w,d dimensions
+                 if p_per_axis > np.random.uniform():
+                   sample[channel, axis] = apply_aug(sample[channel, axis])
+        Therefore, to enable any augmentation the AUG_P_PER_SAMPLE must be > 0.
+        """
         print("Composing Transforms")
-        # Define whether we crop before or after applying augmentations
+
         # Define if the cropping performed during the spatial transform is random or always centered
         #   We have ALREADY selected a random crop when we prepared the case in the dataloader
         #   so unless you know what you're doing this should be disabled to avoid border artifacts
         self.random_crop = False
         self.mask_image_for_reconstruction = False
         self.patch_size = patch_size
         self.cval = "min"  # can be an int, float or a str in ['min', 'max']
+        self.clip_to_input_range = False  # ensures no augmentations go beyond the input range of the image/patch
+        self.normalize = False
 
         # label/segmentation transforms
         self.skip_label = False
         self.label_dtype = int
         self.copy_image_to_label = False
 
-        # Default probabilities (all ON by default)
-        # For augmentations with AUG_P_PER_SAMPLE, AUG_P_PER_CHANNEL and AUG_P_PER_AXIS they are applied in the following order:
-        #
-        # for sample in dataset: # iterate over the batch
-        #  if p_per_sample > np.random.uniform():
-        #    for channel in sample: # iterate over the channel/modalities
-        #      if p_per_channel > np.random.uniform():
-        #        for axis in channel: # iterate over the h,w,d dimensions
-        #          if p_per_axis > np.random.uniform():
-        #            sample[channel, axis] = apply_aug(sample[channel, axis])
-        # Therefore, to enable any augmentation the AUG_P_PER_SAMPLE must be > 0.
-
+        # default augmentation probabilities
         self.additive_noise_p_per_sample = 0.2
         self.biasfield_p_per_sample = 0.33
         self.blurring_p_per_sample = 0.2
         self.blurring_p_per_channel = 0.5
         self.elastic_deform_p_per_sample = 0.33
         self.gamma_p_per_sample = 0.2
         self.gamma_p_invert_image = 0.05
@@ -92,28 +90,30 @@
         self.blurring_sigma = (0.0, 1.0)
 
         self.elastic_deform_alpha = (200, 600)
         self.elastic_deform_sigma = (20, 30)
 
         self.gamma_range = (0.5, 2.0)
 
-        self.gibbs_ringing_cutfreq = (96, 129)
+        self.gibbs_ringing_cut_freq = (96, 129)
         self.gibbs_ringing_axes = (0, 2) if is_2D else (0, 3)
 
         self.mask_ratio = 0.5
 
         self.mirror_axes = (0, 1) if is_2D else (0, 1, 2)
 
         self.motion_ghosting_alpha = (0.85, 0.95)
-        self.motion_ghosting_numreps = (2, 11)
+        self.motion_ghosting_num_reps = (2, 11)
         self.motion_ghosting_axes = (0, 2) if is_2D else (0, 3)
 
         self.multiplicative_noise_mean = (0, 0)
         self.multiplicative_noise_sigma = (1e-3, 1e-4)
 
+        self.normalization_scheme = "volume_wise_znorm"
+
         self.rotation_x = (-30.0, 30.0)
         self.rotation_y = (-0.0, 0.0) if is_2D else (-30.0, 30.0)
         self.rotation_z = (-0.0, 0.0) if is_2D else (-30.0, 30.0)
 
         self.scale_factor = (0.9, 1.1)
 
         self.simulate_lowres_zoom_range = (0.5, 1.0)
@@ -125,39 +125,39 @@
             self._pre_aug_patch_size = get_max_rotated_size(self.patch_size)
         return self._pre_aug_patch_size
 
     def apply_task_type_specific_preset(self, preset):
         if preset == "segmentation":
             # we do nothing and use the default parameters
             pass
-
         elif preset == "classification":
             self.skip_label = True
-
         elif preset == "self-supervised":
             self.skip_label = True
             self.copy_image_to_label = True
             self.mask_image_for_reconstruction = True
-
         else:
             raise ValueError(f"{preset} is not a valid `task_type_preset`.")
 
     def overwrite_params(self, parameter_dict):
         for key, value in parameter_dict.items():
             setattr(self, key, value)
 
     def compose_train_transforms(self):
         tr_transforms = transforms.Compose(
             [
+                CollectMetadata(),
                 AddBatchDimension(),
+                # augmentations
                 Spatial(
                     patch_size=self.patch_size,
                     crop=True,
                     random_crop=self.random_crop,
                     cval=self.cval,
+                    clip_to_input_range=self.clip_to_input_range,
                     p_deform_per_sample=self.elastic_deform_p_per_sample,
                     deform_sigma=self.elastic_deform_sigma,
                     deform_alpha=self.elastic_deform_alpha,
                     p_rot_per_sample=self.rotation_p_per_sample,
                     p_rot_per_axis=self.rotation_p_per_axis,
                     x_rot_in_degrees=self.rotation_x,
                     y_rot_in_degrees=self.rotation_y,
@@ -166,67 +166,80 @@
                     scale_factor=self.scale_factor,
                     skip_label=self.skip_label,
                 ),
                 AdditiveNoise(
                     p_per_sample=self.additive_noise_p_per_sample,
                     mean=self.additive_noise_mean,
                     sigma=self.additive_noise_sigma,
+                    clip_to_input_range=self.clip_to_input_range,
                 ),
                 Blur(
                     p_per_sample=self.blurring_p_per_sample,
                     p_per_channel=self.blurring_p_per_channel,
                     sigma=self.blurring_sigma,
+                    clip_to_input_range=self.clip_to_input_range,
                 ),
                 MultiplicativeNoise(
                     p_per_sample=self.multiplicative_noise_p_per_sample,
                     mean=self.multiplicative_noise_mean,
                     sigma=self.multiplicative_noise_sigma,
+                    clip_to_input_range=self.clip_to_input_range,
                 ),
                 MotionGhosting(
                     p_per_sample=self.motion_ghosting_p_per_sample,
                     alpha=self.motion_ghosting_alpha,
-                    numReps=self.motion_ghosting_numreps,
+                    num_reps=self.motion_ghosting_num_reps,
                     axes=self.motion_ghosting_axes,
+                    clip_to_input_range=self.clip_to_input_range,
                 ),
                 GibbsRinging(
                     p_per_sample=self.gibbs_ringing_p_per_sample,
-                    cutFreq=self.gibbs_ringing_cutfreq,
+                    cut_freq=self.gibbs_ringing_cut_freq,
                     axes=self.gibbs_ringing_axes,
+                    clip_to_input_range=self.clip_to_input_range,
                 ),
                 SimulateLowres(
                     p_per_sample=self.simulate_lowres_p_per_sample,
                     p_per_channel=self.simulate_lowres_p_per_channel,
                     p_per_axis=self.simulate_lowres_p_per_axis,
                     zoom_range=self.simulate_lowres_zoom_range,
+                    clip_to_input_range=self.clip_to_input_range,
+                ),
+                BiasField(
+                    p_per_sample=self.biasfield_p_per_sample,
+                    clip_to_input_range=self.clip_to_input_range,
                 ),
-                BiasField(p_per_sample=self.biasfield_p_per_sample),
                 Gamma(
                     p_per_sample=self.gamma_p_per_sample,
                     p_invert_image=self.gamma_p_invert_image,
                     gamma_range=self.gamma_range,
+                    clip_to_input_range=self.clip_to_input_range,
                 ),
                 Mirror(
                     p_per_sample=self.mirror_p_per_sample,
                     axes=self.mirror_axes,
                     p_mirror_per_axis=self.mirror_p_per_axis,
                     skip_label=self.skip_label,
                 ),
+                Normalize(normalize=self.normalize, scheme=self.normalization_scheme),
+                # seg
+                CopyImageToLabel(copy=self.copy_image_to_label),
                 DownsampleSegForDS(deep_supervision=self.deep_supervision),
-                CopyImageToSeg(copy=self.copy_image_to_label),
+                # mae
                 Masking(mask=self.mask_image_for_reconstruction, pixel_value=self.cval, ratio=self.mask_ratio),
                 RemoveBatchDimension(),
             ]
         )
         return tr_transforms
 
     def compose_val_transforms(self):
         val_transforms = transforms.Compose(
             [
                 AddBatchDimension(),
-                CopyImageToSeg(copy=self.copy_image_to_label),
+                CopyImageToLabel(copy=self.copy_image_to_label),
                 Masking(mask=self.mask_image_for_reconstruction, pixel_value=self.cval, ratio=self.mask_ratio),
                 RemoveBatchDimension(),
             ]
         )
         return val_transforms
 
     def lm_hparams(self):
@@ -251,23 +264,23 @@
                 "elastic_deform_p_per_sample": self.elastic_deform_p_per_sample,
                 "elastic_deform_alpha": self.elastic_deform_alpha,
                 "elastic_deform_sigma": self.elastic_deform_sigma,
                 "gamma_p_per_sample": self.gamma_p_per_sample,
                 "gamma_p_invert_image": self.gamma_p_invert_image,
                 "gamma_range": self.gamma_range,
                 "gibbs_ringing_p_per_sample": self.gibbs_ringing_p_per_sample,
-                "gibbs_ringing_cutfreq": self.gibbs_ringing_cutfreq,
+                "gibbs_ringing_cut_freq": self.gibbs_ringing_cut_freq,
                 "gibbs_ringing_axes": self.gibbs_ringing_axes,
                 "mask_ratio": self.mask_ratio,
                 "mirror_p_per_sample": self.mirror_p_per_sample,
                 "mirror_p_per_axis": self.mirror_p_per_axis,
                 "mirror_axes": self.mirror_axes,
                 "motion_ghosting_p_per_sample": self.motion_ghosting_p_per_sample,
                 "motion_ghosting_alpha": self.motion_ghosting_alpha,
-                "motion_ghosting_numreps": self.motion_ghosting_numreps,
+                "motion_ghosting_num_reps": self.motion_ghosting_num_reps,
                 "motion_ghosting_axes": self.motion_ghosting_axes,
                 "multiplicative_noise_p_per_sample": self.multiplicative_noise_p_per_sample,
                 "multiplicative_noise_mean": self.multiplicative_noise_mean,
                 "multiplicative_noise_sigma": self.multiplicative_noise_sigma,
                 "rotation_p_per_sample": self.rotation_p_per_sample,
                 "rotation_p_per_axis": self.rotation_p_per_axis,
                 "rotation_x": self.rotation_x,
@@ -281,13 +294,41 @@
                 "simulate_lowres_zoom_range": self.simulate_lowres_zoom_range,
             }
         }
         return hparams
 
 
 if __name__ == "__main__":
-    from yucca.training.augmentation.augmentation_presets import basic
+    from yucca.data.augmentation.augmentation_presets import all_always
+    import numpy as np
 
-    x = YuccaAugmentationComposer(patch_size=(32, 32), parameter_dict=basic)
-    print("ALL AUGMENTATION PARAMETERS: ", x.lm_hparams())
-    print("")
-    print("BASIC PARAMETERS: ", basic)
+    print("NO CLIPPING")
+    augs = all_always
+    augs["clip_to_input_range"] = False
+    x = YuccaAugmentationComposer(patch_size=(32, 32, 32), parameter_dict=augs)
+    ttf = x.train_transforms
+    mns = []
+    for i in range(100):
+        arr = np.random.randn(1, 32, 32, 32)
+        arr = (arr - arr.min()) / (arr.max() - arr.min())
+        mn = arr.min()
+        mx = arr.max()
+        arr = ttf({"image": arr})["image"]
+        # print(f"BEFORE: min: {mn} max: {mx} AFTER: min: {arr.min()} max: {arr.max()}")
+        mns.append(arr.min())
+    print("no clip min:", np.min(mns))
+
+    print("WITH CLIPPING")
+    augs = all_always
+    augs["clip_to_input_range"] = True
+    x = YuccaAugmentationComposer(patch_size=(32, 32, 32), parameter_dict=augs)
+    ttf = x.train_transforms
+    mns = []
+    for i in range(100):
+        arr = np.random.randn(1, 32, 32, 32)
+        arr = (arr - arr.min()) / (arr.max() - arr.min())
+        mn = arr.min()
+        mx = arr.max()
+        arr = ttf({"image": arr})["image"]
+        # print(f"BEFORE: min: {mn} max: {mx} AFTER: min: {arr.min()} max: {arr.max()}")
+        mns.append(arr.min())
+    print("with clip min:", np.min(mns))
```

### Comparing `yucca-1.0.2/yucca/training/configuration/configure_callbacks.py` & `yucca-1.1.2/yucca/pipeline/configuration/configure_callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 from lightning.pytorch.loggers.logger import Logger
 from typing import Optional, Union
 from dataclasses import dataclass
 from lightning.pytorch.callbacks import ModelCheckpoint, LearningRateMonitor
 from lightning.pytorch.profilers import AdvancedProfiler
 from lightning.pytorch.loggers import WandbLogger
-from yucca.evaluation.loggers import YuccaLogger
-from yucca.utils.saving import WritePredictionFromLogits
-from yucca.paths import yucca_wandb_entity
 from lightning.pytorch.profilers.profiler import Profiler
+from yucca.callbacks.loggers import YuccaLogger
+from yucca.callbacks.prediction_writer import WritePredictionFromLogits
+from yucca.paths import yucca_wandb_entity
 
 
 @dataclass
 class CallbackConfig:
     callbacks: list
     loggers: list
     profiler: Profiler
```

### Comparing `yucca-1.0.2/yucca/training/configuration/configure_checkpoint.py` & `yucca-1.1.2/yucca/pipeline/configuration/configure_checkpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 from batchgenerators.utilities.file_and_folder_operations import join, isfile
 from dataclasses import dataclass
 from typing import Union
-from yucca.training.configuration.configure_paths import PathConfig
-from yucca.utils.dict import without_keys
+from yucca.pipeline.configuration.configure_paths import PathConfig
+from yucca.functional.utils.dict import without_keys
 import logging
 
 
 @dataclass
 class CkptConfig:
     """
     This class serves to preserve information between runs and should thus be extended to include
```

### Comparing `yucca-1.0.2/yucca/training/configuration/configure_input_dims.py` & `yucca-1.1.2/yucca/pipeline/configuration/configure_input_dims.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 from typing import Tuple, Union, Optional, Literal, Iterable
-from yucca.network_architectures.utils.model_memory_estimation import find_optimal_tensor_dims
+from yucca.networks.utils.model_memory_estimation import find_optimal_tensor_dims
 import logging
 
 
 @dataclass
 class InputDimensionsConfig:
     batch_size: int
     patch_size: Union[Tuple[int, int], Tuple[int, int, int]]
```

### Comparing `yucca-1.0.2/yucca/training/configuration/configure_paths.py` & `yucca-1.1.2/yucca/pipeline/configuration/configure_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from batchgenerators.utilities.file_and_folder_operations import join, isdir, subdirs, maybe_mkdir_p
 from dataclasses import dataclass
 from typing import Union
 from yucca.paths import yucca_models, yucca_preprocessed_data
-from yucca.training.configuration.configure_task import TaskConfig
+from yucca.pipeline.configuration.configure_task import TaskConfig
 
 
 @dataclass
 class PathConfig:
     plans_path: str
     save_dir: str
     task_dir: str
```

### Comparing `yucca-1.0.2/yucca/training/configuration/configure_plans.py` & `yucca-1.1.2/yucca/pipeline/configuration/configure_plans.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import yucca
 from batchgenerators.utilities.file_and_folder_operations import join, load_json
 from dataclasses import dataclass
 from typing import Union, Literal
-from yucca.preprocessing.UnsupervisedPreprocessor import UnsupervisedPreprocessor
-from yucca.preprocessing.ClassificationPreprocessor import ClassificationPreprocessor
-from yucca.utils.dict import without_keys
-from yucca.utils.files_and_folders import recursive_find_python_class
+from yucca.pipeline.preprocessing.UnsupervisedPreprocessor import UnsupervisedPreprocessor
+from yucca.pipeline.preprocessing.ClassificationPreprocessor import ClassificationPreprocessor
+from yucca.functional.utils.dict import without_keys
+from yucca.functional.utils.files_and_folders import recursive_find_python_class
 import logging
 
 
 @dataclass
 class PlanConfig:
+    allow_missing_modalities: bool
     image_extension: str
     num_classes: int
     plans: dict
     task_type: str
 
     def lm_hparams(self, without: [] = []):
         hparams = {
+            "allow_missing_modalities": self.allow_missing_modalities,
             "image_extension": self.image_extension,
             "num_classes": self.num_classes,
             "plans": self.plans,
             "task_type": self.task_type,
         }
         return without_keys(hparams, without)
 
@@ -40,18 +42,23 @@
     if stage == "predict":
         # In this case we don't want to rely on plans being found in the preprocessed folder,
         # as it might not exist.
         assert ckpt_plans is not None
         plans = ckpt_plans
 
     task_type = setup_task_type(plans)
-    num_classes = max(1, plans.get("num_classes") or len(plans["dataset_properties"]["classes"]))
+    if task_type == "self-supervised":
+        num_classes = max(1, plans.get("num_modalities") or len(plans["dataset_properties"]["modalities"]))
+    else:
+        num_classes = max(1, plans.get("num_classes") or len(plans["dataset_properties"]["classes"]))
     image_extension = plans.get("image_extension") or plans["dataset_properties"].get("image_extension") or "nii.gz"
+    allow_missing_modalities = plans.get("allow_missing_modalities") or False
 
     return PlanConfig(
+        allow_missing_modalities=allow_missing_modalities,
         image_extension=image_extension,
         num_classes=num_classes,
         plans=plans,
         task_type=task_type,
     )
 
 
@@ -66,18 +73,23 @@
             plan.pop(key)
         elif key in plan["dataset_properties"]:
             plan["dataset_properties"].pop(key)
     return plan
 
 
 def setup_task_type(plans):
+    if plans.get("task_type"):
+        task_type = plans.get("task_type")
+        return task_type
+
+    # If key is not present in plan then we try to infer the task_type from the Type of Preprocessor
     preprocessor_class = recursive_find_python_class(
-        folder=[join(yucca.__path__[0], "preprocessing")],
+        folder=[join(yucca.__path__[0], "pipeline", "preprocessing")],
         class_name=plans["preprocessor"],
-        current_module="yucca.preprocessing",
+        current_module="yucca.pipeline.preprocessing",
     )
     assert (
         preprocessor_class
     ), f"{plans['preprocessor']} was found in plans, but no class with the corresponding name was found"
     if issubclass(preprocessor_class, ClassificationPreprocessor):
         task_type = "classification"
     elif issubclass(preprocessor_class, UnsupervisedPreprocessor):
```

### Comparing `yucca-1.0.2/yucca/training/configuration/configure_seed.py` & `yucca-1.1.2/yucca/pipeline/configuration/configure_seed.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/training/configuration/configure_task.py` & `yucca-1.1.2/yucca/pipeline/configuration/configure_task.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/training/configuration/split_data.py` & `yucca-1.1.2/yucca/pipeline/configuration/split_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import math
 from typing import Union
 import numpy as np
-from batchgenerators.utilities.file_and_folder_operations import join, subfiles, isfile, save_pickle, load_pickle
+from batchgenerators.utilities.file_and_folder_operations import join, isfile, save_pickle, load_pickle
 from sklearn.model_selection import KFold
 from dataclasses import dataclass
-from yucca.training.configuration.configure_paths import PathConfig
+from yucca.functional.utils.files_and_folders import subfiles
+from yucca.pipeline.configuration.configure_paths import PathConfig
 
 
 @dataclass
 class SplitConfig:
     splits: Union[dict[dict[list[dict]]], None] = None  # Contains `{ method: { parameter_value: [splits] }}`
     method: str = None
     param: Union[int, float] = None
@@ -91,15 +92,15 @@
     num_val = math.ceil(len(file_names) * p)
     if num_val < 10:
         logging.warning("The validation split is very small. Consider using a higher `p`.")
     return [{"train": list(file_names[num_val:]), "val": list(file_names[:num_val])}]
 
 
 def get_file_names(train_data_dir):
-    file_names = subfiles(train_data_dir, join=False, suffix=".npy")
+    file_names = subfiles(train_data_dir, join=False, remove_extension=True, suffix=".npy")
     if not file_names:
-        file_names = subfiles(train_data_dir, join=False, suffix=".npz")
+        file_names = subfiles(train_data_dir, join=False, remove_extension=True, suffix=".npz")
         if file_names:
             logging.warning("Only found compressed (.npz) files. This might increase runtime.")
 
     assert file_names, f"Couldn't find any .npy or .npz files in {train_data_dir}"
     return np.array(file_names)
```

### Comparing `yucca-1.0.2/yucca/training/data_loading/YuccaDataModule.py` & `yucca-1.1.2/yucca/data/data_modules/YuccaDataModule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import lightning as pl
 import torchvision
 import logging
 import torch
 from typing import Literal, Optional, Union
 from torch.utils.data import DataLoader, Sampler
 from batchgenerators.utilities.file_and_folder_operations import join
-from yucca.training.configuration.configure_input_dims import InputDimensionsConfig
-from yucca.training.configuration.split_data import SplitConfig
-from yucca.training.data_loading.YuccaDataset import YuccaTestDataset, YuccaTrainDataset
-from yucca.training.data_loading.samplers import InfiniteRandomSampler
+from yucca.pipeline.configuration.configure_input_dims import InputDimensionsConfig
+from yucca.pipeline.configuration.split_data import SplitConfig
+from yucca.data.datasets.YuccaDataset import YuccaTestDataset, YuccaTrainDataset
+from yucca.data.samplers import InfiniteRandomSampler
 
 
 class YuccaDataModule(pl.LightningDataModule):
     """
     The YuccaDataModule class is a PyTorch Lightning DataModule designed for handling data loading
     and preprocessing in the context of the Yucca project.
 
@@ -44,57 +44,66 @@
         This can potentially avoid dark or low-intensity areas at the borders and it also helps mitigate the risk of
         introducing artifacts during data augmentation, especially in regions where interpolation may have a significant impact.
     """
 
     def __init__(
         self,
         input_dims_config: InputDimensionsConfig,
-        image_extension: str,
+        allow_missing_modalities: Optional[bool] = False,
+        image_extension: Optional[str] = None,
         composed_train_transforms: Optional[torchvision.transforms.Compose] = None,
         composed_val_transforms: Optional[torchvision.transforms.Compose] = None,
         num_workers: Optional[int] = None,
         overwrite_predictions: bool = False,
         pred_data_dir: Optional[str] = None,
         pred_save_dir: Optional[str] = None,
         pre_aug_patch_size: Optional[Union[list, tuple]] = None,
         splits_config: Optional[SplitConfig] = None,
         split_idx: Optional[int] = None,
         task_type: Optional[str] = None,
+        test_dataset_class: Optional[torch.utils.data.Dataset] = YuccaTestDataset,
+        train_data_dir: Optional[str] = None,
+        train_dataset_class: Optional[torch.utils.data.Dataset] = YuccaTrainDataset,
         train_sampler: Optional[Sampler] = InfiniteRandomSampler,
         val_sampler: Optional[Sampler] = InfiniteRandomSampler,
-        train_data_dir: Optional[str] = None,
     ):
         super().__init__()
 
         # extract parameters
         self.batch_size = input_dims_config.batch_size
         self.patch_size = input_dims_config.patch_size
         self.image_extension = image_extension
         self.task_type = task_type
 
         self.split_idx = split_idx
         self.splits_config = splits_config
         self.train_data_dir = train_data_dir
 
         # Set by initialize()
+        self.allow_missing_modalities = allow_missing_modalities
         self.composed_train_transforms = composed_train_transforms
         self.composed_val_transforms = composed_val_transforms
         self.pre_aug_patch_size = pre_aug_patch_size
 
         # Set in the predict loop
         self.overwrite_predictions = overwrite_predictions
         self.pred_data_dir = pred_data_dir
         self.pred_save_dir = pred_save_dir
 
         # Set default values
         self.num_workers = max(0, int(torch.get_num_threads() - 1)) if num_workers is None else num_workers
         self.val_num_workers = self.num_workers
+        self.test_dataset_class = test_dataset_class
         self.train_sampler = train_sampler
+        self.train_dataset_class = train_dataset_class
         self.val_sampler = val_sampler
         logging.info(f"Using {self.num_workers} workers")
+        logging.info(
+            f"Using dataset class: {self.train_dataset_class} for train/val and {self.test_dataset_class} for inference"
+        )
 
     def setup(self, stage: Literal["fit", "test", "predict"]):
         logging.info(f"Setting up data for stage: {stage}")
         expected_stages = ["fit", "test", "predict"]
         assert stage in expected_stages, "unexpected stage. " f"Expected: {expected_stages} and found: {stage}"
 
         # Assign train/val datasets for use in dataloaders
@@ -109,33 +118,37 @@
 
             if len(self.train_samples) < 100:
                 logging.info(f"Training on samples: {self.train_samples}")
 
             if len(self.val_samples) < 100:
                 logging.info(f"Validating on samples: {self.val_samples}")
 
-            self.train_dataset = YuccaTrainDataset(
+            self.train_dataset = self.train_dataset_class(
                 self.train_samples,
                 composed_transforms=self.composed_train_transforms,
                 patch_size=self.pre_aug_patch_size if self.pre_aug_patch_size is not None else self.patch_size,
                 task_type=self.task_type,
+                allow_missing_modalities=self.allow_missing_modalities,
             )
 
-            self.val_dataset = YuccaTrainDataset(
+            self.val_dataset = self.train_dataset_class(
                 self.val_samples,
                 composed_transforms=self.composed_val_transforms,
                 patch_size=self.patch_size,
                 task_type=self.task_type,
+                allow_missing_modalities=self.allow_missing_modalities,
             )
 
         if stage == "predict":
-            assert self.pred_data_dir is not None, "set a pred_data_dir for inference to work"
+            assert self.pred_data_dir is not None, "`pred_data_dir` is required in inference"
+            assert self.pred_save_dir is not None, "`pred_save_dir` is required in inference"
+            assert self.image_extension is not None, "`image_extension` is required in inference"
             # This dataset contains ONLY the images (and not the labels)
             # It will return a tuple of (case, case_id)
-            self.pred_dataset = YuccaTestDataset(
+            self.pred_dataset = self.test_dataset_class(
                 self.pred_data_dir,
                 pred_save_dir=self.pred_save_dir,
                 overwrite_predictions=self.overwrite_predictions,
                 suffix=self.image_extension,
             )
 
     def train_dataloader(self):
```

### Comparing `yucca-1.0.2/yucca/training/data_loading/YuccaDataset.py` & `yucca-1.1.2/yucca/data/datasets/YuccaDataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import numpy as np
 import torch
 import os
-from typing import Union, Literal, Optional
 import logging
-from batchgenerators.utilities.file_and_folder_operations import subfiles, load_pickle
-from yucca.image_processing.transforms.cropping_and_padding import CropPad
-from yucca.image_processing.transforms.formatting import NumpyToTorch
+from typing import Union, Literal, Optional
+from batchgenerators.utilities.file_and_folder_operations import subfiles, load_pickle, isfile
+from yucca.data.augmentation.transforms.cropping_and_padding import CropPad
+from yucca.data.augmentation.transforms.formatting import NumpyToTorch
 
 
 class YuccaTrainDataset(torch.utils.data.Dataset):
     def __init__(
         self,
         samples: list,
         patch_size: list | tuple,
         keep_in_ram: Union[bool, None] = None,
         label_dtype: Optional[Union[int, float]] = None,
         composed_transforms=None,
         task_type: Literal["classification", "segmentation", "self-supervised", "contrastive"] = "segmentation",
+        allow_missing_modalities=False,
     ):
         self.all_cases = samples
         self.composed_transforms = composed_transforms
         self.patch_size = patch_size
         self.task_type = task_type
         assert task_type in ["classification", "segmentation", "self-supervised", "contrastive"]
+        self.supervised = self.task_type in ["classification", "segmentation"]
         self.label_dtype = label_dtype
+        self.allow_missing_modalities = allow_missing_modalities
 
         self.already_loaded_cases = {}
 
         # for segmentation and classification we override the default None
         # because arrays are saved as floats and we want them to be ints.
         if self.label_dtype is None:
-            if self.task_type in ["segmentation", "classification"]:
+            if self.supervised:
                 self.label_dtype = torch.int32
 
         self.croppad = CropPad(patch_size=self.patch_size, p_oversample_foreground=0.33)
         self.to_torch = NumpyToTorch(label_dtype=self.label_dtype)
 
         self._keep_in_ram = keep_in_ram
 
@@ -45,81 +48,107 @@
         if len(self.all_cases) < 50:
             self._keep_in_ram = True
         else:
             logging.debug("Large dataset detected. Will not keep cases in RAM during training.")
             self._keep_in_ram = False
         return self._keep_in_ram
 
-    def load_and_maybe_keep_pickle(self, picklepath):
+    def load_and_maybe_keep_pickle(self, path):
+        path = path + ".pkl"
         if not self.keep_in_ram:
-            return load_pickle(picklepath)
-        if picklepath in self.already_loaded_cases:
-            return self.already_loaded_cases[picklepath]
-        self.already_loaded_cases[picklepath] = load_pickle(picklepath)
-        return self.already_loaded_cases[picklepath]
+            return load_pickle(path)
+        if path in self.already_loaded_cases:
+            return self.already_loaded_cases[path]
+        self.already_loaded_cases[path] = load_pickle(path)
+        return self.already_loaded_cases[path]
 
     def load_and_maybe_keep_volume(self, path):
+        path = path + ".npy"
         if not self.keep_in_ram:
-            if path[-3:] == "npy":
+            if isfile(path):
                 try:
                     return np.load(path, "r")
                 except ValueError:
                     return np.load(path, allow_pickle=True)
-            image = np.load(path)
-            assert len(image.files) == 1, (
-                "More than one entry in data array. " f"Should only be ['data'] but is {[key for key in image.files]}"
-            )
-            return image[image.files[0]]
-
-        if path in self.already_loaded_cases:
-            return self.already_loaded_cases[path]
+            else:
+                print("uncompressed data was not found.")
 
-        if path[-3:] == "npy":
+        if isfile(path):
+            if path in self.already_loaded_cases:
+                return self.already_loaded_cases[path]
             try:
                 self.already_loaded_cases[path] = np.load(path, "r")
             except ValueError:
                 self.already_loaded_cases[path] = np.load(path, allow_pickle=True)
-            return self.already_loaded_cases[path]
+        else:
+            print("uncompressed data was not found.")
 
-        image = np.load(path)
-        assert len(image.files) == 1, (
-            "More than one entry in data array. " f"Should only be ['data'] but is {[key for key in image.files]}"
-        )
-        self.already_loaded_cases = image[image.files[0]]
         return self.already_loaded_cases[path]
 
     def __len__(self):
         return len(self.all_cases)
 
     def __getitem__(self, idx):
-        case = self.all_cases[idx]
+        # remove extension if file splits include extensions
+        case, _ = os.path.splitext(self.all_cases[idx])
         data = self.load_and_maybe_keep_volume(case)
+        metadata = self.load_and_maybe_keep_pickle(case)
+
+        if self.allow_missing_modalities:
+            image, label = self.unpack_with_zeros(data, supervised=self.supervised)
+        else:
+            image, label = self.unpack(data, supervised=self.supervised)
+
         data_dict = {"file_path": case}  # metadata that can be very useful for debugging.
-        if self.task_type == "classification":
-            data_dict.update({"image": data[:-1][0], "label": data[-1:][0]})
-        elif self.task_type == "segmentation":
-            data_dict.update({"image": data[:-1], "label": data[-1:]})
+        if self.task_type in ["classification", "segmentation"]:
+            data_dict.update({"image": image, "label": label})
         elif self.task_type == "self-supervised":
-            data_dict.update({"image": data})
+            data_dict.update({"image": image})
         elif self.task_type == "contrastive":
-            view1 = self._transform({"image": data}, case)["image"]
-            view2 = self._transform({"image": data}, case)["image"]
+            view1 = self._transform({"image": image}, case)["image"]
+            view2 = self._transform({"image": image}, case)["image"]
             data_dict.update({"image": (view1, view2)})
             return data_dict
         else:
             logging.error(f"Task Type not recognized. Found {self.task_type}")
-        return self._transform(data_dict, case)
+        return self._transform(data_dict, metadata)
 
-    def _transform(self, data_dict, case):
-        metadata = self.load_and_maybe_keep_pickle(case[: -len(".npy")] + ".pkl")
+    def _transform(self, data_dict, metadata):
         data_dict = self.croppad(data_dict, metadata)
         if self.composed_transforms is not None:
             data_dict = self.composed_transforms(data_dict)
         return self.to_torch(data_dict)
 
+    def unpack(self, data, supervised: bool):
+        if supervised:
+            return data[:-1], data[-1:]
+        return data, None
+
+    def unpack_with_zeros(self, data, supervised: bool):
+        assert data.dtype == "object", "allow missing modalities is true but dtype is not object"
+
+        # First find the array with the largest array.
+        # in classification this avoids setting the zero array to the 1d array with classes
+        sizes = [i.size for i in data]
+        idx_largest_array = np.where(sizes == np.max(sizes))[0][0]
+
+        # replace missing modalities with zero-filed arrays
+        for idx, i in enumerate(data):
+            if i.size == 0:
+                data[idx] = np.zeros(data[idx_largest_array].squeeze().shape)
+
+        # unpack array into images and (maybe) labels
+        if supervised:
+            images = np.array([mod for mod in data[:-1]])
+            label = data[-1:][0]
+        else:
+            images = np.array([mod for mod in data])
+            label = None
+        return images, label
+
 
 class YuccaTestDataset(torch.utils.data.Dataset):
     def __init__(self, raw_data_dir: str, pred_save_dir: str, overwrite_predictions: bool = False, suffix="nii.gz"):
         self.data_path = raw_data_dir
         self.pred_save_dir = pred_save_dir
         self.overwrite = overwrite_predictions
         self.suffix = suffix
@@ -152,13 +181,13 @@
         return case, case_id
 
 
 if __name__ == "__main__":
     import torch
     from yucca.paths import yucca_preprocessed_data
     from batchgenerators.utilities.file_and_folder_operations import join
-    from yucca.training.data_loading.samplers import InfiniteRandomSampler
+    from yucca.data.samplers import InfiniteRandomSampler
 
     files = subfiles(join(yucca_preprocessed_data, "Task001_OASIS/YuccaPlanner"), suffix="npy")
     ds = YuccaTrainDataset(files, patch_size=(12, 12, 12))
     sampler = InfiniteRandomSampler(ds)
     dl = torch.utils.data.DataLoader(ds, num_workers=2, batch_size=2, sampler=sampler)
```

### Comparing `yucca-1.0.2/yucca/training/data_loading/samplers.py` & `yucca-1.1.2/yucca/data/samplers.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/training/lightning_modules/YuccaLightningModule.py` & `yucca-1.1.2/yucca/lightning_modules/YuccaLightningModule.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 import copy
 import logging
 import numpy as np
 import os
 import matplotlib.pyplot as plt
 from batchgenerators.utilities.file_and_folder_operations import join
 from torchmetrics import MetricCollection
-from torchmetrics.classification import Dice, Accuracy, AUROC
+from torchmetrics.classification import Dice
 from torchmetrics.regression import MeanAbsoluteError
-from yucca.training.loss_and_optim.loss_functions.deep_supervision import DeepSupervisionLoss
-from yucca.utils.files_and_folders import recursive_find_python_class
-from yucca.utils.kwargs import filter_kwargs
-from yucca.evaluation.training_metrics import F1
+from yucca.optimization.loss_functions.deep_supervision import DeepSupervisionLoss
+from yucca.functional.utils.files_and_folders import recursive_find_python_class
+from yucca.functional.utils.kwargs import filter_kwargs
+from yucca.metrics.training_metrics import Accuracy, AUROC, F1
+from yucca.functional.visualization import get_train_fig_with_inp_out_tar
 
 
 class YuccaLightningModule(L.LightningModule):
     """
     The YuccaLightningModule class is an implementation of the PyTorch Lightning module designed for the Yucca project.
     It extends the LightningModule class and encapsulates the neural network model, loss functions, and optimization logic.
     This class is responsible for handling training, validation, and inference steps within the Yucca machine learning pipeline.
@@ -35,14 +36,15 @@
         lr_scheduler: torch.optim.lr_scheduler._LRScheduler = torch.optim.lr_scheduler.CosineAnnealingLR,
         momentum: float = 0.9,
         optimizer: torch.optim.Optimizer = torch.optim.SGD,
         sliding_window_overlap: float = 0.5,
         step_logging: bool = False,
         test_time_augmentation: bool = False,
         progress_bar: bool = False,
+        log_image_every_n_epochs: int = None,
     ):
         super().__init__()
         # Extract parameters from the configurator
         self.num_classes = config["num_classes"]
         self.num_modalities = config["num_modalities"]
         self.version_dir = config["version_dir"]
         self.plans = config["plans"]
@@ -68,29 +70,32 @@
             self.epoch_logging = None
         else:
             self.step_logging = False
             self.epoch_logging = True
 
         self.progress_bar = progress_bar
 
+        logging.info(f"Starting a {self.task_type} task \n" f"Deep Supervision Enabled: {self.deep_supervision}")
+
         if self.task_type == "classification":
             tmetrics_task = "multiclass" if self.num_classes > 2 else "binary"
             # can we get per-class?
             self.train_metrics = MetricCollection(
                 {
-                    "train_acc": Accuracy(task=tmetrics_task, num_classes=self.num_classes),
-                    "train_roc_auc": AUROC(task=tmetrics_task, num_classes=self.num_classes),
+                    "train/acc": Accuracy(task=tmetrics_task, num_classes=self.num_classes),
+                    "train/roc_auc": AUROC(task=tmetrics_task, num_classes=self.num_classes),
                 }
             )
             self.val_metrics = MetricCollection(
                 {
-                    "val_acc": Accuracy(task=tmetrics_task, num_classes=self.num_classes),
-                    "val_roc_auc": AUROC(task=tmetrics_task, num_classes=self.num_classes),
+                    "val/acc": Accuracy(task=tmetrics_task, num_classes=self.num_classes),
+                    "val/roc_auc": AUROC(task=tmetrics_task, num_classes=self.num_classes),
                 }
             )
+            _default_loss = "CE"
 
         if self.task_type == "segmentation":
             self.train_metrics = MetricCollection(
                 {
                     "train/dice": Dice(num_classes=self.num_classes, ignore_index=0 if self.num_classes > 1 else None),
                     "train/F1": F1(
                         num_classes=self.num_classes, ignore_index=0 if self.num_classes > 1 else None, average=None
@@ -110,30 +115,31 @@
             self.train_metrics = MetricCollection({"train/MAE": MeanAbsoluteError()})
             self.val_metrics = MetricCollection({"train/MAE": MeanAbsoluteError()})
             _default_loss = "MSE"
 
         if self.loss_fn is None:
             self.loss_fn = _default_loss
 
-        self.log_image_every_n_epochs = 1
+        self.log_image_every_n_epochs = log_image_every_n_epochs
+
         # Inference
         self.sliding_window_overlap = sliding_window_overlap
         self.test_time_augmentation = test_time_augmentation
 
         # If we are training we save params and then start training
         # Do not overwrite parameters during inference.
         self.save_hyperparameters()
         self.load_model()
 
     def load_model(self):
         logging.info(f"Loading Model: {self.model_dimensions} {self.model_name}")
         self.model = recursive_find_python_class(
-            folder=[join(yucca.__path__[0], "network_architectures")],
+            folder=[join(yucca.__path__[0], "networks")],
             class_name=self.model_name,
-            current_module="yucca.network_architectures",
+            current_module="yucca.networks",
         )
         if self.model_dimensions == "3D":
             conv_op = torch.nn.Conv3d
             norm_op = torch.nn.InstanceNorm3d
         else:
             conv_op = torch.nn.Conv2d
             norm_op = torch.nn.BatchNorm2d
@@ -148,22 +154,22 @@
             "norm_op": norm_op,
             # UNetR
             "patch_size": self.patch_size,
             # MedNeXt
             "checkpoint_style": "outside_block",
         }
         model_kwargs = filter_kwargs(self.model, model_kwargs)
-
         self.model = self.model(**model_kwargs)
 
     def forward(self, inputs):
         return self.model(inputs)
 
-    def teardown(self, stage: str):  # noqa: U100
-        wandb.finish()
+    def on_train_start(self):
+        if self.log_image_every_n_epochs is None:
+            self.log_image_every_n_epochs = self.get_image_logging_epochs(self.trainer.max_epochs)
 
     def training_step(self, batch, batch_idx):
         inputs, target, file_path = batch["image"], batch["label"], batch["file_path"]
         output = self(inputs)
         loss = self.loss_fn_train(output, target)
 
         if self.deep_supervision:
@@ -177,15 +183,15 @@
             {"train/loss": loss} | metrics,
             on_step=self.step_logging,
             on_epoch=self.epoch_logging,
             prog_bar=self.progress_bar,
             logger=True,
         )
 
-        if batch_idx == 0 and self.current_epoch % self.log_image_every_n_epochs == 0 and wandb.run is not None:
+        if batch_idx == 0 and wandb.run is not None and self.log_image_this_epoch is True:
             self._log_dict_of_images_to_wandb(
                 {
                     "input": inputs.detach().cpu().to(torch.float32).numpy(),
                     "target": target.detach().cpu().to(torch.float32).numpy(),
                     "output": output.detach().cpu().to(torch.float32).numpy(),
                     "file_path": file_path,
                 },
@@ -204,31 +210,31 @@
             {"val/loss": loss} | metrics,
             on_step=self.step_logging,
             on_epoch=self.epoch_logging,
             prog_bar=self.progress_bar,
             logger=True,
         )
 
-        if batch_idx == 0 and self.current_epoch % self.log_image_every_n_epochs == 0 and wandb.run is not None:
+        if batch_idx == 0 and wandb.run is not None and self.log_image_this_epoch is True:
             self._log_dict_of_images_to_wandb(
                 {
                     "input": inputs.detach().cpu().to(torch.float32).numpy(),
                     "target": target.detach().cpu().to(torch.float32).numpy(),
                     "output": output.detach().cpu().to(torch.float32).numpy(),
                     "file_path": file_path,
                 },
                 log_key="val",
                 task_type=self.task_type,
             )
 
     def on_predict_start(self):
         preprocessor_class = recursive_find_python_class(
-            folder=[join(yucca.__path__[0], "preprocessing")],
+            folder=[join(yucca.__path__[0], "pipeline", "preprocessing")],
             class_name=self.plans["preprocessor"],
-            current_module="yucca.preprocessing",
+            current_module="yucca.pipeline.preprocessing",
         )
         self.preprocessor = preprocessor_class(join(self.version_dir, "hparams.yaml"))
 
     def predict_step(self, batch, _batch_idx, _dataloader_idx=0):
         case, case_id = batch
         (
             case_preprocessed,
@@ -238,15 +244,14 @@
             data=case_preprocessed,
             mode=self.model_dimensions,
             mirror=self.test_time_augmentation,
             overlap=self.sliding_window_overlap,
             patch_size=self.patch_size,
             sliding_window_prediction=self.sliding_window_prediction,
         )
-
         logits, case_properties = self.preprocessor.reverse_preprocessing(logits, case_properties)
         return {"logits": logits, "properties": case_properties, "case_id": case_id[0]}
 
     def compute_metrics(self, metrics, output, target, ignore_index: int = 0):
         metrics = metrics(output, target)
         tmp = {}
         to_drop = []
@@ -262,17 +267,17 @@
         return metrics
 
     def configure_optimizers(self):
         # Initialize and configure the loss(es) here.
         # loss_kwargs holds args for any scheduler class,
         # but using filtering we only pass arguments relevant to the selected class.
         self.loss_fn = recursive_find_python_class(
-            folder=[join(yucca.__path__[0], "training/loss_and_optim")],
+            folder=[join(yucca.__path__[0], "optimization", "loss_functions")],
             class_name=self.loss_fn,
-            current_module="yucca.training.loss_and_optim",
+            current_module="yucca.optimization.loss_functions",
         )
         loss_kwargs = {
             # DCE
             "soft_dice_kwargs": {"apply_softmax": True},
         }
 
         loss_kwargs = filter_kwargs(self.loss_fn, loss_kwargs)
@@ -354,61 +359,33 @@
             f"Wrong shape: {rejected_keys_shape}.\n"
             f"Post check not succesful: {rejected_keys_data}."
         )
 
         return successful
 
     def _log_dict_of_images_to_wandb(self, imagedict: {}, log_key: str, task_type: str = "segmentation"):
-        # This needs to handle the following cases:
-        # Segmentation      : {"input": (b,m,x,y(,z)), "target": (b,1,x,y(,z)), "output": (b,c,x,y(,z)), "file_path": [pathA, pathB, ...]}
-        # Self-supervised   : {"input": (b,m,x,y(,z)), "target": (b,m,x,y(,z)), "output": (b,m,x,y(,z)), "file_path": [pathA, pathB, ...]}
-        # Classification    : {"input": (b,m,x,y(,z)), "target": (b,1,x), "output": (b,c,x), "file_path": [pathA, pathB, ...]}
-
         batch_idx = np.random.randint(0, imagedict["input"].shape[0])
-        channel_idx = np.random.randint(0, imagedict["input"].shape[1])
-
-        if len(imagedict["input"].shape) == 5:  # 3D images.
-            # We need to select a slice to visualize.
-            if task_type == "segmentation" and len(imagedict["target"][batch_idx, 0].nonzero()[0]) > 0:
-                # Select a foreground slice if any exist.
-                foreground_locations = imagedict["target"][batch_idx, 0].nonzero()
-                slice_to_visualize = foreground_locations[0][np.random.randint(0, len(foreground_locations[0]))]
-            else:
-                slice_to_visualize = np.random.randint(0, imagedict["input"].shape[2])
-
-            imagedict["input"] = imagedict["input"][:, :, slice_to_visualize]
-            if len(imagedict["target"].shape) == 5:
-                imagedict["target"] = imagedict["target"][:, :, slice_to_visualize]
-            if len(imagedict["output"].shape) == 5:
-                imagedict["output"] = imagedict["output"][:, :, slice_to_visualize]
-
-        image = imagedict["input"][batch_idx, channel_idx]
         case = os.path.splitext(os.path.split(imagedict["file_path"][batch_idx])[-1])[0]
 
-        if task_type in ["segmentation", "classification"]:
-            target = imagedict["target"][batch_idx, 0]
-            output = imagedict["output"][batch_idx].argmax(0)
-        elif task_type == "self-supervised":
-            target = imagedict["target"][batch_idx, channel_idx]
-            output = imagedict["output"][batch_idx, channel_idx]
-        else:
-            logging.warn(
-                f"Unknown task type. Found {task_type} and expected one in ['classification', 'segmentation', 'self-supervised']"
-            )
-
-        if len(target.shape) == 1:
-            fig, axes = plt.subplots(nrows=1, ncols=1, figsize=(5, 5), dpi=100, constrained_layout=True)
-            axes[0].imshow(image, cmap="gray", vmin=np.quantile(image, 0.01), vmax=np.quantile(image, 0.99))
-            axes[0].set_title("input")
-            fig.suptitle(f"{case}. Target: {target} | Output: {output}", fontsize=16)
-        else:
-            fig, axes = plt.subplots(nrows=1, ncols=3, figsize=(15, 5), dpi=100, constrained_layout=True)
-            axes[0].imshow(image, cmap="gray", vmin=np.quantile(image, 0.01), vmax=np.quantile(image, 0.99))
-            axes[0].set_title("input")
-            axes[1].imshow(target, cmap="gray")
-            axes[1].set_title("target")
-            axes[2].imshow(output, cmap="gray")
-            axes[2].set_title("output")
-            fig.suptitle(case, fontsize=16)
+        fig = get_train_fig_with_inp_out_tar(
+            input=imagedict["input"][batch_idx],
+            output=imagedict["output"][batch_idx],
+            target=imagedict["target"][batch_idx],
+            fig_title=case,
+            task_type=task_type,
+        )
+        wandb.log({log_key: wandb.Image(fig)}, commit=False)
+        plt.close(fig)
 
-            wandb.log({log_key: wandb.Image(fig)}, commit=False)
-            plt.close(fig)
+    @property
+    def log_image_this_epoch(self):
+        if isinstance(self.log_image_every_n_epochs, int):
+            return self.current_epoch % self.log_image_every_n_epochs == 0
+        if isinstance(self.log_image_every_n_epochs, list):
+            return self.current_epoch in self.log_image_every_n_epochs
+
+    @staticmethod
+    def get_image_logging_epochs(final_epoch: int = 1000):
+        first_half = np.logspace(0, 5, 10, base=4, endpoint=False)
+        second_half = final_epoch - np.logspace(0, 5, 10, base=4, endpoint=False)[::-1]
+        indices = sorted(np.concatenate((first_half, second_half)).astype(int))
+        return indices
```

### Comparing `yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/NLL.py` & `yucca-1.1.2/yucca/optimization/loss_functions/NLL.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/deep_supervision.py` & `yucca-1.1.2/yucca/optimization/loss_functions/deep_supervision.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,11 +14,13 @@
         self.loss = loss
         self.weights = weights
 
     def forward(self, list_of_logits, list_of_segs):
         if self.weights is None:
             weights = np.array([1 / (2**i) for i in range(len(list_of_logits))])
             self.weights = weights / np.sum(weights)
+
         loss = self.loss(list_of_logits[0], list_of_segs[0]) * self.weights[0]
+
         for i in range(1, len(list_of_logits)):
             loss += self.loss(list_of_logits[i], list_of_segs[i]) * self.weights[i]
         return loss
```

### Comparing `yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/hierarchical_losses.py` & `yucca-1.1.2/yucca/optimization/hierarchical_losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 import torch.nn.functional as F
 from torch import nn, Tensor
-from yucca.training.loss_and_optim.utils.LossTree import LossTree
-from yucca.training.loss_and_optim.loss_functions.nnUNet_losses import DiceCE
-from yucca.training.loss_and_optim.loss_functions.NLL import NLL
+from yucca.optimization.utils.LossTree import LossTree
+from yucca.optimization.loss_functions.nnUNet_losses import DiceCE
+from yucca.optimization.loss_functions.NLL import NLL
 
 
 class HierarchicalLoss(nn.Module):
     def __init__(self, hierarchical_kwargs={}):
         super(HierarchicalLoss, self).__init__()
         self.root = LossTree(hierarchical_kwargs["rootdict"])  # root represents your hierarchy
         self.loss = NLL(log=True)
```

### Comparing `yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/nnUNet_losses.py` & `yucca-1.1.2/yucca/optimization/loss_functions/nnUNet_losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Implementation by:
     https://github.com/Sllambias/UNetDA/blob/main/nnUNet/nnunet/training/loss_functions/dice_loss.py
 """
 
 import torch
 import numpy as np
 from torch import nn
-from yucca.training.loss_and_optim.loss_functions.CE import CE
+from yucca.optimization.loss_functions.CE import CE
 import torch.nn.functional as F
 
 
 def sum_tensor(inp, axes, keepdim=False):
     axes = np.unique(axes).astype(int)
     if keepdim:
         for ax in axes:
@@ -41,15 +41,14 @@
     """
 
     if axes is None:
         axes = tuple(range(2, len(net_output.size())))
 
     shp_x = net_output.shape
     shp_y = gt.shape
-
     with torch.no_grad():
         if len(shp_x) != len(shp_y):
             gt = gt.view((shp_y[0], 1, *shp_y[1:]))
 
         if all([i == j for i, j in zip(net_output.shape, gt.shape)]):
             # if this is the case then gt is probably already a one hot encoding
             y_onehot = gt
```

### Comparing `yucca-1.0.2/yucca/training/loss_and_optim/loss_functions/unified_focal_loss.py` & `yucca-1.1.2/yucca/optimization/loss_functions/unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/training/loss_and_optim/utils/LossTree.py` & `yucca-1.1.2/yucca/optimization/utils/LossTree.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/training/managers/alternative_managers/YuccaManager_PatchSizeMax.py` & `yucca-1.1.2/yucca/pipeline/managers/alternative_managers/YuccaManager_PatchSizeMax.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from yucca.training.managers.YuccaManager import YuccaManager
+from yucca.pipeline.managers.YuccaManager import YuccaManager
 
 
 class YuccaManager_PatchSizeMax(YuccaManager):
     """
     Instantiate a YuccaLightningManager object with the patch size set to the maximum patch size
     (no sliding window prediction).
     """
```

### Comparing `yucca-1.0.2/yucca/training/managers/augmentation/YuccaManager_SpatialOnly.py` & `yucca-1.1.2/yucca/pipeline/managers/augmentation/YuccaManager_SpatialOnly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from yucca.training.managers.YuccaManager import YuccaManager
+from yucca.pipeline.managers.YuccaManager import YuccaManager
 
 
 class YuccaManager_SpatialOnly(YuccaManager):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.augmentation_params = {
             "additive_noise_p_per_sample": 0.0,
```

### Comparing `yucca-1.0.2/yucca/training/managers/epochs/YuccaManager_1epoch.py` & `yucca-1.1.2/yucca/pipeline/managers/epochs/YuccaManager_1epoch.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from yucca.training.managers.YuccaManager import YuccaManager
+from yucca.pipeline.managers.YuccaManager import YuccaManager
 
 
 class YuccaManager_1epoch(YuccaManager):
     def __init__(
         self,
         model,
         model_dimensions: str,
```

### Comparing `yucca-1.0.2/yucca/training/managers/losses/YuccaManager_CE.py` & `yucca-1.1.2/yucca/pipeline/managers/losses/YuccaManager_CE.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from yucca.training.managers.YuccaManager import YuccaManager
-from yucca.training.loss_and_optim.loss_functions.CE import CE
+from yucca.pipeline.managers.YuccaManager import YuccaManager
+from yucca.optimization.loss_functions.CE import CE
 
 
 class YuccaManager_CE(YuccaManager):
     def __init__(
         self,
         model,
         model_dimensions: str,
```

### Comparing `yucca-1.0.2/yucca/training/managers/losses/YuccaManager_DS.py` & `yucca-1.1.2/yucca/pipeline/managers/losses/YuccaManager_DS.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from yucca.training.managers.YuccaManager import YuccaManager
-from yucca.training.loss_and_optim.loss_functions.deep_supervision import DeepSupervisionLoss
+from yucca.pipeline.managers.YuccaManager import YuccaManager
+from yucca.optimization.loss_functions.deep_supervision import DeepSupervisionLoss
 
 
 class YuccaManager_DS(YuccaManager):
     """
     The difference from YuccaTrainerV2 --> YuccaTrainerV3 is:
     - Introduces Deep Supervision
     - Uses data augmentation scheme V2
```

### Comparing `yucca-1.0.2/yucca/utils/files_and_folders.py` & `yucca-1.1.2/yucca/functional/utils/files_and_folders.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,27 +2,65 @@
 import importlib
 import fileinput
 import re
 import shutil
 import os
 from batchgenerators.utilities.file_and_folder_operations import (
     join,
-    subfiles,
     subdirs,
 )
+from typing import Union, List
 
 
 def replace_in_file(file_path, pattern_replacement):
     with fileinput.input(file_path, inplace=True) as file:
         for line in file:
             for pattern, replacement in pattern_replacement.items():
                 line = line.replace(pattern, replacement)
             print(line, end="")
 
 
+def subfiles(
+    folder: str,
+    join: bool = True,
+    remove_extension: bool = False,
+    prefix: Union[List[str], str] = None,
+    suffix: Union[List[str], str] = None,
+    sort: bool = True,
+) -> List[str]:
+    # Copy of batchgenerators subfiles with the added "remove_extension" arg
+
+    if join:
+        l = os.path.join
+    else:
+        l = lambda x, y: y  # noqa: U100
+
+    if remove_extension:
+        r = lambda x: x.split(".")[0]  # regular os.splitext doesn't account for double extensions like .nii.gz or .tar.gz
+    else:
+        r = lambda x: x
+
+    if prefix is not None and isinstance(prefix, str):
+        prefix = [prefix]
+    if suffix is not None and isinstance(suffix, str):
+        suffix = [suffix]
+
+    res = [
+        r(l(folder, i))
+        for i in os.listdir(folder)
+        if os.path.isfile(os.path.join(folder, i))
+        and (prefix is None or any([i.startswith(j) for j in prefix]))
+        and (suffix is None or any([i.endswith(j) for j in suffix]))
+    ]
+
+    if sort:
+        res.sort()
+    return res
+
+
 def rename_file_or_dir(file: str, patterns: dict):
     # Patterns is a dict of key, value pairs where keys are the words to replace and values are
     # what to substitute them by. E.g. if patterns = {"foo": "bar"}
     # then the sentence "foo bar" --> "bar bar"
     newfile = file
     for k, v in patterns.items():
         newfile = re.sub(k, v, newfile)
```

### Comparing `yucca-1.0.2/yucca/utils/loading.py` & `yucca-1.1.2/yucca/functional/utils/loading.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/utils/nib_utils.py` & `yucca-1.1.2/yucca/functional/utils/nib_utils.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/utils/saving.py` & `yucca-1.1.2/yucca/functional/utils/saving.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import nibabel as nib
 import numpy as np
-from lightning.pytorch.callbacks import BasePredictionWriter
-from yucca.utils.softmax import softmax
-from yucca.utils.nib_utils import reorient_nib_image
+from yucca.functional.utils.softmax import softmax
+from yucca.functional.utils.nib_utils import reorient_nib_image
 from PIL import Image
 from batchgenerators.utilities.file_and_folder_operations import (
     join,
     subfiles,
     maybe_mkdir_p,
 )
 
@@ -77,30 +76,7 @@
         save_nifti_from_numpy(
             files_for_case,
             join(outpath, case[:-4]),
             properties=properties_for_case.item(),
         )
 
     del files_for_case, properties_for_case
-
-
-class WritePredictionFromLogits(BasePredictionWriter):
-    def __init__(self, output_dir, save_softmax, write_interval):
-        super().__init__(write_interval)
-        self.output_dir = output_dir
-        self.save_softmax = save_softmax
-
-    def write_on_batch_end(self, _trainer, _pl_module, data_dict, _batch_indices, _batch, _batch_idx, _dataloader_idx):
-        # this will create N (num processes) files in `output_dir` each containing
-        # the predictions of it's respective rank
-        logits, properties, case_id = (
-            data_dict["logits"],
-            data_dict["properties"],
-            data_dict["case_id"],
-        )
-        save_prediction_from_logits(
-            logits,
-            join(self.output_dir, case_id),
-            properties=properties,
-            save_softmax=self.save_softmax,
-        )
-        del data_dict
```

### Comparing `yucca-1.0.2/yucca/utils/torch_utils.py` & `yucca-1.1.2/yucca/functional/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca/utils/type_conversions.py` & `yucca-1.1.2/yucca/functional/utils/type_conversions.py`

 * *Files identical despite different names*

### Comparing `yucca-1.0.2/yucca.egg-info/PKG-INFO` & `yucca-1.1.2/yucca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: yucca
-Version: 1.0.2
+Version: 1.1.2
 Summary: The modern framework for sandbox experimentation and out-of-the box machine learning on medical data.
-Author-email: Sebastian Llambias <llambias@live.dk>, Asbjørn Munk <9844416+asbjrnmunk@users.noreply.github.com>, Jakob Ambsdorf <20045425+jakobamb@users.noreply.github.com>
+Author-email: Sebastian Llambias <llambias@live.com>, Asbjørn Munk <9844416+asbjrnmunk@users.noreply.github.com>, Jakob Ambsdorf <20045425+jakobamb@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/sllambias/yucca
 Project-URL: Bug Tracker, https://github.com/sllambias/yucca/issues
 Keywords: deep learning,image segmentation,medical image analysis,medical image segmentation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

