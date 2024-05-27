# Comparing `tmp/pybaseutils-1.0.9.tar.gz` & `tmp/pybaseutils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybaseutils-1.0.9.tar", last modified: Tue Apr 30 10:23:57 2024, max compression
+gzip compressed data, was "pybaseutils-1.1.1.tar", last modified: Mon May 27 12:01:48 2024, max compression
```

## Comparing `pybaseutils-1.0.9.tar` & `pybaseutils-1.1.1.tar`

### file list

```diff
@@ -1,251 +1,255 @@
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.580976 pybaseutils-1.0.9/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-1.0.9/LICENCE
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3964 2024-04-30 10:23:57.580721 pybaseutils-1.0.9/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-22 02:45:56.000000 pybaseutils-1.0.9/README.md
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.450854 pybaseutils-1.0.9/pybaseutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2024-04-30 10:23:50.000000 pybaseutils-1.0.9/pybaseutils/__init__.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.456191 pybaseutils-1.0.9/pybaseutils/audio/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-1.0.9/pybaseutils/audio/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13844 2023-08-21 03:28:21.000000 pybaseutils-1.0.9/pybaseutils/audio/audio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1857 2023-07-26 01:11:04.000000 pybaseutils-1.0.9/pybaseutils/audio/pyaudio_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11049 2023-08-09 08:16:14.000000 pybaseutils-1.0.9/pybaseutils/audio/vad_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/pybaseutils/base64_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2333 2023-08-21 01:44:07.000000 pybaseutils-1.0.9/pybaseutils/batch_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.458385 pybaseutils-1.0.9/pybaseutils/build_utils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-20 06:36:23.000000 pybaseutils-1.0.9/pybaseutils/build_utils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6003 2023-09-20 10:26:35.000000 pybaseutils-1.0.9/pybaseutils/build_utils/cython_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2981 2023-12-06 02:32:14.000000 pybaseutils-1.0.9/pybaseutils/build_utils/pyarmor_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.461202 pybaseutils-1.0.9/pybaseutils/cluster/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/pybaseutils/cluster/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/pybaseutils/cluster/kmean.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/pybaseutils/cluster/maxmin_distance.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/pybaseutils/cluster/similarity.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7049 2022-11-16 02:12:19.000000 pybaseutils-1.0.9/pybaseutils/color_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-1.0.9/pybaseutils/config_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.472087 pybaseutils-1.0.9/pybaseutils/converter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/pybaseutils/converter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14586 2023-10-16 10:00:40.000000 pybaseutils-1.0.9/pybaseutils/converter/build_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1695 2023-07-11 07:13:11.000000 pybaseutils-1.0.9/pybaseutils/converter/build_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14159 2023-12-18 07:43:36.000000 pybaseutils-1.0.9/pybaseutils/converter/build_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5161 2023-08-18 02:32:51.000000 pybaseutils-1.0.9/pybaseutils/converter/concat_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2576 2024-03-18 08:50:01.000000 pybaseutils-1.0.9/pybaseutils/converter/convert_coco2labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3876 2023-10-17 09:34:43.000000 pybaseutils-1.0.9/pybaseutils/converter/convert_coco2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8994 2023-11-06 09:53:41.000000 pybaseutils-1.0.9/pybaseutils/converter/convert_labelme2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6015 2024-03-12 11:20:45.000000 pybaseutils-1.0.9/pybaseutils/converter/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3366 2023-09-14 06:08:22.000000 pybaseutils-1.0.9/pybaseutils/converter/convert_labelme2yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3823 2023-08-18 02:48:56.000000 pybaseutils-1.0.9/pybaseutils/converter/convert_voc2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2024-03-18 07:31:15.000000 pybaseutils-1.0.9/pybaseutils/converter/convert_voc2labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4163 2023-09-08 10:36:36.000000 pybaseutils-1.0.9/pybaseutils/converter/convert_voc2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9455 2023-08-18 02:51:52.000000 pybaseutils-1.0.9/pybaseutils/converter/convert_voc2yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3468 2023-08-11 05:43:39.000000 pybaseutils-1.0.9/pybaseutils/converter/convert_yolo2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12625 2024-02-04 09:03:56.000000 pybaseutils-1.0.9/pybaseutils/coords_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.475898 pybaseutils-1.0.9/pybaseutils/cvutils/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-1.0.9/pybaseutils/cvutils/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10684 2024-04-30 07:58:54.000000 pybaseutils-1.0.9/pybaseutils/cvutils/corner_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-1.0.9/pybaseutils/cvutils/monitor.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/pybaseutils/cvutils/mouse_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12675 2024-02-01 07:25:13.000000 pybaseutils-1.0.9/pybaseutils/cvutils/video_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.482935 pybaseutils-1.0.9/pybaseutils/dataloader/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/pybaseutils/dataloader/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    18727 2023-09-26 07:21:19.000000 pybaseutils-1.0.9/pybaseutils/dataloader/base_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9083 2024-04-30 09:00:41.000000 pybaseutils-1.0.9/pybaseutils/dataloader/base_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6286 2024-03-18 07:53:24.000000 pybaseutils-1.0.9/pybaseutils/dataloader/parser_coco_det.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7946 2024-03-18 07:53:24.000000 pybaseutils-1.0.9/pybaseutils/dataloader/parser_coco_ins.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2024-03-18 07:53:24.000000 pybaseutils-1.0.9/pybaseutils/dataloader/parser_coco_kps.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17134 2024-04-30 09:13:17.000000 pybaseutils-1.0.9/pybaseutils/dataloader/parser_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    16395 2024-04-30 09:06:38.000000 pybaseutils-1.0.9/pybaseutils/dataloader/parser_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13264 2024-03-18 07:53:24.000000 pybaseutils-1.0.9/pybaseutils/dataloader/parser_yolo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4360 2023-08-11 05:47:15.000000 pybaseutils-1.0.9/pybaseutils/dataloader/voc_seg_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    39284 2024-03-15 09:42:00.000000 pybaseutils-1.0.9/pybaseutils/file_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.488477 pybaseutils-1.0.9/pybaseutils/filter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.9/pybaseutils/filter/QueueTable.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.9/pybaseutils/filter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.9/pybaseutils/filter/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.9/pybaseutils/filter/kalman_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1785 2023-11-22 02:11:08.000000 pybaseutils-1.0.9/pybaseutils/filter/mean_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1559 2023-11-22 02:10:23.000000 pybaseutils-1.0.9/pybaseutils/filter/motion_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      787 2023-11-22 02:11:08.000000 pybaseutils-1.0.9/pybaseutils/filter/pose_filter.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.489231 pybaseutils-1.0.9/pybaseutils/font_style/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/pybaseutils/font_style/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/pybaseutils/font_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13933 2023-10-08 08:52:58.000000 pybaseutils-1.0.9/pybaseutils/geometry_tools.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5305 2023-11-20 07:29:44.000000 pybaseutils-1.0.9/pybaseutils/heatmap_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)   103016 2024-04-30 10:23:30.000000 pybaseutils-1.0.9/pybaseutils/image_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4756 2024-04-30 08:52:04.000000 pybaseutils-1.0.9/pybaseutils/json_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/pybaseutils/log.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-1.0.9/pybaseutils/logger.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.493459 pybaseutils-1.0.9/pybaseutils/metrics/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/pybaseutils/metrics/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/pybaseutils/metrics/accuracy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/pybaseutils/metrics/average_meter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/pybaseutils/metrics/class_report.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/pybaseutils/metrics/plot_pr.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/pybaseutils/metrics/plot_roc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19252 2023-10-08 08:31:16.000000 pybaseutils-1.0.9/pybaseutils/numpy_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2092 2023-08-17 02:19:40.000000 pybaseutils-1.0.9/pybaseutils/pandas_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-1.0.9/pybaseutils/plot_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.496041 pybaseutils-1.0.9/pybaseutils/pose/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:27:54.000000 pybaseutils-1.0.9/pybaseutils/pose/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3080 2023-11-30 07:45:37.000000 pybaseutils-1.0.9/pybaseutils/pose/bones_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12406 2023-11-13 06:49:34.000000 pybaseutils-1.0.9/pybaseutils/pose/human_pose.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1976 2023-09-08 03:10:04.000000 pybaseutils-1.0.9/pybaseutils/pose/pose_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.497837 pybaseutils-1.0.9/pybaseutils/pycpp/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-1.0.9/pybaseutils/pycpp/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-1.0.9/pybaseutils/pycpp/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/pybaseutils/pycpp/main.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.499078 pybaseutils-1.0.9/pybaseutils/server/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-07-18 02:35:00.000000 pybaseutils-1.0.9/pybaseutils/server/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2004 2023-07-18 03:25:38.000000 pybaseutils-1.0.9/pybaseutils/server/apm_server.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-1.0.9/pybaseutils/setup_config.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1361 2023-12-26 05:59:47.000000 pybaseutils-1.0.9/pybaseutils/singleton_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7501 2023-12-26 07:29:39.000000 pybaseutils-1.0.9/pybaseutils/thread_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/pybaseutils/time_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/pybaseutils/tracemalloc_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-1.0.9/pybaseutils/tracemalloc_utils2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.503938 pybaseutils-1.0.9/pybaseutils/tracking/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.0.9/pybaseutils/tracking/QueueTable.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.0.9/pybaseutils/tracking/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.0.9/pybaseutils/tracking/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.0.9/pybaseutils/tracking/kalman_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1787 2023-11-28 10:29:05.000000 pybaseutils-1.0.9/pybaseutils/tracking/mean_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1561 2023-11-28 10:29:05.000000 pybaseutils-1.0.9/pybaseutils/tracking/motion_filter.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      869 2023-11-28 10:29:05.000000 pybaseutils-1.0.9/pybaseutils/tracking/pose_filter.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.506655 pybaseutils-1.0.9/pybaseutils/transforms/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/pybaseutils/transforms/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    22405 2023-12-14 09:09:08.000000 pybaseutils-1.0.9/pybaseutils/transforms/affine_transform.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5112 2024-04-28 11:41:39.000000 pybaseutils-1.0.9/pybaseutils/transforms/face_alignment.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7169 2024-04-30 07:42:15.000000 pybaseutils-1.0.9/pybaseutils/transforms/transform_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-1.0.9/pybaseutils/word_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-1.0.9/pybaseutils/worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-1.0.9/pybaseutils/yaml_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.453508 pybaseutils-1.0.9/pybaseutils.egg-info/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3964 2024-04-30 10:23:57.000000 pybaseutils-1.0.9/pybaseutils.egg-info/PKG-INFO
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6972 2024-04-30 10:23:57.000000 pybaseutils-1.0.9/pybaseutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2024-04-30 10:23:57.000000 pybaseutils-1.0.9/pybaseutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2022-04-01 01:42:31.000000 pybaseutils-1.0.9/pybaseutils.egg-info/not-zip-safe
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2024-04-30 10:23:57.000000 pybaseutils-1.0.9/pybaseutils.egg-info/top_level.txt
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2024-04-30 10:23:57.581107 pybaseutils-1.0.9/setup.cfg
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-1.0.9/setup.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.529446 pybaseutils-1.0.9/test_py/
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.531495 pybaseutils-1.0.9/test_py/WebCrawler/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-25 09:17:11.000000 pybaseutils-1.0.9/test_py/WebCrawler/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3615 2023-08-25 09:36:35.000000 pybaseutils-1.0.9/test_py/WebCrawler/search_image.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3183 2023-08-25 09:18:23.000000 pybaseutils-1.0.9/test_py/WebCrawler/search_image_for_baidu.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/test_py/__init__.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.536290 pybaseutils-1.0.9/test_py/aije/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-13 02:52:05.000000 pybaseutils-1.0.9/test_py/aije/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1672 2023-11-10 11:13:57.000000 pybaseutils-1.0.9/test_py/aije/convert_labelme2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1003 2024-03-12 11:20:31.000000 pybaseutils-1.0.9/test_py/aije/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      646 2024-03-15 09:39:47.000000 pybaseutils-1.0.9/test_py/aije/copy_move.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3927 2024-04-15 12:43:54.000000 pybaseutils-1.0.9/test_py/aije/demo_video_aije.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3743 2023-12-12 07:26:52.000000 pybaseutils-1.0.9/test_py/aije/demo_voc_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1948 2024-03-12 11:22:23.000000 pybaseutils-1.0.9/test_py/aije/demo_voc_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2187 2023-10-31 01:05:59.000000 pybaseutils-1.0.9/test_py/aije/video_demo.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.541376 pybaseutils-1.0.9/test_py/audio/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-01 02:27:48.000000 pybaseutils-1.0.9/test_py/audio/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      935 2023-08-04 10:15:41.000000 pybaseutils-1.0.9/test_py/audio/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9241 2023-08-03 04:19:03.000000 pybaseutils-1.0.9/test_py/audio/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1154 2023-08-03 02:53:43.000000 pybaseutils-1.0.9/test_py/audio/main_read.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1269 2023-08-07 09:21:59.000000 pybaseutils-1.0.9/test_py/audio/segment.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    31217 2023-05-10 02:07:39.000000 pybaseutils-1.0.9/test_py/audio/speechbrain_asr_indoor_prod.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4657 2023-08-09 08:17:18.000000 pybaseutils-1.0.9/test_py/audio/speechbrain_demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1296 2023-10-10 06:07:18.000000 pybaseutils-1.0.9/test_py/class_attribute.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-1.0.9/test_py/class_names.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.559364 pybaseutils-1.0.9/test_py/converter/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-1.0.9/test_py/converter/AffectNet.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3494 2023-07-19 08:44:04.000000 pybaseutils-1.0.9/test_py/converter/AsianMovie.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3697 2023-08-11 05:35:11.000000 pybaseutils-1.0.9/test_py/converter/BITVehicle2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4581 2023-08-11 05:35:11.000000 pybaseutils-1.0.9/test_py/converter/BSTLD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5581 2023-08-17 02:19:40.000000 pybaseutils-1.0.9/test_py/converter/CCPD.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7029 2023-08-17 02:19:40.000000 pybaseutils-1.0.9/test_py/converter/CCPD2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1297 2023-07-13 07:17:07.000000 pybaseutils-1.0.9/test_py/converter/FL3D_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-01 01:02:46.000000 pybaseutils-1.0.9/test_py/converter/FreiHAND2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-18 07:53:20.000000 pybaseutils-1.0.9/test_py/converter/MTFL2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2572 2023-08-11 05:35:11.000000 pybaseutils-1.0.9/test_py/converter/TT100K.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3567 2024-04-30 08:17:22.000000 pybaseutils-1.0.9/test_py/converter/WaterMeters1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3275 2024-04-30 08:02:49.000000 pybaseutils-1.0.9/test_py/converter/WaterMeters2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/test_py/converter/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5514 2023-08-17 02:19:40.000000 pybaseutils-1.0.9/test_py/converter/concat_coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      842 2023-10-25 08:51:49.000000 pybaseutils-1.0.9/test_py/converter/convert_coco2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1410 2023-09-08 11:04:11.000000 pybaseutils-1.0.9/test_py/converter/convert_gesture2hand.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10536 2023-11-06 10:11:14.000000 pybaseutils-1.0.9/test_py/converter/convert_labelme2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6727 2023-11-08 03:36:12.000000 pybaseutils-1.0.9/test_py/converter/convert_labelme2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      726 2023-07-10 09:58:46.000000 pybaseutils-1.0.9/test_py/converter/fatigue_driving.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2321 2023-08-17 02:19:40.000000 pybaseutils-1.0.9/test_py/converter/fdd_dataset.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4726 2023-09-01 07:54:12.000000 pybaseutils-1.0.9/test_py/converter/handpose2coco.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1208 2023-08-17 02:19:40.000000 pybaseutils-1.0.9/test_py/converter/insects_for_aichallenger.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-1.0.9/test_py/converter/tt100k_utils.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7596 2023-08-11 05:35:11.000000 pybaseutils-1.0.9/test_py/converter/ua_detrac2voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2798 2024-03-18 08:47:50.000000 pybaseutils-1.0.9/test_py/converter/voc_sbd2labelme.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.565042 pybaseutils-1.0.9/test_py/cython_build/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-21 00:54:56.000000 pybaseutils-1.0.9/test_py/cython_build/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      988 2023-12-06 02:17:29.000000 pybaseutils-1.0.9/test_py/cython_build/build_cython.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1464 2023-12-06 09:27:08.000000 pybaseutils-1.0.9/test_py/cython_build/build_pyarmor.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1836 2023-09-22 03:30:02.000000 pybaseutils-1.0.9/test_py/cython_build/cryptography_demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      164 2023-09-20 00:50:56.000000 pybaseutils-1.0.9/test_py/cython_build/fun_sum.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      197 2023-09-20 00:51:59.000000 pybaseutils-1.0.9/test_py/cython_build/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2167 2023-09-22 01:20:56.000000 pybaseutils-1.0.9/test_py/cython_build/model_des_enctypt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2762 2023-09-22 01:35:52.000000 pybaseutils-1.0.9/test_py/cython_build/model_enctypt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1151 2024-04-30 08:52:27.000000 pybaseutils-1.0.9/test_py/demo1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      864 2023-11-10 09:54:32.000000 pybaseutils-1.0.9/test_py/demo2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      983 2023-09-06 06:55:38.000000 pybaseutils-1.0.9/test_py/demo3.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-1.0.9/test_py/demo_async_await1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-1.0.9/test_py/demo_async_await2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4875 2024-02-04 11:57:57.000000 pybaseutils-1.0.9/test_py/demo_coco_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5184 2023-08-28 09:18:09.000000 pybaseutils-1.0.9/test_py/demo_copy_files.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2169 2023-07-17 09:29:30.000000 pybaseutils-1.0.9/test_py/demo_copy_files_for_voc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      913 2023-06-28 11:52:23.000000 pybaseutils-1.0.9/test_py/demo_ffmpy.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      719 2024-02-20 06:47:57.000000 pybaseutils-1.0.9/test_py/demo_for_pair_file.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1670 2024-03-01 02:07:11.000000 pybaseutils-1.0.9/test_py/demo_for_polygon.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-1.0.9/test_py/demo_for_trt.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4613 2023-12-18 07:46:39.000000 pybaseutils-1.0.9/test_py/demo_get_file_list.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      637 2023-11-27 08:52:43.000000 pybaseutils-1.0.9/test_py/demo_gif.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1742 2024-01-12 07:19:32.000000 pybaseutils-1.0.9/test_py/demo_gif_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1125 2024-03-07 10:19:09.000000 pybaseutils-1.0.9/test_py/demo_image_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      825 2023-08-11 06:37:13.000000 pybaseutils-1.0.9/test_py/demo_labelme.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/test_py/demo_metrics.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/test_py/demo_mouse.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      972 2023-07-04 07:11:29.000000 pybaseutils-1.0.9/test_py/demo_nii.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2089 2023-08-11 05:35:11.000000 pybaseutils-1.0.9/test_py/demo_pandas.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-1.0.9/test_py/demo_plot.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1056 2024-04-19 09:16:57.000000 pybaseutils-1.0.9/test_py/demo_rename.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-1.0.9/test_py/demo_standard_image .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1174 2023-09-15 08:45:39.000000 pybaseutils-1.0.9/test_py/demo_standard_video .py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/test_py/demo_taichi.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      801 2023-10-17 03:30:20.000000 pybaseutils-1.0.9/test_py/demo_video.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3600 2023-10-17 07:58:27.000000 pybaseutils-1.0.9/test_py/demo_voc_crop.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2914 2023-11-09 03:13:50.000000 pybaseutils-1.0.9/test_py/demo_voc_vis.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-1.0.9/test_py/demo_word_similar.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-1.0.9/test_py/demo_worker1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/test_py/demo_worker2.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.567838 pybaseutils-1.0.9/test_py/detector/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-1.0.9/test_py/detector/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1867 2023-08-11 05:35:01.000000 pybaseutils-1.0.9/test_py/detector/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6707 2023-10-17 07:58:27.000000 pybaseutils-1.0.9/test_py/detector/detect_face_person.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6126 2023-08-17 02:19:40.000000 pybaseutils-1.0.9/test_py/detector/predet_labelme.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.570393 pybaseutils-1.0.9/test_py/edit_distance/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-11-08 06:53:33.000000 pybaseutils-1.0.9/test_py/edit_distance/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1359 2023-11-23 06:50:21.000000 pybaseutils-1.0.9/test_py/edit_distance/demo.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5613 2023-11-10 02:24:56.000000 pybaseutils-1.0.9/test_py/edit_distance/text_matching.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8212 2023-11-10 02:30:01.000000 pybaseutils-1.0.9/test_py/edit_distance/text_utils.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.572486 pybaseutils-1.0.9/test_py/flask_demo/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-1.0.9/test_py/flask_demo/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-1.0.9/test_py/flask_demo/func.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-1.0.9/test_py/flask_demo/server.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.575385 pybaseutils-1.0.9/test_py/image_correction/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-1.0.9/test_py/image_correction/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-1.0.9/test_py/image_correction/demo_correction_v1.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5603 2024-02-29 06:08:41.000000 pybaseutils-1.0.9/test_py/image_correction/demo_correction_v2.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-1.0.9/test_py/image_correction/demo_correction_v3.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-1.0.9/test_py/kafka_worker.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-1.0.9/test_py/men_tracemalloc.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-1.0.9/test_py/performance.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.576624 pybaseutils-1.0.9/test_py/pose/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:28:44.000000 pybaseutils-1.0.9/test_py/pose/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1530 2023-09-11 07:32:44.000000 pybaseutils-1.0.9/test_py/pose/human_pose.py
-drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-04-30 10:23:57.580034 pybaseutils-1.0.9/test_py/registry/
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-07 01:10:07.000000 pybaseutils-1.0.9/test_py/registry/__init__.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1195 2023-09-07 05:56:01.000000 pybaseutils-1.0.9/test_py/registry/base.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3057 2023-09-07 02:42:07.000000 pybaseutils-1.0.9/test_py/registry/component.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1701 2023-09-07 04:32:01.000000 pybaseutils-1.0.9/test_py/registry/main.py
--rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1093 2023-09-07 05:50:04.000000 pybaseutils-1.0.9/test_py/registry/register.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:48.010186 pybaseutils-1.1.1/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1073 2021-12-28 07:55:19.000000 pybaseutils-1.1.1/LICENCE
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3964 2024-05-27 12:01:48.009898 pybaseutils-1.1.1/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-22 02:45:56.000000 pybaseutils-1.1.1/README.md
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.890301 pybaseutils-1.1.1/pybaseutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      137 2024-05-27 12:01:01.000000 pybaseutils-1.1.1/pybaseutils/__init__.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.895126 pybaseutils-1.1.1/pybaseutils/audio/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-11 02:35:54.000000 pybaseutils-1.1.1/pybaseutils/audio/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13844 2023-08-21 03:28:21.000000 pybaseutils-1.1.1/pybaseutils/audio/audio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1857 2023-07-26 01:11:04.000000 pybaseutils-1.1.1/pybaseutils/audio/pyaudio_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    11049 2023-08-09 08:16:14.000000 pybaseutils-1.1.1/pybaseutils/audio/vad_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5094 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/pybaseutils/base64_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2333 2023-08-21 01:44:07.000000 pybaseutils-1.1.1/pybaseutils/batch_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.896644 pybaseutils-1.1.1/pybaseutils/build_utils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-20 06:36:23.000000 pybaseutils-1.1.1/pybaseutils/build_utils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6003 2023-09-20 10:26:35.000000 pybaseutils-1.1.1/pybaseutils/build_utils/cython_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2981 2023-12-06 02:32:14.000000 pybaseutils-1.1.1/pybaseutils/build_utils/pyarmor_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.898554 pybaseutils-1.1.1/pybaseutils/cluster/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/pybaseutils/cluster/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1952 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/pybaseutils/cluster/kmean.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3038 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/pybaseutils/cluster/maxmin_distance.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2744 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/pybaseutils/cluster/similarity.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7168 2024-05-09 10:39:08.000000 pybaseutils-1.1.1/pybaseutils/color_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-06-14 03:12:10.000000 pybaseutils-1.1.1/pybaseutils/config_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.907230 pybaseutils-1.1.1/pybaseutils/converter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/pybaseutils/converter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14586 2023-10-16 10:00:40.000000 pybaseutils-1.1.1/pybaseutils/converter/build_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2991 2024-05-23 03:22:06.000000 pybaseutils-1.1.1/pybaseutils/converter/build_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    14159 2023-12-18 07:43:36.000000 pybaseutils-1.1.1/pybaseutils/converter/build_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5161 2023-08-18 02:32:51.000000 pybaseutils-1.1.1/pybaseutils/converter/concat_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2576 2024-03-18 08:50:01.000000 pybaseutils-1.1.1/pybaseutils/converter/convert_coco2labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3876 2023-10-17 09:34:43.000000 pybaseutils-1.1.1/pybaseutils/converter/convert_coco2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8994 2023-11-06 09:53:41.000000 pybaseutils-1.1.1/pybaseutils/converter/convert_labelme2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6015 2024-03-12 11:20:45.000000 pybaseutils-1.1.1/pybaseutils/converter/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3366 2023-09-14 06:08:22.000000 pybaseutils-1.1.1/pybaseutils/converter/convert_labelme2yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3823 2023-08-18 02:48:56.000000 pybaseutils-1.1.1/pybaseutils/converter/convert_voc2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2024-03-18 07:31:15.000000 pybaseutils-1.1.1/pybaseutils/converter/convert_voc2labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4163 2023-09-08 10:36:36.000000 pybaseutils-1.1.1/pybaseutils/converter/convert_voc2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9455 2023-08-18 02:51:52.000000 pybaseutils-1.1.1/pybaseutils/converter/convert_voc2yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3468 2023-08-11 05:43:39.000000 pybaseutils-1.1.1/pybaseutils/converter/convert_yolo2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12625 2024-02-04 09:03:56.000000 pybaseutils-1.1.1/pybaseutils/coords_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.910472 pybaseutils-1.1.1/pybaseutils/cvutils/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2022-11-25 02:19:14.000000 pybaseutils-1.1.1/pybaseutils/cvutils/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10713 2024-05-14 10:15:35.000000 pybaseutils-1.1.1/pybaseutils/cvutils/corner_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6233 2023-06-21 02:12:33.000000 pybaseutils-1.1.1/pybaseutils/cvutils/monitor.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8265 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/pybaseutils/cvutils/mouse_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12675 2024-02-01 07:25:13.000000 pybaseutils-1.1.1/pybaseutils/cvutils/video_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.918016 pybaseutils-1.1.1/pybaseutils/dataloader/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/pybaseutils/dataloader/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    18727 2023-09-26 07:21:19.000000 pybaseutils-1.1.1/pybaseutils/dataloader/base_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9083 2024-05-11 08:56:25.000000 pybaseutils-1.1.1/pybaseutils/dataloader/base_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6286 2024-03-18 07:53:24.000000 pybaseutils-1.1.1/pybaseutils/dataloader/parser_coco_det.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7944 2024-05-09 10:38:10.000000 pybaseutils-1.1.1/pybaseutils/dataloader/parser_coco_ins.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2024-03-18 07:53:24.000000 pybaseutils-1.1.1/pybaseutils/dataloader/parser_coco_kps.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    17282 2024-05-23 03:02:20.000000 pybaseutils-1.1.1/pybaseutils/dataloader/parser_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    16395 2024-05-10 11:43:00.000000 pybaseutils-1.1.1/pybaseutils/dataloader/parser_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13264 2024-03-18 07:53:24.000000 pybaseutils-1.1.1/pybaseutils/dataloader/parser_yolo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4360 2023-08-11 05:47:15.000000 pybaseutils-1.1.1/pybaseutils/dataloader/voc_seg_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    39465 2024-05-20 09:01:26.000000 pybaseutils-1.1.1/pybaseutils/file_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.922365 pybaseutils-1.1.1/pybaseutils/filter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.1.1/pybaseutils/filter/QueueTable.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.1.1/pybaseutils/filter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.1.1/pybaseutils/filter/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.1.1/pybaseutils/filter/kalman_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1785 2023-11-22 02:11:08.000000 pybaseutils-1.1.1/pybaseutils/filter/mean_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1559 2023-11-22 02:10:23.000000 pybaseutils-1.1.1/pybaseutils/filter/motion_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      787 2023-11-22 02:11:08.000000 pybaseutils-1.1.1/pybaseutils/filter/pose_filter.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.923113 pybaseutils-1.1.1/pybaseutils/font_style/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      537 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/pybaseutils/font_style/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7786 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/pybaseutils/font_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13933 2023-10-08 08:52:58.000000 pybaseutils-1.1.1/pybaseutils/geometry_tools.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5305 2023-11-20 07:29:44.000000 pybaseutils-1.1.1/pybaseutils/heatmap_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)   102749 2024-05-14 09:55:00.000000 pybaseutils-1.1.1/pybaseutils/image_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4756 2024-04-30 08:52:04.000000 pybaseutils-1.1.1/pybaseutils/json_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6813 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/pybaseutils/log.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1874 2022-10-10 02:04:07.000000 pybaseutils-1.1.1/pybaseutils/logger.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.927102 pybaseutils-1.1.1/pybaseutils/metrics/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/pybaseutils/metrics/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      795 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/pybaseutils/metrics/accuracy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2191 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/pybaseutils/metrics/average_meter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5895 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/pybaseutils/metrics/class_report.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5576 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/pybaseutils/metrics/plot_pr.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5375 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/pybaseutils/metrics/plot_roc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    19252 2023-10-08 08:31:16.000000 pybaseutils-1.1.1/pybaseutils/numpy_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2092 2023-08-17 02:19:40.000000 pybaseutils-1.1.1/pybaseutils/pandas_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7522 2023-05-26 03:47:33.000000 pybaseutils-1.1.1/pybaseutils/plot_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.929528 pybaseutils-1.1.1/pybaseutils/pose/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:27:54.000000 pybaseutils-1.1.1/pybaseutils/pose/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3080 2023-11-30 07:45:37.000000 pybaseutils-1.1.1/pybaseutils/pose/bones_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    12406 2023-11-13 06:49:34.000000 pybaseutils-1.1.1/pybaseutils/pose/human_pose.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1976 2023-09-08 03:10:04.000000 pybaseutils-1.1.1/pybaseutils/pose/pose_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.931504 pybaseutils-1.1.1/pybaseutils/pycpp/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2022-10-25 08:09:00.000000 pybaseutils-1.1.1/pybaseutils/pycpp/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1337 2022-10-26 09:40:02.000000 pybaseutils-1.1.1/pybaseutils/pycpp/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4309 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/pybaseutils/pycpp/main.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.932696 pybaseutils-1.1.1/pybaseutils/server/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-07-18 02:35:00.000000 pybaseutils-1.1.1/pybaseutils/server/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2004 2023-07-18 03:25:38.000000 pybaseutils-1.1.1/pybaseutils/server/apm_server.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5027 2022-10-20 02:03:17.000000 pybaseutils-1.1.1/pybaseutils/setup_config.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1361 2023-12-26 05:59:47.000000 pybaseutils-1.1.1/pybaseutils/singleton_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9467 2024-05-27 12:00:18.000000 pybaseutils-1.1.1/pybaseutils/thread_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3306 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/pybaseutils/time_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4985 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/pybaseutils/tracemalloc_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4239 2023-02-24 10:15:12.000000 pybaseutils-1.1.1/pybaseutils/tracemalloc_utils2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.936566 pybaseutils-1.1.1/pybaseutils/tracking/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3310 2023-09-15 08:56:34.000000 pybaseutils-1.1.1/pybaseutils/tracking/QueueTable.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-15 08:56:34.000000 pybaseutils-1.1.1/pybaseutils/tracking/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2118 2023-11-22 02:10:23.000000 pybaseutils-1.1.1/pybaseutils/tracking/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2477 2023-09-15 08:56:34.000000 pybaseutils-1.1.1/pybaseutils/tracking/kalman_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1787 2023-11-28 10:29:05.000000 pybaseutils-1.1.1/pybaseutils/tracking/mean_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1561 2023-11-28 10:29:05.000000 pybaseutils-1.1.1/pybaseutils/tracking/motion_filter.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      869 2023-11-28 10:29:05.000000 pybaseutils-1.1.1/pybaseutils/tracking/pose_filter.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.938750 pybaseutils-1.1.1/pybaseutils/transforms/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/pybaseutils/transforms/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    22405 2023-12-14 09:09:08.000000 pybaseutils-1.1.1/pybaseutils/transforms/affine_transform.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5112 2024-04-28 11:41:39.000000 pybaseutils-1.1.1/pybaseutils/transforms/face_alignment.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7718 2024-05-14 10:12:52.000000 pybaseutils-1.1.1/pybaseutils/transforms/transform_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    13662 2023-05-30 01:11:50.000000 pybaseutils-1.1.1/pybaseutils/word_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4090 2023-05-25 05:47:07.000000 pybaseutils-1.1.1/pybaseutils/worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1141 2020-04-15 02:17:42.000000 pybaseutils-1.1.1/pybaseutils/yaml_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.893271 pybaseutils-1.1.1/pybaseutils.egg-info/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3964 2024-05-27 12:01:47.000000 pybaseutils-1.1.1/pybaseutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7104 2024-05-27 12:01:47.000000 pybaseutils-1.1.1/pybaseutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2024-05-27 12:01:47.000000 pybaseutils-1.1.1/pybaseutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)        1 2024-05-27 03:20:38.000000 pybaseutils-1.1.1/pybaseutils.egg-info/not-zip-safe
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       20 2024-05-27 12:01:47.000000 pybaseutils-1.1.1/pybaseutils.egg-info/top_level.txt
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)       38 2024-05-27 12:01:48.010293 pybaseutils-1.1.1/setup.cfg
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2228 2023-06-14 03:05:11.000000 pybaseutils-1.1.1/setup.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.960989 pybaseutils-1.1.1/test_py/
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.962894 pybaseutils-1.1.1/test_py/WebCrawler/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-25 09:17:11.000000 pybaseutils-1.1.1/test_py/WebCrawler/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3615 2023-08-25 09:36:35.000000 pybaseutils-1.1.1/test_py/WebCrawler/search_image.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3183 2023-08-25 09:18:23.000000 pybaseutils-1.1.1/test_py/WebCrawler/search_image_for_baidu.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/test_py/__init__.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.970191 pybaseutils-1.1.1/test_py/aije/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-13 02:52:05.000000 pybaseutils-1.1.1/test_py/aije/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1672 2023-11-10 11:13:57.000000 pybaseutils-1.1.1/test_py/aije/convert_labelme2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1003 2024-03-12 11:20:31.000000 pybaseutils-1.1.1/test_py/aije/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      646 2024-03-15 09:39:47.000000 pybaseutils-1.1.1/test_py/aije/copy_move.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4063 2024-05-21 11:44:36.000000 pybaseutils-1.1.1/test_py/aije/demo_labelme_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3927 2024-04-15 12:43:54.000000 pybaseutils-1.1.1/test_py/aije/demo_video_aije.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3743 2023-12-12 07:26:52.000000 pybaseutils-1.1.1/test_py/aije/demo_voc_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1948 2024-03-12 11:22:23.000000 pybaseutils-1.1.1/test_py/aije/demo_voc_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2187 2023-10-31 01:05:59.000000 pybaseutils-1.1.1/test_py/aije/video_demo.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.974656 pybaseutils-1.1.1/test_py/audio/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-08-01 02:27:48.000000 pybaseutils-1.1.1/test_py/audio/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      935 2023-08-04 10:15:41.000000 pybaseutils-1.1.1/test_py/audio/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     9241 2023-08-03 04:19:03.000000 pybaseutils-1.1.1/test_py/audio/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1154 2023-08-03 02:53:43.000000 pybaseutils-1.1.1/test_py/audio/main_read.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1269 2023-08-07 09:21:59.000000 pybaseutils-1.1.1/test_py/audio/segment.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    31217 2023-05-10 02:07:39.000000 pybaseutils-1.1.1/test_py/audio/speechbrain_asr_indoor_prod.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4657 2023-08-09 08:17:18.000000 pybaseutils-1.1.1/test_py/audio/speechbrain_demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1296 2023-10-10 06:07:18.000000 pybaseutils-1.1.1/test_py/class_attribute.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      790 2023-04-06 03:02:23.000000 pybaseutils-1.1.1/test_py/class_names.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.991121 pybaseutils-1.1.1/test_py/converter/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4473 2023-03-14 07:41:09.000000 pybaseutils-1.1.1/test_py/converter/AffectNet.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3494 2023-07-19 08:44:04.000000 pybaseutils-1.1.1/test_py/converter/AsianMovie.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3697 2023-08-11 05:35:11.000000 pybaseutils-1.1.1/test_py/converter/BITVehicle2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4581 2023-08-11 05:35:11.000000 pybaseutils-1.1.1/test_py/converter/BSTLD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5581 2023-08-17 02:19:40.000000 pybaseutils-1.1.1/test_py/converter/CCPD.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7029 2023-08-17 02:19:40.000000 pybaseutils-1.1.1/test_py/converter/CCPD2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1297 2023-07-13 07:17:07.000000 pybaseutils-1.1.1/test_py/converter/FL3D_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-01 01:02:46.000000 pybaseutils-1.1.1/test_py/converter/FreiHAND2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3420 2023-12-18 07:53:20.000000 pybaseutils-1.1.1/test_py/converter/MTFL2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2572 2023-08-11 05:35:11.000000 pybaseutils-1.1.1/test_py/converter/TT100K.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3583 2024-04-30 11:17:19.000000 pybaseutils-1.1.1/test_py/converter/WaterMeters1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3268 2024-05-14 09:49:38.000000 pybaseutils-1.1.1/test_py/converter/WaterMeters2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      128 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/test_py/converter/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5514 2023-08-17 02:19:40.000000 pybaseutils-1.1.1/test_py/converter/concat_coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      842 2023-10-25 08:51:49.000000 pybaseutils-1.1.1/test_py/converter/convert_coco2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1410 2023-09-08 11:04:11.000000 pybaseutils-1.1.1/test_py/converter/convert_gesture2hand.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)    10536 2023-11-06 10:11:14.000000 pybaseutils-1.1.1/test_py/converter/convert_labelme2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6727 2023-11-08 03:36:12.000000 pybaseutils-1.1.1/test_py/converter/convert_labelme2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2780 2024-05-17 08:53:22.000000 pybaseutils-1.1.1/test_py/converter/convert_voc2labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      726 2023-07-10 09:58:46.000000 pybaseutils-1.1.1/test_py/converter/fatigue_driving.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2321 2023-08-17 02:19:40.000000 pybaseutils-1.1.1/test_py/converter/fdd_dataset.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4726 2023-09-01 07:54:12.000000 pybaseutils-1.1.1/test_py/converter/handpose2coco.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1208 2023-08-17 02:19:40.000000 pybaseutils-1.1.1/test_py/converter/insects_for_aichallenger.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8806 2023-04-10 06:56:11.000000 pybaseutils-1.1.1/test_py/converter/tt100k_utils.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7596 2023-08-11 05:35:11.000000 pybaseutils-1.1.1/test_py/converter/ua_detrac2voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2798 2024-03-18 08:47:50.000000 pybaseutils-1.1.1/test_py/converter/voc_sbd2labelme.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.995739 pybaseutils-1.1.1/test_py/cython_build/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-21 00:54:56.000000 pybaseutils-1.1.1/test_py/cython_build/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      988 2023-12-06 02:17:29.000000 pybaseutils-1.1.1/test_py/cython_build/build_cython.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1464 2023-12-06 09:27:08.000000 pybaseutils-1.1.1/test_py/cython_build/build_pyarmor.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1836 2023-09-22 03:30:02.000000 pybaseutils-1.1.1/test_py/cython_build/cryptography_demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      164 2023-09-20 00:50:56.000000 pybaseutils-1.1.1/test_py/cython_build/fun_sum.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      197 2023-09-20 00:51:59.000000 pybaseutils-1.1.1/test_py/cython_build/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2167 2023-09-22 01:20:56.000000 pybaseutils-1.1.1/test_py/cython_build/model_des_enctypt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2762 2023-09-22 01:35:52.000000 pybaseutils-1.1.1/test_py/cython_build/model_enctypt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1154 2024-05-23 03:48:25.000000 pybaseutils-1.1.1/test_py/demo1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      864 2023-11-10 09:54:32.000000 pybaseutils-1.1.1/test_py/demo2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      983 2023-09-06 06:55:38.000000 pybaseutils-1.1.1/test_py/demo3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      204 2023-05-25 03:47:34.000000 pybaseutils-1.1.1/test_py/demo_async_await1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1612 2023-06-16 03:39:04.000000 pybaseutils-1.1.1/test_py/demo_async_await2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4875 2024-02-04 11:57:57.000000 pybaseutils-1.1.1/test_py/demo_coco_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5184 2023-08-28 09:18:09.000000 pybaseutils-1.1.1/test_py/demo_copy_files.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2169 2023-07-17 09:29:30.000000 pybaseutils-1.1.1/test_py/demo_copy_files_for_voc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      913 2023-06-28 11:52:23.000000 pybaseutils-1.1.1/test_py/demo_ffmpy.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      719 2024-02-20 06:47:57.000000 pybaseutils-1.1.1/test_py/demo_for_pair_file.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1670 2024-03-01 02:07:11.000000 pybaseutils-1.1.1/test_py/demo_for_polygon.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      174 2022-12-23 02:56:57.000000 pybaseutils-1.1.1/test_py/demo_for_trt.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     4613 2023-12-18 07:46:39.000000 pybaseutils-1.1.1/test_py/demo_get_file_list.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      637 2023-11-27 08:52:43.000000 pybaseutils-1.1.1/test_py/demo_gif.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1742 2024-01-12 07:19:32.000000 pybaseutils-1.1.1/test_py/demo_gif_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1125 2024-03-07 10:19:09.000000 pybaseutils-1.1.1/test_py/demo_image_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      825 2023-08-11 06:37:13.000000 pybaseutils-1.1.1/test_py/demo_labelme.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5296 2024-05-23 03:37:21.000000 pybaseutils-1.1.1/test_py/demo_labelme_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1900 2024-05-23 03:26:55.000000 pybaseutils-1.1.1/test_py/demo_lableme_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2639 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/test_py/demo_metrics.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1675 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/test_py/demo_mouse.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      972 2023-07-04 07:11:29.000000 pybaseutils-1.1.1/test_py/demo_nii.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2089 2023-08-11 05:35:11.000000 pybaseutils-1.1.1/test_py/demo_pandas.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      731 2023-01-13 09:22:52.000000 pybaseutils-1.1.1/test_py/demo_plot.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      871 2024-05-23 01:27:23.000000 pybaseutils-1.1.1/test_py/demo_rename.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1124 2023-03-28 00:52:07.000000 pybaseutils-1.1.1/test_py/demo_standard_image .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1174 2023-09-15 08:45:39.000000 pybaseutils-1.1.1/test_py/demo_standard_video .py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      749 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/test_py/demo_taichi.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      801 2023-10-17 03:30:20.000000 pybaseutils-1.1.1/test_py/demo_video.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3600 2023-10-17 07:58:27.000000 pybaseutils-1.1.1/test_py/demo_voc_crop.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2995 2024-05-17 06:14:55.000000 pybaseutils-1.1.1/test_py/demo_voc_vis.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1323 2023-04-06 02:34:20.000000 pybaseutils-1.1.1/test_py/demo_word_similar.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2906 2023-04-19 09:05:27.000000 pybaseutils-1.1.1/test_py/demo_worker1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3151 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/test_py/demo_worker2.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:47.998070 pybaseutils-1.1.1/test_py/detector/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 10:06:32.000000 pybaseutils-1.1.1/test_py/detector/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1867 2023-08-11 05:35:01.000000 pybaseutils-1.1.1/test_py/detector/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6707 2023-10-17 07:58:27.000000 pybaseutils-1.1.1/test_py/detector/detect_face_person.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     6126 2023-08-17 02:19:40.000000 pybaseutils-1.1.1/test_py/detector/predet_labelme.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:48.000643 pybaseutils-1.1.1/test_py/edit_distance/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-11-08 06:53:33.000000 pybaseutils-1.1.1/test_py/edit_distance/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1359 2023-11-23 06:50:21.000000 pybaseutils-1.1.1/test_py/edit_distance/demo.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5613 2023-11-10 02:24:56.000000 pybaseutils-1.1.1/test_py/edit_distance/text_matching.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     8212 2023-11-10 02:30:01.000000 pybaseutils-1.1.1/test_py/edit_distance/text_utils.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:48.002499 pybaseutils-1.1.1/test_py/flask_demo/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      109 2023-05-16 00:53:07.000000 pybaseutils-1.1.1/test_py/flask_demo/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      386 2023-05-16 00:55:43.000000 pybaseutils-1.1.1/test_py/flask_demo/func.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      990 2023-05-16 01:11:46.000000 pybaseutils-1.1.1/test_py/flask_demo/server.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:48.004916 pybaseutils-1.1.1/test_py/image_correction/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      130 2023-04-23 09:02:28.000000 pybaseutils-1.1.1/test_py/image_correction/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     7370 2022-11-26 02:52:34.000000 pybaseutils-1.1.1/test_py/image_correction/demo_correction_v1.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     5603 2024-02-29 06:08:41.000000 pybaseutils-1.1.1/test_py/image_correction/demo_correction_v2.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1558 2023-04-19 09:05:26.000000 pybaseutils-1.1.1/test_py/image_correction/demo_correction_v3.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      575 2023-05-24 09:15:25.000000 pybaseutils-1.1.1/test_py/kafka_worker.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      665 2023-02-27 08:49:34.000000 pybaseutils-1.1.1/test_py/men_tracemalloc.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     2222 2023-01-05 06:46:58.000000 pybaseutils-1.1.1/test_py/performance.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:48.006041 pybaseutils-1.1.1/test_py/pose/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-11 07:28:44.000000 pybaseutils-1.1.1/test_py/pose/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1530 2023-09-11 07:32:44.000000 pybaseutils-1.1.1/test_py/pose/human_pose.py
+drwxrwxrwx   0 PKing     (1000) PKing     (1000)        0 2024-05-27 12:01:48.009142 pybaseutils-1.1.1/test_py/registry/
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)      114 2023-09-07 01:10:07.000000 pybaseutils-1.1.1/test_py/registry/__init__.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1195 2023-09-07 05:56:01.000000 pybaseutils-1.1.1/test_py/registry/base.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     3057 2023-09-07 02:42:07.000000 pybaseutils-1.1.1/test_py/registry/component.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1701 2023-09-07 04:32:01.000000 pybaseutils-1.1.1/test_py/registry/main.py
+-rwxrwxrwx   0 PKing     (1000) PKing     (1000)     1093 2023-09-07 05:50:04.000000 pybaseutils-1.1.1/test_py/registry/register.py
```

### Comparing `pybaseutils-1.0.9/LICENCE` & `pybaseutils-1.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/PKG-INFO` & `pybaseutils-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 1.0.9
+Version: 1.1.1
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENCE
```

### Comparing `pybaseutils-1.0.9/README.md` & `pybaseutils-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/audio/audio_utils.py` & `pybaseutils-1.1.1/pybaseutils/audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/audio/pyaudio_utils.py` & `pybaseutils-1.1.1/pybaseutils/audio/pyaudio_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/audio/vad_utils.py` & `pybaseutils-1.1.1/pybaseutils/audio/vad_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/base64_utils.py` & `pybaseutils-1.1.1/pybaseutils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/batch_utils.py` & `pybaseutils-1.1.1/pybaseutils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/build_utils/cython_utils.py` & `pybaseutils-1.1.1/pybaseutils/build_utils/cython_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/build_utils/pyarmor_utils.py` & `pybaseutils-1.1.1/pybaseutils/build_utils/pyarmor_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/cluster/kmean.py` & `pybaseutils-1.1.1/pybaseutils/cluster/kmean.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/cluster/maxmin_distance.py` & `pybaseutils-1.1.1/pybaseutils/cluster/maxmin_distance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/cluster/similarity.py` & `pybaseutils-1.1.1/pybaseutils/cluster/similarity.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/color_utils.py` & `pybaseutils-1.1.1/pybaseutils/color_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
               'bottle', 'wine glass', 'cup', 'fork', 'knife', 'spoon', 'bowl', 'banana',
               'apple', 'sandwich', 'orange', 'broccoli', 'carrot', 'hot dog', 'pizza',
               'donut', 'cake', 'chair', 'couch', 'potted plant', 'bed', 'dining table', 'toilet',
               'tv', 'laptop', 'mouse', 'remote', 'keyboard', 'cell phone', 'microwave',
               'oven', 'toaster', 'sink', 'refrigerator', 'book', 'clock', 'vase', 'scissors',
               'teddy bear', 'hair drier', 'toothbrush']
 
