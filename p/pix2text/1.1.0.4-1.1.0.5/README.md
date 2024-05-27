# Comparing `tmp/pix2text-1.1.0.4.tar.gz` & `tmp/pix2text-1.1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix2text-1.1.0.4.tar", last modified: Mon May 20 15:16:50 2024, max compression
+gzip compressed data, was "pix2text-1.1.0.5.tar", last modified: Mon May 27 04:08:12 2024, max compression
```

## Comparing `pix2text-1.1.0.4.tar` & `pix2text-1.1.0.5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-20 15:16:50.685139 pix2text-1.1.0.4/
--rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-1.1.0.4/LICENSE
--rw-r--r--   0 king       (501) staff       (20)    14231 2024-05-20 15:16:50.684970 pix2text-1.1.0.4/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    13012 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-20 15:16:50.674025 pix2text-1.1.0.4/pix2text/
--rw-r--r--   0 king       (501) staff       (20)      456 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      203 2024-05-20 15:15:35.000000 pix2text-1.1.0.4/pix2text/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-1.1.0.4/pix2text/app.py
--rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-1.1.0.4/pix2text/category_mapping.py
--rw-r--r--   0 king       (501) staff       (20)    10451 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/cli.py
--rw-r--r--   0 king       (501) staff       (20)     4158 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-20 15:16:50.676307 pix2text-1.1.0.4/pix2text/doc_xl_layout/
--rw-r--r--   0 king       (501) staff       (20)      192 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/__init__.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-20 15:16:50.677666 pix2text-1.1.0.4/pix2text/doc_xl_layout/detectors/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/detectors/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     8390 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/detectors/base_detector_subfield.py
--rw-r--r--   0 king       (501) staff       (20)     8722 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/detectors/ctdet_subfield.py
--rw-r--r--   0 king       (501) staff       (20)      137 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/detectors/detector_factory.py
--rw-r--r--   0 king       (501) staff       (20)    17964 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/doc_xl_layout_parser.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-20 15:16:50.677994 pix2text-1.1.0.4/pix2text/doc_xl_layout/external/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/external/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     2510 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/external/shapelyNMS.py
--rw-r--r--   0 king       (501) staff       (20)      365 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/huntie_subfield.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-20 15:16:50.679271 pix2text-1.1.0.4/pix2text/doc_xl_layout/models/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/models/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     5178 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/models/data_parallel.py
--rw-r--r--   0 king       (501) staff       (20)    23840 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/models/decode.py
--rw-r--r--   0 king       (501) staff       (20)     3443 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/models/model.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-20 15:16:50.679498 pix2text-1.1.0.4/pix2text/doc_xl_layout/models/networks/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/models/networks/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    24395 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py
--rw-r--r--   0 king       (501) staff       (20)     1528 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/models/scatter_gather.py
--rw-r--r--   0 king       (501) staff       (20)     1800 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/models/utils.py
--rw-r--r--   0 king       (501) staff       (20)    23801 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/opts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-20 15:16:50.681371 pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     4818 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/ddd_utils.py
--rw-r--r--   0 king       (501) staff       (20)    26623 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/debugger.py
--rw-r--r--   0 king       (501) staff       (20)    18383 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/evaluation_bk.py
--rw-r--r--   0 king       (501) staff       (20)     7851 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/image.py
--rw-r--r--   0 king       (501) staff       (20)     5368 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/post_process.py
--rw-r--r--   0 king       (501) staff       (20)      533 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/utils.py
--rw-r--r--   0 king       (501) staff       (20)     8844 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/doc_xl_layout/wrapper.py
--rw-r--r--   0 king       (501) staff       (20)    12517 2024-03-27 09:59:17.000000 pix2text-1.1.0.4/pix2text/element.py
--rw-r--r--   0 king       (501) staff       (20)    17923 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/latex_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    13244 2024-01-11 04:27:38.000000 pix2text-1.1.0.4/pix2text/latex_ocr0.py
--rw-r--r--   0 king       (501) staff       (20)    22526 2024-01-10 13:35:10.000000 pix2text-1.1.0.4/pix2text/latex_recog.py
--rw-r--r--   0 king       (501) staff       (20)     4016 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/layout_parser.py
--rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-1.1.0.4/pix2text/object_detector.py
--rw-r--r--   0 king       (501) staff       (20)     7485 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/ocr_engine.py
--rw-r--r--   0 king       (501) staff       (20)    11361 2024-05-20 15:08:23.000000 pix2text-1.1.0.4/pix2text/page_elements.py
--rw-r--r--   0 king       (501) staff       (20)    28288 2024-05-20 15:08:23.000000 pix2text-1.1.0.4/pix2text/pix_to_text.py
--rw-r--r--   0 king       (501) staff       (20)     5413 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/render.py
--rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-1.1.0.4/pix2text/screenshot_daemon_with_server2.py
--rw-r--r--   0 king       (501) staff       (20)     2776 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/serve.py
--rw-r--r--   0 king       (501) staff       (20)    38505 2024-03-27 14:55:51.000000 pix2text-1.1.0.4/pix2text/table_inference.py
--rw-r--r--   0 king       (501) staff       (20)    38370 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/table_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    37328 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/table_postprocess.py
--rw-r--r--   0 king       (501) staff       (20)    24628 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/text_formula_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    31718 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/pix2text/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-20 15:16:50.675188 pix2text-1.1.0.4/pix2text.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    14231 2024-05-20 15:16:50.000000 pix2text-1.1.0.4/pix2text.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)     2405 2024-05-20 15:16:50.000000 pix2text-1.1.0.4/pix2text.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2024-05-20 15:16:50.000000 pix2text-1.1.0.4/pix2text.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       42 2024-05-20 15:16:50.000000 pix2text-1.1.0.4/pix2text.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-1.1.0.4/pix2text.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      269 2024-05-20 15:16:50.000000 pix2text-1.1.0.4/pix2text.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)       17 2024-05-20 15:16:50.000000 pix2text-1.1.0.4/pix2text.egg-info/top_level.txt
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-20 15:16:50.684253 pix2text-1.1.0.4/scripts/
--rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-1.1.0.4/scripts/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-1.1.0.4/scripts/convert_label_studio_to_yolov7.py
--rw-r--r--   0 king       (501) staff       (20)     6678 2024-01-03 07:40:48.000000 pix2text-1.1.0.4/scripts/extract_p2t_results.py
--rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-1.1.0.4/scripts/gen_label_studio_json.py
--rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-1.1.0.4/scripts/gen_pure_formula_to_yolov7.py
--rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-1.1.0.4/scripts/merge_label_studio_anno_pred_json.py
--rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-1.1.0.4/scripts/object_detection3.py
--rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-1.1.0.4/scripts/screenshot_daemon.py
--rw-r--r--   0 king       (501) staff       (20)      143 2024-01-01 08:28:55.000000 pix2text-1.1.0.4/scripts/try_easyocr.py
--rw-r--r--   0 king       (501) staff       (20)      796 2024-03-13 15:31:39.000000 pix2text-1.1.0.4/scripts/try_latex_correction.py
--rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-1.1.0.4/scripts/try_layout.py
--rw-r--r--   0 king       (501) staff       (20)      861 2024-03-29 15:11:40.000000 pix2text-1.1.0.4/scripts/try_pix2text_mfr.py
--rw-r--r--   0 king       (501) staff       (20)      845 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/scripts/try_service.py
--rw-r--r--   0 king       (501) staff       (20)     1614 2024-01-05 04:02:17.000000 pix2text-1.1.0.4/scripts/try_texify.py
--rw-r--r--   0 king       (501) staff       (20)       38 2024-05-20 15:16:50.685207 pix2text-1.1.0.4/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     2522 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/setup.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-20 15:16:50.684747 pix2text-1.1.0.4/tests/
--rw-r--r--   0 king       (501) staff       (20)     5861 2024-05-20 15:08:06.000000 pix2text-1.1.0.4/tests/test_pix2text.py
--rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-1.1.0.4/tests/test_sort_boxes.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-27 04:08:12.309330 pix2text-1.1.0.5/
+-rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-1.1.0.5/LICENSE
+-rw-r--r--   0 king       (501) staff       (20)    14231 2024-05-27 04:08:12.309110 pix2text-1.1.0.5/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    13012 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-27 04:08:12.297311 pix2text-1.1.0.5/pix2text/
+-rw-r--r--   0 king       (501) staff       (20)      456 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      203 2024-05-27 04:04:33.000000 pix2text-1.1.0.5/pix2text/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-1.1.0.5/pix2text/app.py
+-rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-1.1.0.5/pix2text/category_mapping.py
+-rw-r--r--   0 king       (501) staff       (20)    10451 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/cli.py
+-rw-r--r--   0 king       (501) staff       (20)     4365 2024-05-27 04:01:44.000000 pix2text-1.1.0.5/pix2text/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-27 04:08:12.299775 pix2text-1.1.0.5/pix2text/doc_xl_layout/
+-rw-r--r--   0 king       (501) staff       (20)      192 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/__init__.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-27 04:08:12.300753 pix2text-1.1.0.5/pix2text/doc_xl_layout/detectors/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/detectors/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     8390 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/detectors/base_detector_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)     8722 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/detectors/ctdet_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)      137 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/detectors/detector_factory.py
+-rw-r--r--   0 king       (501) staff       (20)    17977 2024-05-24 15:23:18.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/doc_xl_layout_parser.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-27 04:08:12.301059 pix2text-1.1.0.5/pix2text/doc_xl_layout/external/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/external/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     2510 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/external/shapelyNMS.py
+-rw-r--r--   0 king       (501) staff       (20)      365 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/huntie_subfield.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-27 04:08:12.302363 pix2text-1.1.0.5/pix2text/doc_xl_layout/models/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/models/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     5178 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/models/data_parallel.py
+-rw-r--r--   0 king       (501) staff       (20)    23840 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/models/decode.py
+-rw-r--r--   0 king       (501) staff       (20)     3443 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/models/model.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-27 04:08:12.302617 pix2text-1.1.0.5/pix2text/doc_xl_layout/models/networks/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/models/networks/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    24395 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)     1528 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/models/scatter_gather.py
+-rw-r--r--   0 king       (501) staff       (20)     1800 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/models/utils.py
+-rw-r--r--   0 king       (501) staff       (20)    23801 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/opts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-27 04:08:12.304817 pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     4818 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/ddd_utils.py
+-rw-r--r--   0 king       (501) staff       (20)    26623 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/debugger.py
+-rw-r--r--   0 king       (501) staff       (20)    18383 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/evaluation_bk.py
+-rw-r--r--   0 king       (501) staff       (20)     7851 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/image.py
+-rw-r--r--   0 king       (501) staff       (20)     5368 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/post_process.py
+-rw-r--r--   0 king       (501) staff       (20)      533 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/utils.py
+-rw-r--r--   0 king       (501) staff       (20)     8844 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/doc_xl_layout/wrapper.py
+-rw-r--r--   0 king       (501) staff       (20)    12517 2024-03-27 09:59:17.000000 pix2text-1.1.0.5/pix2text/element.py
+-rw-r--r--   0 king       (501) staff       (20)    17923 2024-05-23 14:44:20.000000 pix2text-1.1.0.5/pix2text/latex_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    13244 2024-01-11 04:27:38.000000 pix2text-1.1.0.5/pix2text/latex_ocr0.py
+-rw-r--r--   0 king       (501) staff       (20)    22526 2024-01-10 13:35:10.000000 pix2text-1.1.0.5/pix2text/latex_recog.py
+-rw-r--r--   0 king       (501) staff       (20)     4016 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/layout_parser.py
+-rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-1.1.0.5/pix2text/object_detector.py
+-rw-r--r--   0 king       (501) staff       (20)     7485 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/ocr_engine.py
+-rw-r--r--   0 king       (501) staff       (20)    11361 2024-05-20 15:08:23.000000 pix2text-1.1.0.5/pix2text/page_elements.py
+-rw-r--r--   0 king       (501) staff       (20)    28389 2024-05-27 03:57:25.000000 pix2text-1.1.0.5/pix2text/pix_to_text.py
+-rw-r--r--   0 king       (501) staff       (20)     5413 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/render.py
+-rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-1.1.0.5/pix2text/screenshot_daemon_with_server2.py
+-rw-r--r--   0 king       (501) staff       (20)     2776 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/serve.py
+-rw-r--r--   0 king       (501) staff       (20)    38505 2024-03-27 14:55:51.000000 pix2text-1.1.0.5/pix2text/table_inference.py
+-rw-r--r--   0 king       (501) staff       (20)    38370 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/table_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    37328 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/table_postprocess.py
+-rw-r--r--   0 king       (501) staff       (20)    24628 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/text_formula_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    31718 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/pix2text/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-27 04:08:12.298472 pix2text-1.1.0.5/pix2text.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    14231 2024-05-27 04:08:12.000000 pix2text-1.1.0.5/pix2text.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)     2405 2024-05-27 04:08:12.000000 pix2text-1.1.0.5/pix2text.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2024-05-27 04:08:12.000000 pix2text-1.1.0.5/pix2text.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       42 2024-05-27 04:08:12.000000 pix2text-1.1.0.5/pix2text.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-1.1.0.5/pix2text.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      269 2024-05-27 04:08:12.000000 pix2text-1.1.0.5/pix2text.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)       17 2024-05-27 04:08:12.000000 pix2text-1.1.0.5/pix2text.egg-info/top_level.txt
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-27 04:08:12.308131 pix2text-1.1.0.5/scripts/
+-rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-1.1.0.5/scripts/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-1.1.0.5/scripts/convert_label_studio_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     6678 2024-01-03 07:40:48.000000 pix2text-1.1.0.5/scripts/extract_p2t_results.py
+-rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-1.1.0.5/scripts/gen_label_studio_json.py
+-rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-1.1.0.5/scripts/gen_pure_formula_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-1.1.0.5/scripts/merge_label_studio_anno_pred_json.py
+-rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-1.1.0.5/scripts/object_detection3.py
+-rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-1.1.0.5/scripts/screenshot_daemon.py
+-rw-r--r--   0 king       (501) staff       (20)      143 2024-01-01 08:28:55.000000 pix2text-1.1.0.5/scripts/try_easyocr.py
+-rw-r--r--   0 king       (501) staff       (20)      796 2024-03-13 15:31:39.000000 pix2text-1.1.0.5/scripts/try_latex_correction.py
+-rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-1.1.0.5/scripts/try_layout.py
+-rw-r--r--   0 king       (501) staff       (20)      861 2024-03-29 15:11:40.000000 pix2text-1.1.0.5/scripts/try_pix2text_mfr.py
+-rw-r--r--   0 king       (501) staff       (20)      845 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/scripts/try_service.py
+-rw-r--r--   0 king       (501) staff       (20)     1614 2024-01-05 04:02:17.000000 pix2text-1.1.0.5/scripts/try_texify.py
+-rw-r--r--   0 king       (501) staff       (20)       38 2024-05-27 04:08:12.309397 pix2text-1.1.0.5/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     2522 2024-05-20 15:08:06.000000 pix2text-1.1.0.5/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-27 04:08:12.308849 pix2text-1.1.0.5/tests/
+-rw-r--r--   0 king       (501) staff       (20)     6006 2024-05-23 14:20:18.000000 pix2text-1.1.0.5/tests/test_pix2text.py
+-rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-1.1.0.5/tests/test_sort_boxes.py
```

### Comparing `pix2text-1.1.0.4/LICENSE` & `pix2text-1.1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/PKG-INFO` & `pix2text-1.1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix2text
-Version: 1.1.0.4
+Version: 1.1.0.5
 Summary: An Open-Source Python3 tool for recognizing layouts, tables, math formulas, and text in images, converting them into Markdown format. A free alternative to Mathpix, empowering seamless conversion of visual content into text-based representations.
 Home-page: https://github.com/breezedeus/pix2text
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: MIT
 Platform: Mac
 Platform: Linux
