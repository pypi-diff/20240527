# Comparing `tmp/sustainability-scanner-1.2.6.tar.gz` & `tmp/sustainability-scanner-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sustainability-scanner-1.2.6.tar", last modified: Mon May 27 14:35:39 2024, max compression
+gzip compressed data, was "sustainability-scanner-1.2.7.tar", last modified: Mon May 27 14:37:50 2024, max compression
```

## Comparing `sustainability-scanner-1.2.6.tar` & `sustainability-scanner-1.2.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jyrseige   (504) staff       (20)        0 2024-05-27 14:35:39.115449 sustainability-scanner-1.2.6/
--rw-r--r--   0 jyrseige   (504) staff       (20)      947 2023-12-20 07:40:55.000000 sustainability-scanner-1.2.6/LICENSE.txt
--rw-r--r--   0 jyrseige   (504) staff       (20)     9807 2024-05-27 14:35:39.115567 sustainability-scanner-1.2.6/PKG-INFO
--rw-r--r--   0 jyrseige   (504) staff       (20)     9185 2024-05-27 13:50:01.000000 sustainability-scanner-1.2.6/README.md
--rw-r--r--   0 jyrseige   (504) staff       (20)       79 2024-05-27 14:35:39.115813 sustainability-scanner-1.2.6/setup.cfg
--rw-r--r--   0 jyrseige   (504) staff       (20)     1068 2024-05-27 13:50:01.000000 sustainability-scanner-1.2.6/setup.py
-drwxr-xr-x   0 jyrseige   (504) staff       (20)        0 2024-05-27 14:35:39.109621 sustainability-scanner-1.2.6/susscanner/
--rw-r--r--   0 jyrseige   (504) staff       (20)      680 2024-05-27 13:50:01.000000 sustainability-scanner-1.2.6/susscanner/__init__.py
--rw-r--r--   0 jyrseige   (504) staff       (20)      114 2023-11-24 06:41:31.000000 sustainability-scanner-1.2.6/susscanner/__main__.py
--rw-r--r--   0 jyrseige   (504) staff       (20)     3986 2024-03-18 06:39:01.000000 sustainability-scanner-1.2.6/susscanner/cli.py
--rw-r--r--   0 jyrseige   (504) staff       (20)      851 2023-12-06 10:16:43.000000 sustainability-scanner-1.2.6/susscanner/config.py
-drwxr-xr-x   0 jyrseige   (504) staff       (20)        0 2024-05-27 14:35:39.112328 sustainability-scanner-1.2.6/susscanner/rules/
--rw-r--r--   0 jyrseige   (504) staff       (20)      973 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/api_gw.guard
--rw-r--r--   0 jyrseige   (504) staff       (20)     1423 2023-12-06 10:16:43.000000 sustainability-scanner-1.2.6/susscanner/rules/cloud_front.guard
--rw-r--r--   0 jyrseige   (504) staff       (20)      477 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/cloudwatch.guard
--rw-r--r--   0 jyrseige   (504) staff       (20)      677 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/codeguru.guard
--rw-r--r--   0 jyrseige   (504) staff       (20)     2483 2024-03-18 06:39:23.000000 sustainability-scanner-1.2.6/susscanner/rules/ec2.guard
--rw-r--r--   0 jyrseige   (504) staff       (20)      586 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/emr.guard
--rw-r--r--   0 jyrseige   (504) staff       (20)      726 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/glue.guard
--rw-r--r--   0 jyrseige   (504) staff       (20)      686 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/graviton.guard
--rw-r--r--   0 jyrseige   (504) staff       (20)      685 2023-12-06 10:16:43.000000 sustainability-scanner-1.2.6/susscanner/rules/rds.guard
--rw-r--r--   0 jyrseige   (504) staff       (20)      411 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/s3.guard
-drwxr-xr-x   0 jyrseige   (504) staff       (20)        0 2024-05-27 14:35:39.114153 sustainability-scanner-1.2.6/susscanner/rules/test_cases/
--rw-r--r--   0 jyrseige   (504) staff       (20)      746 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/test_cases/api_gw_tests.yaml
--rw-r--r--   0 jyrseige   (504) staff       (20)     3453 2023-12-06 10:16:43.000000 sustainability-scanner-1.2.6/susscanner/rules/test_cases/cloud_front_tests.yaml
--rw-r--r--   0 jyrseige   (504) staff       (20)     1048 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/test_cases/cloudwatch_tests.yaml
--rw-r--r--   0 jyrseige   (504) staff       (20)     1332 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/test_cases/codeguru_tests.yaml
--rw-r--r--   0 jyrseige   (504) staff       (20)     4037 2024-03-18 06:39:23.000000 sustainability-scanner-1.2.6/susscanner/rules/test_cases/ec2_tests.yaml
--rw-r--r--   0 jyrseige   (504) staff       (20)     1704 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/test_cases/emr_tests.yaml
--rw-r--r--   0 jyrseige   (504) staff       (20)     3798 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/test_cases/glue_tests.yaml
--rw-r--r--   0 jyrseige   (504) staff       (20)     4305 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/test_cases/graviton_tests.yaml
--rw-r--r--   0 jyrseige   (504) staff       (20)     1803 2023-12-06 10:16:43.000000 sustainability-scanner-1.2.6/susscanner/rules/test_cases/rds_tests.yaml
--rw-r--r--   0 jyrseige   (504) staff       (20)     2494 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules/test_cases/s3_tests.yaml
--rw-r--r--   0 jyrseige   (504) staff       (20)    14957 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.6/susscanner/rules_metadata.json
--rw-r--r--   0 jyrseige   (504) staff       (20)    10465 2024-05-27 13:50:01.000000 sustainability-scanner-1.2.6/susscanner/scan.py
-drwxr-xr-x   0 jyrseige   (504) staff       (20)        0 2024-05-27 14:35:39.115316 sustainability-scanner-1.2.6/sustainability_scanner.egg-info/
--rw-r--r--   0 jyrseige   (504) staff       (20)     9807 2024-05-27 14:35:39.000000 sustainability-scanner-1.2.6/sustainability_scanner.egg-info/PKG-INFO
--rw-r--r--   0 jyrseige   (504) staff       (20)     1209 2024-05-27 14:35:39.000000 sustainability-scanner-1.2.6/sustainability_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 jyrseige   (504) staff       (20)        1 2024-05-27 14:35:39.000000 sustainability-scanner-1.2.6/sustainability_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 jyrseige   (504) staff       (20)       56 2024-05-27 14:35:39.000000 sustainability-scanner-1.2.6/sustainability_scanner.egg-info/entry_points.txt
--rw-r--r--   0 jyrseige   (504) staff       (20)       13 2024-05-27 14:35:39.000000 sustainability-scanner-1.2.6/sustainability_scanner.egg-info/requires.txt
--rw-r--r--   0 jyrseige   (504) staff       (20)       11 2024-05-27 14:35:39.000000 sustainability-scanner-1.2.6/sustainability_scanner.egg-info/top_level.txt
+drwxr-xr-x   0 jyrseige   (504) staff       (20)        0 2024-05-27 14:37:50.866235 sustainability-scanner-1.2.7/
+-rw-r--r--   0 jyrseige   (504) staff       (20)      947 2023-12-20 07:40:55.000000 sustainability-scanner-1.2.7/LICENSE.txt
+-rw-r--r--   0 jyrseige   (504) staff       (20)     9807 2024-05-27 14:37:50.866345 sustainability-scanner-1.2.7/PKG-INFO
+-rw-r--r--   0 jyrseige   (504) staff       (20)     9185 2024-05-27 14:37:43.000000 sustainability-scanner-1.2.7/README.md
+-rw-r--r--   0 jyrseige   (504) staff       (20)       79 2024-05-27 14:37:50.866557 sustainability-scanner-1.2.7/setup.cfg
+-rw-r--r--   0 jyrseige   (504) staff       (20)     1082 2024-05-27 14:37:43.000000 sustainability-scanner-1.2.7/setup.py
+drwxr-xr-x   0 jyrseige   (504) staff       (20)        0 2024-05-27 14:37:50.860931 sustainability-scanner-1.2.7/susscanner/
+-rw-r--r--   0 jyrseige   (504) staff       (20)      664 2024-05-27 14:37:43.000000 sustainability-scanner-1.2.7/susscanner/__init__.py
+-rw-r--r--   0 jyrseige   (504) staff       (20)      114 2023-11-24 06:41:31.000000 sustainability-scanner-1.2.7/susscanner/__main__.py
+-rw-r--r--   0 jyrseige   (504) staff       (20)     4019 2024-05-27 14:37:43.000000 sustainability-scanner-1.2.7/susscanner/cli.py
+-rw-r--r--   0 jyrseige   (504) staff       (20)      851 2023-12-06 10:16:43.000000 sustainability-scanner-1.2.7/susscanner/config.py
+drwxr-xr-x   0 jyrseige   (504) staff       (20)        0 2024-05-27 14:37:50.863088 sustainability-scanner-1.2.7/susscanner/rules/
+-rw-r--r--   0 jyrseige   (504) staff       (20)      973 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/api_gw.guard
+-rw-r--r--   0 jyrseige   (504) staff       (20)     1423 2023-12-06 10:16:43.000000 sustainability-scanner-1.2.7/susscanner/rules/cloud_front.guard
+-rw-r--r--   0 jyrseige   (504) staff       (20)      477 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/cloudwatch.guard
+-rw-r--r--   0 jyrseige   (504) staff       (20)      677 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/codeguru.guard
+-rw-r--r--   0 jyrseige   (504) staff       (20)     2483 2024-03-18 06:39:23.000000 sustainability-scanner-1.2.7/susscanner/rules/ec2.guard
+-rw-r--r--   0 jyrseige   (504) staff       (20)      586 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/emr.guard
+-rw-r--r--   0 jyrseige   (504) staff       (20)      726 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/glue.guard
+-rw-r--r--   0 jyrseige   (504) staff       (20)      686 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/graviton.guard
+-rw-r--r--   0 jyrseige   (504) staff       (20)      685 2023-12-06 10:16:43.000000 sustainability-scanner-1.2.7/susscanner/rules/rds.guard
+-rw-r--r--   0 jyrseige   (504) staff       (20)      411 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/s3.guard
+drwxr-xr-x   0 jyrseige   (504) staff       (20)        0 2024-05-27 14:37:50.865252 sustainability-scanner-1.2.7/susscanner/rules/test_cases/
+-rw-r--r--   0 jyrseige   (504) staff       (20)      746 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/test_cases/api_gw_tests.yaml
+-rw-r--r--   0 jyrseige   (504) staff       (20)     3453 2023-12-06 10:16:43.000000 sustainability-scanner-1.2.7/susscanner/rules/test_cases/cloud_front_tests.yaml
+-rw-r--r--   0 jyrseige   (504) staff       (20)     1048 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/test_cases/cloudwatch_tests.yaml
+-rw-r--r--   0 jyrseige   (504) staff       (20)     1332 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/test_cases/codeguru_tests.yaml
+-rw-r--r--   0 jyrseige   (504) staff       (20)     4037 2024-03-18 06:39:23.000000 sustainability-scanner-1.2.7/susscanner/rules/test_cases/ec2_tests.yaml
+-rw-r--r--   0 jyrseige   (504) staff       (20)     1704 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/test_cases/emr_tests.yaml
+-rw-r--r--   0 jyrseige   (504) staff       (20)     3798 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/test_cases/glue_tests.yaml
+-rw-r--r--   0 jyrseige   (504) staff       (20)     4305 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/test_cases/graviton_tests.yaml
+-rw-r--r--   0 jyrseige   (504) staff       (20)     1803 2023-12-06 10:16:43.000000 sustainability-scanner-1.2.7/susscanner/rules/test_cases/rds_tests.yaml
+-rw-r--r--   0 jyrseige   (504) staff       (20)     2494 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules/test_cases/s3_tests.yaml
+-rw-r--r--   0 jyrseige   (504) staff       (20)    14957 2023-11-21 08:23:03.000000 sustainability-scanner-1.2.7/susscanner/rules_metadata.json
+-rw-r--r--   0 jyrseige   (504) staff       (20)    10457 2024-05-27 14:37:43.000000 sustainability-scanner-1.2.7/susscanner/scan.py
+drwxr-xr-x   0 jyrseige   (504) staff       (20)        0 2024-05-27 14:37:50.866114 sustainability-scanner-1.2.7/sustainability_scanner.egg-info/
+-rw-r--r--   0 jyrseige   (504) staff       (20)     9807 2024-05-27 14:37:50.000000 sustainability-scanner-1.2.7/sustainability_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 jyrseige   (504) staff       (20)     1209 2024-05-27 14:37:50.000000 sustainability-scanner-1.2.7/sustainability_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 jyrseige   (504) staff       (20)        1 2024-05-27 14:37:50.000000 sustainability-scanner-1.2.7/sustainability_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 jyrseige   (504) staff       (20)       56 2024-05-27 14:37:50.000000 sustainability-scanner-1.2.7/sustainability_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 jyrseige   (504) staff       (20)       13 2024-05-27 14:37:50.000000 sustainability-scanner-1.2.7/sustainability_scanner.egg-info/requires.txt
+-rw-r--r--   0 jyrseige   (504) staff       (20)       11 2024-05-27 14:37:50.000000 sustainability-scanner-1.2.7/sustainability_scanner.egg-info/top_level.txt
```

### Comparing `sustainability-scanner-1.2.6/LICENSE.txt` & `sustainability-scanner-1.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/PKG-INFO` & `sustainability-scanner-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sustainability-scanner
-Version: 1.2.6
+Version: 1.2.7
 Summary: Sustainability Scanner
 Home-page: http://github.com/awslabs/sustainability-scanner
 Author: AWS
 License: MIT-0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -97,15 +97,15 @@
 You should see an output like below;
 
 ```sh
 susscanner test.yaml
 {
     "title": "Sustainability Scanner Report",
     "file": "test.yaml",
-    "version": "1.2.6",
+    "version": "1.2.7",
     "sustainability_score": 8,
     "failed_rules": [
         {
             "rule_name": "rest_api_compression_max",
             "severity": "MEDIUM",
             "message": "Consider configuring the payload compression with MinimumCompressionSize. Compressing the payload will in general reduce the network traffic.",
             "links": [
@@ -230,15 +230,15 @@
 
 You will get a Sustainability Scanner Report without failed rules. This looks as follows:
 
 ```
 {
     "title": "Sustainability Scanner Report",
     "file": "cloudformation.yaml",
-    "version": "1.2.6",
+    "version": "1.2.7",
     "sustainability_score": 0,
     "failed_rules": []
 }
 ```
 
 ### Can I use it as part of a Github workflow?
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sustainability-scanner Version: 1.2.6 Summary:
+Metadata-Version: 2.1 Name: sustainability-scanner Version: 1.2.7 Summary:
 Sustainability Scanner Home-page: http://github.com/awslabs/sustainability-
 scanner Author: AWS License: MIT-0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 System Administrators Classifier: Natural Language :: English Classifier:
 License :: OSI Approved :: MIT No Attribution License (MIT-0) Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
@@ -38,15 +38,15 @@
 susscanner [OPTIONS] [CloudFormation Template] Arguments: [CloudFormation
 Template] The AWS CloudFormation template(s) to use [required] Options: --
 version -v Show the application version and exit. --rules -r PATH Location for
 a custom rules metadata file. --help Show this message and exit. ``` You can
 scan a template by using the command: ```sh susscanner [path/to/cloudformation/
 template_or_templates] ``` You should see an output like below; ```sh
 susscanner test.yaml { "title": "Sustainability Scanner Report", "file":
-"test.yaml", "version": "1.2.6", "sustainability_score": 8, "failed_rules": [
+"test.yaml", "version": "1.2.7", "sustainability_score": 8, "failed_rules": [
 { "rule_name": "rest_api_compression_max", "severity": "MEDIUM", "message":
 "Consider configuring the payload compression with MinimumCompressionSize.
 Compressing the payload will in general reduce the network traffic.", "links":
 [ "https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-
 gzip-compression-decompression.html", "https://docs.aws.amazon.com/
 wellarchitected/latest/sustainability-pillar/sus_sus_data_a8.html" ],
 "resources": [ { "name": "/Resources/API-GW-2/Properties/
@@ -107,13 +107,13 @@
 in the `rule_name` variable. ## FAQs ### Are all the recommendations mandatory
 to implement? No, the recommendations are not mandatory to implement, if you
 categorize a best practice as not applicable or prefer the status quo given
 your workload, you can choose to either ignore the failed rule or disable it.
 ### What happens if there are no suggested improvements? You will get a
 Sustainability Scanner Report without failed rules. This looks as follows: ```
 { "title": "Sustainability Scanner Report", "file": "cloudformation.yaml",
-"version": "1.2.6", "sustainability_score": 0, "failed_rules": [] } ``` ### Can
+"version": "1.2.7", "sustainability_score": 0, "failed_rules": [] } ``` ### Can
 I use it as part of a Github workflow? Yes, a Github Action to run the scanner
 is available on the [marketplace](https://github.com/marketplace/actions/aws-
 sustainability-scanner-github-action). ## Security See [CONTRIBUTING]
 (CONTRIBUTING.md#security-issue-notifications) for more information. ## License
 This project is licensed under the MIT-0 License.
```

### Comparing `sustainability-scanner-1.2.6/README.md` & `sustainability-scanner-1.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 You should see an output like below;
 
 ```sh
 susscanner test.yaml
 {
     "title": "Sustainability Scanner Report",
     "file": "test.yaml",
-    "version": "1.2.6",
+    "version": "1.2.7",
     "sustainability_score": 8,
     "failed_rules": [
         {
             "rule_name": "rest_api_compression_max",
             "severity": "MEDIUM",
             "message": "Consider configuring the payload compression with MinimumCompressionSize. Compressing the payload will in general reduce the network traffic.",
             "links": [
@@ -212,15 +212,15 @@
 
 You will get a Sustainability Scanner Report without failed rules. This looks as follows:
 
 ```
 {
     "title": "Sustainability Scanner Report",
     "file": "cloudformation.yaml",
-    "version": "1.2.6",
+    "version": "1.2.7",
     "sustainability_score": 0,
     "failed_rules": []
 }
 ```
 
 ### Can I use it as part of a Github workflow?
```

#### html2text {}

```diff
@@ -30,15 +30,15 @@
 susscanner [OPTIONS] [CloudFormation Template] Arguments: [CloudFormation
 Template] The AWS CloudFormation template(s) to use [required] Options: --
 version -v Show the application version and exit. --rules -r PATH Location for
 a custom rules metadata file. --help Show this message and exit. ``` You can
 scan a template by using the command: ```sh susscanner [path/to/cloudformation/
 template_or_templates] ``` You should see an output like below; ```sh
 susscanner test.yaml { "title": "Sustainability Scanner Report", "file":
-"test.yaml", "version": "1.2.6", "sustainability_score": 8, "failed_rules": [
+"test.yaml", "version": "1.2.7", "sustainability_score": 8, "failed_rules": [
 { "rule_name": "rest_api_compression_max", "severity": "MEDIUM", "message":
 "Consider configuring the payload compression with MinimumCompressionSize.
 Compressing the payload will in general reduce the network traffic.", "links":
 [ "https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-
 gzip-compression-decompression.html", "https://docs.aws.amazon.com/
 wellarchitected/latest/sustainability-pillar/sus_sus_data_a8.html" ],
 "resources": [ { "name": "/Resources/API-GW-2/Properties/
@@ -99,13 +99,13 @@
 in the `rule_name` variable. ## FAQs ### Are all the recommendations mandatory
 to implement? No, the recommendations are not mandatory to implement, if you
 categorize a best practice as not applicable or prefer the status quo given
 your workload, you can choose to either ignore the failed rule or disable it.
 ### What happens if there are no suggested improvements? You will get a
 Sustainability Scanner Report without failed rules. This looks as follows: ```
 { "title": "Sustainability Scanner Report", "file": "cloudformation.yaml",
-"version": "1.2.6", "sustainability_score": 0, "failed_rules": [] } ``` ### Can
+"version": "1.2.7", "sustainability_score": 0, "failed_rules": [] } ``` ### Can
 I use it as part of a Github workflow? Yes, a Github Action to run the scanner
 is available on the [marketplace](https://github.com/marketplace/actions/aws-
 sustainability-scanner-github-action). ## Security See [CONTRIBUTING]
 (CONTRIBUTING.md#security-issue-notifications) for more information. ## License
 This project is licensed under the MIT-0 License.
```

### Comparing `sustainability-scanner-1.2.6/setup.py` & `sustainability-scanner-1.2.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from setuptools import find_packages, setup
 
 setup(
     name="sustainability-scanner",
-    version="1.2.6",
+    version="1.2.7",
     author="AWS",
     description="Sustainability Scanner",
     long_description_content_type="text/markdown",
-    long_description=open('README.md').read(),
+    long_description=open("README.md").read(),
     packages=find_packages(include=["susscanner", "susscanner.*"]),
-    package_data={"": ["rules_metadata.json", "rules/*", "rules/test_cases/*", "static/*"]},
+    package_data={
+        "": ["rules_metadata.json", "rules/*", "rules/test_cases/*", "static/*"]
+    },
     include_package_data=True,
     install_requires=["typer==0.7.0"],
     url="http://github.com/awslabs/sustainability-scanner",
     python_requires=">=3.6",
     license="MIT-0",
     entry_points={
         "console_scripts": ["susscanner=susscanner.__main__:main"],
     },
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'Intended Audience :: System Administrators',
-        'Natural Language :: English',
-        'License :: OSI Approved :: MIT No Attribution License (MIT-0)',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "Intended Audience :: System Administrators",
+        "Natural Language :: English",
+        "License :: OSI Approved :: MIT No Attribution License (MIT-0)",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
     ],
 )
```

### Comparing `sustainability-scanner-1.2.6/susscanner/__init__.py` & `sustainability-scanner-1.2.7/susscanner/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from susscanner.scan import Scan
 from susscanner.config import init_app
 from susscanner.cli import main
 
 
 __app_name__ = "susscanner"
-__version__ = "1.2.6"
+__version__ = "1.2.7"
 
 (
     SUCCESS,
     FILE_ERROR,
     JSON_ERROR,
     TEMPLATE_ERROR,
     ID_ERROR,
@@ -27,10 +27,10 @@
 ERRORS = {
     FILE_ERROR: "config file error",
     JSON_ERROR: "json error",
     TEMPLATE_ERROR: "CloudFormation Template error",
     ID_ERROR: "id error",
 }
 
-DIR_PATH = absolute_path = os.path.dirname(__file__)
+DIR_PATH = os.path.dirname(__file__)
 CONFIG_FILE_NAME = "rules_metadata.json"
 CONFIG_FILE_PATH = Path(os.path.join(DIR_PATH, CONFIG_FILE_NAME))
```

### Comparing `sustainability-scanner-1.2.6/susscanner/cli.py` & `sustainability-scanner-1.2.7/susscanner/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,18 +110,18 @@
     if app_init_error == ss.TEMPLATE_ERROR:
         typer.secho(
             f'CloudFormation template not found "{ss.ERRORS[app_init_error]}"',
             fg=typer.colors.RED,
         )
         raise typer.Exit(3)
 
-    rules = f"{ss.DIR_PATH}/rules/"
+    rules = Path(ss.DIR_PATH).joinpath(Path("rules")).__str__()
 
     for template in cfn_template:
-        command = f"cfn-guard validate -o json --rules {rules} --data {template}"
+        command = rf"cfn-guard validate -o json --rules '{rules}' --data '{template}'"
         args = shlex.split(command)
 
         cfn_guard_output = subprocess.Popen(
             args,
             shell=False,
             universal_newlines=True,
             stdout=subprocess.PIPE,
```

### Comparing `sustainability-scanner-1.2.6/susscanner/config.py` & `sustainability-scanner-1.2.7/susscanner/config.py`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/api_gw.guard` & `sustainability-scanner-1.2.7/susscanner/rules/api_gw.guard`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/cloud_front.guard` & `sustainability-scanner-1.2.7/susscanner/rules/cloud_front.guard`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/codeguru.guard` & `sustainability-scanner-1.2.7/susscanner/rules/codeguru.guard`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/ec2.guard` & `sustainability-scanner-1.2.7/susscanner/rules/ec2.guard`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/emr.guard` & `sustainability-scanner-1.2.7/susscanner/rules/emr.guard`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/glue.guard` & `sustainability-scanner-1.2.7/susscanner/rules/glue.guard`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/graviton.guard` & `sustainability-scanner-1.2.7/susscanner/rules/graviton.guard`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/rds.guard` & `sustainability-scanner-1.2.7/susscanner/rules/rds.guard`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/test_cases/api_gw_tests.yaml` & `sustainability-scanner-1.2.7/susscanner/rules/test_cases/api_gw_tests.yaml`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/test_cases/cloud_front_tests.yaml` & `sustainability-scanner-1.2.7/susscanner/rules/test_cases/cloud_front_tests.yaml`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/test_cases/cloudwatch_tests.yaml` & `sustainability-scanner-1.2.7/susscanner/rules/test_cases/cloudwatch_tests.yaml`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/test_cases/codeguru_tests.yaml` & `sustainability-scanner-1.2.7/susscanner/rules/test_cases/codeguru_tests.yaml`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/test_cases/ec2_tests.yaml` & `sustainability-scanner-1.2.7/susscanner/rules/test_cases/ec2_tests.yaml`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/test_cases/emr_tests.yaml` & `sustainability-scanner-1.2.7/susscanner/rules/test_cases/emr_tests.yaml`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/test_cases/glue_tests.yaml` & `sustainability-scanner-1.2.7/susscanner/rules/test_cases/glue_tests.yaml`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/test_cases/graviton_tests.yaml` & `sustainability-scanner-1.2.7/susscanner/rules/test_cases/graviton_tests.yaml`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/test_cases/rds_tests.yaml` & `sustainability-scanner-1.2.7/susscanner/rules/test_cases/rds_tests.yaml`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules/test_cases/s3_tests.yaml` & `sustainability-scanner-1.2.7/susscanner/rules/test_cases/s3_tests.yaml`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/rules_metadata.json` & `sustainability-scanner-1.2.7/susscanner/rules_metadata.json`

 * *Files identical despite different names*

### Comparing `sustainability-scanner-1.2.6/susscanner/scan.py` & `sustainability-scanner-1.2.7/susscanner/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,15 @@
                "links": [],
                "resources": [{"name": "", "line": 123}]
             }
         """
         md = self.load_metadata(rules_metadata)
         failed_rules = []
         matcher = re.match(
-            r".*(}|^)([A-Za-z\d_./-]+) Status = FAIL", cfn_guard_output, re.DOTALL
+            r".*(}|^)([\d\S]+) Status = FAIL", cfn_guard_output, re.DOTALL
         )
         if matcher:
             file_name = matcher.group(2)
             failed_pieces = cfn_guard_output.split(file_name + " ")
             for p in failed_pieces:
                 delim = p.find("---")
                 if delim >= 0:
```

### Comparing `sustainability-scanner-1.2.6/sustainability_scanner.egg-info/PKG-INFO` & `sustainability-scanner-1.2.7/sustainability_scanner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sustainability-scanner
-Version: 1.2.6
+Version: 1.2.7
 Summary: Sustainability Scanner
 Home-page: http://github.com/awslabs/sustainability-scanner
 Author: AWS
 License: MIT-0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -97,15 +97,15 @@
 You should see an output like below;
 
 ```sh
 susscanner test.yaml
 {
     "title": "Sustainability Scanner Report",
     "file": "test.yaml",
-    "version": "1.2.6",
+    "version": "1.2.7",
     "sustainability_score": 8,
     "failed_rules": [
         {
             "rule_name": "rest_api_compression_max",
             "severity": "MEDIUM",
             "message": "Consider configuring the payload compression with MinimumCompressionSize. Compressing the payload will in general reduce the network traffic.",
             "links": [
@@ -230,15 +230,15 @@
 
 You will get a Sustainability Scanner Report without failed rules. This looks as follows:
 
 ```
 {
     "title": "Sustainability Scanner Report",
     "file": "cloudformation.yaml",
-    "version": "1.2.6",
+    "version": "1.2.7",
     "sustainability_score": 0,
     "failed_rules": []
 }
 ```
 
 ### Can I use it as part of a Github workflow?
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sustainability-scanner Version: 1.2.6 Summary:
+Metadata-Version: 2.1 Name: sustainability-scanner Version: 1.2.7 Summary:
 Sustainability Scanner Home-page: http://github.com/awslabs/sustainability-
 scanner Author: AWS License: MIT-0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 System Administrators Classifier: Natural Language :: English Classifier:
 License :: OSI Approved :: MIT No Attribution License (MIT-0) Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
@@ -38,15 +38,15 @@
 susscanner [OPTIONS] [CloudFormation Template] Arguments: [CloudFormation
 Template] The AWS CloudFormation template(s) to use [required] Options: --
 version -v Show the application version and exit. --rules -r PATH Location for
 a custom rules metadata file. --help Show this message and exit. ``` You can
 scan a template by using the command: ```sh susscanner [path/to/cloudformation/
 template_or_templates] ``` You should see an output like below; ```sh
 susscanner test.yaml { "title": "Sustainability Scanner Report", "file":
-"test.yaml", "version": "1.2.6", "sustainability_score": 8, "failed_rules": [
+"test.yaml", "version": "1.2.7", "sustainability_score": 8, "failed_rules": [
 { "rule_name": "rest_api_compression_max", "severity": "MEDIUM", "message":
 "Consider configuring the payload compression with MinimumCompressionSize.
 Compressing the payload will in general reduce the network traffic.", "links":
 [ "https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-
 gzip-compression-decompression.html", "https://docs.aws.amazon.com/
 wellarchitected/latest/sustainability-pillar/sus_sus_data_a8.html" ],
 "resources": [ { "name": "/Resources/API-GW-2/Properties/
@@ -107,13 +107,13 @@
 in the `rule_name` variable. ## FAQs ### Are all the recommendations mandatory
 to implement? No, the recommendations are not mandatory to implement, if you
 categorize a best practice as not applicable or prefer the status quo given
 your workload, you can choose to either ignore the failed rule or disable it.
 ### What happens if there are no suggested improvements? You will get a
 Sustainability Scanner Report without failed rules. This looks as follows: ```
 { "title": "Sustainability Scanner Report", "file": "cloudformation.yaml",
-"version": "1.2.6", "sustainability_score": 0, "failed_rules": [] } ``` ### Can
+"version": "1.2.7", "sustainability_score": 0, "failed_rules": [] } ``` ### Can
 I use it as part of a Github workflow? Yes, a Github Action to run the scanner
 is available on the [marketplace](https://github.com/marketplace/actions/aws-
 sustainability-scanner-github-action). ## Security See [CONTRIBUTING]
 (CONTRIBUTING.md#security-issue-notifications) for more information. ## License
 This project is licensed under the MIT-0 License.
```

### Comparing `sustainability-scanner-1.2.6/sustainability_scanner.egg-info/SOURCES.txt` & `sustainability-scanner-1.2.7/sustainability_scanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