+
 def get_colormap(data_type="custom"):
     if data_type == 'pascal':
         num_classes = 21
         colormap = get_pascal_colormap()
     elif data_type == 'coco':
         num_classes = 21
         colormap = get_coco_colormap()
@@ -94,34 +95,38 @@
         omask[m == ll] = colormap[ll]
     if plot:
         plt.imshow(omask)
         plt.show()
     return omask
 
 
-def decode_color_image_mask(image, mask, data_type='custom'):
+def draw_image_mask_color(image, mask, data_type='custom'):
     """
     :param image: BGR原始图像
     :param mask: 对应的Mask
     :param data_type: 数据类型
     :return:
     """
+    if mask.max() >= 255: mask = np.array(mask / 255, dtype=np.uint8)
     color_mask = decode_color_mask(mask, data_type=data_type, plot=False)
     alpha = mask.copy()
     alpha[mask > 0] = 255
     if len(alpha.shape) == 2:
         # alpha = cv2.cvtColor(alpha, cv2.COLOR_GRAY2BGR)
         alpha = alpha[:, :, np.newaxis]
     alpha = np.asarray(alpha / 255.0, dtype=np.float32)
     color_image = np.asarray(image / 2 + color_mask / 2, dtype=np.uint8)
     color_image = color_image * alpha + image * (1 - alpha)
     color_image = np.asarray(np.clip(color_image, 0, 255), dtype=np.uint8)
     return color_image, color_mask
 
 