```

### Comparing `pix2text-1.1.0.4/README.md` & `pix2text-1.1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/app.py` & `pix2text-1.1.0.5/pix2text/app.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/category_mapping.py` & `pix2text-1.1.0.5/pix2text/category_mapping.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/cli.py` & `pix2text-1.1.0.5/pix2text/cli.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/consts.py` & `pix2text-1.1.0.5/pix2text/consts.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,32 +40,35 @@
         }
     )
 
     PAID_MODELS = OrderedDict(
         {
             ('mfr', 'pytorch'): {
                 'filename': 'p2t-mfr-pytorch.zip',  # download the file from CN OSS
+                'hf_model_id': 'breezedeus/pix2text-mfr-pytorch',
                 'local_model_id': 'mfr-pytorch',
             },
             ('mfr-pro', 'onnx'): {
                 'filename': 'p2t-mfr-pro-onnx.zip',  # download the file from CN OSS
                 'hf_model_id': 'breezedeus/pix2text-mfr-pro',
                 'local_model_id': 'mfr-pro-onnx',
             },
             ('mfr-pro', 'pytorch'): {
                 'filename': 'p2t-mfr-pro-pytorch.zip',  # download the file from CN OSS
+                'hf_model_id': 'breezedeus/pix2text-mfr-pro-pytorch',
                 'local_model_id': 'mfr-pro-pytorch',
             },
             ('mfr-plus', 'onnx'): {
                 'filename': 'p2t-mfr-plus-onnx.zip',  # download the file from CN OSS
                 'hf_model_id': 'breezedeus/pix2text-mfr-plus',
                 'local_model_id': 'mfr-plus-onnx',
             },
             ('mfr-plus', 'pytorch'): {
                 'filename': 'p2t-mfr-plus-pytorch.zip',  # download the file from CN OSS
+                'hf_model_id': 'breezedeus/pix2text-mfr-plus-pytorch',
                 'local_model_id': 'mfr-plus-pytorch',
             },
         }
     )
 
     P2T_MODELS = deepcopy(FREE_MODELS)
     P2T_MODELS.update(PAID_MODELS)
