# Comparing `tmp/pytest_splunk_addon-5.3.0b1.tar.gz` & `tmp/pytest_splunk_addon-5.3.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_splunk_addon-5.3.0b1.tar", max compression
+gzip compressed data, was "pytest_splunk_addon-5.3.0b2.tar", max compression
```

## Comparing `pytest_splunk_addon-5.3.0b1.tar` & `pytest_splunk_addon-5.3.0b2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0    11341 2024-05-16 10:02:01.376977 pytest_splunk_addon-5.3.0b1/LICENSE
--rw-r--r--   0        0        0     2160 2024-05-16 10:02:56.605110 pytest_splunk_addon-5.3.0b1/pyproject.toml
--rw-r--r--   0        0        0     1886 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/.ignore_splunk_internal_errors
--rw-r--r--   0        0        0      751 2024-05-16 10:02:56.601110 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/__init__.py
--rw-r--r--   0        0        0     5364 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/docker_class.py
--rw-r--r--   0        0        0     8543 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/plugin.py
--rw-r--r--   0        0        0    34181 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/splunk.py
--rw-r--r--   0        0        0      579 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py
--rw-r--r--   0        0        0    46781 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py
--rw-r--r--   0        0        0     1220 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/__init__.py
--rw-r--r--   0        0        0     2791 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_basic.py
--rw-r--r--   0        0        0     3312 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py
--rw-r--r--   0        0        0     2082 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py
--rw-r--r--   0        0        0     3136 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/fields.py
--rw-r--r--   0        0        0    13284 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py
--rw-r--r--   0        0        0     2760 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py
--rw-r--r--   0        0        0     2447 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py
--rw-r--r--   0        0        0     5391 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py
--rw-r--r--   0        0        0     6168 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/app_test_generator.py
--rw-r--r--   0        0        0      754 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py
--rw-r--r--   0        0        0     1251 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py
--rw-r--r--   0        0        0     1130 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py
--rw-r--r--   0        0        0     9586 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py
--rw-r--r--   0        0        0     2351 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py
--rw-r--r--   0        0        0     2801 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py
--rw-r--r--   0        0        0     2442 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py
--rw-r--r--   0        0        0     3553 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json
--rw-r--r--   0        0        0     3699 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json
--rw-r--r--   0        0        0      970 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py
--rw-r--r--   0        0        0     2024 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py
--rw-r--r--   0        0        0     2386 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py
--rw-r--r--   0        0        0     3937 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py
--rw-r--r--   0        0        0     3267 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py
--rw-r--r--   0        0        0     4226 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py
--rw-r--r--   0        0        0     9218 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py
--rw-r--r--   0        0        0     2965 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py
--rw-r--r--   0        0        0    11204 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py
--rw-r--r--   0        0        0    20768 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py
--rw-r--r--   0        0        0     2390 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Alerts.json
--rw-r--r--   0        0        0     5281 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Authentication.json
--rw-r--r--   0        0        0     9626 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Certificates.json
--rw-r--r--   0        0        0     8173 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Change.json
--rw-r--r--   0        0        0     2814 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/DLP.json
--rw-r--r--   0        0        0     8598 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Email.json
--rw-r--r--   0        0        0    18855 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json
--rw-r--r--   0        0        0     9890 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json
--rw-r--r--   0        0        0     4255 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Malware.json
--rw-r--r--   0        0        0     8746 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json
--rw-r--r--   0        0        0     5599 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json
--rw-r--r--   0        0        0    18953 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json
--rw-r--r--   0        0        0     3862 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Updates.json
--rw-r--r--   0        0        0     5184 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json
--rw-r--r--   0        0        0     7178 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Web.json
--rw-r--r--   0        0        0      889 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py
--rw-r--r--   0        0        0      862 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py
--rw-r--r--   0        0        0     7339 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py
--rw-r--r--   0        0        0     5002 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py
--rw-r--r--   0        0        0     4418 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py
--rw-r--r--   0        0        0     4995 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py
--rw-r--r--   0        0        0     3615 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py
--rw-r--r--   0        0        0     3015 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py
--rw-r--r--   0        0        0      812 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py
--rw-r--r--   0        0        0     3305 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py
--rw-r--r--   0        0        0     5420 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py
--rw-r--r--   0        0        0    11040 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py
--rw-r--r--   0        0        0    10360 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py
--rw-r--r--   0        0        0    21984 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py
--rw-r--r--   0        0        0      766 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/__init__.py
--rw-r--r--   0        0        0      711 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py
--rw-r--r--   0        0        0    11987 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py
--rw-r--r--   0        0        0    11457 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py
--rw-r--r--   0        0        0      909 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py
--rw-r--r--   0        0        0     7291 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py
--rw-r--r--   0        0        0    46400 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/rule.py
--rw-r--r--   0        0        0    15413 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py
--rw-r--r--   0        0        0     2290 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py
--rw-r--r--   0        0        0    16792 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py
--rw-r--r--   0        0        0     6032 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py
--rw-r--r--   0        0        0     9990 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd
--rw-r--r--   0        0        0     6217 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py
--rw-r--r--   0        0        0      834 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/__init__.py
--rw-r--r--   0        0        0     4634 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py
--rw-r--r--   0        0        0     1627 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/log_helper.py
--rw-r--r--   0        0        0     3034 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py
--rw-r--r--   0        0        0     3414 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py
--rw-r--r--   0        0        0    17585 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/tools/cim_field_report.py
--rw-r--r--   0        0        0     1427 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.3.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2024-05-27 08:10:07.067065 pytest_splunk_addon-5.3.0b2/LICENSE
+-rw-r--r--   0        0        0     2160 2024-05-27 08:11:05.815477 pytest_splunk_addon-5.3.0b2/pyproject.toml
+-rw-r--r--   0        0        0     1886 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/.ignore_splunk_internal_errors
+-rw-r--r--   0        0        0      751 2024-05-27 08:11:05.811477 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/__init__.py
+-rw-r--r--   0        0        0     5364 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/docker_class.py
+-rw-r--r--   0        0        0     8543 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/plugin.py
+-rw-r--r--   0        0        0    34181 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/splunk.py
+-rw-r--r--   0        0        0      579 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py
+-rw-r--r--   0        0        0    46781 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py
+-rw-r--r--   0        0        0     1220 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/__init__.py
+-rw-r--r--   0        0        0     2791 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_basic.py
+-rw-r--r--   0        0        0     3312 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/__init__.py
+-rw-r--r--   0        0        0     2082 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py
+-rw-r--r--   0        0        0     3136 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/fields.py
+-rw-r--r--   0        0        0    13284 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py
+-rw-r--r--   0        0        0     2760 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py
+-rw-r--r--   0        0        0     2447 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py
+-rw-r--r--   0        0        0     5391 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py
+-rw-r--r--   0        0        0     6168 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/app_test_generator.py
+-rw-r--r--   0        0        0      754 2024-05-27 08:10:07.071065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py
+-rw-r--r--   0        0        0     1130 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py
+-rw-r--r--   0        0        0     9586 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py
+-rw-r--r--   0        0        0     2351 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py
+-rw-r--r--   0        0        0     2801 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py
+-rw-r--r--   0        0        0     2442 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py
+-rw-r--r--   0        0        0     3553 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json
+-rw-r--r--   0        0        0     3699 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json
+-rw-r--r--   0        0        0      970 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/__init__.py
+-rw-r--r--   0        0        0     2024 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py
+-rw-r--r--   0        0        0     2386 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/data_model.py
+-rw-r--r--   0        0        0     3937 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py
+-rw-r--r--   0        0        0     3267 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/data_set.py
+-rw-r--r--   0        0        0     4226 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py
+-rw-r--r--   0        0        0     9218 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py
+-rw-r--r--   0        0        0     2965 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py
+-rw-r--r--   0        0        0    11204 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py
+-rw-r--r--   0        0        0    20768 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py
+-rw-r--r--   0        0        0     2390 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Alerts.json
+-rw-r--r--   0        0        0     5281 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Authentication.json
+-rw-r--r--   0        0        0     9626 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Certificates.json
+-rw-r--r--   0        0        0     8173 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Change.json
+-rw-r--r--   0        0        0     2814 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/DLP.json
+-rw-r--r--   0        0        0     8598 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Email.json
+-rw-r--r--   0        0        0    18855 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Endpoint.json
+-rw-r--r--   0        0        0     9890 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json
+-rw-r--r--   0        0        0     4255 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Malware.json
+-rw-r--r--   0        0        0     8683 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json
+-rw-r--r--   0        0        0     5599 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json
+-rw-r--r--   0        0        0    18953 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json
+-rw-r--r--   0        0        0     3862 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Updates.json
+-rw-r--r--   0        0        0     5184 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json
+-rw-r--r--   0        0        0     7178 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Web.json
+-rw-r--r--   0        0        0      889 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py
+-rw-r--r--   0        0        0      862 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py
+-rw-r--r--   0        0        0     7339 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py
+-rw-r--r--   0        0        0     5002 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py
+-rw-r--r--   0        0        0     4418 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py
+-rw-r--r--   0        0        0     4995 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py
+-rw-r--r--   0        0        0     3615 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py
+-rw-r--r--   0        0        0     3015 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py
+-rw-r--r--   0        0        0      812 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/__init__.py
+-rw-r--r--   0        0        0     3305 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py
+-rw-r--r--   0        0        0     5420 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py
+-rw-r--r--   0        0        0    11040 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py
+-rw-r--r--   0        0        0    10360 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py
+-rw-r--r--   0        0        0    21984 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py
+-rw-r--r--   0        0        0      766 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/__init__.py
+-rw-r--r--   0        0        0      711 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/key_fields.py
+-rw-r--r--   0        0        0    11987 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/test_generator.py
+-rw-r--r--   0        0        0    11457 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/test_templates.py
+-rw-r--r--   0        0        0      909 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/__init__.py
+-rw-r--r--   0        0        0     7291 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py
+-rw-r--r--   0        0        0    46400 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/rule.py
+-rw-r--r--   0        0        0    15413 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py
+-rw-r--r--   0        0        0     2290 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py
+-rw-r--r--   0        0        0    16792 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py
+-rw-r--r--   0        0        0     6032 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py
+-rw-r--r--   0        0        0     9990 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd
+-rw-r--r--   0        0        0     6217 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py
+-rw-r--r--   0        0        0      834 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/__init__.py
+-rw-r--r--   0        0        0     4634 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/junit_parser.py
+-rw-r--r--   0        0        0     1627 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/log_helper.py
+-rw-r--r--   0        0        0     3034 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py
+-rw-r--r--   0        0        0     3414 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py
+-rw-r--r--   0        0        0    17585 2024-05-27 08:10:07.075065 pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/tools/cim_field_report.py
+-rw-r--r--   0        0        0     1427 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.3.0b2/PKG-INFO
```

### Comparing `pytest_splunk_addon-5.3.0b1/LICENSE` & `pytest_splunk_addon-5.3.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pyproject.toml` & `pytest_splunk_addon-5.3.0b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 [tool.poetry]
 name = "pytest-splunk-addon"