+decode_color_image_mask = draw_image_mask_color
+
+
 def encode_segmap(mask):
     """Encode segmentation label images as pascal classes
     Args:
         mask (np.ndarray): raw segmentation label image of dimension
           (M, N, 3), in which the Pascal classes are encoded as colours.
     Returns:
         (np.ndarray): class map with dimensions (M,N), where the value at
```

### Comparing `pybaseutils-1.0.9/pybaseutils/config_utils.py` & `pybaseutils-1.1.1/pybaseutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/build_coco.py` & `pybaseutils-1.1.1/pybaseutils/converter/build_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/build_voc.py` & `pybaseutils-1.1.1/pybaseutils/converter/build_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/concat_coco.py` & `pybaseutils-1.1.1/pybaseutils/converter/concat_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/convert_coco2labelme.py` & `pybaseutils-1.1.1/pybaseutils/converter/convert_coco2labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/convert_coco2voc.py` & `pybaseutils-1.1.1/pybaseutils/converter/convert_coco2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/convert_labelme2coco.py` & `pybaseutils-1.1.1/pybaseutils/converter/convert_labelme2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/convert_labelme2voc.py` & `pybaseutils-1.1.1/pybaseutils/converter/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/convert_labelme2yolo.py` & `pybaseutils-1.1.1/pybaseutils/converter/convert_labelme2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/convert_voc2coco.py` & `pybaseutils-1.1.1/pybaseutils/converter/convert_voc2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/convert_voc2labelme.py` & `pybaseutils-1.1.1/pybaseutils/converter/convert_voc2labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/convert_voc2voc.py` & `pybaseutils-1.1.1/pybaseutils/converter/convert_voc2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/convert_voc2yolo.py` & `pybaseutils-1.1.1/pybaseutils/converter/convert_voc2yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/converter/convert_yolo2voc.py` & `pybaseutils-1.1.1/pybaseutils/converter/convert_yolo2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/coords_utils.py` & `pybaseutils-1.1.1/pybaseutils/coords_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/cvutils/corner_utils.py` & `pybaseutils-1.1.1/pybaseutils/cvutils/corner_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,81 +36,73 @@
         corners = cv2.approxPolyDP(contour, epsilon, closed=True)
         corners = corners.reshape(-1, 2)
         k += 1
         if log: print(f"k={k},corners={len(corners)},epsilon={epsilon}")
     return corners
 
 
-def get_target_points(src_pts: np.ndarray, method=0):
+def get_obb_points(pts: np.ndarray, order=True):
+    """
+    获得旋转矩形框，即最小外接矩形的四个角点
+    :param pts: [shape(n,2),...,]
+    :param order: 对4个点按顺时针方向进行排序:[top-left, top-right, bottom-right, bottom-left]
+    :return:
+    """
+    # 得到最小外接矩形的（中心(x,y), (宽,高), 旋转角度）,[center, wh, angle]==>[Point2f, Size, float]
+    rotatedRect = cv2.minAreaRect(np.array(pts, dtype=np.int32))
+    pts = cv2.boxPoints(rotatedRect)  # 获取最小外接矩形的4个顶点坐标
+    if order: pts = get_order_points(pts)
+    return pts
+
+
+def get_target_points(src_pts: np.ndarray):
     """
     根据输入的四个角点，计算其矫正后的目标四个角点,src_pts四个点分布：
         0--(w01)---1
         |          |
       (h03)      (h21)
         |          |
         3--(w23)---2
