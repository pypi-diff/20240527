# Comparing `tmp/machinevision-toolbox-python-0.9.6.tar.gz` & `tmp/machinevision_toolbox_python-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machinevision-toolbox-python-0.9.6.tar", last modified: Wed May  3 10:42:55 2023, max compression
+gzip compressed data, was "machinevision_toolbox_python-0.9.7.tar", last modified: Mon May 27 01:57:17 2024, max compression
```

## Comparing `machinevision-toolbox-python-0.9.6.tar` & `machinevision_toolbox_python-0.9.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-03 10:42:55.407884 machinevision-toolbox-python-0.9.6/
--rw-r--r--   0 corkep     (503) staff       (20)     1068 2021-01-26 22:01:12.000000 machinevision-toolbox-python-0.9.6/LICENSE
--rw-rw----   0 corkep     (503) staff       (20)    18814 2023-05-03 10:42:55.407331 machinevision-toolbox-python-0.9.6/PKG-INFO
--rw-r--r--   0 corkep     (503) staff       (20)    17534 2023-01-23 06:08:52.000000 machinevision-toolbox-python-0.9.6/README.md
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-03 10:42:55.288625 machinevision-toolbox-python-0.9.6/machinevision_toolbox_python.egg-info/
--rw-rw----   0 corkep     (503) staff       (20)    18814 2023-05-03 10:42:55.000000 machinevision-toolbox-python-0.9.6/machinevision_toolbox_python.egg-info/PKG-INFO
--rw-rw----   0 corkep     (503) staff       (20)     1871 2023-05-03 10:42:55.000000 machinevision-toolbox-python-0.9.6/machinevision_toolbox_python.egg-info/SOURCES.txt
--rw-rw----   0 corkep     (503) staff       (20)        1 2023-05-03 10:42:55.000000 machinevision-toolbox-python-0.9.6/machinevision_toolbox_python.egg-info/dependency_links.txt
--rw-rw----   0 corkep     (503) staff       (20)      276 2023-05-03 10:42:55.000000 machinevision-toolbox-python-0.9.6/machinevision_toolbox_python.egg-info/requires.txt
--rw-rw----   0 corkep     (503) staff       (20)       21 2023-05-03 10:42:55.000000 machinevision-toolbox-python-0.9.6/machinevision_toolbox_python.egg-info/top_level.txt
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-03 10:42:55.361003 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/
--rw-r--r--   0 corkep     (503) staff       (20)    19680 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/BagOfWords.py
--rw-r--r--   0 corkep     (503) staff       (20)    36081 2023-03-14 22:06:01.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/BundleAdjust.py
--rw-r--r--   0 corkep     (503) staff       (20)   135063 2023-03-13 20:32:42.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/Camera.py
--rw-r--r--   0 corkep     (503) staff       (20)    48997 2023-03-13 20:31:31.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageBlobs.py
--rw-r--r--   0 corkep     (503) staff       (20)    17111 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageColor.py
--rw-r--r--   0 corkep     (503) staff       (20)    13307 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageConstants.py
--rw-r--r--   0 corkep     (503) staff       (20)    79464 2023-03-15 04:46:45.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageCore.py
--rw-r--r--   0 corkep     (503) staff       (20)    20600 2023-03-15 04:24:24.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageIO.py
--rw-r--r--   0 corkep     (503) staff       (20)     9104 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageLineFeatures.py
--rw-r--r--   0 corkep     (503) staff       (20)    23789 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageMorph.py
--rw-r--r--   0 corkep     (503) staff       (20)    14703 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageMultiview.py
--rw-r--r--   0 corkep     (503) staff       (20)    76218 2023-03-13 20:29:31.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImagePointFeatures.py
--rw-r--r--   0 corkep     (503) staff       (20)    37975 2023-03-15 04:50:05.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageProcessing.py
--rw-r--r--   0 corkep     (503) staff       (20)    22175 2023-03-13 20:30:59.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageRegionFeatures.py
--rw-r--r--   0 corkep     (503) staff       (20)    45673 2023-03-15 04:34:59.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageReshape.py
--rw-r--r--   0 corkep     (503) staff       (20)    64761 2023-03-13 21:41:01.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageSpatial.py
--rw-r--r--   0 corkep     (503) staff       (20)    27698 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageWholeFeatures.py
--rw-r--r--   0 corkep     (503) staff       (20)    18286 2023-03-14 22:19:23.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/PointCloud.py
--rw-r--r--   0 corkep     (503) staff       (20)    28615 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/Sources.py
--rw-r--r--   0 corkep     (503) staff       (20)    59294 2023-03-15 04:51:49.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/VisualServo.py
--rw-r--r--   0 corkep     (503) staff       (20)     1257 2023-01-26 06:26:45.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/__init__.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-03 10:42:55.392128 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/
--rw-r--r--   0 corkep     (503) staff       (20)     1446 2023-03-14 20:17:58.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/__init__.py
--rwxr--r--   0 corkep     (503) staff       (20)    54593 2023-01-24 10:11:53.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/color.py
--rw-r--r--   0 corkep     (503) staff       (20)     5421 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/data.py
--rw-r--r--   0 corkep     (503) staff       (20)     2323 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/esttheta.py
--rw-r--r--   0 corkep     (503) staff       (20)    10377 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/findpeaks.py
--rw-r--r--   0 corkep     (503) staff       (20)    24663 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/graphics.py
--rw-r--r--   0 corkep     (503) staff       (20)    37425 2023-03-15 04:30:00.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/imageio.py
--rw-r--r--   0 corkep     (503) staff       (20)     2350 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/meshgrid.py
--rw-r--r--   0 corkep     (503) staff       (20)     9926 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/shapes.py
--rw-r--r--   0 corkep     (503) staff       (20)     4716 2023-03-13 20:35:32.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/types.py
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-03 10:42:55.395290 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/blocks/
--rw-r--r--   0 corkep     (503) staff       (20)      104 2023-01-24 11:07:53.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/blocks/__init__.py
--rw-r--r--   0 corkep     (503) staff       (20)     9776 2023-04-30 06:22:36.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/blocks/camera.py
--rwxr--r--   0 corkep     (503) staff       (20)     1572 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/blocks/test_blocks.py
--rw-r--r--   0 corkep     (503) staff       (20)    17557 2022-09-28 11:12:30.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/camera_derivatives.py
--rw-r--r--   0 corkep     (503) staff       (20)     1374 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/fiducial.py
--rw-r--r--   0 corkep     (503) staff       (20)     1225 2023-01-23 02:08:16.000000 machinevision-toolbox-python-0.9.6/machinevisiontoolbox/newcameras.py
--rw-r--r--   0 corkep     (503) staff       (20)     2221 2023-05-03 10:42:34.000000 machinevision-toolbox-python-0.9.6/pyproject.toml
--rw-rw----   0 corkep     (503) staff       (20)       38 2023-05-03 10:42:55.408019 machinevision-toolbox-python-0.9.6/setup.cfg
-drwxrwx---   0 corkep     (503) staff       (20)        0 2023-05-03 10:42:55.405750 machinevision-toolbox-python-0.9.6/tests/
--rw-r--r--   0 corkep     (503) staff       (20)     3120 2022-09-28 11:12:31.000000 machinevision-toolbox-python-0.9.6/tests/test_base_color.py
--rw-r--r--   0 corkep     (503) staff       (20)     5477 2022-09-28 11:12:31.000000 machinevision-toolbox-python-0.9.6/tests/test_camera.py
--rw-r--r--   0 corkep     (503) staff       (20)     2516 2022-11-06 19:14:50.000000 machinevision-toolbox-python-0.9.6/tests/test_color.py
--rw-r--r--   0 corkep     (503) staff       (20)    18846 2022-11-06 19:14:50.000000 machinevision-toolbox-python-0.9.6/tests/test_core.py
--rw-r--r--   0 corkep     (503) staff       (20)     4669 2022-11-06 19:14:50.000000 machinevision-toolbox-python-0.9.6/tests/test_image_io.py
--rw-r--r--   0 corkep     (503) staff       (20)     2702 2022-09-28 11:12:31.000000 machinevision-toolbox-python-0.9.6/tests/test_imageprocessing_kernel.py
--rw-r--r--   0 corkep     (503) staff       (20)    10086 2022-09-28 11:12:31.000000 machinevision-toolbox-python-0.9.6/tests/test_imageprocessing_morph.py
--rw-r--r--   0 corkep     (503) staff       (20)    11781 2022-09-28 11:12:31.000000 machinevision-toolbox-python-0.9.6/tests/test_processing.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-27 01:57:17.040982 machinevision_toolbox_python-0.9.7/
+-rw-r--r--   0 pic        (503) staff       (20)     1068 2021-01-26 22:01:12.000000 machinevision_toolbox_python-0.9.7/LICENSE
+-rw-r--r--   0 pic        (503) staff       (20)    19542 2024-05-27 01:57:17.040154 machinevision_toolbox_python-0.9.7/PKG-INFO
+-rw-r--r--   0 pic        (503) staff       (20)    17534 2023-01-23 06:08:52.000000 machinevision_toolbox_python-0.9.7/README.md
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-27 01:57:17.037817 machinevision_toolbox_python-0.9.7/machinevision_toolbox_python.egg-info/
+-rw-r--r--   0 pic        (503) staff       (20)    19542 2024-05-27 01:57:16.000000 machinevision_toolbox_python-0.9.7/machinevision_toolbox_python.egg-info/PKG-INFO
+-rw-rw----   0 pic        (503) staff       (20)     1871 2024-05-27 01:57:16.000000 machinevision_toolbox_python-0.9.7/machinevision_toolbox_python.egg-info/SOURCES.txt
+-rw-rw----   0 pic        (503) staff       (20)        1 2024-05-27 01:57:16.000000 machinevision_toolbox_python-0.9.7/machinevision_toolbox_python.egg-info/dependency_links.txt
+-rw-rw----   0 pic        (503) staff       (20)      276 2024-05-27 01:57:16.000000 machinevision_toolbox_python-0.9.7/machinevision_toolbox_python.egg-info/requires.txt
+-rw-rw----   0 pic        (503) staff       (20)       21 2024-05-27 01:57:16.000000 machinevision_toolbox_python-0.9.7/machinevision_toolbox_python.egg-info/top_level.txt
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-27 01:57:17.016711 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/
+-rw-r--r--   0 pic        (503) staff       (20)    19680 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/BagOfWords.py
+-rw-r--r--   0 pic        (503) staff       (20)    36081 2023-03-14 22:06:01.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/BundleAdjust.py
+-rw-r--r--   0 pic        (503) staff       (20)   135063 2023-03-13 20:32:42.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/Camera.py
+-rw-r--r--   0 pic        (503) staff       (20)    49166 2024-05-26 02:51:18.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageBlobs.py
+-rw-r--r--   0 pic        (503) staff       (20)    17111 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageColor.py
+-rw-r--r--   0 pic        (503) staff       (20)    13307 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageConstants.py
+-rw-r--r--   0 pic        (503) staff       (20)    79464 2023-03-15 04:46:45.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageCore.py
+-rw-r--r--   0 pic        (503) staff       (20)    20600 2023-03-15 04:24:24.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageIO.py
+-rw-r--r--   0 pic        (503) staff       (20)     9104 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageLineFeatures.py
+-rw-r--r--   0 pic        (503) staff       (20)    23789 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageMorph.py
+-rw-r--r--   0 pic        (503) staff       (20)    14703 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageMultiview.py
+-rw-r--r--   0 pic        (503) staff       (20)    76218 2023-03-13 20:29:31.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImagePointFeatures.py
+-rw-r--r--   0 pic        (503) staff       (20)    37975 2023-03-15 04:50:05.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageProcessing.py
+-rw-r--r--   0 pic        (503) staff       (20)    22175 2023-03-13 20:30:59.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageRegionFeatures.py
+-rw-r--r--   0 pic        (503) staff       (20)    45673 2023-03-15 04:34:59.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageReshape.py
+-rw-r--r--   0 pic        (503) staff       (20)    64761 2023-03-13 21:41:01.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageSpatial.py
+-rw-r--r--   0 pic        (503) staff       (20)    27698 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageWholeFeatures.py
+-rw-r--r--   0 pic        (503) staff       (20)    18286 2023-03-14 22:19:23.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/PointCloud.py
+-rw-r--r--   0 pic        (503) staff       (20)    28615 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/Sources.py
+-rw-r--r--   0 pic        (503) staff       (20)    59294 2023-03-15 04:51:49.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/VisualServo.py
+-rw-r--r--   0 pic        (503) staff       (20)     1257 2023-01-26 06:26:45.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/__init__.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-27 01:57:17.021560 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/
+-rw-r--r--   0 pic        (503) staff       (20)     1446 2023-03-14 20:17:58.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/__init__.py
+-rwxr--r--   0 pic        (503) staff       (20)    54593 2023-01-24 10:11:53.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/color.py
+-rw-r--r--   0 pic        (503) staff       (20)     5421 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/data.py
+-rw-r--r--   0 pic        (503) staff       (20)     2323 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/esttheta.py
+-rw-r--r--   0 pic        (503) staff       (20)    10377 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/findpeaks.py
+-rw-r--r--   0 pic        (503) staff       (20)    24663 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/graphics.py
+-rw-r--r--   0 pic        (503) staff       (20)    37425 2023-03-15 04:30:00.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/imageio.py
+-rw-r--r--   0 pic        (503) staff       (20)     2350 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/meshgrid.py
+-rw-r--r--   0 pic        (503) staff       (20)     9926 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/shapes.py
+-rw-r--r--   0 pic        (503) staff       (20)     4716 2023-03-13 20:35:32.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/types.py
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-27 01:57:17.023215 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/blocks/
+-rw-r--r--   0 pic        (503) staff       (20)      104 2023-01-24 11:07:53.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/blocks/__init__.py
+-rw-r--r--   0 pic        (503) staff       (20)     9776 2023-04-30 06:22:36.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/blocks/camera.py
+-rwxr--r--   0 pic        (503) staff       (20)     1572 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/blocks/test_blocks.py
+-rw-r--r--   0 pic        (503) staff       (20)    17557 2022-09-28 11:12:30.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/camera_derivatives.py
+-rw-r--r--   0 pic        (503) staff       (20)     1374 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/fiducial.py
+-rw-r--r--   0 pic        (503) staff       (20)     1225 2023-01-23 02:08:16.000000 machinevision_toolbox_python-0.9.7/machinevisiontoolbox/newcameras.py
+-rw-r--r--   0 pic        (503) staff       (20)     2222 2024-05-27 01:57:00.000000 machinevision_toolbox_python-0.9.7/pyproject.toml
+-rw-rw----   0 pic        (503) staff       (20)       38 2024-05-27 01:57:17.041078 machinevision_toolbox_python-0.9.7/setup.cfg
+drwxrwx---   0 pic        (503) staff       (20)        0 2024-05-27 01:57:17.028990 machinevision_toolbox_python-0.9.7/tests/
+-rw-r--r--   0 pic        (503) staff       (20)     3120 2022-09-28 11:12:31.000000 machinevision_toolbox_python-0.9.7/tests/test_base_color.py
+-rw-r--r--   0 pic        (503) staff       (20)     5477 2022-09-28 11:12:31.000000 machinevision_toolbox_python-0.9.7/tests/test_camera.py
+-rw-r--r--   0 pic        (503) staff       (20)     2516 2022-11-06 19:14:50.000000 machinevision_toolbox_python-0.9.7/tests/test_color.py
+-rw-r--r--   0 pic        (503) staff       (20)    18846 2022-11-06 19:14:50.000000 machinevision_toolbox_python-0.9.7/tests/test_core.py
+-rw-r--r--   0 pic        (503) staff       (20)     4669 2022-11-06 19:14:50.000000 machinevision_toolbox_python-0.9.7/tests/test_image_io.py
+-rw-r--r--   0 pic        (503) staff       (20)     2702 2022-09-28 11:12:31.000000 machinevision_toolbox_python-0.9.7/tests/test_imageprocessing_kernel.py
+-rw-r--r--   0 pic        (503) staff       (20)    10086 2022-09-28 11:12:31.000000 machinevision_toolbox_python-0.9.7/tests/test_imageprocessing_morph.py
+-rw-r--r--   0 pic        (503) staff       (20)    11781 2022-09-28 11:12:31.000000 machinevision_toolbox_python-0.9.7/tests/test_processing.py
```

### Comparing `machinevision-toolbox-python-0.9.6/LICENSE` & `machinevision_toolbox_python-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/PKG-INFO` & `machinevision_toolbox_python-0.9.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: machinevision-toolbox-python
-Version: 0.9.6
-Summary: Python tools for machine vision - education and research
-Author: Dorian Tsai
-Author-email: Peter Corke <rvc@petercorke.com>
-Project-URL: Homepage, https://github.com/petercorke/machinevision-toolbox-python
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Project-URL: Documentation, https://petercorke.github.io/machinevision-toolbox-python
-Project-URL: Source, https://github.com/petercorke/machinevision-toolbox-python
-Keywords: machine vision,computer vision,multiview geometry,stereo vision,bundle adjustment,visual servoing,image features,color,blobs,morphology,image segmentation,opencv,open3d
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 # Machine Vision Toolbox for Python
 
 [![A Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-python)
 [![Powered by Spatial Maths](https://raw.githubusercontent.com/petercorke/spatialmath-python/master/.github/svg/sm_powered.min.svg)](https://github.com/petercorke/spatialmath-python)
 [![QUT Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https://qcr.github.io)
 
 [![PyPI version](https://badge.fury.io/py/machinevision-toolbox-python.svg)](https://badge.fury.io/py/machinevision-toolbox-python)
```

#### html2text {}

```diff
@@ -1,46 +1,28 @@
-Metadata-Version: 2.1 Name: machinevision-toolbox-python Version: 0.9.6
-Summary: Python tools for machine vision - education and research Author:
-Dorian Tsai Author-email: Peter Corke
-petercorke.com> Project-URL: Homepage, https://github.com/petercorke/
-machinevision-toolbox-python Project-URL: Bug Tracker, https://github.com/pypa/
-sampleproject/issues Project-URL: Documentation, https://petercorke.github.io/
-machinevision-toolbox-python Project-URL: Source, https://github.com/
-petercorke/machinevision-toolbox-python Keywords: machine vision,computer
-vision,multiview geometry,stereo vision,bundle adjustment,visual servoing,image
-features,color,blobs,morphology,image segmentation,opencv,open3d Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Developers Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: License :: OSI Approved ::
-MIT License Classifier: Operating System :: OS Independent Requires-Python:
->=3.7 Description-Content-Type: text/markdown Provides-Extra: dev Provides-
-Extra: docs License-File: LICENSE # Machine Vision Toolbox for Python [![A
-Python Robotics Package](https://raw.githubusercontent.com/petercorke/robotics-
-toolbox-python/master/.github/svg/py_collection.min.svg)](https://github.com/
-petercorke/robotics-toolbox-python) [![Powered by Spatial Maths](https://
-raw.githubusercontent.com/petercorke/spatialmath-python/master/.github/svg/
-sm_powered.min.svg)](https://github.com/petercorke/spatialmath-python) [![QUT
-Centre for Robotics Open Source](https://github.com/qcr/qcr.github.io/raw/
-master/misc/badge.svg)](https://qcr.github.io) [![PyPI version](https://
-badge.fury.io/py/machinevision-toolbox-python.svg)](https://badge.fury.io/py/
-machinevision-toolbox-python) ![Python Version](https://img.shields.io/pypi/
-pyversions/machinevision-toolbox-python.svg) [![Powered by OpenCV](https://
-raw.githubusercontent.com/petercorke/machinevision-toolbox-python/
-master/.github/svg/opencv_powered.svg)](https://opencv.org) [![Powered by
-Open3D](https://raw.githubusercontent.com/petercorke/machinevision-toolbox-
-python/master/.github/svg/open3d_powered.svg)](https://open3d.org) [![License:
-MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
-opensource.org/licenses/MIT) [![Build Status](https://github.com/petercorke/
-machinevision-toolbox-python/workflows/Test-master/badge.svg?branch=master)]
-(https://github.com/petercorke/machinevision-toolbox-python/
-actions?query=workflow%3Abuild) [![Coverage](https://codecov.io/gh/petercorke/
-machinevision-toolbox-python/branch/master/graph/badge.svg)](https://
-codecov.io/gh/petercorke/machinevision-toolbox-python) [![PyPI - Downloads]
+# Machine Vision Toolbox for Python [![A Python Robotics Package](https://
+raw.githubusercontent.com/petercorke/robotics-toolbox-python/master/.github/
+svg/py_collection.min.svg)](https://github.com/petercorke/robotics-toolbox-
+python) [![Powered by Spatial Maths](https://raw.githubusercontent.com/
+petercorke/spatialmath-python/master/.github/svg/sm_powered.min.svg)](https://
+github.com/petercorke/spatialmath-python) [![QUT Centre for Robotics Open
+Source](https://github.com/qcr/qcr.github.io/raw/master/misc/badge.svg)](https:
+//qcr.github.io) [![PyPI version](https://badge.fury.io/py/machinevision-
+toolbox-python.svg)](https://badge.fury.io/py/machinevision-toolbox-python) !
+[Python Version](https://img.shields.io/pypi/pyversions/machinevision-toolbox-
+python.svg) [![Powered by OpenCV](https://raw.githubusercontent.com/petercorke/
+machinevision-toolbox-python/master/.github/svg/opencv_powered.svg)](https://
+opencv.org) [![Powered by Open3D](https://raw.githubusercontent.com/petercorke/
+machinevision-toolbox-python/master/.github/svg/open3d_powered.svg)](https://
+open3d.org) [![License: MIT](https://img.shields.io/badge/License-MIT-
+yellow.svg)](https://opensource.org/licenses/MIT) [![Build Status](https://
+github.com/petercorke/machinevision-toolbox-python/workflows/Test-master/
+badge.svg?branch=master)](https://github.com/petercorke/machinevision-toolbox-
+python/actions?query=workflow%3Abuild) [![Coverage](https://codecov.io/gh/
+petercorke/machinevision-toolbox-python/branch/master/graph/badge.svg)](https:/
+/codecov.io/gh/petercorke/machinevision-toolbox-python) [![PyPI - Downloads]
 (https://img.shields.io/pypi/dw/machinevision-toolbox-python)](https://
 pypistats.org/packages/machinevision-toolbox-python)
                                          A Python implementation of the _M_a_c_h_i_n_e
 [https://github.com/petercorke/          _V_i_s_i_o_n_ _T_o_o_l_b_o_x_ _f_o_r_ _M_A_T_L_A_B_®
 machinevision-toolbox-python/raw/master/     * _G_i_t_H_u_b_ _r_e_p_o_s_i_t_o_r_y
 figs/VisionToolboxLogo_NoBackgnd@2x.png]     * _D_o_c_u_m_e_n_t_a_t_i_o_n
                                              * _E_x_a_m_p_l_e_s_ _a_n_d_ _d_e_t_a_i_l_s
```

### Comparing `machinevision-toolbox-python-0.9.6/README.md` & `machinevision_toolbox_python-0.9.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,1096 +1,1222 @@
-00000000: 2320 4d61 6368 696e 6520 5669 7369 6f6e  # Machine Vision
-00000010: 2054 6f6f 6c62 6f78 2066 6f72 2050 7974   Toolbox for Pyt
-00000020: 686f 6e0a 0a5b 215b 4120 5079 7468 6f6e  hon..[![A Python
-00000030: 2052 6f62 6f74 6963 7320 5061 636b 6167   Robotics Packag
-00000040: 655d 2868 7474 7073 3a2f 2f72 6177 2e67  e](https://raw.g
-00000050: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00000060: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
-00000070: 726f 626f 7469 6373 2d74 6f6f 6c62 6f78  robotics-toolbox
-00000080: 2d70 7974 686f 6e2f 6d61 7374 6572 2f2e  -python/master/.
-00000090: 6769 7468 7562 2f73 7667 2f70 795f 636f  github/svg/py_co
-000000a0: 6c6c 6563 7469 6f6e 2e6d 696e 2e73 7667  llection.min.svg
-000000b0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-000000c0: 622e 636f 6d2f 7065 7465 7263 6f72 6b65  b.com/petercorke
-000000d0: 2f72 6f62 6f74 6963 732d 746f 6f6c 626f  /robotics-toolbo
-000000e0: 782d 7079 7468 6f6e 290a 5b21 5b50 6f77  x-python).[![Pow
-000000f0: 6572 6564 2062 7920 5370 6174 6961 6c20  ered by Spatial 
-00000100: 4d61 7468 735d 2868 7474 7073 3a2f 2f72  Maths](https://r
-00000110: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000120: 7465 6e74 2e63 6f6d 2f70 6574 6572 636f  tent.com/peterco
-00000130: 726b 652f 7370 6174 6961 6c6d 6174 682d  rke/spatialmath-
-00000140: 7079 7468 6f6e 2f6d 6173 7465 722f 2e67  python/master/.g
-00000150: 6974 6875 622f 7376 672f 736d 5f70 6f77  ithub/svg/sm_pow
-00000160: 6572 6564 2e6d 696e 2e73 7667 295d 2868  ered.min.svg)](h
-00000170: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000180: 6d2f 7065 7465 7263 6f72 6b65 2f73 7061  m/petercorke/spa
-00000190: 7469 616c 6d61 7468 2d70 7974 686f 6e29  tialmath-python)
-000001a0: 0a5b 215b 5155 5420 4365 6e74 7265 2066  .[![QUT Centre f
-000001b0: 6f72 2052 6f62 6f74 6963 7320 4f70 656e  or Robotics Open
-000001c0: 2053 6f75 7263 655d 2868 7474 7073 3a2f   Source](https:/
-000001d0: 2f67 6974 6875 622e 636f 6d2f 7163 722f  /github.com/qcr/
-000001e0: 7163 722e 6769 7468 7562 2e69 6f2f 7261  qcr.github.io/ra
-000001f0: 772f 6d61 7374 6572 2f6d 6973 632f 6261  w/master/misc/ba
-00000200: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
-00000210: 2f2f 7163 722e 6769 7468 7562 2e69 6f29  //qcr.github.io)
-00000220: 0a0a 5b21 5b50 7950 4920 7665 7273 696f  ..[![PyPI versio
-00000230: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
-00000240: 2e66 7572 792e 696f 2f70 792f 6d61 6368  .fury.io/py/mach
-00000250: 696e 6576 6973 696f 6e2d 746f 6f6c 626f  inevision-toolbo
-00000260: 782d 7079 7468 6f6e 2e73 7667 295d 2868  x-python.svg)](h
-00000270: 7474 7073 3a2f 2f62 6164 6765 2e66 7572  ttps://badge.fur
-00000280: 792e 696f 2f70 792f 6d61 6368 696e 6576  y.io/py/machinev
-00000290: 6973 696f 6e2d 746f 6f6c 626f 782d 7079  ision-toolbox-py
-000002a0: 7468 6f6e 290a 215b 5079 7468 6f6e 2056  thon).![Python V
-000002b0: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
-000002c0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-000002d0: 7970 692f 7079 7665 7273 696f 6e73 2f6d  ypi/pyversions/m
-000002e0: 6163 6869 6e65 7669 7369 6f6e 2d74 6f6f  achinevision-too
-000002f0: 6c62 6f78 2d70 7974 686f 6e2e 7376 6729  lbox-python.svg)
-00000300: 0a5b 215b 506f 7765 7265 6420 6279 204f  .[![Powered by O
-00000310: 7065 6e43 565d 2868 7474 7073 3a2f 2f72  penCV](https://r
-00000320: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000330: 7465 6e74 2e63 6f6d 2f70 6574 6572 636f  tent.com/peterco
-00000340: 726b 652f 6d61 6368 696e 6576 6973 696f  rke/machinevisio
-00000350: 6e2d 746f 6f6c 626f 782d 7079 7468 6f6e  n-toolbox-python
-00000360: 2f6d 6173 7465 722f 2e67 6974 6875 622f  /master/.github/
-00000370: 7376 672f 6f70 656e 6376 5f70 6f77 6572  svg/opencv_power
-00000380: 6564 2e73 7667 295d 2868 7474 7073 3a2f  ed.svg)](https:/
-00000390: 2f6f 7065 6e63 762e 6f72 6729 0a5b 215b  /opencv.org).[![
-000003a0: 506f 7765 7265 6420 6279 204f 7065 6e33  Powered by Open3
-000003b0: 445d 2868 7474 7073 3a2f 2f72 6177 2e67  D](https://raw.g
-000003c0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-000003d0: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
-000003e0: 6d61 6368 696e 6576 6973 696f 6e2d 746f  machinevision-to
-000003f0: 6f6c 626f 782d 7079 7468 6f6e 2f6d 6173  olbox-python/mas
-00000400: 7465 722f 2e67 6974 6875 622f 7376 672f  ter/.github/svg/
-00000410: 6f70 656e 3364 5f70 6f77 6572 6564 2e73  open3d_powered.s
-00000420: 7667 295d 2868 7474 7073 3a2f 2f6f 7065  vg)](https://ope
-00000430: 6e33 642e 6f72 6729 0a5b 215b 4c69 6365  n3d.org).[![Lice
-00000440: 6e73 653a 204d 4954 5d28 6874 7470 733a  nse: MIT](https:
-00000450: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000460: 2f62 6164 6765 2f4c 6963 656e 7365 2d4d  /badge/License-M
-00000470: 4954 2d79 656c 6c6f 772e 7376 6729 5d28  IT-yellow.svg)](
-00000480: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
-00000490: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
-000004a0: 4d49 5429 0a0a 5b21 5b42 7569 6c64 2053  MIT)..[![Build S
-000004b0: 7461 7475 735d 2868 7474 7073 3a2f 2f67  tatus](https://g
-000004c0: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
-000004d0: 6f72 6b65 2f6d 6163 6869 6e65 7669 7369  orke/machinevisi
-000004e0: 6f6e 2d74 6f6f 6c62 6f78 2d70 7974 686f  on-toolbox-pytho
-000004f0: 6e2f 776f 726b 666c 6f77 732f 5465 7374  n/workflows/Test
-00000500: 2d6d 6173 7465 722f 6261 6467 652e 7376  -master/badge.sv
-00000510: 673f 6272 616e 6368 3d6d 6173 7465 7229  g?branch=master)
-00000520: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000530: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
-00000540: 6d61 6368 696e 6576 6973 696f 6e2d 746f  machinevision-to
-00000550: 6f6c 626f 782d 7079 7468 6f6e 2f61 6374  olbox-python/act
-00000560: 696f 6e73 3f71 7565 7279 3d77 6f72 6b66  ions?query=workf
-00000570: 6c6f 7725 3341 6275 696c 6429 0a5b 215b  low%3Abuild).[![
-00000580: 436f 7665 7261 6765 5d28 6874 7470 733a  Coverage](https:
-00000590: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
-000005a0: 7065 7465 7263 6f72 6b65 2f6d 6163 6869  petercorke/machi
-000005b0: 6e65 7669 7369 6f6e 2d74 6f6f 6c62 6f78  nevision-toolbox
-000005c0: 2d70 7974 686f 6e2f 6272 616e 6368 2f6d  -python/branch/m
-000005d0: 6173 7465 722f 6772 6170 682f 6261 6467  aster/graph/badg
-000005e0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-000005f0: 636f 6465 636f 762e 696f 2f67 682f 7065  codecov.io/gh/pe
-00000600: 7465 7263 6f72 6b65 2f6d 6163 6869 6e65  tercorke/machine
-00000610: 7669 7369 6f6e 2d74 6f6f 6c62 6f78 2d70  vision-toolbox-p
-00000620: 7974 686f 6e29 0a5b 215b 5079 5049 202d  ython).[![PyPI -
-00000630: 2044 6f77 6e6c 6f61 6473 5d28 6874 7470   Downloads](http
-00000640: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000650: 696f 2f70 7970 692f 6477 2f6d 6163 6869  io/pypi/dw/machi
-00000660: 6e65 7669 7369 6f6e 2d74 6f6f 6c62 6f78  nevision-toolbox
-00000670: 2d70 7974 686f 6e29 5d28 6874 7470 733a  -python)](https:
-00000680: 2f2f 7079 7069 7374 6174 732e 6f72 672f  //pypistats.org/
-00000690: 7061 636b 6167 6573 2f6d 6163 6869 6e65  packages/machine
-000006a0: 7669 7369 6f6e 2d74 6f6f 6c62 6f78 2d70  vision-toolbox-p
-000006b0: 7974 686f 6e29 0a0a 3c21 2d2d 205b 215b  ython)..<!-- [![
-000006c0: 4769 7448 7562 2073 7461 7273 5d28 6874  GitHub stars](ht
-000006d0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000006e0: 732e 696f 2f67 6974 6875 622f 7374 6172  s.io/github/star
-000006f0: 732f 7065 7465 7263 6f72 6b65 2f6d 6163  s/petercorke/mac
-00000700: 6869 6e65 7669 7369 6f6e 2d74 6f6f 6c62  hinevision-toolb
-00000710: 6f78 2d70 7974 686f 6e2e 7376 673f 7374  ox-python.svg?st
-00000720: 796c 653d 736f 6369 616c 266c 6162 656c  yle=social&label
-00000730: 3d53 7461 7229 5d28 6874 7470 733a 2f2f  =Star)](https://
-00000740: 4769 7448 7562 2e63 6f6d 2f70 6574 6572  GitHub.com/peter
-00000750: 636f 726b 652f 6d61 6368 696e 6576 6973  corke/machinevis
-00000760: 696f 6e2d 746f 6f6c 626f 782d 7079 7468  ion-toolbox-pyth
-00000770: 6f6e 2f73 7461 7267 617a 6572 732f 2920  on/stargazers/) 
-00000780: 2d2d 3e0a 0a3c 7461 626c 6520 7374 796c  -->..<table styl
-00000790: 653d 2262 6f72 6465 723a 3070 7822 3e0a  e="border:0px">.
-000007a0: 3c74 7220 7374 796c 653d 2262 6f72 6465  <tr style="borde
-000007b0: 723a 3070 7822 3e0a 3c74 6420 7374 796c  r:0px">.<td styl
-000007c0: 653d 2262 6f72 6465 723a 3070 7822 3e0a  e="border:0px">.
-000007d0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-000007e0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 6574  //github.com/pet
-000007f0: 6572 636f 726b 652f 6d61 6368 696e 6576  ercorke/machinev
-00000800: 6973 696f 6e2d 746f 6f6c 626f 782d 7079  ision-toolbox-py
-00000810: 7468 6f6e 2f72 6177 2f6d 6173 7465 722f  thon/raw/master/
-00000820: 6669 6773 2f56 6973 696f 6e54 6f6f 6c62  figs/VisionToolb
-00000830: 6f78 4c6f 676f 5f4e 6f42 6163 6b67 6e64  oxLogo_NoBackgnd
-00000840: 4032 782e 706e 6722 2077 6964 7468 3d22  @2x.png" width="
-00000850: 3230 3022 3e3c 2f74 643e 0a3c 7464 2073  200"></td>.<td s
-00000860: 7479 6c65 3d22 626f 7264 6572 3a30 7078  tyle="border:0px
-00000870: 223e 0a0a 4120 5079 7468 6f6e 2069 6d70  ">..A Python imp
-00000880: 6c65 6d65 6e74 6174 696f 6e20 6f66 2074  lementation of t
-00000890: 6865 203c 6120 6872 6566 3d22 6874 7470  he <a href="http
-000008a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-000008b0: 6574 6572 636f 726b 652f 6d61 6368 696e  etercorke/machin
-000008c0: 6576 6973 696f 6e2d 746f 6f6c 626f 782d  evision-toolbox-
-000008d0: 6d61 746c 6162 223e 4d61 6368 696e 6520  matlab">Machine 
-000008e0: 5669 7369 6f6e 2054 6f6f 6c62 6f78 2066  Vision Toolbox f
-000008f0: 6f72 204d 4154 4c41 423c 7375 703e 2672  or MATLAB<sup>&r
-00000900: 6567 3b3c 2f73 7570 3e3c 2f61 3e3c 756c  eg;</sup></a><ul
-00000910: 3e0a 0a3c 6c69 3e3c 6120 6872 6566 3d22  >..<li><a href="
-00000920: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000930: 6f6d 2f70 6574 6572 636f 726b 652f 6d61  om/petercorke/ma
-00000940: 6368 696e 6576 6973 696f 6e2d 746f 6f6c  chinevision-tool
-00000950: 626f 782d 7079 7468 6f6e 223e 4769 7448  box-python">GitH
-00000960: 7562 2072 6570 6f73 6974 6f72 7920 3c2f  ub repository </
-00000970: 613e 3c2f 6c69 3e0a 3c6c 693e 3c61 2068  a></li>.<li><a h
-00000980: 7265 663d 2268 7474 7073 3a2f 2f70 6574  ref="https://pet
-00000990: 6572 636f 726b 652e 6769 7468 7562 2e69  ercorke.github.i
-000009a0: 6f2f 6d61 6368 696e 6576 6973 696f 6e2d  o/machinevision-
-000009b0: 746f 6f6c 626f 782d 7079 7468 6f6e 2f22  toolbox-python/"
-000009c0: 3e44 6f63 756d 656e 7461 7469 6f6e 3c2f  >Documentation</
-000009d0: 613e 3c2f 6c69 3e0a 3c6c 693e 3c61 2068  a></li>.<li><a h
-000009e0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-000009f0: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
-00000a00: 6b65 2f6d 6163 6869 6e65 7669 7369 6f6e  ke/machinevision
-00000a10: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e2f  -toolbox-python/
-00000a20: 7769 6b69 223e 4578 616d 706c 6573 2061  wiki">Examples a
-00000a30: 6e64 2064 6574 6169 6c73 3c2f 613e 3c2f  nd details</a></
-00000a40: 6c69 3e0a 3c6c 693e 3c61 2068 7265 663d  li>.<li><a href=
-00000a50: 2269 6e73 7461 6c6c 6174 696f 6e23 223e  "installation#">
-00000a60: 496e 7374 616c 6c61 7469 6f6e 3c2f 613e  Installation</a>
-00000a70: 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f 7464  </li>.</ul>.</td
-00000a80: 3e0a 3c2f 7472 3e0a 3c2f 7461 626c 653e  >.</tr>.</table>
-00000a90: 0a0a 2323 2053 796e 6f70 7369 730a 0a54  ..## Synopsis..T
-00000aa0: 6865 204d 6163 6869 6e65 2056 6973 696f  he Machine Visio
-00000ab0: 6e20 546f 6f6c 626f 7820 666f 7220 5079  n Toolbox for Py
-00000ac0: 7468 6f6e 2028 4d56 5442 2d50 2920 7072  thon (MVTB-P) pr
-00000ad0: 6f76 6964 6573 206d 616e 7920 6675 6e63  ovides many func
-00000ae0: 7469 6f6e 7320 7468 6174 2061 7265 2075  tions that are u
-00000af0: 7365 6675 6c20 696e 206d 6163 6869 6e65  seful in machine
-00000b00: 2076 6973 696f 6e20 616e 6420 7669 7369   vision and visi
-00000b10: 6f6e 2d62 6173 6564 2063 6f6e 7472 6f6c  on-based control
-00000b20: 2e20 5468 6520 6d61 696e 2063 6f6d 706f  . The main compo
-00000b30: 6e65 6e74 7320 6172 653a 0a0a 2d20 416e  nents are:..- An
-00000b40: 2060 496d 6167 6560 206f 626a 6563 7420   `Image` object 
-00000b50: 7769 7468 206e 6561 726c 7920 3230 3020  with nearly 200 
-00000b60: 6d65 7468 6f64 7320 616e 6420 7072 6f70  methods and prop
-00000b70: 6572 7469 6573 2074 6861 7420 7772 6170  erties that wrap
-00000b80: 2066 756e 6374 696f 6e73 0a20 2066 726f   functions.  fro
-00000b90: 6d20 4f70 656e 4356 2c20 4e75 6d50 7920  m OpenCV, NumPy 
-00000ba0: 616e 6420 5363 6950 792e 204d 6574 686f  and SciPy. Metho
-00000bb0: 6473 2073 7570 706f 7274 206d 6f6e 6164  ds support monad
-00000bc0: 6963 2c20 6479 6164 6963 2c20 6669 6c74  ic, dyadic, filt
-00000bd0: 6572 696e 672c 2065 6467 6520 6465 7465  ering, edge dete
-00000be0: 6374 696f 6e2c 0a20 206d 6174 6865 6d61  ction,.  mathema
-00000bf0: 7469 6361 6c20 6d6f 7270 686f 6c6f 6779  tical morphology
-00000c00: 2061 6e64 2066 6561 7475 7265 2065 7874   and feature ext
-00000c10: 7261 6374 696f 6e20 2862 6c6f 6273 2c20  raction (blobs, 
-00000c20: 6c69 6e65 7320 616e 6420 706f 696e 742f  lines and point/
-00000c30: 636f 726e 6572 2066 6561 7475 7265 7329  corner features)
-00000c40: 2c20 6173 2077 656c 6c20 6173 206f 7065  , as well as ope
-00000c50: 7261 746f 7220 6f76 6572 6c6f 6164 696e  rator overloadin
-00000c60: 672e 2049 6d61 6765 7320 6172 6520 7374  g. Images are st
-00000c70: 6f72 6564 2061 7320 656e 6361 7073 756c  ored as encapsul
-00000c80: 6174 6564 205b 4e75 6d50 795d 2868 7474  ated [NumPy](htt
-00000c90: 7073 3a2f 2f6e 756d 7079 2e6f 7267 2920  ps://numpy.org) 
-00000ca0: 6172 7261 7973 0a20 2061 6c6f 6e67 2077  arrays.  along w
-00000cb0: 6974 6820 696d 6167 6520 6d65 7461 6461  ith image metada
-00000cc0: 7461 2e0a 2d20 416e 206f 626a 6563 742d  ta..- An object-
-00000cd0: 6f72 6965 6e74 6564 2077 7261 7070 6572  oriented wrapper
-00000ce0: 206f 6620 4f70 656e 3344 2066 756e 6374   of Open3D funct
-00000cf0: 696f 6e73 2074 6861 7420 7375 7070 6f72  ions that suppor
-00000d00: 7473 2061 2073 7562 7365 7420 6f66 206f  ts a subset of o
-00000d10: 7065 7261 7469 6f6e 732c 2062 7574 2061  perations, but a
-00000d20: 6c6c 6f77 7320 6f70 6572 6174 6f72 206f  llows operator o
-00000d30: 7665 726c 6f61 6469 6e67 2061 6e64 2069  verloading and i
-00000d40: 7320 636f 6d70 6174 6962 6c65 2077 6974  s compatible wit
-00000d50: 6820 7468 6520 5b53 7061 7469 616c 204d  h the [Spatial M
-00000d60: 6174 6820 546f 6f6c 626f 785d 2868 7474  ath Toolbox](htt
-00000d70: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000d80: 7065 7465 7263 6f72 6b65 2f73 7061 7469  petercorke/spati
-00000d90: 616c 6d61 7468 2d70 7974 686f 6e29 2e0a  almath-python)..
-00000da0: 2d20 4120 636f 6c6c 6563 7469 6f6e 206f  - A collection o
-00000db0: 6620 6361 6d65 7261 2070 726f 6a65 6374  f camera project
-00000dc0: 696f 6e20 636c 6173 7365 7320 666f 7220  ion classes for 
-00000dd0: 6365 6e74 7261 6c20 286e 6f72 6d61 6c20  central (normal 
-00000de0: 7065 7273 7065 6374 6976 6529 2c20 6669  perspective), fi
-00000df0: 7368 6579 652c 2063 6174 6164 696f 7074  sheye, catadiopt
-00000e00: 7269 6320 616e 6420 7370 6865 7269 6361  ric and spherica
-00000e10: 6c20 6361 6d65 7261 732e 0a2d 2053 6f6d  l cameras..- Som
-00000e20: 6520 6164 7661 6e63 6564 2061 6c67 6f72  e advanced algor
-00000e30: 6974 686d 7320 7375 6368 2061 733a 0a20  ithms such as:. 
-00000e40: 202d 206d 756c 7469 7669 6577 2067 656f   - multiview geo
-00000e50: 6d65 7472 793a 2063 616d 6572 6120 6361  metry: camera ca
-00000e60: 6c69 6272 6174 696f 6e2c 2073 7465 7265  libration, stere
-00000e70: 6f20 7669 7369 6f6e 2c20 6275 6e64 6c65  o vision, bundle
-00000e80: 2061 646a 7573 746d 656e 740a 2020 2d20   adjustment.  - 
-00000e90: 6261 6720 6f66 2077 6f72 6473 0a0a 4164  bag of words..Ad
-00000ea0: 7661 6e74 6167 6573 206f 6620 7468 6973  vantages of this
-00000eb0: 2050 7974 686f 6e20 546f 6f6c 626f 7820   Python Toolbox 
-00000ec0: 6172 6520 7468 6174 3a0a 0a2d 2069 7420  are that:..- it 
-00000ed0: 7573 6573 2c20 6173 206d 7563 6820 6173  uses, as much as
-00000ee0: 2070 6f73 7369 626c 652c 205b 4f70 656e   possible, [Open
-00000ef0: 4356 5d28 6874 7470 733a 2f2f 6f70 656e  CV](https://open
-00000f00: 6376 2e6f 7267 2920 616e 6420 5b4e 756d  cv.org) and [Num
-00000f10: 5079 5d28 6874 7470 733a 2f2f 6e75 6d70  Py](https://nump
-00000f20: 792e 6f72 6729 2077 6869 6368 2061 7265  y.org) which are
-00000f30: 2070 6f72 7461 626c 652c 2065 6666 6963   portable, effic
-00000f40: 6965 6e74 2c20 636f 6d70 7265 6865 6e73  ient, comprehens
-00000f50: 6976 6520 616e 6420 6d61 7475 7265 2063  ive and mature c
-00000f60: 6f6c 6c65 6374 696f 6e20 6f66 2066 756e  ollection of fun
-00000f70: 6374 696f 6e73 2066 6f72 2069 6d61 6765  ctions for image
-00000f80: 2070 726f 6365 7373 696e 6720 616e 6420   processing and 
-00000f90: 6665 6174 7572 6520 6578 7472 6163 7469  feature extracti
-00000fa0: 6f6e 3b0a 2d20 6974 2077 7261 7073 2074  on;.- it wraps t
-00000fb0: 6865 204f 7065 6e43 5620 6675 6e63 7469  he OpenCV functi
-00000fc0: 6f6e 7320 696e 2061 2063 6f6e 7369 7374  ons in a consist
-00000fd0: 656e 7420 7761 792c 2068 6964 696e 6720  ent way, hiding 
-00000fe0: 736f 6d65 206f 6620 7468 6520 676e 6172  some of the gnar
-00000ff0: 6c79 2064 6574 6169 6c73 206f 6620 4f70  ly details of Op
-00001000: 656e 4356 206c 696b 6520 636f 6e76 6572  enCV like conver
-00001010: 7369 6f6e 2074 6f2f 6672 6f6d 2066 6c6f  sion to/from flo
-00001020: 6174 3332 2061 6e64 2074 6865 2042 4752  at32 and the BGR
-00001030: 2063 6f6c 6f72 206f 7264 6572 2e0a 2d20   color order..- 
-00001040: 6974 2069 7320 6861 7320 7369 6d69 6c61  it is has simila
-00001050: 7269 7479 2074 6f20 7468 6520 4d61 6368  rity to the Mach
-00001060: 696e 6520 5669 7369 6f6e 2054 6f6f 6c62  ine Vision Toolb
-00001070: 6f78 2066 6f72 204d 4154 4c41 422e 0a0a  ox for MATLAB...
-00001080: 2320 4765 7474 696e 6720 676f 696e 670a  # Getting going.
-00001090: 0a23 2320 5573 696e 6720 7069 700a 0a49  .## Using pip..I
-000010a0: 6e73 7461 6c6c 2061 2073 6e61 7073 686f  nstall a snapsho
-000010b0: 7420 6672 6f6d 2050 7950 490a 0a60 6060  t from PyPI..```
-000010c0: 0a25 2070 6970 2069 6e73 7461 6c6c 206d  .% pip install m
-000010d0: 6163 6869 6e65 7669 7369 6f6e 2d74 6f6f  achinevision-too
-000010e0: 6c62 6f78 2d70 7974 686f 6e0a 6060 600a  lbox-python.```.
-000010f0: 0a23 2320 4672 6f6d 2047 6974 4875 620a  .## From GitHub.
-00001100: 0a49 6e73 7461 6c6c 2074 6865 2063 7572  .Install the cur
-00001110: 7265 6e74 2063 6f64 6520 6261 7365 2066  rent code base f
-00001120: 726f 6d20 4769 7448 7562 2061 6e64 2070  rom GitHub and p
-00001130: 6970 2069 6e73 7461 6c6c 2061 206c 696e  ip install a lin
-00001140: 6b20 746f 2074 6861 7420 636c 6f6e 6564  k to that cloned
-00001150: 2063 6f70 790a 0a60 6060 0a25 2067 6974   copy..```.% git
-00001160: 2063 6c6f 6e65 2068 7474 7073 3a2f 2f67   clone https://g
-00001170: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
-00001180: 6f72 6b65 2f6d 6163 6869 6e65 7669 7369  orke/machinevisi
-00001190: 6f6e 2d74 6f6f 6c62 6f78 2d70 7974 686f  on-toolbox-pytho
-000011a0: 6e2e 6769 740a 2520 6364 206d 6163 6869  n.git.% cd machi
-000011b0: 6e65 7669 7369 6f6e 2d74 6f6f 6c62 6f78  nevision-toolbox
-000011c0: 2d70 7974 686f 6e0a 2520 7069 7020 696e  -python.% pip in
-000011d0: 7374 616c 6c20 2d65 202e 0a60 6060 0a0a  stall -e ..```..
-000011e0: 2320 4578 616d 706c 6573 0a0a 2323 2320  # Examples..### 
-000011f0: 5265 6164 696e 6720 616e 6420 6469 7370  Reading and disp
-00001200: 6c61 7920 616e 2069 6d61 6765 0a0a 6060  lay an image..``
-00001210: 6070 7974 686f 6e0a 6672 6f6d 206d 6163  `python.from mac
-00001220: 6869 6e65 7669 7369 6f6e 746f 6f6c 626f  hinevisiontoolbo
-00001230: 7820 696d 706f 7274 2049 6d61 6765 0a6d  x import Image.m
-00001240: 6f6e 6120 3d20 496d 6167 652e 5265 6164  ona = Image.Read
-00001250: 2822 6d6f 6e61 6c69 7361 2e70 6e67 2229  ("monalisa.png")
-00001260: 0a6d 6f6e 612e 6469 7370 2829 0a60 6060  .mona.disp().```
-00001270: 0a0a 215b 4d6f 6e61 204c 6973 6120 696d  ..![Mona Lisa im
-00001280: 6167 655d 2868 7474 7073 3a2f 2f67 6974  age](https://git
-00001290: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
-000012a0: 6b65 2f6d 6163 6869 6e65 7669 7369 6f6e  ke/machinevision
-000012b0: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e2f  -toolbox-python/
-000012c0: 7261 772f 6d61 7374 6572 2f66 6967 732f  raw/master/figs/
-000012d0: 6d6f 6e61 2e70 6e67 290a 0a49 6d61 6765  mona.png)..Image
-000012e0: 7320 6361 6e20 616c 736f 2062 6520 7265  s can also be re
-000012f0: 7475 726e 6564 2062 7920 6974 6572 6174  turned by iterat
-00001300: 6f72 7320 7468 6174 206f 7065 7261 7465  ors that operate
-00001310: 206f 7665 7220 666f 6c64 6572 732c 207a   over folders, z
-00001320: 6970 2066 696c 6573 2c20 6c6f 6361 6c20  ip files, local 
-00001330: 6361 6d65 7261 732c 2077 6562 2063 616d  cameras, web cam
-00001340: 6572 6173 2061 6e64 2076 6964 656f 2066  eras and video f
-00001350: 696c 6573 2e0a 0a23 2323 2053 696d 706c  iles...### Simpl
-00001360: 6520 696d 6167 6520 7072 6f63 6573 7369  e image processi
-00001370: 6e67 0a0a 5468 6520 746f 6f6c 626f 7820  ng..The toolbox 
-00001380: 7375 7070 6f72 7473 206d 616e 7920 6f70  supports many op
-00001390: 6572 6174 696f 6e73 206f 6e20 696d 6167  erations on imag
-000013a0: 6573 2073 7563 6820 6173 2032 4420 6669  es such as 2D fi
-000013b0: 6c74 6572 696e 672c 2065 6467 6520 6465  ltering, edge de
-000013c0: 7465 6374 696f 6e2c 206d 6174 6865 6d61  tection, mathema
-000013d0: 7469 6361 6c20 6d6f 7270 686f 6c6f 6779  tical morphology
-000013e0: 2c20 636f 6c6f 7273 7061 6365 2063 6f6e  , colorspace con
-000013f0: 7665 7273 696f 6e2c 2070 6164 6469 6e67  version, padding
-00001400: 2c20 6372 6f70 7069 6e67 2c20 7265 7369  , cropping, resi
-00001410: 7a69 6e67 2c20 726f 7461 7469 6f6e 2061  zing, rotation a
-00001420: 6e64 2077 6172 7069 6e67 2e0a 0a60 6060  nd warping...```
-00001430: 7079 7468 6f6e 0a6d 6f6e 612e 736d 6f6f  python.mona.smoo
-00001440: 7468 2873 6967 6d61 3d35 292e 6469 7370  th(sigma=5).disp
-00001450: 2829 0a60 6060 0a0a 215b 4d6f 6e61 204c  ().```..![Mona L
-00001460: 6973 6120 696d 6167 6520 7769 7468 2073  isa image with s
-00001470: 6d6f 6f74 6869 6e67 5d28 6874 7470 733a  moothing](https:
-00001480: 2f2f 6769 7468 7562 2e63 6f6d 2f70 6574  //github.com/pet
-00001490: 6572 636f 726b 652f 6d61 6368 696e 6576  ercorke/machinev
-000014a0: 6973 696f 6e2d 746f 6f6c 626f 782d 7079  ision-toolbox-py
-000014b0: 7468 6f6e 2f72 6177 2f6d 6173 7465 722f  thon/raw/master/
-000014c0: 6669 6773 2f6d 6f6e 615f 736d 6f6f 7468  figs/mona_smooth
-000014d0: 2e70 6e67 290a 0a54 6865 7265 2061 7265  .png)..There are
-000014e0: 2061 6c73 6f20 6d61 6e79 2066 756e 6374   also many funct
-000014f0: 696f 6e73 2074 6861 7420 6f70 6572 6174  ions that operat
-00001500: 6520 6f6e 2070 6169 7273 206f 6620 696d  e on pairs of im
-00001510: 6167 652e 2041 6c6c 2074 6865 2061 7269  age. All the ari
-00001520: 7468 6d65 7469 6320 6f70 6572 6174 6f72  thmetic operator
-00001530: 7320 6172 6520 6f76 6572 6c6f 6164 6564  s are overloaded
-00001540: 2c20 616e 6420 7468 6572 6520 6172 6520  , and there are 
-00001550: 6d65 7468 6f64 7320 746f 2063 6f6d 6269  methods to combi
-00001560: 6e65 2069 6d61 6765 7320 696e 206d 6f72  ne images in mor
-00001570: 6520 636f 6d70 6c65 7820 7761 7973 2e20  e complex ways. 
-00001580: 4d75 6c74 6970 6c65 2069 6d61 6765 7320  Multiple images 
-00001590: 6361 6e20 6265 2073 7461 636b 6564 2068  can be stacked h
-000015a0: 6f72 697a 6f6e 7461 6c2c 2076 6572 7469  orizontal, verti
-000015b0: 6361 6c6c 7920 6f72 2074 696c 6564 2069  cally or tiled i
-000015c0: 6e20 6120 3244 2067 7269 642e 2046 6f72  n a 2D grid. For
-000015d0: 2065 7861 6d70 6c65 2c20 7765 2063 6f75   example, we cou
-000015e0: 6c64 2064 6973 706c 6179 2074 6865 206f  ld display the o
-000015f0: 7269 6769 6e61 6c20 616e 6420 736d 6f6f  riginal and smoo
-00001600: 7468 6564 2069 6d61 6765 7320 7369 6465  thed images side
-00001610: 2062 7920 7369 6465 0a0a 6060 6070 7974   by side..```pyt
-00001620: 686f 6e0a 496d 6167 652e 4873 7461 636b  hon.Image.Hstack
-00001630: 285b 6d6f 6e61 2c20 6d6f 6e61 2e73 6d6f  ([mona, mona.smo
-00001640: 6f74 6828 7369 676d 613d 3529 5d29 2e64  oth(sigma=5)]).d
-00001650: 6973 7028 290a 6060 600a 0a77 6865 7265  isp().```..where
-00001660: 2060 4873 7461 636b 6020 6973 2061 2063   `Hstack` is a c
-00001670: 6c61 7373 206d 6574 686f 6420 7468 6174  lass method that
-00001680: 2063 7265 6174 6573 2061 206e 6577 2069   creates a new i
-00001690: 6d61 6765 2062 7920 7374 6163 6b69 6e67  mage by stacking
-000016a0: 2074 6865 0a69 6d61 6765 7320 6672 6f6d   the.images from
-000016b0: 2069 7473 2061 7267 756d 656e 742c 2061   its argument, a
-000016c0: 6e20 696d 6167 6520 7365 7175 656e 6365  n image sequence
-000016d0: 2c20 686f 7269 7a6f 6e74 616c 6c79 2e0a  , horizontally..
-000016e0: 0a21 5b4d 6f6e 6120 4c69 7361 2069 6d61  .![Mona Lisa ima
-000016f0: 6765 2077 6974 6820 736d 6f6f 7468 696e  ge with smoothin
-00001700: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
-00001710: 622e 636f 6d2f 7065 7465 7263 6f72 6b65  b.com/petercorke
-00001720: 2f6d 6163 6869 6e65 7669 7369 6f6e 2d74  /machinevision-t
-00001730: 6f6f 6c62 6f78 2d70 7974 686f 6e2f 7261  oolbox-python/ra
-00001740: 772f 6d61 7374 6572 2f66 6967 732f 6d6f  w/master/figs/mo
-00001750: 6e61 2b73 6d6f 6f74 682e 706e 6729 0a0a  na+smooth.png)..
-00001760: 2323 2320 4269 6e61 7279 2062 6c6f 6273  ### Binary blobs
-00001770: 0a0a 4120 636f 6d6d 6f6e 2070 726f 626c  ..A common probl
-00001780: 656d 2069 6e20 726f 626f 7469 6320 7669  em in robotic vi
-00001790: 7369 6f6e 2069 7320 746f 2065 7874 7261  sion is to extra
-000017a0: 6374 2066 6561 7475 7265 7320 6672 6f6d  ct features from
-000017b0: 2074 6865 2069 6d61 6765 2c20 746f 2064   the image, to d
-000017c0: 6573 6372 6962 6520 7468 6520 706f 7369  escribe the posi
-000017d0: 7469 6f6e 2c20 7369 7a65 2c20 7368 6170  tion, size, shap
-000017e0: 6520 616e 6420 6f72 6965 6e74 6174 696f  e and orientatio
-000017f0: 6e20 6f66 206f 626a 6563 7473 2069 6e20  n of objects in 
-00001800: 7468 6520 7363 656e 652e 2046 6f72 2073  the scene. For s
-00001810: 696d 706c 6520 6269 6e61 7279 2073 6365  imple binary sce
-00001820: 6e65 7320 626c 6f62 2066 6561 7475 7265  nes blob feature
-00001830: 7320 6172 6520 636f 6d6d 6f6e 6c79 2075  s are commonly u
-00001840: 7365 642e 0a0a 6060 6070 7974 686f 6e0a  sed...```python.
-00001850: 696d 203d 2049 6d61 6765 2e52 6561 6428  im = Image.Read(
-00001860: 2273 6861 726b 322e 706e 6722 2920 2020  "shark2.png")   
-00001870: 2320 7265 6164 2061 2062 696e 6172 7920  # read a binary 
-00001880: 696d 6167 6520 6f66 2074 776f 2073 6861  image of two sha
-00001890: 726b 730a 696d 2e64 6973 7028 293b 2020  rks.im.disp();  
-000018a0: 2023 2064 6973 706c 6179 2069 7420 7769   # display it wi
-000018b0: 7468 2069 6e74 6572 6163 7469 7665 2076  th interactive v
-000018c0: 6965 7769 6e67 2074 6f6f 6c0a 626c 6f62  iewing tool.blob
-000018d0: 7320 3d20 696d 2e62 6c6f 6273 2829 2020  s = im.blobs()  
-000018e0: 2320 6669 6e64 2061 6c6c 2074 6865 2077  # find all the w
-000018f0: 6869 7465 2062 6c6f 6273 0a70 7269 6e74  hite blobs.print
-00001900: 2862 6c6f 6273 290a 0a09 e294 8ce2 9480  (blobs).........
-00001910: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
-00001920: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001930: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
-00001940: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001950: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001960: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001970: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001980: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
-00001990: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
-000019a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000019b0: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
-000019c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000019d0: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
-000019e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000019f0: 80e2 9480 e294 ace2 9480 e294 80e2 9480  ................
-00001a00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001a10: 9490 0a09 e294 8269 6420 e294 8220 7061  .......id ... pa
-00001a20: 7265 6e74 20e2 9482 2020 2020 2063 656e  rent ...     cen
-00001a30: 7472 6f69 6420 e294 8220 2020 2020 6172  troid ...     ar
-00001a40: 6561 20e2 9482 2074 6f75 6368 20e2 9482  ea ... touch ...
-00001a50: 2070 6572 696d 20e2 9482 2063 6972 6375   perim ... circu
-00001a60: 6c61 7269 7479 20e2 9482 206f 7269 656e  larity ... orien
-00001a70: 7420 e294 8220 6173 7065 6374 20e2 9482  t ... aspect ...
-00001a80: 0a09 e294 9ce2 9480 e294 80e2 9480 e294  ................
-00001a90: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001aa0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00001ab0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ac0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001ad0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-00001ae0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001af0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-00001b00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001b10: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b20: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-00001b30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001b40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b50: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-00001b60: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-00001b70: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001b80: 80e2 9480 e294 80e2 94a4 0a09 e294 8220  ............... 
-00001b90: 3020 e294 8220 2020 2020 2d31 20e2 9482  0 ...     -1 ...
-00001ba0: 2033 3731 2e32 2c20 3335 352e 3220 e294   371.2, 355.2 ..
-00001bb0: 8220 372e 3539 652b 3033 20e2 9482 2046  . 7.59e+03 ... F
-00001bc0: 616c 7365 20e2 9482 2035 3537 2e36 20e2  alse ... 557.6 .
-00001bd0: 9482 2020 2020 2020 2030 2e33 3431 20e2  ..       0.341 .
-00001be0: 9482 2020 3832 2e39 c2b0 20e2 9482 2020  ..  82.9.. ...  
-00001bf0: 302e 3937 3620 e294 820a 09e2 9482 2031  0.976 ........ 1
-00001c00: 20e2 9482 2020 2020 202d 3120 e294 8220   ...     -1 ... 
-00001c10: 3137 312e 322c 2031 3535 2e32 20e2 9482  171.2, 155.2 ...
-00001c20: 2037 2e35 3965 2b30 3320 e294 8220 4661   7.59e+03 ... Fa
-00001c30: 6c73 6520 e294 8220 3535 372e 3620 e294  lse ... 557.6 ..
-00001c40: 8220 2020 2020 2020 302e 3334 3120 e294  .       0.341 ..
-00001c50: 8220 2038 322e 39c2 b020 e294 8220 2030  .  82.9.. ...  0
-00001c60: 2e39 3736 20e2 9482 0a09 e294 94e2 9480  .976 ...........
-00001c70: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
-00001c80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001c90: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
-00001ca0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001cb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001cc0: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001cd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001ce0: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001cf0: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
-00001d00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001d10: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001d20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001d30: e294 80e2 9480 e294 80e2 94b4 e294 80e2  ................
-00001d40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001d50: 80e2 9480 e294 b4e2 9480 e294 80e2 9480  ................
-00001d60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001d70: 9498 0a60 6060 0a0a 7768 6572 6520 6062  ...```..where `b
-00001d80: 6c6f 6273 6020 6973 2061 206c 6973 742d  lobs` is a list-
-00001d90: 6c69 6b65 206f 626a 6563 7420 616e 6420  like object and 
-00001da0: 6561 6368 2065 6c65 6d65 6e74 2064 6573  each element des
-00001db0: 6372 6962 6573 2061 2062 6c6f 6220 696e  cribes a blob in
-00001dc0: 2074 6865 2073 6365 6e65 2e20 5468 6520   the scene. The 
-00001dd0: 656c 656d 656e 7427 7320 6174 7472 6962  element's attrib
-00001de0: 7574 6573 2064 6573 6372 6962 6520 7661  utes describe va
-00001df0: 7269 6f75 7320 7061 7261 6d65 7465 7273  rious parameters
-00001e00: 206f 6620 7468 6520 6f62 6a65 6374 2c20   of the object, 
-00001e10: 616e 6420 6d65 7468 6f64 7320 6361 6e20  and methods can 
-00001e20: 6265 2075 7365 6420 746f 206f 7665 726c  be used to overl
-00001e30: 6179 2067 7261 7068 6963 7320 7375 6368  ay graphics such
-00001e40: 2061 7320 626f 756e 6469 6e67 2062 6f78   as bounding box
-00001e50: 6573 2061 6e64 2063 656e 7472 6f69 6473  es and centroids
-00001e60: 0a0a 6060 6070 7974 686f 6e0a 626c 6f62  ..```python.blob
-00001e70: 732e 706c 6f74 5f62 6f78 2863 6f6c 6f72  s.plot_box(color
-00001e80: 3d22 6722 2c20 6c69 6e65 7769 6474 683d  ="g", linewidth=
-00001e90: 3229 2020 2320 7075 7420 6120 6772 6565  2)  # put a gree
-00001ea0: 6e20 626f 756e 6469 6e67 2062 6f78 206f  n bounding box o
-00001eb0: 6e20 6561 6368 2062 6c6f 620a 626c 6f62  n each blob.blob
-00001ec0: 732e 706c 6f74 5f63 656e 7472 6f69 6428  s.plot_centroid(
-00001ed0: 6c61 6265 6c3d 5472 7565 2920 2023 2070  label=True)  # p
-00001ee0: 7574 2061 2063 6972 636c 652b 6372 6f73  ut a circle+cros
-00001ef0: 7320 6f6e 2074 6865 2063 656e 7472 6f69  s on the centroi
-00001f00: 6420 6f66 2065 6163 6820 626c 6f62 0a70  d of each blob.p
-00001f10: 6c74 2e73 686f 7728 626c 6f63 6b3d 5472  lt.show(block=Tr
-00001f20: 7565 2920 2023 2064 6973 706c 6179 2074  ue)  # display t
-00001f30: 6865 2072 6573 756c 740a 6060 600a 0a21  he result.```..!
-00001f40: 5b42 696e 6172 7920 696d 6167 6520 7368  [Binary image sh
-00001f50: 6f77 696e 6720 626f 756e 6469 6e67 2062  owing bounding b
-00001f60: 6f78 6573 2061 6e64 2063 656e 7472 6f69  oxes and centroi
-00001f70: 6473 5d28 6874 7470 733a 2f2f 6769 7468  ds](https://gith
-00001f80: 7562 2e63 6f6d 2f70 6574 6572 636f 726b  ub.com/petercork
-00001f90: 652f 6d61 6368 696e 6576 6973 696f 6e2d  e/machinevision-
-00001fa0: 746f 6f6c 626f 782d 7079 7468 6f6e 2f72  toolbox-python/r
-00001fb0: 6177 2f6d 6173 7465 722f 6669 6773 2f73  aw/master/figs/s
-00001fc0: 6861 726b 322b 626f 7865 732e 706e 6729  hark2+boxes.png)
-00001fd0: 0a0a 2323 2323 2042 696e 6172 7920 626c  ..#### Binary bl
-00001fe0: 6f62 2068 6965 7261 7263 6879 0a0a 4120  ob hierarchy..A 
-00001ff0: 6d6f 7265 2063 6f6d 706c 6578 2069 6d61  more complex ima
-00002000: 6765 2069 730a 0a60 6060 7079 7468 6f6e  ge is..```python
-00002010: 0a69 6d20 3d20 496d 6167 652e 5265 6164  .im = Image.Read
-00002020: 2822 6d75 6c74 6962 6c6f 6273 2e70 6e67  ("multiblobs.png
-00002030: 2229 0a69 6d2e 6469 7370 2829 0a60 6060  ").im.disp().```
-00002040: 0a0a 215b 4269 6e61 7279 2069 6d61 6765  ..![Binary image
-00002050: 2077 6974 6820 6e65 7374 6564 2062 6c6f   with nested blo
-00002060: 6273 5d28 6874 7470 733a 2f2f 6769 7468  bs](https://gith
-00002070: 7562 2e63 6f6d 2f70 6574 6572 636f 726b  ub.com/petercork
-00002080: 652f 6d61 6368 696e 6576 6973 696f 6e2d  e/machinevision-
-00002090: 746f 6f6c 626f 782d 7079 7468 6f6e 2f72  toolbox-python/r
-000020a0: 6177 2f6d 6173 7465 722f 6669 6773 2f6d  aw/master/figs/m
-000020b0: 756c 7469 2e70 6e67 290a 0a61 6e64 2077  ulti.png)..and w
-000020c0: 6520 7365 6520 7468 6174 2073 6f6d 6520  e see that some 
-000020d0: 626c 6f62 7320 6172 6520 636f 6e74 6169  blobs are contai
-000020e0: 6e65 6420 7769 7468 696e 206f 7468 6572  ned within other
-000020f0: 2062 6c6f 6273 2e20 5468 6520 7265 7375   blobs. The resu
-00002100: 6c74 7320 696e 2074 6162 756c 6172 2066  lts in tabular f
-00002110: 6f72 6d0a 0a60 6060 7079 7468 6f6e 0a62  orm..```python.b
-00002120: 6c6f 6273 2020 3d20 696d 2e62 6c6f 6273  lobs  = im.blobs
-00002130: 2829 0a70 7269 6e74 2862 6c6f 6273 290a  ().print(blobs).
-00002140: 09e2 948c e294 80e2 9480 e294 80e2 94ac  ................
-00002150: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002160: 9480 e294 80e2 9480 e294 ace2 9480 e294  ................
-00002170: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002180: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002190: 9480 e294 80e2 9480 e294 ace2 9480 e294  ................
-000021a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000021b0: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
-000021c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000021d0: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
-000021e0: e294 80e2 9480 e294 80e2 9480 e294 ace2  ................
-000021f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002200: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002210: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
-00002220: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002230: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
-00002240: e294 80e2 9480 e294 80e2 9480 e294 900a  ................
-00002250: 09e2 9482 6964 20e2 9482 2070 6172 656e  ....id ... paren
-00002260: 7420 e294 8220 2020 2020 2063 656e 7472  t ...      centr
-00002270: 6f69 6420 e294 8220 2020 2020 6172 6561  oid ...     area
-00002280: 20e2 9482 2074 6f75 6368 20e2 9482 2020   ... touch ...  
-00002290: 7065 7269 6d20 e294 8220 6369 7263 756c  perim ... circul
-000022a0: 6172 6974 7920 e294 8220 6f72 6965 6e74  arity ... orient
-000022b0: 20e2 9482 2061 7370 6563 7420 e294 820a   ... aspect ....
-000022c0: 09e2 949c e294 80e2 9480 e294 80e2 94bc  ................
-000022d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000022e0: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-000022f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002300: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002310: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-00002320: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002330: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00002340: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002350: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-00002360: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-00002370: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002380: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002390: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-000023a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000023b0: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-000023c0: e294 80e2 9480 e294 80e2 9480 e294 a40a  ................
-000023d0: 09e2 9482 2030 20e2 9482 2020 2020 2020  .... 0 ...      
-000023e0: 3120 e294 8220 2038 3938 2e38 2c20 3732  1 ...  898.8, 72
-000023f0: 352e 3320 e294 8220 312e 3635 652b 3035  5.3 ... 1.65e+05
-00002400: 20e2 9482 2046 616c 7365 20e2 9482 2032   ... False ... 2
-00002410: 3232 302e 3020 e294 8220 2020 2020 2020  220.0 ...       
-00002420: 302e 3436 3720 e294 8220 2038 362e 37c2  0.467 ...  86.7.
-00002430: b020 e294 8220 2030 2e37 3534 20e2 9482  . ...  0.754 ...
-00002440: 0a09 e294 8220 3120 e294 8220 2020 2020  ..... 1 ...     
-00002450: 2032 20e2 9482 2031 3032 352e 302c 2038   2 ... 1025.0, 8
-00002460: 3133 2e37 20e2 9482 2031 2e30 3665 2b30  13.7 ... 1.06e+0
-00002470: 3520 e294 8220 4661 6c73 6520 e294 8220  5 ... False ... 
-00002480: 3133 3837 2e39 20e2 9482 2020 2020 2020  1387.9 ...      
-00002490: 2030 2e37 3639 20e2 9482 202d 3838 2e39   0.769 ... -88.9
-000024a0: c2b0 20e2 9482 2020 302e 3733 3920 e294  .. ...  0.739 ..
-000024b0: 820a 09e2 9482 2032 20e2 9482 2020 2020  ...... 2 ...    
-000024c0: 202d 3120 e294 8220 2039 3338 2e31 2c20   -1 ...  938.1, 
-000024d0: 3835 352e 3220 e294 8220 312e 3732 652b  855.2 ... 1.72e+
-000024e0: 3034 20e2 9482 2046 616c 7365 20e2 9482  04 ... False ...
-000024f0: 2020 3439 302e 3720 e294 8220 2020 2020    490.7 ...     
-00002500: 2020 312e 3030 3120 e294 8220 2038 382e    1.001 ...  88.
-00002510: 37c2 b020 e294 8220 2030 2e38 3632 20e2  7.. ...  0.862 .
-00002520: 9482 0a09 e294 8220 3320 e294 8220 2020  ....... 3 ...   
-00002530: 2020 2d31 20e2 9482 2020 3938 382e 312c    -1 ...  988.1,
-00002540: 2036 3937 2e32 20e2 9482 2031 2e32 3165   697.2 ... 1.21e
-00002550: 2b30 3420 e294 8220 4661 6c73 6520 e294  +04 ... False ..
-00002560: 8220 2034 3132 2e35 20e2 9482 2020 2020  .  412.5 ...    
-00002570: 2020 2030 2e39 3934 20e2 9482 202d 3837     0.994 ... -87
-00002580: 2e38 c2b0 20e2 9482 2020 302e 3830 3920  .8.. ...  0.809 
-00002590: e294 820a 09e2 9482 2034 20e2 9482 2020  ........ 4 ...  
-000025a0: 2020 202d 3120 e294 8220 2038 3436 2e30     -1 ...  846.0
-000025b0: 2c20 3531 312e 3720 e294 8220 312e 3735  , 511.7 ... 1.75
-000025c0: 652b 3034 20e2 9482 2046 616c 7365 20e2  e+04 ... False .
-000025d0: 9482 2020 3439 362e 3920 e294 8220 2020  ..  496.9 ...   
-000025e0: 2020 2020 302e 3939 3220 e294 8220 2d39      0.992 ... -9
-000025f0: 302e 30c2 b020 e294 8220 2030 2e37 3738  0.0.. ...  0.778
-00002600: 20e2 9482 0a09 e294 8220 3520 e294 8220   ........ 5 ... 
-00002610: 2020 2020 2036 20e2 9482 2020 3239 312e       6 ...  291.
-00002620: 372c 2033 3737 2e38 20e2 9482 2020 312e  7, 377.8 ...  1.
-00002630: 3765 2b30 3520 e294 8220 4661 6c73 6520  7e+05 ... False 
-00002640: e294 8220 3137 3132 2e36 20e2 9482 2020  ... 1712.6 ...  
-00002650: 2020 2020 2030 2e38 3130 20e2 9482 202d       0.810 ... -
-00002660: 3835 2e33 c2b0 20e2 9482 2020 302e 3736  85.3.. ...  0.76
-00002670: 3720 e294 820a 09e2 9482 2036 20e2 9482  7 ........ 6 ...
-00002680: 2020 2020 202d 3120 e294 8220 2033 3132       -1 ...  312
-00002690: 2e37 2c20 3437 322e 3120 e294 8220 312e  .7, 472.1 ... 1.
-000026a0: 3735 652b 3034 20e2 9482 2046 616c 7365  75e+04 ... False
-000026b0: 20e2 9482 2020 3439 352e 3520 e294 8220   ...  495.5 ... 
-000026c0: 2020 2020 2020 302e 3939 3720 e294 8220        0.997 ... 
-000026d0: 2d38 392e 39c2 b020 e294 8220 2030 2e37  -89.9.. ...  0.7
-000026e0: 3737 20e2 9482 0a09 e294 8220 3720 e294  77 ........ 7 ..
-000026f0: 8220 2020 2020 2d31 20e2 9482 2020 3234  .     -1 ...  24
-00002700: 312e 392c 2032 3435 2e30 20e2 9482 2031  1.9, 245.0 ... 1
-00002710: 2e37 3565 2b30 3420 e294 8220 4661 6c73  .75e+04 ... Fals
-00002720: 6520 e294 8220 2034 3936 2e39 20e2 9482  e ...  496.9 ...
-00002730: 2020 2020 2020 2030 2e39 3932 20e2 9482         0.992 ...
-00002740: 202d 3930 2e30 c2b0 20e2 9482 2020 302e   -90.0.. ...  0.
-00002750: 3737 3720 e294 820a 09e2 9482 2038 20e2  777 ........ 8 .
-00002760: 9482 2020 2020 2020 3920 e294 8220 3132  ..      9 ... 12
-00002770: 3238 2e30 2c20 3235 342e 3320 e294 8220  28.0, 254.3 ... 
-00002780: 382e 3134 652b 3034 20e2 9482 2046 616c  8.14e+04 ... Fal
-00002790: 7365 20e2 9482 2031 3231 352e 3220 e294  se ... 1215.2 ..
-000027a0: 8220 2020 2020 2020 302e 3737 3120 e294  .       0.771 ..
-000027b0: 8220 2d37 372e 32c2 b020 e294 8220 2030  . -77.2.. ...  0
-000027c0: 2e37 3133 20e2 9482 0a09 e294 8220 3920  .713 ........ 9 
-000027d0: e294 8220 2020 2020 2d31 20e2 9482 2031  ...     -1 ... 1
-000027e0: 3232 352e 322c 2032 3230 2e30 20e2 9482  225.2, 220.0 ...
-000027f0: 2031 2e37 3565 2b30 3420 e294 8220 4661   1.75e+04 ... Fa
-00002800: 6c73 6520 e294 8220 2034 3936 2e39 20e2  lse ...  496.9 .
-00002810: 9482 2020 2020 2020 2030 2e39 3932 20e2  ..       0.992 .
-00002820: 9482 202d 3930 2e30 c2b0 20e2 9482 2020  .. -90.0.. ...  
-00002830: 302e 3737 3720 e294 820a 09e2 9494 e294  0.777 ..........
-00002840: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
-00002850: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002860: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
-00002870: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002880: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002890: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
-000028a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000028b0: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
-000028c0: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
-000028d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000028e0: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
-000028f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002900: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002910: e294 b4e2 9480 e294 80e2 9480 e294 80e2  ................
-00002920: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6d61 6368  : 2.1.Name: mach
+00000020: 696e 6576 6973 696f 6e2d 746f 6f6c 626f  inevision-toolbo
+00000030: 782d 7079 7468 6f6e 0a56 6572 7369 6f6e  x-python.Version
+00000040: 3a20 302e 392e 370a 5375 6d6d 6172 793a  : 0.9.7.Summary:
+00000050: 2050 7974 686f 6e20 746f 6f6c 7320 666f   Python tools fo
+00000060: 7220 6d61 6368 696e 6520 7669 7369 6f6e  r machine vision
+00000070: 202d 2065 6475 6361 7469 6f6e 2061 6e64   - education and
+00000080: 2072 6573 6561 7263 680a 4175 7468 6f72   research.Author
+00000090: 3a20 446f 7269 616e 2054 7361 690a 4175  : Dorian Tsai.Au
+000000a0: 7468 6f72 2d65 6d61 696c 3a20 5065 7465  thor-email: Pete
+000000b0: 7220 436f 726b 6520 3c72 7663 4070 6574  r Corke <rvc@pet
+000000c0: 6572 636f 726b 652e 636f 6d3e 0a50 726f  ercorke.com>.Pro
+000000d0: 6a65 6374 2d55 524c 3a20 486f 6d65 7061  ject-URL: Homepa
+000000e0: 6765 2c20 6874 7470 733a 2f2f 6769 7468  ge, https://gith
+000000f0: 7562 2e63 6f6d 2f70 6574 6572 636f 726b  ub.com/petercork
+00000100: 652f 6d61 6368 696e 6576 6973 696f 6e2d  e/machinevision-
+00000110: 746f 6f6c 626f 782d 7079 7468 6f6e 0a50  toolbox-python.P
+00000120: 726f 6a65 6374 2d55 524c 3a20 4275 6720  roject-URL: Bug 
+00000130: 5472 6163 6b65 722c 2068 7474 7073 3a2f  Tracker, https:/
+00000140: 2f67 6974 6875 622e 636f 6d2f 7079 7061  /github.com/pypa
+00000150: 2f73 616d 706c 6570 726f 6a65 6374 2f69  /sampleproject/i
+00000160: 7373 7565 730a 5072 6f6a 6563 742d 5552  ssues.Project-UR
+00000170: 4c3a 2044 6f63 756d 656e 7461 7469 6f6e  L: Documentation
+00000180: 2c20 6874 7470 733a 2f2f 7065 7465 7263  , https://peterc
+00000190: 6f72 6b65 2e67 6974 6875 622e 696f 2f6d  orke.github.io/m
+000001a0: 6163 6869 6e65 7669 7369 6f6e 2d74 6f6f  achinevision-too
+000001b0: 6c62 6f78 2d70 7974 686f 6e0a 5072 6f6a  lbox-python.Proj
+000001c0: 6563 742d 5552 4c3a 2053 6f75 7263 652c  ect-URL: Source,
+000001d0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000001e0: 636f 6d2f 7065 7465 7263 6f72 6b65 2f6d  com/petercorke/m
+000001f0: 6163 6869 6e65 7669 7369 6f6e 2d74 6f6f  achinevision-too
+00000200: 6c62 6f78 2d70 7974 686f 6e0a 4b65 7977  lbox-python.Keyw
+00000210: 6f72 6473 3a20 6d61 6368 696e 6520 7669  ords: machine vi
+00000220: 7369 6f6e 2c63 6f6d 7075 7465 7220 7669  sion,computer vi
+00000230: 7369 6f6e 2c6d 756c 7469 7669 6577 2067  sion,multiview g
+00000240: 656f 6d65 7472 792c 7374 6572 656f 2076  eometry,stereo v
+00000250: 6973 696f 6e2c 6275 6e64 6c65 2061 646a  ision,bundle adj
+00000260: 7573 746d 656e 742c 7669 7375 616c 2073  ustment,visual s
+00000270: 6572 766f 696e 672c 696d 6167 6520 6665  ervoing,image fe
+00000280: 6174 7572 6573 2c63 6f6c 6f72 2c62 6c6f  atures,color,blo
+00000290: 6273 2c6d 6f72 7068 6f6c 6f67 792c 696d  bs,morphology,im
+000002a0: 6167 6520 7365 676d 656e 7461 7469 6f6e  age segmentation
+000002b0: 2c6f 7065 6e63 762c 6f70 656e 3364 0a43  ,opencv,open3d.C
+000002c0: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
+000002d0: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+000002e0: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
+000002f0: 5374 6162 6c65 0a43 6c61 7373 6966 6965  Stable.Classifie
+00000300: 723a 2049 6e74 656e 6465 6420 4175 6469  r: Intended Audi
+00000310: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
+00000320: 7273 0a43 6c61 7373 6966 6965 723a 2050  rs.Classifier: P
+00000330: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000340: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000350: 2033 2e37 0a43 6c61 7373 6966 6965 723a   3.7.Classifier:
+00000360: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000370: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000380: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
+00000390: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000003a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000003b0: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
+000003c0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000003d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000003e0: 686f 6e20 3a3a 2033 2e31 300a 436c 6173  hon :: 3.10.Clas
+000003f0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000400: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000410: 5079 7468 6f6e 203a 3a20 332e 3131 0a43  Python :: 3.11.C
+00000420: 6c61 7373 6966 6965 723a 204c 6963 656e  lassifier: Licen
+00000430: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000440: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000450: 650a 436c 6173 7369 6669 6572 3a20 4f70  e.Classifier: Op
+00000460: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000470: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00000480: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
+00000490: 3a20 3e3d 332e 370a 4465 7363 7269 7074  : >=3.7.Descript
+000004a0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
+000004b0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
+000004c0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+000004d0: 4345 4e53 450a 5265 7175 6972 6573 2d44  CENSE.Requires-D
+000004e0: 6973 743a 206e 756d 7079 3e3d 312e 3137  ist: numpy>=1.17
+000004f0: 2e34 0a52 6571 7569 7265 732d 4469 7374  .4.Requires-Dist
+00000500: 3a20 7363 6970 790a 5265 7175 6972 6573  : scipy.Requires
+00000510: 2d44 6973 743a 206d 6174 706c 6f74 6c69  -Dist: matplotli
+00000520: 620a 5265 7175 6972 6573 2d44 6973 743a  b.Requires-Dist:
+00000530: 206f 7065 6e63 762d 7079 7468 6f6e 0a52   opencv-python.R
+00000540: 6571 7569 7265 732d 4469 7374 3a20 6f70  equires-Dist: op
+00000550: 656e 3364 0a52 6571 7569 7265 732d 4469  en3d.Requires-Di
+00000560: 7374 3a20 6f70 656e 6376 2d63 6f6e 7472  st: opencv-contr
+00000570: 6962 2d70 7974 686f 6e0a 5265 7175 6972  ib-python.Requir
+00000580: 6573 2d44 6973 743a 2073 7061 7469 616c  es-Dist: spatial
+00000590: 6d61 7468 2d70 7974 686f 6e0a 5265 7175  math-python.Requ
+000005a0: 6972 6573 2d44 6973 743a 2070 6772 6170  ires-Dist: pgrap
+000005b0: 682d 7079 7468 6f6e 0a52 6571 7569 7265  h-python.Require
+000005c0: 732d 4469 7374 3a20 616e 7369 7461 626c  s-Dist: ansitabl
+000005d0: 650a 5265 7175 6972 6573 2d44 6973 743a  e.Requires-Dist:
+000005e0: 206d 7674 622d 6461 7461 0a50 726f 7669   mvtb-data.Provi
+000005f0: 6465 732d 4578 7472 613a 2064 6576 0a52  des-Extra: dev.R
+00000600: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000610: 7465 7374 3b20 6578 7472 6120 3d3d 2022  test; extra == "
+00000620: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000630: 7374 3a20 636f 7665 7261 6765 3b20 6578  st: coverage; ex
+00000640: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000650: 7569 7265 732d 4469 7374 3a20 666c 616b  uires-Dist: flak
+00000660: 6538 3b20 6578 7472 6120 3d3d 2022 6465  e8; extra == "de
+00000670: 7622 0a50 726f 7669 6465 732d 4578 7472  v".Provides-Extr
+00000680: 613a 2064 6f63 730a 5265 7175 6972 6573  a: docs.Requires
+00000690: 2d44 6973 743a 2073 7068 696e 783b 2065  -Dist: sphinx; e
+000006a0: 7874 7261 203d 3d20 2264 6f63 7322 0a52  xtra == "docs".R
+000006b0: 6571 7569 7265 732d 4469 7374 3a20 7265  equires-Dist: re
+000006c0: 636f 6d6d 6f6e 6d61 726b 3b20 6578 7472  commonmark; extr
+000006d0: 6120 3d3d 2022 646f 6373 220a 5265 7175  a == "docs".Requ
+000006e0: 6972 6573 2d44 6973 743a 2073 7068 696e  ires-Dist: sphin
+000006f0: 782d 7274 642d 7468 656d 653b 2065 7874  x-rtd-theme; ext
+00000700: 7261 203d 3d20 2264 6f63 7322 0a52 6571  ra == "docs".Req
+00000710: 7569 7265 732d 4469 7374 3a20 7370 6869  uires-Dist: sphi
+00000720: 6e78 2d61 7574 6f72 756e 3b20 6578 7472  nx-autorun; extr
+00000730: 6120 3d3d 2022 646f 6373 220a 5265 7175  a == "docs".Requ
+00000740: 6972 6573 2d44 6973 743a 2073 7068 696e  ires-Dist: sphin
+00000750: 7863 6f6e 7472 6962 2d6a 736d 6174 683b  xcontrib-jsmath;
+00000760: 2065 7874 7261 203d 3d20 2264 6f63 7322   extra == "docs"
+00000770: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000780: 7370 6869 6e78 2d6d 6172 6b64 6f77 6e2d  sphinx-markdown-
+00000790: 7461 626c 6573 3b20 6578 7472 6120 3d3d  tables; extra ==
+000007a0: 2022 646f 6373 220a 5265 7175 6972 6573   "docs".Requires
+000007b0: 2d44 6973 743a 2073 7068 696e 782d 6661  -Dist: sphinx-fa
+000007c0: 7669 636f 6e3b 2065 7874 7261 203d 3d20  vicon; extra == 
+000007d0: 2264 6f63 7322 0a0a 2320 4d61 6368 696e  "docs"..# Machin
+000007e0: 6520 5669 7369 6f6e 2054 6f6f 6c62 6f78  e Vision Toolbox
+000007f0: 2066 6f72 2050 7974 686f 6e0a 0a5b 215b   for Python..[![
+00000800: 4120 5079 7468 6f6e 2052 6f62 6f74 6963  A Python Robotic
+00000810: 7320 5061 636b 6167 655d 2868 7474 7073  s Package](https
+00000820: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000830: 7263 6f6e 7465 6e74 2e63 6f6d 2f70 6574  rcontent.com/pet
+00000840: 6572 636f 726b 652f 726f 626f 7469 6373  ercorke/robotics
+00000850: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e2f  -toolbox-python/
+00000860: 6d61 7374 6572 2f2e 6769 7468 7562 2f73  master/.github/s
+00000870: 7667 2f70 795f 636f 6c6c 6563 7469 6f6e  vg/py_collection
+00000880: 2e6d 696e 2e73 7667 295d 2868 7474 7073  .min.svg)](https
+00000890: 3a2f 2f67 6974 6875 622e 636f 6d2f 7065  ://github.com/pe
+000008a0: 7465 7263 6f72 6b65 2f72 6f62 6f74 6963  tercorke/robotic
+000008b0: 732d 746f 6f6c 626f 782d 7079 7468 6f6e  s-toolbox-python
+000008c0: 290a 5b21 5b50 6f77 6572 6564 2062 7920  ).[![Powered by 
+000008d0: 5370 6174 6961 6c20 4d61 7468 735d 2868  Spatial Maths](h
+000008e0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+000008f0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000900: 2f70 6574 6572 636f 726b 652f 7370 6174  /petercorke/spat
+00000910: 6961 6c6d 6174 682d 7079 7468 6f6e 2f6d  ialmath-python/m
+00000920: 6173 7465 722f 2e67 6974 6875 622f 7376  aster/.github/sv
+00000930: 672f 736d 5f70 6f77 6572 6564 2e6d 696e  g/sm_powered.min
+00000940: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
+00000950: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
+00000960: 6f72 6b65 2f73 7061 7469 616c 6d61 7468  orke/spatialmath
+00000970: 2d70 7974 686f 6e29 0a5b 215b 5155 5420  -python).[![QUT 
+00000980: 4365 6e74 7265 2066 6f72 2052 6f62 6f74  Centre for Robot
+00000990: 6963 7320 4f70 656e 2053 6f75 7263 655d  ics Open Source]
+000009a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000009b0: 636f 6d2f 7163 722f 7163 722e 6769 7468  com/qcr/qcr.gith
+000009c0: 7562 2e69 6f2f 7261 772f 6d61 7374 6572  ub.io/raw/master
+000009d0: 2f6d 6973 632f 6261 6467 652e 7376 6729  /misc/badge.svg)
+000009e0: 5d28 6874 7470 733a 2f2f 7163 722e 6769  ](https://qcr.gi
+000009f0: 7468 7562 2e69 6f29 0a0a 5b21 5b50 7950  thub.io)..[![PyP
+00000a00: 4920 7665 7273 696f 6e5d 2868 7474 7073  I version](https
+00000a10: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
+00000a20: 2f70 792f 6d61 6368 696e 6576 6973 696f  /py/machinevisio
+00000a30: 6e2d 746f 6f6c 626f 782d 7079 7468 6f6e  n-toolbox-python
+00000a40: 2e73 7667 295d 2868 7474 7073 3a2f 2f62  .svg)](https://b
+00000a50: 6164 6765 2e66 7572 792e 696f 2f70 792f  adge.fury.io/py/
+00000a60: 6d61 6368 696e 6576 6973 696f 6e2d 746f  machinevision-to
+00000a70: 6f6c 626f 782d 7079 7468 6f6e 290a 215b  olbox-python).![
+00000a80: 5079 7468 6f6e 2056 6572 7369 6f6e 5d28  Python Version](
+00000a90: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000aa0: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+00000ab0: 7273 696f 6e73 2f6d 6163 6869 6e65 7669  rsions/machinevi
+00000ac0: 7369 6f6e 2d74 6f6f 6c62 6f78 2d70 7974  sion-toolbox-pyt
+00000ad0: 686f 6e2e 7376 6729 0a5b 215b 506f 7765  hon.svg).[![Powe
+00000ae0: 7265 6420 6279 204f 7065 6e43 565d 2868  red by OpenCV](h
+00000af0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000b00: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000b10: 2f70 6574 6572 636f 726b 652f 6d61 6368  /petercorke/mach
+00000b20: 696e 6576 6973 696f 6e2d 746f 6f6c 626f  inevision-toolbo
+00000b30: 782d 7079 7468 6f6e 2f6d 6173 7465 722f  x-python/master/
+00000b40: 2e67 6974 6875 622f 7376 672f 6f70 656e  .github/svg/open
+00000b50: 6376 5f70 6f77 6572 6564 2e73 7667 295d  cv_powered.svg)]
+00000b60: 2868 7474 7073 3a2f 2f6f 7065 6e63 762e  (https://opencv.
+00000b70: 6f72 6729 0a5b 215b 506f 7765 7265 6420  org).[![Powered 
+00000b80: 6279 204f 7065 6e33 445d 2868 7474 7073  by Open3D](https
+00000b90: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000ba0: 7263 6f6e 7465 6e74 2e63 6f6d 2f70 6574  rcontent.com/pet
+00000bb0: 6572 636f 726b 652f 6d61 6368 696e 6576  ercorke/machinev
+00000bc0: 6973 696f 6e2d 746f 6f6c 626f 782d 7079  ision-toolbox-py
+00000bd0: 7468 6f6e 2f6d 6173 7465 722f 2e67 6974  thon/master/.git
+00000be0: 6875 622f 7376 672f 6f70 656e 3364 5f70  hub/svg/open3d_p
+00000bf0: 6f77 6572 6564 2e73 7667 295d 2868 7474  owered.svg)](htt
+00000c00: 7073 3a2f 2f6f 7065 6e33 642e 6f72 6729  ps://open3d.org)
+00000c10: 0a5b 215b 4c69 6365 6e73 653a 204d 4954  .[![License: MIT
+00000c20: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000c30: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
+00000c40: 6963 656e 7365 2d4d 4954 2d79 656c 6c6f  icense-MIT-yello
+00000c50: 772e 7376 6729 5d28 6874 7470 733a 2f2f  w.svg)](https://
+00000c60: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
+00000c70: 6963 656e 7365 732f 4d49 5429 0a0a 5b21  icenses/MIT)..[!
+00000c80: 5b42 7569 6c64 2053 7461 7475 735d 2868  [Build Status](h
+00000c90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ca0: 6d2f 7065 7465 7263 6f72 6b65 2f6d 6163  m/petercorke/mac
+00000cb0: 6869 6e65 7669 7369 6f6e 2d74 6f6f 6c62  hinevision-toolb
+00000cc0: 6f78 2d70 7974 686f 6e2f 776f 726b 666c  ox-python/workfl
+00000cd0: 6f77 732f 5465 7374 2d6d 6173 7465 722f  ows/Test-master/
+00000ce0: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
+00000cf0: 3d6d 6173 7465 7229 5d28 6874 7470 733a  =master)](https:
+00000d00: 2f2f 6769 7468 7562 2e63 6f6d 2f70 6574  //github.com/pet
+00000d10: 6572 636f 726b 652f 6d61 6368 696e 6576  ercorke/machinev
+00000d20: 6973 696f 6e2d 746f 6f6c 626f 782d 7079  ision-toolbox-py
+00000d30: 7468 6f6e 2f61 6374 696f 6e73 3f71 7565  thon/actions?que
+00000d40: 7279 3d77 6f72 6b66 6c6f 7725 3341 6275  ry=workflow%3Abu
+00000d50: 696c 6429 0a5b 215b 436f 7665 7261 6765  ild).[![Coverage
+00000d60: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
+00000d70: 762e 696f 2f67 682f 7065 7465 7263 6f72  v.io/gh/petercor
+00000d80: 6b65 2f6d 6163 6869 6e65 7669 7369 6f6e  ke/machinevision
+00000d90: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e2f  -toolbox-python/
+00000da0: 6272 616e 6368 2f6d 6173 7465 722f 6772  branch/master/gr
+00000db0: 6170 682f 6261 6467 652e 7376 6729 5d28  aph/badge.svg)](
+00000dc0: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+00000dd0: 696f 2f67 682f 7065 7465 7263 6f72 6b65  io/gh/petercorke
+00000de0: 2f6d 6163 6869 6e65 7669 7369 6f6e 2d74  /machinevision-t
+00000df0: 6f6f 6c62 6f78 2d70 7974 686f 6e29 0a5b  oolbox-python).[
+00000e00: 215b 5079 5049 202d 2044 6f77 6e6c 6f61  ![PyPI - Downloa
+00000e10: 6473 5d28 6874 7470 733a 2f2f 696d 672e  ds](https://img.
+00000e20: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000e30: 6477 2f6d 6163 6869 6e65 7669 7369 6f6e  dw/machinevision
+00000e40: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e29  -toolbox-python)
+00000e50: 5d28 6874 7470 733a 2f2f 7079 7069 7374  ](https://pypist
+00000e60: 6174 732e 6f72 672f 7061 636b 6167 6573  ats.org/packages
+00000e70: 2f6d 6163 6869 6e65 7669 7369 6f6e 2d74  /machinevision-t
+00000e80: 6f6f 6c62 6f78 2d70 7974 686f 6e29 0a0a  oolbox-python)..
+00000e90: 3c21 2d2d 205b 215b 4769 7448 7562 2073  <!-- [![GitHub s
+00000ea0: 7461 7273 5d28 6874 7470 733a 2f2f 696d  tars](https://im
+00000eb0: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000ec0: 6875 622f 7374 6172 732f 7065 7465 7263  hub/stars/peterc
+00000ed0: 6f72 6b65 2f6d 6163 6869 6e65 7669 7369  orke/machinevisi
+00000ee0: 6f6e 2d74 6f6f 6c62 6f78 2d70 7974 686f  on-toolbox-pytho
+00000ef0: 6e2e 7376 673f 7374 796c 653d 736f 6369  n.svg?style=soci
+00000f00: 616c 266c 6162 656c 3d53 7461 7229 5d28  al&label=Star)](
+00000f10: 6874 7470 733a 2f2f 4769 7448 7562 2e63  https://GitHub.c
+00000f20: 6f6d 2f70 6574 6572 636f 726b 652f 6d61  om/petercorke/ma
+00000f30: 6368 696e 6576 6973 696f 6e2d 746f 6f6c  chinevision-tool
+00000f40: 626f 782d 7079 7468 6f6e 2f73 7461 7267  box-python/starg
+00000f50: 617a 6572 732f 2920 2d2d 3e0a 0a3c 7461  azers/) -->..<ta
+00000f60: 626c 6520 7374 796c 653d 2262 6f72 6465  ble style="borde
+00000f70: 723a 3070 7822 3e0a 3c74 7220 7374 796c  r:0px">.<tr styl
+00000f80: 653d 2262 6f72 6465 723a 3070 7822 3e0a  e="border:0px">.
+00000f90: 3c74 6420 7374 796c 653d 2262 6f72 6465  <td style="borde
+00000fa0: 723a 3070 7822 3e0a 3c69 6d67 2073 7263  r:0px">.<img src
+00000fb0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000fc0: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
+00000fd0: 6d61 6368 696e 6576 6973 696f 6e2d 746f  machinevision-to
+00000fe0: 6f6c 626f 782d 7079 7468 6f6e 2f72 6177  olbox-python/raw
+00000ff0: 2f6d 6173 7465 722f 6669 6773 2f56 6973  /master/figs/Vis
+00001000: 696f 6e54 6f6f 6c62 6f78 4c6f 676f 5f4e  ionToolboxLogo_N
+00001010: 6f42 6163 6b67 6e64 4032 782e 706e 6722  oBackgnd@2x.png"
+00001020: 2077 6964 7468 3d22 3230 3022 3e3c 2f74   width="200"></t
+00001030: 643e 0a3c 7464 2073 7479 6c65 3d22 626f  d>.<td style="bo
+00001040: 7264 6572 3a30 7078 223e 0a0a 4120 5079  rder:0px">..A Py
+00001050: 7468 6f6e 2069 6d70 6c65 6d65 6e74 6174  thon implementat
+00001060: 696f 6e20 6f66 2074 6865 203c 6120 6872  ion of the <a hr
+00001070: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00001080: 7562 2e63 6f6d 2f70 6574 6572 636f 726b  ub.com/petercork
+00001090: 652f 6d61 6368 696e 6576 6973 696f 6e2d  e/machinevision-
+000010a0: 746f 6f6c 626f 782d 6d61 746c 6162 223e  toolbox-matlab">
+000010b0: 4d61 6368 696e 6520 5669 7369 6f6e 2054  Machine Vision T
+000010c0: 6f6f 6c62 6f78 2066 6f72 204d 4154 4c41  oolbox for MATLA
+000010d0: 423c 7375 703e 2672 6567 3b3c 2f73 7570  B<sup>&reg;</sup
+000010e0: 3e3c 2f61 3e3c 756c 3e0a 0a3c 6c69 3e3c  ></a><ul>..<li><
+000010f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001100: 6769 7468 7562 2e63 6f6d 2f70 6574 6572  github.com/peter
+00001110: 636f 726b 652f 6d61 6368 696e 6576 6973  corke/machinevis
+00001120: 696f 6e2d 746f 6f6c 626f 782d 7079 7468  ion-toolbox-pyth
+00001130: 6f6e 223e 4769 7448 7562 2072 6570 6f73  on">GitHub repos
+00001140: 6974 6f72 7920 3c2f 613e 3c2f 6c69 3e0a  itory </a></li>.
+00001150: 3c6c 693e 3c61 2068 7265 663d 2268 7474  <li><a href="htt
+00001160: 7073 3a2f 2f70 6574 6572 636f 726b 652e  ps://petercorke.
+00001170: 6769 7468 7562 2e69 6f2f 6d61 6368 696e  github.io/machin
+00001180: 6576 6973 696f 6e2d 746f 6f6c 626f 782d  evision-toolbox-
+00001190: 7079 7468 6f6e 2f22 3e44 6f63 756d 656e  python/">Documen
+000011a0: 7461 7469 6f6e 3c2f 613e 3c2f 6c69 3e0a  tation</a></li>.
+000011b0: 3c6c 693e 3c61 2068 7265 663d 2268 7474  <li><a href="htt
+000011c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000011d0: 7065 7465 7263 6f72 6b65 2f6d 6163 6869  petercorke/machi
+000011e0: 6e65 7669 7369 6f6e 2d74 6f6f 6c62 6f78  nevision-toolbox
+000011f0: 2d70 7974 686f 6e2f 7769 6b69 223e 4578  -python/wiki">Ex
+00001200: 616d 706c 6573 2061 6e64 2064 6574 6169  amples and detai
+00001210: 6c73 3c2f 613e 3c2f 6c69 3e0a 3c6c 693e  ls</a></li>.<li>
+00001220: 3c61 2068 7265 663d 2269 6e73 7461 6c6c  <a href="install
+00001230: 6174 696f 6e23 223e 496e 7374 616c 6c61  ation#">Installa
+00001240: 7469 6f6e 3c2f 613e 3c2f 6c69 3e0a 3c2f  tion</a></li>.</
+00001250: 756c 3e0a 3c2f 7464 3e0a 3c2f 7472 3e0a  ul>.</td>.</tr>.
+00001260: 3c2f 7461 626c 653e 0a0a 2323 2053 796e  </table>..## Syn
+00001270: 6f70 7369 730a 0a54 6865 204d 6163 6869  opsis..The Machi
+00001280: 6e65 2056 6973 696f 6e20 546f 6f6c 626f  ne Vision Toolbo
+00001290: 7820 666f 7220 5079 7468 6f6e 2028 4d56  x for Python (MV
+000012a0: 5442 2d50 2920 7072 6f76 6964 6573 206d  TB-P) provides m
+000012b0: 616e 7920 6675 6e63 7469 6f6e 7320 7468  any functions th
+000012c0: 6174 2061 7265 2075 7365 6675 6c20 696e  at are useful in
+000012d0: 206d 6163 6869 6e65 2076 6973 696f 6e20   machine vision 
+000012e0: 616e 6420 7669 7369 6f6e 2d62 6173 6564  and vision-based
+000012f0: 2063 6f6e 7472 6f6c 2e20 5468 6520 6d61   control. The ma
+00001300: 696e 2063 6f6d 706f 6e65 6e74 7320 6172  in components ar
+00001310: 653a 0a0a 2d20 416e 2060 496d 6167 6560  e:..- An `Image`
+00001320: 206f 626a 6563 7420 7769 7468 206e 6561   object with nea
+00001330: 726c 7920 3230 3020 6d65 7468 6f64 7320  rly 200 methods 
+00001340: 616e 6420 7072 6f70 6572 7469 6573 2074  and properties t
+00001350: 6861 7420 7772 6170 2066 756e 6374 696f  hat wrap functio
+00001360: 6e73 0a20 2066 726f 6d20 4f70 656e 4356  ns.  from OpenCV
+00001370: 2c20 4e75 6d50 7920 616e 6420 5363 6950  , NumPy and SciP
+00001380: 792e 204d 6574 686f 6473 2073 7570 706f  y. Methods suppo
+00001390: 7274 206d 6f6e 6164 6963 2c20 6479 6164  rt monadic, dyad
+000013a0: 6963 2c20 6669 6c74 6572 696e 672c 2065  ic, filtering, e
+000013b0: 6467 6520 6465 7465 6374 696f 6e2c 0a20  dge detection,. 
+000013c0: 206d 6174 6865 6d61 7469 6361 6c20 6d6f   mathematical mo
+000013d0: 7270 686f 6c6f 6779 2061 6e64 2066 6561  rphology and fea
+000013e0: 7475 7265 2065 7874 7261 6374 696f 6e20  ture extraction 
+000013f0: 2862 6c6f 6273 2c20 6c69 6e65 7320 616e  (blobs, lines an
+00001400: 6420 706f 696e 742f 636f 726e 6572 2066  d point/corner f
+00001410: 6561 7475 7265 7329 2c20 6173 2077 656c  eatures), as wel
+00001420: 6c20 6173 206f 7065 7261 746f 7220 6f76  l as operator ov
+00001430: 6572 6c6f 6164 696e 672e 2049 6d61 6765  erloading. Image
+00001440: 7320 6172 6520 7374 6f72 6564 2061 7320  s are stored as 
+00001450: 656e 6361 7073 756c 6174 6564 205b 4e75  encapsulated [Nu
+00001460: 6d50 795d 2868 7474 7073 3a2f 2f6e 756d  mPy](https://num
+00001470: 7079 2e6f 7267 2920 6172 7261 7973 0a20  py.org) arrays. 
+00001480: 2061 6c6f 6e67 2077 6974 6820 696d 6167   along with imag
+00001490: 6520 6d65 7461 6461 7461 2e0a 2d20 416e  e metadata..- An
+000014a0: 206f 626a 6563 742d 6f72 6965 6e74 6564   object-oriented
+000014b0: 2077 7261 7070 6572 206f 6620 4f70 656e   wrapper of Open
+000014c0: 3344 2066 756e 6374 696f 6e73 2074 6861  3D functions tha
+000014d0: 7420 7375 7070 6f72 7473 2061 2073 7562  t supports a sub
+000014e0: 7365 7420 6f66 206f 7065 7261 7469 6f6e  set of operation
+000014f0: 732c 2062 7574 2061 6c6c 6f77 7320 6f70  s, but allows op
+00001500: 6572 6174 6f72 206f 7665 726c 6f61 6469  erator overloadi
+00001510: 6e67 2061 6e64 2069 7320 636f 6d70 6174  ng and is compat
+00001520: 6962 6c65 2077 6974 6820 7468 6520 5b53  ible with the [S
+00001530: 7061 7469 616c 204d 6174 6820 546f 6f6c  patial Math Tool
+00001540: 626f 785d 2868 7474 7073 3a2f 2f67 6974  box](https://git
+00001550: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
+00001560: 6b65 2f73 7061 7469 616c 6d61 7468 2d70  ke/spatialmath-p
+00001570: 7974 686f 6e29 2e0a 2d20 4120 636f 6c6c  ython)..- A coll
+00001580: 6563 7469 6f6e 206f 6620 6361 6d65 7261  ection of camera
+00001590: 2070 726f 6a65 6374 696f 6e20 636c 6173   projection clas
+000015a0: 7365 7320 666f 7220 6365 6e74 7261 6c20  ses for central 
+000015b0: 286e 6f72 6d61 6c20 7065 7273 7065 6374  (normal perspect
+000015c0: 6976 6529 2c20 6669 7368 6579 652c 2063  ive), fisheye, c
+000015d0: 6174 6164 696f 7074 7269 6320 616e 6420  atadioptric and 
+000015e0: 7370 6865 7269 6361 6c20 6361 6d65 7261  spherical camera
+000015f0: 732e 0a2d 2053 6f6d 6520 6164 7661 6e63  s..- Some advanc
+00001600: 6564 2061 6c67 6f72 6974 686d 7320 7375  ed algorithms su
+00001610: 6368 2061 733a 0a20 202d 206d 756c 7469  ch as:.  - multi
+00001620: 7669 6577 2067 656f 6d65 7472 793a 2063  view geometry: c
+00001630: 616d 6572 6120 6361 6c69 6272 6174 696f  amera calibratio
+00001640: 6e2c 2073 7465 7265 6f20 7669 7369 6f6e  n, stereo vision
+00001650: 2c20 6275 6e64 6c65 2061 646a 7573 746d  , bundle adjustm
+00001660: 656e 740a 2020 2d20 6261 6720 6f66 2077  ent.  - bag of w
+00001670: 6f72 6473 0a0a 4164 7661 6e74 6167 6573  ords..Advantages
+00001680: 206f 6620 7468 6973 2050 7974 686f 6e20   of this Python 
+00001690: 546f 6f6c 626f 7820 6172 6520 7468 6174  Toolbox are that
+000016a0: 3a0a 0a2d 2069 7420 7573 6573 2c20 6173  :..- it uses, as
+000016b0: 206d 7563 6820 6173 2070 6f73 7369 626c   much as possibl
+000016c0: 652c 205b 4f70 656e 4356 5d28 6874 7470  e, [OpenCV](http
+000016d0: 733a 2f2f 6f70 656e 6376 2e6f 7267 2920  s://opencv.org) 
+000016e0: 616e 6420 5b4e 756d 5079 5d28 6874 7470  and [NumPy](http
+000016f0: 733a 2f2f 6e75 6d70 792e 6f72 6729 2077  s://numpy.org) w
+00001700: 6869 6368 2061 7265 2070 6f72 7461 626c  hich are portabl
+00001710: 652c 2065 6666 6963 6965 6e74 2c20 636f  e, efficient, co
+00001720: 6d70 7265 6865 6e73 6976 6520 616e 6420  mprehensive and 
+00001730: 6d61 7475 7265 2063 6f6c 6c65 6374 696f  mature collectio
+00001740: 6e20 6f66 2066 756e 6374 696f 6e73 2066  n of functions f
+00001750: 6f72 2069 6d61 6765 2070 726f 6365 7373  or image process
+00001760: 696e 6720 616e 6420 6665 6174 7572 6520  ing and feature 
+00001770: 6578 7472 6163 7469 6f6e 3b0a 2d20 6974  extraction;.- it
+00001780: 2077 7261 7073 2074 6865 204f 7065 6e43   wraps the OpenC
+00001790: 5620 6675 6e63 7469 6f6e 7320 696e 2061  V functions in a
+000017a0: 2063 6f6e 7369 7374 656e 7420 7761 792c   consistent way,
+000017b0: 2068 6964 696e 6720 736f 6d65 206f 6620   hiding some of 
+000017c0: 7468 6520 676e 6172 6c79 2064 6574 6169  the gnarly detai
+000017d0: 6c73 206f 6620 4f70 656e 4356 206c 696b  ls of OpenCV lik
+000017e0: 6520 636f 6e76 6572 7369 6f6e 2074 6f2f  e conversion to/
+000017f0: 6672 6f6d 2066 6c6f 6174 3332 2061 6e64  from float32 and
+00001800: 2074 6865 2042 4752 2063 6f6c 6f72 206f   the BGR color o
+00001810: 7264 6572 2e0a 2d20 6974 2069 7320 6861  rder..- it is ha
+00001820: 7320 7369 6d69 6c61 7269 7479 2074 6f20  s similarity to 
+00001830: 7468 6520 4d61 6368 696e 6520 5669 7369  the Machine Visi
+00001840: 6f6e 2054 6f6f 6c62 6f78 2066 6f72 204d  on Toolbox for M
+00001850: 4154 4c41 422e 0a0a 2320 4765 7474 696e  ATLAB...# Gettin
+00001860: 6720 676f 696e 670a 0a23 2320 5573 696e  g going..## Usin
+00001870: 6720 7069 700a 0a49 6e73 7461 6c6c 2061  g pip..Install a
+00001880: 2073 6e61 7073 686f 7420 6672 6f6d 2050   snapshot from P
+00001890: 7950 490a 0a60 6060 0a25 2070 6970 2069  yPI..```.% pip i
+000018a0: 6e73 7461 6c6c 206d 6163 6869 6e65 7669  nstall machinevi
+000018b0: 7369 6f6e 2d74 6f6f 6c62 6f78 2d70 7974  sion-toolbox-pyt
+000018c0: 686f 6e0a 6060 600a 0a23 2320 4672 6f6d  hon.```..## From
+000018d0: 2047 6974 4875 620a 0a49 6e73 7461 6c6c   GitHub..Install
+000018e0: 2074 6865 2063 7572 7265 6e74 2063 6f64   the current cod
+000018f0: 6520 6261 7365 2066 726f 6d20 4769 7448  e base from GitH
+00001900: 7562 2061 6e64 2070 6970 2069 6e73 7461  ub and pip insta
+00001910: 6c6c 2061 206c 696e 6b20 746f 2074 6861  ll a link to tha
+00001920: 7420 636c 6f6e 6564 2063 6f70 790a 0a60  t cloned copy..`
+00001930: 6060 0a25 2067 6974 2063 6c6f 6e65 2068  ``.% git clone h
+00001940: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001950: 6d2f 7065 7465 7263 6f72 6b65 2f6d 6163  m/petercorke/mac
+00001960: 6869 6e65 7669 7369 6f6e 2d74 6f6f 6c62  hinevision-toolb
+00001970: 6f78 2d70 7974 686f 6e2e 6769 740a 2520  ox-python.git.% 
+00001980: 6364 206d 6163 6869 6e65 7669 7369 6f6e  cd machinevision
+00001990: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e0a  -toolbox-python.
+000019a0: 2520 7069 7020 696e 7374 616c 6c20 2d65  % pip install -e
+000019b0: 202e 0a60 6060 0a0a 2320 4578 616d 706c   ..```..# Exampl
+000019c0: 6573 0a0a 2323 2320 5265 6164 696e 6720  es..### Reading 
+000019d0: 616e 6420 6469 7370 6c61 7920 616e 2069  and display an i
+000019e0: 6d61 6765 0a0a 6060 6070 7974 686f 6e0a  mage..```python.
+000019f0: 6672 6f6d 206d 6163 6869 6e65 7669 7369  from machinevisi
+00001a00: 6f6e 746f 6f6c 626f 7820 696d 706f 7274  ontoolbox import
+00001a10: 2049 6d61 6765 0a6d 6f6e 6120 3d20 496d   Image.mona = Im
+00001a20: 6167 652e 5265 6164 2822 6d6f 6e61 6c69  age.Read("monali
+00001a30: 7361 2e70 6e67 2229 0a6d 6f6e 612e 6469  sa.png").mona.di
+00001a40: 7370 2829 0a60 6060 0a0a 215b 4d6f 6e61  sp().```..![Mona
+00001a50: 204c 6973 6120 696d 6167 655d 2868 7474   Lisa image](htt
+00001a60: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001a70: 7065 7465 7263 6f72 6b65 2f6d 6163 6869  petercorke/machi
+00001a80: 6e65 7669 7369 6f6e 2d74 6f6f 6c62 6f78  nevision-toolbox
+00001a90: 2d70 7974 686f 6e2f 7261 772f 6d61 7374  -python/raw/mast
+00001aa0: 6572 2f66 6967 732f 6d6f 6e61 2e70 6e67  er/figs/mona.png
+00001ab0: 290a 0a49 6d61 6765 7320 6361 6e20 616c  )..Images can al
+00001ac0: 736f 2062 6520 7265 7475 726e 6564 2062  so be returned b
+00001ad0: 7920 6974 6572 6174 6f72 7320 7468 6174  y iterators that
+00001ae0: 206f 7065 7261 7465 206f 7665 7220 666f   operate over fo
+00001af0: 6c64 6572 732c 207a 6970 2066 696c 6573  lders, zip files
+00001b00: 2c20 6c6f 6361 6c20 6361 6d65 7261 732c  , local cameras,
+00001b10: 2077 6562 2063 616d 6572 6173 2061 6e64   web cameras and
+00001b20: 2076 6964 656f 2066 696c 6573 2e0a 0a23   video files...#
+00001b30: 2323 2053 696d 706c 6520 696d 6167 6520  ## Simple image 
+00001b40: 7072 6f63 6573 7369 6e67 0a0a 5468 6520  processing..The 
+00001b50: 746f 6f6c 626f 7820 7375 7070 6f72 7473  toolbox supports
+00001b60: 206d 616e 7920 6f70 6572 6174 696f 6e73   many operations
+00001b70: 206f 6e20 696d 6167 6573 2073 7563 6820   on images such 
+00001b80: 6173 2032 4420 6669 6c74 6572 696e 672c  as 2D filtering,
+00001b90: 2065 6467 6520 6465 7465 6374 696f 6e2c   edge detection,
+00001ba0: 206d 6174 6865 6d61 7469 6361 6c20 6d6f   mathematical mo
+00001bb0: 7270 686f 6c6f 6779 2c20 636f 6c6f 7273  rphology, colors
+00001bc0: 7061 6365 2063 6f6e 7665 7273 696f 6e2c  pace conversion,
+00001bd0: 2070 6164 6469 6e67 2c20 6372 6f70 7069   padding, croppi
+00001be0: 6e67 2c20 7265 7369 7a69 6e67 2c20 726f  ng, resizing, ro
+00001bf0: 7461 7469 6f6e 2061 6e64 2077 6172 7069  tation and warpi
+00001c00: 6e67 2e0a 0a60 6060 7079 7468 6f6e 0a6d  ng...```python.m
+00001c10: 6f6e 612e 736d 6f6f 7468 2873 6967 6d61  ona.smooth(sigma
+00001c20: 3d35 292e 6469 7370 2829 0a60 6060 0a0a  =5).disp().```..
+00001c30: 215b 4d6f 6e61 204c 6973 6120 696d 6167  ![Mona Lisa imag
+00001c40: 6520 7769 7468 2073 6d6f 6f74 6869 6e67  e with smoothing
+00001c50: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001c60: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
+00001c70: 6d61 6368 696e 6576 6973 696f 6e2d 746f  machinevision-to
+00001c80: 6f6c 626f 782d 7079 7468 6f6e 2f72 6177  olbox-python/raw
+00001c90: 2f6d 6173 7465 722f 6669 6773 2f6d 6f6e  /master/figs/mon
+00001ca0: 615f 736d 6f6f 7468 2e70 6e67 290a 0a54  a_smooth.png)..T
+00001cb0: 6865 7265 2061 7265 2061 6c73 6f20 6d61  here are also ma
+00001cc0: 6e79 2066 756e 6374 696f 6e73 2074 6861  ny functions tha
+00001cd0: 7420 6f70 6572 6174 6520 6f6e 2070 6169  t operate on pai
+00001ce0: 7273 206f 6620 696d 6167 652e 2041 6c6c  rs of image. All
+00001cf0: 2074 6865 2061 7269 7468 6d65 7469 6320   the arithmetic 
+00001d00: 6f70 6572 6174 6f72 7320 6172 6520 6f76  operators are ov
+00001d10: 6572 6c6f 6164 6564 2c20 616e 6420 7468  erloaded, and th
+00001d20: 6572 6520 6172 6520 6d65 7468 6f64 7320  ere are methods 
+00001d30: 746f 2063 6f6d 6269 6e65 2069 6d61 6765  to combine image
+00001d40: 7320 696e 206d 6f72 6520 636f 6d70 6c65  s in more comple
+00001d50: 7820 7761 7973 2e20 4d75 6c74 6970 6c65  x ways. Multiple
+00001d60: 2069 6d61 6765 7320 6361 6e20 6265 2073   images can be s
+00001d70: 7461 636b 6564 2068 6f72 697a 6f6e 7461  tacked horizonta
+00001d80: 6c2c 2076 6572 7469 6361 6c6c 7920 6f72  l, vertically or
+00001d90: 2074 696c 6564 2069 6e20 6120 3244 2067   tiled in a 2D g
+00001da0: 7269 642e 2046 6f72 2065 7861 6d70 6c65  rid. For example
+00001db0: 2c20 7765 2063 6f75 6c64 2064 6973 706c  , we could displ
+00001dc0: 6179 2074 6865 206f 7269 6769 6e61 6c20  ay the original 
+00001dd0: 616e 6420 736d 6f6f 7468 6564 2069 6d61  and smoothed ima
+00001de0: 6765 7320 7369 6465 2062 7920 7369 6465  ges side by side
+00001df0: 0a0a 6060 6070 7974 686f 6e0a 496d 6167  ..```python.Imag
+00001e00: 652e 4873 7461 636b 285b 6d6f 6e61 2c20  e.Hstack([mona, 
+00001e10: 6d6f 6e61 2e73 6d6f 6f74 6828 7369 676d  mona.smooth(sigm
+00001e20: 613d 3529 5d29 2e64 6973 7028 290a 6060  a=5)]).disp().``
+00001e30: 600a 0a77 6865 7265 2060 4873 7461 636b  `..where `Hstack
+00001e40: 6020 6973 2061 2063 6c61 7373 206d 6574  ` is a class met
+00001e50: 686f 6420 7468 6174 2063 7265 6174 6573  hod that creates
+00001e60: 2061 206e 6577 2069 6d61 6765 2062 7920   a new image by 
+00001e70: 7374 6163 6b69 6e67 2074 6865 0a69 6d61  stacking the.ima
+00001e80: 6765 7320 6672 6f6d 2069 7473 2061 7267  ges from its arg
+00001e90: 756d 656e 742c 2061 6e20 696d 6167 6520  ument, an image 
+00001ea0: 7365 7175 656e 6365 2c20 686f 7269 7a6f  sequence, horizo
+00001eb0: 6e74 616c 6c79 2e0a 0a21 5b4d 6f6e 6120  ntally...![Mona 
+00001ec0: 4c69 7361 2069 6d61 6765 2077 6974 6820  Lisa image with 
+00001ed0: 736d 6f6f 7468 696e 675d 2868 7474 7073  smoothing](https
+00001ee0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7065  ://github.com/pe
+00001ef0: 7465 7263 6f72 6b65 2f6d 6163 6869 6e65  tercorke/machine
+00001f00: 7669 7369 6f6e 2d74 6f6f 6c62 6f78 2d70  vision-toolbox-p
+00001f10: 7974 686f 6e2f 7261 772f 6d61 7374 6572  ython/raw/master
+00001f20: 2f66 6967 732f 6d6f 6e61 2b73 6d6f 6f74  /figs/mona+smoot
+00001f30: 682e 706e 6729 0a0a 2323 2320 4269 6e61  h.png)..### Bina
+00001f40: 7279 2062 6c6f 6273 0a0a 4120 636f 6d6d  ry blobs..A comm
+00001f50: 6f6e 2070 726f 626c 656d 2069 6e20 726f  on problem in ro
+00001f60: 626f 7469 6320 7669 7369 6f6e 2069 7320  botic vision is 
+00001f70: 746f 2065 7874 7261 6374 2066 6561 7475  to extract featu
+00001f80: 7265 7320 6672 6f6d 2074 6865 2069 6d61  res from the ima
+00001f90: 6765 2c20 746f 2064 6573 6372 6962 6520  ge, to describe 
+00001fa0: 7468 6520 706f 7369 7469 6f6e 2c20 7369  the position, si
+00001fb0: 7a65 2c20 7368 6170 6520 616e 6420 6f72  ze, shape and or
+00001fc0: 6965 6e74 6174 696f 6e20 6f66 206f 626a  ientation of obj
+00001fd0: 6563 7473 2069 6e20 7468 6520 7363 656e  ects in the scen
+00001fe0: 652e 2046 6f72 2073 696d 706c 6520 6269  e. For simple bi
+00001ff0: 6e61 7279 2073 6365 6e65 7320 626c 6f62  nary scenes blob
+00002000: 2066 6561 7475 7265 7320 6172 6520 636f   features are co
+00002010: 6d6d 6f6e 6c79 2075 7365 642e 0a0a 6060  mmonly used...``
+00002020: 6070 7974 686f 6e0a 696d 203d 2049 6d61  `python.im = Ima
+00002030: 6765 2e52 6561 6428 2273 6861 726b 322e  ge.Read("shark2.
+00002040: 706e 6722 2920 2020 2320 7265 6164 2061  png")   # read a
+00002050: 2062 696e 6172 7920 696d 6167 6520 6f66   binary image of
+00002060: 2074 776f 2073 6861 726b 730a 696d 2e64   two sharks.im.d
+00002070: 6973 7028 293b 2020 2023 2064 6973 706c  isp();   # displ
+00002080: 6179 2069 7420 7769 7468 2069 6e74 6572  ay it with inter
+00002090: 6163 7469 7665 2076 6965 7769 6e67 2074  active viewing t
+000020a0: 6f6f 6c0a 626c 6f62 7320 3d20 696d 2e62  ool.blobs = im.b
+000020b0: 6c6f 6273 2829 2020 2320 6669 6e64 2061  lobs()  # find a
+000020c0: 6c6c 2074 6865 2077 6869 7465 2062 6c6f  ll the white blo
+000020d0: 6273 0a70 7269 6e74 2862 6c6f 6273 290a  bs.print(blobs).
+000020e0: 0a09 e294 8ce2 9480 e294 80e2 9480 e294  ................
+000020f0: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002100: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
+00002110: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002120: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002130: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
+00002140: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002150: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
+00002160: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002170: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
+00002180: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
+00002190: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000021a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000021b0: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
+000021c0: e294 80e2 9480 e294 80e2 9480 e294 ace2  ................
+000021d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000021e0: 80e2 9480 e294 80e2 9490 0a09 e294 8269  ...............i
+000021f0: 6420 e294 8220 7061 7265 6e74 20e2 9482  d ... parent ...
+00002200: 2020 2020 2063 656e 7472 6f69 6420 e294       centroid ..
+00002210: 8220 2020 2020 6172 6561 20e2 9482 2074  .     area ... t
+00002220: 6f75 6368 20e2 9482 2070 6572 696d 20e2  ouch ... perim .
+00002230: 9482 2063 6972 6375 6c61 7269 7479 20e2  .. circularity .
+00002240: 9482 206f 7269 656e 7420 e294 8220 6173  .. orient ... as
+00002250: 7065 6374 20e2 9482 0a09 e294 9ce2 9480  pect ...........
+00002260: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+00002270: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002280: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+00002290: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000022a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000022b0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000022c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000022d0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+000022e0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+000022f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002300: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+00002310: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002320: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+00002330: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002340: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+00002350: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002360: 94a4 0a09 e294 8220 3020 e294 8220 2020  ....... 0 ...   
+00002370: 2020 2d31 20e2 9482 2033 3731 2e32 2c20    -1 ... 371.2, 
+00002380: 3335 352e 3220 e294 8220 372e 3539 652b  355.2 ... 7.59e+
+00002390: 3033 20e2 9482 2046 616c 7365 20e2 9482  03 ... False ...
+000023a0: 2035 3537 2e36 20e2 9482 2020 2020 2020   557.6 ...      
+000023b0: 2030 2e33 3431 20e2 9482 2020 3832 2e39   0.341 ...  82.9
+000023c0: c2b0 20e2 9482 2020 302e 3937 3620 e294  .. ...  0.976 ..
+000023d0: 820a 09e2 9482 2031 20e2 9482 2020 2020  ...... 1 ...    
+000023e0: 202d 3120 e294 8220 3137 312e 322c 2031   -1 ... 171.2, 1
+000023f0: 3535 2e32 20e2 9482 2037 2e35 3965 2b30  55.2 ... 7.59e+0
+00002400: 3320 e294 8220 4661 6c73 6520 e294 8220  3 ... False ... 
+00002410: 3535 372e 3620 e294 8220 2020 2020 2020  557.6 ...       
+00002420: 302e 3334 3120 e294 8220 2038 322e 39c2  0.341 ...  82.9.
+00002430: b020 e294 8220 2030 2e39 3736 20e2 9482  . ...  0.976 ...
+00002440: 0a09 e294 94e2 9480 e294 80e2 9480 e294  ................
+00002450: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002460: e294 80e2 9480 e294 80e2 94b4 e294 80e2  ................
+00002470: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002480: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002490: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
+000024a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000024b0: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
+000024c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000024d0: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
+000024e0: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
+000024f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002500: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002510: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
+00002520: e294 80e2 9480 e294 80e2 9480 e294 b4e2  ................
+00002530: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002540: 80e2 9480 e294 80e2 9498 0a60 6060 0a0a  ...........```..
+00002550: 7768 6572 6520 6062 6c6f 6273 6020 6973  where `blobs` is
+00002560: 2061 206c 6973 742d 6c69 6b65 206f 626a   a list-like obj
+00002570: 6563 7420 616e 6420 6561 6368 2065 6c65  ect and each ele
+00002580: 6d65 6e74 2064 6573 6372 6962 6573 2061  ment describes a
+00002590: 2062 6c6f 6220 696e 2074 6865 2073 6365   blob in the sce
+000025a0: 6e65 2e20 5468 6520 656c 656d 656e 7427  ne. The element'
+000025b0: 7320 6174 7472 6962 7574 6573 2064 6573  s attributes des
+000025c0: 6372 6962 6520 7661 7269 6f75 7320 7061  cribe various pa
+000025d0: 7261 6d65 7465 7273 206f 6620 7468 6520  rameters of the 
+000025e0: 6f62 6a65 6374 2c20 616e 6420 6d65 7468  object, and meth
+000025f0: 6f64 7320 6361 6e20 6265 2075 7365 6420  ods can be used 
+00002600: 746f 206f 7665 726c 6179 2067 7261 7068  to overlay graph
+00002610: 6963 7320 7375 6368 2061 7320 626f 756e  ics such as boun
+00002620: 6469 6e67 2062 6f78 6573 2061 6e64 2063  ding boxes and c
+00002630: 656e 7472 6f69 6473 0a0a 6060 6070 7974  entroids..```pyt
+00002640: 686f 6e0a 626c 6f62 732e 706c 6f74 5f62  hon.blobs.plot_b
+00002650: 6f78 2863 6f6c 6f72 3d22 6722 2c20 6c69  ox(color="g", li
+00002660: 6e65 7769 6474 683d 3229 2020 2320 7075  newidth=2)  # pu
+00002670: 7420 6120 6772 6565 6e20 626f 756e 6469  t a green boundi
+00002680: 6e67 2062 6f78 206f 6e20 6561 6368 2062  ng box on each b
+00002690: 6c6f 620a 626c 6f62 732e 706c 6f74 5f63  lob.blobs.plot_c
+000026a0: 656e 7472 6f69 6428 6c61 6265 6c3d 5472  entroid(label=Tr
+000026b0: 7565 2920 2023 2070 7574 2061 2063 6972  ue)  # put a cir
+000026c0: 636c 652b 6372 6f73 7320 6f6e 2074 6865  cle+cross on the
+000026d0: 2063 656e 7472 6f69 6420 6f66 2065 6163   centroid of eac
+000026e0: 6820 626c 6f62 0a70 6c74 2e73 686f 7728  h blob.plt.show(
+000026f0: 626c 6f63 6b3d 5472 7565 2920 2023 2064  block=True)  # d
+00002700: 6973 706c 6179 2074 6865 2072 6573 756c  isplay the resul
+00002710: 740a 6060 600a 0a21 5b42 696e 6172 7920  t.```..![Binary 
+00002720: 696d 6167 6520 7368 6f77 696e 6720 626f  image showing bo
+00002730: 756e 6469 6e67 2062 6f78 6573 2061 6e64  unding boxes and
+00002740: 2063 656e 7472 6f69 6473 5d28 6874 7470   centroids](http
+00002750: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00002760: 6574 6572 636f 726b 652f 6d61 6368 696e  etercorke/machin
+00002770: 6576 6973 696f 6e2d 746f 6f6c 626f 782d  evision-toolbox-
+00002780: 7079 7468 6f6e 2f72 6177 2f6d 6173 7465  python/raw/maste
+00002790: 722f 6669 6773 2f73 6861 726b 322b 626f  r/figs/shark2+bo
+000027a0: 7865 732e 706e 6729 0a0a 2323 2323 2042  xes.png)..#### B
+000027b0: 696e 6172 7920 626c 6f62 2068 6965 7261  inary blob hiera
+000027c0: 7263 6879 0a0a 4120 6d6f 7265 2063 6f6d  rchy..A more com
+000027d0: 706c 6578 2069 6d61 6765 2069 730a 0a60  plex image is..`
+000027e0: 6060 7079 7468 6f6e 0a69 6d20 3d20 496d  ``python.im = Im
+000027f0: 6167 652e 5265 6164 2822 6d75 6c74 6962  age.Read("multib
+00002800: 6c6f 6273 2e70 6e67 2229 0a69 6d2e 6469  lobs.png").im.di
+00002810: 7370 2829 0a60 6060 0a0a 215b 4269 6e61  sp().```..![Bina
+00002820: 7279 2069 6d61 6765 2077 6974 6820 6e65  ry image with ne
+00002830: 7374 6564 2062 6c6f 6273 5d28 6874 7470  sted blobs](http
+00002840: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00002850: 6574 6572 636f 726b 652f 6d61 6368 696e  etercorke/machin
+00002860: 6576 6973 696f 6e2d 746f 6f6c 626f 782d  evision-toolbox-
+00002870: 7079 7468 6f6e 2f72 6177 2f6d 6173 7465  python/raw/maste
+00002880: 722f 6669 6773 2f6d 756c 7469 2e70 6e67  r/figs/multi.png
+00002890: 290a 0a61 6e64 2077 6520 7365 6520 7468  )..and we see th
+000028a0: 6174 2073 6f6d 6520 626c 6f62 7320 6172  at some blobs ar
+000028b0: 6520 636f 6e74 6169 6e65 6420 7769 7468  e contained with
+000028c0: 696e 206f 7468 6572 2062 6c6f 6273 2e20  in other blobs. 
+000028d0: 5468 6520 7265 7375 6c74 7320 696e 2074  The results in t
+000028e0: 6162 756c 6172 2066 6f72 6d0a 0a60 6060  abular form..```
+000028f0: 7079 7468 6f6e 0a62 6c6f 6273 2020 3d20  python.blobs  = 
+00002900: 696d 2e62 6c6f 6273 2829 0a70 7269 6e74  im.blobs().print
+00002910: 2862 6c6f 6273 290a 09e2 948c e294 80e2  (blobs).........
+00002920: 9480 e294 80e2 94ac e294 80e2 9480 e294  ................
 00002930: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002940: e294 80e2 9480 e294 980a 6060 600a 0a57  ..........```..W
-00002950: 6520 6361 6e20 6469 7370 6c61 7920 6120  e can display a 
-00002960: 6c61 6265 6c20 696d 6167 652c 2077 6865  label image, whe
-00002970: 7265 2074 6865 2076 616c 7565 206f 6620  re the value of 
-00002980: 6561 6368 2070 6978 656c 2069 7320 7468  each pixel is th
-00002990: 6520 6c61 6265 6c20 6f66 2074 6865 2062  e label of the b
-000029a0: 6c6f 6220 7468 6174 2074 6865 2070 6978  lob that the pix
-000029b0: 656c 0a62 656c 6f6e 6773 2074 6f2c 2074  el.belongs to, t
-000029c0: 6865 2060 6964 6020 6174 7472 6962 7574  he `id` attribut
-000029d0: 650a 0a60 6060 7079 7468 6f6e 0a6c 6162  e..```python.lab
-000029e0: 656c 7320 3d20 626c 6f62 732e 6c61 6265  els = blobs.labe
-000029f0: 6c5f 696d 6167 6528 290a 6c61 6265 6c73  l_image().labels
-00002a00: 2e64 6973 7028 636f 6c6f 726d 6170 3d22  .disp(colormap="
-00002a10: 7669 7269 6469 7322 2c20 6e63 6f6c 6f72  viridis", ncolor
-00002a20: 733d 6c65 6e28 626c 6f62 7329 2c20 636f  s=len(blobs), co
-00002a30: 6c6f 7262 6172 3d64 6963 7428 7368 7269  lorbar=dict(shri
-00002a40: 6e6b 3d30 2e38 2c20 6173 7065 6374 3d32  nk=0.8, aspect=2
-00002a50: 302a 302e 3829 290a 6060 600a 0a21 5b46  0*0.8)).```..![F
-00002a60: 616c 7365 2063 6f6c 6f72 206c 6162 656c  alse color label
-00002a70: 2069 6d61 6765 5d28 6874 7470 733a 2f2f   image](https://
-00002a80: 6769 7468 7562 2e63 6f6d 2f70 6574 6572  github.com/peter
-00002a90: 636f 726b 652f 6d61 6368 696e 6576 6973  corke/machinevis
-00002aa0: 696f 6e2d 746f 6f6c 626f 782d 7079 7468  ion-toolbox-pyth
-00002ab0: 6f6e 2f72 6177 2f6d 6173 7465 722f 6669  on/raw/master/fi
-00002ac0: 6773 2f6d 756c 7469 5f6c 6162 656c 6c65  gs/multi_labelle
-00002ad0: 642e 706e 6729 0a0a 5765 2063 616e 2061  d.png)..We can a
-00002ae0: 6c73 6f20 7468 696e 6b20 6f66 2074 6865  lso think of the
-00002af0: 2062 6c6f 6273 2066 6f72 6d69 6e67 2061   blobs forming a
-00002b00: 2068 6965 6172 6368 7920 616e 6420 7468   hiearchy and th
-00002b10: 6174 2072 656c 6174 696f 6e73 6869 7020  at relationship 
-00002b20: 6973 2072 6566 6c65 6374 6564 2069 6e20  is reflected in 
-00002b30: 7468 6520 6070 6172 656e 7460 2061 6e64  the `parent` and
-00002b40: 2060 6368 696c 6472 656e 6020 6174 7472   `children` attr
-00002b50: 6962 7574 6573 206f 6620 7468 6520 626c  ibutes of the bl
-00002b60: 6f62 732e 0a57 6520 6361 6e20 616c 736f  obs..We can also
-00002b70: 2065 7870 7265 7373 2069 7420 6173 2061   express it as a
-00002b80: 2064 6972 6563 7465 6420 6772 6170 680a   directed graph.
-00002b90: 0a60 6060 7079 7468 6f6e 0a62 6c6f 6273  .```python.blobs
-00002ba0: 2e64 6f74 6669 6c65 2873 686f 773d 5472  .dotfile(show=Tr
-00002bb0: 7565 290a 6060 600a 0a21 5b42 6c6f 6220  ue).```..![Blob 
-00002bc0: 6869 6572 6172 6368 7920 6173 2061 2067  hierarchy as a g
-00002bd0: 7261 7068 5d28 6874 7470 733a 2f2f 6769  raph](https://gi
-00002be0: 7468 7562 2e63 6f6d 2f70 6574 6572 636f  thub.com/peterco
-00002bf0: 726b 652f 6d61 6368 696e 6576 6973 696f  rke/machinevisio
-00002c00: 6e2d 746f 6f6c 626f 782d 7079 7468 6f6e  n-toolbox-python
-00002c10: 2f72 6177 2f6d 6173 7465 722f 6669 6773  /raw/master/figs
-00002c20: 2f62 6c6f 6273 5f67 7261 7068 2e70 6e67  /blobs_graph.png
-00002c30: 290a 0a23 2323 2043 616d 6572 6120 6d6f  )..### Camera mo
-00002c40: 6465 6c6c 696e 670a 0a60 6060 7079 7468  delling..```pyth
-00002c50: 6f6e 0a66 726f 6d20 6d61 6368 696e 6576  on.from machinev
-00002c60: 6973 696f 6e74 6f6f 6c62 6f78 2069 6d70  isiontoolbox imp
-00002c70: 6f72 7420 4365 6e74 7261 6c43 616d 6572  ort CentralCamer
-00002c80: 610a 6361 6d20 3d20 4365 6e74 7261 6c43  a.cam = CentralC
-00002c90: 616d 6572 6128 663d 302e 3031 352c 2072  amera(f=0.015, r
-00002ca0: 686f 3d31 3065 2d36 2c20 696d 6167 6573  ho=10e-6, images
-00002cb0: 697a 653d 5b31 3238 302c 2031 3032 345d  ize=[1280, 1024]
-00002cc0: 2c20 7070 3d5b 3634 302c 2035 3132 5d2c  , pp=[640, 512],
-00002cd0: 206e 616d 653d 226d 7963 616d 6572 6122   name="mycamera"
-00002ce0: 290a 7072 696e 7428 6361 6d29 0a20 2020  ).print(cam).   
-00002cf0: 2020 2020 2020 2020 4e61 6d65 3a20 6d79          Name: my
-00002d00: 6361 6d65 7261 205b 4365 6e74 7261 6c43  camera [CentralC
-00002d10: 616d 6572 615d 0a20 2020 2020 7069 7865  amera].     pixe
-00002d20: 6c20 7369 7a65 3a20 3165 2d30 3520 7820  l size: 1e-05 x 
-00002d30: 3165 2d30 350a 2020 2020 2069 6d61 6765  1e-05.     image
-00002d40: 2073 697a 653a 2031 3238 3020 7820 3130   size: 1280 x 10
-00002d50: 3234 0a20 2020 2020 2020 2020 2020 706f  24.           po
-00002d60: 7365 3a20 7420 3d20 302c 2030 2c20 303b  se: t = 0, 0, 0;
-00002d70: 2072 7079 2f79 787a 203d 2030 c2b0 2c20   rpy/yxz = 0.., 
-00002d80: 30c2 b02c 2030 c2b0 0a20 2020 7072 696e  0.., 0...   prin
-00002d90: 6369 7061 6c20 7074 3a20 5b20 2020 2020  cipal pt: [     
-00002da0: 3634 3020 2020 2020 2035 3132 5d0a 2020  640      512].  
-00002db0: 2066 6f63 616c 206c 656e 6774 683a 205b   focal length: [
-00002dc0: 2020 2030 2e30 3135 2020 2020 302e 3031     0.015    0.01
-00002dd0: 355d 0a60 6060 0a0a 616e 6420 6974 7320  5].```..and its 
-00002de0: 696e 7472 696e 7369 6320 7061 7261 6d65  intrinsic parame
-00002df0: 7465 7273 2061 7265 0a0a 6060 6070 7974  ters are..```pyt
-00002e00: 686f 6e0a 7072 696e 7428 6361 6d2e 4b29  hon.print(cam.K)
-00002e10: 0a09 5b5b 312e 3530 652b 3033 2030 2e30  ..[[1.50e+03 0.0
-00002e20: 3065 2b30 3020 362e 3430 652b 3032 5d0a  0e+00 6.40e+02].
-00002e30: 0920 5b30 2e30 3065 2b30 3020 312e 3530  . [0.00e+00 1.50
-00002e40: 652b 3033 2035 2e31 3265 2b30 325d 0a09  e+03 5.12e+02]..
-00002e50: 205b 302e 3030 652b 3030 2030 2e30 3065   [0.00e+00 0.00e
-00002e60: 2b30 3020 312e 3030 652b 3030 5d5d 0a60  +00 1.00e+00]].`
-00002e70: 6060 0a0a 5765 2063 616e 2064 6566 696e  ``..We can defin
-00002e80: 6520 616e 2061 7262 6974 7261 7279 2070  e an arbitrary p
-00002e90: 6f69 6e74 2069 6e20 7468 6520 776f 726c  oint in the worl
-00002ea0: 640a 0a60 6060 7079 7468 6f6e 0a50 203d  d..```python.P =
-00002eb0: 205b 302e 332c 2030 2e34 2c20 332e 305d   [0.3, 0.4, 3.0]
-00002ec0: 0a60 6060 0a0a 616e 6420 7468 656e 2070  .```..and then p
-00002ed0: 726f 6a65 6374 2069 7420 696e 746f 2074  roject it into t
-00002ee0: 6865 2063 616d 6572 610a 0a60 6060 7079  he camera..```py
-00002ef0: 7468 6f6e 0a70 203d 2063 616d 2e70 726f  thon.p = cam.pro
-00002f00: 6a65 6374 2850 290a 7072 696e 7428 7029  ject(P).print(p)
-00002f10: 0a09 5b37 3930 2e20 3731 322e 5d0a 6060  ..[790. 712.].``
-00002f20: 600a 0a77 6869 6368 2069 7320 7468 6520  `..which is the 
-00002f30: 636f 7272 6573 706f 6e64 696e 6720 636f  corresponding co
-00002f40: 6f72 6469 6e61 7465 2069 6e20 7069 7865  ordinate in pixe
-00002f50: 6c73 2e20 4966 2077 6520 7368 6966 7420  ls. If we shift 
-00002f60: 7468 6520 6361 6d65 7261 2073 6c69 6768  the camera sligh
-00002f70: 746c 7920 7468 6520 696d 6167 6520 706c  tly the image pl
-00002f80: 616e 6520 636f 6f72 6469 6e61 7465 2077  ane coordinate w
-00002f90: 696c 6c20 616c 736f 2063 6861 6e67 650a  ill also change.
-00002fa0: 0a60 6060 7079 7468 6f6e 0a70 203d 2063  .```python.p = c
-00002fb0: 616d 2e70 726f 6a65 6374 2850 2c20 543d  am.project(P, T=
-00002fc0: 5345 3328 302e 312c 2030 2c20 3029 2029  SE3(0.1, 0, 0) )
-00002fd0: 0a70 7269 6e74 2870 290a 5b37 3430 2e20  .print(p).[740. 
-00002fe0: 3731 322e 5d0a 6060 600a 0a57 6520 6361  712.].```..We ca
-00002ff0: 6e20 6465 6669 6e65 2061 6e20 6564 6765  n define an edge
-00003000: 2d62 6173 6564 2063 7562 6520 6d6f 6465  -based cube mode
-00003010: 6c20 616e 6420 7072 6f6a 6563 7420 6974  l and project it
-00003020: 2069 6e74 6f20 7468 6520 6361 6d65 7261   into the camera
-00003030: 2773 2069 6d61 6765 2070 6c61 6e65 0a0a  's image plane..
-00003040: 6060 6070 7974 686f 6e0a 6672 6f6d 2073  ```python.from s
-00003050: 7061 7469 616c 6d61 7468 2069 6d70 6f72  patialmath impor
-00003060: 7420 5345 330a 582c 2059 2c20 5a20 3d20  t SE3.X, Y, Z = 
-00003070: 6d6b 6375 6265 2830 2e32 2c20 706f 7365  mkcube(0.2, pose
-00003080: 3d53 4533 2830 2c20 302c 2031 292c 2065  =SE3(0, 0, 1), e
-00003090: 6467 653d 5472 7565 290a 6361 6d2e 706c  dge=True).cam.pl
-000030a0: 6f74 5f77 6972 6566 7261 6d65 2858 2c20  ot_wireframe(X, 
-000030b0: 592c 205a 290a 6060 600a 0a21 5b50 6572  Y, Z).```..![Per
-000030c0: 7370 6563 7469 7665 2063 616d 6572 6120  spective camera 
-000030d0: 7669 6577 206f 6620 6375 6265 5d28 6874  view of cube](ht
-000030e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000030f0: 2f70 6574 6572 636f 726b 652f 6d61 6368  /petercorke/mach
-00003100: 696e 6576 6973 696f 6e2d 746f 6f6c 626f  inevision-toolbo
-00003110: 782d 7079 7468 6f6e 2f72 6177 2f6d 6173  x-python/raw/mas
-00003120: 7465 722f 6669 6773 2f63 7562 652e 706e  ter/figs/cube.pn
-00003130: 6729 0a0a 3c21 2d2d 2d6f 7220 7769 7468  g)..<!---or with
-00003140: 2061 2066 6973 6865 7965 2063 616d 6572   a fisheye camer
-00003150: 610a 0a60 6060 6d61 746c 6162 0a3e 3e20  a..```matlab.>> 
-00003160: 6361 6d20 3d20 4669 7368 4579 6543 616d  cam = FishEyeCam
-00003170: 6572 6128 276e 616d 6527 2c20 2766 6973  era('name', 'fis
-00003180: 6865 7965 272c 202e 2e2e 0a27 7072 6f6a  heye', ....'proj
-00003190: 6563 7469 6f6e 272c 2027 6571 7569 616e  ection', 'equian
-000031a0: 6775 6c61 7227 2c20 2e2e 2e0a 2770 6978  gular', ....'pix
-000031b0: 656c 272c 2031 3065 2d36 2c20 2e2e 2e0a  el', 10e-6, ....
-000031c0: 2772 6573 6f6c 7574 696f 6e27 2c20 5b31  'resolution', [1
-000031d0: 3238 3020 3130 3234 5d29 3b0a 3e3e 205b  280 1024]);.>> [
-000031e0: 582c 592c 5a5d 203d 206d 6b63 7562 6528  X,Y,Z] = mkcube(
-000031f0: 302e 322c 2027 6365 6e74 7265 272c 205b  0.2, 'centre', [
-00003200: 302e 322c 2030 2c20 302e 335d 2c20 2765  0.2, 0, 0.3], 'e
-00003210: 6467 6527 293b 0a3e 3e20 6361 6d2e 6d65  dge');.>> cam.me
-00003220: 7368 2858 2c20 592c 205a 293b 0a60 6060  sh(X, Y, Z);.```
-00003230: 0a21 5b46 6973 6865 7965 206c 656e 7320  .![Fisheye lens 
-00003240: 6361 6d65 7261 2076 6965 775d 2866 6967  camera view](fig
-00003250: 732f 6375 6265 5f66 6973 6865 7965 2e70  s/cube_fisheye.p
-00003260: 6e67 290a 0a0a 2323 2320 4275 6e64 6c65  ng)...### Bundle
-00003270: 2061 646a 7573 746d 656e 740a 2d2d 2d3e   adjustment.--->
-00003280: 0a0a 2323 2320 436f 6c6f 7220 7370 6163  ..### Color spac
-00003290: 650a 0a50 6c6f 7420 7468 6520 4349 4520  e..Plot the CIE 
-000032a0: 6368 726f 6d61 7469 6369 7479 2073 7061  chromaticity spa
-000032b0: 6365 0a0a 6060 6070 7974 686f 6e0a 706c  ce..```python.pl
-000032c0: 6f74 5f63 6872 6f6d 6174 6963 6974 795f  ot_chromaticity_
-000032d0: 6469 6167 7261 6d28 2278 7922 293b 0a70  diagram("xy");.p
-000032e0: 6c6f 745f 7370 6563 7472 616c 5f6c 6f63  lot_spectral_loc
-000032f0: 7573 2822 7879 2229 0a60 6060 0a0a 215b  us("xy").```..![
-00003300: 4349 4520 6368 726f 6d61 7469 6369 7479  CIE chromaticity
-00003310: 2073 7061 6365 5d28 6874 7470 733a 2f2f   space](https://
-00003320: 6769 7468 7562 2e63 6f6d 2f70 6574 6572  github.com/peter
-00003330: 636f 726b 652f 6d61 6368 696e 6576 6973  corke/machinevis
-00003340: 696f 6e2d 746f 6f6c 626f 782d 7079 7468  ion-toolbox-pyth
-00003350: 6f6e 2f72 6177 2f6d 6173 7465 722f 6669  on/raw/master/fi
-00003360: 6773 2f63 6f6c 6f72 7370 6163 652e 706e  gs/colorspace.pn
-00003370: 6729 0a0a 4c6f 6164 2074 6865 2073 7065  g)..Load the spe
-00003380: 6374 7275 6d20 6f66 2073 756e 6c69 6768  ctrum of sunligh
-00003390: 7420 6174 2074 6865 2045 6172 7468 2773  t at the Earth's
-000033a0: 2073 7572 6661 6365 2061 6e64 2063 6f6d   surface and com
-000033b0: 7075 7465 2074 6865 2043 4945 2078 7920  pute the CIE xy 
-000033c0: 6368 726f 6d61 7469 6369 7479 2063 6f6f  chromaticity coo
-000033d0: 7264 696e 6174 6573 0a0a 6060 6070 7974  rdinates..```pyt
-000033e0: 686f 6e0a 6e6d 203d 2031 652d 390a 6c61  hon.nm = 1e-9.la
-000033f0: 6d20 3d20 6e70 2e6c 696e 7370 6163 6528  m = np.linspace(
-00003400: 3430 302c 2037 3031 2c20 3529 202a 206e  400, 701, 5) * n
-00003410: 6d20 2320 7669 7369 626c 6520 6c69 6768  m # visible ligh
-00003420: 740a 7375 6e5f 6174 5f67 726f 756e 6420  t.sun_at_ground 
-00003430: 3d20 6c6f 6164 7370 6563 7472 756d 286c  = loadspectrum(l
-00003440: 616d 2c20 2273 6f6c 6172 2229 0a78 7920  am, "solar").xy 
-00003450: 3d20 6c61 6d62 6461 3278 7928 6c61 6d62  = lambda2xy(lamb
-00003460: 6461 2c20 7375 6e5f 6174 5f67 726f 756e  da, sun_at_groun
-00003470: 6429 0a70 7269 6e74 2878 7929 0a09 5b5b  d).print(xy)..[[
-00003480: 302e 3333 3237 3237 3938 2030 2e33 3435  0.33272798 0.345
-00003490: 3430 3133 205d 5d0a 7072 696e 7428 636f  4013 ]].print(co
-000034a0: 6c6f 726e 616d 6528 7879 2c20 2278 7922  lorname(xy, "xy"
-000034b0: 2929 0a09 6b68 616b 690a 6060 600a 0a23  ))..khaki.```..#
-000034c0: 2323 2048 6f75 6768 2074 7261 6e73 666f  ## Hough transfo
-000034d0: 726d 0a0a 6060 6070 7974 686f 6e0a 696d  rm..```python.im
-000034e0: 203d 2049 6d61 6765 2e52 6561 6428 2263   = Image.Read("c
-000034f0: 6875 7263 682e 706e 6722 2c20 6d6f 6e6f  hurch.png", mono
-00003500: 3d54 7275 6529 0a65 6467 6573 203d 2069  =True).edges = i
-00003510: 6d2e 6361 6e6e 7928 290a 6820 3d20 6564  m.canny().h = ed
-00003520: 6765 732e 486f 7567 6828 290a 6c69 6e65  ges.Hough().line
-00003530: 7320 3d20 682e 6c69 6e65 735f 7028 3130  s = h.lines_p(10
-00003540: 302c 206d 696e 6c69 6e65 6c65 6e67 7468  0, minlinelength
-00003550: 3d32 3030 2c20 6d61 786c 696e 6567 6170  =200, maxlinegap
-00003560: 3d35 2c20 7365 6564 3d30 290a 0a69 6d2e  =5, seed=0)..im.
-00003570: 6469 7370 2864 6172 6b65 6e3d 5472 7565  disp(darken=True
-00003580: 290a 682e 706c 6f74 5f6c 696e 6573 286c  ).h.plot_lines(l
-00003590: 696e 6573 2c20 2272 2d2d 2229 0a60 6060  ines, "r--").```
-000035a0: 0a0a 215b 486f 7567 6820 7472 616e 7366  ..![Hough transf
-000035b0: 6f72 6d5d 2868 7474 7073 3a2f 2f67 6974  orm](https://git
-000035c0: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
-000035d0: 6b65 2f6d 6163 6869 6e65 7669 7369 6f6e  ke/machinevision
-000035e0: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e2f  -toolbox-python/
-000035f0: 7261 772f 6d61 7374 6572 2f66 6967 732f  raw/master/figs/
-00003600: 686f 7567 682e 706e 6729 0a0a 2323 2320  hough.png)..### 
-00003610: 5355 5246 2066 6561 7475 7265 730a 0a57  SURF features..W
-00003620: 6520 6c6f 6164 2074 776f 2069 6d61 6765  e load two image
-00003630: 7320 616e 6420 636f 6d70 7574 6520 6120  s and compute a 
-00003640: 7365 7420 6f66 2053 5552 4620 6665 6174  set of SURF feat
-00003650: 7572 6573 2066 6f72 2065 6163 680a 0a60  ures for each..`
-00003660: 6060 7079 7468 6f6e 0a76 6965 7731 203d  ``python.view1 =
-00003670: 2049 6d61 6765 2e52 6561 6428 2265 6966   Image.Read("eif
-00003680: 6665 6c2d 312e 706e 6722 2c20 6d6f 6e6f  fel-1.png", mono
-00003690: 3d54 7275 6529 0a76 6965 7732 203d 2049  =True).view2 = I
-000036a0: 6d61 6765 2e52 6561 6428 2265 6966 6665  mage.Read("eiffe
-000036b0: 6c2d 322e 706e 6722 2c20 6d6f 6e6f 3d54  l-2.png", mono=T
-000036c0: 7275 6529 0a73 6631 203d 2076 6965 7731  rue).sf1 = view1
-000036d0: 2e53 4946 5428 290a 7366 3220 3d20 7669  .SIFT().sf2 = vi
-000036e0: 6577 322e 5349 4654 2829 0a60 6060 0a0a  ew2.SIFT().```..
-000036f0: 5765 2063 616e 206d 6174 6368 2066 6561  We can match fea
-00003700: 7475 7265 7320 6265 7477 6565 6e20 696d  tures between im
-00003710: 6167 6573 2062 6173 6564 2070 7572 656c  ages based purel
-00003720: 7920 6f6e 2074 6865 2073 696d 696c 6172  y on the similar
-00003730: 6974 7920 6f66 2074 6865 2066 6561 7475  ity of the featu
-00003740: 7265 732c 2061 6e64 2064 6973 706c 6179  res, and display
-00003750: 2074 6865 2063 6f72 7265 7370 6f6e 6465   the corresponde
-00003760: 6e63 6573 2066 6f75 6e64 0a0a 6060 6070  nces found..```p
-00003770: 7974 686f 6e0a 6d61 7463 6865 7320 3d20  ython.matches = 
-00003780: 7366 312e 6d61 7463 6828 7366 3229 0a70  sf1.match(sf2).p
-00003790: 7269 6e74 286d 6174 6368 6573 290a 3831  rint(matches).81
-000037a0: 3320 6d61 7463 6865 730a 6d61 7463 6865  3 matches.matche
-000037b0: 735b 313a 355d 2e74 6162 6c65 2829 0ae2  s[1:5].table()..
-000037c0: 948c e294 80e2 9480 e294 ace2 9480 e294  ................
-000037d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000037e0: e294 80e2 94ac e294 80e2 9480 e294 80e2  ................
-000037f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003800: 80e2 9480 e294 ace2 9480 e294 80e2 9480  ................
-00003810: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003820: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003830: 80e2 9480 e294 80e2 9480 e294 ace2 9480  ................
-00003840: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003850: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003860: 80e2 9480 e294 80e2 9480 e294 80e2 9490  ................
-00003870: 0ae2 9482 2320 e294 8220 696e 6c69 6572  ....# ... inlier
-00003880: 20e2 9482 2073 7472 656e 6774 6820 e294   ... strength ..
-00003890: 8220 2020 2020 2020 2020 2020 2020 2070  .              p
-000038a0: 3120 e294 8220 2020 2020 2020 2020 2020  1 ...           
-000038b0: 2020 7032 20e2 9482 0ae2 949c e294 80e2    p2 ...........
-000038c0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-000038d0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-000038e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000038f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003900: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003910: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003920: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003930: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-00003940: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003950: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003960: 80e2 9480 e294 80e2 94a4 0ae2 9482 3020  ..............0 
-00003970: e294 8220 2020 2020 2020 20e2 9482 2020  ...        ...  
-00003980: 2020 2032 362e 3420 e294 8220 2831 3131     26.4 ... (111
-00003990: 382e 362c 2031 3738 2e38 2920 e294 8220  8.6, 178.8) ... 
-000039a0: 2839 3532 2e35 2c20 3431 382e 3029 20e2  (952.5, 418.0) .
-000039b0: 9482 0ae2 9482 3120 e294 8220 2020 2020  ......1 ...     
-000039c0: 2020 20e2 9482 2020 2020 2032 382e 3220     ...     28.2 
-000039d0: e294 8220 2838 3230 2e36 2c20 3531 392e  ... (820.6, 519.
-000039e0: 3129 2020 e294 8220 2837 3038 2e31 2c20  1)  ... (708.1, 
-000039f0: 3730 312e 3629 20e2 9482 0ae2 9482 3220  701.6) .......2 
-00003a00: e294 8220 2020 2020 2020 20e2 9482 2020  ...        ...  
-00003a10: 2020 2032 392e 3620 e294 8220 2838 3031     29.6 ... (801
-00003a20: 2e31 2c20 3633 322e 3429 2020 e294 8220  .1, 632.4)  ... 
-00003a30: 2836 3934 2e31 2c20 3830 302e 3329 20e2  (694.1, 800.3) .
-00003a40: 9482 0ae2 9482 3320 e294 8220 2020 2020  ......3 ...     
-00003a50: 2020 20e2 9482 2020 2020 2033 322e 3420     ...     32.4 
-00003a60: e294 8220 2837 3436 2e30 2c20 3135 332e  ... (746.0, 153.
-00003a70: 3129 2020 e294 8220 2836 3434 2e35 2c20  1)  ... (644.5, 
-00003a80: 3339 322e 3229 20e2 9482 0ae2 9494 e294  392.2) .........
-00003a90: 80e2 9480 e294 b4e2 9480 e294 80e2 9480  ................
-00003aa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003ab0: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003ac0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003ad0: e294 b4e2 9480 e294 80e2 9480 e294 80e2  ................
-00003ae0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003af0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003b00: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
-00003b10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003b20: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003b30: e294 80e2 9480 e294 80e2 9498 0a60 6060  .............```
-00003b40: 0a0a 7768 6572 6520 7765 2068 6176 6520  ..where we have 
-00003b50: 6469 7370 6c61 7965 6420 7468 6520 6665  displayed the fe
-00003b60: 6174 7572 6520 636f 6f72 6469 6e61 7465  ature coordinate
-00003b70: 7320 666f 7220 666f 7572 2063 6f72 7265  s for four corre
-00003b80: 7370 6f6e 6465 6e63 6573 2e0a 0a57 6520  spondences...We 
-00003b90: 6361 6e20 616c 736f 2064 6973 706c 6179  can also display
-00003ba0: 2074 6865 2063 6f72 7265 7370 6f6e 6465   the corresponde
-00003bb0: 6e63 6573 2067 7261 7068 6963 616c 6c79  nces graphically
-00003bc0: 0a0a 6060 6070 7974 686f 6e0a 6d61 7463  ..```python.matc
-00003bd0: 6865 732e 7375 6273 6574 2831 3030 292e  hes.subset(100).
-00003be0: 706c 6f74 2822 7722 290a 6060 600a 0a69  plot("w").```..i
-00003bf0: 6e20 7468 6973 2063 6173 652c 2061 2073  n this case, a s
-00003c00: 7562 7365 7420 6f66 2031 3030 2f38 3133  ubset of 100/813
-00003c10: 206f 6620 7468 6520 636f 7272 6573 706f   of the correspo
-00003c20: 6e64 656e 6365 732e 0a0a 215b 4665 6174  ndences...![Feat
-00003c30: 7572 6520 6d61 7463 6869 6e67 5d28 6874  ure matching](ht
-00003c40: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003c50: 2f70 6574 6572 636f 726b 652f 6d61 6368  /petercorke/mach
-00003c60: 696e 6576 6973 696f 6e2d 746f 6f6c 626f  inevision-toolbo
-00003c70: 782d 7079 7468 6f6e 2f72 6177 2f6d 6173  x-python/raw/mas
-00003c80: 7465 722f 6669 6773 2f6d 6174 6368 696e  ter/figs/matchin
-00003c90: 672e 706e 6729 0a0a 436c 6561 726c 7920  g.png)..Clearly 
-00003ca0: 7468 6572 6520 6172 6520 736f 6d65 2062  there are some b
-00003cb0: 6164 206d 6174 6368 6573 2068 6572 652c  ad matches here,
-00003cc0: 2062 7574 2077 6520 7765 2063 616e 2075   but we we can u
-00003cd0: 7365 2052 414e 5341 4320 616e 6420 7468  se RANSAC and th
-00003ce0: 6520 6570 6970 6f6c 6172 2063 6f6e 7374  e epipolar const
-00003cf0: 7261 696e 7420 696d 706c 6965 6420 6279  raint implied by
-00003d00: 2074 6865 2066 756e 6461 6d65 6e74 616c   the fundamental
-00003d10: 206d 6174 7269 7820 746f 2065 7374 696d   matrix to estim
-00003d20: 6174 6520 7468 6520 6675 6e64 616d 656e  ate the fundamen
-00003d30: 7461 6c20 6d61 7472 6978 2061 6e64 2063  tal matrix and c
-00003d40: 6c61 7373 6966 7920 636f 7272 6573 706f  lassify correspo
-00003d50: 6e64 656e 6365 7320 6173 2069 6e6c 6965  ndences as inlie
-00003d60: 7273 206f 7220 6f75 746c 6965 7273 0a0a  rs or outliers..
-00003d70: 6060 6070 7974 686f 6e0a 462c 2072 6573  ```python.F, res
-00003d80: 6964 203d 206d 6174 6368 6573 2e65 7374  id = matches.est
-00003d90: 696d 6174 6528 4365 6e74 7261 6c43 616d  imate(CentralCam
-00003da0: 6572 612e 706f 696e 7473 3246 2c20 6d65  era.points2F, me
-00003db0: 7468 6f64 3d22 7261 6e73 6163 222c 2063  thod="ransac", c
-00003dc0: 6f6e 6669 6465 6e63 653d 302e 3939 2c20  onfidence=0.99, 
-00003dd0: 7365 6564 3d30 290a 7072 696e 7428 4629  seed=0).print(F)
-00003de0: 0a61 7272 6179 285b 5b31 2e30 3333 652d  .array([[1.033e-
-00003df0: 3038 2c20 2d33 2e37 3939 652d 3036 2c20  08, -3.799e-06, 
-00003e00: 302e 3030 3236 3738 5d2c 0a20 2020 2020  0.002678],.     
-00003e10: 2020 5b33 2e36 3638 652d 3036 2c20 312e    [3.668e-06, 1.
-00003e20: 3231 3765 2d30 372c 202d 302e 3030 3430  217e-07, -0.0040
-00003e30: 3333 5d2c 0a20 2020 2020 2020 5b2d 302e  33],.       [-0.
-00003e40: 3030 3331 392c 2030 2e30 3033 3433 362c  00319, 0.003436,
-00003e50: 2020 2020 2020 2020 315d 5d29 0a70 7269          1]]).pri
-00003e60: 6e74 2872 6573 6964 290a 302e 3034 3035  nt(resid).0.0405
-00003e70: 0a0a 496d 6167 652e 4873 7461 636b 2828  ..Image.Hstack((
-00003e80: 7669 6577 312c 2076 6965 7732 2929 2e64  view1, view2)).d
-00003e90: 6973 7028 290a 6d61 7463 6865 732e 696e  isp().matches.in
-00003ea0: 6c69 6572 732e 7375 6273 6574 2831 3030  liers.subset(100
-00003eb0: 292e 706c 6f74 2822 6722 2c20 6178 3d70  ).plot("g", ax=p
-00003ec0: 6c74 2e67 6361 2829 290a 6d61 7463 6865  lt.gca()).matche
-00003ed0: 732e 6f75 746c 6965 7273 2e73 7562 7365  s.outliers.subse
-00003ee0: 7428 3130 3029 2e70 6c6f 7428 2272 222c  t(100).plot("r",
-00003ef0: 2061 783d 706c 742e 6763 6128 2929 0a60   ax=plt.gca()).`
-00003f00: 6060 0a0a 7768 6572 6520 6772 6565 6e20  ``..where green 
-00003f10: 6c69 6e65 7320 7368 6f77 2063 6f72 7265  lines show corre
-00003f20: 6374 2063 6f72 7265 7370 6f6e 6465 6e63  ct correspondenc
-00003f30: 6573 2028 696e 6c69 6572 7329 2061 6e64  es (inliers) and
-00003f40: 2072 6564 206c 696e 6573 2073 686f 7720   red lines show 
-00003f50: 6261 6420 636f 7272 6573 706f 6e64 656e  bad corresponden
-00003f60: 6365 7320 286f 7574 6c69 6572 7329 0a0a  ces (outliers)..
-00003f70: 215b 4665 6174 7572 6520 6d61 7463 6869  ![Feature matchi
-00003f80: 6e67 2061 6674 6572 2052 414e 5341 435d  ng after RANSAC]
-00003f90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003fa0: 636f 6d2f 7065 7465 7263 6f72 6b65 2f6d  com/petercorke/m
-00003fb0: 6163 6869 6e65 7669 7369 6f6e 2d74 6f6f  achinevision-too
-00003fc0: 6c62 6f78 2d70 7974 686f 6e2f 7261 772f  lbox-python/raw/
-00003fd0: 6d61 7374 6572 2f66 6967 732f 6d61 7463  master/figs/matc
-00003fe0: 6869 6e67 5f72 616e 7361 632e 706e 6729  hing_ransac.png)
-00003ff0: 0a0a 2320 4869 7374 6f72 790a 0a54 6869  ..# History..Thi
-00004000: 7320 7061 636b 6167 6520 6361 6e20 6265  s package can be
-00004010: 2063 6f6e 7369 6465 7265 6420 6173 2061   considered as a
-00004020: 2050 7974 686f 6e20 7665 7273 696f 6e20   Python version 
-00004030: 6f66 2074 6865 205b 4d61 6368 696e 6520  of the [Machine 
-00004040: 5669 7369 6f6e 0a54 6f6f 6c62 6f78 2066  Vision.Toolbox f
-00004050: 6f72 204d 4154 4c41 425d 2829 2e20 5468  or MATLAB](). Th
-00004060: 6174 2054 6f6f 6c62 6f78 2c20 6e6f 7720  at Toolbox, now 
-00004070: 7175 6974 6520 6f6c 642c 2069 7320 6120  quite old, is a 
-00004080: 636f 6c6c 6563 7469 6f6e 206f 6620 4d41  collection of MA
-00004090: 544c 4142 0a66 756e 6374 696f 6e73 2061  TLAB.functions a
-000040a0: 6e64 2063 6c61 7373 6573 2074 6861 7420  nd classes that 
-000040b0: 7375 7070 6f72 7465 6420 7468 6520 6669  supported the fi
-000040c0: 7273 7420 7477 6f20 6564 6974 696f 6e73  rst two editions
-000040d0: 206f 6620 7468 6520 526f 626f 7469 6373   of the Robotics
-000040e0: 2c0a 5669 7369 6f6e 2026 2043 6f6e 7472  ,.Vision & Contr
-000040f0: 6f6c 2062 6f6f 6b2e 2049 7420 6973 2061  ol book. It is a
-00004100: 2073 6f6d 6577 6861 7420 6563 6c65 6374   somewhat eclect
-00004110: 6963 2063 6f6c 6c65 6374 696f 6e20 7265  ic collection re
-00004120: 666c 6563 7469 6e67 206d 790a 7065 7273  flecting my.pers
-00004130: 6f6e 616c 2069 6e74 6572 6573 7420 696e  onal interest in
-00004140: 2061 7265 6173 206f 6620 7068 6f74 6f6d   areas of photom
-00004150: 6574 7279 2c20 7068 6f74 6f67 7261 6d6d  etry, photogramm
-00004160: 6574 7279 2c20 636f 6c6f 7269 6d65 7472  etry, colorimetr
-00004170: 792e 2049 740a 696e 636c 7564 6573 206f  y. It.includes o
-00004180: 7665 7220 3130 3020 6675 6e63 7469 6f6e  ver 100 function
-00004190: 7320 7370 616e 6e69 6e67 206f 7065 7261  s spanning opera
-000041a0: 7469 6f6e 7320 7375 6368 2061 7320 696d  tions such as im
-000041b0: 6167 6520 6669 6c65 2072 6561 6469 6e67  age file reading
-000041c0: 2061 6e64 0a77 7269 7469 6e67 2c20 6163   and.writing, ac
-000041d0: 7175 6973 6974 696f 6e2c 2064 6973 706c  quisition, displ
-000041e0: 6179 2c20 6669 6c74 6572 696e 672c 2062  ay, filtering, b
-000041f0: 6c6f 622c 2070 6f69 6e74 2061 6e64 206c  lob, point and l
-00004200: 696e 6520 6665 6174 7572 650a 6578 7472  ine feature.extr
-00004210: 6163 7469 6f6e 2c20 6d61 7468 656d 6174  action, mathemat
-00004220: 6963 616c 206d 6f72 7068 6f6c 6f67 792c  ical morphology,
-00004230: 2068 6f6d 6f67 7261 7068 6965 732c 2076   homographies, v
-00004240: 6973 7561 6c20 4a61 636f 6269 616e 732c  isual Jacobians,
-00004250: 2063 616d 6572 610a 6361 6c69 6272 6174   camera.calibrat
-00004260: 696f 6e20 616e 6420 636f 6c6f 7220 7370  ion and color sp
-00004270: 6163 6520 636f 6e76 6572 7369 6f6e 2e0a  ace conversion..
-00004280: 0a54 6869 7320 5079 7468 6f6e 2076 6572  .This Python ver
-00004290: 7369 6f6e 2064 6966 6665 7273 2069 6e20  sion differs in 
-000042a0: 7573 696e 6720 616e 206f 626a 6563 7420  using an object 
-000042b0: 746f 2065 6e63 6170 7375 6c61 7465 2074  to encapsulate t
-000042c0: 6865 2070 6978 656c 2064 6174 6120 616e  he pixel data an
-000042d0: 640a 696d 6167 6520 6d65 7461 6461 7461  d.image metadata
-000042e0: 2c20 7261 7468 6572 2074 6861 6e20 6a75  , rather than ju
-000042f0: 7374 2061 206e 6174 6976 6520 6f62 6a65  st a native obje
-00004300: 6374 2068 6f6c 6469 6e67 2070 6978 656c  ct holding pixel
-00004310: 2064 6174 612e 2054 6865 206d 616e 790a   data. The many.
-00004320: 6675 6e63 7469 6f6e 7320 6265 636f 6d65  functions become
-00004330: 206d 6574 686f 6473 206f 6620 7468 6520   methods of the 
-00004340: 696d 6167 6520 6f62 6a65 6374 2077 6869  image object whi
-00004350: 6368 2072 6564 7563 6573 206e 616d 6573  ch reduces names
-00004360: 7061 6365 2070 6f6c 6c75 7469 6f6e 732c  pace pollutions,
-00004370: 0a61 6e64 2061 6c6c 6f77 7320 7468 6520  .and allows the 
-00004380: 6561 7379 2065 7870 7265 7373 696f 6e20  easy expression 
-00004390: 6f66 2073 6571 7565 6e74 6961 6c20 6f70  of sequential op
-000043a0: 6572 6174 696f 6e73 2075 7369 6e67 2022  erations using "
-000043b0: 646f 7420 6368 6169 6e69 6e67 222e 0a0a  dot chaining"...
-000043c0: 5468 6520 6669 7273 7420 7665 7273 696f  The first versio
-000043d0: 6e20 7761 7320 6372 6561 7465 6420 6279  n was created by
-000043e0: 2044 6f72 6961 6e20 5473 6169 2064 7572   Dorian Tsai dur
-000043f0: 696e 6720 3230 3230 2c20 616e 6420 6261  ing 2020, and ba
-00004400: 7365 6420 6f6e 2074 6865 0a4d 4154 4c41  sed on the.MATLA
-00004410: 4220 7665 7273 696f 6e2e 2020 5468 6174  B version.  That
-00004420: 2077 6f72 6b20 7761 7320 6675 6e64 6564   work was funded
-00004430: 2062 7920 616e 2041 7573 7472 616c 6961   by an Australia
-00004440: 6e20 556e 6976 6572 7369 7479 2054 6561  n University Tea
-00004450: 6368 6572 206f 660a 7468 6520 7965 6172  cher of.the year
-00004460: 2061 7761 7264 2028 3230 3137 2920 746f   award (2017) to
-00004470: 2050 6574 6572 2043 6f72 6b65 2e0a        Peter Corke..
+00002940: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
+00002950: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002960: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002970: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
+00002980: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002990: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
+000029a0: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
+000029b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000029c0: 80e2 9480 e294 ace2 9480 e294 80e2 9480  ................
+000029d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000029e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000029f0: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002a00: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
+00002a10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002a20: 80e2 9480 e294 900a 09e2 9482 6964 20e2  ............id .
+00002a30: 9482 2070 6172 656e 7420 e294 8220 2020  .. parent ...   
+00002a40: 2020 2063 656e 7472 6f69 6420 e294 8220     centroid ... 
+00002a50: 2020 2020 6172 6561 20e2 9482 2074 6f75      area ... tou
+00002a60: 6368 20e2 9482 2020 7065 7269 6d20 e294  ch ...  perim ..
+00002a70: 8220 6369 7263 756c 6172 6974 7920 e294  . circularity ..
+00002a80: 8220 6f72 6965 6e74 20e2 9482 2061 7370  . orient ... asp
+00002a90: 6563 7420 e294 820a 09e2 949c e294 80e2  ect ............
+00002aa0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+00002ab0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002ac0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+00002ad0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002ae0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002af0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+00002b00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002b10: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+00002b20: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+00002b30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002b40: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+00002b50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002b60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002b70: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002b80: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+00002b90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002ba0: 80e2 9480 e294 a40a 09e2 9482 2030 20e2  ............ 0 .
+00002bb0: 9482 2020 2020 2020 3120 e294 8220 2038  ..      1 ...  8
+00002bc0: 3938 2e38 2c20 3732 352e 3320 e294 8220  98.8, 725.3 ... 
+00002bd0: 312e 3635 652b 3035 20e2 9482 2046 616c  1.65e+05 ... Fal
+00002be0: 7365 20e2 9482 2032 3232 302e 3020 e294  se ... 2220.0 ..
+00002bf0: 8220 2020 2020 2020 302e 3436 3720 e294  .       0.467 ..
+00002c00: 8220 2038 362e 37c2 b020 e294 8220 2030  .  86.7.. ...  0
+00002c10: 2e37 3534 20e2 9482 0a09 e294 8220 3120  .754 ........ 1 
+00002c20: e294 8220 2020 2020 2032 20e2 9482 2031  ...      2 ... 1
+00002c30: 3032 352e 302c 2038 3133 2e37 20e2 9482  025.0, 813.7 ...
+00002c40: 2031 2e30 3665 2b30 3520 e294 8220 4661   1.06e+05 ... Fa
+00002c50: 6c73 6520 e294 8220 3133 3837 2e39 20e2  lse ... 1387.9 .
+00002c60: 9482 2020 2020 2020 2030 2e37 3639 20e2  ..       0.769 .
+00002c70: 9482 202d 3838 2e39 c2b0 20e2 9482 2020  .. -88.9.. ...  
+00002c80: 302e 3733 3920 e294 820a 09e2 9482 2032  0.739 ........ 2
+00002c90: 20e2 9482 2020 2020 202d 3120 e294 8220   ...     -1 ... 
+00002ca0: 2039 3338 2e31 2c20 3835 352e 3220 e294   938.1, 855.2 ..
+00002cb0: 8220 312e 3732 652b 3034 20e2 9482 2046  . 1.72e+04 ... F
+00002cc0: 616c 7365 20e2 9482 2020 3439 302e 3720  alse ...  490.7 
+00002cd0: e294 8220 2020 2020 2020 312e 3030 3120  ...       1.001 
+00002ce0: e294 8220 2038 382e 37c2 b020 e294 8220  ...  88.7.. ... 
+00002cf0: 2030 2e38 3632 20e2 9482 0a09 e294 8220   0.862 ........ 
+00002d00: 3320 e294 8220 2020 2020 2d31 20e2 9482  3 ...     -1 ...
+00002d10: 2020 3938 382e 312c 2036 3937 2e32 20e2    988.1, 697.2 .
+00002d20: 9482 2031 2e32 3165 2b30 3420 e294 8220  .. 1.21e+04 ... 
+00002d30: 4661 6c73 6520 e294 8220 2034 3132 2e35  False ...  412.5
+00002d40: 20e2 9482 2020 2020 2020 2030 2e39 3934   ...       0.994
+00002d50: 20e2 9482 202d 3837 2e38 c2b0 20e2 9482   ... -87.8.. ...
+00002d60: 2020 302e 3830 3920 e294 820a 09e2 9482    0.809 ........
+00002d70: 2034 20e2 9482 2020 2020 202d 3120 e294   4 ...     -1 ..
+00002d80: 8220 2038 3436 2e30 2c20 3531 312e 3720  .  846.0, 511.7 
+00002d90: e294 8220 312e 3735 652b 3034 20e2 9482  ... 1.75e+04 ...
+00002da0: 2046 616c 7365 20e2 9482 2020 3439 362e   False ...  496.
+00002db0: 3920 e294 8220 2020 2020 2020 302e 3939  9 ...       0.99
+00002dc0: 3220 e294 8220 2d39 302e 30c2 b020 e294  2 ... -90.0.. ..
+00002dd0: 8220 2030 2e37 3738 20e2 9482 0a09 e294  .  0.778 .......
+00002de0: 8220 3520 e294 8220 2020 2020 2036 20e2  . 5 ...      6 .
+00002df0: 9482 2020 3239 312e 372c 2033 3737 2e38  ..  291.7, 377.8
+00002e00: 20e2 9482 2020 312e 3765 2b30 3520 e294   ...  1.7e+05 ..
+00002e10: 8220 4661 6c73 6520 e294 8220 3137 3132  . False ... 1712
+00002e20: 2e36 20e2 9482 2020 2020 2020 2030 2e38  .6 ...       0.8
+00002e30: 3130 20e2 9482 202d 3835 2e33 c2b0 20e2  10 ... -85.3.. .
+00002e40: 9482 2020 302e 3736 3720 e294 820a 09e2  ..  0.767 ......
+00002e50: 9482 2036 20e2 9482 2020 2020 202d 3120  .. 6 ...     -1 
+00002e60: e294 8220 2033 3132 2e37 2c20 3437 322e  ...  312.7, 472.
+00002e70: 3120 e294 8220 312e 3735 652b 3034 20e2  1 ... 1.75e+04 .
+00002e80: 9482 2046 616c 7365 20e2 9482 2020 3439  .. False ...  49
+00002e90: 352e 3520 e294 8220 2020 2020 2020 302e  5.5 ...       0.
+00002ea0: 3939 3720 e294 8220 2d38 392e 39c2 b020  997 ... -89.9.. 
+00002eb0: e294 8220 2030 2e37 3737 20e2 9482 0a09  ...  0.777 .....
+00002ec0: e294 8220 3720 e294 8220 2020 2020 2d31  ... 7 ...     -1
+00002ed0: 20e2 9482 2020 3234 312e 392c 2032 3435   ...  241.9, 245
+00002ee0: 2e30 20e2 9482 2031 2e37 3565 2b30 3420  .0 ... 1.75e+04 
+00002ef0: e294 8220 4661 6c73 6520 e294 8220 2034  ... False ...  4
+00002f00: 3936 2e39 20e2 9482 2020 2020 2020 2030  96.9 ...       0
+00002f10: 2e39 3932 20e2 9482 202d 3930 2e30 c2b0  .992 ... -90.0..
+00002f20: 20e2 9482 2020 302e 3737 3720 e294 820a   ...  0.777 ....
+00002f30: 09e2 9482 2038 20e2 9482 2020 2020 2020  .... 8 ...      
+00002f40: 3920 e294 8220 3132 3238 2e30 2c20 3235  9 ... 1228.0, 25
+00002f50: 342e 3320 e294 8220 382e 3134 652b 3034  4.3 ... 8.14e+04
+00002f60: 20e2 9482 2046 616c 7365 20e2 9482 2031   ... False ... 1
+00002f70: 3231 352e 3220 e294 8220 2020 2020 2020  215.2 ...       
+00002f80: 302e 3737 3120 e294 8220 2d37 372e 32c2  0.771 ... -77.2.
+00002f90: b020 e294 8220 2030 2e37 3133 20e2 9482  . ...  0.713 ...
+00002fa0: 0a09 e294 8220 3920 e294 8220 2020 2020  ..... 9 ...     
+00002fb0: 2d31 20e2 9482 2031 3232 352e 322c 2032  -1 ... 1225.2, 2
+00002fc0: 3230 2e30 20e2 9482 2031 2e37 3565 2b30  20.0 ... 1.75e+0
+00002fd0: 3420 e294 8220 4661 6c73 6520 e294 8220  4 ... False ... 
+00002fe0: 2034 3936 2e39 20e2 9482 2020 2020 2020   496.9 ...      
+00002ff0: 2030 2e39 3932 20e2 9482 202d 3930 2e30   0.992 ... -90.0
+00003000: c2b0 20e2 9482 2020 302e 3737 3720 e294  .. ...  0.777 ..
+00003010: 820a 09e2 9494 e294 80e2 9480 e294 80e2  ................
+00003020: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003030: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
+00003040: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003050: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003060: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
+00003070: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003080: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
+00003090: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000030a0: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
+000030b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000030c0: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000030d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000030e0: 9480 e294 80e2 9480 e294 b4e2 9480 e294  ................
+000030f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003100: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
+00003110: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003120: 980a 6060 600a 0a57 6520 6361 6e20 6469  ..```..We can di
+00003130: 7370 6c61 7920 6120 6c61 6265 6c20 696d  splay a label im
+00003140: 6167 652c 2077 6865 7265 2074 6865 2076  age, where the v
+00003150: 616c 7565 206f 6620 6561 6368 2070 6978  alue of each pix
+00003160: 656c 2069 7320 7468 6520 6c61 6265 6c20  el is the label 
+00003170: 6f66 2074 6865 2062 6c6f 6220 7468 6174  of the blob that
+00003180: 2074 6865 2070 6978 656c 0a62 656c 6f6e   the pixel.belon
+00003190: 6773 2074 6f2c 2074 6865 2060 6964 6020  gs to, the `id` 
+000031a0: 6174 7472 6962 7574 650a 0a60 6060 7079  attribute..```py
+000031b0: 7468 6f6e 0a6c 6162 656c 7320 3d20 626c  thon.labels = bl
+000031c0: 6f62 732e 6c61 6265 6c5f 696d 6167 6528  obs.label_image(
+000031d0: 290a 6c61 6265 6c73 2e64 6973 7028 636f  ).labels.disp(co
+000031e0: 6c6f 726d 6170 3d22 7669 7269 6469 7322  lormap="viridis"
+000031f0: 2c20 6e63 6f6c 6f72 733d 6c65 6e28 626c  , ncolors=len(bl
+00003200: 6f62 7329 2c20 636f 6c6f 7262 6172 3d64  obs), colorbar=d
+00003210: 6963 7428 7368 7269 6e6b 3d30 2e38 2c20  ict(shrink=0.8, 
+00003220: 6173 7065 6374 3d32 302a 302e 3829 290a  aspect=20*0.8)).
+00003230: 6060 600a 0a21 5b46 616c 7365 2063 6f6c  ```..![False col
+00003240: 6f72 206c 6162 656c 2069 6d61 6765 5d28  or label image](
+00003250: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003260: 6f6d 2f70 6574 6572 636f 726b 652f 6d61  om/petercorke/ma
+00003270: 6368 696e 6576 6973 696f 6e2d 746f 6f6c  chinevision-tool
+00003280: 626f 782d 7079 7468 6f6e 2f72 6177 2f6d  box-python/raw/m
+00003290: 6173 7465 722f 6669 6773 2f6d 756c 7469  aster/figs/multi
+000032a0: 5f6c 6162 656c 6c65 642e 706e 6729 0a0a  _labelled.png)..
+000032b0: 5765 2063 616e 2061 6c73 6f20 7468 696e  We can also thin
+000032c0: 6b20 6f66 2074 6865 2062 6c6f 6273 2066  k of the blobs f
+000032d0: 6f72 6d69 6e67 2061 2068 6965 6172 6368  orming a hiearch
+000032e0: 7920 616e 6420 7468 6174 2072 656c 6174  y and that relat
+000032f0: 696f 6e73 6869 7020 6973 2072 6566 6c65  ionship is refle
+00003300: 6374 6564 2069 6e20 7468 6520 6070 6172  cted in the `par
+00003310: 656e 7460 2061 6e64 2060 6368 696c 6472  ent` and `childr
+00003320: 656e 6020 6174 7472 6962 7574 6573 206f  en` attributes o
+00003330: 6620 7468 6520 626c 6f62 732e 0a57 6520  f the blobs..We 
+00003340: 6361 6e20 616c 736f 2065 7870 7265 7373  can also express
+00003350: 2069 7420 6173 2061 2064 6972 6563 7465   it as a directe
+00003360: 6420 6772 6170 680a 0a60 6060 7079 7468  d graph..```pyth
+00003370: 6f6e 0a62 6c6f 6273 2e64 6f74 6669 6c65  on.blobs.dotfile
+00003380: 2873 686f 773d 5472 7565 290a 6060 600a  (show=True).```.
+00003390: 0a21 5b42 6c6f 6220 6869 6572 6172 6368  .![Blob hierarch
+000033a0: 7920 6173 2061 2067 7261 7068 5d28 6874  y as a graph](ht
+000033b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000033c0: 2f70 6574 6572 636f 726b 652f 6d61 6368  /petercorke/mach
+000033d0: 696e 6576 6973 696f 6e2d 746f 6f6c 626f  inevision-toolbo
+000033e0: 782d 7079 7468 6f6e 2f72 6177 2f6d 6173  x-python/raw/mas
+000033f0: 7465 722f 6669 6773 2f62 6c6f 6273 5f67  ter/figs/blobs_g
+00003400: 7261 7068 2e70 6e67 290a 0a23 2323 2043  raph.png)..### C
+00003410: 616d 6572 6120 6d6f 6465 6c6c 696e 670a  amera modelling.
+00003420: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00003430: 6d61 6368 696e 6576 6973 696f 6e74 6f6f  machinevisiontoo
+00003440: 6c62 6f78 2069 6d70 6f72 7420 4365 6e74  lbox import Cent
+00003450: 7261 6c43 616d 6572 610a 6361 6d20 3d20  ralCamera.cam = 
+00003460: 4365 6e74 7261 6c43 616d 6572 6128 663d  CentralCamera(f=
+00003470: 302e 3031 352c 2072 686f 3d31 3065 2d36  0.015, rho=10e-6
+00003480: 2c20 696d 6167 6573 697a 653d 5b31 3238  , imagesize=[128
+00003490: 302c 2031 3032 345d 2c20 7070 3d5b 3634  0, 1024], pp=[64
+000034a0: 302c 2035 3132 5d2c 206e 616d 653d 226d  0, 512], name="m
+000034b0: 7963 616d 6572 6122 290a 7072 696e 7428  ycamera").print(
+000034c0: 6361 6d29 0a20 2020 2020 2020 2020 2020  cam).           
+000034d0: 4e61 6d65 3a20 6d79 6361 6d65 7261 205b  Name: mycamera [
+000034e0: 4365 6e74 7261 6c43 616d 6572 615d 0a20  CentralCamera]. 
+000034f0: 2020 2020 7069 7865 6c20 7369 7a65 3a20      pixel size: 
+00003500: 3165 2d30 3520 7820 3165 2d30 350a 2020  1e-05 x 1e-05.  
+00003510: 2020 2069 6d61 6765 2073 697a 653a 2031     image size: 1
+00003520: 3238 3020 7820 3130 3234 0a20 2020 2020  280 x 1024.     
+00003530: 2020 2020 2020 706f 7365 3a20 7420 3d20        pose: t = 
+00003540: 302c 2030 2c20 303b 2072 7079 2f79 787a  0, 0, 0; rpy/yxz
+00003550: 203d 2030 c2b0 2c20 30c2 b02c 2030 c2b0   = 0.., 0.., 0..
+00003560: 0a20 2020 7072 696e 6369 7061 6c20 7074  .   principal pt
+00003570: 3a20 5b20 2020 2020 3634 3020 2020 2020  : [     640     
+00003580: 2035 3132 5d0a 2020 2066 6f63 616c 206c   512].   focal l
+00003590: 656e 6774 683a 205b 2020 2030 2e30 3135  ength: [   0.015
+000035a0: 2020 2020 302e 3031 355d 0a60 6060 0a0a      0.015].```..
+000035b0: 616e 6420 6974 7320 696e 7472 696e 7369  and its intrinsi
+000035c0: 6320 7061 7261 6d65 7465 7273 2061 7265  c parameters are
+000035d0: 0a0a 6060 6070 7974 686f 6e0a 7072 696e  ..```python.prin
+000035e0: 7428 6361 6d2e 4b29 0a09 5b5b 312e 3530  t(cam.K)..[[1.50
+000035f0: 652b 3033 2030 2e30 3065 2b30 3020 362e  e+03 0.00e+00 6.
+00003600: 3430 652b 3032 5d0a 0920 5b30 2e30 3065  40e+02].. [0.00e
+00003610: 2b30 3020 312e 3530 652b 3033 2035 2e31  +00 1.50e+03 5.1
+00003620: 3265 2b30 325d 0a09 205b 302e 3030 652b  2e+02].. [0.00e+
+00003630: 3030 2030 2e30 3065 2b30 3020 312e 3030  00 0.00e+00 1.00
+00003640: 652b 3030 5d5d 0a60 6060 0a0a 5765 2063  e+00]].```..We c
+00003650: 616e 2064 6566 696e 6520 616e 2061 7262  an define an arb
+00003660: 6974 7261 7279 2070 6f69 6e74 2069 6e20  itrary point in 
+00003670: 7468 6520 776f 726c 640a 0a60 6060 7079  the world..```py
+00003680: 7468 6f6e 0a50 203d 205b 302e 332c 2030  thon.P = [0.3, 0
+00003690: 2e34 2c20 332e 305d 0a60 6060 0a0a 616e  .4, 3.0].```..an
+000036a0: 6420 7468 656e 2070 726f 6a65 6374 2069  d then project i
+000036b0: 7420 696e 746f 2074 6865 2063 616d 6572  t into the camer
+000036c0: 610a 0a60 6060 7079 7468 6f6e 0a70 203d  a..```python.p =
+000036d0: 2063 616d 2e70 726f 6a65 6374 2850 290a   cam.project(P).
+000036e0: 7072 696e 7428 7029 0a09 5b37 3930 2e20  print(p)..[790. 
+000036f0: 3731 322e 5d0a 6060 600a 0a77 6869 6368  712.].```..which
+00003700: 2069 7320 7468 6520 636f 7272 6573 706f   is the correspo
+00003710: 6e64 696e 6720 636f 6f72 6469 6e61 7465  nding coordinate
+00003720: 2069 6e20 7069 7865 6c73 2e20 4966 2077   in pixels. If w
+00003730: 6520 7368 6966 7420 7468 6520 6361 6d65  e shift the came
+00003740: 7261 2073 6c69 6768 746c 7920 7468 6520  ra slightly the 
+00003750: 696d 6167 6520 706c 616e 6520 636f 6f72  image plane coor
+00003760: 6469 6e61 7465 2077 696c 6c20 616c 736f  dinate will also
+00003770: 2063 6861 6e67 650a 0a60 6060 7079 7468   change..```pyth
+00003780: 6f6e 0a70 203d 2063 616d 2e70 726f 6a65  on.p = cam.proje
+00003790: 6374 2850 2c20 543d 5345 3328 302e 312c  ct(P, T=SE3(0.1,
+000037a0: 2030 2c20 3029 2029 0a70 7269 6e74 2870   0, 0) ).print(p
+000037b0: 290a 5b37 3430 2e20 3731 322e 5d0a 6060  ).[740. 712.].``
+000037c0: 600a 0a57 6520 6361 6e20 6465 6669 6e65  `..We can define
+000037d0: 2061 6e20 6564 6765 2d62 6173 6564 2063   an edge-based c
+000037e0: 7562 6520 6d6f 6465 6c20 616e 6420 7072  ube model and pr
+000037f0: 6f6a 6563 7420 6974 2069 6e74 6f20 7468  oject it into th
+00003800: 6520 6361 6d65 7261 2773 2069 6d61 6765  e camera's image
+00003810: 2070 6c61 6e65 0a0a 6060 6070 7974 686f   plane..```pytho
+00003820: 6e0a 6672 6f6d 2073 7061 7469 616c 6d61  n.from spatialma
+00003830: 7468 2069 6d70 6f72 7420 5345 330a 582c  th import SE3.X,
+00003840: 2059 2c20 5a20 3d20 6d6b 6375 6265 2830   Y, Z = mkcube(0
+00003850: 2e32 2c20 706f 7365 3d53 4533 2830 2c20  .2, pose=SE3(0, 
+00003860: 302c 2031 292c 2065 6467 653d 5472 7565  0, 1), edge=True
+00003870: 290a 6361 6d2e 706c 6f74 5f77 6972 6566  ).cam.plot_wiref
+00003880: 7261 6d65 2858 2c20 592c 205a 290a 6060  rame(X, Y, Z).``
+00003890: 600a 0a21 5b50 6572 7370 6563 7469 7665  `..![Perspective
+000038a0: 2063 616d 6572 6120 7669 6577 206f 6620   camera view of 
+000038b0: 6375 6265 5d28 6874 7470 733a 2f2f 6769  cube](https://gi
+000038c0: 7468 7562 2e63 6f6d 2f70 6574 6572 636f  thub.com/peterco
+000038d0: 726b 652f 6d61 6368 696e 6576 6973 696f  rke/machinevisio
+000038e0: 6e2d 746f 6f6c 626f 782d 7079 7468 6f6e  n-toolbox-python
+000038f0: 2f72 6177 2f6d 6173 7465 722f 6669 6773  /raw/master/figs
+00003900: 2f63 7562 652e 706e 6729 0a0a 3c21 2d2d  /cube.png)..<!--
+00003910: 2d6f 7220 7769 7468 2061 2066 6973 6865  -or with a fishe
+00003920: 7965 2063 616d 6572 610a 0a60 6060 6d61  ye camera..```ma
+00003930: 746c 6162 0a3e 3e20 6361 6d20 3d20 4669  tlab.>> cam = Fi
+00003940: 7368 4579 6543 616d 6572 6128 276e 616d  shEyeCamera('nam
+00003950: 6527 2c20 2766 6973 6865 7965 272c 202e  e', 'fisheye', .
+00003960: 2e2e 0a27 7072 6f6a 6563 7469 6f6e 272c  ...'projection',
+00003970: 2027 6571 7569 616e 6775 6c61 7227 2c20   'equiangular', 
+00003980: 2e2e 2e0a 2770 6978 656c 272c 2031 3065  ....'pixel', 10e
+00003990: 2d36 2c20 2e2e 2e0a 2772 6573 6f6c 7574  -6, ....'resolut
+000039a0: 696f 6e27 2c20 5b31 3238 3020 3130 3234  ion', [1280 1024
+000039b0: 5d29 3b0a 3e3e 205b 582c 592c 5a5d 203d  ]);.>> [X,Y,Z] =
+000039c0: 206d 6b63 7562 6528 302e 322c 2027 6365   mkcube(0.2, 'ce
+000039d0: 6e74 7265 272c 205b 302e 322c 2030 2c20  ntre', [0.2, 0, 
+000039e0: 302e 335d 2c20 2765 6467 6527 293b 0a3e  0.3], 'edge');.>
+000039f0: 3e20 6361 6d2e 6d65 7368 2858 2c20 592c  > cam.mesh(X, Y,
+00003a00: 205a 293b 0a60 6060 0a21 5b46 6973 6865   Z);.```.![Fishe
+00003a10: 7965 206c 656e 7320 6361 6d65 7261 2076  ye lens camera v
+00003a20: 6965 775d 2866 6967 732f 6375 6265 5f66  iew](figs/cube_f
+00003a30: 6973 6865 7965 2e70 6e67 290a 0a0a 2323  isheye.png)...##
+00003a40: 2320 4275 6e64 6c65 2061 646a 7573 746d  # Bundle adjustm
+00003a50: 656e 740a 2d2d 2d3e 0a0a 2323 2320 436f  ent.--->..### Co
+00003a60: 6c6f 7220 7370 6163 650a 0a50 6c6f 7420  lor space..Plot 
+00003a70: 7468 6520 4349 4520 6368 726f 6d61 7469  the CIE chromati
+00003a80: 6369 7479 2073 7061 6365 0a0a 6060 6070  city space..```p
+00003a90: 7974 686f 6e0a 706c 6f74 5f63 6872 6f6d  ython.plot_chrom
+00003aa0: 6174 6963 6974 795f 6469 6167 7261 6d28  aticity_diagram(
+00003ab0: 2278 7922 293b 0a70 6c6f 745f 7370 6563  "xy");.plot_spec
+00003ac0: 7472 616c 5f6c 6f63 7573 2822 7879 2229  tral_locus("xy")
+00003ad0: 0a60 6060 0a0a 215b 4349 4520 6368 726f  .```..![CIE chro
+00003ae0: 6d61 7469 6369 7479 2073 7061 6365 5d28  maticity space](
+00003af0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003b00: 6f6d 2f70 6574 6572 636f 726b 652f 6d61  om/petercorke/ma
+00003b10: 6368 696e 6576 6973 696f 6e2d 746f 6f6c  chinevision-tool
+00003b20: 626f 782d 7079 7468 6f6e 2f72 6177 2f6d  box-python/raw/m
+00003b30: 6173 7465 722f 6669 6773 2f63 6f6c 6f72  aster/figs/color
+00003b40: 7370 6163 652e 706e 6729 0a0a 4c6f 6164  space.png)..Load
+00003b50: 2074 6865 2073 7065 6374 7275 6d20 6f66   the spectrum of
+00003b60: 2073 756e 6c69 6768 7420 6174 2074 6865   sunlight at the
+00003b70: 2045 6172 7468 2773 2073 7572 6661 6365   Earth's surface
+00003b80: 2061 6e64 2063 6f6d 7075 7465 2074 6865   and compute the
+00003b90: 2043 4945 2078 7920 6368 726f 6d61 7469   CIE xy chromati
+00003ba0: 6369 7479 2063 6f6f 7264 696e 6174 6573  city coordinates
+00003bb0: 0a0a 6060 6070 7974 686f 6e0a 6e6d 203d  ..```python.nm =
+00003bc0: 2031 652d 390a 6c61 6d20 3d20 6e70 2e6c   1e-9.lam = np.l
+00003bd0: 696e 7370 6163 6528 3430 302c 2037 3031  inspace(400, 701
+00003be0: 2c20 3529 202a 206e 6d20 2320 7669 7369  , 5) * nm # visi
+00003bf0: 626c 6520 6c69 6768 740a 7375 6e5f 6174  ble light.sun_at
+00003c00: 5f67 726f 756e 6420 3d20 6c6f 6164 7370  _ground = loadsp
+00003c10: 6563 7472 756d 286c 616d 2c20 2273 6f6c  ectrum(lam, "sol
+00003c20: 6172 2229 0a78 7920 3d20 6c61 6d62 6461  ar").xy = lambda
+00003c30: 3278 7928 6c61 6d62 6461 2c20 7375 6e5f  2xy(lambda, sun_
+00003c40: 6174 5f67 726f 756e 6429 0a70 7269 6e74  at_ground).print
+00003c50: 2878 7929 0a09 5b5b 302e 3333 3237 3237  (xy)..[[0.332727
+00003c60: 3938 2030 2e33 3435 3430 3133 205d 5d0a  98 0.3454013 ]].
+00003c70: 7072 696e 7428 636f 6c6f 726e 616d 6528  print(colorname(
+00003c80: 7879 2c20 2278 7922 2929 0a09 6b68 616b  xy, "xy"))..khak
+00003c90: 690a 6060 600a 0a23 2323 2048 6f75 6768  i.```..### Hough
+00003ca0: 2074 7261 6e73 666f 726d 0a0a 6060 6070   transform..```p
+00003cb0: 7974 686f 6e0a 696d 203d 2049 6d61 6765  ython.im = Image
+00003cc0: 2e52 6561 6428 2263 6875 7263 682e 706e  .Read("church.pn
+00003cd0: 6722 2c20 6d6f 6e6f 3d54 7275 6529 0a65  g", mono=True).e
+00003ce0: 6467 6573 203d 2069 6d2e 6361 6e6e 7928  dges = im.canny(
+00003cf0: 290a 6820 3d20 6564 6765 732e 486f 7567  ).h = edges.Houg
+00003d00: 6828 290a 6c69 6e65 7320 3d20 682e 6c69  h().lines = h.li
+00003d10: 6e65 735f 7028 3130 302c 206d 696e 6c69  nes_p(100, minli
+00003d20: 6e65 6c65 6e67 7468 3d32 3030 2c20 6d61  nelength=200, ma
+00003d30: 786c 696e 6567 6170 3d35 2c20 7365 6564  xlinegap=5, seed
+00003d40: 3d30 290a 0a69 6d2e 6469 7370 2864 6172  =0)..im.disp(dar
+00003d50: 6b65 6e3d 5472 7565 290a 682e 706c 6f74  ken=True).h.plot
+00003d60: 5f6c 696e 6573 286c 696e 6573 2c20 2272  _lines(lines, "r
+00003d70: 2d2d 2229 0a60 6060 0a0a 215b 486f 7567  --").```..![Houg
+00003d80: 6820 7472 616e 7366 6f72 6d5d 2868 7474  h transform](htt
+00003d90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00003da0: 7065 7465 7263 6f72 6b65 2f6d 6163 6869  petercorke/machi
+00003db0: 6e65 7669 7369 6f6e 2d74 6f6f 6c62 6f78  nevision-toolbox
+00003dc0: 2d70 7974 686f 6e2f 7261 772f 6d61 7374  -python/raw/mast
+00003dd0: 6572 2f66 6967 732f 686f 7567 682e 706e  er/figs/hough.pn
+00003de0: 6729 0a0a 2323 2320 5355 5246 2066 6561  g)..### SURF fea
+00003df0: 7475 7265 730a 0a57 6520 6c6f 6164 2074  tures..We load t
+00003e00: 776f 2069 6d61 6765 7320 616e 6420 636f  wo images and co
+00003e10: 6d70 7574 6520 6120 7365 7420 6f66 2053  mpute a set of S
+00003e20: 5552 4620 6665 6174 7572 6573 2066 6f72  URF features for
+00003e30: 2065 6163 680a 0a60 6060 7079 7468 6f6e   each..```python
+00003e40: 0a76 6965 7731 203d 2049 6d61 6765 2e52  .view1 = Image.R
+00003e50: 6561 6428 2265 6966 6665 6c2d 312e 706e  ead("eiffel-1.pn
+00003e60: 6722 2c20 6d6f 6e6f 3d54 7275 6529 0a76  g", mono=True).v
+00003e70: 6965 7732 203d 2049 6d61 6765 2e52 6561  iew2 = Image.Rea
+00003e80: 6428 2265 6966 6665 6c2d 322e 706e 6722  d("eiffel-2.png"
+00003e90: 2c20 6d6f 6e6f 3d54 7275 6529 0a73 6631  , mono=True).sf1
+00003ea0: 203d 2076 6965 7731 2e53 4946 5428 290a   = view1.SIFT().
+00003eb0: 7366 3220 3d20 7669 6577 322e 5349 4654  sf2 = view2.SIFT
+00003ec0: 2829 0a60 6060 0a0a 5765 2063 616e 206d  ().```..We can m
+00003ed0: 6174 6368 2066 6561 7475 7265 7320 6265  atch features be
+00003ee0: 7477 6565 6e20 696d 6167 6573 2062 6173  tween images bas
+00003ef0: 6564 2070 7572 656c 7920 6f6e 2074 6865  ed purely on the
+00003f00: 2073 696d 696c 6172 6974 7920 6f66 2074   similarity of t
+00003f10: 6865 2066 6561 7475 7265 732c 2061 6e64  he features, and
+00003f20: 2064 6973 706c 6179 2074 6865 2063 6f72   display the cor
+00003f30: 7265 7370 6f6e 6465 6e63 6573 2066 6f75  respondences fou
+00003f40: 6e64 0a0a 6060 6070 7974 686f 6e0a 6d61  nd..```python.ma
+00003f50: 7463 6865 7320 3d20 7366 312e 6d61 7463  tches = sf1.matc
+00003f60: 6828 7366 3229 0a70 7269 6e74 286d 6174  h(sf2).print(mat
+00003f70: 6368 6573 290a 3831 3320 6d61 7463 6865  ches).813 matche
+00003f80: 730a 6d61 7463 6865 735b 313a 355d 2e74  s.matches[1:5].t
+00003f90: 6162 6c65 2829 0ae2 948c e294 80e2 9480  able()..........
+00003fa0: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
+00003fb0: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
+00003fc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003fd0: e294 80e2 9480 e294 80e2 9480 e294 ace2  ................
+00003fe0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003ff0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004000: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004010: 9480 e294 ace2 9480 e294 80e2 9480 e294  ................
+00004020: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004040: 9480 e294 80e2 9490 0ae2 9482 2320 e294  ............# ..
+00004050: 8220 696e 6c69 6572 20e2 9482 2073 7472  . inlier ... str
+00004060: 656e 6774 6820 e294 8220 2020 2020 2020  ength ...       
+00004070: 2020 2020 2020 2070 3120 e294 8220 2020         p1 ...   
+00004080: 2020 2020 2020 2020 2020 7032 20e2 9482            p2 ...
+00004090: 0ae2 949c e294 80e2 9480 e294 bce2 9480  ................
+000040a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000040b0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+000040c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000040d0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+000040e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000040f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004100: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00004110: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004120: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004130: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004140: 94a4 0ae2 9482 3020 e294 8220 2020 2020  ......0 ...     
+00004150: 2020 20e2 9482 2020 2020 2032 362e 3420     ...     26.4 
+00004160: e294 8220 2831 3131 382e 362c 2031 3738  ... (1118.6, 178
+00004170: 2e38 2920 e294 8220 2839 3532 2e35 2c20  .8) ... (952.5, 
+00004180: 3431 382e 3029 20e2 9482 0ae2 9482 3120  418.0) .......1 
+00004190: e294 8220 2020 2020 2020 20e2 9482 2020  ...        ...  
+000041a0: 2020 2032 382e 3220 e294 8220 2838 3230     28.2 ... (820
+000041b0: 2e36 2c20 3531 392e 3129 2020 e294 8220  .6, 519.1)  ... 
+000041c0: 2837 3038 2e31 2c20 3730 312e 3629 20e2  (708.1, 701.6) .
+000041d0: 9482 0ae2 9482 3220 e294 8220 2020 2020  ......2 ...     
+000041e0: 2020 20e2 9482 2020 2020 2032 392e 3620     ...     29.6 
+000041f0: e294 8220 2838 3031 2e31 2c20 3633 322e  ... (801.1, 632.
+00004200: 3429 2020 e294 8220 2836 3934 2e31 2c20  4)  ... (694.1, 
+00004210: 3830 302e 3329 20e2 9482 0ae2 9482 3320  800.3) .......3 
+00004220: e294 8220 2020 2020 2020 20e2 9482 2020  ...        ...  
+00004230: 2020 2033 322e 3420 e294 8220 2837 3436     32.4 ... (746
+00004240: 2e30 2c20 3135 332e 3129 2020 e294 8220  .0, 153.1)  ... 
+00004250: 2836 3434 2e35 2c20 3339 322e 3229 20e2  (644.5, 392.2) .
+00004260: 9482 0ae2 9494 e294 80e2 9480 e294 b4e2  ................
+00004270: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004280: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
+00004290: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000042a0: 9480 e294 80e2 9480 e294 b4e2 9480 e294  ................
+000042b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000042c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000042d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000042e0: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000042f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004300: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004310: 80e2 9498 0a60 6060 0a0a 7768 6572 6520  .....```..where 
+00004320: 7765 2068 6176 6520 6469 7370 6c61 7965  we have displaye
+00004330: 6420 7468 6520 6665 6174 7572 6520 636f  d the feature co
+00004340: 6f72 6469 6e61 7465 7320 666f 7220 666f  ordinates for fo
+00004350: 7572 2063 6f72 7265 7370 6f6e 6465 6e63  ur correspondenc
+00004360: 6573 2e0a 0a57 6520 6361 6e20 616c 736f  es...We can also
+00004370: 2064 6973 706c 6179 2074 6865 2063 6f72   display the cor
+00004380: 7265 7370 6f6e 6465 6e63 6573 2067 7261  respondences gra
+00004390: 7068 6963 616c 6c79 0a0a 6060 6070 7974  phically..```pyt
+000043a0: 686f 6e0a 6d61 7463 6865 732e 7375 6273  hon.matches.subs
+000043b0: 6574 2831 3030 292e 706c 6f74 2822 7722  et(100).plot("w"
+000043c0: 290a 6060 600a 0a69 6e20 7468 6973 2063  ).```..in this c
+000043d0: 6173 652c 2061 2073 7562 7365 7420 6f66  ase, a subset of
+000043e0: 2031 3030 2f38 3133 206f 6620 7468 6520   100/813 of the 
+000043f0: 636f 7272 6573 706f 6e64 656e 6365 732e  correspondences.
+00004400: 0a0a 215b 4665 6174 7572 6520 6d61 7463  ..![Feature matc
+00004410: 6869 6e67 5d28 6874 7470 733a 2f2f 6769  hing](https://gi
+00004420: 7468 7562 2e63 6f6d 2f70 6574 6572 636f  thub.com/peterco
+00004430: 726b 652f 6d61 6368 696e 6576 6973 696f  rke/machinevisio
+00004440: 6e2d 746f 6f6c 626f 782d 7079 7468 6f6e  n-toolbox-python
+00004450: 2f72 6177 2f6d 6173 7465 722f 6669 6773  /raw/master/figs
+00004460: 2f6d 6174 6368 696e 672e 706e 6729 0a0a  /matching.png)..
+00004470: 436c 6561 726c 7920 7468 6572 6520 6172  Clearly there ar
+00004480: 6520 736f 6d65 2062 6164 206d 6174 6368  e some bad match
+00004490: 6573 2068 6572 652c 2062 7574 2077 6520  es here, but we 
+000044a0: 7765 2063 616e 2075 7365 2052 414e 5341  we can use RANSA
+000044b0: 4320 616e 6420 7468 6520 6570 6970 6f6c  C and the epipol
+000044c0: 6172 2063 6f6e 7374 7261 696e 7420 696d  ar constraint im
+000044d0: 706c 6965 6420 6279 2074 6865 2066 756e  plied by the fun
+000044e0: 6461 6d65 6e74 616c 206d 6174 7269 7820  damental matrix 
+000044f0: 746f 2065 7374 696d 6174 6520 7468 6520  to estimate the 
+00004500: 6675 6e64 616d 656e 7461 6c20 6d61 7472  fundamental matr
+00004510: 6978 2061 6e64 2063 6c61 7373 6966 7920  ix and classify 
+00004520: 636f 7272 6573 706f 6e64 656e 6365 7320  correspondences 
+00004530: 6173 2069 6e6c 6965 7273 206f 7220 6f75  as inliers or ou
+00004540: 746c 6965 7273 0a0a 6060 6070 7974 686f  tliers..```pytho
+00004550: 6e0a 462c 2072 6573 6964 203d 206d 6174  n.F, resid = mat
+00004560: 6368 6573 2e65 7374 696d 6174 6528 4365  ches.estimate(Ce
+00004570: 6e74 7261 6c43 616d 6572 612e 706f 696e  ntralCamera.poin
+00004580: 7473 3246 2c20 6d65 7468 6f64 3d22 7261  ts2F, method="ra
+00004590: 6e73 6163 222c 2063 6f6e 6669 6465 6e63  nsac", confidenc
+000045a0: 653d 302e 3939 2c20 7365 6564 3d30 290a  e=0.99, seed=0).
+000045b0: 7072 696e 7428 4629 0a61 7272 6179 285b  print(F).array([
+000045c0: 5b31 2e30 3333 652d 3038 2c20 2d33 2e37  [1.033e-08, -3.7
+000045d0: 3939 652d 3036 2c20 302e 3030 3236 3738  99e-06, 0.002678
+000045e0: 5d2c 0a20 2020 2020 2020 5b33 2e36 3638  ],.       [3.668
+000045f0: 652d 3036 2c20 312e 3231 3765 2d30 372c  e-06, 1.217e-07,
+00004600: 202d 302e 3030 3430 3333 5d2c 0a20 2020   -0.004033],.   
+00004610: 2020 2020 5b2d 302e 3030 3331 392c 2030      [-0.00319, 0
+00004620: 2e30 3033 3433 362c 2020 2020 2020 2020  .003436,        
+00004630: 315d 5d29 0a70 7269 6e74 2872 6573 6964  1]]).print(resid
+00004640: 290a 302e 3034 3035 0a0a 496d 6167 652e  ).0.0405..Image.
+00004650: 4873 7461 636b 2828 7669 6577 312c 2076  Hstack((view1, v
+00004660: 6965 7732 2929 2e64 6973 7028 290a 6d61  iew2)).disp().ma
+00004670: 7463 6865 732e 696e 6c69 6572 732e 7375  tches.inliers.su
+00004680: 6273 6574 2831 3030 292e 706c 6f74 2822  bset(100).plot("
+00004690: 6722 2c20 6178 3d70 6c74 2e67 6361 2829  g", ax=plt.gca()
+000046a0: 290a 6d61 7463 6865 732e 6f75 746c 6965  ).matches.outlie
+000046b0: 7273 2e73 7562 7365 7428 3130 3029 2e70  rs.subset(100).p
+000046c0: 6c6f 7428 2272 222c 2061 783d 706c 742e  lot("r", ax=plt.
+000046d0: 6763 6128 2929 0a60 6060 0a0a 7768 6572  gca()).```..wher
+000046e0: 6520 6772 6565 6e20 6c69 6e65 7320 7368  e green lines sh
+000046f0: 6f77 2063 6f72 7265 6374 2063 6f72 7265  ow correct corre
+00004700: 7370 6f6e 6465 6e63 6573 2028 696e 6c69  spondences (inli
+00004710: 6572 7329 2061 6e64 2072 6564 206c 696e  ers) and red lin
+00004720: 6573 2073 686f 7720 6261 6420 636f 7272  es show bad corr
+00004730: 6573 706f 6e64 656e 6365 7320 286f 7574  espondences (out
+00004740: 6c69 6572 7329 0a0a 215b 4665 6174 7572  liers)..![Featur
+00004750: 6520 6d61 7463 6869 6e67 2061 6674 6572  e matching after
+00004760: 2052 414e 5341 435d 2868 7474 7073 3a2f   RANSAC](https:/
+00004770: 2f67 6974 6875 622e 636f 6d2f 7065 7465  /github.com/pete
+00004780: 7263 6f72 6b65 2f6d 6163 6869 6e65 7669  rcorke/machinevi
+00004790: 7369 6f6e 2d74 6f6f 6c62 6f78 2d70 7974  sion-toolbox-pyt
+000047a0: 686f 6e2f 7261 772f 6d61 7374 6572 2f66  hon/raw/master/f
+000047b0: 6967 732f 6d61 7463 6869 6e67 5f72 616e  igs/matching_ran
+000047c0: 7361 632e 706e 6729 0a0a 2320 4869 7374  sac.png)..# Hist
+000047d0: 6f72 790a 0a54 6869 7320 7061 636b 6167  ory..This packag
+000047e0: 6520 6361 6e20 6265 2063 6f6e 7369 6465  e can be conside
+000047f0: 7265 6420 6173 2061 2050 7974 686f 6e20  red as a Python 
+00004800: 7665 7273 696f 6e20 6f66 2074 6865 205b  version of the [
+00004810: 4d61 6368 696e 6520 5669 7369 6f6e 0a54  Machine Vision.T
+00004820: 6f6f 6c62 6f78 2066 6f72 204d 4154 4c41  oolbox for MATLA
+00004830: 425d 2829 2e20 5468 6174 2054 6f6f 6c62  B](). That Toolb
+00004840: 6f78 2c20 6e6f 7720 7175 6974 6520 6f6c  ox, now quite ol
+00004850: 642c 2069 7320 6120 636f 6c6c 6563 7469  d, is a collecti
+00004860: 6f6e 206f 6620 4d41 544c 4142 0a66 756e  on of MATLAB.fun
+00004870: 6374 696f 6e73 2061 6e64 2063 6c61 7373  ctions and class
+00004880: 6573 2074 6861 7420 7375 7070 6f72 7465  es that supporte
+00004890: 6420 7468 6520 6669 7273 7420 7477 6f20  d the first two 
+000048a0: 6564 6974 696f 6e73 206f 6620 7468 6520  editions of the 
+000048b0: 526f 626f 7469 6373 2c0a 5669 7369 6f6e  Robotics,.Vision
+000048c0: 2026 2043 6f6e 7472 6f6c 2062 6f6f 6b2e   & Control book.
+000048d0: 2049 7420 6973 2061 2073 6f6d 6577 6861   It is a somewha
+000048e0: 7420 6563 6c65 6374 6963 2063 6f6c 6c65  t eclectic colle
+000048f0: 6374 696f 6e20 7265 666c 6563 7469 6e67  ction reflecting
+00004900: 206d 790a 7065 7273 6f6e 616c 2069 6e74   my.personal int
+00004910: 6572 6573 7420 696e 2061 7265 6173 206f  erest in areas o
+00004920: 6620 7068 6f74 6f6d 6574 7279 2c20 7068  f photometry, ph
+00004930: 6f74 6f67 7261 6d6d 6574 7279 2c20 636f  otogrammetry, co
+00004940: 6c6f 7269 6d65 7472 792e 2049 740a 696e  lorimetry. It.in
+00004950: 636c 7564 6573 206f 7665 7220 3130 3020  cludes over 100 
+00004960: 6675 6e63 7469 6f6e 7320 7370 616e 6e69  functions spanni
+00004970: 6e67 206f 7065 7261 7469 6f6e 7320 7375  ng operations su
+00004980: 6368 2061 7320 696d 6167 6520 6669 6c65  ch as image file
+00004990: 2072 6561 6469 6e67 2061 6e64 0a77 7269   reading and.wri
+000049a0: 7469 6e67 2c20 6163 7175 6973 6974 696f  ting, acquisitio
+000049b0: 6e2c 2064 6973 706c 6179 2c20 6669 6c74  n, display, filt
+000049c0: 6572 696e 672c 2062 6c6f 622c 2070 6f69  ering, blob, poi
+000049d0: 6e74 2061 6e64 206c 696e 6520 6665 6174  nt and line feat
+000049e0: 7572 650a 6578 7472 6163 7469 6f6e 2c20  ure.extraction, 
+000049f0: 6d61 7468 656d 6174 6963 616c 206d 6f72  mathematical mor
+00004a00: 7068 6f6c 6f67 792c 2068 6f6d 6f67 7261  phology, homogra
+00004a10: 7068 6965 732c 2076 6973 7561 6c20 4a61  phies, visual Ja
+00004a20: 636f 6269 616e 732c 2063 616d 6572 610a  cobians, camera.
+00004a30: 6361 6c69 6272 6174 696f 6e20 616e 6420  calibration and 
+00004a40: 636f 6c6f 7220 7370 6163 6520 636f 6e76  color space conv
+00004a50: 6572 7369 6f6e 2e0a 0a54 6869 7320 5079  ersion...This Py
+00004a60: 7468 6f6e 2076 6572 7369 6f6e 2064 6966  thon version dif
+00004a70: 6665 7273 2069 6e20 7573 696e 6720 616e  fers in using an
+00004a80: 206f 626a 6563 7420 746f 2065 6e63 6170   object to encap
+00004a90: 7375 6c61 7465 2074 6865 2070 6978 656c  sulate the pixel
+00004aa0: 2064 6174 6120 616e 640a 696d 6167 6520   data and.image 
+00004ab0: 6d65 7461 6461 7461 2c20 7261 7468 6572  metadata, rather
+00004ac0: 2074 6861 6e20 6a75 7374 2061 206e 6174   than just a nat
+00004ad0: 6976 6520 6f62 6a65 6374 2068 6f6c 6469  ive object holdi
+00004ae0: 6e67 2070 6978 656c 2064 6174 612e 2054  ng pixel data. T
+00004af0: 6865 206d 616e 790a 6675 6e63 7469 6f6e  he many.function
+00004b00: 7320 6265 636f 6d65 206d 6574 686f 6473  s become methods
+00004b10: 206f 6620 7468 6520 696d 6167 6520 6f62   of the image ob
+00004b20: 6a65 6374 2077 6869 6368 2072 6564 7563  ject which reduc
+00004b30: 6573 206e 616d 6573 7061 6365 2070 6f6c  es namespace pol
+00004b40: 6c75 7469 6f6e 732c 0a61 6e64 2061 6c6c  lutions,.and all
+00004b50: 6f77 7320 7468 6520 6561 7379 2065 7870  ows the easy exp
+00004b60: 7265 7373 696f 6e20 6f66 2073 6571 7565  ression of seque
+00004b70: 6e74 6961 6c20 6f70 6572 6174 696f 6e73  ntial operations
+00004b80: 2075 7369 6e67 2022 646f 7420 6368 6169   using "dot chai
+00004b90: 6e69 6e67 222e 0a0a 5468 6520 6669 7273  ning"...The firs
+00004ba0: 7420 7665 7273 696f 6e20 7761 7320 6372  t version was cr
+00004bb0: 6561 7465 6420 6279 2044 6f72 6961 6e20  eated by Dorian 
+00004bc0: 5473 6169 2064 7572 696e 6720 3230 3230  Tsai during 2020
+00004bd0: 2c20 616e 6420 6261 7365 6420 6f6e 2074  , and based on t
+00004be0: 6865 0a4d 4154 4c41 4220 7665 7273 696f  he.MATLAB versio
+00004bf0: 6e2e 2020 5468 6174 2077 6f72 6b20 7761  n.  That work wa
+00004c00: 7320 6675 6e64 6564 2062 7920 616e 2041  s funded by an A
+00004c10: 7573 7472 616c 6961 6e20 556e 6976 6572  ustralian Univer
+00004c20: 7369 7479 2054 6561 6368 6572 206f 660a  sity Teacher of.
+00004c30: 7468 6520 7965 6172 2061 7761 7264 2028  the year award (
+00004c40: 3230 3137 2920 746f 2050 6574 6572 2043  2017) to Peter C
+00004c50: 6f72 6b65 2e0a                           orke..
```

### Comparing `machinevision-toolbox-python-0.9.6/machinevision_toolbox_python.egg-info/PKG-INFO` & `machinevision_toolbox_python-0.9.7/machinevision_toolbox_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d61 6368  : 2.1.Name: mach
 00000020: 696e 6576 6973 696f 6e2d 746f 6f6c 626f  inevision-toolbo
 00000030: 782d 7079 7468 6f6e 0a56 6572 7369 6f6e  x-python.Version
-00000040: 3a20 302e 392e 360a 5375 6d6d 6172 793a  : 0.9.6.Summary:
+00000040: 3a20 302e 392e 370a 5375 6d6d 6172 793a  : 0.9.7.Summary:
 00000050: 2050 7974 686f 6e20 746f 6f6c 7320 666f   Python tools fo
 00000060: 7220 6d61 6368 696e 6520 7669 7369 6f6e  r machine vision
 00000070: 202d 2065 6475 6361 7469 6f6e 2061 6e64   - education and
 00000080: 2072 6573 6561 7263 680a 4175 7468 6f72   research.Author
 00000090: 3a20 446f 7269 616e 2054 7361 690a 4175  : Dorian Tsai.Au
 000000a0: 7468 6f72 2d65 6d61 696c 3a20 5065 7465  thor-email: Pete
 000000b0: 7220 436f 726b 6520 3c72 7663 4070 6574  r Corke <rvc@pet
@@ -70,1107 +70,1153 @@
 00000450: 650a 436c 6173 7369 6669 6572 3a20 4f70  e.Classifier: Op
 00000460: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
 00000470: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
 00000480: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
 00000490: 3a20 3e3d 332e 370a 4465 7363 7269 7074  : >=3.7.Descript
 000004a0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
 000004b0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-000004c0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-000004d0: 6465 760a 5072 6f76 6964 6573 2d45 7874  dev.Provides-Ext
-000004e0: 7261 3a20 646f 6373 0a4c 6963 656e 7365  ra: docs.License
-000004f0: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
-00000500: 2320 4d61 6368 696e 6520 5669 7369 6f6e  # Machine Vision
-00000510: 2054 6f6f 6c62 6f78 2066 6f72 2050 7974   Toolbox for Pyt
-00000520: 686f 6e0a 0a5b 215b 4120 5079 7468 6f6e  hon..[![A Python
-00000530: 2052 6f62 6f74 6963 7320 5061 636b 6167   Robotics Packag
-00000540: 655d 2868 7474 7073 3a2f 2f72 6177 2e67  e](https://raw.g
-00000550: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-00000560: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
-00000570: 726f 626f 7469 6373 2d74 6f6f 6c62 6f78  robotics-toolbox
-00000580: 2d70 7974 686f 6e2f 6d61 7374 6572 2f2e  -python/master/.
-00000590: 6769 7468 7562 2f73 7667 2f70 795f 636f  github/svg/py_co
-000005a0: 6c6c 6563 7469 6f6e 2e6d 696e 2e73 7667  llection.min.svg
-000005b0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-000005c0: 622e 636f 6d2f 7065 7465 7263 6f72 6b65  b.com/petercorke
-000005d0: 2f72 6f62 6f74 6963 732d 746f 6f6c 626f  /robotics-toolbo
-000005e0: 782d 7079 7468 6f6e 290a 5b21 5b50 6f77  x-python).[![Pow
-000005f0: 6572 6564 2062 7920 5370 6174 6961 6c20  ered by Spatial 
-00000600: 4d61 7468 735d 2868 7474 7073 3a2f 2f72  Maths](https://r
-00000610: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000620: 7465 6e74 2e63 6f6d 2f70 6574 6572 636f  tent.com/peterco
-00000630: 726b 652f 7370 6174 6961 6c6d 6174 682d  rke/spatialmath-
-00000640: 7079 7468 6f6e 2f6d 6173 7465 722f 2e67  python/master/.g
-00000650: 6974 6875 622f 7376 672f 736d 5f70 6f77  ithub/svg/sm_pow
-00000660: 6572 6564 2e6d 696e 2e73 7667 295d 2868  ered.min.svg)](h
-00000670: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000680: 6d2f 7065 7465 7263 6f72 6b65 2f73 7061  m/petercorke/spa
-00000690: 7469 616c 6d61 7468 2d70 7974 686f 6e29  tialmath-python)
-000006a0: 0a5b 215b 5155 5420 4365 6e74 7265 2066  .[![QUT Centre f
-000006b0: 6f72 2052 6f62 6f74 6963 7320 4f70 656e  or Robotics Open
-000006c0: 2053 6f75 7263 655d 2868 7474 7073 3a2f   Source](https:/
-000006d0: 2f67 6974 6875 622e 636f 6d2f 7163 722f  /github.com/qcr/
-000006e0: 7163 722e 6769 7468 7562 2e69 6f2f 7261  qcr.github.io/ra
-000006f0: 772f 6d61 7374 6572 2f6d 6973 632f 6261  w/master/misc/ba
-00000700: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
-00000710: 2f2f 7163 722e 6769 7468 7562 2e69 6f29  //qcr.github.io)
-00000720: 0a0a 5b21 5b50 7950 4920 7665 7273 696f  ..[![PyPI versio
-00000730: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
-00000740: 2e66 7572 792e 696f 2f70 792f 6d61 6368  .fury.io/py/mach
-00000750: 696e 6576 6973 696f 6e2d 746f 6f6c 626f  inevision-toolbo
-00000760: 782d 7079 7468 6f6e 2e73 7667 295d 2868  x-python.svg)](h
-00000770: 7474 7073 3a2f 2f62 6164 6765 2e66 7572  ttps://badge.fur
-00000780: 792e 696f 2f70 792f 6d61 6368 696e 6576  y.io/py/machinev
-00000790: 6973 696f 6e2d 746f 6f6c 626f 782d 7079  ision-toolbox-py
-000007a0: 7468 6f6e 290a 215b 5079 7468 6f6e 2056  thon).![Python V
-000007b0: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
-000007c0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-000007d0: 7970 692f 7079 7665 7273 696f 6e73 2f6d  ypi/pyversions/m
-000007e0: 6163 6869 6e65 7669 7369 6f6e 2d74 6f6f  achinevision-too
-000007f0: 6c62 6f78 2d70 7974 686f 6e2e 7376 6729  lbox-python.svg)
-00000800: 0a5b 215b 506f 7765 7265 6420 6279 204f  .[![Powered by O
-00000810: 7065 6e43 565d 2868 7474 7073 3a2f 2f72  penCV](https://r
-00000820: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00000830: 7465 6e74 2e63 6f6d 2f70 6574 6572 636f  tent.com/peterco
-00000840: 726b 652f 6d61 6368 696e 6576 6973 696f  rke/machinevisio
-00000850: 6e2d 746f 6f6c 626f 782d 7079 7468 6f6e  n-toolbox-python
-00000860: 2f6d 6173 7465 722f 2e67 6974 6875 622f  /master/.github/
-00000870: 7376 672f 6f70 656e 6376 5f70 6f77 6572  svg/opencv_power
-00000880: 6564 2e73 7667 295d 2868 7474 7073 3a2f  ed.svg)](https:/
-00000890: 2f6f 7065 6e63 762e 6f72 6729 0a5b 215b  /opencv.org).[![
-000008a0: 506f 7765 7265 6420 6279 204f 7065 6e33  Powered by Open3
-000008b0: 445d 2868 7474 7073 3a2f 2f72 6177 2e67  D](https://raw.g
-000008c0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-000008d0: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
-000008e0: 6d61 6368 696e 6576 6973 696f 6e2d 746f  machinevision-to
-000008f0: 6f6c 626f 782d 7079 7468 6f6e 2f6d 6173  olbox-python/mas
-00000900: 7465 722f 2e67 6974 6875 622f 7376 672f  ter/.github/svg/
-00000910: 6f70 656e 3364 5f70 6f77 6572 6564 2e73  open3d_powered.s
-00000920: 7667 295d 2868 7474 7073 3a2f 2f6f 7065  vg)](https://ope
-00000930: 6e33 642e 6f72 6729 0a5b 215b 4c69 6365  n3d.org).[![Lice
-00000940: 6e73 653a 204d 4954 5d28 6874 7470 733a  nse: MIT](https:
-00000950: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000960: 2f62 6164 6765 2f4c 6963 656e 7365 2d4d  /badge/License-M
-00000970: 4954 2d79 656c 6c6f 772e 7376 6729 5d28  IT-yellow.svg)](
-00000980: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
-00000990: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
-000009a0: 4d49 5429 0a0a 5b21 5b42 7569 6c64 2053  MIT)..[![Build S
-000009b0: 7461 7475 735d 2868 7474 7073 3a2f 2f67  tatus](https://g
-000009c0: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
-000009d0: 6f72 6b65 2f6d 6163 6869 6e65 7669 7369  orke/machinevisi
-000009e0: 6f6e 2d74 6f6f 6c62 6f78 2d70 7974 686f  on-toolbox-pytho
-000009f0: 6e2f 776f 726b 666c 6f77 732f 5465 7374  n/workflows/Test
-00000a00: 2d6d 6173 7465 722f 6261 6467 652e 7376  -master/badge.sv
-00000a10: 673f 6272 616e 6368 3d6d 6173 7465 7229  g?branch=master)
-00000a20: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000a30: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
-00000a40: 6d61 6368 696e 6576 6973 696f 6e2d 746f  machinevision-to
-00000a50: 6f6c 626f 782d 7079 7468 6f6e 2f61 6374  olbox-python/act
-00000a60: 696f 6e73 3f71 7565 7279 3d77 6f72 6b66  ions?query=workf
-00000a70: 6c6f 7725 3341 6275 696c 6429 0a5b 215b  low%3Abuild).[![
-00000a80: 436f 7665 7261 6765 5d28 6874 7470 733a  Coverage](https:
-00000a90: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
-00000aa0: 7065 7465 7263 6f72 6b65 2f6d 6163 6869  petercorke/machi
-00000ab0: 6e65 7669 7369 6f6e 2d74 6f6f 6c62 6f78  nevision-toolbox
-00000ac0: 2d70 7974 686f 6e2f 6272 616e 6368 2f6d  -python/branch/m
-00000ad0: 6173 7465 722f 6772 6170 682f 6261 6467  aster/graph/badg
-00000ae0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-00000af0: 636f 6465 636f 762e 696f 2f67 682f 7065  codecov.io/gh/pe
-00000b00: 7465 7263 6f72 6b65 2f6d 6163 6869 6e65  tercorke/machine
-00000b10: 7669 7369 6f6e 2d74 6f6f 6c62 6f78 2d70  vision-toolbox-p
-00000b20: 7974 686f 6e29 0a5b 215b 5079 5049 202d  ython).[![PyPI -
-00000b30: 2044 6f77 6e6c 6f61 6473 5d28 6874 7470   Downloads](http
-00000b40: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000b50: 696f 2f70 7970 692f 6477 2f6d 6163 6869  io/pypi/dw/machi
-00000b60: 6e65 7669 7369 6f6e 2d74 6f6f 6c62 6f78  nevision-toolbox
-00000b70: 2d70 7974 686f 6e29 5d28 6874 7470 733a  -python)](https:
-00000b80: 2f2f 7079 7069 7374 6174 732e 6f72 672f  //pypistats.org/
-00000b90: 7061 636b 6167 6573 2f6d 6163 6869 6e65  packages/machine
-00000ba0: 7669 7369 6f6e 2d74 6f6f 6c62 6f78 2d70  vision-toolbox-p
-00000bb0: 7974 686f 6e29 0a0a 3c21 2d2d 205b 215b  ython)..<!-- [![
-00000bc0: 4769 7448 7562 2073 7461 7273 5d28 6874  GitHub stars](ht
-00000bd0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000be0: 732e 696f 2f67 6974 6875 622f 7374 6172  s.io/github/star
-00000bf0: 732f 7065 7465 7263 6f72 6b65 2f6d 6163  s/petercorke/mac
-00000c00: 6869 6e65 7669 7369 6f6e 2d74 6f6f 6c62  hinevision-toolb
-00000c10: 6f78 2d70 7974 686f 6e2e 7376 673f 7374  ox-python.svg?st
-00000c20: 796c 653d 736f 6369 616c 266c 6162 656c  yle=social&label
-00000c30: 3d53 7461 7229 5d28 6874 7470 733a 2f2f  =Star)](https://
-00000c40: 4769 7448 7562 2e63 6f6d 2f70 6574 6572  GitHub.com/peter
-00000c50: 636f 726b 652f 6d61 6368 696e 6576 6973  corke/machinevis
-00000c60: 696f 6e2d 746f 6f6c 626f 782d 7079 7468  ion-toolbox-pyth
-00000c70: 6f6e 2f73 7461 7267 617a 6572 732f 2920  on/stargazers/) 
-00000c80: 2d2d 3e0a 0a3c 7461 626c 6520 7374 796c  -->..<table styl
-00000c90: 653d 2262 6f72 6465 723a 3070 7822 3e0a  e="border:0px">.
-00000ca0: 3c74 7220 7374 796c 653d 2262 6f72 6465  <tr style="borde
-00000cb0: 723a 3070 7822 3e0a 3c74 6420 7374 796c  r:0px">.<td styl
-00000cc0: 653d 2262 6f72 6465 723a 3070 7822 3e0a  e="border:0px">.
-00000cd0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000ce0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 6574  //github.com/pet
-00000cf0: 6572 636f 726b 652f 6d61 6368 696e 6576  ercorke/machinev
-00000d00: 6973 696f 6e2d 746f 6f6c 626f 782d 7079  ision-toolbox-py
-00000d10: 7468 6f6e 2f72 6177 2f6d 6173 7465 722f  thon/raw/master/
-00000d20: 6669 6773 2f56 6973 696f 6e54 6f6f 6c62  figs/VisionToolb
-00000d30: 6f78 4c6f 676f 5f4e 6f42 6163 6b67 6e64  oxLogo_NoBackgnd
-00000d40: 4032 782e 706e 6722 2077 6964 7468 3d22  @2x.png" width="
-00000d50: 3230 3022 3e3c 2f74 643e 0a3c 7464 2073  200"></td>.<td s
-00000d60: 7479 6c65 3d22 626f 7264 6572 3a30 7078  tyle="border:0px
-00000d70: 223e 0a0a 4120 5079 7468 6f6e 2069 6d70  ">..A Python imp
-00000d80: 6c65 6d65 6e74 6174 696f 6e20 6f66 2074  lementation of t
-00000d90: 6865 203c 6120 6872 6566 3d22 6874 7470  he <a href="http
-00000da0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00000db0: 6574 6572 636f 726b 652f 6d61 6368 696e  etercorke/machin
-00000dc0: 6576 6973 696f 6e2d 746f 6f6c 626f 782d  evision-toolbox-
-00000dd0: 6d61 746c 6162 223e 4d61 6368 696e 6520  matlab">Machine 
-00000de0: 5669 7369 6f6e 2054 6f6f 6c62 6f78 2066  Vision Toolbox f
-00000df0: 6f72 204d 4154 4c41 423c 7375 703e 2672  or MATLAB<sup>&r
-00000e00: 6567 3b3c 2f73 7570 3e3c 2f61 3e3c 756c  eg;</sup></a><ul
-00000e10: 3e0a 0a3c 6c69 3e3c 6120 6872 6566 3d22  >..<li><a href="
-00000e20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000e30: 6f6d 2f70 6574 6572 636f 726b 652f 6d61  om/petercorke/ma
-00000e40: 6368 696e 6576 6973 696f 6e2d 746f 6f6c  chinevision-tool
-00000e50: 626f 782d 7079 7468 6f6e 223e 4769 7448  box-python">GitH
-00000e60: 7562 2072 6570 6f73 6974 6f72 7920 3c2f  ub repository </
-00000e70: 613e 3c2f 6c69 3e0a 3c6c 693e 3c61 2068  a></li>.<li><a h
-00000e80: 7265 663d 2268 7474 7073 3a2f 2f70 6574  ref="https://pet
-00000e90: 6572 636f 726b 652e 6769 7468 7562 2e69  ercorke.github.i
-00000ea0: 6f2f 6d61 6368 696e 6576 6973 696f 6e2d  o/machinevision-
-00000eb0: 746f 6f6c 626f 782d 7079 7468 6f6e 2f22  toolbox-python/"
-00000ec0: 3e44 6f63 756d 656e 7461 7469 6f6e 3c2f  >Documentation</
-00000ed0: 613e 3c2f 6c69 3e0a 3c6c 693e 3c61 2068  a></li>.<li><a h
-00000ee0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00000ef0: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
-00000f00: 6b65 2f6d 6163 6869 6e65 7669 7369 6f6e  ke/machinevision
-00000f10: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e2f  -toolbox-python/
-00000f20: 7769 6b69 223e 4578 616d 706c 6573 2061  wiki">Examples a
-00000f30: 6e64 2064 6574 6169 6c73 3c2f 613e 3c2f  nd details</a></
-00000f40: 6c69 3e0a 3c6c 693e 3c61 2068 7265 663d  li>.<li><a href=
-00000f50: 2269 6e73 7461 6c6c 6174 696f 6e23 223e  "installation#">
-00000f60: 496e 7374 616c 6c61 7469 6f6e 3c2f 613e  Installation</a>
-00000f70: 3c2f 6c69 3e0a 3c2f 756c 3e0a 3c2f 7464  </li>.</ul>.</td
-00000f80: 3e0a 3c2f 7472 3e0a 3c2f 7461 626c 653e  >.</tr>.</table>
-00000f90: 0a0a 2323 2053 796e 6f70 7369 730a 0a54  ..## Synopsis..T
-00000fa0: 6865 204d 6163 6869 6e65 2056 6973 696f  he Machine Visio
-00000fb0: 6e20 546f 6f6c 626f 7820 666f 7220 5079  n Toolbox for Py
-00000fc0: 7468 6f6e 2028 4d56 5442 2d50 2920 7072  thon (MVTB-P) pr
-00000fd0: 6f76 6964 6573 206d 616e 7920 6675 6e63  ovides many func
-00000fe0: 7469 6f6e 7320 7468 6174 2061 7265 2075  tions that are u
-00000ff0: 7365 6675 6c20 696e 206d 6163 6869 6e65  seful in machine
-00001000: 2076 6973 696f 6e20 616e 6420 7669 7369   vision and visi
-00001010: 6f6e 2d62 6173 6564 2063 6f6e 7472 6f6c  on-based control
-00001020: 2e20 5468 6520 6d61 696e 2063 6f6d 706f  . The main compo
-00001030: 6e65 6e74 7320 6172 653a 0a0a 2d20 416e  nents are:..- An
-00001040: 2060 496d 6167 6560 206f 626a 6563 7420   `Image` object 
-00001050: 7769 7468 206e 6561 726c 7920 3230 3020  with nearly 200 
-00001060: 6d65 7468 6f64 7320 616e 6420 7072 6f70  methods and prop
-00001070: 6572 7469 6573 2074 6861 7420 7772 6170  erties that wrap
-00001080: 2066 756e 6374 696f 6e73 0a20 2066 726f   functions.  fro
-00001090: 6d20 4f70 656e 4356 2c20 4e75 6d50 7920  m OpenCV, NumPy 
-000010a0: 616e 6420 5363 6950 792e 204d 6574 686f  and SciPy. Metho
-000010b0: 6473 2073 7570 706f 7274 206d 6f6e 6164  ds support monad
-000010c0: 6963 2c20 6479 6164 6963 2c20 6669 6c74  ic, dyadic, filt
-000010d0: 6572 696e 672c 2065 6467 6520 6465 7465  ering, edge dete
-000010e0: 6374 696f 6e2c 0a20 206d 6174 6865 6d61  ction,.  mathema
-000010f0: 7469 6361 6c20 6d6f 7270 686f 6c6f 6779  tical morphology
-00001100: 2061 6e64 2066 6561 7475 7265 2065 7874   and feature ext
-00001110: 7261 6374 696f 6e20 2862 6c6f 6273 2c20  raction (blobs, 
-00001120: 6c69 6e65 7320 616e 6420 706f 696e 742f  lines and point/
-00001130: 636f 726e 6572 2066 6561 7475 7265 7329  corner features)
-00001140: 2c20 6173 2077 656c 6c20 6173 206f 7065  , as well as ope
-00001150: 7261 746f 7220 6f76 6572 6c6f 6164 696e  rator overloadin
-00001160: 672e 2049 6d61 6765 7320 6172 6520 7374  g. Images are st
-00001170: 6f72 6564 2061 7320 656e 6361 7073 756c  ored as encapsul
-00001180: 6174 6564 205b 4e75 6d50 795d 2868 7474  ated [NumPy](htt
-00001190: 7073 3a2f 2f6e 756d 7079 2e6f 7267 2920  ps://numpy.org) 
-000011a0: 6172 7261 7973 0a20 2061 6c6f 6e67 2077  arrays.  along w
-000011b0: 6974 6820 696d 6167 6520 6d65 7461 6461  ith image metada
-000011c0: 7461 2e0a 2d20 416e 206f 626a 6563 742d  ta..- An object-
-000011d0: 6f72 6965 6e74 6564 2077 7261 7070 6572  oriented wrapper
-000011e0: 206f 6620 4f70 656e 3344 2066 756e 6374   of Open3D funct
-000011f0: 696f 6e73 2074 6861 7420 7375 7070 6f72  ions that suppor
-00001200: 7473 2061 2073 7562 7365 7420 6f66 206f  ts a subset of o
-00001210: 7065 7261 7469 6f6e 732c 2062 7574 2061  perations, but a
-00001220: 6c6c 6f77 7320 6f70 6572 6174 6f72 206f  llows operator o
-00001230: 7665 726c 6f61 6469 6e67 2061 6e64 2069  verloading and i
-00001240: 7320 636f 6d70 6174 6962 6c65 2077 6974  s compatible wit
-00001250: 6820 7468 6520 5b53 7061 7469 616c 204d  h the [Spatial M
-00001260: 6174 6820 546f 6f6c 626f 785d 2868 7474  ath Toolbox](htt
-00001270: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001280: 7065 7465 7263 6f72 6b65 2f73 7061 7469  petercorke/spati
-00001290: 616c 6d61 7468 2d70 7974 686f 6e29 2e0a  almath-python)..
-000012a0: 2d20 4120 636f 6c6c 6563 7469 6f6e 206f  - A collection o
-000012b0: 6620 6361 6d65 7261 2070 726f 6a65 6374  f camera project
-000012c0: 696f 6e20 636c 6173 7365 7320 666f 7220  ion classes for 
-000012d0: 6365 6e74 7261 6c20 286e 6f72 6d61 6c20  central (normal 
-000012e0: 7065 7273 7065 6374 6976 6529 2c20 6669  perspective), fi
-000012f0: 7368 6579 652c 2063 6174 6164 696f 7074  sheye, catadiopt
-00001300: 7269 6320 616e 6420 7370 6865 7269 6361  ric and spherica
-00001310: 6c20 6361 6d65 7261 732e 0a2d 2053 6f6d  l cameras..- Som
-00001320: 6520 6164 7661 6e63 6564 2061 6c67 6f72  e advanced algor
-00001330: 6974 686d 7320 7375 6368 2061 733a 0a20  ithms such as:. 
-00001340: 202d 206d 756c 7469 7669 6577 2067 656f   - multiview geo
-00001350: 6d65 7472 793a 2063 616d 6572 6120 6361  metry: camera ca
-00001360: 6c69 6272 6174 696f 6e2c 2073 7465 7265  libration, stere
-00001370: 6f20 7669 7369 6f6e 2c20 6275 6e64 6c65  o vision, bundle
-00001380: 2061 646a 7573 746d 656e 740a 2020 2d20   adjustment.  - 
-00001390: 6261 6720 6f66 2077 6f72 6473 0a0a 4164  bag of words..Ad
-000013a0: 7661 6e74 6167 6573 206f 6620 7468 6973  vantages of this
-000013b0: 2050 7974 686f 6e20 546f 6f6c 626f 7820   Python Toolbox 
-000013c0: 6172 6520 7468 6174 3a0a 0a2d 2069 7420  are that:..- it 
-000013d0: 7573 6573 2c20 6173 206d 7563 6820 6173  uses, as much as
-000013e0: 2070 6f73 7369 626c 652c 205b 4f70 656e   possible, [Open
-000013f0: 4356 5d28 6874 7470 733a 2f2f 6f70 656e  CV](https://open
-00001400: 6376 2e6f 7267 2920 616e 6420 5b4e 756d  cv.org) and [Num
-00001410: 5079 5d28 6874 7470 733a 2f2f 6e75 6d70  Py](https://nump
-00001420: 792e 6f72 6729 2077 6869 6368 2061 7265  y.org) which are
-00001430: 2070 6f72 7461 626c 652c 2065 6666 6963   portable, effic
-00001440: 6965 6e74 2c20 636f 6d70 7265 6865 6e73  ient, comprehens
-00001450: 6976 6520 616e 6420 6d61 7475 7265 2063  ive and mature c
-00001460: 6f6c 6c65 6374 696f 6e20 6f66 2066 756e  ollection of fun
-00001470: 6374 696f 6e73 2066 6f72 2069 6d61 6765  ctions for image
-00001480: 2070 726f 6365 7373 696e 6720 616e 6420   processing and 
-00001490: 6665 6174 7572 6520 6578 7472 6163 7469  feature extracti
-000014a0: 6f6e 3b0a 2d20 6974 2077 7261 7073 2074  on;.- it wraps t
-000014b0: 6865 204f 7065 6e43 5620 6675 6e63 7469  he OpenCV functi
-000014c0: 6f6e 7320 696e 2061 2063 6f6e 7369 7374  ons in a consist
-000014d0: 656e 7420 7761 792c 2068 6964 696e 6720  ent way, hiding 
-000014e0: 736f 6d65 206f 6620 7468 6520 676e 6172  some of the gnar
-000014f0: 6c79 2064 6574 6169 6c73 206f 6620 4f70  ly details of Op
-00001500: 656e 4356 206c 696b 6520 636f 6e76 6572  enCV like conver
-00001510: 7369 6f6e 2074 6f2f 6672 6f6d 2066 6c6f  sion to/from flo
-00001520: 6174 3332 2061 6e64 2074 6865 2042 4752  at32 and the BGR
-00001530: 2063 6f6c 6f72 206f 7264 6572 2e0a 2d20   color order..- 
-00001540: 6974 2069 7320 6861 7320 7369 6d69 6c61  it is has simila
-00001550: 7269 7479 2074 6f20 7468 6520 4d61 6368  rity to the Mach
-00001560: 696e 6520 5669 7369 6f6e 2054 6f6f 6c62  ine Vision Toolb
-00001570: 6f78 2066 6f72 204d 4154 4c41 422e 0a0a  ox for MATLAB...
-00001580: 2320 4765 7474 696e 6720 676f 696e 670a  # Getting going.
-00001590: 0a23 2320 5573 696e 6720 7069 700a 0a49  .## Using pip..I
-000015a0: 6e73 7461 6c6c 2061 2073 6e61 7073 686f  nstall a snapsho
-000015b0: 7420 6672 6f6d 2050 7950 490a 0a60 6060  t from PyPI..```
-000015c0: 0a25 2070 6970 2069 6e73 7461 6c6c 206d  .% pip install m
-000015d0: 6163 6869 6e65 7669 7369 6f6e 2d74 6f6f  achinevision-too
-000015e0: 6c62 6f78 2d70 7974 686f 6e0a 6060 600a  lbox-python.```.
-000015f0: 0a23 2320 4672 6f6d 2047 6974 4875 620a  .## From GitHub.
-00001600: 0a49 6e73 7461 6c6c 2074 6865 2063 7572  .Install the cur
-00001610: 7265 6e74 2063 6f64 6520 6261 7365 2066  rent code base f
-00001620: 726f 6d20 4769 7448 7562 2061 6e64 2070  rom GitHub and p
-00001630: 6970 2069 6e73 7461 6c6c 2061 206c 696e  ip install a lin
-00001640: 6b20 746f 2074 6861 7420 636c 6f6e 6564  k to that cloned
-00001650: 2063 6f70 790a 0a60 6060 0a25 2067 6974   copy..```.% git
-00001660: 2063 6c6f 6e65 2068 7474 7073 3a2f 2f67   clone https://g
-00001670: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
-00001680: 6f72 6b65 2f6d 6163 6869 6e65 7669 7369  orke/machinevisi
-00001690: 6f6e 2d74 6f6f 6c62 6f78 2d70 7974 686f  on-toolbox-pytho
-000016a0: 6e2e 6769 740a 2520 6364 206d 6163 6869  n.git.% cd machi
-000016b0: 6e65 7669 7369 6f6e 2d74 6f6f 6c62 6f78  nevision-toolbox
-000016c0: 2d70 7974 686f 6e0a 2520 7069 7020 696e  -python.% pip in
-000016d0: 7374 616c 6c20 2d65 202e 0a60 6060 0a0a  stall -e ..```..
-000016e0: 2320 4578 616d 706c 6573 0a0a 2323 2320  # Examples..### 
-000016f0: 5265 6164 696e 6720 616e 6420 6469 7370  Reading and disp
-00001700: 6c61 7920 616e 2069 6d61 6765 0a0a 6060  lay an image..``
-00001710: 6070 7974 686f 6e0a 6672 6f6d 206d 6163  `python.from mac
-00001720: 6869 6e65 7669 7369 6f6e 746f 6f6c 626f  hinevisiontoolbo
-00001730: 7820 696d 706f 7274 2049 6d61 6765 0a6d  x import Image.m
-00001740: 6f6e 6120 3d20 496d 6167 652e 5265 6164  ona = Image.Read
-00001750: 2822 6d6f 6e61 6c69 7361 2e70 6e67 2229  ("monalisa.png")
-00001760: 0a6d 6f6e 612e 6469 7370 2829 0a60 6060  .mona.disp().```
-00001770: 0a0a 215b 4d6f 6e61 204c 6973 6120 696d  ..![Mona Lisa im
-00001780: 6167 655d 2868 7474 7073 3a2f 2f67 6974  age](https://git
-00001790: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
-000017a0: 6b65 2f6d 6163 6869 6e65 7669 7369 6f6e  ke/machinevision
-000017b0: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e2f  -toolbox-python/
-000017c0: 7261 772f 6d61 7374 6572 2f66 6967 732f  raw/master/figs/
-000017d0: 6d6f 6e61 2e70 6e67 290a 0a49 6d61 6765  mona.png)..Image
-000017e0: 7320 6361 6e20 616c 736f 2062 6520 7265  s can also be re
-000017f0: 7475 726e 6564 2062 7920 6974 6572 6174  turned by iterat
-00001800: 6f72 7320 7468 6174 206f 7065 7261 7465  ors that operate
-00001810: 206f 7665 7220 666f 6c64 6572 732c 207a   over folders, z
-00001820: 6970 2066 696c 6573 2c20 6c6f 6361 6c20  ip files, local 
-00001830: 6361 6d65 7261 732c 2077 6562 2063 616d  cameras, web cam
-00001840: 6572 6173 2061 6e64 2076 6964 656f 2066  eras and video f
-00001850: 696c 6573 2e0a 0a23 2323 2053 696d 706c  iles...### Simpl
-00001860: 6520 696d 6167 6520 7072 6f63 6573 7369  e image processi
-00001870: 6e67 0a0a 5468 6520 746f 6f6c 626f 7820  ng..The toolbox 
-00001880: 7375 7070 6f72 7473 206d 616e 7920 6f70  supports many op
-00001890: 6572 6174 696f 6e73 206f 6e20 696d 6167  erations on imag
-000018a0: 6573 2073 7563 6820 6173 2032 4420 6669  es such as 2D fi
-000018b0: 6c74 6572 696e 672c 2065 6467 6520 6465  ltering, edge de
-000018c0: 7465 6374 696f 6e2c 206d 6174 6865 6d61  tection, mathema
-000018d0: 7469 6361 6c20 6d6f 7270 686f 6c6f 6779  tical morphology
-000018e0: 2c20 636f 6c6f 7273 7061 6365 2063 6f6e  , colorspace con
-000018f0: 7665 7273 696f 6e2c 2070 6164 6469 6e67  version, padding
-00001900: 2c20 6372 6f70 7069 6e67 2c20 7265 7369  , cropping, resi
-00001910: 7a69 6e67 2c20 726f 7461 7469 6f6e 2061  zing, rotation a
-00001920: 6e64 2077 6172 7069 6e67 2e0a 0a60 6060  nd warping...```
-00001930: 7079 7468 6f6e 0a6d 6f6e 612e 736d 6f6f  python.mona.smoo
-00001940: 7468 2873 6967 6d61 3d35 292e 6469 7370  th(sigma=5).disp
-00001950: 2829 0a60 6060 0a0a 215b 4d6f 6e61 204c  ().```..![Mona L
-00001960: 6973 6120 696d 6167 6520 7769 7468 2073  isa image with s
-00001970: 6d6f 6f74 6869 6e67 5d28 6874 7470 733a  moothing](https:
-00001980: 2f2f 6769 7468 7562 2e63 6f6d 2f70 6574  //github.com/pet
-00001990: 6572 636f 726b 652f 6d61 6368 696e 6576  ercorke/machinev
-000019a0: 6973 696f 6e2d 746f 6f6c 626f 782d 7079  ision-toolbox-py
-000019b0: 7468 6f6e 2f72 6177 2f6d 6173 7465 722f  thon/raw/master/
-000019c0: 6669 6773 2f6d 6f6e 615f 736d 6f6f 7468  figs/mona_smooth
-000019d0: 2e70 6e67 290a 0a54 6865 7265 2061 7265  .png)..There are
-000019e0: 2061 6c73 6f20 6d61 6e79 2066 756e 6374   also many funct
-000019f0: 696f 6e73 2074 6861 7420 6f70 6572 6174  ions that operat
-00001a00: 6520 6f6e 2070 6169 7273 206f 6620 696d  e on pairs of im
-00001a10: 6167 652e 2041 6c6c 2074 6865 2061 7269  age. All the ari
-00001a20: 7468 6d65 7469 6320 6f70 6572 6174 6f72  thmetic operator
-00001a30: 7320 6172 6520 6f76 6572 6c6f 6164 6564  s are overloaded
-00001a40: 2c20 616e 6420 7468 6572 6520 6172 6520  , and there are 
-00001a50: 6d65 7468 6f64 7320 746f 2063 6f6d 6269  methods to combi
-00001a60: 6e65 2069 6d61 6765 7320 696e 206d 6f72  ne images in mor
-00001a70: 6520 636f 6d70 6c65 7820 7761 7973 2e20  e complex ways. 
-00001a80: 4d75 6c74 6970 6c65 2069 6d61 6765 7320  Multiple images 
-00001a90: 6361 6e20 6265 2073 7461 636b 6564 2068  can be stacked h
-00001aa0: 6f72 697a 6f6e 7461 6c2c 2076 6572 7469  orizontal, verti
-00001ab0: 6361 6c6c 7920 6f72 2074 696c 6564 2069  cally or tiled i
-00001ac0: 6e20 6120 3244 2067 7269 642e 2046 6f72  n a 2D grid. For
-00001ad0: 2065 7861 6d70 6c65 2c20 7765 2063 6f75   example, we cou
-00001ae0: 6c64 2064 6973 706c 6179 2074 6865 206f  ld display the o
-00001af0: 7269 6769 6e61 6c20 616e 6420 736d 6f6f  riginal and smoo
-00001b00: 7468 6564 2069 6d61 6765 7320 7369 6465  thed images side
-00001b10: 2062 7920 7369 6465 0a0a 6060 6070 7974   by side..```pyt
-00001b20: 686f 6e0a 496d 6167 652e 4873 7461 636b  hon.Image.Hstack
-00001b30: 285b 6d6f 6e61 2c20 6d6f 6e61 2e73 6d6f  ([mona, mona.smo
-00001b40: 6f74 6828 7369 676d 613d 3529 5d29 2e64  oth(sigma=5)]).d
-00001b50: 6973 7028 290a 6060 600a 0a77 6865 7265  isp().```..where
-00001b60: 2060 4873 7461 636b 6020 6973 2061 2063   `Hstack` is a c
-00001b70: 6c61 7373 206d 6574 686f 6420 7468 6174  lass method that
-00001b80: 2063 7265 6174 6573 2061 206e 6577 2069   creates a new i
-00001b90: 6d61 6765 2062 7920 7374 6163 6b69 6e67  mage by stacking
-00001ba0: 2074 6865 0a69 6d61 6765 7320 6672 6f6d   the.images from
-00001bb0: 2069 7473 2061 7267 756d 656e 742c 2061   its argument, a
-00001bc0: 6e20 696d 6167 6520 7365 7175 656e 6365  n image sequence
-00001bd0: 2c20 686f 7269 7a6f 6e74 616c 6c79 2e0a  , horizontally..
-00001be0: 0a21 5b4d 6f6e 6120 4c69 7361 2069 6d61  .![Mona Lisa ima
-00001bf0: 6765 2077 6974 6820 736d 6f6f 7468 696e  ge with smoothin
-00001c00: 675d 2868 7474 7073 3a2f 2f67 6974 6875  g](https://githu
-00001c10: 622e 636f 6d2f 7065 7465 7263 6f72 6b65  b.com/petercorke
-00001c20: 2f6d 6163 6869 6e65 7669 7369 6f6e 2d74  /machinevision-t
-00001c30: 6f6f 6c62 6f78 2d70 7974 686f 6e2f 7261  oolbox-python/ra
-00001c40: 772f 6d61 7374 6572 2f66 6967 732f 6d6f  w/master/figs/mo
-00001c50: 6e61 2b73 6d6f 6f74 682e 706e 6729 0a0a  na+smooth.png)..
-00001c60: 2323 2320 4269 6e61 7279 2062 6c6f 6273  ### Binary blobs
-00001c70: 0a0a 4120 636f 6d6d 6f6e 2070 726f 626c  ..A common probl
-00001c80: 656d 2069 6e20 726f 626f 7469 6320 7669  em in robotic vi
-00001c90: 7369 6f6e 2069 7320 746f 2065 7874 7261  sion is to extra
-00001ca0: 6374 2066 6561 7475 7265 7320 6672 6f6d  ct features from
-00001cb0: 2074 6865 2069 6d61 6765 2c20 746f 2064   the image, to d
-00001cc0: 6573 6372 6962 6520 7468 6520 706f 7369  escribe the posi
-00001cd0: 7469 6f6e 2c20 7369 7a65 2c20 7368 6170  tion, size, shap
-00001ce0: 6520 616e 6420 6f72 6965 6e74 6174 696f  e and orientatio
-00001cf0: 6e20 6f66 206f 626a 6563 7473 2069 6e20  n of objects in 
-00001d00: 7468 6520 7363 656e 652e 2046 6f72 2073  the scene. For s
-00001d10: 696d 706c 6520 6269 6e61 7279 2073 6365  imple binary sce
-00001d20: 6e65 7320 626c 6f62 2066 6561 7475 7265  nes blob feature
-00001d30: 7320 6172 6520 636f 6d6d 6f6e 6c79 2075  s are commonly u
-00001d40: 7365 642e 0a0a 6060 6070 7974 686f 6e0a  sed...```python.
-00001d50: 696d 203d 2049 6d61 6765 2e52 6561 6428  im = Image.Read(
-00001d60: 2273 6861 726b 322e 706e 6722 2920 2020  "shark2.png")   
-00001d70: 2320 7265 6164 2061 2062 696e 6172 7920  # read a binary 
-00001d80: 696d 6167 6520 6f66 2074 776f 2073 6861  image of two sha
-00001d90: 726b 730a 696d 2e64 6973 7028 293b 2020  rks.im.disp();  
-00001da0: 2023 2064 6973 706c 6179 2069 7420 7769   # display it wi
-00001db0: 7468 2069 6e74 6572 6163 7469 7665 2076  th interactive v
-00001dc0: 6965 7769 6e67 2074 6f6f 6c0a 626c 6f62  iewing tool.blob
-00001dd0: 7320 3d20 696d 2e62 6c6f 6273 2829 2020  s = im.blobs()  
-00001de0: 2320 6669 6e64 2061 6c6c 2074 6865 2077  # find all the w
-00001df0: 6869 7465 2062 6c6f 6273 0a70 7269 6e74  hite blobs.print
-00001e00: 2862 6c6f 6273 290a 0a09 e294 8ce2 9480  (blobs).........
-00001e10: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
-00001e20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001e30: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
-00001e40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001e50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001e60: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001e70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001e80: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
-00001e90: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
-00001ea0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001eb0: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ec0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001ed0: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
-00001ee0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ef0: 80e2 9480 e294 ace2 9480 e294 80e2 9480  ................
-00001f00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00001f10: 9490 0a09 e294 8269 6420 e294 8220 7061  .......id ... pa
-00001f20: 7265 6e74 20e2 9482 2020 2020 2063 656e  rent ...     cen
-00001f30: 7472 6f69 6420 e294 8220 2020 2020 6172  troid ...     ar
-00001f40: 6561 20e2 9482 2074 6f75 6368 20e2 9482  ea ... touch ...
-00001f50: 2070 6572 696d 20e2 9482 2063 6972 6375   perim ... circu
-00001f60: 6c61 7269 7479 20e2 9482 206f 7269 656e  larity ... orien
-00001f70: 7420 e294 8220 6173 7065 6374 20e2 9482  t ... aspect ...
-00001f80: 0a09 e294 9ce2 9480 e294 80e2 9480 e294  ................
-00001f90: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001fa0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00001fb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001fc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00001fd0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-00001fe0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00001ff0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-00002000: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002010: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-00002020: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-00002030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002040: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002050: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-00002060: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-00002070: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002080: 80e2 9480 e294 80e2 94a4 0a09 e294 8220  ............... 
-00002090: 3020 e294 8220 2020 2020 2d31 20e2 9482  0 ...     -1 ...
-000020a0: 2033 3731 2e32 2c20 3335 352e 3220 e294   371.2, 355.2 ..
-000020b0: 8220 372e 3539 652b 3033 20e2 9482 2046  . 7.59e+03 ... F
-000020c0: 616c 7365 20e2 9482 2035 3537 2e36 20e2  alse ... 557.6 .
-000020d0: 9482 2020 2020 2020 2030 2e33 3431 20e2  ..       0.341 .
-000020e0: 9482 2020 3832 2e39 c2b0 20e2 9482 2020  ..  82.9.. ...  
-000020f0: 302e 3937 3620 e294 820a 09e2 9482 2031  0.976 ........ 1
-00002100: 20e2 9482 2020 2020 202d 3120 e294 8220   ...     -1 ... 
-00002110: 3137 312e 322c 2031 3535 2e32 20e2 9482  171.2, 155.2 ...
-00002120: 2037 2e35 3965 2b30 3320 e294 8220 4661   7.59e+03 ... Fa
-00002130: 6c73 6520 e294 8220 3535 372e 3620 e294  lse ... 557.6 ..
-00002140: 8220 2020 2020 2020 302e 3334 3120 e294  .       0.341 ..
-00002150: 8220 2038 322e 39c2 b020 e294 8220 2030  .  82.9.. ...  0
-00002160: 2e39 3736 20e2 9482 0a09 e294 94e2 9480  .976 ...........
-00002170: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
-00002180: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002190: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
-000021a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000021b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000021c0: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000021d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000021e0: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
-000021f0: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
-00002200: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002210: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002220: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002230: e294 80e2 9480 e294 80e2 94b4 e294 80e2  ................
-00002240: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002250: 80e2 9480 e294 b4e2 9480 e294 80e2 9480  ................
-00002260: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002270: 9498 0a60 6060 0a0a 7768 6572 6520 6062  ...```..where `b
-00002280: 6c6f 6273 6020 6973 2061 206c 6973 742d  lobs` is a list-
-00002290: 6c69 6b65 206f 626a 6563 7420 616e 6420  like object and 
-000022a0: 6561 6368 2065 6c65 6d65 6e74 2064 6573  each element des
-000022b0: 6372 6962 6573 2061 2062 6c6f 6220 696e  cribes a blob in
-000022c0: 2074 6865 2073 6365 6e65 2e20 5468 6520   the scene. The 
-000022d0: 656c 656d 656e 7427 7320 6174 7472 6962  element's attrib
-000022e0: 7574 6573 2064 6573 6372 6962 6520 7661  utes describe va
-000022f0: 7269 6f75 7320 7061 7261 6d65 7465 7273  rious parameters
-00002300: 206f 6620 7468 6520 6f62 6a65 6374 2c20   of the object, 
-00002310: 616e 6420 6d65 7468 6f64 7320 6361 6e20  and methods can 
-00002320: 6265 2075 7365 6420 746f 206f 7665 726c  be used to overl
-00002330: 6179 2067 7261 7068 6963 7320 7375 6368  ay graphics such
-00002340: 2061 7320 626f 756e 6469 6e67 2062 6f78   as bounding box
-00002350: 6573 2061 6e64 2063 656e 7472 6f69 6473  es and centroids
-00002360: 0a0a 6060 6070 7974 686f 6e0a 626c 6f62  ..```python.blob
-00002370: 732e 706c 6f74 5f62 6f78 2863 6f6c 6f72  s.plot_box(color
-00002380: 3d22 6722 2c20 6c69 6e65 7769 6474 683d  ="g", linewidth=
-00002390: 3229 2020 2320 7075 7420 6120 6772 6565  2)  # put a gree
-000023a0: 6e20 626f 756e 6469 6e67 2062 6f78 206f  n bounding box o
-000023b0: 6e20 6561 6368 2062 6c6f 620a 626c 6f62  n each blob.blob
-000023c0: 732e 706c 6f74 5f63 656e 7472 6f69 6428  s.plot_centroid(
-000023d0: 6c61 6265 6c3d 5472 7565 2920 2023 2070  label=True)  # p
-000023e0: 7574 2061 2063 6972 636c 652b 6372 6f73  ut a circle+cros
-000023f0: 7320 6f6e 2074 6865 2063 656e 7472 6f69  s on the centroi
-00002400: 6420 6f66 2065 6163 6820 626c 6f62 0a70  d of each blob.p
-00002410: 6c74 2e73 686f 7728 626c 6f63 6b3d 5472  lt.show(block=Tr
-00002420: 7565 2920 2023 2064 6973 706c 6179 2074  ue)  # display t
-00002430: 6865 2072 6573 756c 740a 6060 600a 0a21  he result.```..!
-00002440: 5b42 696e 6172 7920 696d 6167 6520 7368  [Binary image sh
-00002450: 6f77 696e 6720 626f 756e 6469 6e67 2062  owing bounding b
-00002460: 6f78 6573 2061 6e64 2063 656e 7472 6f69  oxes and centroi
-00002470: 6473 5d28 6874 7470 733a 2f2f 6769 7468  ds](https://gith
-00002480: 7562 2e63 6f6d 2f70 6574 6572 636f 726b  ub.com/petercork
-00002490: 652f 6d61 6368 696e 6576 6973 696f 6e2d  e/machinevision-
-000024a0: 746f 6f6c 626f 782d 7079 7468 6f6e 2f72  toolbox-python/r
-000024b0: 6177 2f6d 6173 7465 722f 6669 6773 2f73  aw/master/figs/s
-000024c0: 6861 726b 322b 626f 7865 732e 706e 6729  hark2+boxes.png)
-000024d0: 0a0a 2323 2323 2042 696e 6172 7920 626c  ..#### Binary bl
-000024e0: 6f62 2068 6965 7261 7263 6879 0a0a 4120  ob hierarchy..A 
-000024f0: 6d6f 7265 2063 6f6d 706c 6578 2069 6d61  more complex ima
-00002500: 6765 2069 730a 0a60 6060 7079 7468 6f6e  ge is..```python
-00002510: 0a69 6d20 3d20 496d 6167 652e 5265 6164  .im = Image.Read
-00002520: 2822 6d75 6c74 6962 6c6f 6273 2e70 6e67  ("multiblobs.png
-00002530: 2229 0a69 6d2e 6469 7370 2829 0a60 6060  ").im.disp().```
-00002540: 0a0a 215b 4269 6e61 7279 2069 6d61 6765  ..![Binary image
-00002550: 2077 6974 6820 6e65 7374 6564 2062 6c6f   with nested blo
-00002560: 6273 5d28 6874 7470 733a 2f2f 6769 7468  bs](https://gith
-00002570: 7562 2e63 6f6d 2f70 6574 6572 636f 726b  ub.com/petercork
-00002580: 652f 6d61 6368 696e 6576 6973 696f 6e2d  e/machinevision-
-00002590: 746f 6f6c 626f 782d 7079 7468 6f6e 2f72  toolbox-python/r
-000025a0: 6177 2f6d 6173 7465 722f 6669 6773 2f6d  aw/master/figs/m
-000025b0: 756c 7469 2e70 6e67 290a 0a61 6e64 2077  ulti.png)..and w
-000025c0: 6520 7365 6520 7468 6174 2073 6f6d 6520  e see that some 
-000025d0: 626c 6f62 7320 6172 6520 636f 6e74 6169  blobs are contai
-000025e0: 6e65 6420 7769 7468 696e 206f 7468 6572  ned within other
-000025f0: 2062 6c6f 6273 2e20 5468 6520 7265 7375   blobs. The resu
-00002600: 6c74 7320 696e 2074 6162 756c 6172 2066  lts in tabular f
-00002610: 6f72 6d0a 0a60 6060 7079 7468 6f6e 0a62  orm..```python.b
-00002620: 6c6f 6273 2020 3d20 696d 2e62 6c6f 6273  lobs  = im.blobs
-00002630: 2829 0a70 7269 6e74 2862 6c6f 6273 290a  ().print(blobs).
-00002640: 09e2 948c e294 80e2 9480 e294 80e2 94ac  ................
-00002650: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002660: 9480 e294 80e2 9480 e294 ace2 9480 e294  ................
-00002670: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002680: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002690: 9480 e294 80e2 9480 e294 ace2 9480 e294  ................
-000026a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000026b0: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
-000026c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000026d0: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
-000026e0: e294 80e2 9480 e294 80e2 9480 e294 ace2  ................
-000026f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002700: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002710: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
-00002720: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002730: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
-00002740: e294 80e2 9480 e294 80e2 9480 e294 900a  ................
-00002750: 09e2 9482 6964 20e2 9482 2070 6172 656e  ....id ... paren
-00002760: 7420 e294 8220 2020 2020 2063 656e 7472  t ...      centr
-00002770: 6f69 6420 e294 8220 2020 2020 6172 6561  oid ...     area
-00002780: 20e2 9482 2074 6f75 6368 20e2 9482 2020   ... touch ...  
-00002790: 7065 7269 6d20 e294 8220 6369 7263 756c  perim ... circul
-000027a0: 6172 6974 7920 e294 8220 6f72 6965 6e74  arity ... orient
-000027b0: 20e2 9482 2061 7370 6563 7420 e294 820a   ... aspect ....
-000027c0: 09e2 949c e294 80e2 9480 e294 80e2 94bc  ................
-000027d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000027e0: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-000027f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002800: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002810: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-00002820: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002830: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00002840: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002850: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-00002860: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-00002870: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002880: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002890: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-000028a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000028b0: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-000028c0: e294 80e2 9480 e294 80e2 9480 e294 a40a  ................
-000028d0: 09e2 9482 2030 20e2 9482 2020 2020 2020  .... 0 ...      
-000028e0: 3120 e294 8220 2038 3938 2e38 2c20 3732  1 ...  898.8, 72
-000028f0: 352e 3320 e294 8220 312e 3635 652b 3035  5.3 ... 1.65e+05
-00002900: 20e2 9482 2046 616c 7365 20e2 9482 2032   ... False ... 2
-00002910: 3232 302e 3020 e294 8220 2020 2020 2020  220.0 ...       
-00002920: 302e 3436 3720 e294 8220 2038 362e 37c2  0.467 ...  86.7.
-00002930: b020 e294 8220 2030 2e37 3534 20e2 9482  . ...  0.754 ...
-00002940: 0a09 e294 8220 3120 e294 8220 2020 2020  ..... 1 ...     
-00002950: 2032 20e2 9482 2031 3032 352e 302c 2038   2 ... 1025.0, 8
-00002960: 3133 2e37 20e2 9482 2031 2e30 3665 2b30  13.7 ... 1.06e+0
-00002970: 3520 e294 8220 4661 6c73 6520 e294 8220  5 ... False ... 
-00002980: 3133 3837 2e39 20e2 9482 2020 2020 2020  1387.9 ...      
-00002990: 2030 2e37 3639 20e2 9482 202d 3838 2e39   0.769 ... -88.9
-000029a0: c2b0 20e2 9482 2020 302e 3733 3920 e294  .. ...  0.739 ..
-000029b0: 820a 09e2 9482 2032 20e2 9482 2020 2020  ...... 2 ...    
-000029c0: 202d 3120 e294 8220 2039 3338 2e31 2c20   -1 ...  938.1, 
-000029d0: 3835 352e 3220 e294 8220 312e 3732 652b  855.2 ... 1.72e+
-000029e0: 3034 20e2 9482 2046 616c 7365 20e2 9482  04 ... False ...
-000029f0: 2020 3439 302e 3720 e294 8220 2020 2020    490.7 ...     
-00002a00: 2020 312e 3030 3120 e294 8220 2038 382e    1.001 ...  88.
-00002a10: 37c2 b020 e294 8220 2030 2e38 3632 20e2  7.. ...  0.862 .
-00002a20: 9482 0a09 e294 8220 3320 e294 8220 2020  ....... 3 ...   
-00002a30: 2020 2d31 20e2 9482 2020 3938 382e 312c    -1 ...  988.1,
-00002a40: 2036 3937 2e32 20e2 9482 2031 2e32 3165   697.2 ... 1.21e
-00002a50: 2b30 3420 e294 8220 4661 6c73 6520 e294  +04 ... False ..
-00002a60: 8220 2034 3132 2e35 20e2 9482 2020 2020  .  412.5 ...    
-00002a70: 2020 2030 2e39 3934 20e2 9482 202d 3837     0.994 ... -87
-00002a80: 2e38 c2b0 20e2 9482 2020 302e 3830 3920  .8.. ...  0.809 
-00002a90: e294 820a 09e2 9482 2034 20e2 9482 2020  ........ 4 ...  
-00002aa0: 2020 202d 3120 e294 8220 2038 3436 2e30     -1 ...  846.0
-00002ab0: 2c20 3531 312e 3720 e294 8220 312e 3735  , 511.7 ... 1.75
-00002ac0: 652b 3034 20e2 9482 2046 616c 7365 20e2  e+04 ... False .
-00002ad0: 9482 2020 3439 362e 3920 e294 8220 2020  ..  496.9 ...   
-00002ae0: 2020 2020 302e 3939 3220 e294 8220 2d39      0.992 ... -9
-00002af0: 302e 30c2 b020 e294 8220 2030 2e37 3738  0.0.. ...  0.778
-00002b00: 20e2 9482 0a09 e294 8220 3520 e294 8220   ........ 5 ... 
-00002b10: 2020 2020 2036 20e2 9482 2020 3239 312e       6 ...  291.
-00002b20: 372c 2033 3737 2e38 20e2 9482 2020 312e  7, 377.8 ...  1.
-00002b30: 3765 2b30 3520 e294 8220 4661 6c73 6520  7e+05 ... False 
-00002b40: e294 8220 3137 3132 2e36 20e2 9482 2020  ... 1712.6 ...  
-00002b50: 2020 2020 2030 2e38 3130 20e2 9482 202d       0.810 ... -
-00002b60: 3835 2e33 c2b0 20e2 9482 2020 302e 3736  85.3.. ...  0.76
-00002b70: 3720 e294 820a 09e2 9482 2036 20e2 9482  7 ........ 6 ...
-00002b80: 2020 2020 202d 3120 e294 8220 2033 3132       -1 ...  312
-00002b90: 2e37 2c20 3437 322e 3120 e294 8220 312e  .7, 472.1 ... 1.
-00002ba0: 3735 652b 3034 20e2 9482 2046 616c 7365  75e+04 ... False
-00002bb0: 20e2 9482 2020 3439 352e 3520 e294 8220   ...  495.5 ... 
-00002bc0: 2020 2020 2020 302e 3939 3720 e294 8220        0.997 ... 
-00002bd0: 2d38 392e 39c2 b020 e294 8220 2030 2e37  -89.9.. ...  0.7
-00002be0: 3737 20e2 9482 0a09 e294 8220 3720 e294  77 ........ 7 ..
-00002bf0: 8220 2020 2020 2d31 20e2 9482 2020 3234  .     -1 ...  24
-00002c00: 312e 392c 2032 3435 2e30 20e2 9482 2031  1.9, 245.0 ... 1
-00002c10: 2e37 3565 2b30 3420 e294 8220 4661 6c73  .75e+04 ... Fals
-00002c20: 6520 e294 8220 2034 3936 2e39 20e2 9482  e ...  496.9 ...
-00002c30: 2020 2020 2020 2030 2e39 3932 20e2 9482         0.992 ...
-00002c40: 202d 3930 2e30 c2b0 20e2 9482 2020 302e   -90.0.. ...  0.
-00002c50: 3737 3720 e294 820a 09e2 9482 2038 20e2  777 ........ 8 .
-00002c60: 9482 2020 2020 2020 3920 e294 8220 3132  ..      9 ... 12
-00002c70: 3238 2e30 2c20 3235 342e 3320 e294 8220  28.0, 254.3 ... 
-00002c80: 382e 3134 652b 3034 20e2 9482 2046 616c  8.14e+04 ... Fal
-00002c90: 7365 20e2 9482 2031 3231 352e 3220 e294  se ... 1215.2 ..
-00002ca0: 8220 2020 2020 2020 302e 3737 3120 e294  .       0.771 ..
-00002cb0: 8220 2d37 372e 32c2 b020 e294 8220 2030  . -77.2.. ...  0
-00002cc0: 2e37 3133 20e2 9482 0a09 e294 8220 3920  .713 ........ 9 
-00002cd0: e294 8220 2020 2020 2d31 20e2 9482 2031  ...     -1 ... 1
-00002ce0: 3232 352e 322c 2032 3230 2e30 20e2 9482  225.2, 220.0 ...
-00002cf0: 2031 2e37 3565 2b30 3420 e294 8220 4661   1.75e+04 ... Fa
-00002d00: 6c73 6520 e294 8220 2034 3936 2e39 20e2  lse ...  496.9 .
-00002d10: 9482 2020 2020 2020 2030 2e39 3932 20e2  ..       0.992 .
-00002d20: 9482 202d 3930 2e30 c2b0 20e2 9482 2020  .. -90.0.. ...  
-00002d30: 302e 3737 3720 e294 820a 09e2 9494 e294  0.777 ..........
-00002d40: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
-00002d50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002d60: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
-00002d70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002d80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00002d90: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
-00002da0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002db0: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
-00002dc0: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
-00002dd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002de0: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
-00002df0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00002e00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002e10: e294 b4e2 9480 e294 80e2 9480 e294 80e2  ................
-00002e20: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
-00002e30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00002e40: e294 80e2 9480 e294 980a 6060 600a 0a57  ..........```..W
-00002e50: 6520 6361 6e20 6469 7370 6c61 7920 6120  e can display a 
-00002e60: 6c61 6265 6c20 696d 6167 652c 2077 6865  label image, whe
-00002e70: 7265 2074 6865 2076 616c 7565 206f 6620  re the value of 
-00002e80: 6561 6368 2070 6978 656c 2069 7320 7468  each pixel is th
-00002e90: 6520 6c61 6265 6c20 6f66 2074 6865 2062  e label of the b
-00002ea0: 6c6f 6220 7468 6174 2074 6865 2070 6978  lob that the pix
-00002eb0: 656c 0a62 656c 6f6e 6773 2074 6f2c 2074  el.belongs to, t
-00002ec0: 6865 2060 6964 6020 6174 7472 6962 7574  he `id` attribut
-00002ed0: 650a 0a60 6060 7079 7468 6f6e 0a6c 6162  e..```python.lab
-00002ee0: 656c 7320 3d20 626c 6f62 732e 6c61 6265  els = blobs.labe
-00002ef0: 6c5f 696d 6167 6528 290a 6c61 6265 6c73  l_image().labels
-00002f00: 2e64 6973 7028 636f 6c6f 726d 6170 3d22  .disp(colormap="
-00002f10: 7669 7269 6469 7322 2c20 6e63 6f6c 6f72  viridis", ncolor
-00002f20: 733d 6c65 6e28 626c 6f62 7329 2c20 636f  s=len(blobs), co
-00002f30: 6c6f 7262 6172 3d64 6963 7428 7368 7269  lorbar=dict(shri
-00002f40: 6e6b 3d30 2e38 2c20 6173 7065 6374 3d32  nk=0.8, aspect=2
-00002f50: 302a 302e 3829 290a 6060 600a 0a21 5b46  0*0.8)).```..![F
-00002f60: 616c 7365 2063 6f6c 6f72 206c 6162 656c  alse color label
-00002f70: 2069 6d61 6765 5d28 6874 7470 733a 2f2f   image](https://
-00002f80: 6769 7468 7562 2e63 6f6d 2f70 6574 6572  github.com/peter
-00002f90: 636f 726b 652f 6d61 6368 696e 6576 6973  corke/machinevis
-00002fa0: 696f 6e2d 746f 6f6c 626f 782d 7079 7468  ion-toolbox-pyth
-00002fb0: 6f6e 2f72 6177 2f6d 6173 7465 722f 6669  on/raw/master/fi
-00002fc0: 6773 2f6d 756c 7469 5f6c 6162 656c 6c65  gs/multi_labelle
-00002fd0: 642e 706e 6729 0a0a 5765 2063 616e 2061  d.png)..We can a
-00002fe0: 6c73 6f20 7468 696e 6b20 6f66 2074 6865  lso think of the
-00002ff0: 2062 6c6f 6273 2066 6f72 6d69 6e67 2061   blobs forming a
-00003000: 2068 6965 6172 6368 7920 616e 6420 7468   hiearchy and th
-00003010: 6174 2072 656c 6174 696f 6e73 6869 7020  at relationship 
-00003020: 6973 2072 6566 6c65 6374 6564 2069 6e20  is reflected in 
-00003030: 7468 6520 6070 6172 656e 7460 2061 6e64  the `parent` and
-00003040: 2060 6368 696c 6472 656e 6020 6174 7472   `children` attr
-00003050: 6962 7574 6573 206f 6620 7468 6520 626c  ibutes of the bl
-00003060: 6f62 732e 0a57 6520 6361 6e20 616c 736f  obs..We can also
-00003070: 2065 7870 7265 7373 2069 7420 6173 2061   express it as a
-00003080: 2064 6972 6563 7465 6420 6772 6170 680a   directed graph.
-00003090: 0a60 6060 7079 7468 6f6e 0a62 6c6f 6273  .```python.blobs
-000030a0: 2e64 6f74 6669 6c65 2873 686f 773d 5472  .dotfile(show=Tr
-000030b0: 7565 290a 6060 600a 0a21 5b42 6c6f 6220  ue).```..![Blob 
-000030c0: 6869 6572 6172 6368 7920 6173 2061 2067  hierarchy as a g
-000030d0: 7261 7068 5d28 6874 7470 733a 2f2f 6769  raph](https://gi
-000030e0: 7468 7562 2e63 6f6d 2f70 6574 6572 636f  thub.com/peterco
-000030f0: 726b 652f 6d61 6368 696e 6576 6973 696f  rke/machinevisio
-00003100: 6e2d 746f 6f6c 626f 782d 7079 7468 6f6e  n-toolbox-python
-00003110: 2f72 6177 2f6d 6173 7465 722f 6669 6773  /raw/master/figs
-00003120: 2f62 6c6f 6273 5f67 7261 7068 2e70 6e67  /blobs_graph.png
-00003130: 290a 0a23 2323 2043 616d 6572 6120 6d6f  )..### Camera mo
-00003140: 6465 6c6c 696e 670a 0a60 6060 7079 7468  delling..```pyth
-00003150: 6f6e 0a66 726f 6d20 6d61 6368 696e 6576  on.from machinev
-00003160: 6973 696f 6e74 6f6f 6c62 6f78 2069 6d70  isiontoolbox imp
-00003170: 6f72 7420 4365 6e74 7261 6c43 616d 6572  ort CentralCamer
-00003180: 610a 6361 6d20 3d20 4365 6e74 7261 6c43  a.cam = CentralC
-00003190: 616d 6572 6128 663d 302e 3031 352c 2072  amera(f=0.015, r
-000031a0: 686f 3d31 3065 2d36 2c20 696d 6167 6573  ho=10e-6, images
-000031b0: 697a 653d 5b31 3238 302c 2031 3032 345d  ize=[1280, 1024]
-000031c0: 2c20 7070 3d5b 3634 302c 2035 3132 5d2c  , pp=[640, 512],
-000031d0: 206e 616d 653d 226d 7963 616d 6572 6122   name="mycamera"
-000031e0: 290a 7072 696e 7428 6361 6d29 0a20 2020  ).print(cam).   
-000031f0: 2020 2020 2020 2020 4e61 6d65 3a20 6d79          Name: my
-00003200: 6361 6d65 7261 205b 4365 6e74 7261 6c43  camera [CentralC
-00003210: 616d 6572 615d 0a20 2020 2020 7069 7865  amera].     pixe
-00003220: 6c20 7369 7a65 3a20 3165 2d30 3520 7820  l size: 1e-05 x 
-00003230: 3165 2d30 350a 2020 2020 2069 6d61 6765  1e-05.     image
-00003240: 2073 697a 653a 2031 3238 3020 7820 3130   size: 1280 x 10
-00003250: 3234 0a20 2020 2020 2020 2020 2020 706f  24.           po
-00003260: 7365 3a20 7420 3d20 302c 2030 2c20 303b  se: t = 0, 0, 0;
-00003270: 2072 7079 2f79 787a 203d 2030 c2b0 2c20   rpy/yxz = 0.., 
-00003280: 30c2 b02c 2030 c2b0 0a20 2020 7072 696e  0.., 0...   prin
-00003290: 6369 7061 6c20 7074 3a20 5b20 2020 2020  cipal pt: [     
-000032a0: 3634 3020 2020 2020 2035 3132 5d0a 2020  640      512].  
-000032b0: 2066 6f63 616c 206c 656e 6774 683a 205b   focal length: [
-000032c0: 2020 2030 2e30 3135 2020 2020 302e 3031     0.015    0.01
-000032d0: 355d 0a60 6060 0a0a 616e 6420 6974 7320  5].```..and its 
-000032e0: 696e 7472 696e 7369 6320 7061 7261 6d65  intrinsic parame
-000032f0: 7465 7273 2061 7265 0a0a 6060 6070 7974  ters are..```pyt
-00003300: 686f 6e0a 7072 696e 7428 6361 6d2e 4b29  hon.print(cam.K)
-00003310: 0a09 5b5b 312e 3530 652b 3033 2030 2e30  ..[[1.50e+03 0.0
-00003320: 3065 2b30 3020 362e 3430 652b 3032 5d0a  0e+00 6.40e+02].
-00003330: 0920 5b30 2e30 3065 2b30 3020 312e 3530  . [0.00e+00 1.50
-00003340: 652b 3033 2035 2e31 3265 2b30 325d 0a09  e+03 5.12e+02]..
-00003350: 205b 302e 3030 652b 3030 2030 2e30 3065   [0.00e+00 0.00e
-00003360: 2b30 3020 312e 3030 652b 3030 5d5d 0a60  +00 1.00e+00]].`
-00003370: 6060 0a0a 5765 2063 616e 2064 6566 696e  ``..We can defin
-00003380: 6520 616e 2061 7262 6974 7261 7279 2070  e an arbitrary p
-00003390: 6f69 6e74 2069 6e20 7468 6520 776f 726c  oint in the worl
-000033a0: 640a 0a60 6060 7079 7468 6f6e 0a50 203d  d..```python.P =
-000033b0: 205b 302e 332c 2030 2e34 2c20 332e 305d   [0.3, 0.4, 3.0]
-000033c0: 0a60 6060 0a0a 616e 6420 7468 656e 2070  .```..and then p
-000033d0: 726f 6a65 6374 2069 7420 696e 746f 2074  roject it into t
-000033e0: 6865 2063 616d 6572 610a 0a60 6060 7079  he camera..```py
-000033f0: 7468 6f6e 0a70 203d 2063 616d 2e70 726f  thon.p = cam.pro
-00003400: 6a65 6374 2850 290a 7072 696e 7428 7029  ject(P).print(p)
-00003410: 0a09 5b37 3930 2e20 3731 322e 5d0a 6060  ..[790. 712.].``
-00003420: 600a 0a77 6869 6368 2069 7320 7468 6520  `..which is the 
-00003430: 636f 7272 6573 706f 6e64 696e 6720 636f  corresponding co
-00003440: 6f72 6469 6e61 7465 2069 6e20 7069 7865  ordinate in pixe
-00003450: 6c73 2e20 4966 2077 6520 7368 6966 7420  ls. If we shift 
-00003460: 7468 6520 6361 6d65 7261 2073 6c69 6768  the camera sligh
-00003470: 746c 7920 7468 6520 696d 6167 6520 706c  tly the image pl
-00003480: 616e 6520 636f 6f72 6469 6e61 7465 2077  ane coordinate w
-00003490: 696c 6c20 616c 736f 2063 6861 6e67 650a  ill also change.
-000034a0: 0a60 6060 7079 7468 6f6e 0a70 203d 2063  .```python.p = c
-000034b0: 616d 2e70 726f 6a65 6374 2850 2c20 543d  am.project(P, T=
-000034c0: 5345 3328 302e 312c 2030 2c20 3029 2029  SE3(0.1, 0, 0) )
-000034d0: 0a70 7269 6e74 2870 290a 5b37 3430 2e20  .print(p).[740. 
-000034e0: 3731 322e 5d0a 6060 600a 0a57 6520 6361  712.].```..We ca
-000034f0: 6e20 6465 6669 6e65 2061 6e20 6564 6765  n define an edge
-00003500: 2d62 6173 6564 2063 7562 6520 6d6f 6465  -based cube mode
-00003510: 6c20 616e 6420 7072 6f6a 6563 7420 6974  l and project it
-00003520: 2069 6e74 6f20 7468 6520 6361 6d65 7261   into the camera
-00003530: 2773 2069 6d61 6765 2070 6c61 6e65 0a0a  's image plane..
-00003540: 6060 6070 7974 686f 6e0a 6672 6f6d 2073  ```python.from s
-00003550: 7061 7469 616c 6d61 7468 2069 6d70 6f72  patialmath impor
-00003560: 7420 5345 330a 582c 2059 2c20 5a20 3d20  t SE3.X, Y, Z = 
-00003570: 6d6b 6375 6265 2830 2e32 2c20 706f 7365  mkcube(0.2, pose
-00003580: 3d53 4533 2830 2c20 302c 2031 292c 2065  =SE3(0, 0, 1), e
-00003590: 6467 653d 5472 7565 290a 6361 6d2e 706c  dge=True).cam.pl
-000035a0: 6f74 5f77 6972 6566 7261 6d65 2858 2c20  ot_wireframe(X, 
-000035b0: 592c 205a 290a 6060 600a 0a21 5b50 6572  Y, Z).```..![Per
-000035c0: 7370 6563 7469 7665 2063 616d 6572 6120  spective camera 
-000035d0: 7669 6577 206f 6620 6375 6265 5d28 6874  view of cube](ht
-000035e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000035f0: 2f70 6574 6572 636f 726b 652f 6d61 6368  /petercorke/mach
-00003600: 696e 6576 6973 696f 6e2d 746f 6f6c 626f  inevision-toolbo
-00003610: 782d 7079 7468 6f6e 2f72 6177 2f6d 6173  x-python/raw/mas
-00003620: 7465 722f 6669 6773 2f63 7562 652e 706e  ter/figs/cube.pn
-00003630: 6729 0a0a 3c21 2d2d 2d6f 7220 7769 7468  g)..<!---or with
-00003640: 2061 2066 6973 6865 7965 2063 616d 6572   a fisheye camer
-00003650: 610a 0a60 6060 6d61 746c 6162 0a3e 3e20  a..```matlab.>> 
-00003660: 6361 6d20 3d20 4669 7368 4579 6543 616d  cam = FishEyeCam
-00003670: 6572 6128 276e 616d 6527 2c20 2766 6973  era('name', 'fis
-00003680: 6865 7965 272c 202e 2e2e 0a27 7072 6f6a  heye', ....'proj
-00003690: 6563 7469 6f6e 272c 2027 6571 7569 616e  ection', 'equian
-000036a0: 6775 6c61 7227 2c20 2e2e 2e0a 2770 6978  gular', ....'pix
-000036b0: 656c 272c 2031 3065 2d36 2c20 2e2e 2e0a  el', 10e-6, ....
-000036c0: 2772 6573 6f6c 7574 696f 6e27 2c20 5b31  'resolution', [1
-000036d0: 3238 3020 3130 3234 5d29 3b0a 3e3e 205b  280 1024]);.>> [
-000036e0: 582c 592c 5a5d 203d 206d 6b63 7562 6528  X,Y,Z] = mkcube(
-000036f0: 302e 322c 2027 6365 6e74 7265 272c 205b  0.2, 'centre', [
-00003700: 302e 322c 2030 2c20 302e 335d 2c20 2765  0.2, 0, 0.3], 'e
-00003710: 6467 6527 293b 0a3e 3e20 6361 6d2e 6d65  dge');.>> cam.me
-00003720: 7368 2858 2c20 592c 205a 293b 0a60 6060  sh(X, Y, Z);.```
-00003730: 0a21 5b46 6973 6865 7965 206c 656e 7320  .![Fisheye lens 
-00003740: 6361 6d65 7261 2076 6965 775d 2866 6967  camera view](fig
-00003750: 732f 6375 6265 5f66 6973 6865 7965 2e70  s/cube_fisheye.p
-00003760: 6e67 290a 0a0a 2323 2320 4275 6e64 6c65  ng)...### Bundle
-00003770: 2061 646a 7573 746d 656e 740a 2d2d 2d3e   adjustment.--->
-00003780: 0a0a 2323 2320 436f 6c6f 7220 7370 6163  ..### Color spac
-00003790: 650a 0a50 6c6f 7420 7468 6520 4349 4520  e..Plot the CIE 
-000037a0: 6368 726f 6d61 7469 6369 7479 2073 7061  chromaticity spa
-000037b0: 6365 0a0a 6060 6070 7974 686f 6e0a 706c  ce..```python.pl
-000037c0: 6f74 5f63 6872 6f6d 6174 6963 6974 795f  ot_chromaticity_
-000037d0: 6469 6167 7261 6d28 2278 7922 293b 0a70  diagram("xy");.p
-000037e0: 6c6f 745f 7370 6563 7472 616c 5f6c 6f63  lot_spectral_loc
-000037f0: 7573 2822 7879 2229 0a60 6060 0a0a 215b  us("xy").```..![
-00003800: 4349 4520 6368 726f 6d61 7469 6369 7479  CIE chromaticity
-00003810: 2073 7061 6365 5d28 6874 7470 733a 2f2f   space](https://
-00003820: 6769 7468 7562 2e63 6f6d 2f70 6574 6572  github.com/peter
-00003830: 636f 726b 652f 6d61 6368 696e 6576 6973  corke/machinevis
-00003840: 696f 6e2d 746f 6f6c 626f 782d 7079 7468  ion-toolbox-pyth
-00003850: 6f6e 2f72 6177 2f6d 6173 7465 722f 6669  on/raw/master/fi
-00003860: 6773 2f63 6f6c 6f72 7370 6163 652e 706e  gs/colorspace.pn
-00003870: 6729 0a0a 4c6f 6164 2074 6865 2073 7065  g)..Load the spe
-00003880: 6374 7275 6d20 6f66 2073 756e 6c69 6768  ctrum of sunligh
-00003890: 7420 6174 2074 6865 2045 6172 7468 2773  t at the Earth's
-000038a0: 2073 7572 6661 6365 2061 6e64 2063 6f6d   surface and com
-000038b0: 7075 7465 2074 6865 2043 4945 2078 7920  pute the CIE xy 
-000038c0: 6368 726f 6d61 7469 6369 7479 2063 6f6f  chromaticity coo
-000038d0: 7264 696e 6174 6573 0a0a 6060 6070 7974  rdinates..```pyt
-000038e0: 686f 6e0a 6e6d 203d 2031 652d 390a 6c61  hon.nm = 1e-9.la
-000038f0: 6d20 3d20 6e70 2e6c 696e 7370 6163 6528  m = np.linspace(
-00003900: 3430 302c 2037 3031 2c20 3529 202a 206e  400, 701, 5) * n
-00003910: 6d20 2320 7669 7369 626c 6520 6c69 6768  m # visible ligh
-00003920: 740a 7375 6e5f 6174 5f67 726f 756e 6420  t.sun_at_ground 
-00003930: 3d20 6c6f 6164 7370 6563 7472 756d 286c  = loadspectrum(l
-00003940: 616d 2c20 2273 6f6c 6172 2229 0a78 7920  am, "solar").xy 
-00003950: 3d20 6c61 6d62 6461 3278 7928 6c61 6d62  = lambda2xy(lamb
-00003960: 6461 2c20 7375 6e5f 6174 5f67 726f 756e  da, sun_at_groun
-00003970: 6429 0a70 7269 6e74 2878 7929 0a09 5b5b  d).print(xy)..[[
-00003980: 302e 3333 3237 3237 3938 2030 2e33 3435  0.33272798 0.345
-00003990: 3430 3133 205d 5d0a 7072 696e 7428 636f  4013 ]].print(co
-000039a0: 6c6f 726e 616d 6528 7879 2c20 2278 7922  lorname(xy, "xy"
-000039b0: 2929 0a09 6b68 616b 690a 6060 600a 0a23  ))..khaki.```..#
-000039c0: 2323 2048 6f75 6768 2074 7261 6e73 666f  ## Hough transfo
-000039d0: 726d 0a0a 6060 6070 7974 686f 6e0a 696d  rm..```python.im
-000039e0: 203d 2049 6d61 6765 2e52 6561 6428 2263   = Image.Read("c
-000039f0: 6875 7263 682e 706e 6722 2c20 6d6f 6e6f  hurch.png", mono
-00003a00: 3d54 7275 6529 0a65 6467 6573 203d 2069  =True).edges = i
-00003a10: 6d2e 6361 6e6e 7928 290a 6820 3d20 6564  m.canny().h = ed
-00003a20: 6765 732e 486f 7567 6828 290a 6c69 6e65  ges.Hough().line
-00003a30: 7320 3d20 682e 6c69 6e65 735f 7028 3130  s = h.lines_p(10
-00003a40: 302c 206d 696e 6c69 6e65 6c65 6e67 7468  0, minlinelength
-00003a50: 3d32 3030 2c20 6d61 786c 696e 6567 6170  =200, maxlinegap
-00003a60: 3d35 2c20 7365 6564 3d30 290a 0a69 6d2e  =5, seed=0)..im.
-00003a70: 6469 7370 2864 6172 6b65 6e3d 5472 7565  disp(darken=True
-00003a80: 290a 682e 706c 6f74 5f6c 696e 6573 286c  ).h.plot_lines(l
-00003a90: 696e 6573 2c20 2272 2d2d 2229 0a60 6060  ines, "r--").```
-00003aa0: 0a0a 215b 486f 7567 6820 7472 616e 7366  ..![Hough transf
-00003ab0: 6f72 6d5d 2868 7474 7073 3a2f 2f67 6974  orm](https://git
-00003ac0: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
-00003ad0: 6b65 2f6d 6163 6869 6e65 7669 7369 6f6e  ke/machinevision
-00003ae0: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e2f  -toolbox-python/
-00003af0: 7261 772f 6d61 7374 6572 2f66 6967 732f  raw/master/figs/
-00003b00: 686f 7567 682e 706e 6729 0a0a 2323 2320  hough.png)..### 
-00003b10: 5355 5246 2066 6561 7475 7265 730a 0a57  SURF features..W
-00003b20: 6520 6c6f 6164 2074 776f 2069 6d61 6765  e load two image
-00003b30: 7320 616e 6420 636f 6d70 7574 6520 6120  s and compute a 
-00003b40: 7365 7420 6f66 2053 5552 4620 6665 6174  set of SURF feat
-00003b50: 7572 6573 2066 6f72 2065 6163 680a 0a60  ures for each..`
-00003b60: 6060 7079 7468 6f6e 0a76 6965 7731 203d  ``python.view1 =
-00003b70: 2049 6d61 6765 2e52 6561 6428 2265 6966   Image.Read("eif
-00003b80: 6665 6c2d 312e 706e 6722 2c20 6d6f 6e6f  fel-1.png", mono
-00003b90: 3d54 7275 6529 0a76 6965 7732 203d 2049  =True).view2 = I
-00003ba0: 6d61 6765 2e52 6561 6428 2265 6966 6665  mage.Read("eiffe
-00003bb0: 6c2d 322e 706e 6722 2c20 6d6f 6e6f 3d54  l-2.png", mono=T
-00003bc0: 7275 6529 0a73 6631 203d 2076 6965 7731  rue).sf1 = view1
-00003bd0: 2e53 4946 5428 290a 7366 3220 3d20 7669  .SIFT().sf2 = vi
-00003be0: 6577 322e 5349 4654 2829 0a60 6060 0a0a  ew2.SIFT().```..
-00003bf0: 5765 2063 616e 206d 6174 6368 2066 6561  We can match fea
-00003c00: 7475 7265 7320 6265 7477 6565 6e20 696d  tures between im
-00003c10: 6167 6573 2062 6173 6564 2070 7572 656c  ages based purel
-00003c20: 7920 6f6e 2074 6865 2073 696d 696c 6172  y on the similar
-00003c30: 6974 7920 6f66 2074 6865 2066 6561 7475  ity of the featu
-00003c40: 7265 732c 2061 6e64 2064 6973 706c 6179  res, and display
-00003c50: 2074 6865 2063 6f72 7265 7370 6f6e 6465   the corresponde
-00003c60: 6e63 6573 2066 6f75 6e64 0a0a 6060 6070  nces found..```p
-00003c70: 7974 686f 6e0a 6d61 7463 6865 7320 3d20  ython.matches = 
-00003c80: 7366 312e 6d61 7463 6828 7366 3229 0a70  sf1.match(sf2).p
-00003c90: 7269 6e74 286d 6174 6368 6573 290a 3831  rint(matches).81
-00003ca0: 3320 6d61 7463 6865 730a 6d61 7463 6865  3 matches.matche
-00003cb0: 735b 313a 355d 2e74 6162 6c65 2829 0ae2  s[1:5].table()..
-00003cc0: 948c e294 80e2 9480 e294 ace2 9480 e294  ................
-00003cd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003ce0: e294 80e2 94ac e294 80e2 9480 e294 80e2  ................
-00003cf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003d00: 80e2 9480 e294 ace2 9480 e294 80e2 9480  ................
-00003d10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003d20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003d30: 80e2 9480 e294 80e2 9480 e294 ace2 9480  ................
-00003d40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003d50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003d60: 80e2 9480 e294 80e2 9480 e294 80e2 9490  ................
-00003d70: 0ae2 9482 2320 e294 8220 696e 6c69 6572  ....# ... inlier
-00003d80: 20e2 9482 2073 7472 656e 6774 6820 e294   ... strength ..
-00003d90: 8220 2020 2020 2020 2020 2020 2020 2070  .              p
-00003da0: 3120 e294 8220 2020 2020 2020 2020 2020  1 ...           
-00003db0: 2020 7032 20e2 9482 0ae2 949c e294 80e2    p2 ...........
-00003dc0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-00003dd0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-00003de0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003df0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003e00: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003e10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003e20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003e30: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-00003e40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003e50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00003e60: 80e2 9480 e294 80e2 94a4 0ae2 9482 3020  ..............0 
-00003e70: e294 8220 2020 2020 2020 20e2 9482 2020  ...        ...  
-00003e80: 2020 2032 362e 3420 e294 8220 2831 3131     26.4 ... (111
-00003e90: 382e 362c 2031 3738 2e38 2920 e294 8220  8.6, 178.8) ... 
-00003ea0: 2839 3532 2e35 2c20 3431 382e 3029 20e2  (952.5, 418.0) .
-00003eb0: 9482 0ae2 9482 3120 e294 8220 2020 2020  ......1 ...     
-00003ec0: 2020 20e2 9482 2020 2020 2032 382e 3220     ...     28.2 
-00003ed0: e294 8220 2838 3230 2e36 2c20 3531 392e  ... (820.6, 519.
-00003ee0: 3129 2020 e294 8220 2837 3038 2e31 2c20  1)  ... (708.1, 
-00003ef0: 3730 312e 3629 20e2 9482 0ae2 9482 3220  701.6) .......2 
-00003f00: e294 8220 2020 2020 2020 20e2 9482 2020  ...        ...  
-00003f10: 2020 2032 392e 3620 e294 8220 2838 3031     29.6 ... (801
-00003f20: 2e31 2c20 3633 322e 3429 2020 e294 8220  .1, 632.4)  ... 
-00003f30: 2836 3934 2e31 2c20 3830 302e 3329 20e2  (694.1, 800.3) .
-00003f40: 9482 0ae2 9482 3320 e294 8220 2020 2020  ......3 ...     
-00003f50: 2020 20e2 9482 2020 2020 2033 322e 3420     ...     32.4 
-00003f60: e294 8220 2837 3436 2e30 2c20 3135 332e  ... (746.0, 153.
-00003f70: 3129 2020 e294 8220 2836 3434 2e35 2c20  1)  ... (644.5, 
-00003f80: 3339 322e 3229 20e2 9482 0ae2 9494 e294  392.2) .........
-00003f90: 80e2 9480 e294 b4e2 9480 e294 80e2 9480  ................
-00003fa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00003fb0: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
+000004c0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+000004d0: 4345 4e53 450a 5265 7175 6972 6573 2d44  CENSE.Requires-D
+000004e0: 6973 743a 206e 756d 7079 3e3d 312e 3137  ist: numpy>=1.17
+000004f0: 2e34 0a52 6571 7569 7265 732d 4469 7374  .4.Requires-Dist
+00000500: 3a20 7363 6970 790a 5265 7175 6972 6573  : scipy.Requires
+00000510: 2d44 6973 743a 206d 6174 706c 6f74 6c69  -Dist: matplotli
+00000520: 620a 5265 7175 6972 6573 2d44 6973 743a  b.Requires-Dist:
+00000530: 206f 7065 6e63 762d 7079 7468 6f6e 0a52   opencv-python.R
+00000540: 6571 7569 7265 732d 4469 7374 3a20 6f70  equires-Dist: op
+00000550: 656e 3364 0a52 6571 7569 7265 732d 4469  en3d.Requires-Di
+00000560: 7374 3a20 6f70 656e 6376 2d63 6f6e 7472  st: opencv-contr
+00000570: 6962 2d70 7974 686f 6e0a 5265 7175 6972  ib-python.Requir
+00000580: 6573 2d44 6973 743a 2073 7061 7469 616c  es-Dist: spatial
+00000590: 6d61 7468 2d70 7974 686f 6e0a 5265 7175  math-python.Requ
+000005a0: 6972 6573 2d44 6973 743a 2070 6772 6170  ires-Dist: pgrap
+000005b0: 682d 7079 7468 6f6e 0a52 6571 7569 7265  h-python.Require
+000005c0: 732d 4469 7374 3a20 616e 7369 7461 626c  s-Dist: ansitabl
+000005d0: 650a 5265 7175 6972 6573 2d44 6973 743a  e.Requires-Dist:
+000005e0: 206d 7674 622d 6461 7461 0a50 726f 7669   mvtb-data.Provi
+000005f0: 6465 732d 4578 7472 613a 2064 6576 0a52  des-Extra: dev.R
+00000600: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000610: 7465 7374 3b20 6578 7472 6120 3d3d 2022  test; extra == "
+00000620: 6465 7622 0a52 6571 7569 7265 732d 4469  dev".Requires-Di
+00000630: 7374 3a20 636f 7665 7261 6765 3b20 6578  st: coverage; ex
+00000640: 7472 6120 3d3d 2022 6465 7622 0a52 6571  tra == "dev".Req
+00000650: 7569 7265 732d 4469 7374 3a20 666c 616b  uires-Dist: flak
+00000660: 6538 3b20 6578 7472 6120 3d3d 2022 6465  e8; extra == "de
+00000670: 7622 0a50 726f 7669 6465 732d 4578 7472  v".Provides-Extr
+00000680: 613a 2064 6f63 730a 5265 7175 6972 6573  a: docs.Requires
+00000690: 2d44 6973 743a 2073 7068 696e 783b 2065  -Dist: sphinx; e
+000006a0: 7874 7261 203d 3d20 2264 6f63 7322 0a52  xtra == "docs".R
+000006b0: 6571 7569 7265 732d 4469 7374 3a20 7265  equires-Dist: re
+000006c0: 636f 6d6d 6f6e 6d61 726b 3b20 6578 7472  commonmark; extr
+000006d0: 6120 3d3d 2022 646f 6373 220a 5265 7175  a == "docs".Requ
+000006e0: 6972 6573 2d44 6973 743a 2073 7068 696e  ires-Dist: sphin
+000006f0: 782d 7274 642d 7468 656d 653b 2065 7874  x-rtd-theme; ext
+00000700: 7261 203d 3d20 2264 6f63 7322 0a52 6571  ra == "docs".Req
+00000710: 7569 7265 732d 4469 7374 3a20 7370 6869  uires-Dist: sphi
+00000720: 6e78 2d61 7574 6f72 756e 3b20 6578 7472  nx-autorun; extr
+00000730: 6120 3d3d 2022 646f 6373 220a 5265 7175  a == "docs".Requ
+00000740: 6972 6573 2d44 6973 743a 2073 7068 696e  ires-Dist: sphin
+00000750: 7863 6f6e 7472 6962 2d6a 736d 6174 683b  xcontrib-jsmath;
+00000760: 2065 7874 7261 203d 3d20 2264 6f63 7322   extra == "docs"
+00000770: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000780: 7370 6869 6e78 2d6d 6172 6b64 6f77 6e2d  sphinx-markdown-
+00000790: 7461 626c 6573 3b20 6578 7472 6120 3d3d  tables; extra ==
+000007a0: 2022 646f 6373 220a 5265 7175 6972 6573   "docs".Requires
+000007b0: 2d44 6973 743a 2073 7068 696e 782d 6661  -Dist: sphinx-fa
+000007c0: 7669 636f 6e3b 2065 7874 7261 203d 3d20  vicon; extra == 
+000007d0: 2264 6f63 7322 0a0a 2320 4d61 6368 696e  "docs"..# Machin
+000007e0: 6520 5669 7369 6f6e 2054 6f6f 6c62 6f78  e Vision Toolbox
+000007f0: 2066 6f72 2050 7974 686f 6e0a 0a5b 215b   for Python..[![
+00000800: 4120 5079 7468 6f6e 2052 6f62 6f74 6963  A Python Robotic
+00000810: 7320 5061 636b 6167 655d 2868 7474 7073  s Package](https
+00000820: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000830: 7263 6f6e 7465 6e74 2e63 6f6d 2f70 6574  rcontent.com/pet
+00000840: 6572 636f 726b 652f 726f 626f 7469 6373  ercorke/robotics
+00000850: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e2f  -toolbox-python/
+00000860: 6d61 7374 6572 2f2e 6769 7468 7562 2f73  master/.github/s
+00000870: 7667 2f70 795f 636f 6c6c 6563 7469 6f6e  vg/py_collection
+00000880: 2e6d 696e 2e73 7667 295d 2868 7474 7073  .min.svg)](https
+00000890: 3a2f 2f67 6974 6875 622e 636f 6d2f 7065  ://github.com/pe
+000008a0: 7465 7263 6f72 6b65 2f72 6f62 6f74 6963  tercorke/robotic
+000008b0: 732d 746f 6f6c 626f 782d 7079 7468 6f6e  s-toolbox-python
+000008c0: 290a 5b21 5b50 6f77 6572 6564 2062 7920  ).[![Powered by 
+000008d0: 5370 6174 6961 6c20 4d61 7468 735d 2868  Spatial Maths](h
+000008e0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+000008f0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000900: 2f70 6574 6572 636f 726b 652f 7370 6174  /petercorke/spat
+00000910: 6961 6c6d 6174 682d 7079 7468 6f6e 2f6d  ialmath-python/m
+00000920: 6173 7465 722f 2e67 6974 6875 622f 7376  aster/.github/sv
+00000930: 672f 736d 5f70 6f77 6572 6564 2e6d 696e  g/sm_powered.min
+00000940: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
+00000950: 6974 6875 622e 636f 6d2f 7065 7465 7263  ithub.com/peterc
+00000960: 6f72 6b65 2f73 7061 7469 616c 6d61 7468  orke/spatialmath
+00000970: 2d70 7974 686f 6e29 0a5b 215b 5155 5420  -python).[![QUT 
+00000980: 4365 6e74 7265 2066 6f72 2052 6f62 6f74  Centre for Robot
+00000990: 6963 7320 4f70 656e 2053 6f75 7263 655d  ics Open Source]
+000009a0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000009b0: 636f 6d2f 7163 722f 7163 722e 6769 7468  com/qcr/qcr.gith
+000009c0: 7562 2e69 6f2f 7261 772f 6d61 7374 6572  ub.io/raw/master
+000009d0: 2f6d 6973 632f 6261 6467 652e 7376 6729  /misc/badge.svg)
+000009e0: 5d28 6874 7470 733a 2f2f 7163 722e 6769  ](https://qcr.gi
+000009f0: 7468 7562 2e69 6f29 0a0a 5b21 5b50 7950  thub.io)..[![PyP
+00000a00: 4920 7665 7273 696f 6e5d 2868 7474 7073  I version](https
+00000a10: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
+00000a20: 2f70 792f 6d61 6368 696e 6576 6973 696f  /py/machinevisio
+00000a30: 6e2d 746f 6f6c 626f 782d 7079 7468 6f6e  n-toolbox-python
+00000a40: 2e73 7667 295d 2868 7474 7073 3a2f 2f62  .svg)](https://b
+00000a50: 6164 6765 2e66 7572 792e 696f 2f70 792f  adge.fury.io/py/
+00000a60: 6d61 6368 696e 6576 6973 696f 6e2d 746f  machinevision-to
+00000a70: 6f6c 626f 782d 7079 7468 6f6e 290a 215b  olbox-python).![
+00000a80: 5079 7468 6f6e 2056 6572 7369 6f6e 5d28  Python Version](
+00000a90: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000aa0: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+00000ab0: 7273 696f 6e73 2f6d 6163 6869 6e65 7669  rsions/machinevi
+00000ac0: 7369 6f6e 2d74 6f6f 6c62 6f78 2d70 7974  sion-toolbox-pyt
+00000ad0: 686f 6e2e 7376 6729 0a5b 215b 506f 7765  hon.svg).[![Powe
+00000ae0: 7265 6420 6279 204f 7065 6e43 565d 2868  red by OpenCV](h
+00000af0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000b00: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000b10: 2f70 6574 6572 636f 726b 652f 6d61 6368  /petercorke/mach
+00000b20: 696e 6576 6973 696f 6e2d 746f 6f6c 626f  inevision-toolbo
+00000b30: 782d 7079 7468 6f6e 2f6d 6173 7465 722f  x-python/master/
+00000b40: 2e67 6974 6875 622f 7376 672f 6f70 656e  .github/svg/open
+00000b50: 6376 5f70 6f77 6572 6564 2e73 7667 295d  cv_powered.svg)]
+00000b60: 2868 7474 7073 3a2f 2f6f 7065 6e63 762e  (https://opencv.
+00000b70: 6f72 6729 0a5b 215b 506f 7765 7265 6420  org).[![Powered 
+00000b80: 6279 204f 7065 6e33 445d 2868 7474 7073  by Open3D](https
+00000b90: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000ba0: 7263 6f6e 7465 6e74 2e63 6f6d 2f70 6574  rcontent.com/pet
+00000bb0: 6572 636f 726b 652f 6d61 6368 696e 6576  ercorke/machinev
+00000bc0: 6973 696f 6e2d 746f 6f6c 626f 782d 7079  ision-toolbox-py
+00000bd0: 7468 6f6e 2f6d 6173 7465 722f 2e67 6974  thon/master/.git
+00000be0: 6875 622f 7376 672f 6f70 656e 3364 5f70  hub/svg/open3d_p
+00000bf0: 6f77 6572 6564 2e73 7667 295d 2868 7474  owered.svg)](htt
+00000c00: 7073 3a2f 2f6f 7065 6e33 642e 6f72 6729  ps://open3d.org)
+00000c10: 0a5b 215b 4c69 6365 6e73 653a 204d 4954  .[![License: MIT
+00000c20: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000c30: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
+00000c40: 6963 656e 7365 2d4d 4954 2d79 656c 6c6f  icense-MIT-yello
+00000c50: 772e 7376 6729 5d28 6874 7470 733a 2f2f  w.svg)](https://
+00000c60: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
+00000c70: 6963 656e 7365 732f 4d49 5429 0a0a 5b21  icenses/MIT)..[!
+00000c80: 5b42 7569 6c64 2053 7461 7475 735d 2868  [Build Status](h
+00000c90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ca0: 6d2f 7065 7465 7263 6f72 6b65 2f6d 6163  m/petercorke/mac
+00000cb0: 6869 6e65 7669 7369 6f6e 2d74 6f6f 6c62  hinevision-toolb
+00000cc0: 6f78 2d70 7974 686f 6e2f 776f 726b 666c  ox-python/workfl
+00000cd0: 6f77 732f 5465 7374 2d6d 6173 7465 722f  ows/Test-master/
+00000ce0: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
+00000cf0: 3d6d 6173 7465 7229 5d28 6874 7470 733a  =master)](https:
+00000d00: 2f2f 6769 7468 7562 2e63 6f6d 2f70 6574  //github.com/pet
+00000d10: 6572 636f 726b 652f 6d61 6368 696e 6576  ercorke/machinev
+00000d20: 6973 696f 6e2d 746f 6f6c 626f 782d 7079  ision-toolbox-py
+00000d30: 7468 6f6e 2f61 6374 696f 6e73 3f71 7565  thon/actions?que
+00000d40: 7279 3d77 6f72 6b66 6c6f 7725 3341 6275  ry=workflow%3Abu
+00000d50: 696c 6429 0a5b 215b 436f 7665 7261 6765  ild).[![Coverage
+00000d60: 5d28 6874 7470 733a 2f2f 636f 6465 636f  ](https://codeco
+00000d70: 762e 696f 2f67 682f 7065 7465 7263 6f72  v.io/gh/petercor
+00000d80: 6b65 2f6d 6163 6869 6e65 7669 7369 6f6e  ke/machinevision
+00000d90: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e2f  -toolbox-python/
+00000da0: 6272 616e 6368 2f6d 6173 7465 722f 6772  branch/master/gr
+00000db0: 6170 682f 6261 6467 652e 7376 6729 5d28  aph/badge.svg)](
+00000dc0: 6874 7470 733a 2f2f 636f 6465 636f 762e  https://codecov.
+00000dd0: 696f 2f67 682f 7065 7465 7263 6f72 6b65  io/gh/petercorke
+00000de0: 2f6d 6163 6869 6e65 7669 7369 6f6e 2d74  /machinevision-t
+00000df0: 6f6f 6c62 6f78 2d70 7974 686f 6e29 0a5b  oolbox-python).[
+00000e00: 215b 5079 5049 202d 2044 6f77 6e6c 6f61  ![PyPI - Downloa
+00000e10: 6473 5d28 6874 7470 733a 2f2f 696d 672e  ds](https://img.
+00000e20: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000e30: 6477 2f6d 6163 6869 6e65 7669 7369 6f6e  dw/machinevision
+00000e40: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e29  -toolbox-python)
+00000e50: 5d28 6874 7470 733a 2f2f 7079 7069 7374  ](https://pypist
+00000e60: 6174 732e 6f72 672f 7061 636b 6167 6573  ats.org/packages
+00000e70: 2f6d 6163 6869 6e65 7669 7369 6f6e 2d74  /machinevision-t
+00000e80: 6f6f 6c62 6f78 2d70 7974 686f 6e29 0a0a  oolbox-python)..
+00000e90: 3c21 2d2d 205b 215b 4769 7448 7562 2073  <!-- [![GitHub s
+00000ea0: 7461 7273 5d28 6874 7470 733a 2f2f 696d  tars](https://im
+00000eb0: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000ec0: 6875 622f 7374 6172 732f 7065 7465 7263  hub/stars/peterc
+00000ed0: 6f72 6b65 2f6d 6163 6869 6e65 7669 7369  orke/machinevisi
+00000ee0: 6f6e 2d74 6f6f 6c62 6f78 2d70 7974 686f  on-toolbox-pytho
+00000ef0: 6e2e 7376 673f 7374 796c 653d 736f 6369  n.svg?style=soci
+00000f00: 616c 266c 6162 656c 3d53 7461 7229 5d28  al&label=Star)](
+00000f10: 6874 7470 733a 2f2f 4769 7448 7562 2e63  https://GitHub.c
+00000f20: 6f6d 2f70 6574 6572 636f 726b 652f 6d61  om/petercorke/ma
+00000f30: 6368 696e 6576 6973 696f 6e2d 746f 6f6c  chinevision-tool
+00000f40: 626f 782d 7079 7468 6f6e 2f73 7461 7267  box-python/starg
+00000f50: 617a 6572 732f 2920 2d2d 3e0a 0a3c 7461  azers/) -->..<ta
+00000f60: 626c 6520 7374 796c 653d 2262 6f72 6465  ble style="borde
+00000f70: 723a 3070 7822 3e0a 3c74 7220 7374 796c  r:0px">.<tr styl
+00000f80: 653d 2262 6f72 6465 723a 3070 7822 3e0a  e="border:0px">.
+00000f90: 3c74 6420 7374 796c 653d 2262 6f72 6465  <td style="borde
+00000fa0: 723a 3070 7822 3e0a 3c69 6d67 2073 7263  r:0px">.<img src
+00000fb0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000fc0: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
+00000fd0: 6d61 6368 696e 6576 6973 696f 6e2d 746f  machinevision-to
+00000fe0: 6f6c 626f 782d 7079 7468 6f6e 2f72 6177  olbox-python/raw
+00000ff0: 2f6d 6173 7465 722f 6669 6773 2f56 6973  /master/figs/Vis
+00001000: 696f 6e54 6f6f 6c62 6f78 4c6f 676f 5f4e  ionToolboxLogo_N
+00001010: 6f42 6163 6b67 6e64 4032 782e 706e 6722  oBackgnd@2x.png"
+00001020: 2077 6964 7468 3d22 3230 3022 3e3c 2f74   width="200"></t
+00001030: 643e 0a3c 7464 2073 7479 6c65 3d22 626f  d>.<td style="bo
+00001040: 7264 6572 3a30 7078 223e 0a0a 4120 5079  rder:0px">..A Py
+00001050: 7468 6f6e 2069 6d70 6c65 6d65 6e74 6174  thon implementat
+00001060: 696f 6e20 6f66 2074 6865 203c 6120 6872  ion of the <a hr
+00001070: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00001080: 7562 2e63 6f6d 2f70 6574 6572 636f 726b  ub.com/petercork
+00001090: 652f 6d61 6368 696e 6576 6973 696f 6e2d  e/machinevision-
+000010a0: 746f 6f6c 626f 782d 6d61 746c 6162 223e  toolbox-matlab">
+000010b0: 4d61 6368 696e 6520 5669 7369 6f6e 2054  Machine Vision T
+000010c0: 6f6f 6c62 6f78 2066 6f72 204d 4154 4c41  oolbox for MATLA
+000010d0: 423c 7375 703e 2672 6567 3b3c 2f73 7570  B<sup>&reg;</sup
+000010e0: 3e3c 2f61 3e3c 756c 3e0a 0a3c 6c69 3e3c  ></a><ul>..<li><
+000010f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001100: 6769 7468 7562 2e63 6f6d 2f70 6574 6572  github.com/peter
+00001110: 636f 726b 652f 6d61 6368 696e 6576 6973  corke/machinevis
+00001120: 696f 6e2d 746f 6f6c 626f 782d 7079 7468  ion-toolbox-pyth
+00001130: 6f6e 223e 4769 7448 7562 2072 6570 6f73  on">GitHub repos
+00001140: 6974 6f72 7920 3c2f 613e 3c2f 6c69 3e0a  itory </a></li>.
+00001150: 3c6c 693e 3c61 2068 7265 663d 2268 7474  <li><a href="htt
+00001160: 7073 3a2f 2f70 6574 6572 636f 726b 652e  ps://petercorke.
+00001170: 6769 7468 7562 2e69 6f2f 6d61 6368 696e  github.io/machin
+00001180: 6576 6973 696f 6e2d 746f 6f6c 626f 782d  evision-toolbox-
+00001190: 7079 7468 6f6e 2f22 3e44 6f63 756d 656e  python/">Documen
+000011a0: 7461 7469 6f6e 3c2f 613e 3c2f 6c69 3e0a  tation</a></li>.
+000011b0: 3c6c 693e 3c61 2068 7265 663d 2268 7474  <li><a href="htt
+000011c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000011d0: 7065 7465 7263 6f72 6b65 2f6d 6163 6869  petercorke/machi
+000011e0: 6e65 7669 7369 6f6e 2d74 6f6f 6c62 6f78  nevision-toolbox
+000011f0: 2d70 7974 686f 6e2f 7769 6b69 223e 4578  -python/wiki">Ex
+00001200: 616d 706c 6573 2061 6e64 2064 6574 6169  amples and detai
+00001210: 6c73 3c2f 613e 3c2f 6c69 3e0a 3c6c 693e  ls</a></li>.<li>
+00001220: 3c61 2068 7265 663d 2269 6e73 7461 6c6c  <a href="install
+00001230: 6174 696f 6e23 223e 496e 7374 616c 6c61  ation#">Installa
+00001240: 7469 6f6e 3c2f 613e 3c2f 6c69 3e0a 3c2f  tion</a></li>.</
+00001250: 756c 3e0a 3c2f 7464 3e0a 3c2f 7472 3e0a  ul>.</td>.</tr>.
+00001260: 3c2f 7461 626c 653e 0a0a 2323 2053 796e  </table>..## Syn
+00001270: 6f70 7369 730a 0a54 6865 204d 6163 6869  opsis..The Machi
+00001280: 6e65 2056 6973 696f 6e20 546f 6f6c 626f  ne Vision Toolbo
+00001290: 7820 666f 7220 5079 7468 6f6e 2028 4d56  x for Python (MV
+000012a0: 5442 2d50 2920 7072 6f76 6964 6573 206d  TB-P) provides m
+000012b0: 616e 7920 6675 6e63 7469 6f6e 7320 7468  any functions th
+000012c0: 6174 2061 7265 2075 7365 6675 6c20 696e  at are useful in
+000012d0: 206d 6163 6869 6e65 2076 6973 696f 6e20   machine vision 
+000012e0: 616e 6420 7669 7369 6f6e 2d62 6173 6564  and vision-based
+000012f0: 2063 6f6e 7472 6f6c 2e20 5468 6520 6d61   control. The ma
+00001300: 696e 2063 6f6d 706f 6e65 6e74 7320 6172  in components ar
+00001310: 653a 0a0a 2d20 416e 2060 496d 6167 6560  e:..- An `Image`
+00001320: 206f 626a 6563 7420 7769 7468 206e 6561   object with nea
+00001330: 726c 7920 3230 3020 6d65 7468 6f64 7320  rly 200 methods 
+00001340: 616e 6420 7072 6f70 6572 7469 6573 2074  and properties t
+00001350: 6861 7420 7772 6170 2066 756e 6374 696f  hat wrap functio
+00001360: 6e73 0a20 2066 726f 6d20 4f70 656e 4356  ns.  from OpenCV
+00001370: 2c20 4e75 6d50 7920 616e 6420 5363 6950  , NumPy and SciP
+00001380: 792e 204d 6574 686f 6473 2073 7570 706f  y. Methods suppo
+00001390: 7274 206d 6f6e 6164 6963 2c20 6479 6164  rt monadic, dyad
+000013a0: 6963 2c20 6669 6c74 6572 696e 672c 2065  ic, filtering, e
+000013b0: 6467 6520 6465 7465 6374 696f 6e2c 0a20  dge detection,. 
+000013c0: 206d 6174 6865 6d61 7469 6361 6c20 6d6f   mathematical mo
+000013d0: 7270 686f 6c6f 6779 2061 6e64 2066 6561  rphology and fea
+000013e0: 7475 7265 2065 7874 7261 6374 696f 6e20  ture extraction 
+000013f0: 2862 6c6f 6273 2c20 6c69 6e65 7320 616e  (blobs, lines an
+00001400: 6420 706f 696e 742f 636f 726e 6572 2066  d point/corner f
+00001410: 6561 7475 7265 7329 2c20 6173 2077 656c  eatures), as wel
+00001420: 6c20 6173 206f 7065 7261 746f 7220 6f76  l as operator ov
+00001430: 6572 6c6f 6164 696e 672e 2049 6d61 6765  erloading. Image
+00001440: 7320 6172 6520 7374 6f72 6564 2061 7320  s are stored as 
+00001450: 656e 6361 7073 756c 6174 6564 205b 4e75  encapsulated [Nu
+00001460: 6d50 795d 2868 7474 7073 3a2f 2f6e 756d  mPy](https://num
+00001470: 7079 2e6f 7267 2920 6172 7261 7973 0a20  py.org) arrays. 
+00001480: 2061 6c6f 6e67 2077 6974 6820 696d 6167   along with imag
+00001490: 6520 6d65 7461 6461 7461 2e0a 2d20 416e  e metadata..- An
+000014a0: 206f 626a 6563 742d 6f72 6965 6e74 6564   object-oriented
+000014b0: 2077 7261 7070 6572 206f 6620 4f70 656e   wrapper of Open
+000014c0: 3344 2066 756e 6374 696f 6e73 2074 6861  3D functions tha
+000014d0: 7420 7375 7070 6f72 7473 2061 2073 7562  t supports a sub
+000014e0: 7365 7420 6f66 206f 7065 7261 7469 6f6e  set of operation
+000014f0: 732c 2062 7574 2061 6c6c 6f77 7320 6f70  s, but allows op
+00001500: 6572 6174 6f72 206f 7665 726c 6f61 6469  erator overloadi
+00001510: 6e67 2061 6e64 2069 7320 636f 6d70 6174  ng and is compat
+00001520: 6962 6c65 2077 6974 6820 7468 6520 5b53  ible with the [S
+00001530: 7061 7469 616c 204d 6174 6820 546f 6f6c  patial Math Tool
+00001540: 626f 785d 2868 7474 7073 3a2f 2f67 6974  box](https://git
+00001550: 6875 622e 636f 6d2f 7065 7465 7263 6f72  hub.com/petercor
+00001560: 6b65 2f73 7061 7469 616c 6d61 7468 2d70  ke/spatialmath-p
+00001570: 7974 686f 6e29 2e0a 2d20 4120 636f 6c6c  ython)..- A coll
+00001580: 6563 7469 6f6e 206f 6620 6361 6d65 7261  ection of camera
+00001590: 2070 726f 6a65 6374 696f 6e20 636c 6173   projection clas
+000015a0: 7365 7320 666f 7220 6365 6e74 7261 6c20  ses for central 
+000015b0: 286e 6f72 6d61 6c20 7065 7273 7065 6374  (normal perspect
+000015c0: 6976 6529 2c20 6669 7368 6579 652c 2063  ive), fisheye, c
+000015d0: 6174 6164 696f 7074 7269 6320 616e 6420  atadioptric and 
+000015e0: 7370 6865 7269 6361 6c20 6361 6d65 7261  spherical camera
+000015f0: 732e 0a2d 2053 6f6d 6520 6164 7661 6e63  s..- Some advanc
+00001600: 6564 2061 6c67 6f72 6974 686d 7320 7375  ed algorithms su
+00001610: 6368 2061 733a 0a20 202d 206d 756c 7469  ch as:.  - multi
+00001620: 7669 6577 2067 656f 6d65 7472 793a 2063  view geometry: c
+00001630: 616d 6572 6120 6361 6c69 6272 6174 696f  amera calibratio
+00001640: 6e2c 2073 7465 7265 6f20 7669 7369 6f6e  n, stereo vision
+00001650: 2c20 6275 6e64 6c65 2061 646a 7573 746d  , bundle adjustm
+00001660: 656e 740a 2020 2d20 6261 6720 6f66 2077  ent.  - bag of w
+00001670: 6f72 6473 0a0a 4164 7661 6e74 6167 6573  ords..Advantages
+00001680: 206f 6620 7468 6973 2050 7974 686f 6e20   of this Python 
+00001690: 546f 6f6c 626f 7820 6172 6520 7468 6174  Toolbox are that
+000016a0: 3a0a 0a2d 2069 7420 7573 6573 2c20 6173  :..- it uses, as
+000016b0: 206d 7563 6820 6173 2070 6f73 7369 626c   much as possibl
+000016c0: 652c 205b 4f70 656e 4356 5d28 6874 7470  e, [OpenCV](http
+000016d0: 733a 2f2f 6f70 656e 6376 2e6f 7267 2920  s://opencv.org) 
+000016e0: 616e 6420 5b4e 756d 5079 5d28 6874 7470  and [NumPy](http
+000016f0: 733a 2f2f 6e75 6d70 792e 6f72 6729 2077  s://numpy.org) w
+00001700: 6869 6368 2061 7265 2070 6f72 7461 626c  hich are portabl
+00001710: 652c 2065 6666 6963 6965 6e74 2c20 636f  e, efficient, co
+00001720: 6d70 7265 6865 6e73 6976 6520 616e 6420  mprehensive and 
+00001730: 6d61 7475 7265 2063 6f6c 6c65 6374 696f  mature collectio
+00001740: 6e20 6f66 2066 756e 6374 696f 6e73 2066  n of functions f
+00001750: 6f72 2069 6d61 6765 2070 726f 6365 7373  or image process
+00001760: 696e 6720 616e 6420 6665 6174 7572 6520  ing and feature 
+00001770: 6578 7472 6163 7469 6f6e 3b0a 2d20 6974  extraction;.- it
+00001780: 2077 7261 7073 2074 6865 204f 7065 6e43   wraps the OpenC
+00001790: 5620 6675 6e63 7469 6f6e 7320 696e 2061  V functions in a
+000017a0: 2063 6f6e 7369 7374 656e 7420 7761 792c   consistent way,
+000017b0: 2068 6964 696e 6720 736f 6d65 206f 6620   hiding some of 
+000017c0: 7468 6520 676e 6172 6c79 2064 6574 6169  the gnarly detai
+000017d0: 6c73 206f 6620 4f70 656e 4356 206c 696b  ls of OpenCV lik
+000017e0: 6520 636f 6e76 6572 7369 6f6e 2074 6f2f  e conversion to/
+000017f0: 6672 6f6d 2066 6c6f 6174 3332 2061 6e64  from float32 and
+00001800: 2074 6865 2042 4752 2063 6f6c 6f72 206f   the BGR color o
+00001810: 7264 6572 2e0a 2d20 6974 2069 7320 6861  rder..- it is ha
+00001820: 7320 7369 6d69 6c61 7269 7479 2074 6f20  s similarity to 
+00001830: 7468 6520 4d61 6368 696e 6520 5669 7369  the Machine Visi
+00001840: 6f6e 2054 6f6f 6c62 6f78 2066 6f72 204d  on Toolbox for M
+00001850: 4154 4c41 422e 0a0a 2320 4765 7474 696e  ATLAB...# Gettin
+00001860: 6720 676f 696e 670a 0a23 2320 5573 696e  g going..## Usin
+00001870: 6720 7069 700a 0a49 6e73 7461 6c6c 2061  g pip..Install a
+00001880: 2073 6e61 7073 686f 7420 6672 6f6d 2050   snapshot from P
+00001890: 7950 490a 0a60 6060 0a25 2070 6970 2069  yPI..```.% pip i
+000018a0: 6e73 7461 6c6c 206d 6163 6869 6e65 7669  nstall machinevi
+000018b0: 7369 6f6e 2d74 6f6f 6c62 6f78 2d70 7974  sion-toolbox-pyt
+000018c0: 686f 6e0a 6060 600a 0a23 2320 4672 6f6d  hon.```..## From
+000018d0: 2047 6974 4875 620a 0a49 6e73 7461 6c6c   GitHub..Install
+000018e0: 2074 6865 2063 7572 7265 6e74 2063 6f64   the current cod
+000018f0: 6520 6261 7365 2066 726f 6d20 4769 7448  e base from GitH
+00001900: 7562 2061 6e64 2070 6970 2069 6e73 7461  ub and pip insta
+00001910: 6c6c 2061 206c 696e 6b20 746f 2074 6861  ll a link to tha
+00001920: 7420 636c 6f6e 6564 2063 6f70 790a 0a60  t cloned copy..`
+00001930: 6060 0a25 2067 6974 2063 6c6f 6e65 2068  ``.% git clone h
+00001940: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001950: 6d2f 7065 7465 7263 6f72 6b65 2f6d 6163  m/petercorke/mac
+00001960: 6869 6e65 7669 7369 6f6e 2d74 6f6f 6c62  hinevision-toolb
+00001970: 6f78 2d70 7974 686f 6e2e 6769 740a 2520  ox-python.git.% 
+00001980: 6364 206d 6163 6869 6e65 7669 7369 6f6e  cd machinevision
+00001990: 2d74 6f6f 6c62 6f78 2d70 7974 686f 6e0a  -toolbox-python.
+000019a0: 2520 7069 7020 696e 7374 616c 6c20 2d65  % pip install -e
+000019b0: 202e 0a60 6060 0a0a 2320 4578 616d 706c   ..```..# Exampl
+000019c0: 6573 0a0a 2323 2320 5265 6164 696e 6720  es..### Reading 
+000019d0: 616e 6420 6469 7370 6c61 7920 616e 2069  and display an i
+000019e0: 6d61 6765 0a0a 6060 6070 7974 686f 6e0a  mage..```python.
+000019f0: 6672 6f6d 206d 6163 6869 6e65 7669 7369  from machinevisi
+00001a00: 6f6e 746f 6f6c 626f 7820 696d 706f 7274  ontoolbox import
+00001a10: 2049 6d61 6765 0a6d 6f6e 6120 3d20 496d   Image.mona = Im
+00001a20: 6167 652e 5265 6164 2822 6d6f 6e61 6c69  age.Read("monali
+00001a30: 7361 2e70 6e67 2229 0a6d 6f6e 612e 6469  sa.png").mona.di
+00001a40: 7370 2829 0a60 6060 0a0a 215b 4d6f 6e61  sp().```..![Mona
+00001a50: 204c 6973 6120 696d 6167 655d 2868 7474   Lisa image](htt
+00001a60: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001a70: 7065 7465 7263 6f72 6b65 2f6d 6163 6869  petercorke/machi
+00001a80: 6e65 7669 7369 6f6e 2d74 6f6f 6c62 6f78  nevision-toolbox
+00001a90: 2d70 7974 686f 6e2f 7261 772f 6d61 7374  -python/raw/mast
+00001aa0: 6572 2f66 6967 732f 6d6f 6e61 2e70 6e67  er/figs/mona.png
+00001ab0: 290a 0a49 6d61 6765 7320 6361 6e20 616c  )..Images can al
+00001ac0: 736f 2062 6520 7265 7475 726e 6564 2062  so be returned b
+00001ad0: 7920 6974 6572 6174 6f72 7320 7468 6174  y iterators that
+00001ae0: 206f 7065 7261 7465 206f 7665 7220 666f   operate over fo
+00001af0: 6c64 6572 732c 207a 6970 2066 696c 6573  lders, zip files
+00001b00: 2c20 6c6f 6361 6c20 6361 6d65 7261 732c  , local cameras,
+00001b10: 2077 6562 2063 616d 6572 6173 2061 6e64   web cameras and
+00001b20: 2076 6964 656f 2066 696c 6573 2e0a 0a23   video files...#
+00001b30: 2323 2053 696d 706c 6520 696d 6167 6520  ## Simple image 
+00001b40: 7072 6f63 6573 7369 6e67 0a0a 5468 6520  processing..The 
+00001b50: 746f 6f6c 626f 7820 7375 7070 6f72 7473  toolbox supports
+00001b60: 206d 616e 7920 6f70 6572 6174 696f 6e73   many operations
+00001b70: 206f 6e20 696d 6167 6573 2073 7563 6820   on images such 
+00001b80: 6173 2032 4420 6669 6c74 6572 696e 672c  as 2D filtering,
+00001b90: 2065 6467 6520 6465 7465 6374 696f 6e2c   edge detection,
+00001ba0: 206d 6174 6865 6d61 7469 6361 6c20 6d6f   mathematical mo
+00001bb0: 7270 686f 6c6f 6779 2c20 636f 6c6f 7273  rphology, colors
+00001bc0: 7061 6365 2063 6f6e 7665 7273 696f 6e2c  pace conversion,
+00001bd0: 2070 6164 6469 6e67 2c20 6372 6f70 7069   padding, croppi
+00001be0: 6e67 2c20 7265 7369 7a69 6e67 2c20 726f  ng, resizing, ro
+00001bf0: 7461 7469 6f6e 2061 6e64 2077 6172 7069  tation and warpi
+00001c00: 6e67 2e0a 0a60 6060 7079 7468 6f6e 0a6d  ng...```python.m
+00001c10: 6f6e 612e 736d 6f6f 7468 2873 6967 6d61  ona.smooth(sigma
+00001c20: 3d35 292e 6469 7370 2829 0a60 6060 0a0a  =5).disp().```..
+00001c30: 215b 4d6f 6e61 204c 6973 6120 696d 6167  ![Mona Lisa imag
+00001c40: 6520 7769 7468 2073 6d6f 6f74 6869 6e67  e with smoothing
+00001c50: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001c60: 2e63 6f6d 2f70 6574 6572 636f 726b 652f  .com/petercorke/
+00001c70: 6d61 6368 696e 6576 6973 696f 6e2d 746f  machinevision-to
+00001c80: 6f6c 626f 782d 7079 7468 6f6e 2f72 6177  olbox-python/raw
+00001c90: 2f6d 6173 7465 722f 6669 6773 2f6d 6f6e  /master/figs/mon
+00001ca0: 615f 736d 6f6f 7468 2e70 6e67 290a 0a54  a_smooth.png)..T
+00001cb0: 6865 7265 2061 7265 2061 6c73 6f20 6d61  here are also ma
+00001cc0: 6e79 2066 756e 6374 696f 6e73 2074 6861  ny functions tha
+00001cd0: 7420 6f70 6572 6174 6520 6f6e 2070 6169  t operate on pai
+00001ce0: 7273 206f 6620 696d 6167 652e 2041 6c6c  rs of image. All
+00001cf0: 2074 6865 2061 7269 7468 6d65 7469 6320   the arithmetic 
+00001d00: 6f70 6572 6174 6f72 7320 6172 6520 6f76  operators are ov
+00001d10: 6572 6c6f 6164 6564 2c20 616e 6420 7468  erloaded, and th
+00001d20: 6572 6520 6172 6520 6d65 7468 6f64 7320  ere are methods 
+00001d30: 746f 2063 6f6d 6269 6e65 2069 6d61 6765  to combine image
+00001d40: 7320 696e 206d 6f72 6520 636f 6d70 6c65  s in more comple
+00001d50: 7820 7761 7973 2e20 4d75 6c74 6970 6c65  x ways. Multiple
+00001d60: 2069 6d61 6765 7320 6361 6e20 6265 2073   images can be s
+00001d70: 7461 636b 6564 2068 6f72 697a 6f6e 7461  tacked horizonta
+00001d80: 6c2c 2076 6572 7469 6361 6c6c 7920 6f72  l, vertically or
+00001d90: 2074 696c 6564 2069 6e20 6120 3244 2067   tiled in a 2D g
+00001da0: 7269 642e 2046 6f72 2065 7861 6d70 6c65  rid. For example
+00001db0: 2c20 7765 2063 6f75 6c64 2064 6973 706c  , we could displ
+00001dc0: 6179 2074 6865 206f 7269 6769 6e61 6c20  ay the original 
+00001dd0: 616e 6420 736d 6f6f 7468 6564 2069 6d61  and smoothed ima
+00001de0: 6765 7320 7369 6465 2062 7920 7369 6465  ges side by side
+00001df0: 0a0a 6060 6070 7974 686f 6e0a 496d 6167  ..```python.Imag
+00001e00: 652e 4873 7461 636b 285b 6d6f 6e61 2c20  e.Hstack([mona, 
+00001e10: 6d6f 6e61 2e73 6d6f 6f74 6828 7369 676d  mona.smooth(sigm
+00001e20: 613d 3529 5d29 2e64 6973 7028 290a 6060  a=5)]).disp().``
+00001e30: 600a 0a77 6865 7265 2060 4873 7461 636b  `..where `Hstack
+00001e40: 6020 6973 2061 2063 6c61 7373 206d 6574  ` is a class met
+00001e50: 686f 6420 7468 6174 2063 7265 6174 6573  hod that creates
+00001e60: 2061 206e 6577 2069 6d61 6765 2062 7920   a new image by 
+00001e70: 7374 6163 6b69 6e67 2074 6865 0a69 6d61  stacking the.ima
+00001e80: 6765 7320 6672 6f6d 2069 7473 2061 7267  ges from its arg
+00001e90: 756d 656e 742c 2061 6e20 696d 6167 6520  ument, an image 
+00001ea0: 7365 7175 656e 6365 2c20 686f 7269 7a6f  sequence, horizo
+00001eb0: 6e74 616c 6c79 2e0a 0a21 5b4d 6f6e 6120  ntally...![Mona 
+00001ec0: 4c69 7361 2069 6d61 6765 2077 6974 6820  Lisa image with 
+00001ed0: 736d 6f6f 7468 696e 675d 2868 7474 7073  smoothing](https
+00001ee0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7065  ://github.com/pe
+00001ef0: 7465 7263 6f72 6b65 2f6d 6163 6869 6e65  tercorke/machine
+00001f00: 7669 7369 6f6e 2d74 6f6f 6c62 6f78 2d70  vision-toolbox-p
+00001f10: 7974 686f 6e2f 7261 772f 6d61 7374 6572  ython/raw/master
+00001f20: 2f66 6967 732f 6d6f 6e61 2b73 6d6f 6f74  /figs/mona+smoot
+00001f30: 682e 706e 6729 0a0a 2323 2320 4269 6e61  h.png)..### Bina
+00001f40: 7279 2062 6c6f 6273 0a0a 4120 636f 6d6d  ry blobs..A comm
+00001f50: 6f6e 2070 726f 626c 656d 2069 6e20 726f  on problem in ro
+00001f60: 626f 7469 6320 7669 7369 6f6e 2069 7320  botic vision is 
+00001f70: 746f 2065 7874 7261 6374 2066 6561 7475  to extract featu
+00001f80: 7265 7320 6672 6f6d 2074 6865 2069 6d61  res from the ima
+00001f90: 6765 2c20 746f 2064 6573 6372 6962 6520  ge, to describe 
+00001fa0: 7468 6520 706f 7369 7469 6f6e 2c20 7369  the position, si
+00001fb0: 7a65 2c20 7368 6170 6520 616e 6420 6f72  ze, shape and or
+00001fc0: 6965 6e74 6174 696f 6e20 6f66 206f 626a  ientation of obj
+00001fd0: 6563 7473 2069 6e20 7468 6520 7363 656e  ects in the scen
+00001fe0: 652e 2046 6f72 2073 696d 706c 6520 6269  e. For simple bi
+00001ff0: 6e61 7279 2073 6365 6e65 7320 626c 6f62  nary scenes blob
+00002000: 2066 6561 7475 7265 7320 6172 6520 636f   features are co
+00002010: 6d6d 6f6e 6c79 2075 7365 642e 0a0a 6060  mmonly used...``
+00002020: 6070 7974 686f 6e0a 696d 203d 2049 6d61  `python.im = Ima
+00002030: 6765 2e52 6561 6428 2273 6861 726b 322e  ge.Read("shark2.
+00002040: 706e 6722 2920 2020 2320 7265 6164 2061  png")   # read a
+00002050: 2062 696e 6172 7920 696d 6167 6520 6f66   binary image of
+00002060: 2074 776f 2073 6861 726b 730a 696d 2e64   two sharks.im.d
+00002070: 6973 7028 293b 2020 2023 2064 6973 706c  isp();   # displ
+00002080: 6179 2069 7420 7769 7468 2069 6e74 6572  ay it with inter
+00002090: 6163 7469 7665 2076 6965 7769 6e67 2074  active viewing t
+000020a0: 6f6f 6c0a 626c 6f62 7320 3d20 696d 2e62  ool.blobs = im.b
+000020b0: 6c6f 6273 2829 2020 2320 6669 6e64 2061  lobs()  # find a
+000020c0: 6c6c 2074 6865 2077 6869 7465 2062 6c6f  ll the white blo
+000020d0: 6273 0a70 7269 6e74 2862 6c6f 6273 290a  bs.print(blobs).
+000020e0: 0a09 e294 8ce2 9480 e294 80e2 9480 e294  ................
+000020f0: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002100: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
+00002110: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002120: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002130: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
+00002140: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002150: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
+00002160: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002170: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
+00002180: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
+00002190: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000021a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000021b0: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
+000021c0: e294 80e2 9480 e294 80e2 9480 e294 ace2  ................
+000021d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000021e0: 80e2 9480 e294 80e2 9490 0a09 e294 8269  ...............i
+000021f0: 6420 e294 8220 7061 7265 6e74 20e2 9482  d ... parent ...
+00002200: 2020 2020 2063 656e 7472 6f69 6420 e294       centroid ..
+00002210: 8220 2020 2020 6172 6561 20e2 9482 2074  .     area ... t
+00002220: 6f75 6368 20e2 9482 2070 6572 696d 20e2  ouch ... perim .
+00002230: 9482 2063 6972 6375 6c61 7269 7479 20e2  .. circularity .
+00002240: 9482 206f 7269 656e 7420 e294 8220 6173  .. orient ... as
+00002250: 7065 6374 20e2 9482 0a09 e294 9ce2 9480  pect ...........
+00002260: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+00002270: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002280: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+00002290: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000022a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000022b0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000022c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000022d0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+000022e0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+000022f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002300: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+00002310: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002320: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+00002330: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002340: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+00002350: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002360: 94a4 0a09 e294 8220 3020 e294 8220 2020  ....... 0 ...   
+00002370: 2020 2d31 20e2 9482 2033 3731 2e32 2c20    -1 ... 371.2, 
+00002380: 3335 352e 3220 e294 8220 372e 3539 652b  355.2 ... 7.59e+
+00002390: 3033 20e2 9482 2046 616c 7365 20e2 9482  03 ... False ...
+000023a0: 2035 3537 2e36 20e2 9482 2020 2020 2020   557.6 ...      
+000023b0: 2030 2e33 3431 20e2 9482 2020 3832 2e39   0.341 ...  82.9
+000023c0: c2b0 20e2 9482 2020 302e 3937 3620 e294  .. ...  0.976 ..
+000023d0: 820a 09e2 9482 2031 20e2 9482 2020 2020  ...... 1 ...    
+000023e0: 202d 3120 e294 8220 3137 312e 322c 2031   -1 ... 171.2, 1
+000023f0: 3535 2e32 20e2 9482 2037 2e35 3965 2b30  55.2 ... 7.59e+0
+00002400: 3320 e294 8220 4661 6c73 6520 e294 8220  3 ... False ... 
+00002410: 3535 372e 3620 e294 8220 2020 2020 2020  557.6 ...       
+00002420: 302e 3334 3120 e294 8220 2038 322e 39c2  0.341 ...  82.9.
+00002430: b020 e294 8220 2030 2e39 3736 20e2 9482  . ...  0.976 ...
+00002440: 0a09 e294 94e2 9480 e294 80e2 9480 e294  ................
+00002450: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002460: e294 80e2 9480 e294 80e2 94b4 e294 80e2  ................
+00002470: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002480: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002490: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
+000024a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000024b0: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
+000024c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000024d0: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
+000024e0: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
+000024f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002500: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002510: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
+00002520: e294 80e2 9480 e294 80e2 9480 e294 b4e2  ................
+00002530: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002540: 80e2 9480 e294 80e2 9498 0a60 6060 0a0a  ...........```..
+00002550: 7768 6572 6520 6062 6c6f 6273 6020 6973  where `blobs` is
+00002560: 2061 206c 6973 742d 6c69 6b65 206f 626a   a list-like obj
+00002570: 6563 7420 616e 6420 6561 6368 2065 6c65  ect and each ele
+00002580: 6d65 6e74 2064 6573 6372 6962 6573 2061  ment describes a
+00002590: 2062 6c6f 6220 696e 2074 6865 2073 6365   blob in the sce
+000025a0: 6e65 2e20 5468 6520 656c 656d 656e 7427  ne. The element'
+000025b0: 7320 6174 7472 6962 7574 6573 2064 6573  s attributes des
+000025c0: 6372 6962 6520 7661 7269 6f75 7320 7061  cribe various pa
+000025d0: 7261 6d65 7465 7273 206f 6620 7468 6520  rameters of the 
+000025e0: 6f62 6a65 6374 2c20 616e 6420 6d65 7468  object, and meth
+000025f0: 6f64 7320 6361 6e20 6265 2075 7365 6420  ods can be used 
+00002600: 746f 206f 7665 726c 6179 2067 7261 7068  to overlay graph
+00002610: 6963 7320 7375 6368 2061 7320 626f 756e  ics such as boun
+00002620: 6469 6e67 2062 6f78 6573 2061 6e64 2063  ding boxes and c
+00002630: 656e 7472 6f69 6473 0a0a 6060 6070 7974  entroids..```pyt
+00002640: 686f 6e0a 626c 6f62 732e 706c 6f74 5f62  hon.blobs.plot_b
+00002650: 6f78 2863 6f6c 6f72 3d22 6722 2c20 6c69  ox(color="g", li
+00002660: 6e65 7769 6474 683d 3229 2020 2320 7075  newidth=2)  # pu
+00002670: 7420 6120 6772 6565 6e20 626f 756e 6469  t a green boundi
+00002680: 6e67 2062 6f78 206f 6e20 6561 6368 2062  ng box on each b
+00002690: 6c6f 620a 626c 6f62 732e 706c 6f74 5f63  lob.blobs.plot_c
+000026a0: 656e 7472 6f69 6428 6c61 6265 6c3d 5472  entroid(label=Tr
+000026b0: 7565 2920 2023 2070 7574 2061 2063 6972  ue)  # put a cir
+000026c0: 636c 652b 6372 6f73 7320 6f6e 2074 6865  cle+cross on the
+000026d0: 2063 656e 7472 6f69 6420 6f66 2065 6163   centroid of eac
+000026e0: 6820 626c 6f62 0a70 6c74 2e73 686f 7728  h blob.plt.show(
+000026f0: 626c 6f63 6b3d 5472 7565 2920 2023 2064  block=True)  # d
+00002700: 6973 706c 6179 2074 6865 2072 6573 756c  isplay the resul
+00002710: 740a 6060 600a 0a21 5b42 696e 6172 7920  t.```..![Binary 
+00002720: 696d 6167 6520 7368 6f77 696e 6720 626f  image showing bo
+00002730: 756e 6469 6e67 2062 6f78 6573 2061 6e64  unding boxes and
+00002740: 2063 656e 7472 6f69 6473 5d28 6874 7470   centroids](http
+00002750: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00002760: 6574 6572 636f 726b 652f 6d61 6368 696e  etercorke/machin
+00002770: 6576 6973 696f 6e2d 746f 6f6c 626f 782d  evision-toolbox-
+00002780: 7079 7468 6f6e 2f72 6177 2f6d 6173 7465  python/raw/maste
+00002790: 722f 6669 6773 2f73 6861 726b 322b 626f  r/figs/shark2+bo
+000027a0: 7865 732e 706e 6729 0a0a 2323 2323 2042  xes.png)..#### B
+000027b0: 696e 6172 7920 626c 6f62 2068 6965 7261  inary blob hiera
+000027c0: 7263 6879 0a0a 4120 6d6f 7265 2063 6f6d  rchy..A more com
+000027d0: 706c 6578 2069 6d61 6765 2069 730a 0a60  plex image is..`
+000027e0: 6060 7079 7468 6f6e 0a69 6d20 3d20 496d  ``python.im = Im
+000027f0: 6167 652e 5265 6164 2822 6d75 6c74 6962  age.Read("multib
+00002800: 6c6f 6273 2e70 6e67 2229 0a69 6d2e 6469  lobs.png").im.di
+00002810: 7370 2829 0a60 6060 0a0a 215b 4269 6e61  sp().```..![Bina
+00002820: 7279 2069 6d61 6765 2077 6974 6820 6e65  ry image with ne
+00002830: 7374 6564 2062 6c6f 6273 5d28 6874 7470  sted blobs](http
+00002840: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
+00002850: 6574 6572 636f 726b 652f 6d61 6368 696e  etercorke/machin
+00002860: 6576 6973 696f 6e2d 746f 6f6c 626f 782d  evision-toolbox-
+00002870: 7079 7468 6f6e 2f72 6177 2f6d 6173 7465  python/raw/maste
+00002880: 722f 6669 6773 2f6d 756c 7469 2e70 6e67  r/figs/multi.png
+00002890: 290a 0a61 6e64 2077 6520 7365 6520 7468  )..and we see th
+000028a0: 6174 2073 6f6d 6520 626c 6f62 7320 6172  at some blobs ar
+000028b0: 6520 636f 6e74 6169 6e65 6420 7769 7468  e contained with
+000028c0: 696e 206f 7468 6572 2062 6c6f 6273 2e20  in other blobs. 
+000028d0: 5468 6520 7265 7375 6c74 7320 696e 2074  The results in t
+000028e0: 6162 756c 6172 2066 6f72 6d0a 0a60 6060  abular form..```
+000028f0: 7079 7468 6f6e 0a62 6c6f 6273 2020 3d20  python.blobs  = 
+00002900: 696d 2e62 6c6f 6273 2829 0a70 7269 6e74  im.blobs().print
+00002910: 2862 6c6f 6273 290a 09e2 948c e294 80e2  (blobs).........
+00002920: 9480 e294 80e2 94ac e294 80e2 9480 e294  ................
+00002930: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002940: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
+00002950: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002960: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002970: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
+00002980: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002990: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
+000029a0: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
+000029b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000029c0: 80e2 9480 e294 ace2 9480 e294 80e2 9480  ................
+000029d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000029e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000029f0: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002a00: e294 80e2 9480 e294 80e2 94ac e294 80e2  ................
+00002a10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002a20: 80e2 9480 e294 900a 09e2 9482 6964 20e2  ............id .
+00002a30: 9482 2070 6172 656e 7420 e294 8220 2020  .. parent ...   
+00002a40: 2020 2063 656e 7472 6f69 6420 e294 8220     centroid ... 
+00002a50: 2020 2020 6172 6561 20e2 9482 2074 6f75      area ... tou
+00002a60: 6368 20e2 9482 2020 7065 7269 6d20 e294  ch ...  perim ..
+00002a70: 8220 6369 7263 756c 6172 6974 7920 e294  . circularity ..
+00002a80: 8220 6f72 6965 6e74 20e2 9482 2061 7370  . orient ... asp
+00002a90: 6563 7420 e294 820a 09e2 949c e294 80e2  ect ............
+00002aa0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+00002ab0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002ac0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+00002ad0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002ae0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002af0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+00002b00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002b10: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+00002b20: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+00002b30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002b40: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+00002b50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00002b60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002b70: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00002b80: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+00002b90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00002ba0: 80e2 9480 e294 a40a 09e2 9482 2030 20e2  ............ 0 .
+00002bb0: 9482 2020 2020 2020 3120 e294 8220 2038  ..      1 ...  8
+00002bc0: 3938 2e38 2c20 3732 352e 3320 e294 8220  98.8, 725.3 ... 
+00002bd0: 312e 3635 652b 3035 20e2 9482 2046 616c  1.65e+05 ... Fal
+00002be0: 7365 20e2 9482 2032 3232 302e 3020 e294  se ... 2220.0 ..
+00002bf0: 8220 2020 2020 2020 302e 3436 3720 e294  .       0.467 ..
+00002c00: 8220 2038 362e 37c2 b020 e294 8220 2030  .  86.7.. ...  0
+00002c10: 2e37 3534 20e2 9482 0a09 e294 8220 3120  .754 ........ 1 
+00002c20: e294 8220 2020 2020 2032 20e2 9482 2031  ...      2 ... 1
+00002c30: 3032 352e 302c 2038 3133 2e37 20e2 9482  025.0, 813.7 ...
+00002c40: 2031 2e30 3665 2b30 3520 e294 8220 4661   1.06e+05 ... Fa
+00002c50: 6c73 6520 e294 8220 3133 3837 2e39 20e2  lse ... 1387.9 .
+00002c60: 9482 2020 2020 2020 2030 2e37 3639 20e2  ..       0.769 .
+00002c70: 9482 202d 3838 2e39 c2b0 20e2 9482 2020  .. -88.9.. ...  
+00002c80: 302e 3733 3920 e294 820a 09e2 9482 2032  0.739 ........ 2
+00002c90: 20e2 9482 2020 2020 202d 3120 e294 8220   ...     -1 ... 
+00002ca0: 2039 3338 2e31 2c20 3835 352e 3220 e294   938.1, 855.2 ..
+00002cb0: 8220 312e 3732 652b 3034 20e2 9482 2046  . 1.72e+04 ... F
+00002cc0: 616c 7365 20e2 9482 2020 3439 302e 3720  alse ...  490.7 
+00002cd0: e294 8220 2020 2020 2020 312e 3030 3120  ...       1.001 
+00002ce0: e294 8220 2038 382e 37c2 b020 e294 8220  ...  88.7.. ... 
+00002cf0: 2030 2e38 3632 20e2 9482 0a09 e294 8220   0.862 ........ 
+00002d00: 3320 e294 8220 2020 2020 2d31 20e2 9482  3 ...     -1 ...
+00002d10: 2020 3938 382e 312c 2036 3937 2e32 20e2    988.1, 697.2 .
+00002d20: 9482 2031 2e32 3165 2b30 3420 e294 8220  .. 1.21e+04 ... 
+00002d30: 4661 6c73 6520 e294 8220 2034 3132 2e35  False ...  412.5
+00002d40: 20e2 9482 2020 2020 2020 2030 2e39 3934   ...       0.994
+00002d50: 20e2 9482 202d 3837 2e38 c2b0 20e2 9482   ... -87.8.. ...
+00002d60: 2020 302e 3830 3920 e294 820a 09e2 9482    0.809 ........
+00002d70: 2034 20e2 9482 2020 2020 202d 3120 e294   4 ...     -1 ..
+00002d80: 8220 2038 3436 2e30 2c20 3531 312e 3720  .  846.0, 511.7 
+00002d90: e294 8220 312e 3735 652b 3034 20e2 9482  ... 1.75e+04 ...
+00002da0: 2046 616c 7365 20e2 9482 2020 3439 362e   False ...  496.
+00002db0: 3920 e294 8220 2020 2020 2020 302e 3939  9 ...       0.99
+00002dc0: 3220 e294 8220 2d39 302e 30c2 b020 e294  2 ... -90.0.. ..
+00002dd0: 8220 2030 2e37 3738 20e2 9482 0a09 e294  .  0.778 .......
+00002de0: 8220 3520 e294 8220 2020 2020 2036 20e2  . 5 ...      6 .
+00002df0: 9482 2020 3239 312e 372c 2033 3737 2e38  ..  291.7, 377.8
+00002e00: 20e2 9482 2020 312e 3765 2b30 3520 e294   ...  1.7e+05 ..
+00002e10: 8220 4661 6c73 6520 e294 8220 3137 3132  . False ... 1712
+00002e20: 2e36 20e2 9482 2020 2020 2020 2030 2e38  .6 ...       0.8
+00002e30: 3130 20e2 9482 202d 3835 2e33 c2b0 20e2  10 ... -85.3.. .
+00002e40: 9482 2020 302e 3736 3720 e294 820a 09e2  ..  0.767 ......
+00002e50: 9482 2036 20e2 9482 2020 2020 202d 3120  .. 6 ...     -1 
+00002e60: e294 8220 2033 3132 2e37 2c20 3437 322e  ...  312.7, 472.
+00002e70: 3120 e294 8220 312e 3735 652b 3034 20e2  1 ... 1.75e+04 .
+00002e80: 9482 2046 616c 7365 20e2 9482 2020 3439  .. False ...  49
+00002e90: 352e 3520 e294 8220 2020 2020 2020 302e  5.5 ...       0.
+00002ea0: 3939 3720 e294 8220 2d38 392e 39c2 b020  997 ... -89.9.. 
+00002eb0: e294 8220 2030 2e37 3737 20e2 9482 0a09  ...  0.777 .....
+00002ec0: e294 8220 3720 e294 8220 2020 2020 2d31  ... 7 ...     -1
+00002ed0: 20e2 9482 2020 3234 312e 392c 2032 3435   ...  241.9, 245
+00002ee0: 2e30 20e2 9482 2031 2e37 3565 2b30 3420  .0 ... 1.75e+04 
+00002ef0: e294 8220 4661 6c73 6520 e294 8220 2034  ... False ...  4
+00002f00: 3936 2e39 20e2 9482 2020 2020 2020 2030  96.9 ...       0
+00002f10: 2e39 3932 20e2 9482 202d 3930 2e30 c2b0  .992 ... -90.0..
+00002f20: 20e2 9482 2020 302e 3737 3720 e294 820a   ...  0.777 ....
+00002f30: 09e2 9482 2038 20e2 9482 2020 2020 2020  .... 8 ...      
+00002f40: 3920 e294 8220 3132 3238 2e30 2c20 3235  9 ... 1228.0, 25
+00002f50: 342e 3320 e294 8220 382e 3134 652b 3034  4.3 ... 8.14e+04
+00002f60: 20e2 9482 2046 616c 7365 20e2 9482 2031   ... False ... 1
+00002f70: 3231 352e 3220 e294 8220 2020 2020 2020  215.2 ...       
+00002f80: 302e 3737 3120 e294 8220 2d37 372e 32c2  0.771 ... -77.2.
+00002f90: b020 e294 8220 2030 2e37 3133 20e2 9482  . ...  0.713 ...
+00002fa0: 0a09 e294 8220 3920 e294 8220 2020 2020  ..... 9 ...     
+00002fb0: 2d31 20e2 9482 2031 3232 352e 322c 2032  -1 ... 1225.2, 2
+00002fc0: 3230 2e30 20e2 9482 2031 2e37 3565 2b30  20.0 ... 1.75e+0
+00002fd0: 3420 e294 8220 4661 6c73 6520 e294 8220  4 ... False ... 
+00002fe0: 2034 3936 2e39 20e2 9482 2020 2020 2020   496.9 ...      
+00002ff0: 2030 2e39 3932 20e2 9482 202d 3930 2e30   0.992 ... -90.0
+00003000: c2b0 20e2 9482 2020 302e 3737 3720 e294  .. ...  0.777 ..
+00003010: 820a 09e2 9494 e294 80e2 9480 e294 80e2  ................
+00003020: 94b4 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003030: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
+00003040: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003050: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003060: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
+00003070: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00003080: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
+00003090: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000030a0: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
+000030b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000030c0: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000030d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000030e0: 9480 e294 80e2 9480 e294 b4e2 9480 e294  ................
+000030f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00003100: e294 80e2 94b4 e294 80e2 9480 e294 80e2  ................
+00003110: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00003120: 980a 6060 600a 0a57 6520 6361 6e20 6469  ..```..We can di
+00003130: 7370 6c61 7920 6120 6c61 6265 6c20 696d  splay a label im
+00003140: 6167 652c 2077 6865 7265 2074 6865 2076  age, where the v
+00003150: 616c 7565 206f 6620 6561 6368 2070 6978  alue of each pix
+00003160: 656c 2069 7320 7468 6520 6c61 6265 6c20  el is the label 
+00003170: 6f66 2074 6865 2062 6c6f 6220 7468 6174  of the blob that
+00003180: 2074 6865 2070 6978 656c 0a62 656c 6f6e   the pixel.belon
+00003190: 6773 2074 6f2c 2074 6865 2060 6964 6020  gs to, the `id` 
+000031a0: 6174 7472 6962 7574 650a 0a60 6060 7079  attribute..```py
+000031b0: 7468 6f6e 0a6c 6162 656c 7320 3d20 626c  thon.labels = bl
+000031c0: 6f62 732e 6c61 6265 6c5f 696d 6167 6528  obs.label_image(
+000031d0: 290a 6c61 6265 6c73 2e64 6973 7028 636f  ).labels.disp(co
+000031e0: 6c6f 726d 6170 3d22 7669 7269 6469 7322  lormap="viridis"
+000031f0: 2c20 6e63 6f6c 6f72 733d 6c65 6e28 626c  , ncolors=len(bl
+00003200: 6f62 7329 2c20 636f 6c6f 7262 6172 3d64  obs), colorbar=d
+00003210: 6963 7428 7368 7269 6e6b 3d30 2e38 2c20  ict(shrink=0.8, 
+00003220: 6173 7065 6374 3d32 302a 302e 3829 290a  aspect=20*0.8)).
+00003230: 6060 600a 0a21 5b46 616c 7365 2063 6f6c  ```..![False col
+00003240: 6f72 206c 6162 656c 2069 6d61 6765 5d28  or label image](
+00003250: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003260: 6f6d 2f70 6574 6572 636f 726b 652f 6d61  om/petercorke/ma
+00003270: 6368 696e 6576 6973 696f 6e2d 746f 6f6c  chinevision-tool
+00003280: 626f 782d 7079 7468 6f6e 2f72 6177 2f6d  box-python/raw/m
+00003290: 6173 7465 722f 6669 6773 2f6d 756c 7469  aster/figs/multi
+000032a0: 5f6c 6162 656c 6c65 642e 706e 6729 0a0a  _labelled.png)..
+000032b0: 5765 2063 616e 2061 6c73 6f20 7468 696e  We can also thin
+000032c0: 6b20 6f66 2074 6865 2062 6c6f 6273 2066  k of the blobs f
+000032d0: 6f72 6d69 6e67 2061 2068 6965 6172 6368  orming a hiearch
+000032e0: 7920 616e 6420 7468 6174 2072 656c 6174  y and that relat
+000032f0: 696f 6e73 6869 7020 6973 2072 6566 6c65  ionship is refle
+00003300: 6374 6564 2069 6e20 7468 6520 6070 6172  cted in the `par
+00003310: 656e 7460 2061 6e64 2060 6368 696c 6472  ent` and `childr
+00003320: 656e 6020 6174 7472 6962 7574 6573 206f  en` attributes o
+00003330: 6620 7468 6520 626c 6f62 732e 0a57 6520  f the blobs..We 
+00003340: 6361 6e20 616c 736f 2065 7870 7265 7373  can also express
+00003350: 2069 7420 6173 2061 2064 6972 6563 7465   it as a directe
+00003360: 6420 6772 6170 680a 0a60 6060 7079 7468  d graph..```pyth
+00003370: 6f6e 0a62 6c6f 6273 2e64 6f74 6669 6c65  on.blobs.dotfile
+00003380: 2873 686f 773d 5472 7565 290a 6060 600a  (show=True).```.
+00003390: 0a21 5b42 6c6f 6220 6869 6572 6172 6368  .![Blob hierarch
+000033a0: 7920 6173 2061 2067 7261 7068 5d28 6874  y as a graph](ht
+000033b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000033c0: 2f70 6574 6572 636f 726b 652f 6d61 6368  /petercorke/mach
+000033d0: 696e 6576 6973 696f 6e2d 746f 6f6c 626f  inevision-toolbo
+000033e0: 782d 7079 7468 6f6e 2f72 6177 2f6d 6173  x-python/raw/mas
+000033f0: 7465 722f 6669 6773 2f62 6c6f 6273 5f67  ter/figs/blobs_g
+00003400: 7261 7068 2e70 6e67 290a 0a23 2323 2043  raph.png)..### C
+00003410: 616d 6572 6120 6d6f 6465 6c6c 696e 670a  amera modelling.
+00003420: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00003430: 6d61 6368 696e 6576 6973 696f 6e74 6f6f  machinevisiontoo
+00003440: 6c62 6f78 2069 6d70 6f72 7420 4365 6e74  lbox import Cent
+00003450: 7261 6c43 616d 6572 610a 6361 6d20 3d20  ralCamera.cam = 
+00003460: 4365 6e74 7261 6c43 616d 6572 6128 663d  CentralCamera(f=
+00003470: 302e 3031 352c 2072 686f 3d31 3065 2d36  0.015, rho=10e-6
+00003480: 2c20 696d 6167 6573 697a 653d 5b31 3238  , imagesize=[128
+00003490: 302c 2031 3032 345d 2c20 7070 3d5b 3634  0, 1024], pp=[64
+000034a0: 302c 2035 3132 5d2c 206e 616d 653d 226d  0, 512], name="m
+000034b0: 7963 616d 6572 6122 290a 7072 696e 7428  ycamera").print(
+000034c0: 6361 6d29 0a20 2020 2020 2020 2020 2020  cam).           
+000034d0: 4e61 6d65 3a20 6d79 6361 6d65 7261 205b  Name: mycamera [
+000034e0: 4365 6e74 7261 6c43 616d 6572 615d 0a20  CentralCamera]. 
+000034f0: 2020 2020 7069 7865 6c20 7369 7a65 3a20      pixel size: 
+00003500: 3165 2d30 3520 7820 3165 2d30 350a 2020  1e-05 x 1e-05.  
+00003510: 2020 2069 6d61 6765 2073 697a 653a 2031     image size: 1
+00003520: 3238 3020 7820 3130 3234 0a20 2020 2020  280 x 1024.     
+00003530: 2020 2020 2020 706f 7365 3a20 7420 3d20        pose: t = 
+00003540: 302c 2030 2c20 303b 2072 7079 2f79 787a  0, 0, 0; rpy/yxz
+00003550: 203d 2030 c2b0 2c20 30c2 b02c 2030 c2b0   = 0.., 0.., 0..
+00003560: 0a20 2020 7072 696e 6369 7061 6c20 7074  .   principal pt
+00003570: 3a20 5b20 2020 2020 3634 3020 2020 2020  : [     640     
+00003580: 2035 3132 5d0a 2020 2066 6f63 616c 206c   512].   focal l
+00003590: 656e 6774 683a 205b 2020 2030 2e30 3135  ength: [   0.015
+000035a0: 2020 2020 302e 3031 355d 0a60 6060 0a0a      0.015].```..
+000035b0: 616e 6420 6974 7320 696e 7472 696e 7369  and its intrinsi
+000035c0: 6320 7061 7261 6d65 7465 7273 2061 7265  c parameters are
+000035d0: 0a0a 6060 6070 7974 686f 6e0a 7072 696e  ..```python.prin
+000035e0: 7428 6361 6d2e 4b29 0a09 5b5b 312e 3530  t(cam.K)..[[1.50
+000035f0: 652b 3033 2030 2e30 3065 2b30 3020 362e  e+03 0.00e+00 6.
+00003600: 3430 652b 3032 5d0a 0920 5b30 2e30 3065  40e+02].. [0.00e
+00003610: 2b30 3020 312e 3530 652b 3033 2035 2e31  +00 1.50e+03 5.1
+00003620: 3265 2b30 325d 0a09 205b 302e 3030 652b  2e+02].. [0.00e+
+00003630: 3030 2030 2e30 3065 2b30 3020 312e 3030  00 0.00e+00 1.00
+00003640: 652b 3030 5d5d 0a60 6060 0a0a 5765 2063  e+00]].```..We c
+00003650: 616e 2064 6566 696e 6520 616e 2061 7262  an define an arb
+00003660: 6974 7261 7279 2070 6f69 6e74 2069 6e20  itrary point in 
+00003670: 7468 6520 776f 726c 640a 0a60 6060 7079  the world..```py
+00003680: 7468 6f6e 0a50 203d 205b 302e 332c 2030  thon.P = [0.3, 0
+00003690: 2e34 2c20 332e 305d 0a60 6060 0a0a 616e  .4, 3.0].```..an
+000036a0: 6420 7468 656e 2070 726f 6a65 6374 2069  d then project i
+000036b0: 7420 696e 746f 2074 6865 2063 616d 6572  t into the camer
+000036c0: 610a 0a60 6060 7079 7468 6f6e 0a70 203d  a..```python.p =
+000036d0: 2063 616d 2e70 726f 6a65 6374 2850 290a   cam.project(P).
+000036e0: 7072 696e 7428 7029 0a09 5b37 3930 2e20  print(p)..[790. 
+000036f0: 3731 322e 5d0a 6060 600a 0a77 6869 6368  712.].```..which
+00003700: 2069 7320 7468 6520 636f 7272 6573 706f   is the correspo
+00003710: 6e64 696e 6720 636f 6f72 6469 6e61 7465  nding coordinate
+00003720: 2069 6e20 7069 7865 6c73 2e20 4966 2077   in pixels. If w
+00003730: 6520 7368 6966 7420 7468 6520 6361 6d65  e shift the came
+00003740: 7261 2073 6c69 6768 746c 7920 7468 6520  ra slightly the 
+00003750: 696d 6167 6520 706c 616e 6520 636f 6f72  image plane coor
+00003760: 6469 6e61 7465 2077 696c 6c20 616c 736f  dinate will also
+00003770: 2063 6861 6e67 650a 0a60 6060 7079 7468   change..```pyth
+00003780: 6f6e 0a70 203d 2063 616d 2e70 726f 6a65  on.p = cam.proje
+00003790: 6374 2850 2c20 543d 5345 3328 302e 312c  ct(P, T=SE3(0.1,
+000037a0: 2030 2c20 3029 2029 0a70 7269 6e74 2870   0, 0) ).print(p
+000037b0: 290a 5b37 3430 2e20 3731 322e 5d0a 6060  ).[740. 712.].``
+000037c0: 600a 0a57 6520 6361 6e20 6465 6669 6e65  `..We can define
+000037d0: 2061 6e20 6564 6765 2d62 6173 6564 2063   an edge-based c
+000037e0: 7562 6520 6d6f 6465 6c20 616e 6420 7072  ube model and pr
+000037f0: 6f6a 6563 7420 6974 2069 6e74 6f20 7468  oject it into th
+00003800: 6520 6361 6d65 7261 2773 2069 6d61 6765  e camera's image
+00003810: 2070 6c61 6e65 0a0a 6060 6070 7974 686f   plane..```pytho
+00003820: 6e0a 6672 6f6d 2073 7061 7469 616c 6d61  n.from spatialma
+00003830: 7468 2069 6d70 6f72 7420 5345 330a 582c  th import SE3.X,
+00003840: 2059 2c20 5a20 3d20 6d6b 6375 6265 2830   Y, Z = mkcube(0
+00003850: 2e32 2c20 706f 7365 3d53 4533 2830 2c20  .2, pose=SE3(0, 
+00003860: 302c 2031 292c 2065 6467 653d 5472 7565  0, 1), edge=True
+00003870: 290a 6361 6d2e 706c 6f74 5f77 6972 6566  ).cam.plot_wiref
+00003880: 7261 6d65 2858 2c20 592c 205a 290a 6060  rame(X, Y, Z).``
+00003890: 600a 0a21 5b50 6572 7370 6563 7469 7665  `..![Perspective
+000038a0: 2063 616d 6572 6120 7669 6577 206f 6620   camera view of 
+000038b0: 6375 6265 5d28 6874 7470 733a 2f2f 6769  cube](https://gi
+000038c0: 7468 7562 2e63 6f6d 2f70 6574 6572 636f  thub.com/peterco
+000038d0: 726b 652f 6d61 6368 696e 6576 6973 696f  rke/machinevisio
+000038e0: 6e2d 746f 6f6c 626f 782d 7079 7468 6f6e  n-toolbox-python
+000038f0: 2f72 6177 2f6d 6173 7465 722f 6669 6773  /raw/master/figs
+00003900: 2f63 7562 652e 706e 6729 0a0a 3c21 2d2d  /cube.png)..<!--
+00003910: 2d6f 7220 7769 7468 2061 2066 6973 6865  -or with a fishe
+00003920: 7965 2063 616d 6572 610a 0a60 6060 6d61  ye camera..```ma
+00003930: 746c 6162 0a3e 3e20 6361 6d20 3d20 4669  tlab.>> cam = Fi
+00003940: 7368 4579 6543 616d 6572 6128 276e 616d  shEyeCamera('nam
+00003950: 6527 2c20 2766 6973 6865 7965 272c 202e  e', 'fisheye', .
+00003960: 2e2e 0a27 7072 6f6a 6563 7469 6f6e 272c  ...'projection',
+00003970: 2027 6571 7569 616e 6775 6c61 7227 2c20   'equiangular', 
+00003980: 2e2e 2e0a 2770 6978 656c 272c 2031 3065  ....'pixel', 10e
+00003990: 2d36 2c20 2e2e 2e0a 2772 6573 6f6c 7574  -6, ....'resolut
+000039a0: 696f 6e27 2c20 5b31 3238 3020 3130 3234  ion', [1280 1024
+000039b0: 5d29 3b0a 3e3e 205b 582c 592c 5a5d 203d  ]);.>> [X,Y,Z] =
+000039c0: 206d 6b63 7562 6528 302e 322c 2027 6365   mkcube(0.2, 'ce
+000039d0: 6e74 7265 272c 205b 302e 322c 2030 2c20  ntre', [0.2, 0, 
+000039e0: 302e 335d 2c20 2765 6467 6527 293b 0a3e  0.3], 'edge');.>
+000039f0: 3e20 6361 6d2e 6d65 7368 2858 2c20 592c  > cam.mesh(X, Y,
+00003a00: 205a 293b 0a60 6060 0a21 5b46 6973 6865   Z);.```.![Fishe
+00003a10: 7965 206c 656e 7320 6361 6d65 7261 2076  ye lens camera v
+00003a20: 6965 775d 2866 6967 732f 6375 6265 5f66  iew](figs/cube_f
+00003a30: 6973 6865 7965 2e70 6e67 290a 0a0a 2323  isheye.png)...##
+00003a40: 2320 4275 6e64 6c65 2061 646a 7573 746d  # Bundle adjustm
+00003a50: 656e 740a 2d2d 2d3e 0a0a 2323 2320 436f  ent.--->..### Co
+00003a60: 6c6f 7220 7370 6163 650a 0a50 6c6f 7420  lor space..Plot 
+00003a70: 7468 6520 4349 4520 6368 726f 6d61 7469  the CIE chromati
+00003a80: 6369 7479 2073 7061 6365 0a0a 6060 6070  city space..```p
+00003a90: 7974 686f 6e0a 706c 6f74 5f63 6872 6f6d  ython.plot_chrom
+00003aa0: 6174 6963 6974 795f 6469 6167 7261 6d28  aticity_diagram(
+00003ab0: 2278 7922 293b 0a70 6c6f 745f 7370 6563  "xy");.plot_spec
+00003ac0: 7472 616c 5f6c 6f63 7573 2822 7879 2229  tral_locus("xy")
+00003ad0: 0a60 6060 0a0a 215b 4349 4520 6368 726f  .```..![CIE chro
+00003ae0: 6d61 7469 6369 7479 2073 7061 6365 5d28  maticity space](
+00003af0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003b00: 6f6d 2f70 6574 6572 636f 726b 652f 6d61  om/petercorke/ma
+00003b10: 6368 696e 6576 6973 696f 6e2d 746f 6f6c  chinevision-tool
+00003b20: 626f 782d 7079 7468 6f6e 2f72 6177 2f6d  box-python/raw/m
+00003b30: 6173 7465 722f 6669 6773 2f63 6f6c 6f72  aster/figs/color
+00003b40: 7370 6163 652e 706e 6729 0a0a 4c6f 6164  space.png)..Load
+00003b50: 2074 6865 2073 7065 6374 7275 6d20 6f66   the spectrum of
+00003b60: 2073 756e 6c69 6768 7420 6174 2074 6865   sunlight at the
+00003b70: 2045 6172 7468 2773 2073 7572 6661 6365   Earth's surface
+00003b80: 2061 6e64 2063 6f6d 7075 7465 2074 6865   and compute the
+00003b90: 2043 4945 2078 7920 6368 726f 6d61 7469   CIE xy chromati
+00003ba0: 6369 7479 2063 6f6f 7264 696e 6174 6573  city coordinates
+00003bb0: 0a0a 6060 6070 7974 686f 6e0a 6e6d 203d  ..```python.nm =
+00003bc0: 2031 652d 390a 6c61 6d20 3d20 6e70 2e6c   1e-9.lam = np.l
+00003bd0: 696e 7370 6163 6528 3430 302c 2037 3031  inspace(400, 701
+00003be0: 2c20 3529 202a 206e 6d20 2320 7669 7369  , 5) * nm # visi
+00003bf0: 626c 6520 6c69 6768 740a 7375 6e5f 6174  ble light.sun_at
+00003c00: 5f67 726f 756e 6420 3d20 6c6f 6164 7370  _ground = loadsp
+00003c10: 6563 7472 756d 286c 616d 2c20 2273 6f6c  ectrum(lam, "sol
+00003c20: 6172 2229 0a78 7920 3d20 6c61 6d62 6461  ar").xy = lambda
+00003c30: 3278 7928 6c61 6d62 6461 2c20 7375 6e5f  2xy(lambda, sun_
+00003c40: 6174 5f67 726f 756e 6429 0a70 7269 6e74  at_ground).print
+00003c50: 2878 7929 0a09 5b5b 302e 3333 3237 3237  (xy)..[[0.332727
+00003c60: 3938 2030 2e33 3435 3430 3133 205d 5d0a  98 0.3454013 ]].
+00003c70: 7072 696e 7428 636f 6c6f 726e 616d 6528  print(colorname(
+00003c80: 7879 2c20 2278 7922 2929 0a09 6b68 616b  xy, "xy"))..khak
+00003c90: 690a 6060 600a 0a23 2323 2048 6f75 6768  i.```..### Hough
+00003ca0: 2074 7261 6e73 666f 726d 0a0a 6060 6070   transform..```p
+00003cb0: 7974 686f 6e0a 696d 203d 2049 6d61 6765  ython.im = Image
+00003cc0: 2e52 6561 6428 2263 6875 7263 682e 706e  .Read("church.pn
+00003cd0: 6722 2c20 6d6f 6e6f 3d54 7275 6529 0a65  g", mono=True).e
+00003ce0: 6467 6573 203d 2069 6d2e 6361 6e6e 7928  dges = im.canny(
+00003cf0: 290a 6820 3d20 6564 6765 732e 486f 7567  ).h = edges.Houg
+00003d00: 6828 290a 6c69 6e65 7320 3d20 682e 6c69  h().lines = h.li
+00003d10: 6e65 735f 7028 3130 302c 206d 696e 6c69  nes_p(100, minli
+00003d20: 6e65 6c65 6e67 7468 3d32 3030 2c20 6d61  nelength=200, ma
+00003d30: 786c 696e 6567 6170 3d35 2c20 7365 6564  xlinegap=5, seed
+00003d40: 3d30 290a 0a69 6d2e 6469 7370 2864 6172  =0)..im.disp(dar
+00003d50: 6b65 6e3d 5472 7565 290a 682e 706c 6f74  ken=True).h.plot
+00003d60: 5f6c 696e 6573 286c 696e 6573 2c20 2272  _lines(lines, "r
+00003d70: 2d2d 2229 0a60 6060 0a0a 215b 486f 7567  --").```..![Houg
+00003d80: 6820 7472 616e 7366 6f72 6d5d 2868 7474  h transform](htt
+00003d90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00003da0: 7065 7465 7263 6f72 6b65 2f6d 6163 6869  petercorke/machi
+00003db0: 6e65 7669 7369 6f6e 2d74 6f6f 6c62 6f78  nevision-toolbox
+00003dc0: 2d70 7974 686f 6e2f 7261 772f 6d61 7374  -python/raw/mast
+00003dd0: 6572 2f66 6967 732f 686f 7567 682e 706e  er/figs/hough.pn
+00003de0: 6729 0a0a 2323 2320 5355 5246 2066 6561  g)..### SURF fea
+00003df0: 7475 7265 730a 0a57 6520 6c6f 6164 2074  tures..We load t
+00003e00: 776f 2069 6d61 6765 7320 616e 6420 636f  wo images and co
+00003e10: 6d70 7574 6520 6120 7365 7420 6f66 2053  mpute a set of S
+00003e20: 5552 4620 6665 6174 7572 6573 2066 6f72  URF features for
+00003e30: 2065 6163 680a 0a60 6060 7079 7468 6f6e   each..```python
+00003e40: 0a76 6965 7731 203d 2049 6d61 6765 2e52  .view1 = Image.R
+00003e50: 6561 6428 2265 6966 6665 6c2d 312e 706e  ead("eiffel-1.pn
+00003e60: 6722 2c20 6d6f 6e6f 3d54 7275 6529 0a76  g", mono=True).v
+00003e70: 6965 7732 203d 2049 6d61 6765 2e52 6561  iew2 = Image.Rea
+00003e80: 6428 2265 6966 6665 6c2d 322e 706e 6722  d("eiffel-2.png"
+00003e90: 2c20 6d6f 6e6f 3d54 7275 6529 0a73 6631  , mono=True).sf1
+00003ea0: 203d 2076 6965 7731 2e53 4946 5428 290a   = view1.SIFT().
+00003eb0: 7366 3220 3d20 7669 6577 322e 5349 4654  sf2 = view2.SIFT
+00003ec0: 2829 0a60 6060 0a0a 5765 2063 616e 206d  ().```..We can m
+00003ed0: 6174 6368 2066 6561 7475 7265 7320 6265  atch features be
+00003ee0: 7477 6565 6e20 696d 6167 6573 2062 6173  tween images bas
+00003ef0: 6564 2070 7572 656c 7920 6f6e 2074 6865  ed purely on the
+00003f00: 2073 696d 696c 6172 6974 7920 6f66 2074   similarity of t
+00003f10: 6865 2066 6561 7475 7265 732c 2061 6e64  he features, and
+00003f20: 2064 6973 706c 6179 2074 6865 2063 6f72   display the cor
+00003f30: 7265 7370 6f6e 6465 6e63 6573 2066 6f75  respondences fou
+00003f40: 6e64 0a0a 6060 6070 7974 686f 6e0a 6d61  nd..```python.ma
+00003f50: 7463 6865 7320 3d20 7366 312e 6d61 7463  tches = sf1.matc
+00003f60: 6828 7366 3229 0a70 7269 6e74 286d 6174  h(sf2).print(mat
+00003f70: 6368 6573 290a 3831 3320 6d61 7463 6865  ches).813 matche
+00003f80: 730a 6d61 7463 6865 735b 313a 355d 2e74  s.matches[1:5].t
+00003f90: 6162 6c65 2829 0ae2 948c e294 80e2 9480  able()..........
+00003fa0: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
+00003fb0: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
 00003fc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00003fd0: e294 b4e2 9480 e294 80e2 9480 e294 80e2  ................
+00003fd0: e294 80e2 9480 e294 80e2 9480 e294 ace2  ................
 00003fe0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 00003ff0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004000: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
-00004010: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004000: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004010: 9480 e294 ace2 9480 e294 80e2 9480 e294  ................
 00004020: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00004030: e294 80e2 9480 e294 80e2 9498 0a60 6060  .............```
-00004040: 0a0a 7768 6572 6520 7765 2068 6176 6520  ..where we have 
-00004050: 6469 7370 6c61 7965 6420 7468 6520 6665  displayed the fe
-00004060: 6174 7572 6520 636f 6f72 6469 6e61 7465  ature coordinate
-00004070: 7320 666f 7220 666f 7572 2063 6f72 7265  s for four corre
-00004080: 7370 6f6e 6465 6e63 6573 2e0a 0a57 6520  spondences...We 
-00004090: 6361 6e20 616c 736f 2064 6973 706c 6179  can also display
-000040a0: 2074 6865 2063 6f72 7265 7370 6f6e 6465   the corresponde
-000040b0: 6e63 6573 2067 7261 7068 6963 616c 6c79  nces graphically
-000040c0: 0a0a 6060 6070 7974 686f 6e0a 6d61 7463  ..```python.matc
-000040d0: 6865 732e 7375 6273 6574 2831 3030 292e  hes.subset(100).
-000040e0: 706c 6f74 2822 7722 290a 6060 600a 0a69  plot("w").```..i
-000040f0: 6e20 7468 6973 2063 6173 652c 2061 2073  n this case, a s
-00004100: 7562 7365 7420 6f66 2031 3030 2f38 3133  ubset of 100/813
-00004110: 206f 6620 7468 6520 636f 7272 6573 706f   of the correspo
-00004120: 6e64 656e 6365 732e 0a0a 215b 4665 6174  ndences...![Feat
-00004130: 7572 6520 6d61 7463 6869 6e67 5d28 6874  ure matching](ht
-00004140: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00004150: 2f70 6574 6572 636f 726b 652f 6d61 6368  /petercorke/mach
-00004160: 696e 6576 6973 696f 6e2d 746f 6f6c 626f  inevision-toolbo
-00004170: 782d 7079 7468 6f6e 2f72 6177 2f6d 6173  x-python/raw/mas
-00004180: 7465 722f 6669 6773 2f6d 6174 6368 696e  ter/figs/matchin
-00004190: 672e 706e 6729 0a0a 436c 6561 726c 7920  g.png)..Clearly 
-000041a0: 7468 6572 6520 6172 6520 736f 6d65 2062  there are some b
-000041b0: 6164 206d 6174 6368 6573 2068 6572 652c  ad matches here,
-000041c0: 2062 7574 2077 6520 7765 2063 616e 2075   but we we can u
-000041d0: 7365 2052 414e 5341 4320 616e 6420 7468  se RANSAC and th
-000041e0: 6520 6570 6970 6f6c 6172 2063 6f6e 7374  e epipolar const
-000041f0: 7261 696e 7420 696d 706c 6965 6420 6279  raint implied by
-00004200: 2074 6865 2066 756e 6461 6d65 6e74 616c   the fundamental
-00004210: 206d 6174 7269 7820 746f 2065 7374 696d   matrix to estim
-00004220: 6174 6520 7468 6520 6675 6e64 616d 656e  ate the fundamen
-00004230: 7461 6c20 6d61 7472 6978 2061 6e64 2063  tal matrix and c
-00004240: 6c61 7373 6966 7920 636f 7272 6573 706f  lassify correspo
-00004250: 6e64 656e 6365 7320 6173 2069 6e6c 6965  ndences as inlie
-00004260: 7273 206f 7220 6f75 746c 6965 7273 0a0a  rs or outliers..
-00004270: 6060 6070 7974 686f 6e0a 462c 2072 6573  ```python.F, res
-00004280: 6964 203d 206d 6174 6368 6573 2e65 7374  id = matches.est
-00004290: 696d 6174 6528 4365 6e74 7261 6c43 616d  imate(CentralCam
-000042a0: 6572 612e 706f 696e 7473 3246 2c20 6d65  era.points2F, me
-000042b0: 7468 6f64 3d22 7261 6e73 6163 222c 2063  thod="ransac", c
-000042c0: 6f6e 6669 6465 6e63 653d 302e 3939 2c20  onfidence=0.99, 
-000042d0: 7365 6564 3d30 290a 7072 696e 7428 4629  seed=0).print(F)
-000042e0: 0a61 7272 6179 285b 5b31 2e30 3333 652d  .array([[1.033e-
-000042f0: 3038 2c20 2d33 2e37 3939 652d 3036 2c20  08, -3.799e-06, 
-00004300: 302e 3030 3236 3738 5d2c 0a20 2020 2020  0.002678],.     
-00004310: 2020 5b33 2e36 3638 652d 3036 2c20 312e    [3.668e-06, 1.
-00004320: 3231 3765 2d30 372c 202d 302e 3030 3430  217e-07, -0.0040
-00004330: 3333 5d2c 0a20 2020 2020 2020 5b2d 302e  33],.       [-0.
-00004340: 3030 3331 392c 2030 2e30 3033 3433 362c  00319, 0.003436,
-00004350: 2020 2020 2020 2020 315d 5d29 0a70 7269          1]]).pri
-00004360: 6e74 2872 6573 6964 290a 302e 3034 3035  nt(resid).0.0405
-00004370: 0a0a 496d 6167 652e 4873 7461 636b 2828  ..Image.Hstack((
-00004380: 7669 6577 312c 2076 6965 7732 2929 2e64  view1, view2)).d
-00004390: 6973 7028 290a 6d61 7463 6865 732e 696e  isp().matches.in
-000043a0: 6c69 6572 732e 7375 6273 6574 2831 3030  liers.subset(100
-000043b0: 292e 706c 6f74 2822 6722 2c20 6178 3d70  ).plot("g", ax=p
-000043c0: 6c74 2e67 6361 2829 290a 6d61 7463 6865  lt.gca()).matche
-000043d0: 732e 6f75 746c 6965 7273 2e73 7562 7365  s.outliers.subse
-000043e0: 7428 3130 3029 2e70 6c6f 7428 2272 222c  t(100).plot("r",
-000043f0: 2061 783d 706c 742e 6763 6128 2929 0a60   ax=plt.gca()).`
-00004400: 6060 0a0a 7768 6572 6520 6772 6565 6e20  ``..where green 
-00004410: 6c69 6e65 7320 7368 6f77 2063 6f72 7265  lines show corre
-00004420: 6374 2063 6f72 7265 7370 6f6e 6465 6e63  ct correspondenc
-00004430: 6573 2028 696e 6c69 6572 7329 2061 6e64  es (inliers) and
-00004440: 2072 6564 206c 696e 6573 2073 686f 7720   red lines show 
-00004450: 6261 6420 636f 7272 6573 706f 6e64 656e  bad corresponden
-00004460: 6365 7320 286f 7574 6c69 6572 7329 0a0a  ces (outliers)..
-00004470: 215b 4665 6174 7572 6520 6d61 7463 6869  ![Feature matchi
-00004480: 6e67 2061 6674 6572 2052 414e 5341 435d  ng after RANSAC]
-00004490: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000044a0: 636f 6d2f 7065 7465 7263 6f72 6b65 2f6d  com/petercorke/m
-000044b0: 6163 6869 6e65 7669 7369 6f6e 2d74 6f6f  achinevision-too
-000044c0: 6c62 6f78 2d70 7974 686f 6e2f 7261 772f  lbox-python/raw/
-000044d0: 6d61 7374 6572 2f66 6967 732f 6d61 7463  master/figs/matc
-000044e0: 6869 6e67 5f72 616e 7361 632e 706e 6729  hing_ransac.png)
-000044f0: 0a0a 2320 4869 7374 6f72 790a 0a54 6869  ..# History..Thi
-00004500: 7320 7061 636b 6167 6520 6361 6e20 6265  s package can be
-00004510: 2063 6f6e 7369 6465 7265 6420 6173 2061   considered as a
-00004520: 2050 7974 686f 6e20 7665 7273 696f 6e20   Python version 
-00004530: 6f66 2074 6865 205b 4d61 6368 696e 6520  of the [Machine 
-00004540: 5669 7369 6f6e 0a54 6f6f 6c62 6f78 2066  Vision.Toolbox f
-00004550: 6f72 204d 4154 4c41 425d 2829 2e20 5468  or MATLAB](). Th
-00004560: 6174 2054 6f6f 6c62 6f78 2c20 6e6f 7720  at Toolbox, now 
-00004570: 7175 6974 6520 6f6c 642c 2069 7320 6120  quite old, is a 
-00004580: 636f 6c6c 6563 7469 6f6e 206f 6620 4d41  collection of MA
-00004590: 544c 4142 0a66 756e 6374 696f 6e73 2061  TLAB.functions a
-000045a0: 6e64 2063 6c61 7373 6573 2074 6861 7420  nd classes that 
-000045b0: 7375 7070 6f72 7465 6420 7468 6520 6669  supported the fi
-000045c0: 7273 7420 7477 6f20 6564 6974 696f 6e73  rst two editions
-000045d0: 206f 6620 7468 6520 526f 626f 7469 6373   of the Robotics
-000045e0: 2c0a 5669 7369 6f6e 2026 2043 6f6e 7472  ,.Vision & Contr
-000045f0: 6f6c 2062 6f6f 6b2e 2049 7420 6973 2061  ol book. It is a
-00004600: 2073 6f6d 6577 6861 7420 6563 6c65 6374   somewhat eclect
-00004610: 6963 2063 6f6c 6c65 6374 696f 6e20 7265  ic collection re
-00004620: 666c 6563 7469 6e67 206d 790a 7065 7273  flecting my.pers
-00004630: 6f6e 616c 2069 6e74 6572 6573 7420 696e  onal interest in
-00004640: 2061 7265 6173 206f 6620 7068 6f74 6f6d   areas of photom
-00004650: 6574 7279 2c20 7068 6f74 6f67 7261 6d6d  etry, photogramm
-00004660: 6574 7279 2c20 636f 6c6f 7269 6d65 7472  etry, colorimetr
-00004670: 792e 2049 740a 696e 636c 7564 6573 206f  y. It.includes o
-00004680: 7665 7220 3130 3020 6675 6e63 7469 6f6e  ver 100 function
-00004690: 7320 7370 616e 6e69 6e67 206f 7065 7261  s spanning opera
-000046a0: 7469 6f6e 7320 7375 6368 2061 7320 696d  tions such as im
-000046b0: 6167 6520 6669 6c65 2072 6561 6469 6e67  age file reading
-000046c0: 2061 6e64 0a77 7269 7469 6e67 2c20 6163   and.writing, ac
-000046d0: 7175 6973 6974 696f 6e2c 2064 6973 706c  quisition, displ
-000046e0: 6179 2c20 6669 6c74 6572 696e 672c 2062  ay, filtering, b
-000046f0: 6c6f 622c 2070 6f69 6e74 2061 6e64 206c  lob, point and l
-00004700: 696e 6520 6665 6174 7572 650a 6578 7472  ine feature.extr
-00004710: 6163 7469 6f6e 2c20 6d61 7468 656d 6174  action, mathemat
-00004720: 6963 616c 206d 6f72 7068 6f6c 6f67 792c  ical morphology,
-00004730: 2068 6f6d 6f67 7261 7068 6965 732c 2076   homographies, v
-00004740: 6973 7561 6c20 4a61 636f 6269 616e 732c  isual Jacobians,
-00004750: 2063 616d 6572 610a 6361 6c69 6272 6174   camera.calibrat
-00004760: 696f 6e20 616e 6420 636f 6c6f 7220 7370  ion and color sp
-00004770: 6163 6520 636f 6e76 6572 7369 6f6e 2e0a  ace conversion..
-00004780: 0a54 6869 7320 5079 7468 6f6e 2076 6572  .This Python ver
-00004790: 7369 6f6e 2064 6966 6665 7273 2069 6e20  sion differs in 
-000047a0: 7573 696e 6720 616e 206f 626a 6563 7420  using an object 
-000047b0: 746f 2065 6e63 6170 7375 6c61 7465 2074  to encapsulate t
-000047c0: 6865 2070 6978 656c 2064 6174 6120 616e  he pixel data an
-000047d0: 640a 696d 6167 6520 6d65 7461 6461 7461  d.image metadata
-000047e0: 2c20 7261 7468 6572 2074 6861 6e20 6a75  , rather than ju
-000047f0: 7374 2061 206e 6174 6976 6520 6f62 6a65  st a native obje
-00004800: 6374 2068 6f6c 6469 6e67 2070 6978 656c  ct holding pixel
-00004810: 2064 6174 612e 2054 6865 206d 616e 790a   data. The many.
-00004820: 6675 6e63 7469 6f6e 7320 6265 636f 6d65  functions become
-00004830: 206d 6574 686f 6473 206f 6620 7468 6520   methods of the 
-00004840: 696d 6167 6520 6f62 6a65 6374 2077 6869  image object whi
-00004850: 6368 2072 6564 7563 6573 206e 616d 6573  ch reduces names
-00004860: 7061 6365 2070 6f6c 6c75 7469 6f6e 732c  pace pollutions,
-00004870: 0a61 6e64 2061 6c6c 6f77 7320 7468 6520  .and allows the 
-00004880: 6561 7379 2065 7870 7265 7373 696f 6e20  easy expression 
-00004890: 6f66 2073 6571 7565 6e74 6961 6c20 6f70  of sequential op
-000048a0: 6572 6174 696f 6e73 2075 7369 6e67 2022  erations using "
-000048b0: 646f 7420 6368 6169 6e69 6e67 222e 0a0a  dot chaining"...
-000048c0: 5468 6520 6669 7273 7420 7665 7273 696f  The first versio
-000048d0: 6e20 7761 7320 6372 6561 7465 6420 6279  n was created by
-000048e0: 2044 6f72 6961 6e20 5473 6169 2064 7572   Dorian Tsai dur
-000048f0: 696e 6720 3230 3230 2c20 616e 6420 6261  ing 2020, and ba
-00004900: 7365 6420 6f6e 2074 6865 0a4d 4154 4c41  sed on the.MATLA
-00004910: 4220 7665 7273 696f 6e2e 2020 5468 6174  B version.  That
-00004920: 2077 6f72 6b20 7761 7320 6675 6e64 6564   work was funded
-00004930: 2062 7920 616e 2041 7573 7472 616c 6961   by an Australia
-00004940: 6e20 556e 6976 6572 7369 7479 2054 6561  n University Tea
-00004950: 6368 6572 206f 660a 7468 6520 7965 6172  cher of.the year
-00004960: 2061 7761 7264 2028 3230 3137 2920 746f   award (2017) to
-00004970: 2050 6574 6572 2043 6f72 6b65 2e0a        Peter Corke..
+00004030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004040: 9480 e294 80e2 9490 0ae2 9482 2320 e294  ............# ..
+00004050: 8220 696e 6c69 6572 20e2 9482 2073 7472  . inlier ... str
+00004060: 656e 6774 6820 e294 8220 2020 2020 2020  ength ...       
+00004070: 2020 2020 2020 2070 3120 e294 8220 2020         p1 ...   
+00004080: 2020 2020 2020 2020 2020 7032 20e2 9482            p2 ...
+00004090: 0ae2 949c e294 80e2 9480 e294 bce2 9480  ................
+000040a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000040b0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+000040c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000040d0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+000040e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000040f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004100: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+00004110: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004120: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00004130: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004140: 94a4 0ae2 9482 3020 e294 8220 2020 2020  ......0 ...     
+00004150: 2020 20e2 9482 2020 2020 2032 362e 3420     ...     26.4 
+00004160: e294 8220 2831 3131 382e 362c 2031 3738  ... (1118.6, 178
+00004170: 2e38 2920 e294 8220 2839 3532 2e35 2c20  .8) ... (952.5, 
+00004180: 3431 382e 3029 20e2 9482 0ae2 9482 3120  418.0) .......1 
+00004190: e294 8220 2020 2020 2020 20e2 9482 2020  ...        ...  
+000041a0: 2020 2032 382e 3220 e294 8220 2838 3230     28.2 ... (820
+000041b0: 2e36 2c20 3531 392e 3129 2020 e294 8220  .6, 519.1)  ... 
+000041c0: 2837 3038 2e31 2c20 3730 312e 3629 20e2  (708.1, 701.6) .
+000041d0: 9482 0ae2 9482 3220 e294 8220 2020 2020  ......2 ...     
+000041e0: 2020 20e2 9482 2020 2020 2032 392e 3620     ...     29.6 
+000041f0: e294 8220 2838 3031 2e31 2c20 3633 322e  ... (801.1, 632.
+00004200: 3429 2020 e294 8220 2836 3934 2e31 2c20  4)  ... (694.1, 
+00004210: 3830 302e 3329 20e2 9482 0ae2 9482 3320  800.3) .......3 
+00004220: e294 8220 2020 2020 2020 20e2 9482 2020  ...        ...  
+00004230: 2020 2033 322e 3420 e294 8220 2837 3436     32.4 ... (746
+00004240: 2e30 2c20 3135 332e 3129 2020 e294 8220  .0, 153.1)  ... 
+00004250: 2836 3434 2e35 2c20 3339 322e 3229 20e2  (644.5, 392.2) .
+00004260: 9482 0ae2 9494 e294 80e2 9480 e294 b4e2  ................
+00004270: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004280: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
+00004290: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000042a0: 9480 e294 80e2 9480 e294 b4e2 9480 e294  ................
+000042b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000042c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+000042d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+000042e0: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000042f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00004300: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00004310: 80e2 9498 0a60 6060 0a0a 7768 6572 6520  .....```..where 
+00004320: 7765 2068 6176 6520 6469 7370 6c61 7965  we have displaye
+00004330: 6420 7468 6520 6665 6174 7572 6520 636f  d the feature co
+00004340: 6f72 6469 6e61 7465 7320 666f 7220 666f  ordinates for fo
+00004350: 7572 2063 6f72 7265 7370 6f6e 6465 6e63  ur correspondenc
+00004360: 6573 2e0a 0a57 6520 6361 6e20 616c 736f  es...We can also
+00004370: 2064 6973 706c 6179 2074 6865 2063 6f72   display the cor
+00004380: 7265 7370 6f6e 6465 6e63 6573 2067 7261  respondences gra
+00004390: 7068 6963 616c 6c79 0a0a 6060 6070 7974  phically..```pyt
+000043a0: 686f 6e0a 6d61 7463 6865 732e 7375 6273  hon.matches.subs
+000043b0: 6574 2831 3030 292e 706c 6f74 2822 7722  et(100).plot("w"
+000043c0: 290a 6060 600a 0a69 6e20 7468 6973 2063  ).```..in this c
+000043d0: 6173 652c 2061 2073 7562 7365 7420 6f66  ase, a subset of
+000043e0: 2031 3030 2f38 3133 206f 6620 7468 6520   100/813 of the 
+000043f0: 636f 7272 6573 706f 6e64 656e 6365 732e  correspondences.
+00004400: 0a0a 215b 4665 6174 7572 6520 6d61 7463  ..![Feature matc
+00004410: 6869 6e67 5d28 6874 7470 733a 2f2f 6769  hing](https://gi
+00004420: 7468 7562 2e63 6f6d 2f70 6574 6572 636f  thub.com/peterco
+00004430: 726b 652f 6d61 6368 696e 6576 6973 696f  rke/machinevisio
+00004440: 6e2d 746f 6f6c 626f 782d 7079 7468 6f6e  n-toolbox-python
+00004450: 2f72 6177 2f6d 6173 7465 722f 6669 6773  /raw/master/figs
+00004460: 2f6d 6174 6368 696e 672e 706e 6729 0a0a  /matching.png)..
+00004470: 436c 6561 726c 7920 7468 6572 6520 6172  Clearly there ar
+00004480: 6520 736f 6d65 2062 6164 206d 6174 6368  e some bad match
+00004490: 6573 2068 6572 652c 2062 7574 2077 6520  es here, but we 
+000044a0: 7765 2063 616e 2075 7365 2052 414e 5341  we can use RANSA
+000044b0: 4320 616e 6420 7468 6520 6570 6970 6f6c  C and the epipol
+000044c0: 6172 2063 6f6e 7374 7261 696e 7420 696d  ar constraint im
+000044d0: 706c 6965 6420 6279 2074 6865 2066 756e  plied by the fun
+000044e0: 6461 6d65 6e74 616c 206d 6174 7269 7820  damental matrix 
+000044f0: 746f 2065 7374 696d 6174 6520 7468 6520  to estimate the 
+00004500: 6675 6e64 616d 656e 7461 6c20 6d61 7472  fundamental matr
+00004510: 6978 2061 6e64 2063 6c61 7373 6966 7920  ix and classify 
+00004520: 636f 7272 6573 706f 6e64 656e 6365 7320  correspondences 
+00004530: 6173 2069 6e6c 6965 7273 206f 7220 6f75  as inliers or ou
+00004540: 746c 6965 7273 0a0a 6060 6070 7974 686f  tliers..```pytho
+00004550: 6e0a 462c 2072 6573 6964 203d 206d 6174  n.F, resid = mat
+00004560: 6368 6573 2e65 7374 696d 6174 6528 4365  ches.estimate(Ce
+00004570: 6e74 7261 6c43 616d 6572 612e 706f 696e  ntralCamera.poin
+00004580: 7473 3246 2c20 6d65 7468 6f64 3d22 7261  ts2F, method="ra
+00004590: 6e73 6163 222c 2063 6f6e 6669 6465 6e63  nsac", confidenc
+000045a0: 653d 302e 3939 2c20 7365 6564 3d30 290a  e=0.99, seed=0).
+000045b0: 7072 696e 7428 4629 0a61 7272 6179 285b  print(F).array([
+000045c0: 5b31 2e30 3333 652d 3038 2c20 2d33 2e37  [1.033e-08, -3.7
+000045d0: 3939 652d 3036 2c20 302e 3030 3236 3738  99e-06, 0.002678
+000045e0: 5d2c 0a20 2020 2020 2020 5b33 2e36 3638  ],.       [3.668
+000045f0: 652d 3036 2c20 312e 3231 3765 2d30 372c  e-06, 1.217e-07,
+00004600: 202d 302e 3030 3430 3333 5d2c 0a20 2020   -0.004033],.   
+00004610: 2020 2020 5b2d 302e 3030 3331 392c 2030      [-0.00319, 0
+00004620: 2e30 3033 3433 362c 2020 2020 2020 2020  .003436,        
+00004630: 315d 5d29 0a70 7269 6e74 2872 6573 6964  1]]).print(resid
+00004640: 290a 302e 3034 3035 0a0a 496d 6167 652e  ).0.0405..Image.
+00004650: 4873 7461 636b 2828 7669 6577 312c 2076  Hstack((view1, v
+00004660: 6965 7732 2929 2e64 6973 7028 290a 6d61  iew2)).disp().ma
+00004670: 7463 6865 732e 696e 6c69 6572 732e 7375  tches.inliers.su
+00004680: 6273 6574 2831 3030 292e 706c 6f74 2822  bset(100).plot("
+00004690: 6722 2c20 6178 3d70 6c74 2e67 6361 2829  g", ax=plt.gca()
+000046a0: 290a 6d61 7463 6865 732e 6f75 746c 6965  ).matches.outlie
+000046b0: 7273 2e73 7562 7365 7428 3130 3029 2e70  rs.subset(100).p
+000046c0: 6c6f 7428 2272 222c 2061 783d 706c 742e  lot("r", ax=plt.
+000046d0: 6763 6128 2929 0a60 6060 0a0a 7768 6572  gca()).```..wher
+000046e0: 6520 6772 6565 6e20 6c69 6e65 7320 7368  e green lines sh
+000046f0: 6f77 2063 6f72 7265 6374 2063 6f72 7265  ow correct corre
+00004700: 7370 6f6e 6465 6e63 6573 2028 696e 6c69  spondences (inli
+00004710: 6572 7329 2061 6e64 2072 6564 206c 696e  ers) and red lin
+00004720: 6573 2073 686f 7720 6261 6420 636f 7272  es show bad corr
+00004730: 6573 706f 6e64 656e 6365 7320 286f 7574  espondences (out
+00004740: 6c69 6572 7329 0a0a 215b 4665 6174 7572  liers)..![Featur
+00004750: 6520 6d61 7463 6869 6e67 2061 6674 6572  e matching after
+00004760: 2052 414e 5341 435d 2868 7474 7073 3a2f   RANSAC](https:/
+00004770: 2f67 6974 6875 622e 636f 6d2f 7065 7465  /github.com/pete
+00004780: 7263 6f72 6b65 2f6d 6163 6869 6e65 7669  rcorke/machinevi
+00004790: 7369 6f6e 2d74 6f6f 6c62 6f78 2d70 7974  sion-toolbox-pyt
+000047a0: 686f 6e2f 7261 772f 6d61 7374 6572 2f66  hon/raw/master/f
+000047b0: 6967 732f 6d61 7463 6869 6e67 5f72 616e  igs/matching_ran
+000047c0: 7361 632e 706e 6729 0a0a 2320 4869 7374  sac.png)..# Hist
+000047d0: 6f72 790a 0a54 6869 7320 7061 636b 6167  ory..This packag
+000047e0: 6520 6361 6e20 6265 2063 6f6e 7369 6465  e can be conside
+000047f0: 7265 6420 6173 2061 2050 7974 686f 6e20  red as a Python 
+00004800: 7665 7273 696f 6e20 6f66 2074 6865 205b  version of the [
+00004810: 4d61 6368 696e 6520 5669 7369 6f6e 0a54  Machine Vision.T
+00004820: 6f6f 6c62 6f78 2066 6f72 204d 4154 4c41  oolbox for MATLA
+00004830: 425d 2829 2e20 5468 6174 2054 6f6f 6c62  B](). That Toolb
+00004840: 6f78 2c20 6e6f 7720 7175 6974 6520 6f6c  ox, now quite ol
+00004850: 642c 2069 7320 6120 636f 6c6c 6563 7469  d, is a collecti
+00004860: 6f6e 206f 6620 4d41 544c 4142 0a66 756e  on of MATLAB.fun
+00004870: 6374 696f 6e73 2061 6e64 2063 6c61 7373  ctions and class
+00004880: 6573 2074 6861 7420 7375 7070 6f72 7465  es that supporte
+00004890: 6420 7468 6520 6669 7273 7420 7477 6f20  d the first two 
+000048a0: 6564 6974 696f 6e73 206f 6620 7468 6520  editions of the 
+000048b0: 526f 626f 7469 6373 2c0a 5669 7369 6f6e  Robotics,.Vision
+000048c0: 2026 2043 6f6e 7472 6f6c 2062 6f6f 6b2e   & Control book.
+000048d0: 2049 7420 6973 2061 2073 6f6d 6577 6861   It is a somewha
+000048e0: 7420 6563 6c65 6374 6963 2063 6f6c 6c65  t eclectic colle
+000048f0: 6374 696f 6e20 7265 666c 6563 7469 6e67  ction reflecting
+00004900: 206d 790a 7065 7273 6f6e 616c 2069 6e74   my.personal int
+00004910: 6572 6573 7420 696e 2061 7265 6173 206f  erest in areas o
+00004920: 6620 7068 6f74 6f6d 6574 7279 2c20 7068  f photometry, ph
+00004930: 6f74 6f67 7261 6d6d 6574 7279 2c20 636f  otogrammetry, co
+00004940: 6c6f 7269 6d65 7472 792e 2049 740a 696e  lorimetry. It.in
+00004950: 636c 7564 6573 206f 7665 7220 3130 3020  cludes over 100 
+00004960: 6675 6e63 7469 6f6e 7320 7370 616e 6e69  functions spanni
+00004970: 6e67 206f 7065 7261 7469 6f6e 7320 7375  ng operations su
+00004980: 6368 2061 7320 696d 6167 6520 6669 6c65  ch as image file
+00004990: 2072 6561 6469 6e67 2061 6e64 0a77 7269   reading and.wri
+000049a0: 7469 6e67 2c20 6163 7175 6973 6974 696f  ting, acquisitio
+000049b0: 6e2c 2064 6973 706c 6179 2c20 6669 6c74  n, display, filt
+000049c0: 6572 696e 672c 2062 6c6f 622c 2070 6f69  ering, blob, poi
+000049d0: 6e74 2061 6e64 206c 696e 6520 6665 6174  nt and line feat
+000049e0: 7572 650a 6578 7472 6163 7469 6f6e 2c20  ure.extraction, 
+000049f0: 6d61 7468 656d 6174 6963 616c 206d 6f72  mathematical mor
+00004a00: 7068 6f6c 6f67 792c 2068 6f6d 6f67 7261  phology, homogra
+00004a10: 7068 6965 732c 2076 6973 7561 6c20 4a61  phies, visual Ja
+00004a20: 636f 6269 616e 732c 2063 616d 6572 610a  cobians, camera.
+00004a30: 6361 6c69 6272 6174 696f 6e20 616e 6420  calibration and 
+00004a40: 636f 6c6f 7220 7370 6163 6520 636f 6e76  color space conv
+00004a50: 6572 7369 6f6e 2e0a 0a54 6869 7320 5079  ersion...This Py
+00004a60: 7468 6f6e 2076 6572 7369 6f6e 2064 6966  thon version dif
+00004a70: 6665 7273 2069 6e20 7573 696e 6720 616e  fers in using an
+00004a80: 206f 626a 6563 7420 746f 2065 6e63 6170   object to encap
+00004a90: 7375 6c61 7465 2074 6865 2070 6978 656c  sulate the pixel
+00004aa0: 2064 6174 6120 616e 640a 696d 6167 6520   data and.image 
+00004ab0: 6d65 7461 6461 7461 2c20 7261 7468 6572  metadata, rather
+00004ac0: 2074 6861 6e20 6a75 7374 2061 206e 6174   than just a nat
+00004ad0: 6976 6520 6f62 6a65 6374 2068 6f6c 6469  ive object holdi
+00004ae0: 6e67 2070 6978 656c 2064 6174 612e 2054  ng pixel data. T
+00004af0: 6865 206d 616e 790a 6675 6e63 7469 6f6e  he many.function
+00004b00: 7320 6265 636f 6d65 206d 6574 686f 6473  s become methods
+00004b10: 206f 6620 7468 6520 696d 6167 6520 6f62   of the image ob
+00004b20: 6a65 6374 2077 6869 6368 2072 6564 7563  ject which reduc
+00004b30: 6573 206e 616d 6573 7061 6365 2070 6f6c  es namespace pol
+00004b40: 6c75 7469 6f6e 732c 0a61 6e64 2061 6c6c  lutions,.and all
+00004b50: 6f77 7320 7468 6520 6561 7379 2065 7870  ows the easy exp
+00004b60: 7265 7373 696f 6e20 6f66 2073 6571 7565  ression of seque
+00004b70: 6e74 6961 6c20 6f70 6572 6174 696f 6e73  ntial operations
+00004b80: 2075 7369 6e67 2022 646f 7420 6368 6169   using "dot chai
+00004b90: 6e69 6e67 222e 0a0a 5468 6520 6669 7273  ning"...The firs
+00004ba0: 7420 7665 7273 696f 6e20 7761 7320 6372  t version was cr
+00004bb0: 6561 7465 6420 6279 2044 6f72 6961 6e20  eated by Dorian 
+00004bc0: 5473 6169 2064 7572 696e 6720 3230 3230  Tsai during 2020
+00004bd0: 2c20 616e 6420 6261 7365 6420 6f6e 2074  , and based on t
+00004be0: 6865 0a4d 4154 4c41 4220 7665 7273 696f  he.MATLAB versio
+00004bf0: 6e2e 2020 5468 6174 2077 6f72 6b20 7761  n.  That work wa
+00004c00: 7320 6675 6e64 6564 2062 7920 616e 2041  s funded by an A
+00004c10: 7573 7472 616c 6961 6e20 556e 6976 6572  ustralian Univer
+00004c20: 7369 7479 2054 6561 6368 6572 206f 660a  sity Teacher of.
+00004c30: 7468 6520 7965 6172 2061 7761 7264 2028  the year award (
+00004c40: 3230 3137 2920 746f 2050 6574 6572 2043  2017) to Peter C
+00004c50: 6f72 6b65 2e0a                           orke..
```

### Comparing `machinevision-toolbox-python-0.9.6/machinevision_toolbox_python.egg-info/SOURCES.txt` & `machinevision_toolbox_python-0.9.7/machinevision_toolbox_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/BagOfWords.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/BagOfWords.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/BundleAdjust.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/BundleAdjust.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/Camera.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/Camera.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageBlobs.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageBlobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,16 +233,18 @@
             ## perimeter, the contour is not closed
 
             blob.perimeter = contour.T
             blob.perimeter_length = cv.arcLength(contour, closed=False)
 
             blob.contourpoint = blob.perimeter[:, 0]
 
-            ## append the new Blob instance
-            self.data.append(blob)
+            ## For a single set pixel OpenCV returns all moments as zero, skip such blobs
+            ## TODO handle this situation by setting m00=1, m10=x, m01=y etc.
+            if blob.moments["m00"] != 0:
+                self.data.append(blob)
 
         ## second pass: equivalent ellipse
 
         for blob, contour in zip(self.data, contours):
 
             ## moment hierarchy
```

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageColor.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageColor.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageConstants.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageConstants.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageCore.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageCore.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageIO.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageIO.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageLineFeatures.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageLineFeatures.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageMorph.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageMorph.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageMultiview.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageMultiview.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImagePointFeatures.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImagePointFeatures.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageProcessing.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageProcessing.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageRegionFeatures.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageRegionFeatures.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageReshape.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageReshape.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageSpatial.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageSpatial.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/ImageWholeFeatures.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/ImageWholeFeatures.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/PointCloud.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/PointCloud.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/Sources.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/Sources.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/VisualServo.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/VisualServo.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/__init__.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/__init__.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/__init__.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/color.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/color.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/data.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/data.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/esttheta.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/esttheta.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/findpeaks.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/findpeaks.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/graphics.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/graphics.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/imageio.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/imageio.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/meshgrid.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/meshgrid.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/shapes.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/shapes.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/base/types.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/base/types.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/blocks/camera.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/blocks/camera.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/blocks/test_blocks.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/blocks/test_blocks.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/camera_derivatives.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/camera_derivatives.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/fiducial.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/fiducial.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/machinevisiontoolbox/newcameras.py` & `machinevision_toolbox_python-0.9.7/machinevisiontoolbox/newcameras.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/pyproject.toml` & `machinevision_toolbox_python-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "machinevision-toolbox-python"
-version = "0.9.6"
+version = "0.9.7"
 authors = [
   { name="Peter Corke", email="rvc@petercorke.com" },
   { name="Dorian Tsai"},
 ]
 description = "Python tools for machine vision - education and research"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -91,8 +91,8 @@
 [tool.black]
 line-length = 88
 target-version = ['py37']
 exclude = "camera_derivatives.py"
 
 [tool.coverage.run]
 omit = [
-]
+]
```

### Comparing `machinevision-toolbox-python-0.9.6/tests/test_base_color.py` & `machinevision_toolbox_python-0.9.7/tests/test_base_color.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/tests/test_camera.py` & `machinevision_toolbox_python-0.9.7/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/tests/test_color.py` & `machinevision_toolbox_python-0.9.7/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/tests/test_core.py` & `machinevision_toolbox_python-0.9.7/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/tests/test_image_io.py` & `machinevision_toolbox_python-0.9.7/tests/test_image_io.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/tests/test_imageprocessing_kernel.py` & `machinevision_toolbox_python-0.9.7/tests/test_imageprocessing_kernel.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/tests/test_imageprocessing_morph.py` & `machinevision_toolbox_python-0.9.7/tests/test_imageprocessing_morph.py`

 * *Files identical despite different names*

### Comparing `machinevision-toolbox-python-0.9.6/tests/test_processing.py` & `machinevision_toolbox_python-0.9.7/tests/test_processing.py`

 * *Files identical despite different names*

