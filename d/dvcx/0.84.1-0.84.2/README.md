# Comparing `tmp/dvcx-0.84.1.tar.gz` & `tmp/dvcx-0.84.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.84.1.tar", last modified: Fri May 24 08:04:35 2024, max compression
+gzip compressed data, was "dvcx-0.84.2.tar", last modified: Mon May 27 07:29:32 2024, max compression
```

## Comparing `dvcx-0.84.1.tar` & `dvcx-0.84.2.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.131399 dvcx-0.84.1/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-24 08:04:25.000000 dvcx-0.84.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 08:04:25.000000 dvcx-0.84.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.079399 dvcx-0.84.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.079399 dvcx-0.84.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-24 08:04:25.000000 dvcx-0.84.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-24 08:04:25.000000 dvcx-0.84.1/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-24 08:04:25.000000 dvcx-0.84.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-24 08:04:25.000000 dvcx-0.84.1/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-24 08:04:25.000000 dvcx-0.84.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.079399 dvcx-0.84.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-24 08:04:25.000000 dvcx-0.84.1/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-24 08:04:25.000000 dvcx-0.84.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-24 08:04:25.000000 dvcx-0.84.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-24 08:04:25.000000 dvcx-0.84.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-24 08:04:25.000000 dvcx-0.84.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-24 08:04:25.000000 dvcx-0.84.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.079399 dvcx-0.84.1/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-24 08:04:25.000000 dvcx-0.84.1/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-24 08:04:25.000000 dvcx-0.84.1/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-24 08:04:25.000000 dvcx-0.84.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-24 08:04:25.000000 dvcx-0.84.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-24 08:04:25.000000 dvcx-0.84.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.079399 dvcx-0.84.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-24 08:04:25.000000 dvcx-0.84.1/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-24 08:04:25.000000 dvcx-0.84.1/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-24 08:04:25.000000 dvcx-0.84.1/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-24 08:04:35.131399 dvcx-0.84.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-24 08:04:25.000000 dvcx-0.84.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.079399 dvcx-0.84.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-24 08:04:25.000000 dvcx-0.84.1/docs/cv_intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-24 08:04:25.000000 dvcx-0.84.1/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.087399 dvcx-0.84.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/llm-claude-aggregate-query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/llm-claude-simple-query.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/llm-claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.087399 dvcx-0.84.1/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.087399 dvcx-0.84.1/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.091399 dvcx-0.84.1/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-24 08:04:25.000000 dvcx-0.84.1/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-24 08:04:25.000000 dvcx-0.84.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-24 08:04:25.000000 dvcx-0.84.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 08:04:35.131399 dvcx-0.84.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.071399 dvcx-0.84.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.091399 dvcx-0.84.1/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-24 08:04:34.000000 dvcx-0.84.1/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.095399 dvcx-0.84.1/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72836 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.095399 dvcx-0.84.1/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.099399 dvcx-0.84.1/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46749 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24923 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    31666 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    16707 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.103399 dvcx-0.84.1/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/feature_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/vfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.107399 dvcx-0.84.1/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    61693 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/query/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.107399 dvcx-0.84.1/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.107399 dvcx-0.84.1/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.107399 dvcx-0.84.1/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.107399 dvcx-0.84.1/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.111399 dvcx-0.84.1/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-24 08:04:25.000000 dvcx-0.84.1/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.123399 dvcx-0.84.1/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-24 08:04:35.000000 dvcx-0.84.1/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-24 08:04:35.000000 dvcx-0.84.1/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:04:35.000000 dvcx-0.84.1/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 08:04:35.000000 dvcx-0.84.1/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-24 08:04:35.000000 dvcx-0.84.1/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 08:04:35.000000 dvcx-0.84.1/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.111399 dvcx-0.84.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.111399 dvcx-0.84.1/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16386 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.115399 dvcx-0.84.1/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35078 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   112860 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    29484 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/func/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.115399 dvcx-0.84.1/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/scripts/name_len_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/scripts/name_len_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/test_cli_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/test_query_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.119399 dvcx-0.84.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.123399 dvcx-0.84.1/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/lib/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/lib/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/lib/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.123399 dvcx-0.84.1/tests/unit/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:35.123399 dvcx-0.84.1/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_dataset_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-24 08:04:25.000000 dvcx-0.84.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.649377 dvcx-0.84.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-27 07:29:26.000000 dvcx-0.84.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 07:29:26.000000 dvcx-0.84.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.601377 dvcx-0.84.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.601377 dvcx-0.84.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-27 07:29:26.000000 dvcx-0.84.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-27 07:29:26.000000 dvcx-0.84.2/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-27 07:29:26.000000 dvcx-0.84.2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-27 07:29:26.000000 dvcx-0.84.2/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-27 07:29:26.000000 dvcx-0.84.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.601377 dvcx-0.84.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-27 07:29:26.000000 dvcx-0.84.2/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-27 07:29:26.000000 dvcx-0.84.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-27 07:29:26.000000 dvcx-0.84.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-27 07:29:26.000000 dvcx-0.84.2/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-27 07:29:26.000000 dvcx-0.84.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-27 07:29:26.000000 dvcx-0.84.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.601377 dvcx-0.84.2/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-27 07:29:26.000000 dvcx-0.84.2/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-27 07:29:26.000000 dvcx-0.84.2/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-27 07:29:26.000000 dvcx-0.84.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-27 07:29:26.000000 dvcx-0.84.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-27 07:29:26.000000 dvcx-0.84.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.605377 dvcx-0.84.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-27 07:29:26.000000 dvcx-0.84.2/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-27 07:29:26.000000 dvcx-0.84.2/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-27 07:29:26.000000 dvcx-0.84.2/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-27 07:29:32.649377 dvcx-0.84.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-27 07:29:26.000000 dvcx-0.84.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.605377 dvcx-0.84.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-27 07:29:26.000000 dvcx-0.84.2/docs/cv_intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-27 07:29:26.000000 dvcx-0.84.2/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.609377 dvcx-0.84.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.609377 dvcx-0.84.2/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.609377 dvcx-0.84.2/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.609377 dvcx-0.84.2/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 07:29:26.000000 dvcx-0.84.2/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-27 07:29:26.000000 dvcx-0.84.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-27 07:29:26.000000 dvcx-0.84.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 07:29:32.649377 dvcx-0.84.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.597376 dvcx-0.84.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.613376 dvcx-0.84.2/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-27 07:29:32.000000 dvcx-0.84.2/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.613376 dvcx-0.84.2/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73718 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.617377 dvcx-0.84.2/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.617377 dvcx-0.84.2/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46749 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24923 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31666 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16707 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.621377 dvcx-0.84.2/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/vfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.625377 dvcx-0.84.2/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61693 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13071 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7507 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.625377 dvcx-0.84.2/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.625377 dvcx-0.84.2/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.625377 dvcx-0.84.2/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.629377 dvcx-0.84.2/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.629377 dvcx-0.84.2/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-27 07:29:26.000000 dvcx-0.84.2/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.641377 dvcx-0.84.2/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-27 07:29:32.000000 dvcx-0.84.2/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-27 07:29:32.000000 dvcx-0.84.2/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:29:32.000000 dvcx-0.84.2/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 07:29:32.000000 dvcx-0.84.2/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-27 07:29:32.000000 dvcx-0.84.2/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-27 07:29:32.000000 dvcx-0.84.2/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.629377 dvcx-0.84.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.629377 dvcx-0.84.2/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16386 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.633377 dvcx-0.84.2/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35240 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112860 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29484 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.633377 dvcx-0.84.2/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.637377 dvcx-0.84.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.641377 dvcx-0.84.2/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/lib/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/lib/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/lib/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.641377 dvcx-0.84.2/tests/unit/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:32.641377 dvcx-0.84.2/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_dataset_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-27 07:29:26.000000 dvcx-0.84.2/tests/utils.py
```

### Comparing `dvcx-0.84.1/.cruft.json` & `dvcx-0.84.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/.github/workflows/benchmarks.yml` & `dvcx-0.84.2/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/.github/workflows/release.yml` & `dvcx-0.84.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/.github/workflows/tests.yml` & `dvcx-0.84.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/.gitignore` & `dvcx-0.84.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/.pre-commit-config.yaml` & `dvcx-0.84.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/CODE_OF_CONDUCT.rst` & `dvcx-0.84.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/CONTRIBUTING.rst` & `dvcx-0.84.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/LICENSE` & `dvcx-0.84.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/LICENSES/Apache-2.0.txt` & `dvcx-0.84.2/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/LICENSES/BSD-3-Clause.txt` & `dvcx-0.84.2/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/LICENSES/Python-2.0.txt` & `dvcx-0.84.2/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/PKG-INFO` & `dvcx-0.84.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.84.1
+Version: 0.84.2
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.84.1/README.rst` & `dvcx-0.84.2/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/docs/cv_intro.md` & `dvcx-0.84.2/docs/cv_intro.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/docs/udfs.md` & `dvcx-0.84.2/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/blip2_image_desc_lib.py` & `dvcx-0.84.2/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/clip.py` & `dvcx-0.84.2/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/common_sql_functions.py` & `dvcx-0.84.2/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/dir_expansion.py` & `dvcx-0.84.2/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/hf_pipeline.py` & `dvcx-0.84.2/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/llava2_image_desc_lib.py` & `dvcx-0.84.2/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/llm-claude-aggregate-query.py` & `dvcx-0.84.2/examples/llm-claude-aggregate-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/llm-claude-simple-query.py` & `dvcx-0.84.2/examples/llm-claude-simple-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/llm-claude.py` & `dvcx-0.84.2/examples/llm-claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/loader.py` & `dvcx-0.84.2/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/neurips/README` & `dvcx-0.84.2/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/neurips/distance_to_query.py` & `dvcx-0.84.2/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/neurips/llm_chat.py` & `dvcx-0.84.2/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/neurips/single_query.py` & `dvcx-0.84.2/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/neurips/text_loaders.py` & `dvcx-0.84.2/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/openai_image_desc_lib.py` & `dvcx-0.84.2/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/openimage-detect.py` & `dvcx-0.84.2/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/pose_detection.py` & `dvcx-0.84.2/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/torch-loader.py` & `dvcx-0.84.2/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/udfs/batching.py` & `dvcx-0.84.2/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/udfs/image_transformation.py` & `dvcx-0.84.2/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/udfs/parallel.py` & `dvcx-0.84.2/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/udfs/simple.py` & `dvcx-0.84.2/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/udfs/stateful.py` & `dvcx-0.84.2/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/udfs/stateful_similarity.py` & `dvcx-0.84.2/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/unstructured-text.py` & `dvcx-0.84.2/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/wds.py` & `dvcx-0.84.2/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/wds_filtered.py` & `dvcx-0.84.2/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/wds_meta.py` & `dvcx-0.84.2/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/zalando/zalando_clip.py` & `dvcx-0.84.2/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.84.2/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/noxfile.py` & `dvcx-0.84.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/pyproject.toml` & `dvcx-0.84.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/asyn.py` & `dvcx-0.84.2/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/cache.py` & `dvcx-0.84.2/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/catalog/catalog.py` & `dvcx-0.84.2/src/dvcx/catalog/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     QueryScriptRunError,
 )
 from dvcx.listing import Listing
 from dvcx.node import DirType, Node, NodeWithPath
 from dvcx.nodes_thread_pool import NodesThreadPool
 from dvcx.remote.studio import StudioClient
 from dvcx.sql.types import DateTime, SQLType, String