```

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/detectors/base_detector_subfield.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/detectors/base_detector_subfield.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/detectors/ctdet_subfield.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/detectors/ctdet_subfield.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/doc_xl_layout_parser.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/doc_xl_layout_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             device=device,
             model_fp=configs.get('model_fp', None),
             root=configs.get('root', data_dir()),
             **configs,
         )
 
     def _prepare_model_files(self, root, model_info):
-        model_root_dir = Path(root) / MODEL_VERSION
+        model_root_dir = Path(root).expanduser() / MODEL_VERSION
         model_dir = model_root_dir / 'layout-parser'
         model_fp = model_dir / 'DocXLayout_231012.pth'
         if model_fp.exists():
             return model_fp
         if model_dir.exists():
             shutil.rmtree(str(model_dir))
         model_dir.mkdir(parents=True)
```

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/external/shapelyNMS.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/external/shapelyNMS.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/models/data_parallel.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/models/data_parallel.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/models/decode.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/models/decode.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/models/model.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/models/model.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/models/scatter_gather.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/models/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/models/utils.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/models/utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/opts.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/opts.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/ddd_utils.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/ddd_utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/debugger.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/debugger.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/evaluation_bk.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/evaluation_bk.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/image.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/image.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/post_process.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/post_process.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/utils/utils.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/doc_xl_layout/wrapper.py` & `pix2text-1.1.0.5/pix2text/doc_xl_layout/wrapper.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/element.py` & `pix2text-1.1.0.5/pix2text/element.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/latex_ocr.py` & `pix2text-1.1.0.5/pix2text/latex_ocr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/latex_ocr0.py` & `pix2text-1.1.0.5/pix2text/latex_ocr0.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/latex_recog.py` & `pix2text-1.1.0.5/pix2text/latex_recog.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/layout_parser.py` & `pix2text-1.1.0.5/pix2text/layout_parser.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/object_detector.py` & `pix2text-1.1.0.5/pix2text/object_detector.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/ocr_engine.py` & `pix2text-1.1.0.5/pix2text/ocr_engine.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/page_elements.py` & `pix2text-1.1.0.5/pix2text/page_elements.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/pix_to_text.py` & `pix2text-1.1.0.5/pix2text/pix_to_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,16 +402,19 @@
         _out = [_o for _o in _out if len(_o['text']) >= min_text_length]
         # guess which column the box belongs to
         for _box_info in _out:
             overlap_vals = []
             for col_number, col_info in column_meta.items():
                 overlap_val = x_overlap(_box_info, col_info, key='position')
                 overlap_vals.append([col_number, overlap_val])
