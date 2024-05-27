# Comparing `tmp/ena-upload-cli-0.7.1.tar.gz` & `tmp/ena_upload_cli-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ena-upload-cli-0.7.1.tar", last modified: Mon Feb 26 09:08:40 2024, max compression
+gzip compressed data, was "ena_upload_cli-0.7.2.tar", last modified: Mon May 27 20:52:19 2024, max compression
```

## Comparing `ena-upload-cli-0.7.1.tar` & `ena_upload_cli-0.7.2.tar`

### file list

```diff
@@ -1,111 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 09:08:40.720432 ena-upload-cli-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-02-26 09:08:40.720432 ena-upload-cli-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17298 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 09:08:40.700432 ena-upload-cli-0.7.1/ena_upload/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/check_remote.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    39654 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/ena_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 09:08:40.700432 ena-upload-cli-0.7.1/ena_upload/json_parsing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/characteristic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/ena_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/ena_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/ena_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/ena_std_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/ena_study.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/ena_submission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 09:08:40.704432 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/assay_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/comment_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/data_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/factor_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/factor_value_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/investigation_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/material_attribute_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/material_attribute_value_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/material_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/ontology_annotation_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/ontology_source_reference_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/organization_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/person_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/process_parameter_value_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/process_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/protocol_parameter_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/protocol_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/publication_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/sample_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/source_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/study_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/json_parsing/other_material.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 09:08:40.716432 ena-upload-cli-0.7.1/ena_upload/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA.project.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_FILE.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_LIBRARY_SELECTION.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_LIBRARY_SOURCE.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_LIBRARY_STRATEGY.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13860 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_PLATFORM.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     3941 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_experiments.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1574 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_runs.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000011.xml
--rw-r--r--   0 runner    (1001) docker     (127)    23159 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000012.xml
--rw-r--r--   0 runner    (1001) docker     (127)    25952 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000013.xml
--rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000014.xml
--rw-r--r--   0 runner    (1001) docker     (127)    24133 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000015.xml
--rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000016.xml
--rw-r--r--   0 runner    (1001) docker     (127)    24160 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000017.xml
--rw-r--r--   0 runner    (1001) docker     (127)    25738 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000018.xml
--rw-r--r--   0 runner    (1001) docker     (127)    33299 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000019.xml
--rw-r--r--   0 runner    (1001) docker     (127)    29318 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000020.xml
--rw-r--r--   0 runner    (1001) docker     (127)    31653 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000021.xml
--rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000022.xml
--rw-r--r--   0 runner    (1001) docker     (127)    26198 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000023.xml
--rw-r--r--   0 runner    (1001) docker     (127)    38427 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000024.xml
--rw-r--r--   0 runner    (1001) docker     (127)    27714 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000025.xml
--rw-r--r--   0 runner    (1001) docker     (127)    39402 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000027.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000028.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13965 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000029.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10610 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000030.xml
--rw-r--r--   0 runner    (1001) docker     (127)    23556 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000031.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18257 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000032.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11603 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000033.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000034.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000035.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000036.xml
--rw-r--r--   0 runner    (1001) docker     (127)    28819 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000037.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10169 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000038.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000039.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000040.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000041.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000043.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000044.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000045.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18030 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000047.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18408 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000048.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000049.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16645 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000050.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000051.xml
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000052.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13144 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000053.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2398 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_studies.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_submission.xml
--rw-r--r--   0 runner    (1001) docker     (127)    58767 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/SRA.common.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    38057 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/SRA.experiment.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    48712 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/SRA.run.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/SRA.sample.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/SRA.study.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    18180 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/ena_upload/templates/SRA.submission.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 09:08:40.716432 ena-upload-cli-0.7.1/ena_upload_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-02-26 09:08:40.000000 ena-upload-cli-0.7.1/ena_upload_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-02-26 09:08:40.000000 ena-upload-cli-0.7.1/ena_upload_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 09:08:40.000000 ena-upload-cli-0.7.1/ena_upload_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-26 09:08:40.000000 ena-upload-cli-0.7.1/ena_upload_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-26 09:08:40.000000 ena-upload-cli-0.7.1/ena_upload_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-26 09:08:40.000000 ena-upload-cli-0.7.1/ena_upload_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 09:08:40.720432 ena-upload-cli-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 09:08:40.716432 ena-upload-cli-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-02-26 09:08:30.000000 ena-upload-cli-0.7.1/tests/test_ena_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:52:19.716726 ena_upload_cli-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-05-27 20:52:19.716726 ena_upload_cli-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17298 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:52:19.696725 ena_upload_cli-0.7.2/ena_upload/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/check_remote.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39912 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/ena_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:52:19.696725 ena_upload_cli-0.7.2/ena_upload/json_parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/characteristic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/ena_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/ena_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/ena_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/ena_std_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/ena_study.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/ena_submission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:52:19.700726 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/assay_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/comment_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/data_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/factor_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/factor_value_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/investigation_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/material_attribute_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/material_attribute_value_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/material_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/ontology_annotation_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/ontology_source_reference_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/organization_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/person_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/process_parameter_value_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/process_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/protocol_parameter_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/protocol_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/publication_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/sample_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/source_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/study_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/json_parsing/other_material.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:52:19.712726 ena_upload_cli-0.7.2/ena_upload/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA.project.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_FILE.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_LIBRARY_SELECTION.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_LIBRARY_SOURCE.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_LIBRARY_STRATEGY.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13860 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_PLATFORM.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3941 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_experiments.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1574 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_runs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000011.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    23143 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000012.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    28586 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000013.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    30076 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000014.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25179 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000015.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000016.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    25206 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000017.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    27068 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000018.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    33368 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000019.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    35384 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000020.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    34928 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000021.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    32062 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000022.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    27059 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000023.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    39703 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000024.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000025.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    39431 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000027.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000028.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000029.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000030.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    62012 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000031.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18293 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000032.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000033.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000034.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000035.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000036.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    28543 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000037.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000038.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000039.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000040.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000041.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000043.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000044.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000045.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17776 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000047.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18154 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000048.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21422 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000049.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16347 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000050.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000051.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000052.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000053.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    50165 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000055.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    80129 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000056.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    33230 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000057.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    43796 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000058.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2398 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_studies.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_submission.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    58767 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/SRA.common.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    38057 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/SRA.experiment.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    48712 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/SRA.run.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/SRA.sample.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/SRA.study.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    18180 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/ena_upload/templates/SRA.submission.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:52:19.716726 ena_upload_cli-0.7.2/ena_upload_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-05-27 20:52:19.000000 ena_upload_cli-0.7.2/ena_upload_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-27 20:52:19.000000 ena_upload_cli-0.7.2/ena_upload_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:52:19.000000 ena_upload_cli-0.7.2/ena_upload_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-27 20:52:19.000000 ena_upload_cli-0.7.2/ena_upload_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 20:52:19.000000 ena_upload_cli-0.7.2/ena_upload_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 20:52:19.000000 ena_upload_cli-0.7.2/ena_upload_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:52:19.716726 ena_upload_cli-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:52:19.716726 ena_upload_cli-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-27 20:52:16.000000 ena_upload_cli-0.7.2/tests/test_ena_objects.py
```

### Comparing `ena-upload-cli-0.7.1/LICENSE` & `ena_upload_cli-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/PKG-INFO` & `ena_upload_cli-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ena-upload-cli
-Version: 0.7.1
+Version: 0.7.2
 Summary: Command Line Interface to upload data to the European Nucleotide Archive
 Home-page: https://github.com/usegalaxy-eu/ena-upload-cli
 Author: Dilmurat Yusuf
 Author-email: bjoern.gruening@gmail.com
 License: MIT
 Keywords: pip,ena-upload-cli,cli,ENA,upload
 Classifier: Operating System :: OS Independent