-from dvcx.storage import Status, Storage, StorageStats, StorageURI
+from dvcx.storage import Status, Storage, StorageURI
 from dvcx.utils import (
     DVCXDir,
     batched,
     dvcx_paths_join,
     import_object,
     parse_params_string,
 )
@@ -726,14 +726,20 @@
             logger.debug(
                 "Using cached listing %s. Valid till: %s",
                 storage.uri,
                 storage.expires_to_local,
             )
             # Listing has to have correct version of data storage
             # initialized with correct Storage
+
+            self.update_dataset_version_with_warehouse_info(
+                dataset,
+                dataset.latest_version,
+            )
+
             return lst, path
 
         source_metastore.init_partial_id(client.uri)
         partial_id = source_metastore.get_next_partial_id(client.uri)
 
         source_metastore.init(client.uri, partial_id)
         source_metastore = self.metastore.clone(uri=client.uri, partial_id=partial_id)
@@ -751,14 +757,20 @@
                 storage.uri,
                 Status.PARTIAL if prefix else Status.COMPLETE,
                 ttl,
                 prefix=prefix,
                 partial_id=partial_id,
                 dataset=dataset,
             )
+
+            self.update_dataset_version_with_warehouse_info(
+                dataset,
+                dataset.latest_version,
+            )
+
         except ClientError as e:
             # for handling cloud errors
             error_message = INDEX_INTERNAL_ERROR_MESSAGE
             if e.error_code in ["InvalidAccessKeyId", "SignatureDoesNotMatch"]:
                 error_message = "Invalid cloud credentials"
 
             source_metastore.mark_storage_indexed(
@@ -766,31 +778,48 @@
                 Status.FAILED,
                 ttl,
                 prefix=prefix,
                 error_message=error_message,
                 error_stack=traceback.format_exc(),
                 dataset=dataset,
             )