-version = "5.3.0-beta.1"
+version = "5.3.0-beta.2"
 description = "A Dynamic test tool for Splunk Apps and Add-ons"
 authors = ["Splunk <addonfactory@splunk.com>"]
 license = "APACHE-2.0"
 classifiers = [
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Testing",
```

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/.ignore_splunk_internal_errors` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/.ignore_splunk_internal_errors`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/__init__.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,12 +10,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # -*- coding: utf-8 -*-
-"""Top-level package for splunk-app-test-lib."""
+"""
+There are 2 utilities included:
 
-__author__ = """Splunk Inc."""
-__email__ = "addonfactory@splunk.com"
-__version__ = "5.3.0-beta.1"
+1. CIM Compliance report generator for pytest-splunk-addon
+2. pytest-splunk-addon-data.conf generator
+
+"""
+
+from .junit_parser import JunitParser
+from .xml_event_parser import escape_char_event
```

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/docker_class.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/docker_class.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/plugin.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/splunk.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/splunk.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/__init__.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_basic.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_basic.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/fields.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/fields.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/app_test_generator.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/app_test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/data_model.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/data_set.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Alerts.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Alerts.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Authentication.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Authentication.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Certificates.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Certificates.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Change.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Change.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/DLP.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/DLP.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Email.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Email.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Endpoint.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Malware.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Malware.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998168927856428%*

 * *Differences: {"'objects'": "{0: {'fields': {10: {'expected_values': {insert: [(8, 'NXRRSet'), (11, "*

 * *              "'DSOTYPENI'), (19, 'BADTRUNC'), (20, 'BADCOOKIE')]}}, 11: {'expected_values': "*

 * *              "{insert: [(3, '4'), (4, '5'), (5, '6'), (6, '7'), (7, '8'), (8, '9'), (9, '10'), "*

 * *              "(10, '11'), (11, '16'), (12, '17'), (13, '18'), (14, '19'), (15, '20'), (16, '21'), "*

 * *              "(17, '22'), (18, '23')], delete: [17, 16, 15, 14, 13, 12, 11, 10, 9, 8, 7, 6, 5, 4, "*

 * *              "3, 2, 1, 0]},  […]*

```diff
@@ -178,51 +178,53 @@
                         "Format Error",
                         "Server Failure",
                         "Non-Existent Domain",
                         "NotImp",
                         "Refused",
                         "YXDomain",
                         "YXRRSet",
+                        "NXRRSet",
                         "NotAuth",
                         "NotZone",
+                        "DSOTYPENI",
                         "BADVERS",
                         "BADSIG",
                         "BADKEY",
                         "BADTIME",
                         "BADMODE",
                         "BADNAME",
-                        "BADALG"
+                        "BADALG",
+                        "BADTRUNC",
+                        "BADCOOKIE"
                     ],
                     "name": "reply_code",
                     "type": "required"
                 },
                 {
-                    "comment": "The numerical id or name of a return code. For details, see the Domain Name System Parameters on the Internet Assigned Numbers Authority (IANA) web site.",
+                    "comment": "The numerical id of a return code. For details, see the Domain Name System Parameters on the Internet Assigned Numbers Authority (IANA) web site.",
                     "expected_values": [
-                        "No Error",
-                        "Format Error",
-                        "Server Failure",
-                        "Non-Existent Domain",
-                        "NotImp",
-                        "Refused",
-                        "YXDomain",
-                        "YXRRSet",
-                        "NotAuth",
-                        "NotZone",
-                        "BADVERS",
-                        "BADSIG",
-                        "BADKEY",
-                        "BADTIME",
-                        "BADMODE",
-                        "BADNAME",
-                        "BADALG",
-                        "0",
                         "1",
                         "2",
-                        "3"
+                        "3",
+                        "4",
+                        "5",
+                        "6",
+                        "7",
+                        "8",
+                        "9",
+                        "10",
+                        "11",
+                        "16",
+                        "17",
+                        "18",
+                        "19",
+                        "20",
+                        "21",
+                        "22",
+                        "23"
                     ],
                     "name": "reply_code_id",
                     "type": "required"
                 },
                 {
                     "comment": "The amount of time it took to receive a response in the network resolution event, in seconds.",
                     "name": "response_time",
```

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Updates.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Updates.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Web.json` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/data_models/Web.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/__init__.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/key_fields.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/index_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/rule.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/rule.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/junit_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/log_helper.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/log_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/tools/cim_field_report.py` & `pytest_splunk_addon-5.3.0b2/pytest_splunk_addon/tools/cim_field_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.3.0b1/PKG-INFO` & `pytest_splunk_addon-5.3.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-splunk-addon
-Version: 5.3.0b1
+Version: 5.3.0b2
 Summary: A Dynamic test tool for Splunk Apps and Add-ons
 License: Apache-2.0
 Author: Splunk
 Author-email: addonfactory@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