```

### Comparing `ena-upload-cli-0.7.1/README.md` & `ena_upload_cli-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/check_remote.py` & `ena_upload_cli-0.7.2/ena_upload/check_remote.py`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/ena_upload.py` & `ena_upload_cli-0.7.2/ena_upload/ena_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,20 @@
 
     def ntransfercmd(self, cmd, rest=None):
         conn, size = ftplib.FTP.ntransfercmd(self, cmd, rest)
         if self._prot_p:
             conn = self.context.wrap_socket(conn,
                                             server_hostname=self.host,
                                             session=self.sock.session)
+            # fix reuse of ssl socket:
+            # https://stackoverflow.com/a/53456626/10971151 and
+            # https://stackoverflow.com/a/70830916/10971151
+            def custom_unwrap():
+                pass
+            conn.unwrap = custom_unwrap
         return conn, size
 
 
 def create_dataframe(schema_tables, action, dev, auto_action):
     '''create pandas dataframe from the tables in schema_tables
        and return schema_dataframe
 
@@ -403,15 +409,15 @@
     :param file_paths: a dictionary of filename string and file_path string
     :param args: the command-line arguments parsed by ArgumentParser
     """
     ftp_host = "webin2.ebi.ac.uk"
 
     print("\nConnecting to ftp.webin2.ebi.ac.uk....")
     try:
-        ftps = MyFTP_TLS(timeout=10)
+        ftps = MyFTP_TLS(timeout=120)
         ftps.context.set_ciphers('HIGH:!DH:!aNULL')
         ftps.connect(ftp_host, port=21)
         ftps.auth()
         ftps.login(webin_id, password)
         ftps.prot_p()
 
     except IOError as ioe:
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/characteristic.py` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/characteristic.py`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/ena_experiment.py` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/ena_experiment.py`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/ena_run.py` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/ena_run.py`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/ena_sample.py` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/ena_sample.py`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/ena_std_lib.py` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/ena_std_lib.py`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/ena_study.py` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/ena_study.py`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/ena_submission.py` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/ena_submission.py`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/assay_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/assay_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/data_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/data_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/factor_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/factor_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/factor_value_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/factor_value_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/investigation_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/investigation_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/material_attribute_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/material_attribute_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/material_attribute_value_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/material_attribute_value_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/material_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/material_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/ontology_annotation_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/ontology_annotation_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/ontology_source_reference_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/ontology_source_reference_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/person_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/person_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/process_parameter_value_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/process_parameter_value_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/process_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/process_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/protocol_parameter_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/protocol_parameter_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/protocol_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/protocol_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/publication_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/publication_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/sample_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/sample_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/source_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/source_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/json_schemas/study_schema.json` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/json_schemas/study_schema.json`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/json_parsing/other_material.py` & `ena_upload_cli-0.7.2/ena_upload/json_parsing/other_material.py`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA.project.xsd` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA.project.xsd`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_FILE.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_FILE.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_LIBRARY_SELECTION.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_LIBRARY_SELECTION.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_LIBRARY_SOURCE.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_LIBRARY_SOURCE.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_LIBRARY_STRATEGY.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_LIBRARY_STRATEGY.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_PLATFORM.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_PLATFORM.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_experiments.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_experiments.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_runs.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_runs.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000011.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000011.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000012.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000012.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000012.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000012.xml`

```diff
@@ -26,153 +26,123 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'estimated size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
@@ -189,26 +159,14 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'altitude', index)">
@@ -278,87 +236,31 @@
         </py:if>
         <py:if test="attributetest(row, 'ventilation type')">
           <SAMPLE_ATTRIBUTE>
             <TAG>ventilation type</TAG>
             <VALUE>${row['ventilation type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organism count</TAG>
             <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample storage duration</TAG>
             <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host disease status')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host disease status</TAG>
             <VALUE>${row['host disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -462,60 +364,157 @@
         <py:if test="attributetest(row, 'salinity')">
           <SAMPLE_ATTRIBUTE>
             <TAG>salinity</TAG>
             <VALUE>${row['salinity']}</VALUE>
             <UNITS>psu</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'negative control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'positive control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
             <TAG>encoded traits</TAG>
             <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample material processing')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000013.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000013.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000013.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000013.xml`

```diff
@@ -26,151 +26,145 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'observed host symbionts')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>observed host symbionts</TAG>
+            <VALUE>${row['observed host symbionts']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'sample disease stage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>sample disease stage</TAG>
+            <VALUE>${row['sample disease stage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'sample disease status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>sample disease status</TAG>
+            <VALUE>${row['sample disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'sample derived from')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>sample derived from</TAG>
+            <VALUE>${row['sample derived from']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'target gene')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>target gene</TAG>
-            <VALUE>${row['target gene']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'target subfragment')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>target subfragment</TAG>
-            <VALUE>${row['target subfragment']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'multiplex identifiers')">
+        <py:if test="attributetest(row, 'estimated size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>multiplex identifiers</TAG>
-            <VALUE>${row['multiplex identifiers']}</VALUE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
+        <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
+            <TAG>target gene</TAG>
+            <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
+        <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
+            <TAG>target subfragment</TAG>
+            <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
+        <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
+            <TAG>multiplex identifiers</TAG>
+            <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -189,26 +183,14 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'altitude')">
@@ -240,21 +222,14 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'depth')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'local environmental context', index)">
@@ -272,88 +247,43 @@
         <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
             <TAG>elevation</TAG>
             <VALUE>${row['elevation']}</VALUE>
             <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host body product')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>host body product</TAG>
-            <VALUE>${row['host body product']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'host dry mass')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>host dry mass</TAG>
-            <VALUE>${row['host dry mass']}</VALUE>
-            <UNITS>mg</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organism count</TAG>
             <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage duration')">
+        <py:if test="attributetest(row, 'sample capture status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage duration</TAG>
-            <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
+            <TAG>sample capture status</TAG>
+            <VALUE>${row['sample capture status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
+        <py:if test="attributetest(row, 'biological status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
+            <TAG>biological status</TAG>
+            <VALUE>${row['biological status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
+        <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
+            <TAG>sample storage duration</TAG>
+            <VALUE>${row['sample storage duration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host disease status')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host disease status</TAG>
             <VALUE>${row['host disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -487,14 +417,20 @@
         <py:if test="attributetest(row, 'salinity')">
           <SAMPLE_ATTRIBUTE>
             <TAG>salinity</TAG>
             <VALUE>${row['salinity']}</VALUE>
             <UNITS>psu</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'source material identifiers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'host blood pressure diastolic')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host blood pressure diastolic</TAG>
             <VALUE>${row['host blood pressure diastolic']}</VALUE>
             <UNITS>mm Hg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
@@ -531,60 +467,183 @@
         </py:if>
         <py:if test="attributetest(row, 'gravidity')">
           <SAMPLE_ATTRIBUTE>
             <TAG>gravidity</TAG>
             <VALUE>${row['gravidity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'host dry mass')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>host dry mass</TAG>
+            <VALUE>${row['host dry mass']}</VALUE>
+            <UNITS>mg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'host body product')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>host body product</TAG>
+            <VALUE>${row['host body product']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'negative control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'positive control type')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
             <TAG>encoded traits</TAG>
             <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'genetic modification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>genetic modification</TAG>
+            <VALUE>${row['genetic modification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'ancestral data')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>ancestral data</TAG>
+            <VALUE>${row['ancestral data']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'taxonomic classification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'isolation and growth condition')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample material processing')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'depth')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000014.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000018.xml`

 * *Files 3% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000014.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000018.xml`

```diff
@@ -26,153 +26,135 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'observed host symbionts')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>observed host symbionts</TAG>
+            <VALUE>${row['observed host symbionts']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'medical history performed')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>medical history performed</TAG>
+            <VALUE>${row['medical history performed']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'estimated size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
@@ -189,38 +171,27 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'study completion status')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>study completion status</TAG>
-            <VALUE>${row['study completion status']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'altitude')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>altitude</TAG>
+            <VALUE>${row['altitude']}</VALUE>
+            <UNITS>m</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="mandatorytest(row, 'geographic location (country and/or sea)', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (country and/or sea)</TAG>
             <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'geographic location (latitude)', index)">
@@ -257,149 +228,58 @@
         </py:if>
         <py:if test="mandatorytest(row, 'environmental medium', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>environmental medium</TAG>
             <VALUE>${row['environmental medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
+        <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
+            <TAG>elevation</TAG>
+            <VALUE>${row['elevation']}</VALUE>
+            <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host body product')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>host body product</TAG>
-            <VALUE>${row['host body product']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'medical history performed')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>medical history performed</TAG>
-            <VALUE>${row['medical history performed']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'urine/collection method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>urine/collection method</TAG>
-            <VALUE>${row['urine/collection method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organism count</TAG>
             <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample storage duration</TAG>
             <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
+        <py:if test="attributetest(row, 'gynecological disorder')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
+            <TAG>gynecological disorder</TAG>
+            <VALUE>${row['gynecological disorder']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host HIV status')">
+        <py:if test="attributetest(row, 'urogenital disorder')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host HIV status</TAG>
-            <VALUE>${row['host HIV status']}</VALUE>
+            <TAG>urogenital disorder</TAG>
+            <VALUE>${row['urogenital disorder']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host disease status')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host disease status</TAG>
             <VALUE>${row['host disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'lung/pulmonary disorder')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>lung/pulmonary disorder</TAG>
-            <VALUE>${row['lung/pulmonary disorder']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'lung/nose-throat disorder')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>lung/nose-throat disorder</TAG>
-            <VALUE>${row['lung/nose-throat disorder']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'blood/blood disorder')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>blood/blood disorder</TAG>
-            <VALUE>${row['blood/blood disorder']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'urine/kidney disorder')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>urine/kidney disorder</TAG>
-            <VALUE>${row['urine/kidney disorder']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'urine/urogenital tract disorder')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>urine/urogenital tract disorder</TAG>
-            <VALUE>${row['urine/urogenital tract disorder']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'host subject id')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host subject id</TAG>
             <VALUE>${row['host subject id']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'IHMC medication code')">
@@ -417,20 +297,14 @@
         </py:if>
         <py:if test="attributetest(row, 'host body site')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host body site</TAG>
             <VALUE>${row['host body site']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'drug usage')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>drug usage</TAG>
-            <VALUE>${row['drug usage']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'host height')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host height</TAG>
             <VALUE>${row['host height']}</VALUE>
             <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
@@ -481,166 +355,263 @@
         </py:if>
         <py:if test="attributetest(row, 'host scientific name')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host scientific name</TAG>
             <VALUE>${row['host scientific name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'presence of pets or farm animals')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>presence of pets or farm animals</TAG>
-            <VALUE>${row['presence of pets or farm animals']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'temperature')">
           <SAMPLE_ATTRIBUTE>
             <TAG>temperature</TAG>
             <VALUE>${row['temperature']}</VALUE>
             <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'sample salinity')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample salinity</TAG>
+            <VALUE>${row['sample salinity']}</VALUE>
+            <UNITS>psu</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'salinity')">
           <SAMPLE_ATTRIBUTE>
             <TAG>salinity</TAG>
             <VALUE>${row['salinity']}</VALUE>
             <UNITS>psu</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'smoker')">
+        <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>smoker</TAG>
-            <VALUE>${row['smoker']}</VALUE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'major diet change in last six months')">
+        <py:if test="attributetest(row, 'menarche')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>major diet change in last six months</TAG>
-            <VALUE>${row['major diet change in last six months']}</VALUE>
+            <TAG>menarche</TAG>
+            <VALUE>${row['menarche']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'weight loss in last three months')">
+        <py:if test="attributetest(row, 'sexual activity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>weight loss in last three months</TAG>
-            <VALUE>${row['weight loss in last three months']}</VALUE>
-            <UNITS>kg</UNITS>
+            <TAG>sexual activity</TAG>
+            <VALUE>${row['sexual activity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'travel outside the country in last six months')">
+        <py:if test="attributetest(row, 'pregnancy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>travel outside the country in last six months</TAG>
-            <VALUE>${row['travel outside the country in last six months']}</VALUE>
+            <TAG>pregnancy</TAG>
+            <VALUE>${row['pregnancy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host diet')">
+        <py:if test="attributetest(row, 'douche')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host diet</TAG>
-            <VALUE>${row['host diet']}</VALUE>
+            <TAG>douche</TAG>
+            <VALUE>${row['douche']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'twin sibling presence')">
+        <py:if test="attributetest(row, 'birth control')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>twin sibling presence</TAG>
-            <VALUE>${row['twin sibling presence']}</VALUE>
+            <TAG>birth control</TAG>
+            <VALUE>${row['birth control']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host last meal')">
+        <py:if test="attributetest(row, 'menopause')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host last meal</TAG>
-            <VALUE>${row['host last meal']}</VALUE>
+            <TAG>menopause</TAG>
+            <VALUE>${row['menopause']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'amniotic fluid/gestation state')">
+        <py:if test="attributetest(row, 'HRT')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>amniotic fluid/gestation state</TAG>
-            <VALUE>${row['amniotic fluid/gestation state']}</VALUE>
+            <TAG>HRT</TAG>
+            <VALUE>${row['HRT']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host family relationship')">
+        <py:if test="attributetest(row, 'hysterectomy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host family relationship</TAG>
-            <VALUE>${row['host family relationship']}</VALUE>
+            <TAG>hysterectomy</TAG>
+            <VALUE>${row['hysterectomy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'amniotic fluid/maternal health status')">
+        <py:if test="attributetest(row, 'host diet')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>amniotic fluid/maternal health status</TAG>
-            <VALUE>${row['amniotic fluid/maternal health status']}</VALUE>
+            <TAG>host diet</TAG>
+            <VALUE>${row['host diet']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host genotype')">
+        <py:if test="attributetest(row, 'host last meal')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host genotype</TAG>
-            <VALUE>${row['host genotype']}</VALUE>
+            <TAG>host last meal</TAG>
+            <VALUE>${row['host last meal']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'amniotic fluid/foetal health status')">
+        <py:if test="attributetest(row, 'host family relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>amniotic fluid/foetal health status</TAG>
-            <VALUE>${row['amniotic fluid/foetal health status']}</VALUE>
+            <TAG>host family relationship</TAG>
+            <VALUE>${row['host family relationship']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'host genotype')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>host genotype</TAG>
+            <VALUE>${row['host genotype']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host pulse')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host pulse</TAG>
             <VALUE>${row['host pulse']}</VALUE>
             <UNITS>bpm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'amniotic fluid/color')">
+        <py:if test="attributetest(row, 'host body product')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>amniotic fluid/color</TAG>
-            <VALUE>${row['amniotic fluid/color']}</VALUE>
+            <TAG>host body product</TAG>
+            <VALUE>${row['host body product']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'negative control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'positive control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'experimental factor')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
             <TAG>encoded traits</TAG>
             <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample material processing')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000015.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000015.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000015.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000015.xml`

```diff
@@ -26,153 +26,135 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'observed host symbionts')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>observed host symbionts</TAG>
+            <VALUE>${row['observed host symbionts']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'medical history performed')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>medical history performed</TAG>
+            <VALUE>${row['medical history performed']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'estimated size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
@@ -189,32 +171,27 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'altitude')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>altitude</TAG>
+            <VALUE>${row['altitude']}</VALUE>
+            <UNITS>m</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="mandatorytest(row, 'geographic location (country and/or sea)', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (country and/or sea)</TAG>
             <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'geographic location (latitude)', index)">
@@ -251,99 +228,38 @@
         </py:if>
         <py:if test="mandatorytest(row, 'environmental medium', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>environmental medium</TAG>
             <VALUE>${row['environmental medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
+        <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
+            <TAG>elevation</TAG>
+            <VALUE>${row['elevation']}</VALUE>
+            <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host body product')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>host body product</TAG>
-            <VALUE>${row['host body product']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'medical history performed')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>medical history performed</TAG>
-            <VALUE>${row['medical history performed']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organism count</TAG>
             <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample storage duration</TAG>
             <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'gastrointestinal tract disorder')">
           <SAMPLE_ATTRIBUTE>
             <TAG>gastrointestinal tract disorder</TAG>
             <VALUE>${row['gastrointestinal tract disorder']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -433,28 +349,40 @@
         </py:if>
         <py:if test="attributetest(row, 'host sex')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host sex</TAG>
             <VALUE>${row['host sex']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'host scientific name')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>host scientific name</TAG>
+            <VALUE>${row['host scientific name']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'temperature')">
           <SAMPLE_ATTRIBUTE>
             <TAG>temperature</TAG>
             <VALUE>${row['temperature']}</VALUE>
             <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'salinity')">
           <SAMPLE_ATTRIBUTE>
             <TAG>salinity</TAG>
             <VALUE>${row['salinity']}</VALUE>
             <UNITS>psu</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'source material identifiers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'special diet')">
           <SAMPLE_ATTRIBUTE>
             <TAG>special diet</TAG>
             <VALUE>${row['special diet']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host diet')">
@@ -484,60 +412,157 @@
         <py:if test="attributetest(row, 'host pulse')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host pulse</TAG>
             <VALUE>${row['host pulse']}</VALUE>
             <UNITS>bpm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'host body product')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>host body product</TAG>
+            <VALUE>${row['host body product']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'negative control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'positive control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
             <TAG>encoded traits</TAG>
             <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample material processing')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000016.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000016.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000016.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000016.xml`

```diff
@@ -26,153 +26,135 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'observed host symbionts')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>observed host symbionts</TAG>
+            <VALUE>${row['observed host symbionts']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'medical history performed')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>medical history performed</TAG>
+            <VALUE>${row['medical history performed']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'estimated size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
@@ -189,32 +171,33 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
+        <py:if test="attributetest(row, 'lat_lon')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
+            <TAG>lat_lon</TAG>
+            <VALUE>${row['lat_lon']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'altitude')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>altitude</TAG>
+            <VALUE>${row['altitude']}</VALUE>
+            <UNITS>m</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="mandatorytest(row, 'geographic location (country and/or sea)', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (country and/or sea)</TAG>
             <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'geographic location (latitude)', index)">
@@ -251,99 +234,38 @@
         </py:if>
         <py:if test="mandatorytest(row, 'environmental medium', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>environmental medium</TAG>
             <VALUE>${row['environmental medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
+        <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
+            <TAG>elevation</TAG>
+            <VALUE>${row['elevation']}</VALUE>
+            <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host body product')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>host body product</TAG>
-            <VALUE>${row['host body product']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'medical history performed')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>medical history performed</TAG>
-            <VALUE>${row['medical history performed']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organism count</TAG>
             <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample storage duration</TAG>
             <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'nose/mouth/teeth/throat disorder')">
           <SAMPLE_ATTRIBUTE>
             <TAG>nose/mouth/teeth/throat disorder</TAG>
             <VALUE>${row['nose/mouth/teeth/throat disorder']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -427,28 +349,40 @@
         </py:if>
         <py:if test="attributetest(row, 'host sex')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host sex</TAG>
             <VALUE>${row['host sex']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'host scientific name')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>host scientific name</TAG>
+            <VALUE>${row['host scientific name']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'temperature')">
           <SAMPLE_ATTRIBUTE>
             <TAG>temperature</TAG>
             <VALUE>${row['temperature']}</VALUE>
             <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'salinity')">
           <SAMPLE_ATTRIBUTE>
             <TAG>salinity</TAG>
             <VALUE>${row['salinity']}</VALUE>
             <UNITS>psu</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'source material identifiers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'time since last toothbrushing')">
           <SAMPLE_ATTRIBUTE>
             <TAG>time since last toothbrushing</TAG>
             <VALUE>${row['time since last toothbrushing']}</VALUE>
             <UNITS>minutes</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
@@ -479,60 +413,157 @@
         <py:if test="attributetest(row, 'host pulse')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host pulse</TAG>
             <VALUE>${row['host pulse']}</VALUE>
             <UNITS>bpm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'host body product')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>host body product</TAG>
+            <VALUE>${row['host body product']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'negative control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'positive control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
             <TAG>encoded traits</TAG>
             <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample material processing')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000017.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000017.xml`

 * *Files 2% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000017.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000017.xml`

```diff
@@ -26,153 +26,135 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'observed host symbionts')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>observed host symbionts</TAG>
+            <VALUE>${row['observed host symbionts']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'medical history performed')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>medical history performed</TAG>
+            <VALUE>${row['medical history performed']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'estimated size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
@@ -189,32 +171,27 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'altitude')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>altitude</TAG>
+            <VALUE>${row['altitude']}</VALUE>
+            <UNITS>m</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="mandatorytest(row, 'geographic location (country and/or sea)', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (country and/or sea)</TAG>
             <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'geographic location (latitude)', index)">
@@ -251,99 +228,38 @@
         </py:if>
         <py:if test="mandatorytest(row, 'environmental medium', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>environmental medium</TAG>
             <VALUE>${row['environmental medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
+        <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
+            <TAG>elevation</TAG>
+            <VALUE>${row['elevation']}</VALUE>
+            <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host body product')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>host body product</TAG>
-            <VALUE>${row['host body product']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'medical history performed')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>medical history performed</TAG>
-            <VALUE>${row['medical history performed']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organism count</TAG>
             <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample storage duration</TAG>
             <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'dermatology disorder')">
           <SAMPLE_ATTRIBUTE>
             <TAG>dermatology disorder</TAG>
             <VALUE>${row['dermatology disorder']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -427,28 +343,40 @@
         </py:if>
         <py:if test="attributetest(row, 'host sex')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host sex</TAG>
             <VALUE>${row['host sex']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'host scientific name')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>host scientific name</TAG>
+            <VALUE>${row['host scientific name']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'temperature')">
           <SAMPLE_ATTRIBUTE>
             <TAG>temperature</TAG>
             <VALUE>${row['temperature']}</VALUE>
             <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'salinity')">
           <SAMPLE_ATTRIBUTE>
             <TAG>salinity</TAG>
             <VALUE>${row['salinity']}</VALUE>
             <UNITS>psu</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'source material identifiers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'time since last wash')">
           <SAMPLE_ATTRIBUTE>
             <TAG>time since last wash</TAG>
             <VALUE>${row['time since last wash']}</VALUE>
             <UNITS>minutes</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
@@ -485,60 +413,157 @@
         <py:if test="attributetest(row, 'host pulse')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host pulse</TAG>
             <VALUE>${row['host pulse']}</VALUE>
             <UNITS>bpm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'host body product')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>host body product</TAG>
+            <VALUE>${row['host body product']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'negative control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'positive control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
             <TAG>encoded traits</TAG>
             <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample material processing')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000018.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000025.xml`

 * *Files 3% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000018.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000025.xml`

```diff
@@ -26,153 +26,130 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'density')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>density</TAG>
+            <VALUE>${row['density']}</VALUE>
+            <UNITS>g/m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'estimated size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
@@ -189,32 +166,27 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'altitude')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>altitude</TAG>
+            <VALUE>${row['altitude']}</VALUE>
+            <UNITS>m</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="mandatorytest(row, 'geographic location (country and/or sea)', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (country and/or sea)</TAG>
             <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'geographic location (latitude)', index)">
@@ -251,335 +223,418 @@
         </py:if>
         <py:if test="mandatorytest(row, 'environmental medium', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>environmental medium</TAG>
             <VALUE>${row['environmental medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
+        <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
+            <TAG>elevation</TAG>
+            <VALUE>${row['elevation']}</VALUE>
+            <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
+        <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
+            <TAG>amount or size of sample collected</TAG>
+            <VALUE>${row['amount or size of sample collected']}</VALUE>
+            <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
+        <py:if test="attributetest(row, 'biomass')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
+            <TAG>biomass</TAG>
+            <VALUE>${row['biomass']}</VALUE>
+            <UNITS>t</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'propagation')">
+        <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
+            <TAG>organism count</TAG>
+            <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'amount or size of sample collected')">
+        <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>amount or size of sample collected</TAG>
-            <VALUE>${row['amount or size of sample collected']}</VALUE>
-            <UNITS>m3</UNITS>
+            <TAG>sample storage duration</TAG>
+            <VALUE>${row['sample storage duration']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'host disease status')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>host disease status</TAG>
+            <VALUE>${row['host disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host body product')">
+        <py:if test="attributetest(row, 'host scientific name')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host body product</TAG>
-            <VALUE>${row['host body product']}</VALUE>
+            <TAG>host scientific name</TAG>
+            <VALUE>${row['host scientific name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'medical history performed')">
+        <py:if test="attributetest(row, 'water current')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>medical history performed</TAG>
-            <VALUE>${row['medical history performed']}</VALUE>
+            <TAG>water current</TAG>
+            <VALUE>${row['water current']}</VALUE>
+            <UNITS>m3/s</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
+        <py:if test="attributetest(row, 'pressure')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
+            <TAG>pressure</TAG>
+            <VALUE>${row['pressure']}</VALUE>
+            <UNITS>bar</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'organism count')">
+        <py:if test="attributetest(row, 'temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>organism count</TAG>
-            <VALUE>${row['organism count']}</VALUE>
+            <TAG>temperature</TAG>
+            <VALUE>${row['temperature']}</VALUE>
+            <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage duration')">
+        <py:if test="attributetest(row, 'pH')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage duration</TAG>
-            <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
+            <TAG>pH</TAG>
+            <VALUE>${row['pH']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
+        <py:if test="attributetest(row, 'ammonium')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
+            <TAG>ammonium</TAG>
+            <VALUE>${row['ammonium']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
+        <py:if test="attributetest(row, 'bromide')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
+            <TAG>bromide</TAG>
+            <VALUE>${row['bromide']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
+        <py:if test="attributetest(row, 'calcium')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
+            <TAG>calcium</TAG>
+            <VALUE>${row['calcium']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
+        <py:if test="attributetest(row, 'chloride')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
+            <TAG>chloride</TAG>
+            <VALUE>${row['chloride']}</VALUE>
+            <UNITS>mg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'gynecological disorder')">
+        <py:if test="attributetest(row, 'chlorophyll')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>gynecological disorder</TAG>
-            <VALUE>${row['gynecological disorder']}</VALUE>
+            <TAG>chlorophyll</TAG>
+            <VALUE>${row['chlorophyll']}</VALUE>
+            <UNITS>µg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'urogenital disorder')">
+        <py:if test="attributetest(row, 'diether lipids')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>urogenital disorder</TAG>
-            <VALUE>${row['urogenital disorder']}</VALUE>
+            <TAG>diether lipids</TAG>
+            <VALUE>${row['diether lipids']}</VALUE>
+            <UNITS>ng/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host disease status')">
+        <py:if test="attributetest(row, 'dissolved carbon dioxide')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host disease status</TAG>
-            <VALUE>${row['host disease status']}</VALUE>
+            <TAG>dissolved carbon dioxide</TAG>
+            <VALUE>${row['dissolved carbon dioxide']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host subject id')">
+        <py:if test="attributetest(row, 'dissolved hydrogen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host subject id</TAG>
-            <VALUE>${row['host subject id']}</VALUE>
+            <TAG>dissolved hydrogen</TAG>
+            <VALUE>${row['dissolved hydrogen']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'IHMC medication code')">
+        <py:if test="attributetest(row, 'dissolved inorganic carbon')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>IHMC medication code</TAG>
-            <VALUE>${row['IHMC medication code']}</VALUE>
+            <TAG>dissolved inorganic carbon</TAG>
+            <VALUE>${row['dissolved inorganic carbon']}</VALUE>
+            <UNITS>µg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host age')">
+        <py:if test="attributetest(row, 'dissolved organic nitrogen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host age</TAG>
-            <VALUE>${row['host age']}</VALUE>
-            <UNITS>years</UNITS>
+            <TAG>dissolved organic nitrogen</TAG>
+            <VALUE>${row['dissolved organic nitrogen']}</VALUE>
+            <UNITS>µg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host body site')">
+        <py:if test="attributetest(row, 'dissolved oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host body site</TAG>
-            <VALUE>${row['host body site']}</VALUE>
+            <TAG>dissolved oxygen</TAG>
+            <VALUE>${row['dissolved oxygen']}</VALUE>
+            <UNITS>µmol/kg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host height')">
+        <py:if test="attributetest(row, 'nitrate')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host height</TAG>
-            <VALUE>${row['host height']}</VALUE>
-            <UNITS>mm</UNITS>
+            <TAG>nitrate</TAG>
+            <VALUE>${row['nitrate']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host body-mass index')">
+        <py:if test="attributetest(row, 'nitrite')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host body-mass index</TAG>
-            <VALUE>${row['host body-mass index']}</VALUE>
-            <UNITS>kg/m2</UNITS>
+            <TAG>nitrite</TAG>
+            <VALUE>${row['nitrite']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ethnicity')">
+        <py:if test="attributetest(row, 'total nitrogen concentration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ethnicity</TAG>
-            <VALUE>${row['ethnicity']}</VALUE>
+            <TAG>total nitrogen concentration</TAG>
+            <VALUE>${row['total nitrogen concentration']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host occupation')">
+        <py:if test="attributetest(row, 'organic carbon')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host occupation</TAG>
-            <VALUE>${row['host occupation']}</VALUE>
+            <TAG>organic carbon</TAG>
+            <VALUE>${row['organic carbon']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host total mass')">
+        <py:if test="attributetest(row, 'organic matter')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host total mass</TAG>
-            <VALUE>${row['host total mass']}</VALUE>
-            <UNITS>kg</UNITS>
+            <TAG>organic matter</TAG>
+            <VALUE>${row['organic matter']}</VALUE>
+            <UNITS>µg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host phenotype')">
+        <py:if test="attributetest(row, 'organic nitrogen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host phenotype</TAG>
-            <VALUE>${row['host phenotype']}</VALUE>
+            <TAG>organic nitrogen</TAG>
+            <VALUE>${row['organic nitrogen']}</VALUE>
+            <UNITS>µg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host body temperature')">
+        <py:if test="attributetest(row, 'phosphate')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host body temperature</TAG>
-            <VALUE>${row['host body temperature']}</VALUE>
-            <UNITS>ºC</UNITS>
+            <TAG>phosphate</TAG>
+            <VALUE>${row['phosphate']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host sex')">
+        <py:if test="attributetest(row, 'phospholipid fatty acid')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host sex</TAG>
-            <VALUE>${row['host sex']}</VALUE>
+            <TAG>phospholipid fatty acid</TAG>
+            <VALUE>${row['phospholipid fatty acid']}</VALUE>
+            <UNITS>mol/g</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'temperature')">
+        <py:if test="attributetest(row, 'potassium')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>temperature</TAG>
-            <VALUE>${row['temperature']}</VALUE>
-            <UNITS>ºC</UNITS>
+            <TAG>potassium</TAG>
+            <VALUE>${row['potassium']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'salinity')">
           <SAMPLE_ATTRIBUTE>
             <TAG>salinity</TAG>
             <VALUE>${row['salinity']}</VALUE>
             <UNITS>psu</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'menarche')">
+        <py:if test="attributetest(row, 'silicate')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>menarche</TAG>
-            <VALUE>${row['menarche']}</VALUE>
+            <TAG>silicate</TAG>
+            <VALUE>${row['silicate']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sexual activity')">
+        <py:if test="attributetest(row, 'sodium')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sexual activity</TAG>
-            <VALUE>${row['sexual activity']}</VALUE>
+            <TAG>sodium</TAG>
+            <VALUE>${row['sodium']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pregnancy')">
+        <py:if test="attributetest(row, 'sulfate')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>pregnancy</TAG>
-            <VALUE>${row['pregnancy']}</VALUE>
+            <TAG>sulfate</TAG>
+            <VALUE>${row['sulfate']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'douche')">
+        <py:if test="attributetest(row, 'sulfide')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>douche</TAG>
-            <VALUE>${row['douche']}</VALUE>
+            <TAG>sulfide</TAG>
+            <VALUE>${row['sulfide']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'birth control')">
+        <py:if test="attributetest(row, 'alkalinity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>birth control</TAG>
-            <VALUE>${row['birth control']}</VALUE>
+            <TAG>alkalinity</TAG>
+            <VALUE>${row['alkalinity']}</VALUE>
+            <UNITS>mEq/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'menopause')">
+        <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>menopause</TAG>
-            <VALUE>${row['menopause']}</VALUE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'HRT')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>HRT</TAG>
-            <VALUE>${row['HRT']}</VALUE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'hysterectomy')">
+        <py:if test="attributetest(row, 'negative control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>hysterectomy</TAG>
-            <VALUE>${row['hysterectomy']}</VALUE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host diet')">
+        <py:if test="attributetest(row, 'positive control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host diet</TAG>
-            <VALUE>${row['host diet']}</VALUE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host last meal')">
+        <py:if test="attributetest(row, 'experimental factor')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host last meal</TAG>
-            <VALUE>${row['host last meal']}</VALUE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host family relationship')">
+        <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host family relationship</TAG>
-            <VALUE>${row['host family relationship']}</VALUE>
+            <TAG>encoded traits</TAG>
+            <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host genotype')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host genotype</TAG>
-            <VALUE>${row['host genotype']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host pulse')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host pulse</TAG>
-            <VALUE>${row['host pulse']}</VALUE>
-            <UNITS>bpm</UNITS>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'annotation source')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'reference for biomaterial')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'sample material processing')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'encoded traits')">
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>encoded traits</TAG>
-            <VALUE>${row['encoded traits']}</VALUE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'library size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'depth')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000019.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000019.xml`

 * *Files 2% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000019.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000019.xml`

```diff
@@ -26,153 +26,123 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'estimated size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
@@ -189,26 +159,14 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'altitude')">
@@ -240,21 +198,14 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'depth', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'local environmental context', index)">
@@ -272,115 +223,52 @@
         <py:if test="mandatorytest(row, 'elevation', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>elevation</TAG>
             <VALUE>${row['elevation']}</VALUE>
             <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'biomass')">
           <SAMPLE_ATTRIBUTE>
             <TAG>biomass</TAG>
             <VALUE>${row['biomass']}</VALUE>
             <UNITS>t</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organism count</TAG>
             <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample storage duration</TAG>
             <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host disease status')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host disease status</TAG>
             <VALUE>${row['host disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host scientific name')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host scientific name</TAG>
             <VALUE>${row['host scientific name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'alkalinity')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>alkalinity</TAG>
-            <VALUE>${row['alkalinity']}</VALUE>
-            <UNITS>mEq/L</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'mean friction velocity')">
           <SAMPLE_ATTRIBUTE>
             <TAG>mean friction velocity</TAG>
             <VALUE>${row['mean friction velocity']}</VALUE>
             <UNITS>m/s</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
@@ -414,14 +302,21 @@
         </py:if>
         <py:if test="attributetest(row, 'pH')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pH</TAG>
             <VALUE>${row['pH']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'water content')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>water content</TAG>
+            <VALUE>${row['water content']}</VALUE>
+            <UNITS>g/g</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'alkyl diethers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>alkyl diethers</TAG>
             <VALUE>${row['alkyl diethers']}</VALUE>
             <UNITS>µg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
@@ -574,18 +469,18 @@
         <py:if test="attributetest(row, 'nitrite')">
           <SAMPLE_ATTRIBUTE>
             <TAG>nitrite</TAG>
             <VALUE>${row['nitrite']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nitrogen')">
+        <py:if test="attributetest(row, 'total nitrogen concentration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nitrogen</TAG>
-            <VALUE>${row['nitrogen']}</VALUE>
+            <TAG>total nitrogen concentration</TAG>
+            <VALUE>${row['total nitrogen concentration']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'organic carbon')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organic carbon</TAG>
             <VALUE>${row['organic carbon']}</VALUE>
@@ -686,88 +581,192 @@
         <py:if test="attributetest(row, 'total organic carbon')">
           <SAMPLE_ATTRIBUTE>
             <TAG>total organic carbon</TAG>
             <VALUE>${row['total organic carbon']}</VALUE>
             <UNITS>g/kg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'water content')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>water content</TAG>
-            <VALUE>${row['water content']}</VALUE>
-            <UNITS>g/g</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sulfate')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sulfate</TAG>
             <VALUE>${row['sulfate']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sulfide')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sulfide</TAG>
             <VALUE>${row['sulfide']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'total nitrogen')">
+        <py:if test="attributetest(row, 'total nitrogen content')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>total nitrogen</TAG>
-            <VALUE>${row['total nitrogen']}</VALUE>
+            <TAG>total nitrogen content</TAG>
+            <VALUE>${row['total nitrogen content']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'alkalinity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>alkalinity</TAG>
+            <VALUE>${row['alkalinity']}</VALUE>
+            <UNITS>mEq/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'negative control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'positive control type')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
             <TAG>encoded traits</TAG>
             <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample material processing')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'depth', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000020.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000014.xml`

 * *Files 7% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000020.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000014.xml`

```diff
@@ -26,151 +26,145 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'observed host symbionts')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>observed host symbionts</TAG>
+            <VALUE>${row['observed host symbionts']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'urine/collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>urine/collection method</TAG>
+            <VALUE>${row['urine/collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'medical history performed')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>medical history performed</TAG>
+            <VALUE>${row['medical history performed']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'study completion status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>study completion status</TAG>
+            <VALUE>${row['study completion status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'target gene')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>target gene</TAG>
-            <VALUE>${row['target gene']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'target subfragment')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>target subfragment</TAG>
-            <VALUE>${row['target subfragment']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'multiplex identifiers')">
+        <py:if test="attributetest(row, 'estimated size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>multiplex identifiers</TAG>
-            <VALUE>${row['multiplex identifiers']}</VALUE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
+        <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
+            <TAG>target gene</TAG>
+            <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
+        <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
+            <TAG>target subfragment</TAG>
+            <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
+        <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
+            <TAG>multiplex identifiers</TAG>
+            <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -189,26 +183,14 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'altitude')">
@@ -240,21 +222,14 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'depth')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'local environmental context', index)">
@@ -272,158 +247,136 @@
         <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
             <TAG>elevation</TAG>
             <VALUE>${row['elevation']}</VALUE>
             <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host dry mass')">
+        <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host dry mass</TAG>
-            <VALUE>${row['host dry mass']}</VALUE>
-            <UNITS>mg</UNITS>
+            <TAG>organism count</TAG>
+            <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
+        <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
+            <TAG>sample storage duration</TAG>
+            <VALUE>${row['sample storage duration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'plant product')">
+        <py:if test="attributetest(row, 'nose/mouth/teeth/throat disorder')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>plant product</TAG>
-            <VALUE>${row['plant product']}</VALUE>
+            <TAG>nose/mouth/teeth/throat disorder</TAG>
+            <VALUE>${row['nose/mouth/teeth/throat disorder']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'organism count')">
+        <py:if test="attributetest(row, 'host HIV status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>organism count</TAG>
-            <VALUE>${row['organism count']}</VALUE>
+            <TAG>host HIV status</TAG>
+            <VALUE>${row['host HIV status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage duration')">
+        <py:if test="attributetest(row, 'host disease status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage duration</TAG>
-            <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
+            <TAG>host disease status</TAG>
+            <VALUE>${row['host disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
+        <py:if test="attributetest(row, 'lung/pulmonary disorder')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
+            <TAG>lung/pulmonary disorder</TAG>
+            <VALUE>${row['lung/pulmonary disorder']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host wet mass')">
+        <py:if test="attributetest(row, 'lung/nose-throat disorder')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host wet mass</TAG>
-            <VALUE>${row['host wet mass']}</VALUE>
-            <UNITS>mg</UNITS>
+            <TAG>lung/nose-throat disorder</TAG>
+            <VALUE>${row['lung/nose-throat disorder']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
+        <py:if test="attributetest(row, 'blood/blood disorder')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
+            <TAG>blood/blood disorder</TAG>
+            <VALUE>${row['blood/blood disorder']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
+        <py:if test="attributetest(row, 'urine/kidney disorder')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
+            <TAG>urine/kidney disorder</TAG>
+            <VALUE>${row['urine/kidney disorder']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
+        <py:if test="attributetest(row, 'urine/urogenital tract disorder')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
+            <TAG>urine/urogenital tract disorder</TAG>
+            <VALUE>${row['urine/urogenital tract disorder']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host disease status')">
+        <py:if test="attributetest(row, 'host subject id')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host disease status</TAG>
-            <VALUE>${row['host disease status']}</VALUE>
+            <TAG>host subject id</TAG>
+            <VALUE>${row['host subject id']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host common name')">
+        <py:if test="attributetest(row, 'IHMC medication code')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host common name</TAG>
-            <VALUE>${row['host common name']}</VALUE>
+            <TAG>IHMC medication code</TAG>
+            <VALUE>${row['IHMC medication code']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host age')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host age</TAG>
             <VALUE>${row['host age']}</VALUE>
             <UNITS>years</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host taxid')">
+        <py:if test="attributetest(row, 'host body site')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host taxid</TAG>
-            <VALUE>${row['host taxid']}</VALUE>
+            <TAG>host body site</TAG>
+            <VALUE>${row['host body site']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host life stage')">
+        <py:if test="attributetest(row, 'drug usage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host life stage</TAG>
-            <VALUE>${row['host life stage']}</VALUE>
+            <TAG>drug usage</TAG>
+            <VALUE>${row['drug usage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host height')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host height</TAG>
             <VALUE>${row['host height']}</VALUE>
             <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host length')">
+        <py:if test="attributetest(row, 'host body-mass index')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host length</TAG>
-            <VALUE>${row['host length']}</VALUE>
-            <UNITS>mm</UNITS>
+            <TAG>host body-mass index</TAG>
+            <VALUE>${row['host body-mass index']}</VALUE>
+            <UNITS>kg/m2</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'ethnicity')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>ethnicity</TAG>
+            <VALUE>${row['ethnicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'plant body site')">
+        <py:if test="attributetest(row, 'host occupation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>plant body site</TAG>
-            <VALUE>${row['plant body site']}</VALUE>
+            <TAG>host occupation</TAG>
+            <VALUE>${row['host occupation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host total mass')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host total mass</TAG>
             <VALUE>${row['host total mass']}</VALUE>
             <UNITS>kg</UNITS>
@@ -431,36 +384,37 @@
         </py:if>
         <py:if test="attributetest(row, 'host phenotype')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host phenotype</TAG>
             <VALUE>${row['host phenotype']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'host body temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host subspecific genetic lineage</TAG>
-            <VALUE>${row['host subspecific genetic lineage']}</VALUE>
+            <TAG>host body temperature</TAG>
+            <VALUE>${row['host body temperature']}</VALUE>
+            <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'climate environment')">
+        <py:if test="attributetest(row, 'host sex')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>climate environment</TAG>
-            <VALUE>${row['climate environment']}</VALUE>
+            <TAG>host sex</TAG>
+            <VALUE>${row['host sex']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'gaseous environment')">
+        <py:if test="attributetest(row, 'host scientific name')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>gaseous environment</TAG>
-            <VALUE>${row['gaseous environment']}</VALUE>
+            <TAG>host scientific name</TAG>
+            <VALUE>${row['host scientific name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'seasonal environment')">
+        <py:if test="attributetest(row, 'presence of pets, animals, or insects')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>seasonal environment</TAG>
-            <VALUE>${row['seasonal environment']}</VALUE>
+            <TAG>presence of pets, animals, or insects</TAG>
+            <VALUE>${row['presence of pets, animals, or insects']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'temperature')">
           <SAMPLE_ATTRIBUTE>
             <TAG>temperature</TAG>
             <VALUE>${row['temperature']}</VALUE>
             <UNITS>ºC</UNITS>
@@ -469,198 +423,249 @@
         <py:if test="attributetest(row, 'salinity')">
           <SAMPLE_ATTRIBUTE>
             <TAG>salinity</TAG>
             <VALUE>${row['salinity']}</VALUE>
             <UNITS>psu</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host genotype')">
+        <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host genotype</TAG>
-            <VALUE>${row['host genotype']}</VALUE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'smoker')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>smoker</TAG>
+            <VALUE>${row['smoker']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'major diet change in last six months')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>major diet change in last six months</TAG>
+            <VALUE>${row['major diet change in last six months']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'weight loss in last three months')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>weight loss in last three months</TAG>
+            <VALUE>${row['weight loss in last three months']}</VALUE>
+            <UNITS>kg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'travel outside the country in last six months')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>travel outside the country in last six months</TAG>
+            <VALUE>${row['travel outside the country in last six months']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'encoded traits')">
+        <py:if test="attributetest(row, 'host diet')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>encoded traits</TAG>
-            <VALUE>${row['encoded traits']}</VALUE>
+            <TAG>host diet</TAG>
+            <VALUE>${row['host diet']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'twin sibling presence')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>twin sibling presence</TAG>
+            <VALUE>${row['twin sibling presence']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'air temperature regimen')">
+        <py:if test="attributetest(row, 'host last meal')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>air temperature regimen</TAG>
-            <VALUE>${row['air temperature regimen']}</VALUE>
+            <TAG>host last meal</TAG>
+            <VALUE>${row['host last meal']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'antibiotic regimen')">
+        <py:if test="attributetest(row, 'amniotic fluid/gestation state')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>antibiotic regimen</TAG>
-            <VALUE>${row['antibiotic regimen']}</VALUE>
+            <TAG>amniotic fluid/gestation state</TAG>
+            <VALUE>${row['amniotic fluid/gestation state']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical mutagen')">
+        <py:if test="attributetest(row, 'host family relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical mutagen</TAG>
-            <VALUE>${row['chemical mutagen']}</VALUE>
+            <TAG>host family relationship</TAG>
+            <VALUE>${row['host family relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'fertilizer regimen')">
+        <py:if test="attributetest(row, 'amniotic fluid/maternal health status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>fertilizer regimen</TAG>
-            <VALUE>${row['fertilizer regimen']}</VALUE>
+            <TAG>amniotic fluid/maternal health status</TAG>
+            <VALUE>${row['amniotic fluid/maternal health status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'fungicide regimen')">
+        <py:if test="attributetest(row, 'host genotype')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>fungicide regimen</TAG>
-            <VALUE>${row['fungicide regimen']}</VALUE>
+            <TAG>host genotype</TAG>
+            <VALUE>${row['host genotype']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'gravity')">
+        <py:if test="attributetest(row, 'amniotic fluid/foetal health status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>gravity</TAG>
-            <VALUE>${row['gravity']}</VALUE>
+            <TAG>amniotic fluid/foetal health status</TAG>
+            <VALUE>${row['amniotic fluid/foetal health status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'growth hormone regimen')">
+        <py:if test="attributetest(row, 'host pulse')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>growth hormone regimen</TAG>
-            <VALUE>${row['growth hormone regimen']}</VALUE>
+            <TAG>host pulse</TAG>
+            <VALUE>${row['host pulse']}</VALUE>
+            <UNITS>bpm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'growth media')">
+        <py:if test="attributetest(row, 'amniotic fluid/color')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>growth media</TAG>
-            <VALUE>${row['growth media']}</VALUE>
+            <TAG>amniotic fluid/color</TAG>
+            <VALUE>${row['amniotic fluid/color']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'herbicide regimen')">
+        <py:if test="attributetest(row, 'host body product')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>herbicide regimen</TAG>
-            <VALUE>${row['herbicide regimen']}</VALUE>
+            <TAG>host body product</TAG>
+            <VALUE>${row['host body product']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'humidity regimen')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>humidity regimen</TAG>
-            <VALUE>${row['humidity regimen']}</VALUE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'mineral nutrient regimen')">
+        <py:if test="attributetest(row, 'negative control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>mineral nutrient regimen</TAG>
-            <VALUE>${row['mineral nutrient regimen']}</VALUE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'non-mineral nutrient regimen')">
+        <py:if test="attributetest(row, 'positive control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>non-mineral nutrient regimen</TAG>
-            <VALUE>${row['non-mineral nutrient regimen']}</VALUE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pesticide regimen')">
+        <py:if test="attributetest(row, 'experimental factor')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>pesticide regimen</TAG>
-            <VALUE>${row['pesticide regimen']}</VALUE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pH regimen')">
+        <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>pH regimen</TAG>
-            <VALUE>${row['pH regimen']}</VALUE>
+            <TAG>encoded traits</TAG>
+            <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'radiation regimen')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>radiation regimen</TAG>
-            <VALUE>${row['radiation regimen']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'rainfall regimen')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>rainfall regimen</TAG>
-            <VALUE>${row['rainfall regimen']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'salt regimen')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>salt regimen</TAG>
-            <VALUE>${row['salt regimen']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'standing water regimen')">
+        <py:if test="attributetest(row, 'annotation source')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>standing water regimen</TAG>
-            <VALUE>${row['standing water regimen']}</VALUE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'tissue culture growth media')">
+        <py:if test="attributetest(row, 'reference for biomaterial')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>tissue culture growth media</TAG>
-            <VALUE>${row['tissue culture growth media']}</VALUE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'watering regimen')">
+        <py:if test="attributetest(row, 'sample material processing')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>watering regimen</TAG>
-            <VALUE>${row['watering regimen']}</VALUE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'water temperature regimen')">
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>water temperature regimen</TAG>
-            <VALUE>${row['water temperature regimen']}</VALUE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'mechanical damage')">
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>mechanical damage</TAG>
-            <VALUE>${row['mechanical damage']}</VALUE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'library size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000021.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000037.xml`

 * *Files 5% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000021.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000037.xml`

```diff
@@ -26,187 +26,188 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'soil_taxonomic/FAO classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>soil_taxonomic/FAO classification</TAG>
+            <VALUE>${row['soil_taxonomic/FAO classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'soil_taxonomic/local classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>soil_taxonomic/local classification</TAG>
+            <VALUE>${row['soil_taxonomic/local classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'soil_taxonomic/local classification method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>soil_taxonomic/local classification method</TAG>
+            <VALUE>${row['soil_taxonomic/local classification method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'soil type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>soil type</TAG>
+            <VALUE>${row['soil type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'soil type method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>soil type method</TAG>
+            <VALUE>${row['soil type method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'soil texture measurement')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>soil texture measurement</TAG>
+            <VALUE>${row['soil texture measurement']}</VALUE>
+            <UNITS>% sand/silt/clay</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'soil texture method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>soil texture method</TAG>
+            <VALUE>${row['soil texture method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="attributetest(row, 'soil pH')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>soil pH</TAG>
+            <VALUE>${row['soil pH']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'growth facility')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>growth facility</TAG>
+            <VALUE>${row['growth facility']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="mandatorytest(row, 'plant developmental stage', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>plant developmental stage</TAG>
+            <VALUE>${row['plant developmental stage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'sampled age')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>sampled age</TAG>
+            <VALUE>${row['sampled age']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'target gene')">
+        <py:if test="attributetest(row, 'sample health state')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>target gene</TAG>
-            <VALUE>${row['target gene']}</VALUE>
+            <TAG>sample health state</TAG>
+            <VALUE>${row['sample health state']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'target subfragment')">
+        <py:if test="attributetest(row, 'sample wet mass')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>target subfragment</TAG>
-            <VALUE>${row['target subfragment']}</VALUE>
+            <TAG>sample wet mass</TAG>
+            <VALUE>${row['sample wet mass']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
+        <py:if test="attributetest(row, 'sample disease stage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
+            <TAG>sample disease stage</TAG>
+            <VALUE>${row['sample disease stage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'multiplex identifiers')">
+        <py:if test="attributetest(row, 'sample length')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>multiplex identifiers</TAG>
-            <VALUE>${row['multiplex identifiers']}</VALUE>
+            <TAG>sample length</TAG>
+            <VALUE>${row['sample length']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
+        <py:if test="attributetest(row, 'sample height')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
+            <TAG>sample height</TAG>
+            <VALUE>${row['sample height']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
+        <py:if test="attributetest(row, 'sample dry mass')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
+            <TAG>sample dry mass</TAG>
+            <VALUE>${row['sample dry mass']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
+        <py:if test="attributetest(row, 'sample disease status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
+            <TAG>sample disease status</TAG>
+            <VALUE>${row['sample disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sequence quality check')">
+        <py:if test="attributetest(row, 'sample phenotype')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sequence quality check</TAG>
-            <VALUE>${row['sequence quality check']}</VALUE>
+            <TAG>sample phenotype</TAG>
+            <VALUE>${row['sample phenotype']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chimera check software')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chimera check software</TAG>
-            <VALUE>${row['chimera check software']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relevant electronic resources')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relevant electronic resources</TAG>
-            <VALUE>${row['relevant electronic resources']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relevant standard operating procedures')">
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relevant standard operating procedures</TAG>
-            <VALUE>${row['relevant standard operating procedures']}</VALUE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
+        <py:if test="attributetest(row, 'estimated size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
+        <py:if test="attributetest(row, 'collected_by')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
+            <TAG>collected_by</TAG>
+            <VALUE>${row['collected_by']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -240,495 +241,402 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'depth', index)">
+        <py:if test="attributetest(row, 'identified_by')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
+            <TAG>identified_by</TAG>
+            <VALUE>${row['identified_by']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
+        <py:if test="attributetest(row, 'broad-scale environmental context')">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'local environmental context', index)">
+        <py:if test="attributetest(row, 'local environmental context')">
           <SAMPLE_ATTRIBUTE>
             <TAG>local environmental context</TAG>
             <VALUE>${row['local environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'environmental medium', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>environmental medium</TAG>
-            <VALUE>${row['environmental medium']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'elevation', index)">
+        <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
             <TAG>elevation</TAG>
             <VALUE>${row['elevation']}</VALUE>
             <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'biomass')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>biomass</TAG>
-            <VALUE>${row['biomass']}</VALUE>
-            <UNITS>t</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'density')">
+        <py:if test="attributetest(row, 'sampling time point')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>density</TAG>
-            <VALUE>${row['density']}</VALUE>
-            <UNITS>g/m3</UNITS>
+            <TAG>sampling time point</TAG>
+            <VALUE>${row['sampling time point']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
+        <py:if test="attributetest(row, 'sample capture status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
+            <TAG>sample capture status</TAG>
+            <VALUE>${row['sample capture status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'organism count')">
+        <py:if test="attributetest(row, 'organism common name')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>organism count</TAG>
-            <VALUE>${row['organism count']}</VALUE>
+            <TAG>organism common name</TAG>
+            <VALUE>${row['organism common name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage duration')">
+        <py:if test="attributetest(row, 'biological status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage duration</TAG>
-            <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
+            <TAG>biological status</TAG>
+            <VALUE>${row['biological status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
+        <py:if test="attributetest(row, 'growth habit')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
+            <TAG>growth habit</TAG>
+            <VALUE>${row['growth habit']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
+        <py:if test="attributetest(row, 'plant sex')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
+            <TAG>plant sex</TAG>
+            <VALUE>${row['plant sex']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
+        <py:if test="mandatorytest(row, 'plant structure', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
+            <TAG>plant structure</TAG>
+            <VALUE>${row['plant structure']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host disease status')">
+        <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host disease status</TAG>
-            <VALUE>${row['host disease status']}</VALUE>
+            <TAG>sample storage duration</TAG>
+            <VALUE>${row['sample storage duration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host scientific name')">
+        <py:if test="attributetest(row, 'climate environment')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host scientific name</TAG>
-            <VALUE>${row['host scientific name']}</VALUE>
+            <TAG>climate environment</TAG>
+            <VALUE>${row['climate environment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'alkyl diethers')">
+        <py:if test="attributetest(row, 'gaseous environment')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>alkyl diethers</TAG>
-            <VALUE>${row['alkyl diethers']}</VALUE>
-            <UNITS>µg/L</UNITS>
+            <TAG>gaseous environment</TAG>
+            <VALUE>${row['gaseous environment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'aminopeptidase activity')">
+        <py:if test="attributetest(row, 'seasonal environment')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>aminopeptidase activity</TAG>
-            <VALUE>${row['aminopeptidase activity']}</VALUE>
-            <UNITS>mol/L/h</UNITS>
+            <TAG>seasonal environment</TAG>
+            <VALUE>${row['seasonal environment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ammonium')">
+        <py:if test="attributetest(row, 'drainage classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ammonium</TAG>
-            <VALUE>${row['ammonium']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>drainage classification</TAG>
+            <VALUE>${row['drainage classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'bacterial carbon production')">
+        <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>bacterial carbon production</TAG>
-            <VALUE>${row['bacterial carbon production']}</VALUE>
-            <UNITS>ng/h</UNITS>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'bishomohopanol')">
+        <py:if test="attributetest(row, 'source material description')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>bishomohopanol</TAG>
-            <VALUE>${row['bishomohopanol']}</VALUE>
-            <UNITS>µg/g</UNITS>
+            <TAG>source material description</TAG>
+            <VALUE>${row['source material description']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'bromide')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>bromide</TAG>
-            <VALUE>${row['bromide']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'calcium')">
+        <py:if test="attributetest(row, 'genotype')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>calcium</TAG>
-            <VALUE>${row['calcium']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>genotype</TAG>
+            <VALUE>${row['genotype']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'carbon/nitrogen ratio')">
+        <py:if test="attributetest(row, 'genetic modification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>carbon/nitrogen ratio</TAG>
-            <VALUE>${row['carbon/nitrogen ratio']}</VALUE>
+            <TAG>genetic modification</TAG>
+            <VALUE>${row['genetic modification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chloride')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage rank')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chloride</TAG>
-            <VALUE>${row['chloride']}</VALUE>
-            <UNITS>mg/L</UNITS>
+            <TAG>subspecific genetic lineage rank</TAG>
+            <VALUE>${row['subspecific genetic lineage rank']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chlorophyll')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage name')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chlorophyll</TAG>
-            <VALUE>${row['chlorophyll']}</VALUE>
-            <UNITS>µg/L</UNITS>
+            <TAG>subspecific genetic lineage name</TAG>
+            <VALUE>${row['subspecific genetic lineage name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'diether lipids')">
+        <py:if test="attributetest(row, 'organism phenotype')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>diether lipids</TAG>
-            <VALUE>${row['diether lipids']}</VALUE>
-            <UNITS>ng/L</UNITS>
+            <TAG>organism phenotype</TAG>
+            <VALUE>${row['organism phenotype']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'dissolved carbon dioxide')">
+        <py:if test="attributetest(row, 'ancestral data')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>dissolved carbon dioxide</TAG>
-            <VALUE>${row['dissolved carbon dioxide']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>ancestral data</TAG>
+            <VALUE>${row['ancestral data']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'dissolved hydrogen')">
+        <py:if test="mandatorytest(row, 'plant growth medium', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>dissolved hydrogen</TAG>
-            <VALUE>${row['dissolved hydrogen']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>plant growth medium</TAG>
+            <VALUE>${row['plant growth medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'dissolved inorganic carbon')">
+        <py:if test="attributetest(row, 'rooting conditions')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>dissolved inorganic carbon</TAG>
-            <VALUE>${row['dissolved inorganic carbon']}</VALUE>
-            <UNITS>µg/L</UNITS>
+            <TAG>rooting conditions</TAG>
+            <VALUE>${row['rooting conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'dissolved organic carbon')">
+        <py:if test="attributetest(row, 'culture rooting medium')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>dissolved organic carbon</TAG>
-            <VALUE>${row['dissolved organic carbon']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>culture rooting medium</TAG>
+            <VALUE>${row['culture rooting medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'dissolved organic nitrogen')">
+        <py:if test="attributetest(row, 'rooting medium macronutrients')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>dissolved organic nitrogen</TAG>
-            <VALUE>${row['dissolved organic nitrogen']}</VALUE>
-            <UNITS>µg/L</UNITS>
+            <TAG>rooting medium macronutrients</TAG>
+            <VALUE>${row['rooting medium macronutrients']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'methane')">
+        <py:if test="attributetest(row, 'rooting medium micronutrients')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>methane</TAG>
-            <VALUE>${row['methane']}</VALUE>
-            <UNITS>µM/L</UNITS>
+            <TAG>rooting medium micronutrients</TAG>
+            <VALUE>${row['rooting medium micronutrients']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'dissolved oxygen')">
+        <py:if test="attributetest(row, 'rooting medium organic supplements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>dissolved oxygen</TAG>
-            <VALUE>${row['dissolved oxygen']}</VALUE>
-            <UNITS>µmol/kg</UNITS>
+            <TAG>rooting medium organic supplements</TAG>
+            <VALUE>${row['rooting medium organic supplements']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'glucosidase activity')">
+        <py:if test="attributetest(row, 'rooting medium carbon')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>glucosidase activity</TAG>
-            <VALUE>${row['glucosidase activity']}</VALUE>
-            <UNITS>mol/L/h</UNITS>
+            <TAG>rooting medium carbon</TAG>
+            <VALUE>${row['rooting medium carbon']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'magnesium')">
+        <py:if test="attributetest(row, 'rooting medium regulators')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>magnesium</TAG>
-            <VALUE>${row['magnesium']}</VALUE>
-            <UNITS>parts/million</UNITS>
+            <TAG>rooting medium regulators</TAG>
+            <VALUE>${row['rooting medium regulators']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'n-alkanes')">
+        <py:if test="attributetest(row, 'rooting medium solidifier')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>n-alkanes</TAG>
-            <VALUE>${row['n-alkanes']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>rooting medium solidifier</TAG>
+            <VALUE>${row['rooting medium solidifier']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nitrate')">
+        <py:if test="attributetest(row, 'rooting medium pH')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nitrate</TAG>
-            <VALUE>${row['nitrate']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>rooting medium pH</TAG>
+            <VALUE>${row['rooting medium pH']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nitrite')">
+        <py:if test="mandatorytest(row, 'isolation and growth condition', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nitrite</TAG>
-            <VALUE>${row['nitrite']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nitrogen')">
+        <py:if test="attributetest(row, 'sample material processing')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nitrogen</TAG>
-            <VALUE>${row['nitrogen']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'organic carbon')">
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>organic carbon</TAG>
-            <VALUE>${row['organic carbon']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'organic matter')">
+        <py:if test="attributetest(row, 'depth')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>organic matter</TAG>
-            <VALUE>${row['organic matter']}</VALUE>
-            <UNITS>µg/L</UNITS>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'organic nitrogen')">
+        <py:if test="attributetest(row, 'air temperature regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>organic nitrogen</TAG>
-            <VALUE>${row['organic nitrogen']}</VALUE>
-            <UNITS>µg/L</UNITS>
+            <TAG>air temperature regimen</TAG>
+            <VALUE>${row['air temperature regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'particulate organic carbon')">
+        <py:if test="attributetest(row, 'antibiotic regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>particulate organic carbon</TAG>
-            <VALUE>${row['particulate organic carbon']}</VALUE>
-            <UNITS>µg/L</UNITS>
+            <TAG>antibiotic regimen</TAG>
+            <VALUE>${row['antibiotic regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'petroleum hydrocarbon')">
+        <py:if test="attributetest(row, 'chemical mutagen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>petroleum hydrocarbon</TAG>
-            <VALUE>${row['petroleum hydrocarbon']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>chemical mutagen</TAG>
+            <VALUE>${row['chemical mutagen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'phaeopigments')">
+        <py:if test="attributetest(row, 'fertilizer administration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>phaeopigments</TAG>
-            <VALUE>${row['phaeopigments']}</VALUE>
-            <UNITS>µg/L</UNITS>
+            <TAG>fertilizer administration</TAG>
+            <VALUE>${row['fertilizer administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'phosphate')">
+        <py:if test="attributetest(row, 'fungicide regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>phosphate</TAG>
-            <VALUE>${row['phosphate']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>fungicide regimen</TAG>
+            <VALUE>${row['fungicide regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'phospholipid fatty acid')">
+        <py:if test="attributetest(row, 'gravity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>phospholipid fatty acid</TAG>
-            <VALUE>${row['phospholipid fatty acid']}</VALUE>
-            <UNITS>mol/g</UNITS>
+            <TAG>gravity</TAG>
+            <VALUE>${row['gravity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'potassium')">
+        <py:if test="attributetest(row, 'growth hormone regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>potassium</TAG>
-            <VALUE>${row['potassium']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>growth hormone regimen</TAG>
+            <VALUE>${row['growth hormone regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'redox potential')">
+        <py:if test="attributetest(row, 'herbicide regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>redox potential</TAG>
-            <VALUE>${row['redox potential']}</VALUE>
-            <UNITS>mV</UNITS>
+            <TAG>herbicide regimen</TAG>
+            <VALUE>${row['herbicide regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'salinity')">
+        <py:if test="attributetest(row, 'humidity regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>salinity</TAG>
-            <VALUE>${row['salinity']}</VALUE>
-            <UNITS>psu</UNITS>
+            <TAG>humidity regimen</TAG>
+            <VALUE>${row['humidity regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'total carbon')">
+        <py:if test="attributetest(row, 'mineral nutrient regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>total carbon</TAG>
-            <VALUE>${row['total carbon']}</VALUE>
-            <UNITS>µg/L</UNITS>
+            <TAG>mineral nutrient regimen</TAG>
+            <VALUE>${row['mineral nutrient regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'silicate')">
+        <py:if test="attributetest(row, 'non-mineral nutrient regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>silicate</TAG>
-            <VALUE>${row['silicate']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>non-mineral nutrient regimen</TAG>
+            <VALUE>${row['non-mineral nutrient regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sodium')">
+        <py:if test="attributetest(row, 'pesticide regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sodium</TAG>
-            <VALUE>${row['sodium']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>pesticide regimen</TAG>
+            <VALUE>${row['pesticide regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'total organic carbon')">
+        <py:if test="attributetest(row, 'pH regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>total organic carbon</TAG>
-            <VALUE>${row['total organic carbon']}</VALUE>
-            <UNITS>g/kg</UNITS>
+            <TAG>pH regimen</TAG>
+            <VALUE>${row['pH regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'water content')">
+        <py:if test="attributetest(row, 'radiation regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>water content</TAG>
-            <VALUE>${row['water content']}</VALUE>
-            <UNITS>g/g</UNITS>
+            <TAG>radiation regimen</TAG>
+            <VALUE>${row['radiation regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sulfate')">
+        <py:if test="attributetest(row, 'rainfall regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sulfate</TAG>
-            <VALUE>${row['sulfate']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>rainfall regimen</TAG>
+            <VALUE>${row['rainfall regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sulfide')">
+        <py:if test="attributetest(row, 'salt regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sulfide</TAG>
-            <VALUE>${row['sulfide']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>salt regimen</TAG>
+            <VALUE>${row['salt regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'total nitrogen')">
+        <py:if test="attributetest(row, 'standing water regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>total nitrogen</TAG>
-            <VALUE>${row['total nitrogen']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>standing water regimen</TAG>
+            <VALUE>${row['standing water regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'watering regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>watering regimen</TAG>
+            <VALUE>${row['watering regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'water temperature regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>water temperature regimen</TAG>
+            <VALUE>${row['water temperature regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'plant treatment')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>plant treatment</TAG>
+            <VALUE>${row['plant treatment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'light regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>light regimen</TAG>
+            <VALUE>${row['light regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'encoded traits')">
+        <py:if test="attributetest(row, 'biotic regimen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>encoded traits</TAG>
-            <VALUE>${row['encoded traits']}</VALUE>
+            <TAG>biotic regimen</TAG>
+            <VALUE>${row['biotic regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'mechanical damage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>mechanical damage</TAG>
+            <VALUE>${row['mechanical damage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chemical administration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>chemical administration</TAG>
             <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL_VERSION</TAG>
           <VALUE>${tool_version}</VALUE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000022.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000022.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000022.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000022.xml`

```diff
@@ -26,172 +26,160 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="attributetest(row, 'slope gradient')">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>slope gradient</TAG>
-            <VALUE>${row['slope gradient']}</VALUE>
-            <UNITS>%</UNITS>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'slope aspect')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>slope aspect</TAG>
-            <VALUE>${row['slope aspect']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'profile position')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>profile position</TAG>
-            <VALUE>${row['profile position']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'sample storage conditions')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>sample storage conditions</TAG>
+            <VALUE>${row['sample storage conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'soil_taxonomic/FAO classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>soil_taxonomic/FAO classification</TAG>
+            <VALUE>${row['soil_taxonomic/FAO classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'soil_taxonomic/local classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>soil_taxonomic/local classification</TAG>
+            <VALUE>${row['soil_taxonomic/local classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'soil_taxonomic/local classification method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>soil_taxonomic/local classification method</TAG>
+            <VALUE>${row['soil_taxonomic/local classification method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'soil type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>soil type</TAG>
+            <VALUE>${row['soil type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'soil type method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>soil type method</TAG>
+            <VALUE>${row['soil type method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'soil texture measurement')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>soil texture measurement</TAG>
+            <VALUE>${row['soil texture measurement']}</VALUE>
+            <UNITS>% sand/silt/clay</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'soil texture method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>soil texture method</TAG>
+            <VALUE>${row['soil texture method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="attributetest(row, 'microbial biomass')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>microbial biomass</TAG>
+            <VALUE>${row['microbial biomass']}</VALUE>
+            <UNITS>g/kg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'estimated size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
@@ -208,32 +196,14 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pooling of DNA extracts (if done)')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pooling of DNA extracts (if done)</TAG>
-            <VALUE>${row['pooling of DNA extracts (if done)']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'altitude')">
@@ -265,21 +235,14 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'depth', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'local environmental context', index)">
@@ -297,93 +260,37 @@
         <py:if test="mandatorytest(row, 'elevation', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>elevation</TAG>
             <VALUE>${row['elevation']}</VALUE>
             <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'composite design/sieving (if any)')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>composite design/sieving (if any)</TAG>
-            <VALUE>${row['composite design/sieving (if any)']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sieving')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample weight for DNA extraction</TAG>
-            <VALUE>${row['sample weight for DNA extraction']}</VALUE>
-            <UNITS>g</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'storage conditions (fresh/frozen/other)')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>storage conditions (fresh/frozen/other)</TAG>
-            <VALUE>${row['storage conditions (fresh/frozen/other)']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'microbial biomass')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>microbial biomass</TAG>
-            <VALUE>${row['microbial biomass']}</VALUE>
-            <UNITS>g/kg</UNITS>
+            <TAG>sieving</TAG>
+            <VALUE>${row['sieving']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'microbial biomass method')">
           <SAMPLE_ATTRIBUTE>
             <TAG>microbial biomass method</TAG>
             <VALUE>${row['microbial biomass method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
+        <py:if test="attributetest(row, 'horizon method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'salinity method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>salinity method</TAG>
-            <VALUE>${row['salinity method']}</VALUE>
+            <TAG>horizon method</TAG>
+            <VALUE>${row['horizon method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'extreme_unusual_properties/heavy metals')">
           <SAMPLE_ATTRIBUTE>
             <TAG>extreme_unusual_properties/heavy metals</TAG>
             <VALUE>${row['extreme_unusual_properties/heavy metals']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -457,158 +364,133 @@
         </py:if>
         <py:if test="attributetest(row, 'soil horizon')">
           <SAMPLE_ATTRIBUTE>
             <TAG>soil horizon</TAG>
             <VALUE>${row['soil horizon']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'soil horizon method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>soil horizon method</TAG>
-            <VALUE>${row['soil horizon method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'mean annual and seasonal temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>mean annual and seasonal temperature</TAG>
-            <VALUE>${row['mean annual and seasonal temperature']}</VALUE>
-            <UNITS>ºC</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'mean annual and seasonal precipitation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>mean annual and seasonal precipitation</TAG>
-            <VALUE>${row['mean annual and seasonal precipitation']}</VALUE>
-            <UNITS>mm</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'soil_taxonomic/FAO classification')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>soil_taxonomic/FAO classification</TAG>
-            <VALUE>${row['soil_taxonomic/FAO classification']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'soil_taxonomic/local classification')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>soil_taxonomic/local classification</TAG>
-            <VALUE>${row['soil_taxonomic/local classification']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'soil_taxonomic/local classification method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>soil_taxonomic/local classification method</TAG>
-            <VALUE>${row['soil_taxonomic/local classification method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'soil type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>soil type</TAG>
-            <VALUE>${row['soil type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'soil type method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>soil type method</TAG>
-            <VALUE>${row['soil type method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'drainage classification')">
           <SAMPLE_ATTRIBUTE>
             <TAG>drainage classification</TAG>
             <VALUE>${row['drainage classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'temperature')">
           <SAMPLE_ATTRIBUTE>
             <TAG>temperature</TAG>
             <VALUE>${row['temperature']}</VALUE>
             <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'soil texture measurement')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>soil texture measurement</TAG>
-            <VALUE>${row['soil texture measurement']}</VALUE>
-            <UNITS>% sand/silt/clay</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'soil texture method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>soil texture method</TAG>
-            <VALUE>${row['soil texture method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'pH')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pH</TAG>
             <VALUE>${row['pH']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'pH method')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pH method</TAG>
             <VALUE>${row['pH method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'water content')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>water content</TAG>
+            <VALUE>${row['water content']}</VALUE>
+            <UNITS>g/g</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'slope gradient')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>slope gradient</TAG>
+            <VALUE>${row['slope gradient']}</VALUE>
+            <UNITS>%</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'slope aspect')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>slope aspect</TAG>
+            <VALUE>${row['slope aspect']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'profile position')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>profile position</TAG>
+            <VALUE>${row['profile position']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'water content method')">
           <SAMPLE_ATTRIBUTE>
             <TAG>water content method</TAG>
             <VALUE>${row['water content method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'total organic C method')">
+        <py:if test="attributetest(row, 'total organic carbon method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>total organic C method</TAG>
-            <VALUE>${row['total organic C method']}</VALUE>
+            <TAG>total organic carbon method</TAG>
+            <VALUE>${row['total organic carbon method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'total nitrogen method')">
+        <py:if test="attributetest(row, 'total nitrogen content method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>total nitrogen method</TAG>
-            <VALUE>${row['total nitrogen method']}</VALUE>
+            <TAG>total nitrogen content method</TAG>
+            <VALUE>${row['total nitrogen content method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'organic matter')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organic matter</TAG>
             <VALUE>${row['organic matter']}</VALUE>
             <UNITS>µg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'organic nitrogen')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>organic nitrogen</TAG>
+            <VALUE>${row['organic nitrogen']}</VALUE>
+            <UNITS>µg/L</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'total organic carbon')">
           <SAMPLE_ATTRIBUTE>
             <TAG>total organic carbon</TAG>
             <VALUE>${row['total organic carbon']}</VALUE>
             <UNITS>g/kg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'water content')">
+        <py:if test="attributetest(row, 'total nitrogen content')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>water content</TAG>
-            <VALUE>${row['water content']}</VALUE>
-            <UNITS>g/g</UNITS>
+            <TAG>total nitrogen content</TAG>
+            <VALUE>${row['total nitrogen content']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'total nitrogen')">
+        <py:if test="attributetest(row, 'salinity method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>total nitrogen</TAG>
-            <VALUE>${row['total nitrogen']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>salinity method</TAG>
+            <VALUE>${row['salinity method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'source material identifiers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'history/previous land use')">
           <SAMPLE_ATTRIBUTE>
             <TAG>history/previous land use</TAG>
             <VALUE>${row['history/previous land use']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'history/previous land use method')">
+        <py:if test="attributetest(row, 'previous land use method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>history/previous land use method</TAG>
-            <VALUE>${row['history/previous land use method']}</VALUE>
+            <TAG>previous land use method</TAG>
+            <VALUE>${row['previous land use method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'history/crop rotation')">
           <SAMPLE_ATTRIBUTE>
             <TAG>history/crop rotation</TAG>
             <VALUE>${row['history/crop rotation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -639,54 +521,192 @@
         </py:if>
         <py:if test="attributetest(row, 'history/extreme events')">
           <SAMPLE_ATTRIBUTE>
             <TAG>history/extreme events</TAG>
             <VALUE>${row['history/extreme events']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'mean seasonal temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>mean seasonal temperature</TAG>
+            <VALUE>${row['mean seasonal temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'mean seasonal precipitation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>mean seasonal precipitation</TAG>
+            <VALUE>${row['mean seasonal precipitation']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'mean annual precipitation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>mean annual precipitation</TAG>
+            <VALUE>${row['mean annual precipitation']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'mean annual temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>mean annual temperature</TAG>
+            <VALUE>${row['mean annual temperature']}</VALUE>
+            <UNITS>ºC</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'host specificity or range')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>host specificity or range</TAG>
+            <VALUE>${row['host specificity or range']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'perturbation')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'negative control type')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'positive control type')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
             <TAG>encoded traits</TAG>
             <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'isolation and growth condition')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample pooling')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample pooling</TAG>
+            <VALUE>${row['sample pooling']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample material processing')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'depth', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000023.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000023.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000023.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000023.xml`

```diff
@@ -26,153 +26,123 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'estimated size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
@@ -189,32 +159,27 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'altitude')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>altitude</TAG>
+            <VALUE>${row['altitude']}</VALUE>
+            <UNITS>m</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="mandatorytest(row, 'geographic location (country and/or sea)', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (country and/or sea)</TAG>
             <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'geographic location (latitude)', index)">
@@ -233,21 +198,14 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'depth')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'local environmental context', index)">
@@ -258,87 +216,38 @@
         </py:if>
         <py:if test="mandatorytest(row, 'environmental medium', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>environmental medium</TAG>
             <VALUE>${row['environmental medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
+        <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
+            <TAG>elevation</TAG>
+            <VALUE>${row['elevation']}</VALUE>
+            <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organism count</TAG>
             <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample storage duration</TAG>
             <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'biochemical oxygen demand')">
           <SAMPLE_ATTRIBUTE>
             <TAG>biochemical oxygen demand</TAG>
             <VALUE>${row['biochemical oxygen demand']}</VALUE>
             <UNITS>mg/L (over 5 days at 20C)</UNITS>
@@ -396,21 +305,14 @@
         </py:if>
         <py:if test="attributetest(row, 'host scientific name')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host scientific name</TAG>
             <VALUE>${row['host scientific name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'alkalinity')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>alkalinity</TAG>
-            <VALUE>${row['alkalinity']}</VALUE>
-            <UNITS>mEq/L</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'industrial effluent percent')">
           <SAMPLE_ATTRIBUTE>
             <TAG>industrial effluent percent</TAG>
             <VALUE>${row['industrial effluent percent']}</VALUE>
             <UNITS>%</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
@@ -505,14 +407,21 @@
         <py:if test="attributetest(row, 'nitrate')">
           <SAMPLE_ATTRIBUTE>
             <TAG>nitrate</TAG>
             <VALUE>${row['nitrate']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'total nitrogen concentration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>total nitrogen concentration</TAG>
+            <VALUE>${row['total nitrogen concentration']}</VALUE>
+            <UNITS>µmol/L</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'phosphate')">
           <SAMPLE_ATTRIBUTE>
             <TAG>phosphate</TAG>
             <VALUE>${row['phosphate']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
@@ -526,67 +435,178 @@
         <py:if test="attributetest(row, 'sodium')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sodium</TAG>
             <VALUE>${row['sodium']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'total nitrogen')">
+        <py:if test="attributetest(row, 'total nitrogen content')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>total nitrogen</TAG>
-            <VALUE>${row['total nitrogen']}</VALUE>
+            <TAG>total nitrogen content</TAG>
+            <VALUE>${row['total nitrogen content']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'alkalinity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>alkalinity</TAG>
+            <VALUE>${row['alkalinity']}</VALUE>
+            <UNITS>mEq/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'negative control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'positive control type')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
             <TAG>encoded traits</TAG>
             <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample material processing')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'depth')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000024.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000024.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000024.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000024.xml`

```diff
@@ -26,153 +26,144 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'size-fraction lower threshold')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>size-fraction lower threshold</TAG>
+            <VALUE>${row['size-fraction lower threshold']}</VALUE>
+            <UNITS>µm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'size-fraction upper threshold')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>size-fraction upper threshold</TAG>
+            <VALUE>${row['size-fraction upper threshold']}</VALUE>
+            <UNITS>µm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="attributetest(row, 'density')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>density</TAG>
+            <VALUE>${row['density']}</VALUE>
+            <UNITS>g/m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'estimated size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
@@ -189,26 +180,14 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'altitude')">
@@ -240,21 +219,14 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'depth', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'local environmental context', index)">
@@ -272,122 +244,52 @@
         <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
             <TAG>elevation</TAG>
             <VALUE>${row['elevation']}</VALUE>
             <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'biomass')">
           <SAMPLE_ATTRIBUTE>
             <TAG>biomass</TAG>
             <VALUE>${row['biomass']}</VALUE>
             <UNITS>t</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'density')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>density</TAG>
-            <VALUE>${row['density']}</VALUE>
-            <UNITS>g/m3</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organism count</TAG>
             <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample storage duration</TAG>
             <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host disease status')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host disease status</TAG>
             <VALUE>${row['host disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host scientific name')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host scientific name</TAG>
             <VALUE>${row['host scientific name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'alkalinity')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>alkalinity</TAG>
-            <VALUE>${row['alkalinity']}</VALUE>
-            <UNITS>mEq/L</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'atmospheric data')">
           <SAMPLE_ATTRIBUTE>
             <TAG>atmospheric data</TAG>
             <VALUE>${row['atmospheric data']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'conductivity')">
@@ -462,14 +364,21 @@
         </py:if>
         <py:if test="attributetest(row, 'tidal stage')">
           <SAMPLE_ATTRIBUTE>
             <TAG>tidal stage</TAG>
             <VALUE>${row['tidal stage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'turbidity')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>turbidity</TAG>
+            <VALUE>${row['turbidity']}</VALUE>
+            <UNITS>NTU</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'pH')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pH</TAG>
             <VALUE>${row['pH']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'total depth of water column')">
@@ -656,18 +565,18 @@
         <py:if test="attributetest(row, 'nitrite')">
           <SAMPLE_ATTRIBUTE>
             <TAG>nitrite</TAG>
             <VALUE>${row['nitrite']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nitrogen')">
+        <py:if test="attributetest(row, 'total nitrogen concentration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nitrogen</TAG>
-            <VALUE>${row['nitrogen']}</VALUE>
+            <TAG>total nitrogen concentration</TAG>
+            <VALUE>${row['total nitrogen concentration']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'organic carbon')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organic carbon</TAG>
             <VALUE>${row['organic carbon']}</VALUE>
@@ -810,18 +719,18 @@
         <py:if test="attributetest(row, 'total inorganic nitrogen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>total inorganic nitrogen</TAG>
             <VALUE>${row['total inorganic nitrogen']}</VALUE>
             <UNITS>µg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'total nitrogen')">
+        <py:if test="attributetest(row, 'total nitrogen content')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>total nitrogen</TAG>
-            <VALUE>${row['total nitrogen']}</VALUE>
+            <TAG>total nitrogen content</TAG>
+            <VALUE>${row['total nitrogen content']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'total particulate carbon')">
           <SAMPLE_ATTRIBUTE>
             <TAG>total particulate carbon</TAG>
             <VALUE>${row['total particulate carbon']}</VALUE>
@@ -831,60 +740,178 @@
         <py:if test="attributetest(row, 'total phosphorus')">
           <SAMPLE_ATTRIBUTE>
             <TAG>total phosphorus</TAG>
             <VALUE>${row['total phosphorus']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'alkalinity method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>alkalinity method</TAG>
+            <VALUE>${row['alkalinity method']}</VALUE>
+            <UNITS>m2</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'alkalinity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>alkalinity</TAG>
+            <VALUE>${row['alkalinity']}</VALUE>
+            <UNITS>mEq/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'negative control type')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'positive control type')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
             <TAG>encoded traits</TAG>
             <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample material processing')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'depth', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000025.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000021.xml`

 * *Files 12% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000025.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000021.xml`

```diff
@@ -26,153 +26,142 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'particle classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>particle classification</TAG>
+            <VALUE>${row['particle classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'sediment type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>sediment type</TAG>
+            <VALUE>${row['sediment type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="attributetest(row, 'density')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>density</TAG>
+            <VALUE>${row['density']}</VALUE>
+            <UNITS>g/m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'estimated size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
@@ -189,26 +178,14 @@
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant standard operating procedures</TAG>
             <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'altitude')">
@@ -240,21 +217,14 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'depth')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'local environmental context', index)">
@@ -265,134 +235,71 @@
         </py:if>
         <py:if test="mandatorytest(row, 'environmental medium', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>environmental medium</TAG>
             <VALUE>${row['environmental medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'elevation')">
+        <py:if test="mandatorytest(row, 'elevation', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>elevation</TAG>
             <VALUE>${row['elevation']}</VALUE>
             <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'biomass')">
           <SAMPLE_ATTRIBUTE>
             <TAG>biomass</TAG>
             <VALUE>${row['biomass']}</VALUE>
             <UNITS>t</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'density')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>density</TAG>
-            <VALUE>${row['density']}</VALUE>
-            <UNITS>g/m3</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organism count</TAG>
             <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample storage duration</TAG>
             <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host disease status')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host disease status</TAG>
             <VALUE>${row['host disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host scientific name')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host scientific name</TAG>
             <VALUE>${row['host scientific name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'alkalinity')">
+        <py:if test="attributetest(row, 'mean friction velocity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>alkalinity</TAG>
-            <VALUE>${row['alkalinity']}</VALUE>
-            <UNITS>mEq/L</UNITS>
+            <TAG>mean friction velocity</TAG>
+            <VALUE>${row['mean friction velocity']}</VALUE>
+            <UNITS>m/s</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'water current')">
+        <py:if test="attributetest(row, 'mean peak friction velocity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>water current</TAG>
-            <VALUE>${row['water current']}</VALUE>
-            <UNITS>m3/s</UNITS>
+            <TAG>mean peak friction velocity</TAG>
+            <VALUE>${row['mean peak friction velocity']}</VALUE>
+            <UNITS>m/s</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'pressure')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pressure</TAG>
             <VALUE>${row['pressure']}</VALUE>
             <UNITS>bar</UNITS>
@@ -401,41 +308,102 @@
         <py:if test="attributetest(row, 'temperature')">
           <SAMPLE_ATTRIBUTE>
             <TAG>temperature</TAG>
             <VALUE>${row['temperature']}</VALUE>
             <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'tidal stage')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>tidal stage</TAG>
+            <VALUE>${row['tidal stage']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'turbidity')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>turbidity</TAG>
+            <VALUE>${row['turbidity']}</VALUE>
+            <UNITS>NTU</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'pH')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pH</TAG>
             <VALUE>${row['pH']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'total depth of water column')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>total depth of water column</TAG>
+            <VALUE>${row['total depth of water column']}</VALUE>
+            <UNITS>m</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'water content')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>water content</TAG>
+            <VALUE>${row['water content']}</VALUE>
+            <UNITS>g/g</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'alkyl diethers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>alkyl diethers</TAG>
+            <VALUE>${row['alkyl diethers']}</VALUE>
+            <UNITS>µg/L</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'aminopeptidase activity')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>aminopeptidase activity</TAG>
+            <VALUE>${row['aminopeptidase activity']}</VALUE>
+            <UNITS>mol/L/h</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'ammonium')">
           <SAMPLE_ATTRIBUTE>
             <TAG>ammonium</TAG>
             <VALUE>${row['ammonium']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'bacterial carbon production')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>bacterial carbon production</TAG>
+            <VALUE>${row['bacterial carbon production']}</VALUE>
+            <UNITS>ng/h</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'bishomohopanol')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>bishomohopanol</TAG>
+            <VALUE>${row['bishomohopanol']}</VALUE>
+            <UNITS>µg/g</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'bromide')">
           <SAMPLE_ATTRIBUTE>
             <TAG>bromide</TAG>
             <VALUE>${row['bromide']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'calcium')">
           <SAMPLE_ATTRIBUTE>
             <TAG>calcium</TAG>
             <VALUE>${row['calcium']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'carbon/nitrogen ratio')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>carbon/nitrogen ratio</TAG>
+            <VALUE>${row['carbon/nitrogen ratio']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'chloride')">
           <SAMPLE_ATTRIBUTE>
             <TAG>chloride</TAG>
             <VALUE>${row['chloride']}</VALUE>
             <UNITS>mg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
@@ -470,46 +438,81 @@
         <py:if test="attributetest(row, 'dissolved inorganic carbon')">
           <SAMPLE_ATTRIBUTE>
             <TAG>dissolved inorganic carbon</TAG>
             <VALUE>${row['dissolved inorganic carbon']}</VALUE>
             <UNITS>µg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'dissolved organic carbon')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>dissolved organic carbon</TAG>
+            <VALUE>${row['dissolved organic carbon']}</VALUE>
+            <UNITS>µmol/L</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'dissolved organic nitrogen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>dissolved organic nitrogen</TAG>
             <VALUE>${row['dissolved organic nitrogen']}</VALUE>
             <UNITS>µg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'methane')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>methane</TAG>
+            <VALUE>${row['methane']}</VALUE>
+            <UNITS>µM/L</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'dissolved oxygen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>dissolved oxygen</TAG>
             <VALUE>${row['dissolved oxygen']}</VALUE>
             <UNITS>µmol/kg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'glucosidase activity')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>glucosidase activity</TAG>
+            <VALUE>${row['glucosidase activity']}</VALUE>
+            <UNITS>mol/L/h</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'magnesium')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>magnesium</TAG>
+            <VALUE>${row['magnesium']}</VALUE>
+            <UNITS>parts/million</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'n-alkanes')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>n-alkanes</TAG>
+            <VALUE>${row['n-alkanes']}</VALUE>
+            <UNITS>µmol/L</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'nitrate')">
           <SAMPLE_ATTRIBUTE>
             <TAG>nitrate</TAG>
             <VALUE>${row['nitrate']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'nitrite')">
           <SAMPLE_ATTRIBUTE>
             <TAG>nitrite</TAG>
             <VALUE>${row['nitrite']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nitrogen')">
+        <py:if test="attributetest(row, 'total nitrogen concentration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nitrogen</TAG>
-            <VALUE>${row['nitrogen']}</VALUE>
+            <TAG>total nitrogen concentration</TAG>
+            <VALUE>${row['total nitrogen concentration']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'organic carbon')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organic carbon</TAG>
             <VALUE>${row['organic carbon']}</VALUE>
@@ -526,14 +529,35 @@
         <py:if test="attributetest(row, 'organic nitrogen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organic nitrogen</TAG>
             <VALUE>${row['organic nitrogen']}</VALUE>
             <UNITS>µg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'particulate organic carbon')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>particulate organic carbon</TAG>
+            <VALUE>${row['particulate organic carbon']}</VALUE>
+            <UNITS>µg/L</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'petroleum hydrocarbon')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>petroleum hydrocarbon</TAG>
+            <VALUE>${row['petroleum hydrocarbon']}</VALUE>
+            <UNITS>µmol/L</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'phaeopigments')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>phaeopigments</TAG>
+            <VALUE>${row['phaeopigments']}</VALUE>
+            <UNITS>µg/L</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'phosphate')">
           <SAMPLE_ATTRIBUTE>
             <TAG>phosphate</TAG>
             <VALUE>${row['phosphate']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
@@ -547,95 +571,240 @@
         <py:if test="attributetest(row, 'potassium')">
           <SAMPLE_ATTRIBUTE>
             <TAG>potassium</TAG>
             <VALUE>${row['potassium']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'redox potential')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>redox potential</TAG>
+            <VALUE>${row['redox potential']}</VALUE>
+            <UNITS>mV</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'salinity')">
           <SAMPLE_ATTRIBUTE>
             <TAG>salinity</TAG>
             <VALUE>${row['salinity']}</VALUE>
             <UNITS>psu</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'total carbon')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>total carbon</TAG>
+            <VALUE>${row['total carbon']}</VALUE>
+            <UNITS>µg/L</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'silicate')">
           <SAMPLE_ATTRIBUTE>
             <TAG>silicate</TAG>
             <VALUE>${row['silicate']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sodium')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sodium</TAG>
             <VALUE>${row['sodium']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'total organic carbon')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>total organic carbon</TAG>
+            <VALUE>${row['total organic carbon']}</VALUE>
+            <UNITS>g/kg</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sulfate')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sulfate</TAG>
             <VALUE>${row['sulfate']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sulfide')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sulfide</TAG>
             <VALUE>${row['sulfide']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="attributetest(row, 'total nitrogen content')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>total nitrogen content</TAG>
+            <VALUE>${row['total nitrogen content']}</VALUE>
+            <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'alkalinity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>alkalinity</TAG>
+            <VALUE>${row['alkalinity']}</VALUE>
+            <UNITS>mEq/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'perturbation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'negative control type')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'positive control type')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
             <TAG>encoded traits</TAG>
             <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample material processing')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'porosity')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>porosity</TAG>
+            <VALUE>${row['porosity']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'depth', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000027.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000027.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000027.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000027.xml`

```diff
@@ -54,166 +54,136 @@
         <py:if test="attributetest(row, 'Longitude End')">
           <SAMPLE_ATTRIBUTE>
             <TAG>Longitude End</TAG>
             <VALUE>${row['Longitude End']}</VALUE>
             <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'Depth', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>Depth</TAG>
-            <VALUE>${row['Depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'Protocol Label', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>Protocol Label</TAG>
             <VALUE>${row['Protocol Label']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'trophic level')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="attributetest(row, 'propagation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'finishing strategy')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>finishing strategy</TAG>
-            <VALUE>${row['finishing strategy']}</VALUE>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'density')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>density</TAG>
+            <VALUE>${row['density']}</VALUE>
+            <UNITS>g/m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'finishing strategy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>finishing strategy</TAG>
+            <VALUE>${row['finishing strategy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>ploidy</TAG>
+            <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'number of replicons')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>number of replicons</TAG>
+            <VALUE>${row['number of replicons']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'extrachromosomal elements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>extrachromosomal elements</TAG>
+            <VALUE>${row['extrachromosomal elements']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'estimated size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>estimated size</TAG>
+            <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
@@ -284,136 +254,65 @@
         </py:if>
         <py:if test="mandatorytest(row, 'Sampling Platform', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>Sampling Platform</TAG>
             <VALUE>${row['Sampling Platform']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample collection device or method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device or method</TAG>
-            <VALUE>${row['sample collection device or method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'propagation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'biomass')">
           <SAMPLE_ATTRIBUTE>
             <TAG>biomass</TAG>
             <VALUE>${row['biomass']}</VALUE>
             <UNITS>t</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'density')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>density</TAG>
-            <VALUE>${row['density']}</VALUE>
-            <UNITS>g/m3</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'oxygenation status of sample')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>oxygenation status of sample</TAG>
-            <VALUE>${row['oxygenation status of sample']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organism count</TAG>
             <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage duration')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage duration</TAG>
-            <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'Marine Region', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>Marine Region</TAG>
             <VALUE>${row['Marine Region']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'Temperature', index)">
+        <py:if test="mandatorytest(row, 'water temperature', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Temperature</TAG>
-            <VALUE>${row['Temperature']}</VALUE>
+            <TAG>water temperature</TAG>
+            <VALUE>${row['water temperature']}</VALUE>
             <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'Salinity', index)">
+        <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Salinity</TAG>
-            <VALUE>${row['Salinity']}</VALUE>
-            <UNITS>psu</UNITS>
+            <TAG>sample storage duration</TAG>
+            <VALUE>${row['sample storage duration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'specific host')">
           <SAMPLE_ATTRIBUTE>
             <TAG>specific host</TAG>
             <VALUE>${row['specific host']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'health or disease status of specific host')">
           <SAMPLE_ATTRIBUTE>
             <TAG>health or disease status of specific host</TAG>
             <VALUE>${row['health or disease status of specific host']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'alkalinity')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>alkalinity</TAG>
-            <VALUE>${row['alkalinity']}</VALUE>
-            <UNITS>mEq/L</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'atmospheric data')">
           <SAMPLE_ATTRIBUTE>
             <TAG>atmospheric data</TAG>
             <VALUE>${row['atmospheric data']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'conductivity')">
@@ -682,18 +581,18 @@
         <py:if test="attributetest(row, 'nitrite')">
           <SAMPLE_ATTRIBUTE>
             <TAG>nitrite</TAG>
             <VALUE>${row['nitrite']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nitrogen')">
+        <py:if test="attributetest(row, 'total nitrogen concentration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nitrogen</TAG>
-            <VALUE>${row['nitrogen']}</VALUE>
+            <TAG>total nitrogen concentration</TAG>
+            <VALUE>${row['total nitrogen concentration']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'organic carbon')">
           <SAMPLE_ATTRIBUTE>
             <TAG>organic carbon</TAG>
             <VALUE>${row['organic carbon']}</VALUE>
@@ -773,14 +672,21 @@
         <py:if test="attributetest(row, 'redox potential')">
           <SAMPLE_ATTRIBUTE>
             <TAG>redox potential</TAG>
             <VALUE>${row['redox potential']}</VALUE>
             <UNITS>mV</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'salinity')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>salinity</TAG>
+            <VALUE>${row['salinity']}</VALUE>
+            <UNITS>psu</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'silicate')">
           <SAMPLE_ATTRIBUTE>
             <TAG>silicate</TAG>
             <VALUE>${row['silicate']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
@@ -829,18 +735,18 @@
         <py:if test="attributetest(row, 'total inorganic nitrogen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>total inorganic nitrogen</TAG>
             <VALUE>${row['total inorganic nitrogen']}</VALUE>
             <UNITS>µg/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'total nitrogen')">
+        <py:if test="attributetest(row, 'total nitrogen content')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>total nitrogen</TAG>
-            <VALUE>${row['total nitrogen']}</VALUE>
+            <TAG>total nitrogen content</TAG>
+            <VALUE>${row['total nitrogen content']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'total particulate carbon')">
           <SAMPLE_ATTRIBUTE>
             <TAG>total particulate carbon</TAG>
             <VALUE>${row['total particulate carbon']}</VALUE>
@@ -850,66 +756,159 @@
         <py:if test="attributetest(row, 'total phosphorus')">
           <SAMPLE_ATTRIBUTE>
             <TAG>total phosphorus</TAG>
             <VALUE>${row['total phosphorus']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'alkalinity')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>alkalinity</TAG>
+            <VALUE>${row['alkalinity']}</VALUE>
+            <UNITS>mEq/L</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'source material identifiers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'miscellaneous parameter')">
           <SAMPLE_ATTRIBUTE>
             <TAG>miscellaneous parameter</TAG>
             <VALUE>${row['miscellaneous parameter']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'perturbation')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'encoded traits')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>encoded traits</TAG>
+            <VALUE>${row['encoded traits']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
             <TAG>subspecific genetic lineage</TAG>
             <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'annotation source')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'reference for biomaterial')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'encoded traits')">
+        <py:if test="attributetest(row, 'sample material processing')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>encoded traits</TAG>
-            <VALUE>${row['encoded traits']}</VALUE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chemical administration')">
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chemical administration</TAG>
-            <VALUE>${row['chemical administration']}</VALUE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library size')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library reads sequenced')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library vector')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library screening strategy')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'pcr primers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'depth', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chemical administration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chemical administration</TAG>
+            <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000028.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000028.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000029.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000029.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000029.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000029.xml`

```diff
@@ -26,24 +26,24 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="attributetest(row, 'subject exposure')">
+        <py:if test="attributetest(row, 'sample storage conditions')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subject exposure</TAG>
-            <VALUE>${row['subject exposure']}</VALUE>
+            <TAG>sample storage conditions</TAG>
+            <VALUE>${row['sample storage conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subject exposure duration')">
+        <py:if test="attributetest(row, 'subject exposure')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subject exposure duration</TAG>
-            <VALUE>${row['subject exposure duration']}</VALUE>
+            <TAG>subject exposure</TAG>
+            <VALUE>${row['subject exposure']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'travel-relation')">
           <SAMPLE_ATTRIBUTE>
             <TAG>travel-relation</TAG>
             <VALUE>${row['travel-relation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -107,19 +107,19 @@
         </py:if>
         <py:if test="attributetest(row, 'identified_by')">
           <SAMPLE_ATTRIBUTE>
             <TAG>identified_by</TAG>
             <VALUE>${row['identified_by']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'depth')">
+        <py:if test="attributetest(row, 'subject exposure duration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
+            <TAG>subject exposure duration</TAG>
+            <VALUE>${row['subject exposure duration']}</VALUE>
+            <UNITS>year</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
@@ -133,20 +133,14 @@
         </py:if>
         <py:if test="attributetest(row, 'mating_type')">
           <SAMPLE_ATTRIBUTE>
             <TAG>mating_type</TAG>
             <VALUE>${row['mating_type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'genotype')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>genotype</TAG>
-            <VALUE>${row['genotype']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'pathotype')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pathotype</TAG>
             <VALUE>${row['pathotype']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host disease status')">
@@ -212,20 +206,14 @@
         </py:if>
         <py:if test="attributetest(row, 'passage_history')">
           <SAMPLE_ATTRIBUTE>
             <TAG>passage_history</TAG>
             <VALUE>${row['passage_history']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage conditions</TAG>
-            <VALUE>${row['sample storage conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'Is the sequenced pathogen host associated?', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>Is the sequenced pathogen host associated?</TAG>
             <VALUE>${row['Is the sequenced pathogen host associated?']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'bio_material')">
@@ -302,20 +290,33 @@
         </py:if>
         <py:if test="attributetest(row, 'host description')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host description</TAG>
             <VALUE>${row['host description']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'genotype')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>genotype</TAG>
+            <VALUE>${row['genotype']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'isolation source non-host-associated')">
           <SAMPLE_ATTRIBUTE>
             <TAG>isolation source non-host-associated</TAG>
             <VALUE>${row['isolation source non-host-associated']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'depth')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL_VERSION</TAG>
           <VALUE>${tool_version}</VALUE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000030.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000030.xml`

 * *Files 2% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000030.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000030.xml`

```diff
@@ -72,55 +72,56 @@
         <py:if test="attributetest(row, 'Longitude End')">
           <SAMPLE_ATTRIBUTE>
             <TAG>Longitude End</TAG>
             <VALUE>${row['Longitude End']}</VALUE>
             <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'Depth', index)">
+        <py:if test="mandatorytest(row, 'Protocol Label', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Depth</TAG>
-            <VALUE>${row['Depth']}</VALUE>
-            <UNITS>m</UNITS>
+            <TAG>Protocol Label</TAG>
+            <VALUE>${row['Protocol Label']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'Sample Collection Device')">
+        <py:if test="attributetest(row, 'Sample Status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Sample Collection Device</TAG>
-            <VALUE>${row['Sample Collection Device']}</VALUE>
+            <TAG>Sample Status</TAG>
+            <VALUE>${row['Sample Status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'Protocol Label', index)">
+        <py:if test="attributetest(row, 'Last Update Date')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Protocol Label</TAG>
-            <VALUE>${row['Protocol Label']}</VALUE>
+            <TAG>Last Update Date</TAG>
+            <VALUE>${row['Last Update Date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'Size Fraction Lower Threshold')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Size Fraction Lower Threshold</TAG>
-            <VALUE>${row['Size Fraction Lower Threshold']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'Size Fraction Upper Threshold')">
+        <py:if test="attributetest(row, 'sample storage device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Size Fraction Upper Threshold</TAG>
-            <VALUE>${row['Size Fraction Upper Threshold']}</VALUE>
+            <TAG>sample storage device</TAG>
+            <VALUE>${row['sample storage device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'Sample Status')">
+        <py:if test="attributetest(row, 'size-fraction lower threshold')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Sample Status</TAG>
-            <VALUE>${row['Sample Status']}</VALUE>
+            <TAG>size-fraction lower threshold</TAG>
+            <VALUE>${row['size-fraction lower threshold']}</VALUE>
+            <UNITS>µm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'Last Update Date')">
+        <py:if test="attributetest(row, 'size-fraction upper threshold')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Last Update Date</TAG>
-            <VALUE>${row['Last Update Date']}</VALUE>
+            <TAG>size-fraction upper threshold</TAG>
+            <VALUE>${row['size-fraction upper threshold']}</VALUE>
+            <UNITS>µm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>project name</TAG>
             <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -202,18 +203,18 @@
         <py:if test="attributetest(row, 'Nitrate Sensor')">
           <SAMPLE_ATTRIBUTE>
             <TAG>Nitrate Sensor</TAG>
             <VALUE>${row['Nitrate Sensor']}</VALUE>
             <UNITS>µmol/L</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'Temperature', index)">
+        <py:if test="mandatorytest(row, 'water temperature', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Temperature</TAG>
-            <VALUE>${row['Temperature']}</VALUE>
+            <TAG>water temperature</TAG>
+            <VALUE>${row['water temperature']}</VALUE>
             <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'Chlorophyll Sensor')">
           <SAMPLE_ATTRIBUTE>
             <TAG>Chlorophyll Sensor</TAG>
             <VALUE>${row['Chlorophyll Sensor']}</VALUE>
@@ -228,14 +229,21 @@
         </py:if>
         <py:if test="attributetest(row, 'Further Details')">
           <SAMPLE_ATTRIBUTE>
             <TAG>Further Details</TAG>
             <VALUE>${row['Further Details']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'depth')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL_VERSION</TAG>
           <VALUE>${tool_version}</VALUE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000031.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000049.xml`

 * *Files 20% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000031.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000049.xml`

```diff
@@ -26,195 +26,227 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'observed biotic relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'ploidy')">
+        <py:if test="attributetest(row, 'sample collection device')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ploidy</TAG>
-            <VALUE>${row['ploidy']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'number of replicons')">
+        <py:if test="mandatorytest(row, 'metagenomic source', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>number of replicons</TAG>
-            <VALUE>${row['number of replicons']}</VALUE>
+            <TAG>metagenomic source</TAG>
+            <VALUE>${row['metagenomic source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'extrachromosomal elements')">
+        <py:if test="mandatorytest(row, 'sample derived from', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>extrachromosomal elements</TAG>
-            <VALUE>${row['extrachromosomal elements']}</VALUE>
+            <TAG>sample derived from</TAG>
+            <VALUE>${row['sample derived from']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'project name', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'estimated size')">
           <SAMPLE_ATTRIBUTE>
             <TAG>estimated size</TAG>
             <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
+        <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
+            <TAG>multiplex identifiers</TAG>
+            <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
+        <py:if test="attributetest(row, 'relevant electronic resources')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
+            <TAG>relevant electronic resources</TAG>
+            <VALUE>${row['relevant electronic resources']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'relevant standard operating procedures')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>relevant standard operating procedures</TAG>
+            <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'number of standard tRNAs extracted')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>number of standard tRNAs extracted</TAG>
+            <VALUE>${row['number of standard tRNAs extracted']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'feature prediction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>feature prediction</TAG>
+            <VALUE>${row['feature prediction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'similarity search method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>similarity search method</TAG>
+            <VALUE>${row['similarity search method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="attributetest(row, 'tRNA extraction software')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>tRNA extraction software</TAG>
+            <VALUE>${row['tRNA extraction software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'completeness score')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>completeness score</TAG>
+            <VALUE>${row['completeness score']}</VALUE>
+            <UNITS>%</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'completeness software')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>completeness software</TAG>
+            <VALUE>${row['completeness software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'completeness approach')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>completeness approach</TAG>
+            <VALUE>${row['completeness approach']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'target gene')">
+        <py:if test="attributetest(row, 'binning software')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>target gene</TAG>
-            <VALUE>${row['target gene']}</VALUE>
+            <TAG>binning software</TAG>
+            <VALUE>${row['binning software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'target subfragment')">
+        <py:if test="attributetest(row, 'reassembly post binning')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>target subfragment</TAG>
-            <VALUE>${row['target subfragment']}</VALUE>
+            <TAG>reassembly post binning</TAG>
+            <VALUE>${row['reassembly post binning']}</VALUE>
+            <UNITS>Yes</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
+        <py:if test="attributetest(row, 'MAG coverage software')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
+            <TAG>MAG coverage software</TAG>
+            <VALUE>${row['MAG coverage software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'multiplex identifiers')">
+        <py:if test="attributetest(row, 'binning parameters')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>multiplex identifiers</TAG>
-            <VALUE>${row['multiplex identifiers']}</VALUE>
+            <TAG>binning parameters</TAG>
+            <VALUE>${row['binning parameters']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
+        <py:if test="attributetest(row, 'taxonomic identity marker')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
+            <TAG>taxonomic identity marker</TAG>
+            <VALUE>${row['taxonomic identity marker']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr conditions')">
+        <py:if test="mandatorytest(row, 'source of UViGs', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>pcr conditions</TAG>
-            <VALUE>${row['pcr conditions']}</VALUE>
+            <TAG>source of UViGs</TAG>
+            <VALUE>${row['source of UViGs']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
+        <py:if test="mandatorytest(row, 'predicted genome type', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
+            <TAG>predicted genome type</TAG>
+            <VALUE>${row['predicted genome type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sequence quality check')">
+        <py:if test="mandatorytest(row, 'predicted genome structure', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sequence quality check</TAG>
-            <VALUE>${row['sequence quality check']}</VALUE>
+            <TAG>predicted genome structure</TAG>
+            <VALUE>${row['predicted genome structure']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'chimera check software')">
+        <py:if test="mandatorytest(row, 'detection type', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>chimera check software</TAG>
-            <VALUE>${row['chimera check software']}</VALUE>
+            <TAG>detection type</TAG>
+            <VALUE>${row['detection type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relevant electronic resources')">
+        <py:if test="mandatorytest(row, 'viral identification software', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relevant electronic resources</TAG>
-            <VALUE>${row['relevant electronic resources']}</VALUE>
+            <TAG>viral identification software</TAG>
+            <VALUE>${row['viral identification software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relevant standard operating procedures')">
+        <py:if test="attributetest(row, 'OTU classification approach')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relevant standard operating procedures</TAG>
-            <VALUE>${row['relevant standard operating procedures']}</VALUE>
+            <TAG>OTU classification approach</TAG>
+            <VALUE>${row['OTU classification approach']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'OTU sequence comparison approach')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>OTU sequence comparison approach</TAG>
+            <VALUE>${row['OTU sequence comparison approach']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'OTU database')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>OTU database</TAG>
+            <VALUE>${row['OTU database']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'negative control type')">
+        <py:if test="mandatorytest(row, 'UViG assembly quality', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>negative control type</TAG>
-            <VALUE>${row['negative control type']}</VALUE>
+            <TAG>UViG assembly quality</TAG>
+            <VALUE>${row['UViG assembly quality']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'positive control type')">
+        <py:if test="mandatorytest(row, 'isolation_source', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>positive control type</TAG>
-            <VALUE>${row['positive control type']}</VALUE>
+            <TAG>isolation_source</TAG>
+            <VALUE>${row['isolation_source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'altitude')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>altitude</TAG>
+            <VALUE>${row['altitude']}</VALUE>
+            <UNITS>m</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="mandatorytest(row, 'geographic location (country and/or sea)', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (country and/or sea)</TAG>
             <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'geographic location (latitude)', index)">
@@ -251,273 +283,183 @@
         </py:if>
         <py:if test="mandatorytest(row, 'environmental medium', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>environmental medium</TAG>
             <VALUE>${row['environmental medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'surface material')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>surface material</TAG>
-            <VALUE>${row['surface material']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'surface air contaminant')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>surface air contaminant</TAG>
-            <VALUE>${row['surface air contaminant']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'indoor surface')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>indoor surface</TAG>
-            <VALUE>${row['indoor surface']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'indoor space', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>indoor space</TAG>
-            <VALUE>${row['indoor space']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'filter type', index)">
+        <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>filter type</TAG>
-            <VALUE>${row['filter type']}</VALUE>
+            <TAG>elevation</TAG>
+            <VALUE>${row['elevation']}</VALUE>
+            <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'heating and cooling system type', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>heating and cooling system type</TAG>
-            <VALUE>${row['heating and cooling system type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'substructure type')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>substructure type</TAG>
-            <VALUE>${row['substructure type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'light type', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>light type</TAG>
-            <VALUE>${row['light type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'building setting', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>building setting</TAG>
-            <VALUE>${row['building setting']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'building occupancy type', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>building occupancy type</TAG>
-            <VALUE>${row['building occupancy type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'space typical state', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>space typical state</TAG>
-            <VALUE>${row['space typical state']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'typical occupant density', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>typical occupant density</TAG>
-            <VALUE>${row['typical occupant density']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'occupancy at sampling', index)">
+        <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>occupancy at sampling</TAG>
-            <VALUE>${row['occupancy at sampling']}</VALUE>
+            <TAG>amount or size of sample collected</TAG>
+            <VALUE>${row['amount or size of sample collected']}</VALUE>
+            <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'occupant density at sampling', index)">
+        <py:if test="attributetest(row, 'size fraction selected')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>occupant density at sampling</TAG>
-            <VALUE>${row['occupant density at sampling']}</VALUE>
+            <TAG>size fraction selected</TAG>
+            <VALUE>${row['size fraction selected']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'ventilation type', index)">
+        <py:if test="attributetest(row, 'host scientific name')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>ventilation type</TAG>
-            <VALUE>${row['ventilation type']}</VALUE>
+            <TAG>host scientific name</TAG>
+            <VALUE>${row['host scientific name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>source material identifiers</TAG>
             <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
+        <py:if test="attributetest(row, 'host prediction approach')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
+            <TAG>host prediction approach</TAG>
+            <VALUE>${row['host prediction approach']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'propagation')">
+        <py:if test="attributetest(row, 'host prediction estimated accuracy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
+            <TAG>host prediction estimated accuracy</TAG>
+            <VALUE>${row['host prediction estimated accuracy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'amount or size of sample collected')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>amount or size of sample collected</TAG>
-            <VALUE>${row['amount or size of sample collected']}</VALUE>
-            <UNITS>m3</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample size sorting method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample size sorting method</TAG>
-            <VALUE>${row['sample size sorting method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'organism count', index)">
+        <py:if test="attributetest(row, 'experimental factor')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>organism count</TAG>
-            <VALUE>${row['organism count']}</VALUE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
+        <py:if test="attributetest(row, 'annotation source')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host disease status')">
+        <py:if test="attributetest(row, 'reference for biomaterial')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host disease status</TAG>
-            <VALUE>${row['host disease status']}</VALUE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host scientific name')">
+        <py:if test="attributetest(row, 'reference database(s)')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host scientific name</TAG>
-            <VALUE>${row['host scientific name']}</VALUE>
+            <TAG>reference database(s)</TAG>
+            <VALUE>${row['reference database(s)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'relative air humidity', index)">
+        <py:if test="attributetest(row, 'single cell or viral particle lysis approach')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relative air humidity</TAG>
-            <VALUE>${row['relative air humidity']}</VALUE>
-            <UNITS>%</UNITS>
+            <TAG>single cell or viral particle lysis approach</TAG>
+            <VALUE>${row['single cell or viral particle lysis approach']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'absolute air humidity', index)">
+        <py:if test="attributetest(row, 'single cell or viral particle lysis kit protocol')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>absolute air humidity</TAG>
-            <VALUE>${row['absolute air humidity']}</VALUE>
-            <UNITS>kg</UNITS>
+            <TAG>single cell or viral particle lysis kit protocol</TAG>
+            <VALUE>${row['single cell or viral particle lysis kit protocol']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'surface humidity')">
+        <py:if test="attributetest(row, 'sample material processing')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>surface humidity</TAG>
-            <VALUE>${row['surface humidity']}</VALUE>
-            <UNITS>%</UNITS>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'air temperature', index)">
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>air temperature</TAG>
-            <VALUE>${row['air temperature']}</VALUE>
-            <UNITS>ºC</UNITS>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'surface temperature')">
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>surface temperature</TAG>
-            <VALUE>${row['surface temperature']}</VALUE>
-            <UNITS>ºC</UNITS>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'surface moisture')">
+        <py:if test="attributetest(row, 'library size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>surface moisture</TAG>
-            <VALUE>${row['surface moisture']}</VALUE>
-            <UNITS>parts/million</UNITS>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'surface moisture pH')">
+        <py:if test="attributetest(row, 'library reads sequenced')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>surface moisture pH</TAG>
-            <VALUE>${row['surface moisture pH']}</VALUE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'dew point')">
+        <py:if test="attributetest(row, 'library vector')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>dew point</TAG>
-            <VALUE>${row['dew point']}</VALUE>
-            <UNITS>ºC</UNITS>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'carbon dioxide', index)">
+        <py:if test="attributetest(row, 'library screening strategy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>carbon dioxide</TAG>
-            <VALUE>${row['carbon dioxide']}</VALUE>
-            <UNITS>µmol/L</UNITS>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage')">
+        <py:if test="mandatorytest(row, 'assembly software', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage</TAG>
-            <VALUE>${row['subspecific genetic lineage']}</VALUE>
+            <TAG>assembly software</TAG>
+            <VALUE>${row['assembly software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trophic level')">
+        <py:if test="attributetest(row, 'WGA amplification approach')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trophic level</TAG>
-            <VALUE>${row['trophic level']}</VALUE>
+            <TAG>WGA amplification approach</TAG>
+            <VALUE>${row['WGA amplification approach']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'WGA amplification kit')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>WGA amplification kit</TAG>
+            <VALUE>${row['WGA amplification kit']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'sorting technology')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>sorting technology</TAG>
+            <VALUE>${row['sorting technology']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'encoded traits')">
+        <py:if test="mandatorytest(row, 'virus enrichment approach', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>encoded traits</TAG>
-            <VALUE>${row['encoded traits']}</VALUE>
+            <TAG>virus enrichment approach</TAG>
+            <VALUE>${row['virus enrichment approach']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'adapters')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
+        <py:if test="attributetest(row, 'depth')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000032.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000032.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000032.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000032.xml`

```diff
@@ -50,24 +50,24 @@
         </py:if>
         <py:if test="attributetest(row, 'inoculation stock availability')">
           <SAMPLE_ATTRIBUTE>
             <TAG>inoculation stock availability</TAG>
             <VALUE>${row['inoculation stock availability']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subject exposure')">
+        <py:if test="attributetest(row, 'sample storage conditions')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subject exposure</TAG>
-            <VALUE>${row['subject exposure']}</VALUE>
+            <TAG>sample storage conditions</TAG>
+            <VALUE>${row['sample storage conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subject exposure duration')">
+        <py:if test="attributetest(row, 'subject exposure')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subject exposure duration</TAG>
-            <VALUE>${row['subject exposure duration']}</VALUE>
+            <TAG>subject exposure</TAG>
+            <VALUE>${row['subject exposure']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'type exposure')">
           <SAMPLE_ATTRIBUTE>
             <TAG>type exposure</TAG>
             <VALUE>${row['type exposure']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -196,14 +196,21 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'subject exposure duration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>subject exposure duration</TAG>
+            <VALUE>${row['subject exposure duration']}</VALUE>
+            <UNITS>year</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sample capture status')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample capture status</TAG>
             <VALUE>${row['sample capture status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host disease outcome')">
@@ -317,20 +324,14 @@
         </py:if>
         <py:if test="attributetest(row, 'receipt date')">
           <SAMPLE_ATTRIBUTE>
             <TAG>receipt date</TAG>
             <VALUE>${row['receipt date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage conditions</TAG>
-            <VALUE>${row['sample storage conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'definition for seropositive sample')">
           <SAMPLE_ATTRIBUTE>
             <TAG>definition for seropositive sample</TAG>
             <VALUE>${row['definition for seropositive sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'meaning of cut off value')">
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000033.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000033.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000033.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000033.xml`

```diff
@@ -26,24 +26,24 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="attributetest(row, 'subject exposure')">
+        <py:if test="attributetest(row, 'sample storage conditions')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subject exposure</TAG>
-            <VALUE>${row['subject exposure']}</VALUE>
+            <TAG>sample storage conditions</TAG>
+            <VALUE>${row['sample storage conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subject exposure duration')">
+        <py:if test="attributetest(row, 'subject exposure')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subject exposure duration</TAG>
-            <VALUE>${row['subject exposure duration']}</VALUE>
+            <TAG>subject exposure</TAG>
+            <VALUE>${row['subject exposure']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'type exposure')">
           <SAMPLE_ATTRIBUTE>
             <TAG>type exposure</TAG>
             <VALUE>${row['type exposure']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -100,14 +100,21 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'subject exposure duration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>subject exposure duration</TAG>
+            <VALUE>${row['subject exposure duration']}</VALUE>
+            <UNITS>year</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sample capture status')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample capture status</TAG>
             <VALUE>${row['sample capture status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host disease outcome')">
@@ -179,20 +186,14 @@
         </py:if>
         <py:if test="attributetest(row, 'receipt date')">
           <SAMPLE_ATTRIBUTE>
             <TAG>receipt date</TAG>
             <VALUE>${row['receipt date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage conditions</TAG>
-            <VALUE>${row['sample storage conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'definition for seropositive sample')">
           <SAMPLE_ATTRIBUTE>
             <TAG>definition for seropositive sample</TAG>
             <VALUE>${row['definition for seropositive sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'serotype (required for a seropositive sample)')">
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000034.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000034.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000035.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000035.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000035.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000035.xml`

 * *Ordering differences only*

```diff
@@ -56,20 +56,14 @@
         </py:if>
         <py:if test="attributetest(row, 'infect')">
           <SAMPLE_ATTRIBUTE>
             <TAG>infect</TAG>
             <VALUE>${row['infect']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'protocol')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>protocol</TAG>
-            <VALUE>${row['protocol']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'geographic location (country and/or sea)', index)">
@@ -86,44 +80,26 @@
         </py:if>
         <py:if test="attributetest(row, 'initial time point')">
           <SAMPLE_ATTRIBUTE>
             <TAG>initial time point</TAG>
             <VALUE>${row['initial time point']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>growth condition</TAG>
-            <VALUE>${row['growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'genotype')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>genotype</TAG>
-            <VALUE>${row['genotype']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sex')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sex</TAG>
             <VALUE>${row['sex']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'age')">
           <SAMPLE_ATTRIBUTE>
             <TAG>age</TAG>
             <VALUE>${row['age']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'genetic modification')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>genetic modification</TAG>
-            <VALUE>${row['genetic modification']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'phenotype')">
           <SAMPLE_ATTRIBUTE>
             <TAG>phenotype</TAG>
             <VALUE>${row['phenotype']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'cellular component')">
@@ -230,26 +206,50 @@
         </py:if>
         <py:if test="attributetest(row, 'block')">
           <SAMPLE_ATTRIBUTE>
             <TAG>block</TAG>
             <VALUE>${row['block']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'genotype')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>genotype</TAG>
+            <VALUE>${row['genotype']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'genetic modification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>genetic modification</TAG>
+            <VALUE>${row['genetic modification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'protocol')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>protocol</TAG>
+            <VALUE>${row['protocol']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'environmental stress')">
           <SAMPLE_ATTRIBUTE>
             <TAG>environmental stress</TAG>
             <VALUE>${row['environmental stress']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'environmental history')">
           <SAMPLE_ATTRIBUTE>
             <TAG>environmental history</TAG>
             <VALUE>${row['environmental history']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'growth condition')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>growth condition</TAG>
+            <VALUE>${row['growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL_VERSION</TAG>
           <VALUE>${tool_version}</VALUE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000036.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000036.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000036.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000036.xml`

```diff
@@ -26,30 +26,56 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="attributetest(row, 'name of the sampling site')">
+        <py:if test="attributetest(row, 'sample transportation date')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>name of the sampling site</TAG>
-            <VALUE>${row['name of the sampling site']}</VALUE>
+            <TAG>sample transportation date</TAG>
+            <VALUE>${row['sample transportation date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'sample transportation temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>sample transportation temperature</TAG>
+            <VALUE>${row['sample transportation temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'sample transportation time')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>sample transportation time</TAG>
+            <VALUE>${row['sample transportation time']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample storage temperature')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample storage location')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'name of the sampling site')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>name of the sampling site</TAG>
+            <VALUE>${row['name of the sampling site']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'area of sampling site')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>area of sampling site</TAG>
+            <VALUE>${row['area of sampling site']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'investigation type', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>investigation type</TAG>
             <VALUE>${row['investigation type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -95,57 +121,24 @@
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage duration')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage duration</TAG>
-            <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sampling time point')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sampling time point</TAG>
             <VALUE>${row['sampling time point']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample transportation temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample transportation temperature</TAG>
-            <VALUE>${row['sample transportation temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample transportation date')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample transportation date</TAG>
-            <VALUE>${row['sample transportation date']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample transportation time')">
+        <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample transportation time</TAG>
-            <VALUE>${row['sample transportation time']}</VALUE>
+            <TAG>sample storage duration</TAG>
+            <VALUE>${row['sample storage duration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'receipt date')">
           <SAMPLE_ATTRIBUTE>
             <TAG>receipt date</TAG>
             <VALUE>${row['receipt date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -159,32 +152,38 @@
         <py:if test="attributetest(row, 'temperature')">
           <SAMPLE_ATTRIBUTE>
             <TAG>temperature</TAG>
             <VALUE>${row['temperature']}</VALUE>
             <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'area of sampling site')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>area of sampling site</TAG>
-            <VALUE>${row['area of sampling site']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'size of the catchment area')">
           <SAMPLE_ATTRIBUTE>
             <TAG>size of the catchment area</TAG>
             <VALUE>${row['size of the catchment area']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'population size of the catchment area')">
           <SAMPLE_ATTRIBUTE>
             <TAG>population size of the catchment area</TAG>
             <VALUE>${row['population size of the catchment area']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL_VERSION</TAG>
           <VALUE>${tool_version}</VALUE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000037.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000020.xml`

 * *Files 12% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000037.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000020.xml`

```diff
@@ -26,14 +26,105 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
+        <py:if test="attributetest(row, 'trophic level')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>trophic level</TAG>
+            <VALUE>${row['trophic level']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'observed biotic relationship')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>observed biotic relationship</TAG>
+            <VALUE>${row['observed biotic relationship']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'known pathogenicity')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'relationship to oxygen')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'propagation')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>propagation</TAG>
+            <VALUE>${row['propagation']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'observed host symbionts')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>observed host symbionts</TAG>
+            <VALUE>${row['observed host symbionts']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample collection device')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample collection method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample storage temperature')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample storage location')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'growth facility')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>growth facility</TAG>
+            <VALUE>${row['growth facility']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample disease stage')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample disease stage</TAG>
+            <VALUE>${row['sample disease stage']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'oxygenation status of sample')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>oxygenation status of sample</TAG>
+            <VALUE>${row['oxygenation status of sample']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample disease status')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample disease status</TAG>
+            <VALUE>${row['sample disease status']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'project name', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'ploidy')">
           <SAMPLE_ATTRIBUTE>
             <TAG>ploidy</TAG>
             <VALUE>${row['ploidy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'number of replicons')">
@@ -50,25 +141,54 @@
         </py:if>
         <py:if test="attributetest(row, 'estimated size')">
           <SAMPLE_ATTRIBUTE>
             <TAG>estimated size</TAG>
             <VALUE>${row['estimated size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
+        <py:if test="attributetest(row, 'target gene')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>target gene</TAG>
+            <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'collected_by')">
+        <py:if test="attributetest(row, 'target subfragment')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>collected_by</TAG>
-            <VALUE>${row['collected_by']}</VALUE>
+            <TAG>target subfragment</TAG>
+            <VALUE>${row['target subfragment']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'multiplex identifiers')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>multiplex identifiers</TAG>
+            <VALUE>${row['multiplex identifiers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sequence quality check')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequence quality check</TAG>
+            <VALUE>${row['sequence quality check']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'chimera check software')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>chimera check software</TAG>
+            <VALUE>${row['chimera check software']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'relevant electronic resources')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>relevant electronic resources</TAG>
+            <VALUE>${row['relevant electronic resources']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'relevant standard operating procedures')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>relevant standard operating procedures</TAG>
+            <VALUE>${row['relevant standard operating procedures']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -102,396 +222,432 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'identified_by')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>identified_by</TAG>
-            <VALUE>${row['identified_by']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'depth')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'broad-scale environmental context')">
+        <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'local environmental context')">
+        <py:if test="mandatorytest(row, 'local environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>local environmental context</TAG>
             <VALUE>${row['local environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="mandatorytest(row, 'environmental medium', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>environmental medium</TAG>
+            <VALUE>${row['environmental medium']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
             <TAG>elevation</TAG>
             <VALUE>${row['elevation']}</VALUE>
             <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
+        <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
+            <TAG>amount or size of sample collected</TAG>
+            <VALUE>${row['amount or size of sample collected']}</VALUE>
+            <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection device or method')">
+        <py:if test="attributetest(row, 'organism count')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device or method</TAG>
-            <VALUE>${row['sample collection device or method']}</VALUE>
+            <TAG>organism count</TAG>
+            <VALUE>${row['organism count']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
+        <py:if test="attributetest(row, 'sample capture status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
+            <TAG>sample capture status</TAG>
+            <VALUE>${row['sample capture status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'isolation and growth condition', index)">
+        <py:if test="attributetest(row, 'growth habit')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
+            <TAG>growth habit</TAG>
+            <VALUE>${row['growth habit']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'propagation')">
+        <py:if test="attributetest(row, 'plant sex')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>propagation</TAG>
-            <VALUE>${row['propagation']}</VALUE>
+            <TAG>plant sex</TAG>
+            <VALUE>${row['plant sex']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'amount or size of sample collected')">
+        <py:if test="attributetest(row, 'plant structure')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>amount or size of sample collected</TAG>
-            <VALUE>${row['amount or size of sample collected']}</VALUE>
-            <UNITS>m3</UNITS>
+            <TAG>plant structure</TAG>
+            <VALUE>${row['plant structure']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample storage duration</TAG>
             <VALUE>${row['sample storage duration']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'host disease status')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>host disease status</TAG>
+            <VALUE>${row['host disease status']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'host common name')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>host common name</TAG>
+            <VALUE>${row['host common name']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'host age')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>host age</TAG>
+            <VALUE>${row['host age']}</VALUE>
             <UNITS>years</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
+        <py:if test="attributetest(row, 'host taxid')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
+            <TAG>host taxid</TAG>
+            <VALUE>${row['host taxid']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
+        <py:if test="attributetest(row, 'host life stage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
+            <TAG>host life stage</TAG>
+            <VALUE>${row['host life stage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sampling time point')">
+        <py:if test="attributetest(row, 'host height')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sampling time point</TAG>
-            <VALUE>${row['sampling time point']}</VALUE>
+            <TAG>host height</TAG>
+            <VALUE>${row['host height']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'plant structure', index)">
+        <py:if test="attributetest(row, 'host length')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>plant structure</TAG>
-            <VALUE>${row['plant structure']}</VALUE>
+            <TAG>host length</TAG>
+            <VALUE>${row['host length']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'plant developmental stage', index)">
+        <py:if test="attributetest(row, 'plant body site')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>plant developmental stage</TAG>
-            <VALUE>${row['plant developmental stage']}</VALUE>
+            <TAG>plant body site</TAG>
+            <VALUE>${row['plant body site']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sampled age')">
+        <py:if test="attributetest(row, 'host total mass')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sampled age</TAG>
-            <VALUE>${row['sampled age']}</VALUE>
+            <TAG>host total mass</TAG>
+            <VALUE>${row['host total mass']}</VALUE>
+            <UNITS>kg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample phenotype')">
+        <py:if test="attributetest(row, 'host phenotype')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample phenotype</TAG>
-            <VALUE>${row['sample phenotype']}</VALUE>
+            <TAG>host phenotype</TAG>
+            <VALUE>${row['host phenotype']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample health state')">
+        <py:if test="attributetest(row, 'host scientific name')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample health state</TAG>
-            <VALUE>${row['sample health state']}</VALUE>
+            <TAG>host scientific name</TAG>
+            <VALUE>${row['host scientific name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample disease status')">
+        <py:if test="attributetest(row, 'host subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample disease status</TAG>
-            <VALUE>${row['sample disease status']}</VALUE>
+            <TAG>host subspecific genetic lineage</TAG>
+            <VALUE>${row['host subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample disease stage')">
+        <py:if test="attributetest(row, 'climate environment')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample disease stage</TAG>
-            <VALUE>${row['sample disease stage']}</VALUE>
+            <TAG>climate environment</TAG>
+            <VALUE>${row['climate environment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample wet mass')">
+        <py:if test="attributetest(row, 'gaseous environment')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample wet mass</TAG>
-            <VALUE>${row['sample wet mass']}</VALUE>
+            <TAG>gaseous environment</TAG>
+            <VALUE>${row['gaseous environment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample dry mass')">
+        <py:if test="attributetest(row, 'seasonal environment')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample dry mass</TAG>
-            <VALUE>${row['sample dry mass']}</VALUE>
+            <TAG>seasonal environment</TAG>
+            <VALUE>${row['seasonal environment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample height')">
+        <py:if test="attributetest(row, 'temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample height</TAG>
-            <VALUE>${row['sample height']}</VALUE>
+            <TAG>temperature</TAG>
+            <VALUE>${row['temperature']}</VALUE>
+            <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample length')">
+        <py:if test="attributetest(row, 'salinity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample length</TAG>
-            <VALUE>${row['sample length']}</VALUE>
+            <TAG>salinity</TAG>
+            <VALUE>${row['salinity']}</VALUE>
+            <UNITS>psu</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'growth facility')">
+        <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>growth facility</TAG>
-            <VALUE>${row['growth facility']}</VALUE>
+            <TAG>source material identifiers</TAG>
+            <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample capture status')">
+        <py:if test="attributetest(row, 'host genotype')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample capture status</TAG>
-            <VALUE>${row['sample capture status']}</VALUE>
+            <TAG>host genotype</TAG>
+            <VALUE>${row['host genotype']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'genotype')">
+        <py:if test="attributetest(row, 'host dry mass')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>genotype</TAG>
-            <VALUE>${row['genotype']}</VALUE>
+            <TAG>host dry mass</TAG>
+            <VALUE>${row['host dry mass']}</VALUE>
+            <UNITS>mg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'genetic modification')">
+        <py:if test="attributetest(row, 'host wet mass')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>genetic modification</TAG>
-            <VALUE>${row['genetic modification']}</VALUE>
+            <TAG>host wet mass</TAG>
+            <VALUE>${row['host wet mass']}</VALUE>
+            <UNITS>mg</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'perturbation')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>perturbation</TAG>
+            <VALUE>${row['perturbation']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'negative control type')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>negative control type</TAG>
+            <VALUE>${row['negative control type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'organism common name')">
+        <py:if test="attributetest(row, 'positive control type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>organism common name</TAG>
-            <VALUE>${row['organism common name']}</VALUE>
+            <TAG>positive control type</TAG>
+            <VALUE>${row['positive control type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage rank')">
+        <py:if test="attributetest(row, 'experimental factor')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage rank</TAG>
-            <VALUE>${row['subspecific genetic lineage rank']}</VALUE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subspecific genetic lineage name')">
+        <py:if test="attributetest(row, 'encoded traits')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subspecific genetic lineage name</TAG>
-            <VALUE>${row['subspecific genetic lineage name']}</VALUE>
+            <TAG>encoded traits</TAG>
+            <VALUE>${row['encoded traits']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'biological status')">
+        <py:if test="attributetest(row, 'genetic modification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>biological status</TAG>
-            <VALUE>${row['biological status']}</VALUE>
+            <TAG>genetic modification</TAG>
+            <VALUE>${row['genetic modification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'organism phenotype')">
+        <py:if test="attributetest(row, 'subspecific genetic lineage')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>organism phenotype</TAG>
-            <VALUE>${row['organism phenotype']}</VALUE>
+            <TAG>subspecific genetic lineage</TAG>
+            <VALUE>${row['subspecific genetic lineage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'ancestral data')">
           <SAMPLE_ATTRIBUTE>
             <TAG>ancestral data</TAG>
             <VALUE>${row['ancestral data']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material description')">
+        <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>source material description</TAG>
-            <VALUE>${row['source material description']}</VALUE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'biotic relationship')">
+        <py:if test="attributetest(row, 'plant growth medium')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>biotic relationship</TAG>
-            <VALUE>${row['biotic relationship']}</VALUE>
+            <TAG>plant growth medium</TAG>
+            <VALUE>${row['plant growth medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'growth habit')">
+        <py:if test="attributetest(row, 'rooting conditions')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>growth habit</TAG>
-            <VALUE>${row['growth habit']}</VALUE>
+            <TAG>rooting conditions</TAG>
+            <VALUE>${row['rooting conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'plant sex')">
+        <py:if test="attributetest(row, 'culture rooting medium')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>plant sex</TAG>
-            <VALUE>${row['plant sex']}</VALUE>
+            <TAG>culture rooting medium</TAG>
+            <VALUE>${row['culture rooting medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'climate environment')">
+        <py:if test="attributetest(row, 'rooting medium macronutrients')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>climate environment</TAG>
-            <VALUE>${row['climate environment']}</VALUE>
+            <TAG>rooting medium macronutrients</TAG>
+            <VALUE>${row['rooting medium macronutrients']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'gaseous environment')">
+        <py:if test="attributetest(row, 'rooting medium micronutrients')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>gaseous environment</TAG>
-            <VALUE>${row['gaseous environment']}</VALUE>
+            <TAG>rooting medium micronutrients</TAG>
+            <VALUE>${row['rooting medium micronutrients']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'seasonal environment')">
+        <py:if test="attributetest(row, 'rooting medium organic supplements')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>seasonal environment</TAG>
-            <VALUE>${row['seasonal environment']}</VALUE>
+            <TAG>rooting medium organic supplements</TAG>
+            <VALUE>${row['rooting medium organic supplements']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'soil_taxonomic/FAO classification')">
+        <py:if test="attributetest(row, 'rooting medium carbon')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>soil_taxonomic/FAO classification</TAG>
-            <VALUE>${row['soil_taxonomic/FAO classification']}</VALUE>
+            <TAG>rooting medium carbon</TAG>
+            <VALUE>${row['rooting medium carbon']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'soil_taxonomic/local classification')">
+        <py:if test="attributetest(row, 'rooting medium regulators')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>soil_taxonomic/local classification</TAG>
-            <VALUE>${row['soil_taxonomic/local classification']}</VALUE>
+            <TAG>rooting medium regulators</TAG>
+            <VALUE>${row['rooting medium regulators']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'soil_taxonomic/local classification method')">
+        <py:if test="attributetest(row, 'rooting medium solidifier')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>soil_taxonomic/local classification method</TAG>
-            <VALUE>${row['soil_taxonomic/local classification method']}</VALUE>
+            <TAG>rooting medium solidifier</TAG>
+            <VALUE>${row['rooting medium solidifier']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'soil type')">
+        <py:if test="attributetest(row, 'rooting medium pH')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>soil type</TAG>
-            <VALUE>${row['soil type']}</VALUE>
+            <TAG>rooting medium pH</TAG>
+            <VALUE>${row['rooting medium pH']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'soil type method')">
+        <py:if test="attributetest(row, 'isolation and growth condition')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>soil type method</TAG>
-            <VALUE>${row['soil type method']}</VALUE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'drainage classification')">
+        <py:if test="attributetest(row, 'annotation source')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>drainage classification</TAG>
-            <VALUE>${row['drainage classification']}</VALUE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'soil texture measurement')">
+        <py:if test="attributetest(row, 'reference for biomaterial')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>soil texture measurement</TAG>
-            <VALUE>${row['soil texture measurement']}</VALUE>
-            <UNITS>% sand/silt/clay</UNITS>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'soil texture method')">
+        <py:if test="attributetest(row, 'sample material processing')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>soil texture method</TAG>
-            <VALUE>${row['soil texture method']}</VALUE>
+            <TAG>sample material processing</TAG>
+            <VALUE>${row['sample material processing']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'soil water content')">
+        <py:if test="attributetest(row, 'sample volume or weight for DNA extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>soil water content</TAG>
-            <VALUE>${row['soil water content']}</VALUE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'soil pH')">
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>soil pH</TAG>
-            <VALUE>${row['soil pH']}</VALUE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'plant growth medium', index)">
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>plant growth medium</TAG>
-            <VALUE>${row['plant growth medium']}</VALUE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'rooting conditions')">
+        <py:if test="attributetest(row, 'library size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>rooting conditions</TAG>
-            <VALUE>${row['rooting conditions']}</VALUE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'culture rooting medium')">
+        <py:if test="attributetest(row, 'library reads sequenced')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>culture rooting medium</TAG>
-            <VALUE>${row['culture rooting medium']}</VALUE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'rooting medium macronutrients')">
+        <py:if test="attributetest(row, 'library construction method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>rooting medium macronutrients</TAG>
-            <VALUE>${row['rooting medium macronutrients']}</VALUE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'rooting medium micronutrients')">
+        <py:if test="attributetest(row, 'library vector')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>rooting medium micronutrients</TAG>
-            <VALUE>${row['rooting medium micronutrients']}</VALUE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'rooting medium organic supplements')">
+        <py:if test="attributetest(row, 'library screening strategy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>rooting medium organic supplements</TAG>
-            <VALUE>${row['rooting medium organic supplements']}</VALUE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'rooting medium carbon')">
+        <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>rooting medium carbon</TAG>
-            <VALUE>${row['rooting medium carbon']}</VALUE>
+            <TAG>pcr conditions</TAG>
+            <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'rooting medium regulators')">
+        <py:if test="attributetest(row, 'pcr primers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>rooting medium regulators</TAG>
-            <VALUE>${row['rooting medium regulators']}</VALUE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'rooting medium solidifier')">
+        <py:if test="attributetest(row, 'adapters')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>rooting medium solidifier</TAG>
-            <VALUE>${row['rooting medium solidifier']}</VALUE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'rooting medium pH')">
+        <py:if test="attributetest(row, 'plant product')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>rooting medium pH</TAG>
-            <VALUE>${row['rooting medium pH']}</VALUE>
+            <TAG>plant product</TAG>
+            <VALUE>${row['plant product']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'depth')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'air temperature regimen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>air temperature regimen</TAG>
             <VALUE>${row['air temperature regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -504,18 +660,18 @@
         </py:if>
         <py:if test="attributetest(row, 'chemical mutagen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>chemical mutagen</TAG>
             <VALUE>${row['chemical mutagen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'fertilizer regimen')">
+        <py:if test="attributetest(row, 'fertilizer administration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>fertilizer regimen</TAG>
-            <VALUE>${row['fertilizer regimen']}</VALUE>
+            <TAG>fertilizer administration</TAG>
+            <VALUE>${row['fertilizer administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'fungicide regimen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>fungicide regimen</TAG>
             <VALUE>${row['fungicide regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -528,14 +684,20 @@
         </py:if>
         <py:if test="attributetest(row, 'growth hormone regimen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>growth hormone regimen</TAG>
             <VALUE>${row['growth hormone regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'growth media')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>growth media</TAG>
+            <VALUE>${row['growth media']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'herbicide regimen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>herbicide regimen</TAG>
             <VALUE>${row['herbicide regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'humidity regimen')">
@@ -588,32 +750,32 @@
         </py:if>
         <py:if test="attributetest(row, 'standing water regimen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>standing water regimen</TAG>
             <VALUE>${row['standing water regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'tissue culture growth media')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>tissue culture growth media</TAG>
+            <VALUE>${row['tissue culture growth media']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'watering regimen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>watering regimen</TAG>
             <VALUE>${row['watering regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'water temperature regimen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>water temperature regimen</TAG>
             <VALUE>${row['water temperature regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'plant treatment')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>plant treatment</TAG>
-            <VALUE>${row['plant treatment']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'light regimen')">
           <SAMPLE_ATTRIBUTE>
             <TAG>light regimen</TAG>
             <VALUE>${row['light regimen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'biotic regimen')">
@@ -630,20 +792,14 @@
         </py:if>
         <py:if test="attributetest(row, 'chemical administration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>chemical administration</TAG>
             <VALUE>${row['chemical administration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'perturbation')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>perturbation</TAG>
-            <VALUE>${row['perturbation']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL_VERSION</TAG>
           <VALUE>${tool_version}</VALUE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000038.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000038.xml`

 * *Files 3% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000038.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000038.xml`

```diff
@@ -40,31 +40,77 @@
         <py:if test="mandatorytest(row, 'Longitude Start', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>Longitude Start</TAG>
             <VALUE>${row['Longitude Start']}</VALUE>
             <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'Depth', index)">
+        <py:if test="mandatorytest(row, 'Protocol Label', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Depth</TAG>
-            <VALUE>${row['Depth']}</VALUE>
-            <UNITS>m</UNITS>
+            <TAG>Protocol Label</TAG>
+            <VALUE>${row['Protocol Label']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'Sample Collection Device')">
+        <py:if test="attributetest(row, 'sample storage conditions')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Sample Collection Device</TAG>
-            <VALUE>${row['Sample Collection Device']}</VALUE>
+            <TAG>sample storage conditions</TAG>
+            <VALUE>${row['sample storage conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'Protocol Label', index)">
+        <py:if test="mandatorytest(row, 'aquaculture origin', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Protocol Label</TAG>
-            <VALUE>${row['Protocol Label']}</VALUE>
+            <TAG>aquaculture origin</TAG>
+            <VALUE>${row['aquaculture origin']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'shellfish total weight', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>shellfish total weight</TAG>
+            <VALUE>${row['shellfish total weight']}</VALUE>
+            <UNITS>g</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'shellfish soft tissue weight', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>shellfish soft tissue weight</TAG>
+            <VALUE>${row['shellfish soft tissue weight']}</VALUE>
+            <UNITS>g</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'shell length', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>shell length</TAG>
+            <VALUE>${row['shell length']}</VALUE>
+            <UNITS>g</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'shell width', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>shell width</TAG>
+            <VALUE>${row['shell width']}</VALUE>
+            <UNITS>g</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'shell markings')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>shell markings</TAG>
+            <VALUE>${row['shell markings']}</VALUE>
+            <UNITS>g</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample health state')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample health state</TAG>
+            <VALUE>${row['sample health state']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample disease status')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample disease status</TAG>
+            <VALUE>${row['sample disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -107,32 +153,14 @@
         </py:if>
         <py:if test="mandatorytest(row, 'Sampling Platform', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>Sampling Platform</TAG>
             <VALUE>${row['Sampling Platform']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'storage conditions (fresh/frozen/other)')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>storage conditions (fresh/frozen/other)</TAG>
-            <VALUE>${row['storage conditions (fresh/frozen/other)']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample health state')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample health state</TAG>
-            <VALUE>${row['sample health state']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample disease status')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample disease status</TAG>
-            <VALUE>${row['sample disease status']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'Marine Region')">
           <SAMPLE_ATTRIBUTE>
             <TAG>Marine Region</TAG>
             <VALUE>${row['Marine Region']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'seabed habitat', index)">
@@ -143,69 +171,28 @@
         </py:if>
         <py:if test="mandatorytest(row, 'age', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>age</TAG>
             <VALUE>${row['age']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'aquaculture origin', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>aquaculture origin</TAG>
-            <VALUE>${row['aquaculture origin']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'shellfish total weight', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>shellfish total weight</TAG>
-            <VALUE>${row['shellfish total weight']}</VALUE>
-            <UNITS>g</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'shellfish soft tissue weight', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>shellfish soft tissue weight</TAG>
-            <VALUE>${row['shellfish soft tissue weight']}</VALUE>
-            <UNITS>g</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'shell length', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>shell length</TAG>
-            <VALUE>${row['shell length']}</VALUE>
-            <UNITS>g</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'shell width', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>shell width</TAG>
-            <VALUE>${row['shell width']}</VALUE>
-            <UNITS>g</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'adductor weight')">
           <SAMPLE_ATTRIBUTE>
             <TAG>adductor weight</TAG>
             <VALUE>${row['adductor weight']}</VALUE>
             <UNITS>g</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'gonad weight')">
           <SAMPLE_ATTRIBUTE>
             <TAG>gonad weight</TAG>
             <VALUE>${row['gonad weight']}</VALUE>
             <UNITS>g</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'shell markings')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>shell markings</TAG>
-            <VALUE>${row['shell markings']}</VALUE>
-            <UNITS>g</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'toxin burden')">
           <SAMPLE_ATTRIBUTE>
             <TAG>toxin burden</TAG>
             <VALUE>${row['toxin burden']}</VALUE>
             <UNITS>mg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
@@ -217,14 +204,21 @@
         </py:if>
         <py:if test="attributetest(row, 'chemical compound')">
           <SAMPLE_ATTRIBUTE>
             <TAG>chemical compound</TAG>
             <VALUE>${row['chemical compound']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="mandatorytest(row, 'depth', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL_VERSION</TAG>
           <VALUE>${tool_version}</VALUE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000039.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000039.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000039.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000039.xml`

```diff
@@ -32,24 +32,30 @@
       <SAMPLE_ATTRIBUTES>
         <py:if test="mandatorytest(row, 'dev_stage', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>dev_stage</TAG>
             <VALUE>${row['dev_stage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subject exposure')">
+        <py:if test="attributetest(row, 'known pathogenicity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subject exposure</TAG>
-            <VALUE>${row['subject exposure']}</VALUE>
+            <TAG>known pathogenicity</TAG>
+            <VALUE>${row['known pathogenicity']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subject exposure duration')">
+        <py:if test="attributetest(row, 'sample storage conditions')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>subject exposure duration</TAG>
-            <VALUE>${row['subject exposure duration']}</VALUE>
+            <TAG>sample storage conditions</TAG>
+            <VALUE>${row['sample storage conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'subject exposure')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>subject exposure</TAG>
+            <VALUE>${row['subject exposure']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'travel-relation')">
           <SAMPLE_ATTRIBUTE>
             <TAG>travel-relation</TAG>
             <VALUE>${row['travel-relation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -94,18 +100,19 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'genotype')">
+        <py:if test="attributetest(row, 'subject exposure duration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>genotype</TAG>
-            <VALUE>${row['genotype']}</VALUE>
+            <TAG>subject exposure duration</TAG>
+            <VALUE>${row['subject exposure duration']}</VALUE>
+            <UNITS>year</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host disease outcome')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host disease outcome</TAG>
             <VALUE>${row['host disease outcome']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -155,20 +162,14 @@
         </py:if>
         <py:if test="mandatorytest(row, 'collecting institution', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collecting institution</TAG>
             <VALUE>${row['collecting institution']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage conditions')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage conditions</TAG>
-            <VALUE>${row['sample storage conditions']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'isolate', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>isolate</TAG>
             <VALUE>${row['isolate']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'strain')">
@@ -185,18 +186,18 @@
         </py:if>
         <py:if test="attributetest(row, 'diagnostic method')">
           <SAMPLE_ATTRIBUTE>
             <TAG>diagnostic method</TAG>
             <VALUE>${row['diagnostic method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'genotype')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>genotype</TAG>
+            <VALUE>${row['genotype']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'isolation source non-host-associated')">
           <SAMPLE_ATTRIBUTE>
             <TAG>isolation source non-host-associated</TAG>
             <VALUE>${row['isolation source non-host-associated']}</VALUE>
           </SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000040.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000040.xml`

 * *Files 8% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000040.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000040.xml`

```diff
@@ -26,44 +26,46 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="attributetest(row, 'Size Fraction Lower Threshold')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Size Fraction Lower Threshold</TAG>
-            <VALUE>${row['Size Fraction Lower Threshold']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'Size Fraction Upper Threshold')">
+        <py:if test="attributetest(row, 'size-fraction lower threshold')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Size Fraction Upper Threshold</TAG>
-            <VALUE>${row['Size Fraction Upper Threshold']}</VALUE>
+            <TAG>size-fraction lower threshold</TAG>
+            <VALUE>${row['size-fraction lower threshold']}</VALUE>
+            <UNITS>µm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'size-fraction upper threshold')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>size-fraction upper threshold</TAG>
+            <VALUE>${row['size-fraction upper threshold']}</VALUE>
+            <UNITS>µm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'target gene', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>target gene</TAG>
             <VALUE>${row['target gene']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'target subfragment', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>target subfragment</TAG>
             <VALUE>${row['target subfragment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'pcr primers', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'isolation_source')">
           <SAMPLE_ATTRIBUTE>
             <TAG>isolation_source</TAG>
             <VALUE>${row['isolation_source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'collected_by')">
@@ -107,21 +109,14 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'depth')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'local environmental context', index)">
@@ -132,39 +127,46 @@
         </py:if>
         <py:if test="mandatorytest(row, 'environmental medium', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>environmental medium</TAG>
             <VALUE>${row['environmental medium']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection device or method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device or method</TAG>
-            <VALUE>${row['sample collection device or method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'environmental_sample', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>environmental_sample</TAG>
             <VALUE>${row['environmental_sample']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'Salinity')">
+        <py:if test="attributetest(row, 'salinity')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Salinity</TAG>
-            <VALUE>${row['Salinity']}</VALUE>
+            <TAG>salinity</TAG>
+            <VALUE>${row['salinity']}</VALUE>
             <UNITS>psu</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'Further Details')">
           <SAMPLE_ATTRIBUTE>
             <TAG>Further Details</TAG>
             <VALUE>${row['Further Details']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="mandatorytest(row, 'pcr primers', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'depth')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL_VERSION</TAG>
           <VALUE>${tool_version}</VALUE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000041.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000041.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000041.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000041.xml`

```diff
@@ -26,30 +26,44 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'sample transportation date')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>sample transportation date</TAG>
+            <VALUE>${row['sample transportation date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library construction method')">
+        <py:if test="attributetest(row, 'sample transportation temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library construction method</TAG>
-            <VALUE>${row['library construction method']}</VALUE>
+            <TAG>sample transportation temperature</TAG>
+            <VALUE>${row['sample transportation temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'protocol')">
+        <py:if test="attributetest(row, 'sample transportation time')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>protocol</TAG>
-            <VALUE>${row['protocol']}</VALUE>
+            <TAG>sample transportation time</TAG>
+            <VALUE>${row['sample transportation time']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample storage temperature')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample storage location')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'instrument for DNA concentration measurement')">
           <SAMPLE_ATTRIBUTE>
             <TAG>instrument for DNA concentration measurement</TAG>
             <VALUE>${row['instrument for DNA concentration measurement']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -94,57 +108,24 @@
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage duration')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage duration</TAG>
-            <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'sampling time point')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sampling time point</TAG>
             <VALUE>${row['sampling time point']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample transportation temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample transportation temperature</TAG>
-            <VALUE>${row['sample transportation temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample transportation date')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample transportation date</TAG>
-            <VALUE>${row['sample transportation date']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample transportation time')">
+        <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample transportation time</TAG>
-            <VALUE>${row['sample transportation time']}</VALUE>
+            <TAG>sample storage duration</TAG>
+            <VALUE>${row['sample storage duration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'receipt date')">
           <SAMPLE_ATTRIBUTE>
             <TAG>receipt date</TAG>
             <VALUE>${row['receipt date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -169,14 +150,32 @@
         </py:if>
         <py:if test="attributetest(row, 'Further Details')">
           <SAMPLE_ATTRIBUTE>
             <TAG>Further Details</TAG>
             <VALUE>${row['Further Details']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'library construction method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>library construction method</TAG>
+            <VALUE>${row['library construction method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'protocol')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>protocol</TAG>
+            <VALUE>${row['protocol']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL_VERSION</TAG>
           <VALUE>${tool_version}</VALUE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000043.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000043.xml`

 * *Files 2% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000043.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000043.xml`

```diff
@@ -26,19 +26,31 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="attributetest(row, 'Depth')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>Depth</TAG>
-            <VALUE>${row['Depth']}</VALUE>
-            <UNITS>m</UNITS>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample storage conditions')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample storage conditions</TAG>
+            <VALUE>${row['sample storage conditions']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample storage temperature')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'collected_by')">
           <SAMPLE_ATTRIBUTE>
             <TAG>collected_by</TAG>
             <VALUE>${row['collected_by']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -65,71 +77,32 @@
         <py:if test="attributetest(row, 'geographic location (longitude)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (longitude)</TAG>
             <VALUE>${row['geographic location (longitude)']}</VALUE>
             <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection device or method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device or method</TAG>
-            <VALUE>${row['sample collection device or method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'isolation and growth condition')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>isolation and growth condition</TAG>
-            <VALUE>${row['isolation and growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'amount or size of sample collected')">
           <SAMPLE_ATTRIBUTE>
             <TAG>amount or size of sample collected</TAG>
             <VALUE>${row['amount or size of sample collected']}</VALUE>
             <UNITS>m3</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage duration')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage duration</TAG>
-            <VALUE>${row['sample storage duration']}</VALUE>
-            <UNITS>years</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'growth condition')">
+        <py:if test="attributetest(row, 'water temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>growth condition</TAG>
-            <VALUE>${row['growth condition']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'Temperature')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>Temperature</TAG>
-            <VALUE>${row['Temperature']}</VALUE>
+            <TAG>water temperature</TAG>
+            <VALUE>${row['water temperature']}</VALUE>
             <UNITS>ºC</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'Salinity')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>Salinity</TAG>
-            <VALUE>${row['Salinity']}</VALUE>
-            <UNITS>psu</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sample storage conditions')">
+        <py:if test="attributetest(row, 'sample storage duration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage conditions</TAG>
-            <VALUE>${row['sample storage conditions']}</VALUE>
+            <TAG>sample storage duration</TAG>
+            <VALUE>${row['sample storage duration']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'light intensity')">
           <SAMPLE_ATTRIBUTE>
             <TAG>light intensity</TAG>
             <VALUE>${row['light intensity']}</VALUE>
             <UNITS>lux</UNITS>
@@ -137,14 +110,21 @@
         </py:if>
         <py:if test="attributetest(row, 'pH')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pH</TAG>
             <VALUE>${row['pH']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'salinity')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>salinity</TAG>
+            <VALUE>${row['salinity']}</VALUE>
+            <UNITS>psu</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'culture_collection')">
           <SAMPLE_ATTRIBUTE>
             <TAG>culture_collection</TAG>
             <VALUE>${row['culture_collection']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'strain', index)">
@@ -155,14 +135,33 @@
         </py:if>
         <py:if test="attributetest(row, 'Further Details')">
           <SAMPLE_ATTRIBUTE>
             <TAG>Further Details</TAG>
             <VALUE>${row['Further Details']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'isolation and growth condition')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>isolation and growth condition</TAG>
+            <VALUE>${row['isolation and growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'depth')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'growth condition')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>growth condition</TAG>
+            <VALUE>${row['growth condition']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL_VERSION</TAG>
           <VALUE>${tool_version}</VALUE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000044.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000044.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000044.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000044.xml`

```diff
@@ -32,20 +32,14 @@
       <SAMPLE_ATTRIBUTES>
         <py:if test="attributetest(row, 'subject exposure')">
           <SAMPLE_ATTRIBUTE>
             <TAG>subject exposure</TAG>
             <VALUE>${row['subject exposure']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'subject exposure duration')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>subject exposure duration</TAG>
-            <VALUE>${row['subject exposure duration']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'travel-relation')">
           <SAMPLE_ATTRIBUTE>
             <TAG>travel-relation</TAG>
             <VALUE>${row['travel-relation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'clinical setting')">
@@ -80,14 +74,21 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'subject exposure duration')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>subject exposure duration</TAG>
+            <VALUE>${row['subject exposure duration']}</VALUE>
+            <UNITS>year</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'host disease status')">
           <SAMPLE_ATTRIBUTE>
             <TAG>host disease status</TAG>
             <VALUE>${row['host disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'host disease outcome')">
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000045.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000045.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000047.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000047.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000047.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000047.xml`

```diff
@@ -26,92 +26,56 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="mandatorytest(row, 'metagenomic source', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>metagenomic source</TAG>
+            <VALUE>${row['metagenomic source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="mandatorytest(row, 'sample derived from', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>sample derived from</TAG>
+            <VALUE>${row['sample derived from']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'relevant electronic resources')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant electronic resources</TAG>
             <VALUE>${row['relevant electronic resources']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
@@ -122,42 +86,30 @@
         </py:if>
         <py:if test="attributetest(row, 'number of standard tRNAs extracted')">
           <SAMPLE_ATTRIBUTE>
             <TAG>number of standard tRNAs extracted</TAG>
             <VALUE>${row['number of standard tRNAs extracted']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'assembly software')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>assembly software</TAG>
-            <VALUE>${row['assembly software']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'feature prediction')">
           <SAMPLE_ATTRIBUTE>
             <TAG>feature prediction</TAG>
             <VALUE>${row['feature prediction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference database(s)')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>reference database(s)</TAG>
-            <VALUE>${row['reference database(s)']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'similarity search method')">
           <SAMPLE_ATTRIBUTE>
             <TAG>similarity search method</TAG>
             <VALUE>${row['similarity search method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, '16S recovered')">
+        <py:if test="attributetest(row, '16s recovered')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>16S recovered</TAG>
-            <VALUE>${row['16S recovered']}</VALUE>
+            <TAG>16s recovered</TAG>
+            <VALUE>${row['16s recovered']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, '16S recovery software')">
           <SAMPLE_ATTRIBUTE>
             <TAG>16S recovery software</TAG>
             <VALUE>${row['16S recovery software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -245,20 +197,14 @@
         </py:if>
         <py:if test="mandatorytest(row, 'taxonomic identity marker', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>taxonomic identity marker</TAG>
             <VALUE>${row['taxonomic identity marker']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'taxonomic classification')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>taxonomic classification</TAG>
-            <VALUE>${row['taxonomic classification']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'isolation_source', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>isolation_source</TAG>
             <VALUE>${row['isolation_source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
@@ -296,21 +242,14 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'depth')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'local environmental context', index)">
@@ -328,67 +267,122 @@
         <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
             <TAG>elevation</TAG>
             <VALUE>${row['elevation']}</VALUE>
             <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'amount or size of sample collected')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>amount or size of sample collected</TAG>
+            <VALUE>${row['amount or size of sample collected']}</VALUE>
+            <UNITS>m3</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'size fraction selected')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>size fraction selected</TAG>
+            <VALUE>${row['size fraction selected']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>source material identifiers</TAG>
             <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'taxonomic classification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference database(s)')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference database(s)</TAG>
+            <VALUE>${row['reference database(s)']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sample material processing')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample material processing</TAG>
             <VALUE>${row['sample material processing']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'amount or size of sample collected')">
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>amount or size of sample collected</TAG>
-            <VALUE>${row['amount or size of sample collected']}</VALUE>
-            <UNITS>m3</UNITS>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'size fraction selected')">
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>size fraction selected</TAG>
-            <VALUE>${row['size fraction selected']}</VALUE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'sample derived from', index)">
+        <py:if test="attributetest(row, 'library size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample derived from</TAG>
-            <VALUE>${row['sample derived from']}</VALUE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'metagenomic source', index)">
+        <py:if test="attributetest(row, 'library reads sequenced')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>metagenomic source</TAG>
-            <VALUE>${row['metagenomic source']}</VALUE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
+        <py:if test="attributetest(row, 'library vector')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
+        <py:if test="attributetest(row, 'library screening strategy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'assembly software')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>assembly software</TAG>
+            <VALUE>${row['assembly software']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'depth')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000048.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000048.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000048.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000048.xml`

```diff
@@ -26,92 +26,56 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
+        <py:if test="attributetest(row, 'sample collection device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
+            <TAG>sample collection device</TAG>
+            <VALUE>${row['sample collection device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="mandatorytest(row, 'metagenomic source', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>metagenomic source</TAG>
+            <VALUE>${row['metagenomic source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="mandatorytest(row, 'sample derived from', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>sample derived from</TAG>
+            <VALUE>${row['sample derived from']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'relevant electronic resources')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant electronic resources</TAG>
             <VALUE>${row['relevant electronic resources']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
@@ -122,42 +86,30 @@
         </py:if>
         <py:if test="attributetest(row, 'number of standard tRNAs extracted')">
           <SAMPLE_ATTRIBUTE>
             <TAG>number of standard tRNAs extracted</TAG>
             <VALUE>${row['number of standard tRNAs extracted']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'assembly software')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>assembly software</TAG>
-            <VALUE>${row['assembly software']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'feature prediction')">
           <SAMPLE_ATTRIBUTE>
             <TAG>feature prediction</TAG>
             <VALUE>${row['feature prediction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference database(s)')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>reference database(s)</TAG>
-            <VALUE>${row['reference database(s)']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'similarity search method')">
           <SAMPLE_ATTRIBUTE>
             <TAG>similarity search method</TAG>
             <VALUE>${row['similarity search method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, '16S recovered')">
+        <py:if test="attributetest(row, '16s recovered')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>16S recovered</TAG>
-            <VALUE>${row['16S recovered']}</VALUE>
+            <TAG>16s recovered</TAG>
+            <VALUE>${row['16s recovered']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, '16S recovery software')">
           <SAMPLE_ATTRIBUTE>
             <TAG>16S recovery software</TAG>
             <VALUE>${row['16S recovery software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -220,50 +172,14 @@
         </py:if>
         <py:if test="attributetest(row, 'taxonomic identity marker')">
           <SAMPLE_ATTRIBUTE>
             <TAG>taxonomic identity marker</TAG>
             <VALUE>${row['taxonomic identity marker']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'taxonomic classification')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>taxonomic classification</TAG>
-            <VALUE>${row['taxonomic classification']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'sorting technology', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sorting technology</TAG>
-            <VALUE>${row['sorting technology']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'single cell or viral particle lysis approach', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>single cell or viral particle lysis approach</TAG>
-            <VALUE>${row['single cell or viral particle lysis approach']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'single cell or viral particle lysis kit protocol')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>single cell or viral particle lysis kit protocol</TAG>
-            <VALUE>${row['single cell or viral particle lysis kit protocol']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'WGA amplification approach', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>WGA amplification approach</TAG>
-            <VALUE>${row['WGA amplification approach']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'WGA amplification kit')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>WGA amplification kit</TAG>
-            <VALUE>${row['WGA amplification kit']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'isolation_source', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>isolation_source</TAG>
             <VALUE>${row['isolation_source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
@@ -301,21 +217,14 @@
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'depth')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'local environmental context', index)">
@@ -333,67 +242,152 @@
         <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
             <TAG>elevation</TAG>
             <VALUE>${row['elevation']}</VALUE>
             <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'amount or size of sample collected')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>amount or size of sample collected</TAG>
+            <VALUE>${row['amount or size of sample collected']}</VALUE>
+            <UNITS>m3</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'size fraction selected')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>size fraction selected</TAG>
+            <VALUE>${row['size fraction selected']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>source material identifiers</TAG>
             <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'taxonomic classification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'annotation source')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>annotation source</TAG>
+            <VALUE>${row['annotation source']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference database(s)')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference database(s)</TAG>
+            <VALUE>${row['reference database(s)']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'single cell or viral particle lysis approach', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>single cell or viral particle lysis approach</TAG>
+            <VALUE>${row['single cell or viral particle lysis approach']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'single cell or viral particle lysis kit protocol')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>single cell or viral particle lysis kit protocol</TAG>
+            <VALUE>${row['single cell or viral particle lysis kit protocol']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sample material processing')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample material processing</TAG>
             <VALUE>${row['sample material processing']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'amount or size of sample collected')">
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>amount or size of sample collected</TAG>
-            <VALUE>${row['amount or size of sample collected']}</VALUE>
-            <UNITS>m3</UNITS>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'size fraction selected')">
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>size fraction selected</TAG>
-            <VALUE>${row['size fraction selected']}</VALUE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'sample derived from', index)">
+        <py:if test="attributetest(row, 'library size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample derived from</TAG>
-            <VALUE>${row['sample derived from']}</VALUE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'metagenomic source', index)">
+        <py:if test="attributetest(row, 'library reads sequenced')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>metagenomic source</TAG>
-            <VALUE>${row['metagenomic source']}</VALUE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
+        <py:if test="attributetest(row, 'library vector')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
+        <py:if test="attributetest(row, 'library screening strategy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'assembly software')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>assembly software</TAG>
+            <VALUE>${row['assembly software']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'WGA amplification approach', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>WGA amplification approach</TAG>
+            <VALUE>${row['WGA amplification approach']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'WGA amplification kit')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>WGA amplification kit</TAG>
+            <VALUE>${row['WGA amplification kit']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'sorting technology', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sorting technology</TAG>
+            <VALUE>${row['sorting technology']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'adapters')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'depth')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000049.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000050.xml`

 * *Files 16% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000049.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000050.xml`

```diff
@@ -26,98 +26,50 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'relationship to oxygen')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>relationship to oxygen</TAG>
+            <VALUE>${row['relationship to oxygen']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'estimated size')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>estimated size</TAG>
-            <VALUE>${row['estimated size']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'annotation source')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>annotation source</TAG>
-            <VALUE>${row['annotation source']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'library size')">
+        <py:if test="attributetest(row, 'sample collection method')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
+        <py:if test="mandatorytest(row, 'metagenomic source', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
+            <TAG>metagenomic source</TAG>
+            <VALUE>${row['metagenomic source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="mandatorytest(row, 'sample derived from', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>sample derived from</TAG>
+            <VALUE>${row['sample derived from']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'multiplex identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>multiplex identifiers</TAG>
             <VALUE>${row['multiplex identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sequencing method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'relevant electronic resources')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant electronic resources</TAG>
             <VALUE>${row['relevant electronic resources']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
@@ -128,36 +80,24 @@
         </py:if>
         <py:if test="attributetest(row, 'number of standard tRNAs extracted')">
           <SAMPLE_ATTRIBUTE>
             <TAG>number of standard tRNAs extracted</TAG>
             <VALUE>${row['number of standard tRNAs extracted']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'assembly software', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>assembly software</TAG>
-            <VALUE>${row['assembly software']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'feature prediction')">
+        <py:if test="attributetest(row, '16s recovered')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>feature prediction</TAG>
-            <VALUE>${row['feature prediction']}</VALUE>
+            <TAG>16s recovered</TAG>
+            <VALUE>${row['16s recovered']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reference database(s)')">
+        <py:if test="attributetest(row, '16S recovery software')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference database(s)</TAG>
-            <VALUE>${row['reference database(s)']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'similarity search method')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>similarity search method</TAG>
-            <VALUE>${row['similarity search method']}</VALUE>
+            <TAG>16S recovery software</TAG>
+            <VALUE>${row['16S recovery software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'tRNA extraction software')">
           <SAMPLE_ATTRIBUTE>
             <TAG>tRNA extraction software</TAG>
             <VALUE>${row['tRNA extraction software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -177,151 +117,80 @@
         </py:if>
         <py:if test="attributetest(row, 'completeness approach')">
           <SAMPLE_ATTRIBUTE>
             <TAG>completeness approach</TAG>
             <VALUE>${row['completeness approach']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'binning software')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>binning software</TAG>
-            <VALUE>${row['binning software']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'reassembly post binning')">
+        <py:if test="attributetest(row, 'contamination score')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reassembly post binning</TAG>
-            <VALUE>${row['reassembly post binning']}</VALUE>
-            <UNITS>Yes</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'MAG coverage software')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>MAG coverage software</TAG>
-            <VALUE>${row['MAG coverage software']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'binning parameters')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>binning parameters</TAG>
-            <VALUE>${row['binning parameters']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'taxonomic identity marker')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>taxonomic identity marker</TAG>
-            <VALUE>${row['taxonomic identity marker']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'taxonomic classification')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>taxonomic classification</TAG>
-            <VALUE>${row['taxonomic classification']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'sorting technology')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sorting technology</TAG>
-            <VALUE>${row['sorting technology']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'single cell or viral particle lysis approach')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>single cell or viral particle lysis approach</TAG>
-            <VALUE>${row['single cell or viral particle lysis approach']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'single cell or viral particle lysis kit protocol')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>single cell or viral particle lysis kit protocol</TAG>
-            <VALUE>${row['single cell or viral particle lysis kit protocol']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'WGA amplification approach')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>WGA amplification approach</TAG>
-            <VALUE>${row['WGA amplification approach']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'WGA amplification kit')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>WGA amplification kit</TAG>
-            <VALUE>${row['WGA amplification kit']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'source of UViGs', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>source of UViGs</TAG>
-            <VALUE>${row['source of UViGs']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'virus enrichment approach', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>virus enrichment approach</TAG>
-            <VALUE>${row['virus enrichment approach']}</VALUE>
+            <TAG>contamination score</TAG>
+            <VALUE>${row['contamination score']}</VALUE>
+            <UNITS>%</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'predicted genome type', index)">
+        <py:if test="attributetest(row, 'contamination screening input')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>predicted genome type</TAG>
-            <VALUE>${row['predicted genome type']}</VALUE>
+            <TAG>contamination screening input</TAG>
+            <VALUE>${row['contamination screening input']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'predicted genome structure', index)">
+        <py:if test="attributetest(row, 'contamination screening parameters')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>predicted genome structure</TAG>
-            <VALUE>${row['predicted genome structure']}</VALUE>
+            <TAG>contamination screening parameters</TAG>
+            <VALUE>${row['contamination screening parameters']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'detection type', index)">
+        <py:if test="attributetest(row, 'decontamination software')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>detection type</TAG>
-            <VALUE>${row['detection type']}</VALUE>
+            <TAG>decontamination software</TAG>
+            <VALUE>${row['decontamination software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'viral identification software', index)">
+        <py:if test="mandatorytest(row, 'binning software', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>viral identification software</TAG>
-            <VALUE>${row['viral identification software']}</VALUE>
+            <TAG>binning software</TAG>
+            <VALUE>${row['binning software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'OTU classification approach')">
+        <py:if test="attributetest(row, 'reassembly post binning')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>OTU classification approach</TAG>
-            <VALUE>${row['OTU classification approach']}</VALUE>
+            <TAG>reassembly post binning</TAG>
+            <VALUE>${row['reassembly post binning']}</VALUE>
+            <UNITS>Yes</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'OTU sequence comparison approach')">
+        <py:if test="attributetest(row, 'MAG coverage software')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>OTU sequence comparison approach</TAG>
-            <VALUE>${row['OTU sequence comparison approach']}</VALUE>
+            <TAG>MAG coverage software</TAG>
+            <VALUE>${row['MAG coverage software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'OTU database')">
+        <py:if test="attributetest(row, 'assembly quality')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>OTU database</TAG>
-            <VALUE>${row['OTU database']}</VALUE>
+            <TAG>assembly quality</TAG>
+            <VALUE>${row['assembly quality']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host prediction approach')">
+        <py:if test="attributetest(row, 'investigation type')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host prediction approach</TAG>
-            <VALUE>${row['host prediction approach']}</VALUE>
+            <TAG>investigation type</TAG>
+            <VALUE>${row['investigation type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host prediction estimated accuracy')">
+        <py:if test="mandatorytest(row, 'binning parameters', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host prediction estimated accuracy</TAG>
-            <VALUE>${row['host prediction estimated accuracy']}</VALUE>
+            <TAG>binning parameters</TAG>
+            <VALUE>${row['binning parameters']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'UViG assembly quality', index)">
+        <py:if test="attributetest(row, 'taxonomic identity marker')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>UViG assembly quality</TAG>
-            <VALUE>${row['UViG assembly quality']}</VALUE>
+            <TAG>taxonomic identity marker</TAG>
+            <VALUE>${row['taxonomic identity marker']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'isolation_source', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>isolation_source</TAG>
             <VALUE>${row['isolation_source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -355,27 +224,14 @@
         <py:if test="mandatorytest(row, 'geographic location (longitude)', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (longitude)</TAG>
             <VALUE>${row['geographic location (longitude)']}</VALUE>
             <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'geographic location (region and locality)')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>geographic location (region and locality)</TAG>
-            <VALUE>${row['geographic location (region and locality)']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'depth')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>broad-scale environmental context</TAG>
             <VALUE>${row['broad-scale environmental context']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'local environmental context', index)">
@@ -393,79 +249,110 @@
         <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
             <TAG>elevation</TAG>
             <VALUE>${row['elevation']}</VALUE>
             <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'amount or size of sample collected')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>amount or size of sample collected</TAG>
+            <VALUE>${row['amount or size of sample collected']}</VALUE>
+            <UNITS>m3</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'size fraction selected')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>size fraction selected</TAG>
+            <VALUE>${row['size fraction selected']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'source material identifiers')">
           <SAMPLE_ATTRIBUTE>
             <TAG>source material identifiers</TAG>
             <VALUE>${row['source material identifiers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'experimental factor')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>experimental factor</TAG>
+            <VALUE>${row['experimental factor']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'taxonomic classification')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>taxonomic classification</TAG>
+            <VALUE>${row['taxonomic classification']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'reference for biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>reference for biomaterial</TAG>
+            <VALUE>${row['reference for biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sample material processing')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample material processing</TAG>
             <VALUE>${row['sample material processing']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'amount or size of sample collected')">
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>amount or size of sample collected</TAG>
-            <VALUE>${row['amount or size of sample collected']}</VALUE>
-            <UNITS>m3</UNITS>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'size fraction selected')">
+        <py:if test="attributetest(row, 'nucleic acid amplification')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>size fraction selected</TAG>
-            <VALUE>${row['size fraction selected']}</VALUE>
+            <TAG>nucleic acid amplification</TAG>
+            <VALUE>${row['nucleic acid amplification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'sample derived from', index)">
+        <py:if test="attributetest(row, 'library size')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample derived from</TAG>
-            <VALUE>${row['sample derived from']}</VALUE>
+            <TAG>library size</TAG>
+            <VALUE>${row['library size']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'metagenomic source', index)">
+        <py:if test="attributetest(row, 'library reads sequenced')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>metagenomic source</TAG>
-            <VALUE>${row['metagenomic source']}</VALUE>
+            <TAG>library reads sequenced</TAG>
+            <VALUE>${row['library reads sequenced']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection device')">
+        <py:if test="attributetest(row, 'library vector')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device</TAG>
-            <VALUE>${row['sample collection device']}</VALUE>
+            <TAG>library vector</TAG>
+            <VALUE>${row['library vector']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection method')">
+        <py:if test="attributetest(row, 'library screening strategy')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection method</TAG>
-            <VALUE>${row['sample collection method']}</VALUE>
+            <TAG>library screening strategy</TAG>
+            <VALUE>${row['library screening strategy']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host scientific name')">
+        <py:if test="mandatorytest(row, 'assembly software', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host scientific name</TAG>
-            <VALUE>${row['host scientific name']}</VALUE>
+            <TAG>assembly software</TAG>
+            <VALUE>${row['assembly software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'known pathogenicity')">
+        <py:if test="attributetest(row, 'adapters')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>known pathogenicity</TAG>
-            <VALUE>${row['known pathogenicity']}</VALUE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'observed biotic relationship')">
+        <py:if test="attributetest(row, 'depth')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>observed biotic relationship</TAG>
-            <VALUE>${row['observed biotic relationship']}</VALUE>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000050.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000052.xml`

 * *Files 24% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000050.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000052.xml`

```diff
@@ -26,339 +26,227 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'experimental factor')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>experimental factor</TAG>
-            <VALUE>${row['experimental factor']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'reference for biomaterial')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>reference for biomaterial</TAG>
-            <VALUE>${row['reference for biomaterial']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'nucleic acid amplification')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid amplification</TAG>
-            <VALUE>${row['nucleic acid amplification']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'library size')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>library size</TAG>
-            <VALUE>${row['library size']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'library reads sequenced')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>library reads sequenced</TAG>
-            <VALUE>${row['library reads sequenced']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'library vector')">
+        <py:if test="attributetest(row, 'sample storage temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library vector</TAG>
-            <VALUE>${row['library vector']}</VALUE>
+            <TAG>sample storage temperature</TAG>
+            <VALUE>${row['sample storage temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'library screening strategy')">
+        <py:if test="attributetest(row, 'sample storage buffer')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>library screening strategy</TAG>
-            <VALUE>${row['library screening strategy']}</VALUE>
+            <TAG>sample storage buffer</TAG>
+            <VALUE>${row['sample storage buffer']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'multiplex identifiers')">
+        <py:if test="attributetest(row, 'sample storage device')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>multiplex identifiers</TAG>
-            <VALUE>${row['multiplex identifiers']}</VALUE>
+            <TAG>sample storage device</TAG>
+            <VALUE>${row['sample storage device']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
+        <py:if test="attributetest(row, 'sample storage location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
+            <TAG>sample storage location</TAG>
+            <VALUE>${row['sample storage location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'sequencing method', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'relevant electronic resources')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>relevant electronic resources</TAG>
-            <VALUE>${row['relevant electronic resources']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'relevant standard operating procedures')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>relevant standard operating procedures</TAG>
-            <VALUE>${row['relevant standard operating procedures']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'number of standard tRNAs extracted')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>number of standard tRNAs extracted</TAG>
-            <VALUE>${row['number of standard tRNAs extracted']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'assembly software', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>assembly software</TAG>
-            <VALUE>${row['assembly software']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, '16S recovered')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>16S recovered</TAG>
-            <VALUE>${row['16S recovered']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, '16S recovery software')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>16S recovery software</TAG>
-            <VALUE>${row['16S recovery software']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'tRNA extraction software')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>tRNA extraction software</TAG>
-            <VALUE>${row['tRNA extraction software']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'completeness score')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>completeness score</TAG>
-            <VALUE>${row['completeness score']}</VALUE>
-            <UNITS>%</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'completeness software')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>completeness software</TAG>
-            <VALUE>${row['completeness software']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'completeness approach')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>completeness approach</TAG>
-            <VALUE>${row['completeness approach']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'contamination score')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>contamination score</TAG>
-            <VALUE>${row['contamination score']}</VALUE>
-            <UNITS>%</UNITS>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'contamination screening input')">
+        <py:if test="mandatorytest(row, 'project name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>contamination screening input</TAG>
-            <VALUE>${row['contamination screening input']}</VALUE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'contamination screening parameters')">
+        <py:if test="mandatorytest(row, 'reference host genome for decontamination', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>contamination screening parameters</TAG>
-            <VALUE>${row['contamination screening parameters']}</VALUE>
+            <TAG>reference host genome for decontamination</TAG>
+            <VALUE>${row['reference host genome for decontamination']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'decontamination software')">
+        <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>decontamination software</TAG>
-            <VALUE>${row['decontamination software']}</VALUE>
+            <TAG>collection date</TAG>
+            <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'binning software', index)">
+        <py:if test="mandatorytest(row, 'geographic location (country and/or sea)', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>binning software</TAG>
-            <VALUE>${row['binning software']}</VALUE>
+            <TAG>geographic location (country and/or sea)</TAG>
+            <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'reassembly post binning')">
+        <py:if test="attributetest(row, 'geographic location (latitude)')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reassembly post binning</TAG>
-            <VALUE>${row['reassembly post binning']}</VALUE>
-            <UNITS>Yes</UNITS>
+            <TAG>geographic location (latitude)</TAG>
+            <VALUE>${row['geographic location (latitude)']}</VALUE>
+            <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'MAG coverage software')">
+        <py:if test="attributetest(row, 'geographic location (longitude)')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>MAG coverage software</TAG>
-            <VALUE>${row['MAG coverage software']}</VALUE>
+            <TAG>geographic location (longitude)</TAG>
+            <VALUE>${row['geographic location (longitude)']}</VALUE>
+            <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'assembly quality')">
+        <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>assembly quality</TAG>
-            <VALUE>${row['assembly quality']}</VALUE>
+            <TAG>geographic location (region and locality)</TAG>
+            <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'investigation type', index)">
+        <py:if test="attributetest(row, 'trial length')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>investigation type</TAG>
-            <VALUE>${row['investigation type']}</VALUE>
+            <TAG>trial length</TAG>
+            <VALUE>${row['trial length']}</VALUE>
+            <UNITS>years</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'binning parameters', index)">
+        <py:if test="mandatorytest(row, 'trial timepoint', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>binning parameters</TAG>
-            <VALUE>${row['binning parameters']}</VALUE>
+            <TAG>trial timepoint</TAG>
+            <VALUE>${row['trial timepoint']}</VALUE>
+            <UNITS>years</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'taxonomic identity marker')">
+        <py:if test="attributetest(row, 'host disease status')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>taxonomic identity marker</TAG>
-            <VALUE>${row['taxonomic identity marker']}</VALUE>
+            <TAG>host disease status</TAG>
+            <VALUE>${row['host disease status']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'taxonomic classification')">
+        <py:if test="mandatorytest(row, 'host common name', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>taxonomic classification</TAG>
-            <VALUE>${row['taxonomic classification']}</VALUE>
+            <TAG>host common name</TAG>
+            <VALUE>${row['host common name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'isolation_source', index)">
+        <py:if test="mandatorytest(row, 'host subject id', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>isolation_source</TAG>
-            <VALUE>${row['isolation_source']}</VALUE>
+            <TAG>host subject id</TAG>
+            <VALUE>${row['host subject id']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'collection date', index)">
+        <py:if test="mandatorytest(row, 'host taxid', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>collection date</TAG>
-            <VALUE>${row['collection date']}</VALUE>
+            <TAG>host taxid</TAG>
+            <VALUE>${row['host taxid']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'altitude')">
+        <py:if test="mandatorytest(row, 'host body site', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>altitude</TAG>
-            <VALUE>${row['altitude']}</VALUE>
-            <UNITS>m</UNITS>
+            <TAG>host body site</TAG>
+            <VALUE>${row['host body site']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'geographic location (country and/or sea)', index)">
+        <py:if test="attributetest(row, 'host length')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>geographic location (country and/or sea)</TAG>
-            <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
+            <TAG>host length</TAG>
+            <VALUE>${row['host length']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'geographic location (latitude)', index)">
+        <py:if test="attributetest(row, 'host total mass')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>geographic location (latitude)</TAG>
-            <VALUE>${row['geographic location (latitude)']}</VALUE>
-            <UNITS>DD</UNITS>
+            <TAG>host total mass</TAG>
+            <VALUE>${row['host total mass']}</VALUE>
+            <UNITS>kg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'geographic location (longitude)', index)">
+        <py:if test="attributetest(row, 'host sex')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>geographic location (longitude)</TAG>
-            <VALUE>${row['geographic location (longitude)']}</VALUE>
-            <UNITS>DD</UNITS>
+            <TAG>host sex</TAG>
+            <VALUE>${row['host sex']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'depth')">
+        <py:if test="attributetest(row, 'host scientific name')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>depth</TAG>
-            <VALUE>${row['depth']}</VALUE>
-            <UNITS>m</UNITS>
+            <TAG>host scientific name</TAG>
+            <VALUE>${row['host scientific name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'broad-scale environmental context', index)">
+        <py:if test="attributetest(row, 'host breed')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>broad-scale environmental context</TAG>
-            <VALUE>${row['broad-scale environmental context']}</VALUE>
+            <TAG>host breed</TAG>
+            <VALUE>${row['host breed']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'local environmental context', index)">
+        <py:if test="attributetest(row, 'host gutted mass')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>local environmental context</TAG>
-            <VALUE>${row['local environmental context']}</VALUE>
+            <TAG>host gutted mass</TAG>
+            <VALUE>${row['host gutted mass']}</VALUE>
+            <UNITS>kg</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'environmental medium', index)">
+        <py:if test="attributetest(row, 'host diet')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>environmental medium</TAG>
-            <VALUE>${row['environmental medium']}</VALUE>
+            <TAG>host diet</TAG>
+            <VALUE>${row['host diet']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'elevation')">
+        <py:if test="mandatorytest(row, 'host diet treatment', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>elevation</TAG>
-            <VALUE>${row['elevation']}</VALUE>
-            <UNITS>m</UNITS>
+            <TAG>host diet treatment</TAG>
+            <VALUE>${row['host diet treatment']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'source material identifiers')">
+        <py:if test="attributetest(row, 'host diet treatment concentration')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>source material identifiers</TAG>
-            <VALUE>${row['source material identifiers']}</VALUE>
+            <TAG>host diet treatment concentration</TAG>
+            <VALUE>${row['host diet treatment concentration']}</VALUE>
+            <UNITS>% mass</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample collection device or method')">
+        <py:if test="attributetest(row, 'host storage container')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample collection device or method</TAG>
-            <VALUE>${row['sample collection device or method']}</VALUE>
+            <TAG>host storage container</TAG>
+            <VALUE>${row['host storage container']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample material processing')">
+        <py:if test="attributetest(row, 'host storage container pH')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample material processing</TAG>
-            <VALUE>${row['sample material processing']}</VALUE>
+            <TAG>host storage container pH</TAG>
+            <VALUE>${row['host storage container pH']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'amount or size of sample collected')">
+        <py:if test="attributetest(row, 'host storage container temperature')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>amount or size of sample collected</TAG>
-            <VALUE>${row['amount or size of sample collected']}</VALUE>
-            <UNITS>m3</UNITS>
+            <TAG>host storage container temperature</TAG>
+            <VALUE>${row['host storage container temperature']}</VALUE>
+            <UNITS>°C</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'size fraction selected')">
+        <py:if test="mandatorytest(row, 'sample volume or weight for DNA extraction', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>size fraction selected</TAG>
-            <VALUE>${row['size fraction selected']}</VALUE>
+            <TAG>sample volume or weight for DNA extraction</TAG>
+            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
+            <UNITS>ng</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'sample derived from', index)">
+        <py:if test="attributetest(row, 'nucleic acid extraction')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample derived from</TAG>
-            <VALUE>${row['sample derived from']}</VALUE>
+            <TAG>nucleic acid extraction</TAG>
+            <VALUE>${row['nucleic acid extraction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'metagenomic source', index)">
+        <py:if test="attributetest(row, 'pcr primers')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>metagenomic source</TAG>
-            <VALUE>${row['metagenomic source']}</VALUE>
+            <TAG>pcr primers</TAG>
+            <VALUE>${row['pcr primers']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'relationship to oxygen')">
+        <py:if test="attributetest(row, 'adapters')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>relationship to oxygen</TAG>
-            <VALUE>${row['relationship to oxygen']}</VALUE>
+            <TAG>adapters</TAG>
+            <VALUE>${row['adapters']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000051.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000051.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000051.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000051.xml`

 * *Ordering differences only*

```diff
@@ -26,42 +26,54 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'collection date', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>collection date</TAG>
-            <VALUE>${row['collection date']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'geographic location (country and/or sea)', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>geographic location (country and/or sea)</TAG>
-            <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="mandatorytest(row, 'sample origin', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample origin</TAG>
             <VALUE>${row['sample origin']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="mandatorytest(row, 'sample material', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample material</TAG>
+            <VALUE>${row['sample material']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="mandatorytest(row, 'sample taxon name', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>sample taxon name</TAG>
             <VALUE>${row['sample taxon name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'sample material', index)">
+        <py:if test="mandatorytest(row, 'sample unique ID', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample material</TAG>
-            <VALUE>${row['sample material']}</VALUE>
+            <TAG>sample unique ID</TAG>
+            <VALUE>${row['sample unique ID']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'patient tumor type', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>patient tumor type</TAG>
+            <VALUE>${row['patient tumor type']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'collection date', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>collection date</TAG>
+            <VALUE>${row['collection date']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'geographic location (country and/or sea)', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>geographic location (country and/or sea)</TAG>
+            <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'engrafted tumor sample passage', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>engrafted tumor sample passage</TAG>
             <VALUE>${row['engrafted tumor sample passage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -74,26 +86,14 @@
         </py:if>
         <py:if test="mandatorytest(row, 'patient tumor site of collection', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>patient tumor site of collection</TAG>
             <VALUE>${row['patient tumor site of collection']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'patient tumor type', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>patient tumor type</TAG>
-            <VALUE>${row['patient tumor type']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'sample unique ID', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>sample unique ID</TAG>
-            <VALUE>${row['sample unique ID']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'engraftment host strain name')">
           <SAMPLE_ATTRIBUTE>
             <TAG>engraftment host strain name</TAG>
             <VALUE>${row['engraftment host strain name']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'patient age at collection of tumor', index)">
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000052.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000053.xml`

 * *Files 17% similar despite different names*

#### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_samples_ERC000052.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_samples_ERC000053.xml`

```diff
@@ -26,55 +26,118 @@
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <py:if test="attributetest(row, 'sample_description')">
         <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       </py:if>
       <SAMPLE_ATTRIBUTES>
-        <py:if test="mandatorytest(row, 'project name', index)">
+        <py:if test="attributetest(row, 'Latitude Start')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>project name</TAG>
-            <VALUE>${row['project name']}</VALUE>
+            <TAG>Latitude Start</TAG>
+            <VALUE>${row['Latitude Start']}</VALUE>
+            <UNITS>DD</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'Longitude Start')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>Longitude Start</TAG>
+            <VALUE>${row['Longitude Start']}</VALUE>
+            <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'sample volume or weight for DNA extraction', index)">
+        <py:if test="attributetest(row, 'Latitude End')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample volume or weight for DNA extraction</TAG>
-            <VALUE>${row['sample volume or weight for DNA extraction']}</VALUE>
-            <UNITS>ng</UNITS>
+            <TAG>Latitude End</TAG>
+            <VALUE>${row['Latitude End']}</VALUE>
+            <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'nucleic acid extraction')">
+        <py:if test="attributetest(row, 'Longitude End')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>nucleic acid extraction</TAG>
-            <VALUE>${row['nucleic acid extraction']}</VALUE>
+            <TAG>Longitude End</TAG>
+            <VALUE>${row['Longitude End']}</VALUE>
+            <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'pcr primers')">
+        <py:if test="mandatorytest(row, 'organism part', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>pcr primers</TAG>
-            <VALUE>${row['pcr primers']}</VALUE>
+            <TAG>organism part</TAG>
+            <VALUE>${row['organism part']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'adapters')">
+        <py:if test="mandatorytest(row, 'lifestage', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>adapters</TAG>
-            <VALUE>${row['adapters']}</VALUE>
+            <TAG>lifestage</TAG>
+            <VALUE>${row['lifestage']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'sequencing method', index)">
+        <py:if test="attributetest(row, 'relationship')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sequencing method</TAG>
-            <VALUE>${row['sequencing method']}</VALUE>
+            <TAG>relationship</TAG>
+            <VALUE>${row['relationship']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'reference host genome for decontamination', index)">
+        <py:if test="attributetest(row, 'sample symbiont of')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>reference host genome for decontamination</TAG>
-            <VALUE>${row['reference host genome for decontamination']}</VALUE>
+            <TAG>sample symbiont of</TAG>
+            <VALUE>${row['sample symbiont of']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'symbiont')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>symbiont</TAG>
+            <VALUE>${row['symbiont']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample collection method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample collection method</TAG>
+            <VALUE>${row['sample collection method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample coordinator affiliation')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample coordinator affiliation</TAG>
+            <VALUE>${row['sample coordinator affiliation']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample same as')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample same as</TAG>
+            <VALUE>${row['sample same as']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'sample derived from')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sample derived from</TAG>
+            <VALUE>${row['sample derived from']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'project name', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>project name</TAG>
+            <VALUE>${row['project name']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'barcoding center')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>barcoding center</TAG>
+            <VALUE>${row['barcoding center']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'tolid')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>tolid</TAG>
+            <VALUE>${row['tolid']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="mandatorytest(row, 'collected_by', index)">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>collected_by</TAG>
+            <VALUE>${row['collected_by']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="mandatorytest(row, 'collection date', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>collection date</TAG>
             <VALUE>${row['collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
@@ -95,164 +158,142 @@
         <py:if test="attributetest(row, 'geographic location (longitude)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (longitude)</TAG>
             <VALUE>${row['geographic location (longitude)']}</VALUE>
             <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'geographic location (region and locality)')">
+        <py:if test="mandatorytest(row, 'geographic location (region and locality)', index)">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'trial length')">
+        <py:if test="attributetest(row, 'identified_by')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trial length</TAG>
-            <VALUE>${row['trial length']}</VALUE>
-            <UNITS>years</UNITS>
+            <TAG>identified_by</TAG>
+            <VALUE>${row['identified_by']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'trial timepoint', index)">
+        <py:if test="attributetest(row, 'elevation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>trial timepoint</TAG>
-            <VALUE>${row['trial timepoint']}</VALUE>
-            <UNITS>years</UNITS>
+            <TAG>elevation</TAG>
+            <VALUE>${row['elevation']}</VALUE>
+            <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage temperature')">
+        <py:if test="mandatorytest(row, 'habitat', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage temperature</TAG>
-            <VALUE>${row['sample storage temperature']}</VALUE>
-            <UNITS>°C</UNITS>
+            <TAG>habitat</TAG>
+            <VALUE>${row['habitat']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage location')">
+        <py:if test="attributetest(row, 'identifier_affiliation')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage location</TAG>
-            <VALUE>${row['sample storage location']}</VALUE>
+            <TAG>identifier_affiliation</TAG>
+            <VALUE>${row['identifier_affiliation']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage buffer')">
+        <py:if test="attributetest(row, 'original collection date')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage buffer</TAG>
-            <VALUE>${row['sample storage buffer']}</VALUE>
+            <TAG>original collection date</TAG>
+            <VALUE>${row['original collection date']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'sample storage container')">
+        <py:if test="attributetest(row, 'original geographic location')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>sample storage container</TAG>
-            <VALUE>${row['sample storage container']}</VALUE>
+            <TAG>original geographic location</TAG>
+            <VALUE>${row['original geographic location']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host disease status')">
+        <py:if test="attributetest(row, 'original geographic location (latitude)')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host disease status</TAG>
-            <VALUE>${row['host disease status']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'host common name', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>host common name</TAG>
-            <VALUE>${row['host common name']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'host subject id', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>host subject id</TAG>
-            <VALUE>${row['host subject id']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="mandatorytest(row, 'host taxid', index)">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>host taxid</TAG>
-            <VALUE>${row['host taxid']}</VALUE>
+            <TAG>original geographic location (latitude)</TAG>
+            <VALUE>${row['original geographic location (latitude)']}</VALUE>
+            <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'host body site', index)">
+        <py:if test="attributetest(row, 'original geographic location (longitude)')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host body site</TAG>
-            <VALUE>${row['host body site']}</VALUE>
+            <TAG>original geographic location (longitude)</TAG>
+            <VALUE>${row['original geographic location (longitude)']}</VALUE>
+            <UNITS>DD</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host length')">
+        <py:if test="attributetest(row, 'sample coordinator')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host length</TAG>
-            <VALUE>${row['host length']}</VALUE>
-            <UNITS>mm</UNITS>
+            <TAG>sample coordinator</TAG>
+            <VALUE>${row['sample coordinator']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host total mass')">
+        <py:if test="mandatorytest(row, 'sex', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host total mass</TAG>
-            <VALUE>${row['host total mass']}</VALUE>
-            <UNITS>kg</UNITS>
+            <TAG>sex</TAG>
+            <VALUE>${row['sex']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host sex')">
+        <py:if test="mandatorytest(row, 'collecting institution', index)">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host sex</TAG>
-            <VALUE>${row['host sex']}</VALUE>
+            <TAG>collecting institution</TAG>
+            <VALUE>${row['collecting institution']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host scientific name')">
+        <py:if test="attributetest(row, 'GAL')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host scientific name</TAG>
-            <VALUE>${row['host scientific name']}</VALUE>
+            <TAG>GAL</TAG>
+            <VALUE>${row['GAL']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host breed')">
+        <py:if test="attributetest(row, 'specimen_id')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host breed</TAG>
-            <VALUE>${row['host breed']}</VALUE>
+            <TAG>specimen_id</TAG>
+            <VALUE>${row['specimen_id']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host gutted mass')">
+        <py:if test="attributetest(row, 'GAL_sample_id')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host gutted mass</TAG>
-            <VALUE>${row['host gutted mass']}</VALUE>
-            <UNITS>kg</UNITS>
+            <TAG>GAL_sample_id</TAG>
+            <VALUE>${row['GAL_sample_id']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host diet')">
+        <py:if test="attributetest(row, 'proxy voucher')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host diet</TAG>
-            <VALUE>${row['host diet']}</VALUE>
+            <TAG>proxy voucher</TAG>
+            <VALUE>${row['proxy voucher']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="mandatorytest(row, 'host diet treatment', index)">
+        <py:if test="attributetest(row, 'proxy biomaterial')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host diet treatment</TAG>
-            <VALUE>${row['host diet treatment']}</VALUE>
+            <TAG>proxy biomaterial</TAG>
+            <VALUE>${row['proxy biomaterial']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host diet treatment concentration')">
+        <py:if test="attributetest(row, 'bio_material')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host diet treatment concentration</TAG>
-            <VALUE>${row['host diet treatment concentration']}</VALUE>
-            <UNITS>% mass</UNITS>
+            <TAG>bio_material</TAG>
+            <VALUE>${row['bio_material']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host storage container')">
+        <py:if test="attributetest(row, 'specimen_voucher')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host storage container</TAG>
-            <VALUE>${row['host storage container']}</VALUE>
+            <TAG>specimen_voucher</TAG>
+            <VALUE>${row['specimen_voucher']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host storage container pH')">
+        <py:if test="attributetest(row, 'culture_or_strain_id')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host storage container pH</TAG>
-            <VALUE>${row['host storage container pH']}</VALUE>
+            <TAG>culture_or_strain_id</TAG>
+            <VALUE>${row['culture_or_strain_id']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'host storage container temperature')">
+        <py:if test="attributetest(row, 'depth')">
           <SAMPLE_ATTRIBUTE>
-            <TAG>host storage container temperature</TAG>
-            <VALUE>${row['host storage container temperature']}</VALUE>
-            <UNITS>°C</UNITS>
+            <TAG>depth</TAG>
+            <VALUE>${row['depth']}</VALUE>
+            <UNITS>mm</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>SUBMISSION_TOOL</TAG>
           <VALUE>${tool_name}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_studies.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_studies.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/ENA_template_submission.xml` & `ena_upload_cli-0.7.2/ena_upload/templates/ENA_template_submission.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/SRA.common.xsd` & `ena_upload_cli-0.7.2/ena_upload/templates/SRA.common.xsd`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/SRA.experiment.xsd` & `ena_upload_cli-0.7.2/ena_upload/templates/SRA.experiment.xsd`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/SRA.run.xsd` & `ena_upload_cli-0.7.2/ena_upload/templates/SRA.run.xsd`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/SRA.sample.xsd` & `ena_upload_cli-0.7.2/ena_upload/templates/SRA.sample.xsd`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/SRA.study.xsd` & `ena_upload_cli-0.7.2/ena_upload/templates/SRA.study.xsd`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload/templates/SRA.submission.xsd` & `ena_upload_cli-0.7.2/ena_upload/templates/SRA.submission.xsd`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/ena_upload_cli.egg-info/PKG-INFO` & `ena_upload_cli-0.7.2/ena_upload_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ena-upload-cli
-Version: 0.7.1
+Version: 0.7.2
 Summary: Command Line Interface to upload data to the European Nucleotide Archive
 Home-page: https://github.com/usegalaxy-eu/ena-upload-cli
 Author: Dilmurat Yusuf
 Author-email: bjoern.gruening@gmail.com
 License: MIT
 Keywords: pip,ena-upload-cli,cli,ENA,upload
 Classifier: Operating System :: OS Independent
```

### Comparing `ena-upload-cli-0.7.1/ena_upload_cli.egg-info/SOURCES.txt` & `ena_upload_cli-0.7.2/ena_upload_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,18 @@
 ena_upload/templates/ENA_template_samples_ERC000047.xml
 ena_upload/templates/ENA_template_samples_ERC000048.xml
 ena_upload/templates/ENA_template_samples_ERC000049.xml
 ena_upload/templates/ENA_template_samples_ERC000050.xml
 ena_upload/templates/ENA_template_samples_ERC000051.xml
 ena_upload/templates/ENA_template_samples_ERC000052.xml
 ena_upload/templates/ENA_template_samples_ERC000053.xml
+ena_upload/templates/ENA_template_samples_ERC000055.xml
+ena_upload/templates/ENA_template_samples_ERC000056.xml
+ena_upload/templates/ENA_template_samples_ERC000057.xml
+ena_upload/templates/ENA_template_samples_ERC000058.xml
 ena_upload/templates/ENA_template_studies.xml
 ena_upload/templates/ENA_template_submission.xml
 ena_upload/templates/SRA.common.xsd
 ena_upload/templates/SRA.experiment.xsd
 ena_upload/templates/SRA.run.xsd
 ena_upload/templates/SRA.sample.xsd
 ena_upload/templates/SRA.study.xsd
```

### Comparing `ena-upload-cli-0.7.1/setup.py` & `ena_upload_cli-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.7.1/tests/test_ena_objects.py` & `ena_upload_cli-0.7.2/tests/test_ena_objects.py`

 * *Files identical despite different names*