+            self._remove_dataset_rows_and_warehouse_info(
+                dataset, dataset.latest_version
+            )
             raise
         except:
             source_metastore.mark_storage_indexed(
                 storage.uri,
                 Status.FAILED,
                 ttl,
                 prefix=prefix,
                 error_message=INDEX_INTERNAL_ERROR_MESSAGE,
                 error_stack=traceback.format_exc(),
                 dataset=dataset,
             )
+            self._remove_dataset_rows_and_warehouse_info(
+                dataset, dataset.latest_version
+            )
             raise
 
         lst.storage = storage
 
         return lst, path
 
+    def _remove_dataset_rows_and_warehouse_info(
+        self, dataset: DatasetRecord, version: int, **kwargs
+    ):
+        self.warehouse.drop_dataset_rows_table(dataset, version)
+        self.update_dataset_version_with_warehouse_info(
+            dataset,
+            version,
+            rows_dropped=True,
+            **kwargs,
+        )
+
     def enlist_sources(
         self,
         sources: list[str],
         ttl: int,
         update: bool,
         skip_indexing=False,
         client_config=None,
@@ -937,32 +966,24 @@
                 node_groups.append(NodeGroup(listing, dsrc, source_path))
 
         return node_groups
 
     def unlist_source(self, uri: StorageURI) -> None:
         self.metastore.clone(uri=uri).mark_storage_not_indexed(uri)
 
-    def storage_stats(self, uri: StorageURI) -> Optional[StorageStats]:
+    def storage_stats(self, uri: StorageURI) -> Optional[DatasetStats]:
         """
         Returns tuple with storage stats: total number of rows and total dataset size.
         """
         partial_path = self.metastore.get_last_partial_path(uri)
         if partial_path is None:
             return None
         dataset = self.get_dataset(Storage.dataset_name(uri, partial_path))
-        num_objects, size = self.warehouse.dataset_stats(
-            dataset, dataset.latest_version
-        )
-        assert num_objects is not None
-        assert size is not None
 
-        return StorageStats(
-            num_objects=num_objects,
-            size=size,
-        )
+        return self.dataset_stats(dataset.name, dataset.latest_version)
 
     def create_dataset(
         self,
         name: str,
         version: Optional[int] = None,
         query_script: str = "",
         create_rows: Optional[bool] = True,
@@ -1060,20 +1081,31 @@
             )
 
             self.update_dataset_version_with_warehouse_info(dataset, version)
 
         return dataset
 
     def update_dataset_version_with_warehouse_info(
-        self, dataset: DatasetRecord, version: int, **kwargs
+        self, dataset: DatasetRecord, version: int, rows_dropped=False, **kwargs
     ) -> None:
         dataset_version = dataset.get_version(version)
 
         values = {**kwargs}
 
+        if rows_dropped:
+            values["num_objects"] = None
+            values["size"] = None
+            values["preview"] = None
+            self.metastore.update_dataset_version(
+                dataset,
+                version,
+                **values,
+            )
+            return
+
         if not dataset_version.num_objects:
             num_objects, size = self.warehouse.dataset_stats(dataset, version)
             if num_objects != dataset_version.num_objects:
                 values["num_objects"] = num_objects
             if size != dataset_version.size:
                 values["size"] = size
 
@@ -1190,16 +1222,15 @@
                 self.metastore.update_dataset_status(
                     ds,
                     DatasetStatus.FAILED,
                     version=ds.latest_version,
                     error_message=DATASET_INTERNAL_ERROR_MESSAGE,
                     error_stack=traceback.format_exc(),
                 )
-                self.warehouse.drop_dataset_rows_table(ds, ds.latest_version)
-                self.update_dataset_version_with_warehouse_info(
+                self._remove_dataset_rows_and_warehouse_info(
                     ds,
                     ds.latest_version,
                     sources="\n".join(sources),
                 )
                 raise
             except DatasetNotFoundError:
                 raise e from None
```

### Comparing `dvcx-0.84.1/src/dvcx/catalog/datasource.py` & `dvcx-0.84.2/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/catalog/loader.py` & `dvcx-0.84.2/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/cli.py` & `dvcx-0.84.2/src/dvcx/cli.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/cli_utils.py` & `dvcx-0.84.2/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/client/azure.py` & `dvcx-0.84.2/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/client/fileslice.py` & `dvcx-0.84.2/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/client/fsspec.py` & `dvcx-0.84.2/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/client/gcs.py` & `dvcx-0.84.2/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/client/local.py` & `dvcx-0.84.2/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/client/s3.py` & `dvcx-0.84.2/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/config.py` & `dvcx-0.84.2/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/data_storage/db_engine.py` & `dvcx-0.84.2/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/data_storage/id_generator.py` & `dvcx-0.84.2/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/data_storage/metastore.py` & `dvcx-0.84.2/src/dvcx/data_storage/metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/data_storage/schema.py` & `dvcx-0.84.2/src/dvcx/data_storage/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/data_storage/serializer.py` & `dvcx-0.84.2/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/data_storage/sqlite.py` & `dvcx-0.84.2/src/dvcx/data_storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/data_storage/warehouse.py` & `dvcx-0.84.2/src/dvcx/data_storage/warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/dataset.py` & `dvcx-0.84.2/src/dvcx/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/error.py` & `dvcx-0.84.2/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/cached_stream.py` & `dvcx-0.84.2/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/claude.py` & `dvcx-0.84.2/src/dvcx/lib/claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/dataset.py` & `dvcx-0.84.2/src/dvcx/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/feature.py` & `dvcx-0.84.2/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/feature_types.py` & `dvcx-0.84.2/src/dvcx/lib/feature_types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/feature_udf.py` & `dvcx-0.84.2/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/file.py` & `dvcx-0.84.2/src/dvcx/lib/file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.84.2/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.84.2/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.84.2/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/image.py` & `dvcx-0.84.2/src/dvcx/lib/image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/image_transform.py` & `dvcx-0.84.2/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.84.2/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/pytorch.py` & `dvcx-0.84.2/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/reader.py` & `dvcx-0.84.2/src/dvcx/lib/reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/text.py` & `dvcx-0.84.2/src/dvcx/lib/text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/udf.py` & `dvcx-0.84.2/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/unstructured.py` & `dvcx-0.84.2/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/utils.py` & `dvcx-0.84.2/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/webdataset.py` & `dvcx-0.84.2/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.84.2/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.84.2/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/listing.py` & `dvcx-0.84.2/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/node.py` & `dvcx-0.84.2/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/nodes_fetcher.py` & `dvcx-0.84.2/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/nodes_thread_pool.py` & `dvcx-0.84.2/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/progress.py` & `dvcx-0.84.2/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/query/batch.py` & `dvcx-0.84.2/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/query/builtins.py` & `dvcx-0.84.2/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/query/dataset.py` & `dvcx-0.84.2/src/dvcx/query/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/query/dispatch.py` & `dvcx-0.84.2/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/query/params.py` & `dvcx-0.84.2/src/dvcx/query/params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/query/schema.py` & `dvcx-0.84.2/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/query/session.py` & `dvcx-0.84.2/src/dvcx/query/session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/query/udf.py` & `dvcx-0.84.2/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/remote/studio.py` & `dvcx-0.84.2/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/sql/default/base.py` & `dvcx-0.84.2/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/sql/functions/array.py` & `dvcx-0.84.2/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/sql/functions/path.py` & `dvcx-0.84.2/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/sql/selectable.py` & `dvcx-0.84.2/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/sql/sqlite/base.py` & `dvcx-0.84.2/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/sql/sqlite/types.py` & `dvcx-0.84.2/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/sql/types.py` & `dvcx-0.84.2/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/sql/utils.py` & `dvcx-0.84.2/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx/storage.py` & `dvcx-0.84.2/src/dvcx/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import posixpath
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
 from datetime import datetime, timedelta, timezone
 from functools import cached_property
 from typing import NamedTuple, NewType, Optional, Union
 from urllib.parse import urlparse
 
 from dvcx.utils import is_expired, time_to_local_str, time_to_str
 
@@ -13,20 +12,14 @@
 # StorageURI represents a normalised URI to a valid storage location (full bucket or
 # absolute local path).
 # Valid examples: s3://foo, file:///var/data
 # Invalid examples: s3://foo/, s3://foo/bar, file://~
 StorageURI = NewType("StorageURI", str)
 
 
-@dataclass
-class StorageStats:
-    num_objects: int
-    size: int  # in bytes
-
-
 class Status:
     CREATED = 1
     PENDING = 2
     FAILED = 3
     COMPLETE = 4
     PARTIAL = 5
     STALE = 6
```

### Comparing `dvcx-0.84.1/src/dvcx/utils.py` & `dvcx-0.84.2/src/dvcx/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.84.2/src/dvcx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.84.1
+Version: 0.84.2
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.84.1/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.84.2/src/dvcx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/src/dvcx.egg-info/requires.txt` & `dvcx-0.84.2/src/dvcx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/benchmarks/conftest.py` & `dvcx-0.84.2/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/conftest.py` & `dvcx-0.84.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/data.py` & `dvcx-0.84.2/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/func/test_catalog.py` & `dvcx-0.84.2/tests/func/test_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1046,14 +1046,19 @@
     assert stats.size == 36
 
     catalog.enlist_source(f"{src_uri}/dogs/", ttl=1234, force_update=True)
     stats = catalog.storage_stats(src_uri)
     assert stats.num_objects == 6
     assert stats.size == 15
 
+    catalog.enlist_source(f"{src_uri}/dogs/", ttl=1234)
+    stats = catalog.storage_stats(src_uri)
+    assert stats.num_objects == 6
+    assert stats.size == 15
+
 
 @pytest.mark.parametrize("from_cli", [False, True])
 def test_garbage_collect(cloud_test_catalog, from_cli, capsys):
     catalog = cloud_test_catalog.catalog
     assert catalog.get_temp_table_names() == []
     temp_tables = ["tmp_vc12F", "udf_jh653", "ds_shadow_12345", "old_ds_shadow"]
     for t in temp_tables:
```

### Comparing `dvcx-0.84.1/tests/func/test_client.py` & `dvcx-0.84.2/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/func/test_dataset_query.py` & `dvcx-0.84.2/tests/func/test_dataset_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/func/test_datasets.py` & `dvcx-0.84.2/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/func/test_ls.py` & `dvcx-0.84.2/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/func/test_pull.py` & `dvcx-0.84.2/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/func/test_pytorch.py` & `dvcx-0.84.2/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/func/test_query.py` & `dvcx-0.84.2/tests/func/test_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/scripts/name_len_normal.py` & `dvcx-0.84.2/tests/scripts/name_len_normal.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/scripts/name_len_slow.py` & `dvcx-0.84.2/tests/scripts/name_len_slow.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/test_cli_e2e.py` & `dvcx-0.84.2/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/test_query_e2e.py` & `dvcx-0.84.2/tests/test_query_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/lib/test_cached_stream.py` & `dvcx-0.84.2/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/lib/test_feature.py` & `dvcx-0.84.2/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/lib/test_feature_udf.py` & `dvcx-0.84.2/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/lib/test_file.py` & `dvcx-0.84.2/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/lib/test_image.py` & `dvcx-0.84.2/tests/unit/lib/test_image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/lib/test_reader.py` & `dvcx-0.84.2/tests/unit/lib/test_reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/lib/test_text.py` & `dvcx-0.84.2/tests/unit/lib/test_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/lib/test_webdataset.py` & `dvcx-0.84.2/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.84.2/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/sql/test_array.py` & `dvcx-0.84.2/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/sql/test_conditional.py` & `dvcx-0.84.2/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/sql/test_path.py` & `dvcx-0.84.2/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/sql/test_selectable.py` & `dvcx-0.84.2/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/sql/test_string.py` & `dvcx-0.84.2/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_asyn.py` & `dvcx-0.84.2/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_cache.py` & `dvcx-0.84.2/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_catalog.py` & `dvcx-0.84.2/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_catalog_loader.py` & `dvcx-0.84.2/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_cli_parsing.py` & `dvcx-0.84.2/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_client.py` & `dvcx-0.84.2/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_client_s3.py` & `dvcx-0.84.2/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_data_storage.py` & `dvcx-0.84.2/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_database_engine.py` & `dvcx-0.84.2/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_dataset.py` & `dvcx-0.84.2/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_dataset_row.py` & `dvcx-0.84.2/tests/unit/test_dataset_row.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_dispatch.py` & `dvcx-0.84.2/tests/unit/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_fileslice.py` & `dvcx-0.84.2/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_id_generator.py` & `dvcx-0.84.2/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_listing.py` & `dvcx-0.84.2/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_metastore.py` & `dvcx-0.84.2/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_query_params.py` & `dvcx-0.84.2/tests/unit/test_query_params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_serializer.py` & `dvcx-0.84.2/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_session.py` & `dvcx-0.84.2/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_storage.py` & `dvcx-0.84.2/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_udf.py` & `dvcx-0.84.2/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_utils.py` & `dvcx-0.84.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/unit/test_warehouse.py` & `dvcx-0.84.2/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.84.1/tests/utils.py` & `dvcx-0.84.2/tests/utils.py`

 * *Files identical despite different names*