-    :param src_pts:
-    :return:
+    :param src_pts:输入四个角点，必须是有序的，[top-left, top-right, bottom-right, bottom-left]
+    :return: 输出矫正后的目标四个角点；如果要获得矫正后的长宽，则使用(W,H)=dst_pts[2]
     """
     # 计算四个角点的边长
     w01 = np.sqrt(np.sum(np.square(src_pts[0] - src_pts[1]), axis=0))
     h03 = np.sqrt(np.sum(np.square(src_pts[0] - src_pts[3]), axis=0))
     h21 = np.sqrt(np.sum(np.square(src_pts[2] - src_pts[1]), axis=0))
     w23 = np.sqrt(np.sum(np.square(src_pts[2] - src_pts[3]), axis=0))
     xmin, ymin, xmax, ymax = 0, 0, (w01 + w23) / 2, (h03 + h21) / 2
     dst_pts = [[xmin, ymin], [xmax, ymin], [xmax, ymax], [xmin, ymax]]
     dst_pts = np.asarray(dst_pts)
     return dst_pts
 
 
-def get_order_points(pts_src):
+def get_order_points(src_pts):
     """
     对4个点按顺时针方向进行排序:[top-left, top-right, bottom-right, bottom-left]
     top-left    ：对应y+x之和的最小点
     bottom-right：对应y+x之和的最大点
     top-right   ：对应y-x之差的最小点
     bottom-left ：对应y-x之差的最大点
          0(top-left)----(w10)----1(top-right)
             |                       |
           (h30)                    (h21)
             |                       |
         3(bottom-left)--(w23)---2(bottom-right)