-            overlap_vals.sort(key=lambda x: (x[1], x[0]), reverse=True)
-            match_col_number = overlap_vals[0][0]
+            if len(overlap_vals) > 0:
+                overlap_vals.sort(key=lambda x: (x[1], x[0]), reverse=True)
+                match_col_number = overlap_vals[0][0]
+            else:
+                match_col_number = 0
             _box_info['col_number'] = match_col_number
 
         if len(_out) < 2:
             return _out
 
         def _compare(box_info1, box_info2):
             if box_info1['col_number'] != box_info2['col_number']:
```

### Comparing `pix2text-1.1.0.4/pix2text/render.py` & `pix2text-1.1.0.5/pix2text/render.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/screenshot_daemon_with_server2.py` & `pix2text-1.1.0.5/pix2text/screenshot_daemon_with_server2.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/serve.py` & `pix2text-1.1.0.5/pix2text/serve.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/table_inference.py` & `pix2text-1.1.0.5/pix2text/table_inference.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/table_ocr.py` & `pix2text-1.1.0.5/pix2text/table_ocr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/table_postprocess.py` & `pix2text-1.1.0.5/pix2text/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/text_formula_ocr.py` & `pix2text-1.1.0.5/pix2text/text_formula_ocr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text/utils.py` & `pix2text-1.1.0.5/pix2text/utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/pix2text.egg-info/PKG-INFO` & `pix2text-1.1.0.5/pix2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix2text
-Version: 1.1.0.4
+Version: 1.1.0.5
 Summary: An Open-Source Python3 tool for recognizing layouts, tables, math formulas, and text in images, converting them into Markdown format. A free alternative to Mathpix, empowering seamless conversion of visual content into text-based representations.
 Home-page: https://github.com/breezedeus/pix2text
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: MIT
 Platform: Mac
 Platform: Linux