-    :param pts_src: pts_dst [top-left, top-right, bottom-right, bottom-left]
+    :param src_pts: pts_dst [top-left, top-right, bottom-right, bottom-left]
     :return:
     """
-    pts_src = np.array(pts_src)
-    pts_dst = np.zeros(shape=(4, 2), dtype=np.float32)
-    s = pts_src.sum(axis=1)
-    # Top-left point will have the smallest sum.
-    pts_dst[0] = pts_src[np.argmin(s)]
-    # Bottom-right point will have the largest sum.
-    pts_dst[2] = pts_src[np.argmax(s)]
-    diff = np.diff(pts_src, axis=1)  # y-x= pts_src[:, 1] - pts_src[:, 0]
-    # Top-right point will have the smallest difference.
-    pts_dst[1] = pts_src[np.argmin(diff)]
-    # Bottom-left will have the largest difference.
-    pts_dst[3] = pts_src[np.argmax(diff)]
-    # Return the ordered coordinates.
-    return pts_dst
-
-
-def get_order_points_v2(pts_src):
-    """
-    参考DBNet.pytorch项目的order_points_clockwise实现
-    :param pts_src:
-    :return:
-    """
-    pts_dst = np.zeros((4, 2), dtype="float32")
-    s = pts_src.sum(axis=1)
-    pts_dst[0] = pts_src[np.argmin(s)]
-    pts_dst[2] = pts_src[np.argmax(s)]
-    diff = np.diff(pts_src, axis=1)
-    pts_dst[1] = pts_src[np.argmin(diff)]
-    pts_dst[3] = pts_src[np.argmax(diff)]
-    return pts_dst
+    dst_pts = np.zeros(shape=(4, 2), dtype=np.float32)
+    s = src_pts.sum(axis=1)
+    dst_pts[0] = src_pts[np.argmin(s)]
+    dst_pts[2] = src_pts[np.argmax(s)]
+    d = np.diff(src_pts, axis=1)
+    dst_pts[1] = src_pts[np.argmin(d)]
+    dst_pts[3] = src_pts[np.argmax(d)]
+    return dst_pts
 
 
 def get_image_four_corners(image, n_corners=4, ksize=5, blur=True, max_iter=10, vis=False):
     """
     获得图像的角点
        findContours的用法：https://blog.csdn.net/xfijun/article/details/117694917
        approxPolyDP的用法：http://t.zoukankan.com/bjxqmy-p-12347265.html
```

### Comparing `pybaseutils-1.0.9/pybaseutils/cvutils/monitor.py` & `pybaseutils-1.1.1/pybaseutils/cvutils/monitor.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/cvutils/mouse_utils.py` & `pybaseutils-1.1.1/pybaseutils/cvutils/mouse_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/cvutils/video_utils.py` & `pybaseutils-1.1.1/pybaseutils/cvutils/video_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/dataloader/base_coco.py` & `pybaseutils-1.1.1/pybaseutils/dataloader/base_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/dataloader/base_dataset.py` & `pybaseutils-1.1.1/pybaseutils/dataloader/base_dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/dataloader/parser_coco_det.py` & `pybaseutils-1.1.1/pybaseutils/dataloader/parser_coco_det.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/dataloader/parser_coco_ins.py` & `pybaseutils-1.1.1/pybaseutils/dataloader/parser_coco_ins.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     :param class_name:
     :param thickness:
     :param fontScale:
     :param use_rgb:
     :return:
     """
     mask = np.asarray(mask, np.uint8)
-    color_image, color_mask = color_utils.decode_color_image_mask(image, mask)
+    color_image, color_mask = color_utils.draw_image_mask_color(image, mask)
     color_image = image_utils.draw_image_bboxes_labels(color_image, boxes, labels, class_name=class_name,
                                                        thickness=thickness, fontScale=fontScale, drawType="chinese")
     if len(points)>0:
         color_mask = image_utils.draw_image_contours(color_mask, contours=points)
         color_image = image_utils.draw_image_contours(color_image, contours=points)
     vis_image = image_utils.image_hstack([image, mask, color_image, color_mask])
     image_utils.cv_show_image("image", vis_image, use_rgb=use_rgb)
```

### Comparing `pybaseutils-1.0.9/pybaseutils/dataloader/parser_coco_kps.py` & `pybaseutils-1.1.1/pybaseutils/dataloader/parser_coco_kps.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/dataloader/parser_labelme.py` & `pybaseutils-1.1.1/pybaseutils/dataloader/parser_labelme.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         if shuffle:
             random.seed(200)
             random.shuffle(self.image_ids)
         self.num_images = len(self.image_ids)
         print("Dataset data_root     :{}".format(self.data_root))
         print("Dataset anno_dir      :{}".format(self.anno_dir))
         print("Dataset image_dir     :{}".format(self.image_dir))
-        print("Dataset class_name    :{}".format(class_name))
+        print("Dataset class_name    :{}".format(self.class_name))
         print("Dataset class_dict    :{}".format(self.class_dict))
         print("Dataset num images    :{}".format(len(self.image_ids)))
         # print("Dataset num_classes   :{}".format(self.num_classes))
         print("------" * 10)
 
     def __len__(self):
         return len(self.image_ids)
@@ -109,15 +109,17 @@
         for image_id in tqdm(image_ids):
             image_file, annotation_file, image_id = self.get_image_anno_file(image_id)
             if not os.path.exists(annotation_file):
                 continue
             if not os.path.exists(image_file):
                 continue
             annotation, width, height = self.load_annotations(annotation_file)
-            box, label, point, group = self.parser_annotation(annotation, self.class_dict, min_points=self.min_points)
+            box, label, point, group = self.parser_annotation(annotation, self.class_dict,
+                                                              min_points=self.min_points,
+                                                              unique=self.unique)
             if len(label) == 0:
                 continue
             dst_ids.append(image_id)
         print("have nums image:{},legal image:{}".format(len(image_ids), len(dst_ids)))
         return dst_ids
 
     def parser_paths(self, filename=None, data_root=None, anno_dir=None, image_dir=None):
@@ -311,15 +313,14 @@
         except:
             print("illegal annotation:{}".format(ann_file))
             annos = []
             width = -1
             height = -1
         return annos, width, height
 
-
 def LabelMeDatasets(filename=None,
                     data_root=None,
                     anno_dir=None,
                     image_dir=None,
                     class_name=None,
                     use_rgb=False,
                     shuffle=False,
```

### Comparing `pybaseutils-1.0.9/pybaseutils/dataloader/parser_voc.py` & `pybaseutils-1.1.1/pybaseutils/dataloader/parser_voc.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,21 +171,21 @@
         image = self.read_image(image_file, use_rgb=self.use_rgb)
         height, width = image.shape[:2]
         num_boxes = len(boxes)
         if self.transform and len(boxes) > 0:
             image, boxes, labels = self.transform(image, boxes, labels)
         # boxes, labels = self.target_transform(boxes, labels)  # torch.Size([29952, 4]),torch.Size([29952])
         target = self.convert_target(boxes, labels)
-        if num_boxes == 0 or len(labels) == 0:
-            index = int(random.uniform(0, len(self)))
-            return self.__getitem__(index)
         # return image, boxes, labels
         # return image, {"target": target, "image_id": image_id, "size": [width, height]}
         data = {"image": image, "target": target, "boxes": boxes, "labels": labels, "image_id": image_id,
                 "size": [width, height], "image_file": image_file}
+        if num_boxes == 0 or len(labels) == 0:
+            index = int(random.uniform(0, len(self)))
+            data = self.__getitem__(index)
         return data
 
     def get_image_anno_file(self, index):
         """
         :param index:
         :return:
         """
```

### Comparing `pybaseutils-1.0.9/pybaseutils/dataloader/parser_yolo.py` & `pybaseutils-1.1.1/pybaseutils/dataloader/parser_yolo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/dataloader/voc_seg_utils.py` & `pybaseutils-1.1.1/pybaseutils/dataloader/voc_seg_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/file_utils.py` & `pybaseutils-1.1.1/pybaseutils/file_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,29 @@
 import json
 import glob
 import random
 import subprocess
 import concurrent.futures
 import numbers
 import pickle
+import argparse
 from datetime import datetime
 from tqdm import tqdm
 
 IMG_POSTFIX = ['*.jpg', '*.jpeg', '*.png', '*.tif', "*.JPG", "*.bmp"]
 VIDEO_POSTFIX = ['*.mp4', '*.avi']
 
 
 def str2bool(v):
-    return v.lower() in ('yes', 'true', 't', 'y', '1')
+    if v.lower() in ('yes', 'true', 't', 'y', '1'):
+        return True
+    elif v.lower() in ('no', 'false', 'f', 'n', '0'):
+        return False
+    else:
+        raise argparse.ArgumentTypeError('Unsupported value encountered.')
 
 
 def get_time(format="p"):
     """
     :param format:
     :return:
     """
@@ -140,22 +146,22 @@
     :return:
     """
     with open(json_path, 'rb') as f:
         json_data = json.load(f)
     return json_data
 
 
-def write_json_path(out_json_path, json_data):
+def write_json_path(json_file, json_data):
     """
     写入 JSON 数据
-    :param out_json_path:
+    :param json_file:
     :param json_data:
     :return:
     """
-    with open(out_json_path, 'w', encoding="utf-8") as f:
+    with open(json_file, 'w', encoding="utf-8") as f:
         json.dump(json_data, f, indent=4, ensure_ascii=False)
 
 
 def write_data(filename, content_list, split=",", mode='w'):
     """保存list[list[]]的数据到txt文件
     :param filename:文件名
     :param content_list:需要保存的数据,type->list
```

### Comparing `pybaseutils-1.0.9/pybaseutils/filter/QueueTable.py` & `pybaseutils-1.1.1/pybaseutils/filter/QueueTable.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/filter/demo.py` & `pybaseutils-1.1.1/pybaseutils/filter/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/filter/kalman_filter.py` & `pybaseutils-1.1.1/pybaseutils/filter/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/filter/mean_filter.py` & `pybaseutils-1.1.1/pybaseutils/filter/mean_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/filter/motion_filter.py` & `pybaseutils-1.1.1/pybaseutils/filter/motion_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/filter/pose_filter.py` & `pybaseutils-1.1.1/pybaseutils/filter/pose_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/font_style/__init__.py` & `pybaseutils-1.1.1/pybaseutils/font_style/__init__.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/font_utils.py` & `pybaseutils-1.1.1/pybaseutils/font_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/geometry_tools.py` & `pybaseutils-1.1.1/pybaseutils/geometry_tools.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/heatmap_utils.py` & `pybaseutils-1.1.1/pybaseutils/heatmap_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/image_utils.py` & `pybaseutils-1.1.1/pybaseutils/image_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1092,18 +1092,22 @@
     :param image:
     :param bboxes:  [[x1,y1,x2,y2],[x1,y1,x2,y2]]
     :param labels:
     :return:
     """
     if isinstance(labels, np.ndarray): labels = labels.astype(np.int32).reshape(-1).tolist()
     for label, box in zip(labels, bboxes):
-        color_ = color if color else color_table[int(label) + 1]
         box = [int(b) for b in box]