```

### Comparing `pix2text-1.1.0.4/pix2text.egg-info/SOURCES.txt` & `pix2text-1.1.0.5/pix2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/scripts/convert_label_studio_to_yolov7.py` & `pix2text-1.1.0.5/scripts/convert_label_studio_to_yolov7.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/scripts/extract_p2t_results.py` & `pix2text-1.1.0.5/scripts/extract_p2t_results.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/scripts/gen_label_studio_json.py` & `pix2text-1.1.0.5/scripts/gen_label_studio_json.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/scripts/gen_pure_formula_to_yolov7.py` & `pix2text-1.1.0.5/scripts/gen_pure_formula_to_yolov7.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/scripts/merge_label_studio_anno_pred_json.py` & `pix2text-1.1.0.5/scripts/merge_label_studio_anno_pred_json.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/scripts/object_detection3.py` & `pix2text-1.1.0.5/scripts/object_detection3.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/scripts/screenshot_daemon.py` & `pix2text-1.1.0.5/scripts/screenshot_daemon.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/scripts/try_latex_correction.py` & `pix2text-1.1.0.5/scripts/try_latex_correction.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/scripts/try_layout.py` & `pix2text-1.1.0.5/scripts/try_layout.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/scripts/try_pix2text_mfr.py` & `pix2text-1.1.0.5/scripts/try_pix2text_mfr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/scripts/try_service.py` & `pix2text-1.1.0.5/scripts/try_service.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/scripts/try_texify.py` & `pix2text-1.1.0.5/scripts/try_texify.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/setup.py` & `pix2text-1.1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.4/tests/test_pix2text.py` & `pix2text-1.1.0.5/tests/test_pix2text.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,21 @@
 
 def test_recognize_page():
     # img_fp = './docs/examples/formula.jpg'
     img_fp = './docs/examples/page3.png'
     # img_fp = './docs/examples/mixed.jpg'
     total_config = {
         'layout': {'scores_thresh': 0.45},
-        'text_formula': {'formula': {'model_name': 'mfr-pro', 'model_backend': 'onnx'}},
+        'text_formula': {
+            'formula': {
+                'model_name': 'mfr-pro',
+                'model_backend': 'onnx',
+                'more_model_configs': {'provider': 'CPUExecutionProvider'},
+            }
+        },
     }
     p2t = Pix2Text.from_config(total_configs=total_config)
     out_page = p2t.recognize_page(
         img_fp,
         page_id='test_page_1',
         title_contain_formula=False,
         text_contain_formula=False,
```

### Comparing `pix2text-1.1.0.4/tests/test_sort_boxes.py` & `pix2text-1.1.0.5/tests/test_sort_boxes.py`

 * *Files identical despite different names*