-        if class_name: label = class_name[int(label)]
-        image = custom_bbox_line(image, box, color_, str(label), thickness=thickness,
+        name = label
+        color_ = color
+        if isinstance(name, numbers.Number) and class_name:
+            color_ = color_table[int(name) + 1]
+            name = class_name[int(name)]
+        if not color_: color_ = color_table[1]
+        image = custom_bbox_line(image, box, color_, str(name), thickness=thickness,
                                  fontScale=fontScale, drawType=drawType)
     return image
 
 
 def draw_image_rects_labels(image, rects, labels, class_name=None, color=None, thickness=-1, fontScale=-1.0):
     """
     :param image:
@@ -1625,14 +1629,15 @@
     if not center:
         # center = (w // 2, h // 2)
         center = (w / 2., h / 2.)
     mat = cv2.getRotationMatrix2D(center, angle, scale)
     rotated = cv2.warpAffine(image, mat, dsize=(w, h), borderMode=cv2.BORDER_CONSTANT, borderValue=borderValue)
     return rotated
 
+
 def save_image(image_file, image, uint8=False, use_rgb=False):
     """
     保存图片
     :param image_file: 保存图片文件
     :param image: BGR Image
     :param uint8: 乘以255并转换为INT8类型
     :param use_rgb: 是否将输入image(BGR)转换为RGB
@@ -2485,21 +2490,15 @@
     获得旋转矩形框，即最小外接矩形的四个角点
     :param contours: [shape(n,2),...,]
     :param order: 对4个点按顺时针方向进行排序:[top-left, top-right, bottom-right, bottom-left]
     :return:
     """
     points = []
     for i in range(len(contours)):
-        # 得到最小外接矩形的（中心(x,y), (宽,高), 旋转角度）
-        rotatedRect = cv2.minAreaRect(np.array(contours[i],dtype=np.int32))  # [center, wh, angle]==>[Point2f, Size, float]
-        pts = cv2.boxPoints(rotatedRect)  # 获取最小外接矩形的4个顶点坐标
-        pts = pts[[1, 2, 3, 0], :]
-        if order:
-            pts = corner_utils.get_order_points(pts)
-            # pts2 = corner_utils.order_points_clockwise(pts)
+        pts = corner_utils.get_obb_points(pts=contours[i], order=order)
         points.append(pts)
     return points
 
 
 def find_image_contours(mask: np.ndarray, target_label: List[int] = [1, 2]) -> List[List[np.ndarray]]:
     """
     寻找一个多值Mask图像的轮廓
```

### Comparing `pybaseutils-1.0.9/pybaseutils/json_utils.py` & `pybaseutils-1.1.1/pybaseutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/log.py` & `pybaseutils-1.1.1/pybaseutils/log.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/logger.py` & `pybaseutils-1.1.1/pybaseutils/logger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/metrics/accuracy.py` & `pybaseutils-1.1.1/pybaseutils/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/metrics/average_meter.py` & `pybaseutils-1.1.1/pybaseutils/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/metrics/class_report.py` & `pybaseutils-1.1.1/pybaseutils/metrics/class_report.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/metrics/plot_pr.py` & `pybaseutils-1.1.1/pybaseutils/metrics/plot_pr.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/metrics/plot_roc.py` & `pybaseutils-1.1.1/pybaseutils/metrics/plot_roc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/numpy_utils.py` & `pybaseutils-1.1.1/pybaseutils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/pandas_utils.py` & `pybaseutils-1.1.1/pybaseutils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/plot_utils.py` & `pybaseutils-1.1.1/pybaseutils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/pose/bones_utils.py` & `pybaseutils-1.1.1/pybaseutils/pose/bones_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/pose/human_pose.py` & `pybaseutils-1.1.1/pybaseutils/pose/human_pose.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/pose/pose_utils.py` & `pybaseutils-1.1.1/pybaseutils/pose/pose_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/pycpp/demo.py` & `pybaseutils-1.1.1/pybaseutils/pycpp/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/pycpp/main.py` & `pybaseutils-1.1.1/pybaseutils/pycpp/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/server/apm_server.py` & `pybaseutils-1.1.1/pybaseutils/server/apm_server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/setup_config.py` & `pybaseutils-1.1.1/pybaseutils/setup_config.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/singleton_utils.py` & `pybaseutils-1.1.1/pybaseutils/singleton_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/thread_utils.py` & `pybaseutils-1.1.1/pybaseutils/thread_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             参考：https://blog.csdn.net/weixin_42176112/article/details/117790945
 """
 
 import threading
 import time
 from typing import List, Tuple, Callable
 from concurrent.futures import ThreadPoolExecutor, as_completed
-from multiprocessing import Pool
+from multiprocessing import Pool, Process
 
 # 创建线程锁
 thread_lock = threading.Lock()
 
 
 def thread_safety(func, *args, **kwargs):
     """
@@ -65,14 +65,35 @@
     t = int(image_path.split(".")[0])
     time.sleep(t)
     # with thread_lock:
     print("正在处理数据：{},{}  ".format(image_path, data))
     return image_path, data
 
 
+class TaskProcess():
+    def tasks(self, tasks: List, params: List):
+        """
+        返回结果无序
+        :param tasks:
+        :param params:
+        :return:
+        """
+        p_list = []
+        for t, p in zip(tasks, params):
+            p = Process(target=t, args=(p,))
+            p.daemon = True
+            p.start()
+            p_list.append(p)
+        r_list = []
+        for p in p_list:
+            r = p.join()
+            r_list.append(r)
+        return r_list
+
+
 class ProcessPool(object):
     """
     进程池
     进程通信： https://blog.csdn.net/yldmkx/article/details/115948722
     int_data = multiprocessing.Manager().Value(ctypes.c_int, 0)
 	str_data = multiprocessing.Manager().Value(ctypes.c_char_p, 'str0')
     """
@@ -88,15 +109,21 @@
         result = []
         for r in self.pool.map(func, inputs):
             result.append(r)
         return result
 
     def task_apply_async(self, func: Callable, inputs: List, timeout=None):
         """进程任务，返回结果有序"""
-        result = [self.pool.apply_async(func, args=(i,)) for i in inputs]
+        result = [self.pool.apply_async(func, args=(*p,)) for p in inputs]
+        result = [r.get(timeout=timeout) for r in result]
+        return result
+
+    def multi_tasks(self, tasks: List, inputs: List, timeout=None):
+        """多进程多任务，返回结果有序"""
+        result = [self.pool.apply_async(t, args=(*p,)) for t, p in zip(tasks, inputs)]
         result = [r.get(timeout=timeout) for r in result]
         return result
 
     def close(self):
         self.pool.close()
 
     def __getstate__(self):
@@ -146,38 +173,50 @@
         except Exception as e:
             result = []  # 超时异常时，输出列表可能缺失部分值
             print("Error:{}".format(e))
         return result
 
     def task_submit(self, func: Callable, inputs: List, timeout=None):
         """线程任务，返回结果无序(map与submit的性能基本一致)"""
-        task_list = [self.pool.submit(func, p) for p in inputs]
+        task_list = [self.pool.submit(func, *p) for p in inputs]
         result = []
         try:
             for task in as_completed(task_list, timeout=timeout):
                 result.append(task.result(timeout=timeout))
         except Exception as e:
             result = []
             print("Error:{}".format(e))
         return result
 
     def task_submit_v1(self, func: Callable, inputs: List, timeout=None):
         """线程任务，返回结果无序"""
-        task_list = [self.pool.submit(func, p) for p in inputs]
+        task_list = [self.pool.submit(func, *p) for p in inputs]
         result = []
         while len(task_list) > 0:
             index = []
             for i, task in enumerate(task_list):
                 if task.done():
                     result.append(task.result(timeout=timeout))
                 else:
                     index.append(i)
             task_list = [task_list[i] for i in index]
         return result
 
+    def multi_tasks(self, tasks: List, inputs: List, timeout=None):
+        """多线程多任务，返回结果有序"""
+        task_list = [self.pool.submit(t, *p) for t, p in zip(tasks, inputs)]
+        result = []
+        try:
+            for task in as_completed(task_list, timeout=timeout):
+                result.append(task.result(timeout=timeout))
+        except Exception as e:
+            result = []
+            print("Error:{}".format(e))
+        return result
+
     def shutdown(self, wait=True):
         self.pool.shutdown(wait=wait)
 
 
 def thread_lock_decorator():
     def decorator(func):
         def wrapper(*args, **kwargs):
@@ -204,20 +243,39 @@
     print("result2:{}".format(result2))
 
 
 def performanceProcessPool():
     from pybaseutils import time_utils
     tp = ProcessPool(max_workers=4)
     # contents = ["1.jpg", "4.jpg", "4.jpg", "4.jpg", "2.jpg"]
-    contents = ["1.jpg", "5.jpg", "4.jpg", "3.jpg", "2.jpg"]
+    # contents = ["1.jpg", "5.jpg", "4.jpg", "3.jpg", "2.jpg"]
+    contents = ["1.jpg", "5.jpg", "1.jpg", "1.jpg", "1.jpg"]
     print(contents)
-    with time_utils.Performance("task_map") as p:
-        result1 = tp.task_map(func=consumer, inputs=contents)
-    with time_utils.Performance("task_apply_async") as p:
-        result2 = tp.task_apply_async(func=consumer, inputs=contents)
-    print(result1)
-    print(result2)
+    # with time_utils.Performance("task_map") as p:
+    #     result1 = tp.task_map(func=consumer, inputs=contents)
+    # with time_utils.Performance("task_apply_async") as p:
+    #     result2 = tp.task_apply_async(func=consumer, inputs=contents)
+    with time_utils.Performance("mul_tasks") as p:
+        mul_tasks = [consumer] * len(contents)
+        result3 = tp.multi_tasks(mul_tasks, contents)
+    # print(result1)
+    # print(result2)
+    print(result3)
+
+
+def performanceProcess():
+    from pybaseutils import time_utils
+    tp = ProcessPool(max_workers=4)
+    # contents = ["1.jpg", "4.jpg", "4.jpg", "4.jpg", "2.jpg"]
+    contents = ["1.jpg", "5.jpg", "4.jpg", "3.jpg", "2.jpg"]
+    contents = ["1.jpg", "5.jpg", "1.jpg", "1.jpg", "1.jpg"]
+    tasks = [consumer] * len(contents)
+    t = TaskProcess()
+    r = t.tasks(tasks, contents)
+    print(r)
 
 
 if __name__ == "__main__":
-    performanceThreadPool()
+    # performanceThreadPool()
     # performanceProcessPool()
+    # performanceProcess()
+    performanceProcessPool()
```

### Comparing `pybaseutils-1.0.9/pybaseutils/time_utils.py` & `pybaseutils-1.1.1/pybaseutils/time_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/tracemalloc_utils.py` & `pybaseutils-1.1.1/pybaseutils/tracemalloc_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/tracemalloc_utils2.py` & `pybaseutils-1.1.1/pybaseutils/tracemalloc_utils2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/tracking/QueueTable.py` & `pybaseutils-1.1.1/pybaseutils/tracking/QueueTable.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/tracking/demo.py` & `pybaseutils-1.1.1/pybaseutils/tracking/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/tracking/kalman_filter.py` & `pybaseutils-1.1.1/pybaseutils/tracking/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/tracking/mean_filter.py` & `pybaseutils-1.1.1/pybaseutils/tracking/mean_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/tracking/motion_filter.py` & `pybaseutils-1.1.1/pybaseutils/tracking/motion_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/tracking/pose_filter.py` & `pybaseutils-1.1.1/pybaseutils/tracking/pose_filter.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/transforms/affine_transform.py` & `pybaseutils-1.1.1/pybaseutils/transforms/affine_transform.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/transforms/face_alignment.py` & `pybaseutils-1.1.1/pybaseutils/transforms/face_alignment.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/transforms/transform_utils.py` & `pybaseutils-1.1.1/pybaseutils/transforms/transform_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,42 @@
     @Brief  :
 """
 import cv2
 import numpy as np
 from pybaseutils.cvutils import corner_utils
 
 
-def get_target_corner_points(src_pts: np.ndarray):
+def get_obb_points(points, order=True):
+    """
+    获得旋转矩形框，即最小外接矩形的四个角点
+    :param points: [shape(n,2),...,]
+    :param order: 对4个点按顺时针方向进行排序:[top-left, top-right, bottom-right, bottom-left]
+    :return:
+    """
+    return corner_utils.get_obb_points(pts=points, order=order)
+
+
+def get_target_points(src_pts: np.ndarray):
     """
     根据输入的四个角点，计算其矫正后的目标四个角点,src_pts四个点分布：
         0--(w01)---1
         |          |
       (h03)      (h21)
         |          |
         3--(w23)---2
     :param src_pts:
     :return:
     """
     return corner_utils.get_target_points(src_pts=src_pts)
 
 
+def get_order_points(src_pts):
+    return corner_utils.get_order_points(src_pts=src_pts)
+
+
 def get_image_alignment(image, src_pts, dst_pts, dsize=None, method="lstsq"):
     """
     apply affine transform实现对齐图像
     D=M*S or D=H*S
     :param image: input image
     :param src_pts: 原始点S集合(n×2)
     :param dst_pts: 目标点D集合(n×2)
@@ -63,15 +77,15 @@
     :param dsize:
     :param scale:
     :param method:
     :return:
     """
     h, w = image.shape[:2]
     if dst_pts is None:
-        dst_pts = get_target_corner_points(src_pts)
+        dst_pts = get_target_points(src_pts)
         xmin = min(dst_pts[:, 0])
         ymin = min(dst_pts[:, 1])
         xmax = max(dst_pts[:, 0])
         ymax = max(dst_pts[:, 1])
         tsize = (xmax - xmin, ymax - ymin)
     else:
         tsize = (w, h)
@@ -175,27 +189,28 @@
     Minv = np.linalg.pinv(Minv)
     Minv = Minv[0:2, :]
     return Minv
 
 
 def test_transform(image_file):
     from pybaseutils import image_utils
-    src = cv2.imread(image_file)
-    # src[:, :] = 0
-    mask = image_utils.get_image_mask(src)
-    contours = image_utils.find_mask_contours(mask, max_nums=1)
-    src_pts = image_utils.find_minAreaRect(contours, order=True)
-    dst = src.copy()
-    dst_pts = []
-    if len(src_pts) > 0:
-        src_pts = src_pts[0]
-        dst, dst_pts, M, Minv = image_alignment(dst, src_pts, dsize=(-1, -1), scale=(1.2, 1.2))
-    src = image_utils.draw_image_contours(src, [src_pts])
-    src = image_utils.draw_landmark(src, [src_pts], color=(255, 0, 0), vis_id=True)
-    dst = image_utils.draw_landmark(dst, [dst_pts], color=(0, 255, 0), vis_id=True)
-    image_utils.cv_show_image("src", src, delay=10)
-    image_utils.cv_show_image("dst", dst, delay=0)
+    image = cv2.imread(image_file)
+    for i in range(360 * 2):
+        src = image_utils.image_rotation(image.copy(), angle=i)
+        mask = image_utils.get_image_mask(src)
+        contours = image_utils.find_mask_contours(mask, max_nums=1)
+        src_pts = image_utils.find_minAreaRect(contours, order=True)
+        dst = src.copy()
+        dst_pts = []
+        if len(src_pts) > 0:
+            src_pts = src_pts[0]
+            dst, dst_pts, M, Minv = image_alignment(dst, src_pts, dsize=(-1, -1), scale=(1.2, 1.2))
+        src = image_utils.draw_image_contours(src, [src_pts])
+        src = image_utils.draw_landmark(src, [src_pts], color=(255, 0, 0), vis_id=True)
+        dst = image_utils.draw_landmark(dst, [dst_pts], color=(0, 255, 0), vis_id=True)
+        image_utils.cv_show_image("src", src, delay=10)
+        image_utils.cv_show_image("dst", dst, delay=0)
 
 
 if __name__ == '__main__':
     image_file = "../../data/mask/mask4.jpg"
     test_transform(image_file)
```

### Comparing `pybaseutils-1.0.9/pybaseutils/word_utils.py` & `pybaseutils-1.1.1/pybaseutils/word_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/worker.py` & `pybaseutils-1.1.1/pybaseutils/worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils/yaml_utils.py` & `pybaseutils-1.1.1/pybaseutils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/pybaseutils.egg-info/PKG-INFO` & `pybaseutils-1.1.1/pybaseutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybaseutils
-Version: 1.0.9
+Version: 1.1.1
 Summary: pybaseutils
 Home-page: https://github.com/PanJinquan/base-utils
 Author: PanJinquan
 Author-email: 390737991@qq.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENCE
```

### Comparing `pybaseutils-1.0.9/pybaseutils.egg-info/SOURCES.txt` & `pybaseutils-1.1.1/pybaseutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,16 @@
 test_py/demo_for_polygon.py
 test_py/demo_for_trt.py
 test_py/demo_get_file_list.py
 test_py/demo_gif.py
 test_py/demo_gif_video.py
 test_py/demo_image_crop.py
 test_py/demo_labelme.py
+test_py/demo_labelme_crop.py
+test_py/demo_lableme_vis.py
 test_py/demo_metrics.py
 test_py/demo_mouse.py
 test_py/demo_nii.py
 test_py/demo_pandas.py
 test_py/demo_plot.py
 test_py/demo_rename.py
 test_py/demo_standard_image .py
@@ -148,14 +150,15 @@
 test_py/WebCrawler/__init__.py
 test_py/WebCrawler/search_image.py
 test_py/WebCrawler/search_image_for_baidu.py
 test_py/aije/__init__.py
 test_py/aije/convert_labelme2coco.py
 test_py/aije/convert_labelme2voc.py
 test_py/aije/copy_move.py
+test_py/aije/demo_labelme_crop.py
 test_py/aije/demo_video_aije.py
 test_py/aije/demo_voc_crop.py
 test_py/aije/demo_voc_vis.py
 test_py/aije/video_demo.py
 test_py/audio/__init__.py
 test_py/audio/demo.py
 test_py/audio/main.py
@@ -177,14 +180,15 @@
 test_py/converter/WaterMeters2.py
 test_py/converter/__init__.py
 test_py/converter/concat_coco.py
 test_py/converter/convert_coco2voc.py
 test_py/converter/convert_gesture2hand.py
 test_py/converter/convert_labelme2coco.py
 test_py/converter/convert_labelme2voc.py
+test_py/converter/convert_voc2labelme.py
 test_py/converter/fatigue_driving.py
 test_py/converter/fdd_dataset.py
 test_py/converter/handpose2coco.py
 test_py/converter/insects_for_aichallenger.py
 test_py/converter/tt100k_utils.py
 test_py/converter/ua_detrac2voc.py
 test_py/converter/voc_sbd2labelme.py
```

### Comparing `pybaseutils-1.0.9/setup.py` & `pybaseutils-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/WebCrawler/search_image.py` & `pybaseutils-1.1.1/test_py/WebCrawler/search_image.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/WebCrawler/search_image_for_baidu.py` & `pybaseutils-1.1.1/test_py/WebCrawler/search_image_for_baidu.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/aije/convert_labelme2coco.py` & `pybaseutils-1.1.1/test_py/aije/convert_labelme2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/aije/convert_labelme2voc.py` & `pybaseutils-1.1.1/test_py/aije/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/aije/copy_move.py` & `pybaseutils-1.1.1/test_py/aije/copy_move.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/aije/demo_video_aije.py` & `pybaseutils-1.1.1/test_py/aije/demo_video_aije.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/aije/demo_voc_crop.py` & `pybaseutils-1.1.1/test_py/aije/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/aije/demo_voc_vis.py` & `pybaseutils-1.1.1/test_py/aije/demo_voc_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/aije/video_demo.py` & `pybaseutils-1.1.1/test_py/aije/video_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/audio/demo.py` & `pybaseutils-1.1.1/test_py/audio/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/audio/main.py` & `pybaseutils-1.1.1/test_py/audio/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/audio/main_read.py` & `pybaseutils-1.1.1/test_py/audio/main_read.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/audio/segment.py` & `pybaseutils-1.1.1/test_py/audio/segment.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/audio/speechbrain_asr_indoor_prod.py` & `pybaseutils-1.1.1/test_py/audio/speechbrain_asr_indoor_prod.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/audio/speechbrain_demo.py` & `pybaseutils-1.1.1/test_py/audio/speechbrain_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/class_attribute.py` & `pybaseutils-1.1.1/test_py/class_attribute.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/class_names.py` & `pybaseutils-1.1.1/test_py/class_names.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/AffectNet.py` & `pybaseutils-1.1.1/test_py/converter/AffectNet.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/AsianMovie.py` & `pybaseutils-1.1.1/test_py/converter/AsianMovie.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/BITVehicle2voc.py` & `pybaseutils-1.1.1/test_py/converter/BITVehicle2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/BSTLD2voc.py` & `pybaseutils-1.1.1/test_py/converter/BSTLD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/CCPD.py` & `pybaseutils-1.1.1/test_py/converter/CCPD.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/CCPD2voc.py` & `pybaseutils-1.1.1/test_py/converter/CCPD2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/FL3D_dataset.py` & `pybaseutils-1.1.1/test_py/converter/FL3D_dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/MTFL2voc.py` & `pybaseutils-1.1.1/test_py/converter/MTFL2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/TT100K.py` & `pybaseutils-1.1.1/test_py/converter/TT100K.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/WaterMeters1.py` & `pybaseutils-1.1.1/test_py/converter/WaterMeters1.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     data = eval(anno_info[2])
     image_file = os.path.join(image_dir, image_name)
     image = cv2.imread(image_file)
     h, w = image.shape[:2]
     point = [[d['x'], d['y']] for d in data['data']]
     point = np.array(point) * (w, h)
     boxes = image_utils.polygons2boxes([point])
-    # label = "{:0=10.3f}".format(label)
-    label = str(label)
+    label = "{:0=9.3f}".format(label).replace(".", "")
+    # label = str(label)
     return image, image_name, point, label, boxes
 
 
 def WaterMeters(image_dir, ann_file, out_json, crop_root=None, use_align=True, vis=True, delay=5):
     if crop_root: file_utils.create_dir(crop_root)
     if out_json: file_utils.create_dir(out_json)
     pd = pandas_utils.read_csv(anno_file)
```

### Comparing `pybaseutils-1.0.9/test_py/converter/WaterMeters2.py` & `pybaseutils-1.1.1/test_py/converter/WaterMeters2.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         lable_name = image_name.replace(f".{postfix}", ".txt")
         json_name = image_name.replace(f".{postfix}", ".json")
         image_file = os.path.join(image_dir, image_name)
         lable_file = os.path.join(label_dir, lable_name)
         image, point, label, boxes = load_annotation(image_file, lable_file)
         image_h, image_w = image.shape[:2]
         if crop_root and use_align:
-            dst_pts = transform_utils.get_target_corner_points(point)
+            dst_pts = transform_utils.get_target_points(point)
             crop, M, Minv = transform_utils.get_image_alignment(image, src_pts=point, dst_pts=dst_pts, dsize=None,
                                                                 method="lstsq")
             crop_file = os.path.join(crop_root, "{}_{:0=5d}_alignment.jpg".format(label, i))
             cv2.imwrite(crop_file, crop)
         elif crop_root:
             crop = image_utils.get_bbox_crop(image, bbox=boxes[0])
             crop_file = os.path.join(crop_root, "{}_{:0=5d}_crop.jpg".format(label, i))
```

### Comparing `pybaseutils-1.0.9/test_py/converter/concat_coco.py` & `pybaseutils-1.1.1/test_py/converter/concat_coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/convert_coco2voc.py` & `pybaseutils-1.1.1/test_py/converter/convert_coco2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/convert_gesture2hand.py` & `pybaseutils-1.1.1/test_py/converter/convert_gesture2hand.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/convert_labelme2coco.py` & `pybaseutils-1.1.1/test_py/converter/convert_labelme2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/convert_labelme2voc.py` & `pybaseutils-1.1.1/test_py/converter/convert_labelme2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/fatigue_driving.py` & `pybaseutils-1.1.1/test_py/converter/fatigue_driving.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/fdd_dataset.py` & `pybaseutils-1.1.1/test_py/converter/fdd_dataset.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/handpose2coco.py` & `pybaseutils-1.1.1/test_py/converter/handpose2coco.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/insects_for_aichallenger.py` & `pybaseutils-1.1.1/test_py/converter/insects_for_aichallenger.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/tt100k_utils.py` & `pybaseutils-1.1.1/test_py/converter/tt100k_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/ua_detrac2voc.py` & `pybaseutils-1.1.1/test_py/converter/ua_detrac2voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/converter/voc_sbd2labelme.py` & `pybaseutils-1.1.1/test_py/converter/voc_sbd2labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/cython_build/build_cython.py` & `pybaseutils-1.1.1/test_py/cython_build/build_cython.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/cython_build/build_pyarmor.py` & `pybaseutils-1.1.1/test_py/cython_build/build_pyarmor.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/cython_build/cryptography_demo.py` & `pybaseutils-1.1.1/test_py/cython_build/cryptography_demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/cython_build/model_des_enctypt.py` & `pybaseutils-1.1.1/test_py/cython_build/model_des_enctypt.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/cython_build/model_enctypt.py` & `pybaseutils-1.1.1/test_py/cython_build/model_enctypt.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo2.py` & `pybaseutils-1.1.1/test_py/demo2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo3.py` & `pybaseutils-1.1.1/test_py/demo3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_async_await2.py` & `pybaseutils-1.1.1/test_py/demo_async_await2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_coco_vis.py` & `pybaseutils-1.1.1/test_py/demo_coco_vis.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_copy_files.py` & `pybaseutils-1.1.1/test_py/demo_copy_files.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_copy_files_for_voc.py` & `pybaseutils-1.1.1/test_py/demo_copy_files_for_voc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_ffmpy.py` & `pybaseutils-1.1.1/test_py/demo_ffmpy.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_for_pair_file.py` & `pybaseutils-1.1.1/test_py/demo_for_pair_file.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_for_polygon.py` & `pybaseutils-1.1.1/test_py/demo_for_polygon.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_get_file_list.py` & `pybaseutils-1.1.1/test_py/demo_get_file_list.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_gif.py` & `pybaseutils-1.1.1/test_py/demo_gif.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_gif_video.py` & `pybaseutils-1.1.1/test_py/demo_gif_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_image_crop.py` & `pybaseutils-1.1.1/test_py/demo_image_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_labelme.py` & `pybaseutils-1.1.1/test_py/demo_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_metrics.py` & `pybaseutils-1.1.1/test_py/demo_metrics.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_mouse.py` & `pybaseutils-1.1.1/test_py/demo_mouse.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_nii.py` & `pybaseutils-1.1.1/test_py/demo_nii.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_pandas.py` & `pybaseutils-1.1.1/test_py/demo_pandas.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_plot.py` & `pybaseutils-1.1.1/test_py/demo_plot.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_rename.py` & `pybaseutils-1.1.1/test_py/demo_rename.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,11 +19,10 @@
         name = "{}_{}".format(prefix, time) if prefix else time
         name = "{}_{:0=4d}.{}".format(name, i, postfix)
         new = os.path.join(output, name)
         file_utils.copy_file(old, new)
 
 
 if __name__ == '__main__':
-
-    image_dir = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/室内考题/天河视频/20240419_天河训练视频/室内考题-天河数据1"
-    output = "/home/PKing/nasdata/dataset-dmai/AIJE/岗评项目数据/室内考题/天河视频/20240419_天河训练视频/室内考题-天河数据1-train"
-    rename_image_file(image_dir, output, prefix="天河")
+    image_dir = "/home/PKing/nasdata/release/AIJE/aije-algorithm/aije-component-cv/test/data/test"
+    output = image_dir + "-train"
+    rename_image_file(image_dir, output, prefix="test")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pybaseutils-1.0.9/test_py/demo_standard_image .py` & `pybaseutils-1.1.1/test_py/demo_standard_image .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_standard_video .py` & `pybaseutils-1.1.1/test_py/demo_standard_video .py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_taichi.py` & `pybaseutils-1.1.1/test_py/demo_taichi.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_video.py` & `pybaseutils-1.1.1/test_py/demo_video.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_voc_crop.py` & `pybaseutils-1.1.1/test_py/demo_voc_crop.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_voc_vis.py` & `pybaseutils-1.1.1/test_py/demo_voc_vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,21 @@
     # class_name = "/home/dm/nasdata/dataset/csdn/traffic light/VOC/class_name.txt"
     # filename = "/home/dm/nasdata/dataset-dmai/handwriting/word-det/word-v1/train.txt"
     # filename = "/home/dm/nasdata/dataset/csdn/face_person/MPII/test.txt"
     # filename = "/home/dm/nasdata/dataset/csdn/Eyeglasses/dataset/face-eyeglasses/trainval.txt"
     # filename = "/home/dm/nasdata/dataset/tmp/insects/VOC2/VOC/VOCdevkit/trainval.txt"
     # filename = "/home/PKing/nasdata/dataset-dmai/AIJE/dataset/aije-det-dataset/dataset-v4/train.txt"
     filename = "/home/PKing/nasdata/dataset/tmp/pen/dataset-pen-finger-tip-v2/train/train.txt"
+    filename = "/home/PKing/Downloads/S-水表刻度数字检测6800/sample.txt"
     # filename = "/home/dm/nasdata/dataset-dmai/handwriting/word-det/word-old/train.txt"
     # class_name = ["face", "face-eyeglasses"]
     # class_name = "/home/dm/nasdata/dataset/tmp/traffic-sign/TT100K/VOC/train/class_name.txt"
     # class_name = ["unique"]
-    # class_name =None
-    class_name = ['pen_tip',"finger_tip"]
+    class_name =None
+    # class_name = ['pen_tip',"finger_tip"]
     dataset = parser_voc.VOCDataset(filename=filename,
                                     data_root=None,
                                     anno_dir=None,
                                     image_dir=None,
                                     class_name=class_name,
                                     transform=None,
                                     use_rgb=False,
```

### Comparing `pybaseutils-1.0.9/test_py/demo_word_similar.py` & `pybaseutils-1.1.1/test_py/demo_word_similar.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_worker1.py` & `pybaseutils-1.1.1/test_py/demo_worker1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/demo_worker2.py` & `pybaseutils-1.1.1/test_py/demo_worker2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/detector/demo.py` & `pybaseutils-1.1.1/test_py/detector/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/detector/detect_face_person.py` & `pybaseutils-1.1.1/test_py/detector/detect_face_person.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/detector/predet_labelme.py` & `pybaseutils-1.1.1/test_py/detector/predet_labelme.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/edit_distance/demo.py` & `pybaseutils-1.1.1/test_py/edit_distance/demo.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/edit_distance/text_matching.py` & `pybaseutils-1.1.1/test_py/edit_distance/text_matching.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/edit_distance/text_utils.py` & `pybaseutils-1.1.1/test_py/edit_distance/text_utils.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/flask_demo/server.py` & `pybaseutils-1.1.1/test_py/flask_demo/server.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/image_correction/demo_correction_v1.py` & `pybaseutils-1.1.1/test_py/image_correction/demo_correction_v1.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/image_correction/demo_correction_v2.py` & `pybaseutils-1.1.1/test_py/image_correction/demo_correction_v2.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/image_correction/demo_correction_v3.py` & `pybaseutils-1.1.1/test_py/image_correction/demo_correction_v3.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/kafka_worker.py` & `pybaseutils-1.1.1/test_py/kafka_worker.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/men_tracemalloc.py` & `pybaseutils-1.1.1/test_py/men_tracemalloc.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/performance.py` & `pybaseutils-1.1.1/test_py/performance.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/pose/human_pose.py` & `pybaseutils-1.1.1/test_py/pose/human_pose.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/registry/base.py` & `pybaseutils-1.1.1/test_py/registry/base.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/registry/component.py` & `pybaseutils-1.1.1/test_py/registry/component.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/registry/main.py` & `pybaseutils-1.1.1/test_py/registry/main.py`

 * *Files identical despite different names*

### Comparing `pybaseutils-1.0.9/test_py/registry/register.py` & `pybaseutils-1.1.1/test_py/registry/register.py`

 * *Files identical despite different names*

