# Comparing `tmp/cdklabs.aws_data_solutions_framework-1.7.0.tar.gz` & `tmp/cdklabs.aws_data_solutions_framework-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.aws_data_solutions_framework-1.7.0.tar", last modified: Fri May  3 16:49:18 2024, max compression
+gzip compressed data, was "cdklabs.aws_data_solutions_framework-1.8.0.tar", last modified: Mon May 27 14:20:54 2024, max compression
```

## Comparing `cdklabs.aws_data_solutions_framework-1.7.0.tar` & `cdklabs.aws_data_solutions_framework-1.8.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.472687 cdklabs.aws_data_solutions_framework-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.472687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.476687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.476687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  3976219 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/_jsii/aws-data-solutions-framework@1.7.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/consumption/
--rw-r--r--   0 runner    (1001) docker     (127)   263926 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/consumption/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/governance/
--rw-r--r--   0 runner    (1001) docker     (127)    45726 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/governance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/processing/
--rw-r--r--   0 runner    (1001) docker     (127)   259729 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/storage/
--rw-r--r--   0 runner    (1001) docker     (127)    86274 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)    93221 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/streaming/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.480687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    97649 2024-05-03 16:49:04.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:49:18.472687 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-03 16:49:18.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-03 16:49:18.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:49:18.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 16:49:18.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 16:49:18.000000 cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:54.102865 cdklabs.aws_data_solutions_framework-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-27 14:20:54.102865 cdklabs.aws_data_solutions_framework-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:20:54.102865 cdklabs.aws_data_solutions_framework-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:54.094865 cdklabs.aws_data_solutions_framework-1.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:54.094865 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:54.098865 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:54.098865 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4306740 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/_jsii/aws-data-solutions-framework@1.8.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:54.102865 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/consumption/
+-rw-r--r--   0 runner    (1001) docker     (127)   263926 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/consumption/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:54.102865 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/governance/
+-rw-r--r--   0 runner    (1001) docker     (127)    45726 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/governance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:54.102865 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)   259729 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:54.102865 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    86274 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:54.102865 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)   184854 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/streaming/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:54.102865 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    97649 2024-05-27 14:20:38.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:20:54.094865 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs.aws_data_solutions_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-27 14:20:54.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs.aws_data_solutions_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-27 14:20:54.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:20:54.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs.aws_data_solutions_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 14:20:54.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs.aws_data_solutions_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 14:20:54.000000 cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs.aws_data_solutions_framework.egg-info/top_level.txt
```

### Comparing `cdklabs.aws_data_solutions_framework-1.7.0/LICENSE` & `cdklabs.aws_data_solutions_framework-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.7.0/PKG-INFO` & `cdklabs.aws_data_solutions_framework-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.aws_data_solutions_framework
-Version: 1.7.0
+Version: 1.8.0
 Summary: L3 CDK Constructs used to build data solutions with AWS
 Home-page: https://awslabs.github.io/data-solutions-framework-on-aws/
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/data-solutions-framework-on-aws.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.aws_data_solutions_framework-1.7.0/setup.py` & `cdklabs.aws_data_solutions_framework-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.aws_data_solutions_framework",
-    "version": "1.7.0",
+    "version": "1.8.0",
     "description": "L3 CDK Constructs used to build data solutions with AWS",
     "license": "Apache-2.0",
     "url": "https://awslabs.github.io/data-solutions-framework-on-aws/",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -28,15 +28,15 @@
         "cdklabs.aws_data_solutions_framework.processing",
         "cdklabs.aws_data_solutions_framework.storage",
         "cdklabs.aws_data_solutions_framework.streaming",
         "cdklabs.aws_data_solutions_framework.utils"
     ],
     "package_data": {
         "cdklabs.aws_data_solutions_framework._jsii": [
-            "aws-data-solutions-framework@1.7.0.jsii.tgz"
+            "aws-data-solutions-framework@1.8.0.jsii.tgz"
         ],
         "cdklabs.aws_data_solutions_framework": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/__init__.py` & `cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py` & `cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import aws_cdk.lambda_layer_kubectl_v27._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdklabs/aws-data-solutions-framework",
-    "1.7.0",
+    "1.8.0",
     __name__[0:-6],
-    "aws-data-solutions-framework@1.7.0.jsii.tgz",
+    "aws-data-solutions-framework@1.8.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/consumption/__init__.py` & `cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/consumption/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/governance/__init__.py` & `cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/governance/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/processing/__init__.py` & `cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/storage/__init__.py` & `cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs/aws_data_solutions_framework/streaming/__init__.py` & `cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs/aws_data_solutions_framework/utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,438 @@
 '''
-# Kafka Api - Bring your own cluster
+# S3DataCopy
 
-Standalone access to Kafka data plane API to perform Create/Update/Delete operations for ACLs and Topics. The constructs support both MSK Serverless and MSK Provisioned, and is used when you need to bring your own cluster.
+Data copy from one bucket to another during deployment time.
 
 ## Overview
 
-The construct leverages the [CDK Provider Framework](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.custom_resources-readme.html#provider-framework) to deploy a custom resource to manage `topics`, and in case of `mTLS` authentication deploys also a custom resource to manage `ACLs`.
+`S3DataCopy` construct provides a process to copy objects from one bucket to another during CDK deployment time:
+
+* The copy is part of the CDK and CloudFormation deployment process. It's using a synchronous CDK Custom Resource running on AWS Lambda.
+* The Lambda function is written in Typescript and copies objects between source and target buckets.
+* The execution role used by the Lambda function is scoped to the least privileges. A custom role can be provided.
+* The Lambda function can be executed in an Amazon VPC within private subnets. By default, it runs run inside VPCs owned by the AWS Lambda service.
+* The Lambda function is granted read access on the source bucket and write access on the destination bucket using the execution role policy. The construct doesn't grant cross account access.
+
+![S3 Data Copy](../../../website/static/img/s3-data-copy.png)
+
+## Usage
 
 ```python
-certificate_authority = CertificateAuthority.from_certificate_authority_arn(stack, "certificateAuthority", "arn:aws:acm-pca:eu-west-1:12345678912:certificate-authority/dummy-ca")
+class ExampleDefaultS3DataCopyStack(cdk.Stack):
+    def __init__(self, scope, id):
+        super().__init__(scope, id)
+
+        source_bucket = Bucket.from_bucket_name(self, "sourceBucket", "nyc-tlc")
+        target_bucket = Bucket.from_bucket_name(self, "destinationBucket", "staging-bucket")
+
+        dsf.utils.S3DataCopy(self, "S3DataCopy",
+            source_bucket=source_bucket,
+            source_bucket_prefix="trip data/",
+            source_bucket_region="us-east-1",
+            target_bucket=target_bucket,
+            target_bucket_prefix="staging-data/"
+        )
+```
 
-secret = Secret.from_secret_complete_arn(stack, "secret", "arn:aws:secretsmanager:eu-west-1:12345678912:secret:dsf/mskCert-dummy")
+## Private networks
 
-vpc = Vpc.from_vpc_attributes(stack, "vpc",
-    vpc_id="vpc-1111111111",
-    vpc_cidr_block="10.0.0.0/16",
-    availability_zones=["eu-west-1a", "eu-west-1b"],
-    public_subnet_ids=["subnet-111111111", "subnet-11111111"],
-    private_subnet_ids=["subnet-11111111", "subnet-1111111"]
-)
+The lambda Function used by the custom resource can be deployed in a VPC by passing the VPC and a list of private subnets.
+
+Public subnets are not supported.
 
-kafka_api = KafkaApi(stack, "kafkaApi",
+```python
+vpc = Vpc.from_lookup(self, "Vpc", vpc_name="my-vpc")
+subnets = vpc.select_subnets(subnet_type=SubnetType.PRIVATE_WITH_EGRESS)
+
+dsf.utils.S3DataCopy(self, "S3DataCopy",
+    source_bucket=source_bucket,
+    source_bucket_prefix="trip data/",
+    source_bucket_region="us-east-1",
+    target_bucket=target_bucket,
+    target_bucket_prefix="staging-data/",
     vpc=vpc,
-    cluster_arn="arn:aws:kafka:eu-west-1:12345678912:cluster/byo-msk/dummy-5cf3-42d5-aece-dummmy-2",
-    cluster_type=MskClusterType.PROVISIONED,
-    broker_security_group=SecurityGroup.from_security_group_id(stack, "brokerSecurityGroup", "sg-98237412hsa"),
-    certficate_secret=secret,
-    client_authentication=ClientAuthentication.sasl_tls(
-        iam=True,
-        certificate_authorities=[certificate_authority]
-    ),
-    kafka_client_log_level=KafkaClientLogLevel.DEBUG
+    subnets=subnets
 )
 ```
 
-:::warning
+# DataVpc
 
-The construct needs to be deployed in the same region as the MSK cluster.
+Amazon VPC optimized for data solutions.
 
-:::
+## Overview
+
+`DataVpc` construct provides a standard Amazon VPC with best practices for security and data solutions implementations:
 
-## Using mTLS authentication
+* The VPC is created with public and private subnets across 3 availability zones (1 of each per AZ) and 3 NAT gateways.
+* VPC CIDR mask should be larger than 28. The CIDR is split between public and private subnets with private subnets being twice as large as public subnet.
+* The flow logs maaged by a dedicated least-privilege IAM Role. The role can be customized.
+* The flow logs exported to an Amazon CloudWatch LogGroup encrypted with an Amazon KMS customer managed key. The KMS key can be customized.
+* A gateway VPC endpoint is created for S3 access.
 
-When using MSK with mTLS the constructs requires a principal that is assigned to the custom resources that manage ACLs and Topics. The certificate and private key are expected to be in a secret managed by [AWS Secrets Manager](https://docs.aws.amazon.com/secretsmanager/latest/userguide/intro.html). The secret needs to be in the format defined below and stored a `JSON Key/value` and not `Plaintext` in the Secret. The construct grants the lambda that supports the Custom Resource read access to the secret as an `Identity based policy`.
+## Usage
+
+```python
+class ExampleDefaultDataVpcStack(cdk.Stack):
+    def __init__(self, scope, id):
+        super().__init__(scope, id)
+        dsf.utils.DataVpc(self, "MyDataVpc",
+            vpc_cidr="10.0.0.0/16"
+        )
+```
+
+## VPC Flow Logs
+
+The construct logs VPC Flow logs in a Cloudwatch Log Group that is encrypted with a customer managed KMS Key. Exporting VPC Flow Logs to CloudWatch requires an IAM Role.
+You can customize the VPC Flow Logs management with:
+
+* your own KMS Key. Be sure to attach the right permissions to your key.
+  Refer to the [AWS documentation](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/encrypt-log-data-kms.html) for full description.
+* your own IAM Role. Be sure to configure the proper trust policy and permissions. Refer to the [AWS documentation](https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs-cwl.html#flow-logs-iam-role) for full description.
+* a custom log retention policy. Default is one week.
+
+```python
+flow_log_key = Key.from_key_arn(self, "FlowLogKey", "XXXXXXXXXXXXXXXXXXXXXXXX")
+
+flow_log_role = Role.from_role_arn(self, "FlowLogRole", "XXXXXXXXXXXXXXXXXXXXXXXX")
+
+dsf.utils.DataVpc(self, "MyDataVpc",
+    vpc_cidr="10.0.0.0/16",
+    flow_log_key=flow_log_key,
+    flow_log_role=flow_log_role,
+    flow_log_retention=RetentionDays.TWO_WEEKS
+)
+```
+
+## Removal policy
+
+You can specify if the Cloudwatch Log Group and the KMS encryption Key should be deleted when the CDK resource is destroyed using `removalPolicy`. To have an additional layer of protection, we require users to set a global context value for data removal in their CDK applications.
+
+Log group and encryption key can be destroyed when the CDK resource is destroyed only if **both** data vpc removal policy and DSF on AWS global removal policy are set to remove objects.
+
+You can set `@data-solutions-framework-on-aws/removeDataOnDestroy` (`true` or `false`) global data removal policy in `cdk.json`:
 
 ```json
-    {
-      key : "-----BEGIN RSA PRIVATE KEY----- XXXXXXXXXXXXXXXXX -----END RSA PRIVATE KEY-----",
+{
+  "context": {
+    "@data-solutions-framework-on-aws/removeDataOnDestroy": true
+  }
+}
+```
+
+Or programmatically in your CDK app:
 
-      cert : "-----BEGIN CERTIFICATE----- yyyyyyyyyyyyyyyy -----END CERTIFICATE-----"
-    }
+```python
+# Set context value for global data removal policy
+self.node.set_context("@data-solutions-framework-on-aws/removeDataOnDestroy", True)
+
+dsf.utils.DataVpc(self, "MyDataVpc",
+    vpc_cidr="10.0.0.0/16",
+    removal_policy=RemovalPolicy.DESTROY
+)
 ```
 
-You can create the secret with the following AWS CLI command:
+## Client VPN Endpoint
 
-```bash
-aws secretsmanager create-secret --name my-secret \
-    --secret-string '{"key": "PRIVATE-KEY", "cert": "CERTIFICATE"}'
+You can add client VPN endpoint to the DataVpc. Current impelementation supports SAML based authentication only and requires SSL certificate created in Amazon Certificate Manager.
+
+If you don't have an SSL certificate, you can follow this [workshop lab](https://catalog.us-east-1.prod.workshops.aws/workshops/d903ff2b-f043-4126-a4f5-64a7cc2922ec/en-US/3-aws-client-vpn/1-rsacertificatecreation) to generate a self-signed certificate and import it into Amazon Certificate Manager.
+
+Refer to the [documentation](https://docs.aws.amazon.com/vpn/latest/clientvpn-admin/federated-authentication.html) on setting up SAML federated authentication. If you don't currently use any IdP, we suggest AWS IAM Identity Center that can also be used with other DSF constructs, such as OpenSearch construct.
+
+```python
+class ExampleDefaultDataVpcStack(cdk.Stack):
+    def __init__(self, scope, id):
+        super().__init__(scope, id)
+        dsf.utils.DataVpc(self, "MyDataVpc",
+            vpc_cidr="10.0.0.0/16",
+            client_vpn_endpoint_props=dsf.utils.DataVpcClientVpnEndpointProps(
+                server_certificate_arn="arn:aws:acm:us-east-1:XXXXXXXX:certificate/XXXXXXXXXX",
+                saml_metadata_document="""<?xml version="1.0" encoding="UTF-8"?><md:EntityDescriptor xmlns:md="urn:oasis:names:tc:SAML:2.0:metadata" entityID="https://portal.sso.us-east-1.amazonaws.com/saml/assertion/XXXXXXXXXXXXXX">
+                          <md:IDPSSODescriptor WantAuthnRequestsSigned="false" protocolSupportEnumeration="urn:oasis:names:tc:SAML:2.0:protocol">
+                            <md:KeyDescriptor use="signing">
+                              <ds:KeyInfo xmlns:ds="http://www.w3.org/2000/09/xmldsig#">
+                                <ds:X509Data>
+                                  <ds:X509Certificate>XXXXXXXXXXXXXXXXXXXXXXXXX</ds:X509Certificate>
+                                </ds:X509Data>
+                              </ds:KeyInfo>
+                            </md:KeyDescriptor>
+                            <md:SingleLogoutService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST" Location="https://portal.sso.us-east-1.amazonaws.com/saml/logout/XXXXXXXXXXXXXX"/>
+                            <md:SingleLogoutService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect" Location="https://portal.sso.us-east-1.amazonaws.com/saml/logout/XXXXXXXXXXXXXX"/>
+                            <md:NameIDFormat>urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress</md:NameIDFormat>
+                            <md:SingleSignOnService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST" Location="https://portal.sso.us-east-1.amazonaws.com/saml/assertion/XXXXXXXXXXXXXX"/>
+                            <md:SingleSignOnService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect" Location="https://portal.sso.us-east-1.amazonaws.com/saml/assertion/XXXXXXXXXXXXXX"/>
+                          </md:IDPSSODescriptor>
+                        </md:EntityDescriptor>""",
+                self_service_portal=False
+            )
+        )
 ```
 
-:::danger
+# Customize DSF on AWS constructs
+
+You can customize DSF on AWS constructs in several ways to adapt to your specific needs:
+
+1. Use the Constructs properties instead of the smart defaults.
+2. Extend existing constructs and override specific methods or properties.
+3. Access CDK L1 resources and override any property.
 
-Do not create the secret as part of the CDK application. The secret contains the private key and the deployment is not secured.
+## Constructs properties
 
+Use the properties of the construct to adapt the behavior to your needs. With this approach, you bypass the smart defaults provided by the construct.
+Refer to the documentation of each construct to evaluate if your requirements can be implemented.
+
+:::note
+This method should always be preferred because constructs properties are tested as part of the DSF on AWS build process.
 :::
 
-You can use this [utility](https://github.com/aws-samples/amazon-msk-client-authentication) to generate the certificates:
+For example, you can use the `DataLakeStorage` properties to modify the lifecycle configurations for transitioning objects based on your needs instead of using the default rules:
+
+```python
+dsf.storage.DataLakeStorage(self, "MyDataLakeStorage",
+    bronze_bucket_infrequent_access_delay=90,
+    bronze_bucket_archive_delay=180,
+    silver_bucket_infrequent_access_delay=180,
+    silver_bucket_archive_delay=360,
+    gold_bucket_infrequent_access_delay=180,
+    gold_bucket_archive_delay=360
+)
+```
+
+## Construct extension
 
-1. Build the tool
-2. Run the following command to generate the certificates and print them
+AWS CDK allows developers to extend classes like any object-oriented programing language. You can use this method when you want to:
 
-```bash
-java -jar AuthMSK-1.0-SNAPSHOT.jar -caa <PCA_ARN> -ccf tmp/client_cert.pem -pem -pkf tmp/private_key.pem -ksp "XXXXXXXXXX" -ksl tmp/kafka.client.keystore.jks
-cat tmp/client_cert.pem
-cat tmp/private_key.pem
+* Override a specific method exposed by a construct.
+* Implement your own defaults. Refer to the example of the [`AnalyticsBucket`](https://github.com/awslabs/data-solutions-framework-on-aws/blob/main/framework/src/storage/analytics-bucket.ts) that extends the CDK L2 `Bucket` construct to enforce some of the parameters.
+
+## CDK resources override
+
+AWS CDK offers escape hatches to modify constructs that are encapsulated in DSF on AWS constructs. The constructs always expose the AWS resources that are encapsulated so you can manually modify their configuration. For achieving this you have 3 options:
+
+* Modify the L2 construct using its CDK API. For example, you can modify the buckets' policies provided by the [`DataLakeStorage`](https://awslabs.github.io/data-solutions-framework-on-aws/docs/constructs/library/data-lake-storage) to provide cross account write access. All the [buckets](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_s3.Bucket.html) L2 constructs are exposed as an object parameter:
+
+```python
+# Create a data lake using DSF on AWS L3 construct
+storage = dsf.storage.DataLakeStorage(self, "MyDataLakeStorage")
+
+# Access the CDK L2 Bucket construct exposed by the L3 construct
+gold_bucket = storage.gold_bucket
+
+# Use the Bucket CDK API to modify the Bucket Policy and add cross account write access
+gold_bucket.add_to_resource_policy(aws_iam.PolicyStatement(
+    actions=["s3:GetObject", "s3:PutObject", "s3:DeleteObject", "s3:ListBucketMultipartUploads", "s3:ListMultipartUploadParts", "s3:AbortMultipartUpload", "s3:ListBucket"
+    ],
+    effect=aws_iam.Effect.ALLOW,
+    principals=[aws_iam.AccountPrincipal("123456789012")]
+))
 ```
 
-1. Copy/paste the value of the client certificate and the private key in the secret
+* [Modify the L1 construct resource](https://docs.aws.amazon.com/cdk/v2/guide/cfn_layer.html#cfn_layer_resource) when there is a CDK property available on the L1 construct.
+  For example, you can override CDK L1 property for setting the S3 transfer Acceleration on the gold bucket of the `DataLakeStorage`:
 
-### setTopic
+```python
+# Create a data lake using DSF on AWS L3 construct
+storage = dsf.storage.DataLakeStorage(self, "MyDataLakeStorage")
 
-This method allows you to create, update or delete a topic. Its backend uses [kafkajs](https://kafka.js.org/).
-The topic is defined by the property type called `MskTopic`. Below you can see the definition of the topic.
+# Access the CDK L1 Bucket construct exposed by the L3 construct
+cfn_bucket = storage.gold_bucket.node.default_child
 
-```json
-{
-    topic: <String>,
-    numPartitions: <Number>,     // default: -1 (uses broker `num.partitions` configuration)
-    replicationFactor: <Number>, // default: -1 (uses broker `default.replication.factor` configuration)
-}
+# Override the CDK L1 property for transfer acceleration
+cfn_bucket.accelerate_configuration = CfnBucket.AccelerateConfigurationProperty(
+    acceleration_status="Enabled"
+)
 ```
 
-Dependeding on the authentication type used in the cluster, you need to put the right parameter in authentication, for mTLS use `Authentitcation.MTLS` and for IAM use `Authentitcation.IAM`. The example below uses IAM as authentication.
+* [Override the CloudFormation properties](https://docs.aws.amazon.com/cdk/v2/guide/cfn_layer.html#cfn_layer_raw) when there isn't any CDK property, and you need to modify the CFN template directly.
+  For example, you can override CloudFormation property for setting the S3 transfer Acceleration on the gold bucket of the `DataLakeStorage`:
 
 ```python
-kafka_api.set_topic("topic1", Authentication.IAM, MskTopic(
-    topic="topic1",
-    num_partitions=3,
-    replication_factor=1
-), cdk.RemovalPolicy.DESTROY, False, 1500)
+# Create a data lake using DSF on AWS L3 construct
+storage = dsf.storage.DataLakeStorage(self, "MyDataLakeStorage")
+
+# Access the CDK L1 Bucket construct exposed by the L3 construct
+cfn_bucket = storage.gold_bucket.node.default_child
+
+# Override the CloudFormation property for transfer acceleration
+cfn_bucket.add_override("Properties.AccelerateConfiguration.AccelerationStatus", "Enabled")
 ```
 
-:::warning
+# Create custom resources with the DsfProvider
 
-Only the number of partitions can be updated after the creation of the topic.
+DSF provides an internal construct named `DsfProvider` to facilitate the creation of custom resources in DSF constructs.
+The `DsfProvider` construct handles the undifferentiated tasks for you so you can focus on the custom resource logic.
+This construct is an opinionated implementation of the [CDK Custom Resource Provider Framework](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib-readme.html#the-custom-resource-provider-framework).
+It creates:
+
+* A custom resource provider to manage the entire custom resource lifecycle
+* An onEvent Lambda function from the provided code to perform actions you need in your custom resource
+* An optional isComplete Lambda function from the provided code when using [asynchronous custom resources](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.custom_resources-readme.html#asynchronous-providers-iscomplete)
+* The `onEvent` and `isComplete `Lambda functions are scoped down through a resource policy to be invoked only by the `Provider`.
+* CloudWatch Logs log groups for each Lambda function
+* IAM roles for each Lambda function and associated permissions
 
+:::note
+You still need to provide an IAM Managed Policy required by the actions of the Lambda functions.
 :::
 
-### setACL
+## Configuring handlers for the custom resource
 
-This method allows you to create, update or delete an ACL. Its backend uses [kafkajs](https://kafka.js.org/).
-The topic is defined by the property type called `MskACL`. This method should be used only when the cluster authentication is set to `mTLS`. Below you can see the definition of the topic as well as an example of use.
+The `DsfProvider` construct requires a Lambda function handler called `onEvent` to perform the actions of the custom resource. It also supports an optional Lambda function handler called `isComplete` to regularly perform status checks for asynchronous operation triggered in the `onEvent` handler.
 
-```json
-{
-    resourceType: <AclResourceTypes>,
-    resourceName: <String>,
-    resourcePatternType: <ResourcePatternTypes>,
-    principal: <String>,
-    host: <String>,
-    operation: <AclOperationTypes>,
-    permissionType: <AclPermissionTypes>,
-}
+Both Lambda functions are implemented in Typescript.
+`esbuild` is used to package the Lambda code and is automatically installed by `Projen`. If `esbuild` is available, `docker` will be used.
+You need to configure the path of the Lambda code (entry file) and the path of the dependency lock file (`package-lock.json`) for each handler.
+
+To generate the `package-lock.json` file, run from the Lambda code folder:
+
+```bash
+npm install --package-lock-only
 ```
 
+Then you can configure the `onEvent` and `isComplete` handlers in the `DsfProvider` construct:
+
 ```python
-kafka_api.set_acl("acl", Acl(
-    resource_type=AclResourceTypes.TOPIC,
-    resource_name="topic-1",
-    resource_pattern_type=ResourcePatternTypes.LITERAL,
-    principal="User:Cn=MyUser",
-    host="*",
-    operation=AclOperationTypes.CREATE,
-    permission_type=AclPermissionTypes.ALLOW
-), cdk.RemovalPolicy.DESTROY)
+from ...lib.dsf_provider import DsfProvider
+
+cdk.Stack):
+scope, id):
+super().__init__(scope, id)my_provider = DsfProvider(self, "Provider",
+    provider_name="my-provider",
+    on_event_handler_definition=HandlerDefinition(
+        managed_policy=my_on_event_managed_policy,
+        handler="on-event.handler",
+        deps_lock_file_path=path.join(__dirname, "./resources/lambda/my-cr/package-lock.json"),
+        entry_file=path.join(__dirname, "./resources/lambda/my-cr/on-event.mjs")
+    ),
+    is_complete_handler_definition=HandlerDefinition(
+        managed_policy=my_is_complete_managed_policy,
+        handler="is-complete.handler",
+        deps_lock_file_path=path.join(__dirname, "./resources/lambda/my-cr/package-lock.json"),
+        entry_file=path.join(__dirname, "./resources/lambda/my-cr/is-complete.mjs")
+    )
+)
+
+cdk.CustomResource(self, "CustomResource",
+    service_token=my_provider.service_token,
+    resource_type="Custom::MyCustomResource"
+)
+```
+
+## Packaging dependencies in the Lambda function
+
+Dependencies can be added to the Lambda handlers using the bundling options. For example, the following code adds the AWS SDK S3 client to the `onEvent` handler:
+
+```python
+my_provider = DsfProvider(self, "Provider",
+    provider_name="my-provider",
+    on_event_handler_definition=HandlerDefinition(
+        managed_policy=my_managed_policy,
+        handler="on-event.handler",
+        deps_lock_file_path=path.join(__dirname, "./resources/lambda/my-cr/package-lock.json"),
+        entry_file=path.join(__dirname, "./resources/lambda/my-cr/on-event.mjs"),
+        bundling=cdk.aws_lambda_nodejs.BundlingOptions(
+            node_modules=["@aws-sdk/client-s3"
+            ],
+            command_hooks={
+                "after_bundling": () => [],
+                "before_bundling": () => [
+                              'npx esbuild --version'
+                            ],
+                "before_install": () => [
+                            ]
+            }
+        )
+    )
+)
+```
+
+## Running the Custom Resource in VPC
+
+You can configure the `DsfProvider` to run all the Lambda functions within a VPC (for example in private subnets). It includes the Lambda handlers (`onEvent` and `isComplete`) and the Lambda functions used by the custom resource framework. The following configurations are available when running the custom resource in a VPC:
+
+* The VPC where you want to run the custom resource.
+* The subnets where you want to run the Lambda functions. Subnets are optional. If not configured, the construct uses the VPC default strategy to select subnets.
+* The EC2 security groups to attach to the Lambda functions. Security groups are optional. If not configured, a single security group is created for all the Lambda functions.
+
+:::danger
+The `DsfProvider` construct implements a custom process to efficiently clean up ENIs when deleting the custom resource. Without this process it can take up to one hour to delete the ENI and dependant resources.
+This process requires the security groups to be dedicated to the custom resource. If you configure security groups, ensure they are dedicated.
+:::
+
+```python
+vpc = Vpc.from_lookup(self, "Vpc", vpc_name="my-vpc")
+subnets = vpc.select_subnets(subnet_type=SubnetType.PRIVATE_WITH_EGRESS)
+security_group = SecurityGroup.from_security_group_id(self, "SecurityGroup", "sg-123456")
+
+my_provider = DsfProvider(self, "Provider",
+    provider_name="my-provider",
+    on_event_handler_definition=HandlerDefinition(
+        managed_policy=my_managed_policy,
+        handler="on-event.handler",
+        deps_lock_file_path=path.join(__dirname, "./resources/lambda/my-cr/package-lock.json"),
+        entry_file=path.join(__dirname, "./resources/lambda/my-cr/on-event.mjs")
+    ),
+    vpc=vpc,
+    subnets=subnets,
+    # the security group should be dedicated to the custom resource
+    security_groups=[security_group]
+)
 ```
 
-### grantProduce
+## Configuring environment variables of Lambda handlers
 
-This method allows to grant a `Principal` the permissions to write to a kafka topic.
-In case of IAM authentication the method attaches an IAM policy as defined in the [AWS documentation](https://docs.aws.amazon.com/msk/latest/developerguide/iam-access-control.html#iam-access-control-use-cases) scoped only to the topic provided. For mTLS authentication, the method applies an ACL for the provided `Common Name` that allow write operations on the topic.
+Lambda handlers can leverage environment variables to pass values to the Lambda code. You can configure environment variables for each of the Lambda handlers:
 
 ```python
-kafka_api.grant_produce("consume", "foo", Authentication.MTLS, "User:Cn=bar")
+my_provider = DsfProvider(self, "Provider",
+    provider_name="my-provider",
+    on_event_handler_definition=HandlerDefinition(
+        managed_policy=my_managed_policy,
+        handler="on-event.handler",
+        deps_lock_file_path=path.join(__dirname, "./resources/lambda/my-cr/package-lock.json"),
+        entry_file=path.join(__dirname, "./resources/lambda/my-cr/on-event.mjs"),
+        environment={
+            "MY_ENV_VARIABLE": "my-env-variable-value"
+        }
+    )
+)
 ```
 
-### grantConsume
+## Removal policy
+
+You can specify if the Cloudwatch Log Groups should be deleted when the CDK resource is destroyed using `removalPolicy`. To have an additional layer of protection, we require users to set a global context value for data removal in their CDK applications.
+
+Log groups can be destroyed when the CDK resource is destroyed only if **both** `DsfProvider` removal policy and DSF on AWS global removal policy are set to remove objects.
 
-This method allows to grant a `Principal` the permissions to read to a kafka topic.
-In case of IAM authentication the method attachs an IAM policy as defined in the [AWS documentation](https://docs.aws.amazon.com/msk/latest/developerguide/iam-access-control.html#iam-access-control-use-cases) scoped only to the topic provided. For mTLS authentication, the method applies an ACL for the provided `Common Name` that allow read operations on the topic.
+You can set `@data-solutions-framework-on-aws/removeDataOnDestroy` (`true` or `false`) global data removal policy in `cdk.json`:
+
+```json
+{
+  "context": {
+    "@data-solutions-framework-on-aws/removeDataOnDestroy": true
+  }
+}
+```
+
+Or programmatically in your CDK app:
 
 ```python
-kafka_api.grant_consume("consume", "foo", Authentication.MTLS, "User:Cn=bar")
+self.node.set_context("@data-solutions-framework-on-aws/removeDataOnDestroy", True)
+
+my_provider = DsfProvider(self, "Provider",
+    provider_name="my-provider",
+    on_event_handler_definition=HandlerDefinition(
+        managed_policy=my_on_event_managed_policy,
+        handler="on-event.handler",
+        deps_lock_file_path=path.join(__dirname, "./resources/lambda/my-cr/package-lock.json"),
+        entry_file=path.join(__dirname, "./resources/lambda/my-cr/on-event.mjs")
+    ),
+    removal_policy=cdk.RemovalPolicy.DESTROY
+)
 ```
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
@@ -168,1954 +445,1521 @@
 import typing_extensions
 
 from typeguard import check_type
 
 from .._jsii import *
 
 import aws_cdk as _aws_cdk_ceddda9d
-import aws_cdk.aws_acmpca as _aws_cdk_aws_acmpca_ceddda9d
 import aws_cdk.aws_ec2 as _aws_cdk_aws_ec2_ceddda9d
 import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
 import aws_cdk.aws_kms as _aws_cdk_aws_kms_ceddda9d
 import aws_cdk.aws_lambda as _aws_cdk_aws_lambda_ceddda9d
 import aws_cdk.aws_logs as _aws_cdk_aws_logs_ceddda9d
 import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
-import aws_cdk.aws_secretsmanager as _aws_cdk_aws_secretsmanager_ceddda9d
 import constructs as _constructs_77d1e7e8
 
 
-@jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.Acl",
-    jsii_struct_bases=[],
-    name_mapping={
-        "host": "host",
-        "operation": "operation",
-        "permission_type": "permissionType",
-        "principal": "principal",
-        "resource_name": "resourceName",
-        "resource_pattern_type": "resourcePatternType",
-        "resource_type": "resourceType",
-    },
-)
-class Acl:
-    def __init__(
-        self,
-        *,
-        host: builtins.str,
-        operation: "AclOperationTypes",
-        permission_type: "AclPermissionTypes",
-        principal: builtins.str,
-        resource_name: builtins.str,
-        resource_pattern_type: "ResourcePatternTypes",
-        resource_type: "AclResourceTypes",
-    ) -> None:
-        '''Kakfa ACL This is similar to the object used by ``kafkajs``, for more information see this `link <https://kafka.js.org/docs/admin#create-acl>`_.
-
-        :param host: 
-        :param operation: 
-        :param permission_type: 
-        :param principal: 
-        :param resource_name: 
-        :param resource_pattern_type: 
-        :param resource_type: 
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3b2c45eeb82912583d0e203bcc5f7cfa5d4679f4aa75359733b6a3b6d15aaa09)
-            check_type(argname="argument host", value=host, expected_type=type_hints["host"])
-            check_type(argname="argument operation", value=operation, expected_type=type_hints["operation"])
-            check_type(argname="argument permission_type", value=permission_type, expected_type=type_hints["permission_type"])
-            check_type(argname="argument principal", value=principal, expected_type=type_hints["principal"])
-            check_type(argname="argument resource_name", value=resource_name, expected_type=type_hints["resource_name"])
-            check_type(argname="argument resource_pattern_type", value=resource_pattern_type, expected_type=type_hints["resource_pattern_type"])
-            check_type(argname="argument resource_type", value=resource_type, expected_type=type_hints["resource_type"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "host": host,
-            "operation": operation,
-            "permission_type": permission_type,
-            "principal": principal,
-            "resource_name": resource_name,
-            "resource_pattern_type": resource_pattern_type,
-            "resource_type": resource_type,
-        }
-
-    @builtins.property
-    def host(self) -> builtins.str:
-        result = self._values.get("host")
-        assert result is not None, "Required property 'host' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
-    def operation(self) -> "AclOperationTypes":
-        result = self._values.get("operation")
-        assert result is not None, "Required property 'operation' is missing"
-        return typing.cast("AclOperationTypes", result)
+class ApplicationStackFactory(
+    metaclass=jsii.JSIIAbstractClass,
+    jsii_type="@cdklabs/aws-data-solutions-framework.utils.ApplicationStackFactory",
+):
+    '''Abstract class that needs to be implemented to pass the application Stack to the CICD pipeline.
 
-    @builtins.property
-    def permission_type(self) -> "AclPermissionTypes":
-        result = self._values.get("permission_type")
-        assert result is not None, "Required property 'permission_type' is missing"
-        return typing.cast("AclPermissionTypes", result)
+    :exampleMetadata: fixture=imports-only
 
-    @builtins.property
-    def principal(self) -> builtins.str:
-        result = self._values.get("principal")
-        assert result is not None, "Required property 'principal' is missing"
-        return typing.cast(builtins.str, result)
+    Example::
 
-    @builtins.property
-    def resource_name(self) -> builtins.str:
-        result = self._values.get("resource_name")
-        assert result is not None, "Required property 'resource_name' is missing"
-        return typing.cast(builtins.str, result)
+        class MyApplicationStack(cdk.Stack):
+            def __init__(self, scope, id, *, stage, description=None, env=None, stackName=None, tags=None, synthesizer=None, terminationProtection=None, analyticsReporting=None, crossRegionReferences=None, permissionsBoundary=None, suppressTemplateIndentation=None):
+                super().__init__(scope, id, stage=stage, description=description, env=env, stackName=stackName, tags=tags, synthesizer=synthesizer, terminationProtection=terminationProtection, analyticsReporting=analyticsReporting, crossRegionReferences=crossRegionReferences, permissionsBoundary=permissionsBoundary, suppressTemplateIndentation=suppressTemplateIndentation)
+        
+        class MyApplicationStackFactory(dsf.utils.ApplicationStackFactory):
+            def create_stack(self, scope, stage):
+                return MyApplicationStack(scope, "MyApplication",
+                    stage=stage
+                )
+    '''
 
-    @builtins.property
-    def resource_pattern_type(self) -> "ResourcePatternTypes":
-        result = self._values.get("resource_pattern_type")
-        assert result is not None, "Required property 'resource_pattern_type' is missing"
-        return typing.cast("ResourcePatternTypes", result)
+    def __init__(self) -> None:
+        jsii.create(self.__class__, self, [])
 
-    @builtins.property
-    def resource_type(self) -> "AclResourceTypes":
-        result = self._values.get("resource_type")
-        assert result is not None, "Required property 'resource_type' is missing"
-        return typing.cast("AclResourceTypes", result)
+    @jsii.member(jsii_name="createStack")
+    @abc.abstractmethod
+    def create_stack(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        stage: "CICDStage",
+    ) -> _aws_cdk_ceddda9d.Stack:
+        '''Abstract method that needs to be implemented to return the application Stack.
 
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
+        :param scope: The scope to create the stack in.
+        :param stage: The stage of the pipeline.
+        '''
+        ...
 
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
 
-    def __repr__(self) -> str:
-        return "Acl(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
+class _ApplicationStackFactoryProxy(ApplicationStackFactory):
+    @jsii.member(jsii_name="createStack")
+    def create_stack(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        stage: "CICDStage",
+    ) -> _aws_cdk_ceddda9d.Stack:
+        '''Abstract method that needs to be implemented to return the application Stack.
 
+        :param scope: The scope to create the stack in.
+        :param stage: The stage of the pipeline.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__4eef9172971b514785a6ce2346308753b3a0e87079b7ff4a145e5bb81378146a)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
+        return typing.cast(_aws_cdk_ceddda9d.Stack, jsii.invoke(self, "createStack", [scope, stage]))
 
-@jsii.enum(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.AclOperationTypes"
-)
-class AclOperationTypes(enum.Enum):
-    UNKNOWN = "UNKNOWN"
-    ANY = "ANY"
-    ALL = "ALL"
-    READ = "READ"
-    WRITE = "WRITE"
-    CREATE = "CREATE"
-    DELETE = "DELETE"
-    ALTER = "ALTER"
-    DESCRIBE = "DESCRIBE"
-    CLUSTER_ACTION = "CLUSTER_ACTION"
-    DESCRIBE_CONFIGS = "DESCRIBE_CONFIGS"
-    ALTER_CONFIGS = "ALTER_CONFIGS"
-    IDEMPOTENT_WRITE = "IDEMPOTENT_WRITE"
+# Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
+typing.cast(typing.Any, ApplicationStackFactory).__jsii_proxy_class__ = lambda : _ApplicationStackFactoryProxy
 
 
-@jsii.enum(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.AclPermissionTypes"
-)
-class AclPermissionTypes(enum.Enum):
-    UNKNOWN = "UNKNOWN"
-    ANY = "ANY"
-    DENY = "DENY"
-    ALLOW = "ALLOW"
+class ApplicationStage(
+    _aws_cdk_ceddda9d.Stage,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdklabs/aws-data-solutions-framework.utils.ApplicationStage",
+):
+    '''ApplicationStage class that creates a CDK Pipelines Stage from an ApplicationStackFactory.'''
 
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        application_stack_factory: ApplicationStackFactory,
+        stage: "CICDStage",
+        outputs_env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+        outdir: typing.Optional[builtins.str] = None,
+        permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
+        policy_validation_beta1: typing.Optional[typing.Sequence[_aws_cdk_ceddda9d.IPolicyValidationPluginBeta1]] = None,
+        stage_name: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''Construct a new instance of the SparkCICDStage class.
 
-@jsii.enum(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.AclResourceTypes"
-)
-class AclResourceTypes(enum.Enum):
-    UNKNOWN = "UNKNOWN"
-    ANY = "ANY"
-    TOPIC = "TOPIC"
-    GROUP = "GROUP"
-    CLUSTER = "CLUSTER"
-    TRANSACTIONAL_ID = "TRANSACTIONAL_ID"
-    DELEGATION_TOKEN = "DELEGATION_TOKEN"
+        :param scope: the Scope of the CDK Construct.
+        :param id: the ID of the CDK Construct.
+        :param application_stack_factory: The application CDK Stack Factory used to create application Stacks.
+        :param stage: The Stage to deploy the application CDK Stack in. Default: - No stage is passed to the application stack
+        :param outputs_env: The list of values to create CfnOutputs. Default: - No CfnOutputs are created
+        :param env: Default AWS environment (account/region) for ``Stack``s in this ``Stage``. Stacks defined inside this ``Stage`` with either ``region`` or ``account`` missing from its env will use the corresponding field given here. If either ``region`` or ``account``is is not configured for ``Stack`` (either on the ``Stack`` itself or on the containing ``Stage``), the Stack will be *environment-agnostic*. Environment-agnostic stacks can be deployed to any environment, may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups, will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environments should be configured on the ``Stack``s.
+        :param outdir: The output directory into which to emit synthesized artifacts. Can only be specified if this stage is the root stage (the app). If this is specified and this stage is nested within another stage, an error will be thrown. Default: - for nested stages, outdir will be determined as a relative directory to the outdir of the app. For apps, if outdir is not specified, a temporary directory will be created.
+        :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
+        :param policy_validation_beta1: Validation plugins to run during synthesis. If any plugin reports any violation, synthesis will be interrupted and the report displayed to the user. Default: - no validation plugins are used
+        :param stage_name: Name of this stage. Default: - Derived from the id.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d5b5ac3de86725230614eaa05d4d588181e4795f348801b8e9846f7a8ade6698)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = ApplicationStageProps(
+            application_stack_factory=application_stack_factory,
+            stage=stage,
+            outputs_env=outputs_env,
+            env=env,
+            outdir=outdir,
+            permissions_boundary=permissions_boundary,
+            policy_validation_beta1=policy_validation_beta1,
+            stage_name=stage_name,
+        )
 
+        jsii.create(self.__class__, self, [scope, id, props])
 
-@jsii.enum(jsii_type="@cdklabs/aws-data-solutions-framework.streaming.Authentication")
-class Authentication(enum.Enum):
-    IAM = "IAM"
-    MTLS = "MTLS"
+    @builtins.property
+    @jsii.member(jsii_name="stackOutputsEnv")
+    def stack_outputs_env(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, _aws_cdk_ceddda9d.CfnOutput]]:
+        '''The list of CfnOutputs created by the CDK Stack.'''
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, _aws_cdk_ceddda9d.CfnOutput]], jsii.get(self, "stackOutputsEnv"))
 
 
 @jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.BrokerLogging",
-    jsii_struct_bases=[],
+    jsii_type="@cdklabs/aws-data-solutions-framework.utils.ApplicationStageProps",
+    jsii_struct_bases=[_aws_cdk_ceddda9d.StageProps],
     name_mapping={
-        "cloudwatch_log_group": "cloudwatchLogGroup",
-        "firehose_delivery_stream_name": "firehoseDeliveryStreamName",
-        "s3": "s3",
+        "env": "env",
+        "outdir": "outdir",
+        "permissions_boundary": "permissionsBoundary",
+        "policy_validation_beta1": "policyValidationBeta1",
+        "stage_name": "stageName",
+        "application_stack_factory": "applicationStackFactory",
+        "stage": "stage",
+        "outputs_env": "outputsEnv",
     },
 )
-class BrokerLogging:
+class ApplicationStageProps(_aws_cdk_ceddda9d.StageProps):
     def __init__(
         self,
         *,
-        cloudwatch_log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
-        firehose_delivery_stream_name: typing.Optional[builtins.str] = None,
-        s3: typing.Optional[typing.Union["S3LoggingConfiguration", typing.Dict[builtins.str, typing.Any]]] = None,
+        env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+        outdir: typing.Optional[builtins.str] = None,
+        permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
+        policy_validation_beta1: typing.Optional[typing.Sequence[_aws_cdk_ceddda9d.IPolicyValidationPluginBeta1]] = None,
+        stage_name: typing.Optional[builtins.str] = None,
+        application_stack_factory: ApplicationStackFactory,
+        stage: "CICDStage",
+        outputs_env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     ) -> None:
-        '''Configuration details related to broker logs.
+        '''Properties for the ``ApplicationStage`` class.
 
-        :param cloudwatch_log_group: The CloudWatch Logs group that is the destination for broker logs. Default: - disabled
-        :param firehose_delivery_stream_name: The Kinesis Data Firehose delivery stream that is the destination for broker logs. Default: - disabled
-        :param s3: Details of the Amazon S3 destination for broker logs. Default: - disabled
+        :param env: Default AWS environment (account/region) for ``Stack``s in this ``Stage``. Stacks defined inside this ``Stage`` with either ``region`` or ``account`` missing from its env will use the corresponding field given here. If either ``region`` or ``account``is is not configured for ``Stack`` (either on the ``Stack`` itself or on the containing ``Stage``), the Stack will be *environment-agnostic*. Environment-agnostic stacks can be deployed to any environment, may not be able to take advantage of all features of the CDK. For example, they will not be able to use environmental context lookups, will not automatically translate Service Principals to the right format based on the environment's AWS partition, and other such enhancements. Default: - The environments should be configured on the ``Stack``s.
+        :param outdir: The output directory into which to emit synthesized artifacts. Can only be specified if this stage is the root stage (the app). If this is specified and this stage is nested within another stage, an error will be thrown. Default: - for nested stages, outdir will be determined as a relative directory to the outdir of the app. For apps, if outdir is not specified, a temporary directory will be created.
+        :param permissions_boundary: Options for applying a permissions boundary to all IAM Roles and Users created within this Stage. Default: - no permissions boundary is applied
+        :param policy_validation_beta1: Validation plugins to run during synthesis. If any plugin reports any violation, synthesis will be interrupted and the report displayed to the user. Default: - no validation plugins are used
+        :param stage_name: Name of this stage. Default: - Derived from the id.
+        :param application_stack_factory: The application CDK Stack Factory used to create application Stacks.
+        :param stage: The Stage to deploy the application CDK Stack in. Default: - No stage is passed to the application stack
+        :param outputs_env: The list of values to create CfnOutputs. Default: - No CfnOutputs are created
         '''
-        if isinstance(s3, dict):
-            s3 = S3LoggingConfiguration(**s3)
+        if isinstance(env, dict):
+            env = _aws_cdk_ceddda9d.Environment(**env)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bcf29df229d45be6f58cf96f7c79a3fd20c67254205e0d4bf24c15fc1917467f)
-            check_type(argname="argument cloudwatch_log_group", value=cloudwatch_log_group, expected_type=type_hints["cloudwatch_log_group"])
-            check_type(argname="argument firehose_delivery_stream_name", value=firehose_delivery_stream_name, expected_type=type_hints["firehose_delivery_stream_name"])
-            check_type(argname="argument s3", value=s3, expected_type=type_hints["s3"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if cloudwatch_log_group is not None:
-            self._values["cloudwatch_log_group"] = cloudwatch_log_group
-        if firehose_delivery_stream_name is not None:
-            self._values["firehose_delivery_stream_name"] = firehose_delivery_stream_name
-        if s3 is not None:
-            self._values["s3"] = s3
-
-    @builtins.property
-    def cloudwatch_log_group(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
-        '''The CloudWatch Logs group that is the destination for broker logs.
-
-        :default: - disabled
-        '''
-        result = self._values.get("cloudwatch_log_group")
-        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], result)
-
-    @builtins.property
-    def firehose_delivery_stream_name(self) -> typing.Optional[builtins.str]:
-        '''The Kinesis Data Firehose delivery stream that is the destination for broker logs.
-
-        :default: - disabled
+            type_hints = typing.get_type_hints(_typecheckingstub__0d0cd7bb2c6f89ceae419e95586371f2db805a9f35f0aa2ec97dcf48aa8c0209)
+            check_type(argname="argument env", value=env, expected_type=type_hints["env"])
+            check_type(argname="argument outdir", value=outdir, expected_type=type_hints["outdir"])
+            check_type(argname="argument permissions_boundary", value=permissions_boundary, expected_type=type_hints["permissions_boundary"])
+            check_type(argname="argument policy_validation_beta1", value=policy_validation_beta1, expected_type=type_hints["policy_validation_beta1"])
+            check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
+            check_type(argname="argument application_stack_factory", value=application_stack_factory, expected_type=type_hints["application_stack_factory"])
+            check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
+            check_type(argname="argument outputs_env", value=outputs_env, expected_type=type_hints["outputs_env"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "application_stack_factory": application_stack_factory,
+            "stage": stage,
+        }
+        if env is not None:
+            self._values["env"] = env
+        if outdir is not None:
+            self._values["outdir"] = outdir
+        if permissions_boundary is not None:
+            self._values["permissions_boundary"] = permissions_boundary
+        if policy_validation_beta1 is not None:
+            self._values["policy_validation_beta1"] = policy_validation_beta1
+        if stage_name is not None:
+            self._values["stage_name"] = stage_name
+        if outputs_env is not None:
+            self._values["outputs_env"] = outputs_env
+
+    @builtins.property
+    def env(self) -> typing.Optional[_aws_cdk_ceddda9d.Environment]:
+        '''Default AWS environment (account/region) for ``Stack``s in this ``Stage``.
+
+        Stacks defined inside this ``Stage`` with either ``region`` or ``account`` missing
+        from its env will use the corresponding field given here.
+
+        If either ``region`` or ``account``is is not configured for ``Stack`` (either on
+        the ``Stack`` itself or on the containing ``Stage``), the Stack will be
+        *environment-agnostic*.
+
+        Environment-agnostic stacks can be deployed to any environment, may not be
+        able to take advantage of all features of the CDK. For example, they will
+        not be able to use environmental context lookups, will not automatically
+        translate Service Principals to the right format based on the environment's
+        AWS partition, and other such enhancements.
+
+        :default: - The environments should be configured on the ``Stack``s.
+
+        Example::
+
+            // Use a concrete account and region to deploy this Stage to
+            new Stage(app, 'Stage1', {
+              env: { account: '123456789012', region: 'us-east-1' },
+            });
+            
+            // Use the CLI's current credentials to determine the target environment
+            new Stage(app, 'Stage2', {
+              env: { account: process.env.CDK_DEFAULT_ACCOUNT, region: process.env.CDK_DEFAULT_REGION },
+            });
+        '''
+        result = self._values.get("env")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Environment], result)
+
+    @builtins.property
+    def outdir(self) -> typing.Optional[builtins.str]:
+        '''The output directory into which to emit synthesized artifacts.
+
+        Can only be specified if this stage is the root stage (the app). If this is
+        specified and this stage is nested within another stage, an error will be
+        thrown.
+
+        :default:
+
+        - for nested stages, outdir will be determined as a relative
+        directory to the outdir of the app. For apps, if outdir is not specified, a
+        temporary directory will be created.
         '''
-        result = self._values.get("firehose_delivery_stream_name")
+        result = self._values.get("outdir")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def s3(self) -> typing.Optional["S3LoggingConfiguration"]:
-        '''Details of the Amazon S3 destination for broker logs.
-
-        :default: - disabled
-        '''
-        result = self._values.get("s3")
-        return typing.cast(typing.Optional["S3LoggingConfiguration"], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "BrokerLogging(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
-class ClientAuthentication(
-    metaclass=jsii.JSIIMeta,
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.ClientAuthentication",
-):
-    '''Configuration properties for client authentication.'''
-
-    @jsii.member(jsii_name="sasl")
-    @builtins.classmethod
-    def sasl(
-        cls,
-        *,
-        iam: typing.Optional[builtins.bool] = None,
-    ) -> "ClientAuthentication":
-        '''SASL authentication.
+    def permissions_boundary(
+        self,
+    ) -> typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary]:
+        '''Options for applying a permissions boundary to all IAM Roles and Users created within this Stage.
 
-        :param iam: Enable IAM access control. Default: true
+        :default: - no permissions boundary is applied
         '''
-        props = SaslAuthProps(iam=iam)
+        result = self._values.get("permissions_boundary")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary], result)
 
-        return typing.cast("ClientAuthentication", jsii.sinvoke(cls, "sasl", [props]))
+    @builtins.property
+    def policy_validation_beta1(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_ceddda9d.IPolicyValidationPluginBeta1]]:
+        '''Validation plugins to run during synthesis.
 
-    @jsii.member(jsii_name="saslTls")
-    @builtins.classmethod
-    def sasl_tls(
-        cls,
-        *,
-        iam: typing.Optional[builtins.bool] = None,
-        certificate_authorities: typing.Optional[typing.Sequence[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]] = None,
-    ) -> "ClientAuthentication":
-        '''SASL + TLS authentication.
+        If any plugin reports any violation,
+        synthesis will be interrupted and the report displayed to the user.
 
-        :param iam: Enable IAM access control. Default: true
-        :param certificate_authorities: List of ACM Certificate Authorities to enable TLS authentication. Default: - none
+        :default: - no validation plugins are used
         '''
-        sasl_tls_props = SaslTlsAuthProps(
-            iam=iam, certificate_authorities=certificate_authorities
-        )
+        result = self._values.get("policy_validation_beta1")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_ceddda9d.IPolicyValidationPluginBeta1]], result)
 
-        return typing.cast("ClientAuthentication", jsii.sinvoke(cls, "saslTls", [sasl_tls_props]))
-
-    @jsii.member(jsii_name="tls")
-    @builtins.classmethod
-    def tls(
-        cls,
-        *,
-        certificate_authorities: typing.Optional[typing.Sequence[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]] = None,
-    ) -> "ClientAuthentication":
-        '''TLS authentication.
+    @builtins.property
+    def stage_name(self) -> typing.Optional[builtins.str]:
+        '''Name of this stage.
 
-        :param certificate_authorities: List of ACM Certificate Authorities to enable TLS authentication. Default: - none
+        :default: - Derived from the id.
         '''
-        props = TlsAuthProps(certificate_authorities=certificate_authorities)
-
-        return typing.cast("ClientAuthentication", jsii.sinvoke(cls, "tls", [props]))
+        result = self._values.get("stage_name")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="saslProps")
-    def sasl_props(self) -> typing.Optional["SaslAuthProps"]:
-        '''- properties for SASL authentication.'''
-        return typing.cast(typing.Optional["SaslAuthProps"], jsii.get(self, "saslProps"))
+    def application_stack_factory(self) -> ApplicationStackFactory:
+        '''The application CDK Stack Factory used to create application Stacks.'''
+        result = self._values.get("application_stack_factory")
+        assert result is not None, "Required property 'application_stack_factory' is missing"
+        return typing.cast(ApplicationStackFactory, result)
 
     @builtins.property
-    @jsii.member(jsii_name="tlsProps")
-    def tls_props(self) -> typing.Optional["TlsAuthProps"]:
-        '''- properties for TLS authentication.'''
-        return typing.cast(typing.Optional["TlsAuthProps"], jsii.get(self, "tlsProps"))
-
-
-@jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.ClusterConfigurationInfo",
-    jsii_struct_bases=[],
-    name_mapping={"arn": "arn", "revision": "revision"},
-)
-class ClusterConfigurationInfo:
-    def __init__(self, *, arn: builtins.str, revision: jsii.Number) -> None:
-        '''The Amazon MSK configuration to use for the cluster.
+    def stage(self) -> "CICDStage":
+        '''The Stage to deploy the application CDK Stack in.
 
-        Note: There is currently no Cloudformation Resource to create a Configuration
-
-        :param arn: The Amazon Resource Name (ARN) of the MSK configuration to use. For example, arn:aws:kafka:us-east-1:123456789012:configuration/example-configuration-name/abcdabcd-1234-abcd-1234-abcd123e8e8e-1.
-        :param revision: The revision of the Amazon MSK configuration to use.
+        :default: - No stage is passed to the application stack
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3836211b99f5c6335752911fac90a01a7d51a80694071ca21e83d6ed9e4ccd6e)
-            check_type(argname="argument arn", value=arn, expected_type=type_hints["arn"])
-            check_type(argname="argument revision", value=revision, expected_type=type_hints["revision"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "arn": arn,
-            "revision": revision,
-        }
+        result = self._values.get("stage")
+        assert result is not None, "Required property 'stage' is missing"
+        return typing.cast("CICDStage", result)
 
     @builtins.property
-    def arn(self) -> builtins.str:
-        '''The Amazon Resource Name (ARN) of the MSK configuration to use.
+    def outputs_env(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        '''The list of values to create CfnOutputs.
 
-        For example, arn:aws:kafka:us-east-1:123456789012:configuration/example-configuration-name/abcdabcd-1234-abcd-1234-abcd123e8e8e-1.
+        :default: - No CfnOutputs are created
         '''
-        result = self._values.get("arn")
-        assert result is not None, "Required property 'arn' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
-    def revision(self) -> jsii.Number:
-        '''The revision of the Amazon MSK configuration to use.'''
-        result = self._values.get("revision")
-        assert result is not None, "Required property 'revision' is missing"
-        return typing.cast(jsii.Number, result)
+        result = self._values.get("outputs_env")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "ClusterConfigurationInfo(%s)" % ", ".join(
+        return "ApplicationStageProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.enum(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.ClusterMonitoringLevel"
-)
-class ClusterMonitoringLevel(enum.Enum):
-    '''The level of monitoring for the MSK cluster.
-
-    :see: https://docs.aws.amazon.com/msk/latest/developerguide/monitoring.html#metrics-details
-    '''
-
-    DEFAULT = "DEFAULT"
-    '''Default metrics are the essential metrics to monitor.'''
-    PER_BROKER = "PER_BROKER"
-    '''Per Broker metrics give you metrics at the broker level.'''
-    PER_TOPIC_PER_BROKER = "PER_TOPIC_PER_BROKER"
-    '''Per Topic Per Broker metrics help you understand volume at the topic level.'''
-    PER_TOPIC_PER_PARTITION = "PER_TOPIC_PER_PARTITION"
-    '''Per Topic Per Partition metrics help you understand consumer group lag at the topic partition level.'''
-
+@jsii.enum(jsii_type="@cdklabs/aws-data-solutions-framework.utils.Architecture")
+class Architecture(enum.Enum):
+    '''List of supported CPU architecture, either  X86_64 or ARM64.'''
 
-@jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.EbsStorageInfo",
-    jsii_struct_bases=[],
-    name_mapping={"encryption_key": "encryptionKey", "volume_size": "volumeSize"},
-)
-class EbsStorageInfo:
-    def __init__(
-        self,
-        *,
-        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-        volume_size: typing.Optional[jsii.Number] = None,
-    ) -> None:
-        '''EBS volume information.
+    X86_64 = "X86_64"
+    ARM64 = "ARM64"
 
-        :param encryption_key: The AWS KMS key for encrypting data at rest. Default: Uses AWS managed CMK (aws/kafka)
-        :param volume_size: The size in GiB of the EBS volume for the data drive on each broker node. Default: 1000
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3425efae5f0d6400892f5926740e3aa84485ca386ae41ba733ecaca3e0d2825d)
-            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
-            check_type(argname="argument volume_size", value=volume_size, expected_type=type_hints["volume_size"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if encryption_key is not None:
-            self._values["encryption_key"] = encryption_key
-        if volume_size is not None:
-            self._values["volume_size"] = volume_size
 
-    @builtins.property
-    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
-        '''The AWS KMS key for encrypting data at rest.
+class BucketUtils(
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdklabs/aws-data-solutions-framework.utils.BucketUtils",
+):
+    '''Utils for working with Amazon S3 Buckets.'''
 
-        :default: Uses AWS managed CMK (aws/kafka)
-        '''
-        result = self._values.get("encryption_key")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+    def __init__(self) -> None:
+        jsii.create(self.__class__, self, [])
 
-    @builtins.property
-    def volume_size(self) -> typing.Optional[jsii.Number]:
-        '''The size in GiB of the EBS volume for the data drive on each broker node.
+    @jsii.member(jsii_name="generateUniqueBucketName")
+    @builtins.classmethod
+    def generate_unique_bucket_name(
+        cls,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        name: builtins.str,
+    ) -> builtins.str:
+        '''Generate a unique Amazon S3 bucket name based on the provided name, CDK construct ID and CDK construct scope.
+
+        The bucket name is suffixed the AWS account ID, the AWS region and a unique 8 characters hash.
+        The maximum length for name is 26 characters.
+
+        :param scope: the current scope where the construct is created (generally ``this``).
+        :param id: the CDK ID of the construct.
+        :param name: the name of the bucket.
 
-        :default: 1000
+        :return: the unique Name for the bucket
         '''
-        result = self._values.get("volume_size")
-        return typing.cast(typing.Optional[jsii.Number], result)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__88bcefb5e5ed5389168d4178ba329d512cd1938b816b8cfe7bc44a5b3124986f)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+        return typing.cast(builtins.str, jsii.sinvoke(cls, "generateUniqueBucketName", [scope, id, name]))
 
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
 
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
+@jsii.enum(jsii_type="@cdklabs/aws-data-solutions-framework.utils.CICDStage")
+class CICDStage(enum.Enum):
+    '''The list of CICD Stages used in CICD Pipelines.'''
 
-    def __repr__(self) -> str:
-        return "EbsStorageInfo(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
+    STAGING = "STAGING"
+    PROD = "PROD"
 
 
-class KafkaApi(
+class DataVpc(
     _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.KafkaApi",
+    jsii_type="@cdklabs/aws-data-solutions-framework.utils.DataVpc",
 ):
-    '''A construct to create an MSK Serverless cluster.
+    '''Creates a VPC with best practices for securely deploying data solutions.
 
-    :see: https://awslabs.github.io/data-solutions-framework-on-aws/
+    :see: https://awslabs.github.io/data-solutions-framework-on-aws/docs/constructs/library/Utils/data-vpc
+
+    Example::
+
+        vpc = dsf.utils.DataVpc(self, "DataVpc",
+            vpc_cidr="10.0.0.0/16"
+        )
+        
+        vpc.tag_vpc("Name", "My VPC")
     '''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        broker_security_group: _aws_cdk_aws_ec2_ceddda9d.ISecurityGroup,
-        client_authentication: ClientAuthentication,
-        cluster_arn: builtins.str,
-        cluster_type: "MskClusterType",
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-        certficate_secret: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-        iam_handler_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        kafka_client_log_level: typing.Optional["KafkaClientLogLevel"] = None,
-        mtls_handler_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        vpc_cidr: builtins.str,
+        client_vpn_endpoint_props: typing.Optional[typing.Union["DataVpcClientVpnEndpointProps", typing.Dict[builtins.str, typing.Any]]] = None,
+        flow_log_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        flow_log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
+        flow_log_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        nat_gateways: typing.Optional[jsii.Number] = None,
         removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-        subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
-        '''Constructs a new instance of the EmrEksCluster construct.
-
-        :param scope: the Scope of the CDK Construct.
-        :param id: the ID of the CDK Construct.
-        :param broker_security_group: The AWS security groups to associate with the elastic network interfaces in order to specify who can connect to and communicate with the Amazon MSK cluster.
-        :param client_authentication: Configuration properties for client authentication. MSK supports using private TLS certificates or SASL/SCRAM to authenticate the identity of clients.
-        :param cluster_arn: The ARN of the cluster.
-        :param cluster_type: The type of MSK cluster(provisioned or serverless).
-        :param vpc: Defines the virtual networking environment for this cluster. Must have at least 2 subnets in two different AZs.
-        :param certficate_secret: This is the TLS certificate of the Principal that is used by the CDK custom resource which set ACLs and Topics. It must be provided if the cluster is using mTLS authentication. The secret in AWS secrets manager must be a JSON in the following format { "key" : "PRIVATE-KEY", "cert" : "CERTIFICATE" } You can use the following utility to generate the certificates https://github.com/aws-samples/amazon-msk-client-authentication
-        :param iam_handler_role: The IAM role to pass to IAM authentication lambda handler This role must be able to be assumed with ``lambda.amazonaws.com`` service principal.
-        :param kafka_client_log_level: The log level for the lambda that support the Custom Resource for both Managing ACLs and Topics. Default: WARN
-        :param mtls_handler_role: The IAM role to pass to mTLS lambda handler This role must be able to be assumed with ``lambda.amazonaws.com`` service principal.
-        :param removal_policy: The removal policy when deleting the CDK resource. If DESTROY is selected, context value ``@data-solutions-framework-on-aws/removeDataOnDestroy`` needs to be set to true. Otherwise the removalPolicy is reverted to RETAIN. Default: - The resources are not deleted (``RemovalPolicy.RETAIN``).
-        :param subnets: The subnets where the Custom Resource Lambda Function would be created in. Default: - One private subnet with egress is used per AZ.
+        '''
+        :param scope: -
+        :param id: -
+        :param vpc_cidr: The CIDR to use to create the subnets in the VPC.
+        :param client_vpn_endpoint_props: ClientVpnEndpoint propertioes. Required if client vpn endpoint is needed Default: None
+        :param flow_log_key: The KMS key used to encrypt the VPC Flow Logs in the CloudWatch Log Group. The resource policy of the key must be configured according to the AWS documentation. Default: - A new KMS key is created
+        :param flow_log_retention: The retention period to apply to VPC Flow Logs. Default: - One week retention
+        :param flow_log_role: The IAM Role used to send the VPC Flow Logs in CloudWatch. The role must be configured as described in the AWS VPC Flow Log documentation. Default: - A new IAM role is created
+        :param nat_gateways: Number of NAT Gateways. Default: 3 or the AZs defined in the context
+        :param removal_policy: The removal policy when deleting the CDK resource. If DESTROY is selected, context value ``@data-solutions-framework-on-aws/removeDataOnDestroy`` needs to be set to true. Otherwise, the removalPolicy is reverted to RETAIN. Default: - The resources are not deleted (``RemovalPolicy.RETAIN``).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__11acb7f10ba2c540e3c133ed7f79f6ef73b1fa3e856e07fb966b40a1ffd34dc4)
+            type_hints = typing.get_type_hints(_typecheckingstub__9563cd6cefb38ed980d4672a429ac3bfb7e0fdf90feea5a4f416b4ff13b018a7)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        props = KafkaApiProps(
-            broker_security_group=broker_security_group,
-            client_authentication=client_authentication,
-            cluster_arn=cluster_arn,
-            cluster_type=cluster_type,
-            vpc=vpc,
-            certficate_secret=certficate_secret,
-            iam_handler_role=iam_handler_role,
-            kafka_client_log_level=kafka_client_log_level,
-            mtls_handler_role=mtls_handler_role,
+        props = DataVpcProps(
+            vpc_cidr=vpc_cidr,
+            client_vpn_endpoint_props=client_vpn_endpoint_props,
+            flow_log_key=flow_log_key,
+            flow_log_retention=flow_log_retention,
+            flow_log_role=flow_log_role,
+            nat_gateways=nat_gateways,
             removal_policy=removal_policy,
-            subnets=subnets,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.member(jsii_name="grantConsume")
-    def grant_consume(
-        self,
-        id: builtins.str,
-        topic_name: builtins.str,
-        client_authentication: Authentication,
-        principal: typing.Union[builtins.str, _aws_cdk_aws_iam_ceddda9d.IPrincipal],
-        host: typing.Optional[builtins.str] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    ) -> typing.Optional[_aws_cdk_ceddda9d.CustomResource]:
-        '''Grant a principal the right to consume data from a topic.
-
-        :param id: the CDK resource id.
-        :param topic_name: the topic to which the principal can produce data.
-        :param client_authentication: The client authentication to use when grant on resource.
-        :param principal: the IAM principal to grand the produce to.
-        :param host: the host to which the principal can produce data.
-        :param removal_policy: the removal policy to apply to the grant.
-
-        :default: - RETAIN is used
+    @jsii.member(jsii_name="tagVpc")
+    def tag_vpc(self, key: builtins.str, value: builtins.str) -> None:
+        '''Tag the VPC and the subnets.
 
-        :return:
-
-        When MTLS is used as authentication an ACL is created using the MskAcl Custom resource to read from the topic is created and returned,
-        you can use it to add dependency on it.
+        :param key: the tag key.
+        :param value: the tag value.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b17087c46184134a6bdd689601d720ab914b7b56ad32b934fcad3f4c51f29dd0)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument topic_name", value=topic_name, expected_type=type_hints["topic_name"])
-            check_type(argname="argument client_authentication", value=client_authentication, expected_type=type_hints["client_authentication"])
-            check_type(argname="argument principal", value=principal, expected_type=type_hints["principal"])
-            check_type(argname="argument host", value=host, expected_type=type_hints["host"])
-            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.CustomResource], jsii.invoke(self, "grantConsume", [id, topic_name, client_authentication, principal, host, removal_policy]))
-
-    @jsii.member(jsii_name="grantProduce")
-    def grant_produce(
-        self,
-        id: builtins.str,
-        topic_name: builtins.str,
-        client_authentication: Authentication,
-        principal: typing.Union[builtins.str, _aws_cdk_aws_iam_ceddda9d.IPrincipal],
-        host: typing.Optional[builtins.str] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    ) -> typing.Optional[_aws_cdk_ceddda9d.CustomResource]:
-        '''Grant a principal to produce data to a topic.
-
-        :param id: the CDK resource id.
-        :param topic_name: the topic to which the principal can produce data.
-        :param client_authentication: The client authentication to use when grant on resource.
-        :param principal: the IAM principal to grand the produce to.
-        :param host: the host to which the principal can produce data.
-        :param removal_policy: the removal policy to apply to the grant.
-
-        :default: - RETAIN is used
-
-        :return:
-
-        When MTLS is used as authentication an ACL is created using the MskAcl Custom resource to write in the topic is created and returned,
-        you can use it to add dependency on it.
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9c253515c374085f1ae8c19e0362e4924e1a2b781d754123dce2804908888e67)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument topic_name", value=topic_name, expected_type=type_hints["topic_name"])
-            check_type(argname="argument client_authentication", value=client_authentication, expected_type=type_hints["client_authentication"])
-            check_type(argname="argument principal", value=principal, expected_type=type_hints["principal"])
-            check_type(argname="argument host", value=host, expected_type=type_hints["host"])
-            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.CustomResource], jsii.invoke(self, "grantProduce", [id, topic_name, client_authentication, principal, host, removal_policy]))
-
-    @jsii.member(jsii_name="retrieveVersion")
-    def retrieve_version(self) -> typing.Any:
-        '''Retrieve DSF package.json version.'''
-        return typing.cast(typing.Any, jsii.invoke(self, "retrieveVersion", []))
-
-    @jsii.member(jsii_name="setAcl")
-    def set_acl(
-        self,
-        id: builtins.str,
-        acl_definition: typing.Union[Acl, typing.Dict[builtins.str, typing.Any]],
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    ) -> _aws_cdk_ceddda9d.CustomResource:
-        '''Creates a topic in the Msk Cluster.
-
-        :param id: the CDK id for Topic.
-        :param acl_definition: the Kafka Acl definition.
-        :param removal_policy: Wether to keep the ACL or delete it when removing the resource from the Stack.
-
-        :default: - RemovalPolicy.RETAIN
-
-        :return: The MskAcl custom resource created
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0d1c462aeb2582babda671003a454ea0e7a7fec802c2e877a39480d04de2a004)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument acl_definition", value=acl_definition, expected_type=type_hints["acl_definition"])
-            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
-        return typing.cast(_aws_cdk_ceddda9d.CustomResource, jsii.invoke(self, "setAcl", [id, acl_definition, removal_policy]))
-
-    @jsii.member(jsii_name="setTopic")
-    def set_topic(
-        self,
-        id: builtins.str,
-        client_authentication: Authentication,
-        topic_definition: typing.Union["MskTopic", typing.Dict[builtins.str, typing.Any]],
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-        wait_for_leaders: typing.Optional[builtins.bool] = None,
-        timeout: typing.Optional[jsii.Number] = None,
-    ) -> _aws_cdk_ceddda9d.CustomResource:
-        '''Creates a topic in the Msk Cluster.
-
-        :param id: the CDK id for Topic.
-        :param client_authentication: The client authentication to use when creating the Topic.
-        :param topic_definition: the Kafka topic definition.
-        :param removal_policy: Wether to keep the topic or delete it when removing the resource from the Stack.
-        :param wait_for_leaders: If this is true it will wait until metadata for the new topics doesn't throw LEADER_NOT_AVAILABLE.
-        :param timeout: The time in ms to wait for a topic to be completely created on the controller node.
-
-        :default: - 5000
-
-        :return: The MskTopic custom resource created
-        '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0906adf996cc3e4500527d7cc602db45099025693a3968a806f5ecab7596d1bf)
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument client_authentication", value=client_authentication, expected_type=type_hints["client_authentication"])
-            check_type(argname="argument topic_definition", value=topic_definition, expected_type=type_hints["topic_definition"])
-            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
-            check_type(argname="argument wait_for_leaders", value=wait_for_leaders, expected_type=type_hints["wait_for_leaders"])
-            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
-        return typing.cast(_aws_cdk_ceddda9d.CustomResource, jsii.invoke(self, "setTopic", [id, client_authentication, topic_definition, removal_policy, wait_for_leaders, timeout]))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="DSF_OWNED_TAG")
-    def DSF_OWNED_TAG(cls) -> builtins.str:
-        return typing.cast(builtins.str, jsii.sget(cls, "DSF_OWNED_TAG"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="DSF_TRACKING_CODE")
-    def DSF_TRACKING_CODE(cls) -> builtins.str:
-        return typing.cast(builtins.str, jsii.sget(cls, "DSF_TRACKING_CODE"))
+            type_hints = typing.get_type_hints(_typecheckingstub__006cefc76fdc1dca834321b036a66ceab95669c6f8f2eb4389a95b6405c5ca3a)
+            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        return typing.cast(None, jsii.invoke(self, "tagVpc", [key, value]))
 
     @builtins.property
-    @jsii.member(jsii_name="mskAclFunction")
-    def msk_acl_function(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IFunction]:
-        '''The Lambda function used by the Custom Resource provider when MSK is using mTLS authentication.'''
-        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IFunction], jsii.get(self, "mskAclFunction"))
+    @jsii.member(jsii_name="flowLogGroup")
+    def flow_log_group(self) -> _aws_cdk_aws_logs_ceddda9d.ILogGroup:
+        '''The CloudWatch Log Group created for the VPC flow logs.'''
+        return typing.cast(_aws_cdk_aws_logs_ceddda9d.ILogGroup, jsii.get(self, "flowLogGroup"))
 
     @builtins.property
-    @jsii.member(jsii_name="mskAclLogGroup")
-    def msk_acl_log_group(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
-        '''The Cloudwatch Log Group used by the Custom Resource provider when MSK is using mTLS authentication.'''
-        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], jsii.get(self, "mskAclLogGroup"))
+    @jsii.member(jsii_name="flowLogKey")
+    def flow_log_key(self) -> _aws_cdk_aws_kms_ceddda9d.IKey:
+        '''The KMS Key used to encrypt VPC flow logs.'''
+        return typing.cast(_aws_cdk_aws_kms_ceddda9d.IKey, jsii.get(self, "flowLogKey"))
 
     @builtins.property
-    @jsii.member(jsii_name="mskAclRole")
-    def msk_acl_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
-        '''The IAM Role used by the Custom Resource provider when MSK is using mTLS authentication.'''
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], jsii.get(self, "mskAclRole"))
+    @jsii.member(jsii_name="flowLogRole")
+    def flow_log_role(self) -> _aws_cdk_aws_iam_ceddda9d.IRole:
+        '''The IAM role used to publish VPC Flow Logs.'''
+        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IRole, jsii.get(self, "flowLogRole"))
 
     @builtins.property
-    @jsii.member(jsii_name="mskAclSecurityGroup")
-    def msk_acl_security_group(
-        self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
-        '''The Security Group used by the Custom Resource provider when MSK is using mTLS authentication.'''
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], jsii.get(self, "mskAclSecurityGroup"))
+    @jsii.member(jsii_name="s3VpcEndpoint")
+    def s3_vpc_endpoint(self) -> _aws_cdk_aws_ec2_ceddda9d.IGatewayVpcEndpoint:
+        '''The S3 VPC endpoint gateway.'''
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IGatewayVpcEndpoint, jsii.get(self, "s3VpcEndpoint"))
 
     @builtins.property
-    @jsii.member(jsii_name="mskIamFunction")
-    def msk_iam_function(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IFunction]:
-        '''The Lambda function used by the Custom Resource provider when MSK is using IAM authentication.'''
-        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IFunction], jsii.get(self, "mskIamFunction"))
+    @jsii.member(jsii_name="vpc")
+    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.Vpc:
+        '''The amazon VPC created.'''
+        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.Vpc, jsii.get(self, "vpc"))
 
     @builtins.property
-    @jsii.member(jsii_name="mskIamLogGroup")
-    def msk_iam_log_group(
+    @jsii.member(jsii_name="clientVpnEndpoint")
+    def client_vpn_endpoint(
         self,
-    ) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
-        '''The Cloudwatch Log Group used by the Custom Resource provider when MSK is using IAM authentication.'''
-        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], jsii.get(self, "mskIamLogGroup"))
+    ) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ClientVpnEndpoint]:
+        '''The Client VPN Endpoint.'''
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ClientVpnEndpoint], jsii.get(self, "clientVpnEndpoint"))
 
     @builtins.property
-    @jsii.member(jsii_name="mskIamRole")
-    def msk_iam_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
-        '''The IAM Role used by the Custom Resource provider when MSK is using IAM authentication.'''
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], jsii.get(self, "mskIamRole"))
+    @jsii.member(jsii_name="vpnLogGroup")
+    def vpn_log_group(self) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
+        '''The log group for Client VPN Endpoint.'''
+        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], jsii.get(self, "vpnLogGroup"))
 
     @builtins.property
-    @jsii.member(jsii_name="mskIamSecurityGroup")
-    def msk_iam_security_group(
+    @jsii.member(jsii_name="vpnSecurityGroups")
+    def vpn_security_groups(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
-        '''The Security Group used by the Custom Resource provider when MSK is using IAM authentication.'''
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], jsii.get(self, "mskIamSecurityGroup"))
+        '''The security group for Client VPN Endpoint.'''
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], jsii.get(self, "vpnSecurityGroups"))
 
 
 @jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.KafkaApiProps",
+    jsii_type="@cdklabs/aws-data-solutions-framework.utils.DataVpcClientVpnEndpointProps",
     jsii_struct_bases=[],
     name_mapping={
-        "broker_security_group": "brokerSecurityGroup",
-        "client_authentication": "clientAuthentication",
-        "cluster_arn": "clusterArn",
-        "cluster_type": "clusterType",
-        "vpc": "vpc",
-        "certficate_secret": "certficateSecret",
-        "iam_handler_role": "iamHandlerRole",
-        "kafka_client_log_level": "kafkaClientLogLevel",
-        "mtls_handler_role": "mtlsHandlerRole",
-        "removal_policy": "removalPolicy",
-        "subnets": "subnets",
+        "saml_metadata_document": "samlMetadataDocument",
+        "server_certificate_arn": "serverCertificateArn",
+        "authorize_all_users_to_vpc_cidr": "authorizeAllUsersToVpcCidr",
+        "dns_servers": "dnsServers",
+        "logging": "logging",
+        "log_group": "logGroup",
+        "port": "port",
+        "security_groups": "securityGroups",
+        "self_service_portal": "selfServicePortal",
+        "session_timeout": "sessionTimeout",
+        "split_tunnel": "splitTunnel",
+        "transport_protocol": "transportProtocol",
     },
 )
-class KafkaApiProps:
+class DataVpcClientVpnEndpointProps:
     def __init__(
         self,
         *,
-        broker_security_group: _aws_cdk_aws_ec2_ceddda9d.ISecurityGroup,
-        client_authentication: ClientAuthentication,
-        cluster_arn: builtins.str,
-        cluster_type: "MskClusterType",
-        vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-        certficate_secret: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-        iam_handler_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        kafka_client_log_level: typing.Optional["KafkaClientLogLevel"] = None,
-        mtls_handler_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-        subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        saml_metadata_document: builtins.str,
+        server_certificate_arn: builtins.str,
+        authorize_all_users_to_vpc_cidr: typing.Optional[builtins.bool] = None,
+        dns_servers: typing.Optional[typing.Sequence[builtins.str]] = None,
+        logging: typing.Optional[builtins.bool] = None,
+        log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
+        port: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.VpnPort] = None,
+        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        self_service_portal: typing.Optional[builtins.bool] = None,
+        session_timeout: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ClientVpnSessionTimeout] = None,
+        split_tunnel: typing.Optional[builtins.bool] = None,
+        transport_protocol: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.TransportProtocol] = None,
     ) -> None:
-        '''Properties for the ``KafkaApi`` construct.
+        '''The properties for the ClientVPnEndpoint in DataVpc construct.
 
-        :param broker_security_group: The AWS security groups to associate with the elastic network interfaces in order to specify who can connect to and communicate with the Amazon MSK cluster.
-        :param client_authentication: Configuration properties for client authentication. MSK supports using private TLS certificates or SASL/SCRAM to authenticate the identity of clients.
-        :param cluster_arn: The ARN of the cluster.
-        :param cluster_type: The type of MSK cluster(provisioned or serverless).
-        :param vpc: Defines the virtual networking environment for this cluster. Must have at least 2 subnets in two different AZs.
-        :param certficate_secret: This is the TLS certificate of the Principal that is used by the CDK custom resource which set ACLs and Topics. It must be provided if the cluster is using mTLS authentication. The secret in AWS secrets manager must be a JSON in the following format { "key" : "PRIVATE-KEY", "cert" : "CERTIFICATE" } You can use the following utility to generate the certificates https://github.com/aws-samples/amazon-msk-client-authentication
-        :param iam_handler_role: The IAM role to pass to IAM authentication lambda handler This role must be able to be assumed with ``lambda.amazonaws.com`` service principal.
-        :param kafka_client_log_level: The log level for the lambda that support the Custom Resource for both Managing ACLs and Topics. Default: WARN
-        :param mtls_handler_role: The IAM role to pass to mTLS lambda handler This role must be able to be assumed with ``lambda.amazonaws.com`` service principal.
-        :param removal_policy: The removal policy when deleting the CDK resource. If DESTROY is selected, context value ``@data-solutions-framework-on-aws/removeDataOnDestroy`` needs to be set to true. Otherwise the removalPolicy is reverted to RETAIN. Default: - The resources are not deleted (``RemovalPolicy.RETAIN``).
-        :param subnets: The subnets where the Custom Resource Lambda Function would be created in. Default: - One private subnet with egress is used per AZ.
+        :param saml_metadata_document: An XML document generated by an identity provider (IdP) that supports SAML 2.0. The document includes the issuer's name, expiration information, and keys that can be used to validate the SAML authentication response (assertions) that are received from the IdP. You must generate the metadata document using the identity management software that is used as your organization's IdP.
+        :param server_certificate_arn: The ARN of the server certificate.
+        :param authorize_all_users_to_vpc_cidr: Whether to authorize all users to the VPC CIDR. Default: true
+        :param dns_servers: Information about the DNS servers to be used for DNS resolution. Default: DNS server in VPC, e.g. 10.0.0.2
+        :param logging: A CloudWatch Logs log group for connection logging. Default: true
+        :param log_group: A CloudWatch Logs log group for connection logging. Default: new LogGroup is created
+        :param port: The port number to assign to the Client VPN endpoint for TCP and UDP traffic. Default: true
+        :param security_groups: The security groups to apply to the target network. Default: new Securoty Group is created, allowing the incoming connections on port 443
+        :param self_service_portal: Specify whether to enable the self-service portal for the Client VPN endpoint. Default: true
+        :param session_timeout: The maximum VPN session duration time. Default: 480 minutes
+        :param split_tunnel: Indicates whether split-tunnel is enabled on the AWS Client VPN endpoint. Default: true
+        :param transport_protocol: The transport protocol to be used by the VPN session. Default: TCP
         '''
-        if isinstance(subnets, dict):
-            subnets = _aws_cdk_aws_ec2_ceddda9d.SubnetSelection(**subnets)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8aa63759ad33545334567b3e848b5b426d5233e0f36e975fdd69080066c10ef2)
-            check_type(argname="argument broker_security_group", value=broker_security_group, expected_type=type_hints["broker_security_group"])
-            check_type(argname="argument client_authentication", value=client_authentication, expected_type=type_hints["client_authentication"])
-            check_type(argname="argument cluster_arn", value=cluster_arn, expected_type=type_hints["cluster_arn"])
-            check_type(argname="argument cluster_type", value=cluster_type, expected_type=type_hints["cluster_type"])
-            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
-            check_type(argname="argument certficate_secret", value=certficate_secret, expected_type=type_hints["certficate_secret"])
-            check_type(argname="argument iam_handler_role", value=iam_handler_role, expected_type=type_hints["iam_handler_role"])
-            check_type(argname="argument kafka_client_log_level", value=kafka_client_log_level, expected_type=type_hints["kafka_client_log_level"])
-            check_type(argname="argument mtls_handler_role", value=mtls_handler_role, expected_type=type_hints["mtls_handler_role"])
-            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
-            check_type(argname="argument subnets", value=subnets, expected_type=type_hints["subnets"])
+            type_hints = typing.get_type_hints(_typecheckingstub__9f9e02adbd79c0e13152c12f983d4f942b325d9b511985bec14c1b11b1ad7cb9)
+            check_type(argname="argument saml_metadata_document", value=saml_metadata_document, expected_type=type_hints["saml_metadata_document"])
+            check_type(argname="argument server_certificate_arn", value=server_certificate_arn, expected_type=type_hints["server_certificate_arn"])
+            check_type(argname="argument authorize_all_users_to_vpc_cidr", value=authorize_all_users_to_vpc_cidr, expected_type=type_hints["authorize_all_users_to_vpc_cidr"])
+            check_type(argname="argument dns_servers", value=dns_servers, expected_type=type_hints["dns_servers"])
+            check_type(argname="argument logging", value=logging, expected_type=type_hints["logging"])
+            check_type(argname="argument log_group", value=log_group, expected_type=type_hints["log_group"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+            check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
+            check_type(argname="argument self_service_portal", value=self_service_portal, expected_type=type_hints["self_service_portal"])
+            check_type(argname="argument session_timeout", value=session_timeout, expected_type=type_hints["session_timeout"])
+            check_type(argname="argument split_tunnel", value=split_tunnel, expected_type=type_hints["split_tunnel"])
+            check_type(argname="argument transport_protocol", value=transport_protocol, expected_type=type_hints["transport_protocol"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "broker_security_group": broker_security_group,
-            "client_authentication": client_authentication,
-            "cluster_arn": cluster_arn,
-            "cluster_type": cluster_type,
-            "vpc": vpc,
+            "saml_metadata_document": saml_metadata_document,
+            "server_certificate_arn": server_certificate_arn,
         }
-        if certficate_secret is not None:
-            self._values["certficate_secret"] = certficate_secret
-        if iam_handler_role is not None:
-            self._values["iam_handler_role"] = iam_handler_role
-        if kafka_client_log_level is not None:
-            self._values["kafka_client_log_level"] = kafka_client_log_level
-        if mtls_handler_role is not None:
-            self._values["mtls_handler_role"] = mtls_handler_role
-        if removal_policy is not None:
-            self._values["removal_policy"] = removal_policy
-        if subnets is not None:
-            self._values["subnets"] = subnets
+        if authorize_all_users_to_vpc_cidr is not None:
+            self._values["authorize_all_users_to_vpc_cidr"] = authorize_all_users_to_vpc_cidr
+        if dns_servers is not None:
+            self._values["dns_servers"] = dns_servers
+        if logging is not None:
+            self._values["logging"] = logging
+        if log_group is not None:
+            self._values["log_group"] = log_group
+        if port is not None:
+            self._values["port"] = port
+        if security_groups is not None:
+            self._values["security_groups"] = security_groups
+        if self_service_portal is not None:
+            self._values["self_service_portal"] = self_service_portal
+        if session_timeout is not None:
+            self._values["session_timeout"] = session_timeout
+        if split_tunnel is not None:
+            self._values["split_tunnel"] = split_tunnel
+        if transport_protocol is not None:
+            self._values["transport_protocol"] = transport_protocol
+
+    @builtins.property
+    def saml_metadata_document(self) -> builtins.str:
+        '''An XML document generated by an identity provider (IdP) that supports SAML 2.0. The document includes the issuer's name, expiration information, and keys that can be used to validate the SAML authentication response (assertions) that are received from the IdP. You must generate the metadata document using the identity management software that is used as your organization's IdP.'''
+        result = self._values.get("saml_metadata_document")
+        assert result is not None, "Required property 'saml_metadata_document' is missing"
+        return typing.cast(builtins.str, result)
 
     @builtins.property
-    def broker_security_group(self) -> _aws_cdk_aws_ec2_ceddda9d.ISecurityGroup:
-        '''The AWS security groups to associate with the elastic network interfaces in order to specify who can connect to and communicate with the Amazon MSK cluster.'''
-        result = self._values.get("broker_security_group")
-        assert result is not None, "Required property 'broker_security_group' is missing"
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup, result)
+    def server_certificate_arn(self) -> builtins.str:
+        '''The ARN of the server certificate.'''
+        result = self._values.get("server_certificate_arn")
+        assert result is not None, "Required property 'server_certificate_arn' is missing"
+        return typing.cast(builtins.str, result)
 
     @builtins.property
-    def client_authentication(self) -> ClientAuthentication:
-        '''Configuration properties for client authentication.
+    def authorize_all_users_to_vpc_cidr(self) -> typing.Optional[builtins.bool]:
+        '''Whether to authorize all users to the VPC CIDR.
 
-        MSK supports using private TLS certificates or SASL/SCRAM to authenticate the identity of clients.
+        :default: true
         '''
-        result = self._values.get("client_authentication")
-        assert result is not None, "Required property 'client_authentication' is missing"
-        return typing.cast(ClientAuthentication, result)
+        result = self._values.get("authorize_all_users_to_vpc_cidr")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def cluster_arn(self) -> builtins.str:
-        '''The ARN of the cluster.'''
-        result = self._values.get("cluster_arn")
-        assert result is not None, "Required property 'cluster_arn' is missing"
-        return typing.cast(builtins.str, result)
+    def dns_servers(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''Information about the DNS servers to be used for DNS resolution.
 
-    @builtins.property
-    def cluster_type(self) -> "MskClusterType":
-        '''The type of MSK cluster(provisioned or serverless).'''
-        result = self._values.get("cluster_type")
-        assert result is not None, "Required property 'cluster_type' is missing"
-        return typing.cast("MskClusterType", result)
+        :default: DNS server in VPC, e.g. 10.0.0.2
+        '''
+        result = self._values.get("dns_servers")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
-    def vpc(self) -> _aws_cdk_aws_ec2_ceddda9d.IVpc:
-        '''Defines the virtual networking environment for this cluster.
+    def logging(self) -> typing.Optional[builtins.bool]:
+        '''A CloudWatch Logs log group for connection logging.
 
-        Must have at least 2 subnets in two different AZs.
+        :default: true
         '''
-        result = self._values.get("vpc")
-        assert result is not None, "Required property 'vpc' is missing"
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.IVpc, result)
+        result = self._values.get("logging")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def certficate_secret(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret]:
-        '''This is the TLS certificate of the Principal that is used by the CDK custom resource which set ACLs and Topics.
+    def log_group(self) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
+        '''A CloudWatch Logs log group for connection logging.
 
-        It must be provided if the cluster is using mTLS authentication.
-        The secret in AWS secrets manager must be a JSON in the following format
-        {
-        "key" : "PRIVATE-KEY",
-        "cert" : "CERTIFICATE"
-        }
-
-        You can use the following utility to generate the certificates
-        https://github.com/aws-samples/amazon-msk-client-authentication
+        :default: new LogGroup is created
         '''
-        result = self._values.get("certficate_secret")
-        return typing.cast(typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret], result)
+        result = self._values.get("log_group")
+        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], result)
 
     @builtins.property
-    def iam_handler_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
-        '''The IAM role to pass to IAM authentication lambda handler This role must be able to be assumed with ``lambda.amazonaws.com`` service principal.'''
-        result = self._values.get("iam_handler_role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+    def port(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.VpnPort]:
+        '''The port number to assign to the Client VPN endpoint for TCP and UDP traffic.
+
+        :default: true
+        '''
+        result = self._values.get("port")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.VpnPort], result)
 
     @builtins.property
-    def kafka_client_log_level(self) -> typing.Optional["KafkaClientLogLevel"]:
-        '''The log level for the lambda that support the Custom Resource for both Managing ACLs and Topics.
+    def security_groups(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
+        '''The security groups to apply to the target network.
 
-        :default: WARN
+        :default: new Securoty Group is created, allowing the incoming connections on port 443
         '''
-        result = self._values.get("kafka_client_log_level")
-        return typing.cast(typing.Optional["KafkaClientLogLevel"], result)
+        result = self._values.get("security_groups")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
 
     @builtins.property
-    def mtls_handler_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
-        '''The IAM role to pass to mTLS lambda handler This role must be able to be assumed with ``lambda.amazonaws.com`` service principal.'''
-        result = self._values.get("mtls_handler_role")
-        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+    def self_service_portal(self) -> typing.Optional[builtins.bool]:
+        '''Specify whether to enable the self-service portal for the Client VPN endpoint.
+
+        :default: true
+        '''
+        result = self._values.get("self_service_portal")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
-        '''The removal policy when deleting the CDK resource.
+    def session_timeout(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ClientVpnSessionTimeout]:
+        '''The maximum VPN session duration time.
 
-        If DESTROY is selected, context value ``@data-solutions-framework-on-aws/removeDataOnDestroy`` needs to be set to true.
-        Otherwise the removalPolicy is reverted to RETAIN.
+        :default: 480 minutes
+        '''
+        result = self._values.get("session_timeout")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ClientVpnSessionTimeout], result)
 
-        :default: - The resources are not deleted (``RemovalPolicy.RETAIN``).
+    @builtins.property
+    def split_tunnel(self) -> typing.Optional[builtins.bool]:
+        '''Indicates whether split-tunnel is enabled on the AWS Client VPN endpoint.
+
+        :default: true
         '''
-        result = self._values.get("removal_policy")
-        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
+        result = self._values.get("split_tunnel")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def subnets(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection]:
-        '''The subnets where the Custom Resource Lambda Function would be created in.
+    def transport_protocol(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.TransportProtocol]:
+        '''The transport protocol to be used by the VPN session.
 
-        :default: - One private subnet with egress is used per AZ.
+        :default: TCP
         '''
-        result = self._values.get("subnets")
-        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection], result)
+        result = self._values.get("transport_protocol")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.TransportProtocol], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "KafkaApiProps(%s)" % ", ".join(
+        return "DataVpcClientVpnEndpointProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.enum(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.KafkaClientLogLevel"
+@jsii.data_type(
+    jsii_type="@cdklabs/aws-data-solutions-framework.utils.DataVpcProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "vpc_cidr": "vpcCidr",
+        "client_vpn_endpoint_props": "clientVpnEndpointProps",
+        "flow_log_key": "flowLogKey",
+        "flow_log_retention": "flowLogRetention",
+        "flow_log_role": "flowLogRole",
+        "nat_gateways": "natGateways",
+        "removal_policy": "removalPolicy",
+    },
 )
-class KafkaClientLogLevel(enum.Enum):
-    '''The CDK Custom resources uses KafkaJs.
-
-    This enum allow you to set the log level
-    '''
-
-    WARN = "WARN"
-    DEBUG = "DEBUG"
-    INFO = "INFO"
-    ERROR = "ERROR"
-
-
-class KafkaVersion(
-    metaclass=jsii.JSIIMeta,
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.KafkaVersion",
-):
-    '''Kafka cluster version.'''
-
-    @jsii.member(jsii_name="of")
-    @builtins.classmethod
-    def of(cls, version: builtins.str) -> "KafkaVersion":
-        '''Custom cluster version.
+class DataVpcProps:
+    def __init__(
+        self,
+        *,
+        vpc_cidr: builtins.str,
+        client_vpn_endpoint_props: typing.Optional[typing.Union[DataVpcClientVpnEndpointProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        flow_log_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        flow_log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
+        flow_log_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        nat_gateways: typing.Optional[jsii.Number] = None,
+        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+    ) -> None:
+        '''The properties for the ``DataVpc`` construct.
 
-        :param version: custom version number.
+        :param vpc_cidr: The CIDR to use to create the subnets in the VPC.
+        :param client_vpn_endpoint_props: ClientVpnEndpoint propertioes. Required if client vpn endpoint is needed Default: None
+        :param flow_log_key: The KMS key used to encrypt the VPC Flow Logs in the CloudWatch Log Group. The resource policy of the key must be configured according to the AWS documentation. Default: - A new KMS key is created
+        :param flow_log_retention: The retention period to apply to VPC Flow Logs. Default: - One week retention
+        :param flow_log_role: The IAM Role used to send the VPC Flow Logs in CloudWatch. The role must be configured as described in the AWS VPC Flow Log documentation. Default: - A new IAM role is created
+        :param nat_gateways: Number of NAT Gateways. Default: 3 or the AZs defined in the context
+        :param removal_policy: The removal policy when deleting the CDK resource. If DESTROY is selected, context value ``@data-solutions-framework-on-aws/removeDataOnDestroy`` needs to be set to true. Otherwise, the removalPolicy is reverted to RETAIN. Default: - The resources are not deleted (``RemovalPolicy.RETAIN``).
         '''
+        if isinstance(client_vpn_endpoint_props, dict):
+            client_vpn_endpoint_props = DataVpcClientVpnEndpointProps(**client_vpn_endpoint_props)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e0e8e81d0dac96cf7234f1a61b30d53c9a3d1a4d97fb2c0e99ddf481ddfdef08)
-            check_type(argname="argument version", value=version, expected_type=type_hints["version"])
-        return typing.cast("KafkaVersion", jsii.sinvoke(cls, "of", [version]))
+            type_hints = typing.get_type_hints(_typecheckingstub__39f5bd0a66c070362158feeb021d04ddf2268154575ded55b8382334b30740e6)
+            check_type(argname="argument vpc_cidr", value=vpc_cidr, expected_type=type_hints["vpc_cidr"])
+            check_type(argname="argument client_vpn_endpoint_props", value=client_vpn_endpoint_props, expected_type=type_hints["client_vpn_endpoint_props"])
+            check_type(argname="argument flow_log_key", value=flow_log_key, expected_type=type_hints["flow_log_key"])
+            check_type(argname="argument flow_log_retention", value=flow_log_retention, expected_type=type_hints["flow_log_retention"])
+            check_type(argname="argument flow_log_role", value=flow_log_role, expected_type=type_hints["flow_log_role"])
+            check_type(argname="argument nat_gateways", value=nat_gateways, expected_type=type_hints["nat_gateways"])
+            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "vpc_cidr": vpc_cidr,
+        }
+        if client_vpn_endpoint_props is not None:
+            self._values["client_vpn_endpoint_props"] = client_vpn_endpoint_props
+        if flow_log_key is not None:
+            self._values["flow_log_key"] = flow_log_key
+        if flow_log_retention is not None:
+            self._values["flow_log_retention"] = flow_log_retention
+        if flow_log_role is not None:
+            self._values["flow_log_role"] = flow_log_role
+        if nat_gateways is not None:
+            self._values["nat_gateways"] = nat_gateways
+        if removal_policy is not None:
+            self._values["removal_policy"] = removal_policy
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V1_1_1")
-    def V1_1_1(cls) -> "KafkaVersion":
-        '''(deprecated) **Deprecated by Amazon MSK. You can't create a Kafka cluster with a deprecated version.**.
+    @builtins.property
+    def vpc_cidr(self) -> builtins.str:
+        '''The CIDR to use to create the subnets in the VPC.'''
+        result = self._values.get("vpc_cidr")
+        assert result is not None, "Required property 'vpc_cidr' is missing"
+        return typing.cast(builtins.str, result)
 
-        Kafka version 1.1.1
+    @builtins.property
+    def client_vpn_endpoint_props(
+        self,
+    ) -> typing.Optional[DataVpcClientVpnEndpointProps]:
+        '''ClientVpnEndpoint propertioes.
 
-        :deprecated: use the latest runtime instead
+        Required if client vpn endpoint is needed
 
-        :stability: deprecated
+        :default: None
         '''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V1_1_1"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_2_1")
-    def V2_2_1(cls) -> "KafkaVersion":
-        '''Kafka version 2.2.1.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_2_1"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_3_1")
-    def V2_3_1(cls) -> "KafkaVersion":
-        '''Kafka version 2.3.1.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_3_1"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_4_1_1")
-    def V2_4_1_1(cls) -> "KafkaVersion":
-        '''Kafka version 2.4.1.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_4_1_1"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_5_1")
-    def V2_5_1(cls) -> "KafkaVersion":
-        '''Kafka version 2.5.1.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_5_1"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_6_0")
-    def V2_6_0(cls) -> "KafkaVersion":
-        '''Kafka version 2.6.0.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_6_0"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_6_1")
-    def V2_6_1(cls) -> "KafkaVersion":
-        '''Kafka version 2.6.1.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_6_1"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_6_2")
-    def V2_6_2(cls) -> "KafkaVersion":
-        '''Kafka version 2.6.2.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_6_2"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_6_3")
-    def V2_6_3(cls) -> "KafkaVersion":
-        '''Kafka version 2.6.3.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_6_3"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_7_0")
-    def V2_7_0(cls) -> "KafkaVersion":
-        '''Kafka version 2.7.0.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_7_0"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_7_1")
-    def V2_7_1(cls) -> "KafkaVersion":
-        '''Kafka version 2.7.1.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_7_1"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_7_2")
-    def V2_7_2(cls) -> "KafkaVersion":
-        '''Kafka version 2.7.2.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_7_2"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_8_0")
-    def V2_8_0(cls) -> "KafkaVersion":
-        '''Kafka version 2.8.0.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_8_0"))
+        result = self._values.get("client_vpn_endpoint_props")
+        return typing.cast(typing.Optional[DataVpcClientVpnEndpointProps], result)
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_8_1")
-    def V2_8_1(cls) -> "KafkaVersion":
-        '''Kafka version 2.8.1.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_8_1"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V2_8_2_TIERED")
-    def V2_8_2_TIERED(cls) -> "KafkaVersion":
-        '''AWS MSK Kafka version 2.8.2.tiered.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V2_8_2_TIERED"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V3_1_1")
-    def V3_1_1(cls) -> "KafkaVersion":
-        '''Kafka version 3.1.1.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V3_1_1"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V3_2_0")
-    def V3_2_0(cls) -> "KafkaVersion":
-        '''Kafka version 3.2.0.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V3_2_0"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V3_3_1")
-    def V3_3_1(cls) -> "KafkaVersion":
-        '''Kafka version 3.3.1.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V3_3_1"))
+    @builtins.property
+    def flow_log_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+        '''The KMS key used to encrypt the VPC Flow Logs in the CloudWatch Log Group.
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V3_3_2")
-    def V3_3_2(cls) -> "KafkaVersion":
-        '''Kafka version 3.3.2.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V3_3_2"))
+        The resource policy of the key must be configured according to the AWS documentation.
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V3_4_0")
-    def V3_4_0(cls) -> "KafkaVersion":
-        '''Kafka version 3.4.0.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V3_4_0"))
+        :default: - A new KMS key is created
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="V3_5_1")
-    def V3_5_1(cls) -> "KafkaVersion":
-        '''Kafka version 3.5.1.'''
-        return typing.cast("KafkaVersion", jsii.sget(cls, "V3_5_1"))
+        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/encrypt-log-data-kms.html
+        '''
+        result = self._values.get("flow_log_key")
+        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
 
     @builtins.property
-    @jsii.member(jsii_name="version")
-    def version(self) -> builtins.str:
-        '''cluster version number.'''
-        return typing.cast(builtins.str, jsii.get(self, "version"))
-
-
-@jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.MonitoringConfiguration",
-    jsii_struct_bases=[],
-    name_mapping={
-        "cluster_monitoring_level": "clusterMonitoringLevel",
-        "enable_prometheus_jmx_exporter": "enablePrometheusJmxExporter",
-        "enable_prometheus_node_exporter": "enablePrometheusNodeExporter",
-    },
-)
-class MonitoringConfiguration:
-    def __init__(
+    def flow_log_retention(
         self,
-        *,
-        cluster_monitoring_level: typing.Optional[ClusterMonitoringLevel] = None,
-        enable_prometheus_jmx_exporter: typing.Optional[builtins.bool] = None,
-        enable_prometheus_node_exporter: typing.Optional[builtins.bool] = None,
-    ) -> None:
-        '''Monitoring Configuration.
+    ) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays]:
+        '''The retention period to apply to VPC Flow Logs.
 
-        :param cluster_monitoring_level: Specifies the level of monitoring for the MSK cluster. Default: DEFAULT
-        :param enable_prometheus_jmx_exporter: Indicates whether you want to enable or disable the JMX Exporter. Default: false
-        :param enable_prometheus_node_exporter: Indicates whether you want to enable or disable the Prometheus Node Exporter. You can use the Prometheus Node Exporter to get CPU and disk metrics for the broker nodes. Default: false
+        :default: - One week retention
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e2cbd7fca2428428959aa1e6b26222a5eda1ac49ca65e935d98c608d20e95b2a)
-            check_type(argname="argument cluster_monitoring_level", value=cluster_monitoring_level, expected_type=type_hints["cluster_monitoring_level"])
-            check_type(argname="argument enable_prometheus_jmx_exporter", value=enable_prometheus_jmx_exporter, expected_type=type_hints["enable_prometheus_jmx_exporter"])
-            check_type(argname="argument enable_prometheus_node_exporter", value=enable_prometheus_node_exporter, expected_type=type_hints["enable_prometheus_node_exporter"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if cluster_monitoring_level is not None:
-            self._values["cluster_monitoring_level"] = cluster_monitoring_level
-        if enable_prometheus_jmx_exporter is not None:
-            self._values["enable_prometheus_jmx_exporter"] = enable_prometheus_jmx_exporter
-        if enable_prometheus_node_exporter is not None:
-            self._values["enable_prometheus_node_exporter"] = enable_prometheus_node_exporter
+        result = self._values.get("flow_log_retention")
+        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays], result)
 
     @builtins.property
-    def cluster_monitoring_level(self) -> typing.Optional[ClusterMonitoringLevel]:
-        '''Specifies the level of monitoring for the MSK cluster.
+    def flow_log_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+        '''The IAM Role used to send the VPC Flow Logs in CloudWatch.
+
+        The role must be configured as described in the AWS VPC Flow Log documentation.
 
-        :default: DEFAULT
+        :default: - A new IAM role is created
+
+        :see: https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs-cwl.html#flow-logs-iam-role
         '''
-        result = self._values.get("cluster_monitoring_level")
-        return typing.cast(typing.Optional[ClusterMonitoringLevel], result)
+        result = self._values.get("flow_log_role")
+        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
 
     @builtins.property
-    def enable_prometheus_jmx_exporter(self) -> typing.Optional[builtins.bool]:
-        '''Indicates whether you want to enable or disable the JMX Exporter.
+    def nat_gateways(self) -> typing.Optional[jsii.Number]:
+        '''Number of NAT Gateways.
 
-        :default: false
+        :default: 3 or the AZs defined in the context
         '''
-        result = self._values.get("enable_prometheus_jmx_exporter")
-        return typing.cast(typing.Optional[builtins.bool], result)
+        result = self._values.get("nat_gateways")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    def enable_prometheus_node_exporter(self) -> typing.Optional[builtins.bool]:
-        '''Indicates whether you want to enable or disable the Prometheus Node Exporter.
+    def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
+        '''The removal policy when deleting the CDK resource.
 
-        You can use the Prometheus Node Exporter to get CPU and disk metrics for the broker nodes.
+        If DESTROY is selected, context value ``@data-solutions-framework-on-aws/removeDataOnDestroy`` needs to be set to true.
+        Otherwise, the removalPolicy is reverted to RETAIN.
 
-        :default: false
+        :default: - The resources are not deleted (``RemovalPolicy.RETAIN``).
         '''
-        result = self._values.get("enable_prometheus_node_exporter")
-        return typing.cast(typing.Optional[builtins.bool], result)
+        result = self._values.get("removal_policy")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "MonitoringConfiguration(%s)" % ", ".join(
+        return "DataVpcProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class MskBrokerInstanceType(
+class S3DataCopy(
+    _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.MskBrokerInstanceType",
+    jsii_type="@cdklabs/aws-data-solutions-framework.utils.S3DataCopy",
 ):
-    '''Kafka cluster version.'''
+    '''Copy data from one S3 bucket to another.
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M5_12XLARGE")
-    def KAFKA_M5_12_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m5.12xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M5_12XLARGE"))
+    :see: https://awslabs.github.io/data-solutions-framework-on-aws/docs/constructs/library/Utils/s3-data-copy
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M5_16XLARGE")
-    def KAFKA_M5_16_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m5.16xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M5_16XLARGE"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M5_24XLARGE")
-    def KAFKA_M5_24_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m5.24xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M5_24XLARGE"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M5_2XLARGE")
-    def KAFKA_M5_2_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m5.2xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M5_2XLARGE"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M5_4XLARGE")
-    def KAFKA_M5_4_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m5.4xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M5_4XLARGE"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M5_8XLARGE")
-    def KAFKA_M5_8_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m5.8xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M5_8XLARGE"))
+    Example::
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M5_LARGE")
-    def KAFKA_M5_LARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m5.large.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M5_LARGE"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M5_XLARGE")
-    def KAFKA_M5_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m5.xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M5_XLARGE"))
-
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M7G_12XLARGE")
-    def KAFKA_M7_G_12_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m7g.12xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M7G_12XLARGE"))
+        from aws_cdk.aws_s3 import Bucket
+        
+        
+        source_bucket = Bucket.from_bucket_name(self, "SourceBucket", "nyc-tlc")
+        bucket_name = f"test-{this.region}-{this.account}-{dsf.utils.Utils.generateUniqueHash(this, 'TargetBucket')}"
+        
+        target_bucket = Bucket(self, "TargetBucket")
+        
+        dsf.utils.S3DataCopy(self, "S3DataCopy",
+            source_bucket=source_bucket,
+            source_bucket_prefix="trip data/",
+            source_bucket_region="us-east-1",
+            target_bucket=target_bucket
+        )
+    '''
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M7G_16XLARGE")
-    def KAFKA_M7_G_16_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m7g.16xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M7G_16XLARGE"))
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        source_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        source_bucket_region: builtins.str,
+        target_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        execution_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        source_bucket_prefix: typing.Optional[builtins.str] = None,
+        subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        target_bucket_prefix: typing.Optional[builtins.str] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+    ) -> None:
+        '''
+        :param scope: -
+        :param id: -
+        :param source_bucket: The source S3 Bucket containing the data to copy.
+        :param source_bucket_region: The source S3 Bucket region.
+        :param target_bucket: The target S3 Bucket.
+        :param execution_role: The IAM Role to use in the custom resource for copying data. Default: - A new role is created
+        :param removal_policy: The removal policy when deleting the CDK resource. If DESTROY is selected, context value ``@data-solutions-framework-on-aws/removeDataOnDestroy`` needs to be set to true. Otherwise, the removalPolicy is reverted to RETAIN. Default: - The resources are not deleted (``RemovalPolicy.RETAIN``).
+        :param security_groups: The list of security groups to attach to the custom resource. Default: - If ``vpc`` is not supplied, no security groups are attached. Otherwise, a dedicated security group is created for each function.
+        :param source_bucket_prefix: The source bucket prefix with a slash at the end. Default: - No prefix is used
+        :param subnets: The subnets to deploy the custom resource in. Default: - The Custom Resource is executed in VPCs owned by AWS Lambda service.
+        :param target_bucket_prefix: The target S3 Bucket prefix with a slash at the end. Default: - No prefix is used
+        :param vpc: The VPC to deploy the custom resource in. Default: - The Custom Resource is executed in VPCs owned by AWS Lambda service.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__517cea3b12f758ad38d48578dca87a1f97c700253daf18d0fa4f1079fa3b310b)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = S3DataCopyProps(
+            source_bucket=source_bucket,
+            source_bucket_region=source_bucket_region,
+            target_bucket=target_bucket,
+            execution_role=execution_role,
+            removal_policy=removal_policy,
+            security_groups=security_groups,
+            source_bucket_prefix=source_bucket_prefix,
+            subnets=subnets,
+            target_bucket_prefix=target_bucket_prefix,
+            vpc=vpc,
+        )
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M7G_24XLARGE")
-    def KAFKA_M7_G_24_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m7g.24xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M7G_24XLARGE"))
+        jsii.create(self.__class__, self, [scope, id, props])
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M7G_2XLARGE")
-    def KAFKA_M7_G_2_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m7g.2xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M7G_2XLARGE"))
+    @jsii.member(jsii_name="retrieveVersion")
+    def retrieve_version(self) -> typing.Any:
+        '''Retrieve DSF package.json version.'''
+        return typing.cast(typing.Any, jsii.invoke(self, "retrieveVersion", []))
 
     @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M7G_4XLARGE")
-    def KAFKA_M7_G_4_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m7g.4xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M7G_4XLARGE"))
+    @jsii.member(jsii_name="DSF_OWNED_TAG")
+    def DSF_OWNED_TAG(cls) -> builtins.str:
+        return typing.cast(builtins.str, jsii.sget(cls, "DSF_OWNED_TAG"))
 
     @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M7G_8XLARGE")
-    def KAFKA_M7_G_8_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m7g.8xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M7G_8XLARGE"))
+    @jsii.member(jsii_name="DSF_TRACKING_CODE")
+    def DSF_TRACKING_CODE(cls) -> builtins.str:
+        return typing.cast(builtins.str, jsii.sget(cls, "DSF_TRACKING_CODE"))
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M7G_LARGE")
-    def KAFKA_M7_G_LARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m7g.large.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M7G_LARGE"))
+    @builtins.property
+    @jsii.member(jsii_name="copyFunction")
+    def copy_function(self) -> _aws_cdk_aws_lambda_ceddda9d.IFunction:
+        '''The Lambda Function for the copy.'''
+        return typing.cast(_aws_cdk_aws_lambda_ceddda9d.IFunction, jsii.get(self, "copyFunction"))
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_M7G_XLARGE")
-    def KAFKA_M7_G_XLARGE(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.m7g.xlarge.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_M7G_XLARGE"))
+    @builtins.property
+    @jsii.member(jsii_name="copyLogGroup")
+    def copy_log_group(self) -> _aws_cdk_aws_logs_ceddda9d.ILogGroup:
+        '''The CloudWatch Log Group for the S3 data copy.'''
+        return typing.cast(_aws_cdk_aws_logs_ceddda9d.ILogGroup, jsii.get(self, "copyLogGroup"))
 
-    @jsii.python.classproperty
-    @jsii.member(jsii_name="KAFKA_T3_SMALL")
-    def KAFKA_T3_SMALL(cls) -> "MskBrokerInstanceType":
-        '''Borker instance type kafka.t3.small.'''
-        return typing.cast("MskBrokerInstanceType", jsii.sget(cls, "KAFKA_T3_SMALL"))
+    @builtins.property
+    @jsii.member(jsii_name="copyRole")
+    def copy_role(self) -> _aws_cdk_aws_iam_ceddda9d.IRole:
+        '''The IAM Role for the copy Lambba Function.'''
+        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IRole, jsii.get(self, "copyRole"))
 
     @builtins.property
-    @jsii.member(jsii_name="instance")
-    def instance(self) -> _aws_cdk_aws_ec2_ceddda9d.InstanceType:
-        return typing.cast(_aws_cdk_aws_ec2_ceddda9d.InstanceType, jsii.get(self, "instance"))
+    @jsii.member(jsii_name="cleanUpFunction")
+    def clean_up_function(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IFunction]:
+        '''The Lambda function for the S3 data copy cleaning up lambda.'''
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IFunction], jsii.get(self, "cleanUpFunction"))
 
+    @builtins.property
+    @jsii.member(jsii_name="cleanUpLogGroup")
+    def clean_up_log_group(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup]:
+        '''The CloudWatch Log Group for the S3 data copy cleaning up lambda.'''
+        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup], jsii.get(self, "cleanUpLogGroup"))
 
-@jsii.enum(jsii_type="@cdklabs/aws-data-solutions-framework.streaming.MskClusterType")
-class MskClusterType(enum.Enum):
-    '''Enum for MSK cluster types.'''
+    @builtins.property
+    @jsii.member(jsii_name="cleanUpRole")
+    def clean_up_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+        '''The IAM Role for the the S3 data copy cleaning up lambda.'''
+        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], jsii.get(self, "cleanUpRole"))
 
-    PROVISIONED = "PROVISIONED"
-    SERVERLESS = "SERVERLESS"
+    @builtins.property
+    @jsii.member(jsii_name="securityGroups")
+    def security_groups(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
+        '''The list of EC2 Security Groups used by the Lambda Functions.'''
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], jsii.get(self, "securityGroups"))
 
 
 @jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.MskTopic",
+    jsii_type="@cdklabs/aws-data-solutions-framework.utils.S3DataCopyProps",
     jsii_struct_bases=[],
     name_mapping={
-        "num_partitions": "numPartitions",
-        "topic": "topic",
-        "replication_factor": "replicationFactor",
+        "source_bucket": "sourceBucket",
+        "source_bucket_region": "sourceBucketRegion",
+        "target_bucket": "targetBucket",
+        "execution_role": "executionRole",
+        "removal_policy": "removalPolicy",
+        "security_groups": "securityGroups",
+        "source_bucket_prefix": "sourceBucketPrefix",
+        "subnets": "subnets",
+        "target_bucket_prefix": "targetBucketPrefix",
+        "vpc": "vpc",
     },
 )
-class MskTopic:
+class S3DataCopyProps:
     def __init__(
         self,
         *,
-        num_partitions: jsii.Number,
-        topic: builtins.str,
-        replication_factor: typing.Optional[jsii.Number] = None,
+        source_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        source_bucket_region: builtins.str,
+        target_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+        execution_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        source_bucket_prefix: typing.Optional[builtins.str] = None,
+        subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        target_bucket_prefix: typing.Optional[builtins.str] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
-        '''Properties for the ``MskTopic`` As defined in ``ITopicConfig`` in `KafkaJS <https://kafka.js.org/docs/admin>`_ SDK.
+        '''Properties for S3DataCopy construct.
 
-        :param num_partitions: The number of partitions in the topic.
-        :param topic: The name of the topic.
-        :param replication_factor: The replication factor of the partitions. This parameter cannot be updated after the creation of the topic. This parameter should not be provided for MSK Serverless. Default: - For MSK Serverless, the number of AZ. For MSK Provisioned, the cluster default configuration.
+        :param source_bucket: The source S3 Bucket containing the data to copy.
+        :param source_bucket_region: The source S3 Bucket region.
+        :param target_bucket: The target S3 Bucket.
+        :param execution_role: The IAM Role to use in the custom resource for copying data. Default: - A new role is created
+        :param removal_policy: The removal policy when deleting the CDK resource. If DESTROY is selected, context value ``@data-solutions-framework-on-aws/removeDataOnDestroy`` needs to be set to true. Otherwise, the removalPolicy is reverted to RETAIN. Default: - The resources are not deleted (``RemovalPolicy.RETAIN``).
+        :param security_groups: The list of security groups to attach to the custom resource. Default: - If ``vpc`` is not supplied, no security groups are attached. Otherwise, a dedicated security group is created for each function.
+        :param source_bucket_prefix: The source bucket prefix with a slash at the end. Default: - No prefix is used
+        :param subnets: The subnets to deploy the custom resource in. Default: - The Custom Resource is executed in VPCs owned by AWS Lambda service.
+        :param target_bucket_prefix: The target S3 Bucket prefix with a slash at the end. Default: - No prefix is used
+        :param vpc: The VPC to deploy the custom resource in. Default: - The Custom Resource is executed in VPCs owned by AWS Lambda service.
         '''
+        if isinstance(subnets, dict):
+            subnets = _aws_cdk_aws_ec2_ceddda9d.SubnetSelection(**subnets)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__50999f64b2bf57e9a21df87c98a154cffadc71c2285baeebf0f8689e1e777429)
-            check_type(argname="argument num_partitions", value=num_partitions, expected_type=type_hints["num_partitions"])
-            check_type(argname="argument topic", value=topic, expected_type=type_hints["topic"])
-            check_type(argname="argument replication_factor", value=replication_factor, expected_type=type_hints["replication_factor"])
+            type_hints = typing.get_type_hints(_typecheckingstub__b0f1736d011e3dabe341959f89b9b95889c7c24aa7cdfa70fa1893401fa55286)
+            check_type(argname="argument source_bucket", value=source_bucket, expected_type=type_hints["source_bucket"])
+            check_type(argname="argument source_bucket_region", value=source_bucket_region, expected_type=type_hints["source_bucket_region"])
+            check_type(argname="argument target_bucket", value=target_bucket, expected_type=type_hints["target_bucket"])
+            check_type(argname="argument execution_role", value=execution_role, expected_type=type_hints["execution_role"])
+            check_type(argname="argument removal_policy", value=removal_policy, expected_type=type_hints["removal_policy"])
+            check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
+            check_type(argname="argument source_bucket_prefix", value=source_bucket_prefix, expected_type=type_hints["source_bucket_prefix"])
+            check_type(argname="argument subnets", value=subnets, expected_type=type_hints["subnets"])
+            check_type(argname="argument target_bucket_prefix", value=target_bucket_prefix, expected_type=type_hints["target_bucket_prefix"])
+            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "num_partitions": num_partitions,
-            "topic": topic,
+            "source_bucket": source_bucket,
+            "source_bucket_region": source_bucket_region,
+            "target_bucket": target_bucket,
         }
-        if replication_factor is not None:
-            self._values["replication_factor"] = replication_factor
+        if execution_role is not None:
+            self._values["execution_role"] = execution_role
+        if removal_policy is not None:
+            self._values["removal_policy"] = removal_policy
+        if security_groups is not None:
+            self._values["security_groups"] = security_groups
+        if source_bucket_prefix is not None:
+            self._values["source_bucket_prefix"] = source_bucket_prefix
+        if subnets is not None:
+            self._values["subnets"] = subnets
+        if target_bucket_prefix is not None:
+            self._values["target_bucket_prefix"] = target_bucket_prefix
+        if vpc is not None:
+            self._values["vpc"] = vpc
 
     @builtins.property
-    def num_partitions(self) -> jsii.Number:
-        '''The number of partitions in the topic.'''
-        result = self._values.get("num_partitions")
-        assert result is not None, "Required property 'num_partitions' is missing"
-        return typing.cast(jsii.Number, result)
+    def source_bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
+        '''The source S3 Bucket containing the data to copy.'''
+        result = self._values.get("source_bucket")
+        assert result is not None, "Required property 'source_bucket' is missing"
+        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
 
     @builtins.property
-    def topic(self) -> builtins.str:
-        '''The name of the topic.'''
-        result = self._values.get("topic")
-        assert result is not None, "Required property 'topic' is missing"
+    def source_bucket_region(self) -> builtins.str:
+        '''The source S3 Bucket region.'''
+        result = self._values.get("source_bucket_region")
+        assert result is not None, "Required property 'source_bucket_region' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def replication_factor(self) -> typing.Optional[jsii.Number]:
-        '''The replication factor of the partitions.
+    def target_bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
+        '''The target S3 Bucket.'''
+        result = self._values.get("target_bucket")
+        assert result is not None, "Required property 'target_bucket' is missing"
+        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
 
-        This parameter cannot be updated after the creation of the topic.
-        This parameter should not be provided for MSK Serverless.
+    @builtins.property
+    def execution_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+        '''The IAM Role to use in the custom resource for copying data.
 
-        :default: - For MSK Serverless, the number of AZ. For MSK Provisioned, the cluster default configuration.
+        :default: - A new role is created
         '''
-        result = self._values.get("replication_factor")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "MskTopic(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
-@jsii.enum(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.ResourcePatternTypes"
-)
-class ResourcePatternTypes(enum.Enum):
-    UNKNOWN = "UNKNOWN"
-    ANY = "ANY"
-    MATCH = "MATCH"
-    LITERAL = "LITERAL"
-    PREFIXED = "PREFIXED"
+        result = self._values.get("execution_role")
+        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
 
+    @builtins.property
+    def removal_policy(self) -> typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy]:
+        '''The removal policy when deleting the CDK resource.
 
-@jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.S3LoggingConfiguration",
-    jsii_struct_bases=[],
-    name_mapping={"bucket": "bucket", "prefix": "prefix"},
-)
-class S3LoggingConfiguration:
-    def __init__(
-        self,
-        *,
-        bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-        prefix: typing.Optional[builtins.str] = None,
-    ) -> None:
-        '''Details of the Amazon S3 destination for broker logs.
+        If DESTROY is selected, context value ``@data-solutions-framework-on-aws/removeDataOnDestroy`` needs to be set to true.
+        Otherwise, the removalPolicy is reverted to RETAIN.
 
-        :param bucket: The S3 bucket that is the destination for broker logs.
-        :param prefix: The S3 prefix that is the destination for broker logs. Default: - no prefix
+        :default: - The resources are not deleted (``RemovalPolicy.RETAIN``).
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__82ca97be2f9081adbed88410b7981d2cc7bbd6145b59a319f25c899a33c1587f)
-            check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
-            check_type(argname="argument prefix", value=prefix, expected_type=type_hints["prefix"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "bucket": bucket,
-        }
-        if prefix is not None:
-            self._values["prefix"] = prefix
+        result = self._values.get("removal_policy")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy], result)
 
     @builtins.property
-    def bucket(self) -> _aws_cdk_aws_s3_ceddda9d.IBucket:
-        '''The S3 bucket that is the destination for broker logs.'''
-        result = self._values.get("bucket")
-        assert result is not None, "Required property 'bucket' is missing"
-        return typing.cast(_aws_cdk_aws_s3_ceddda9d.IBucket, result)
+    def security_groups(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
+        '''The list of security groups to attach to the custom resource.
 
-    @builtins.property
-    def prefix(self) -> typing.Optional[builtins.str]:
-        '''The S3 prefix that is the destination for broker logs.
+        :default:
 
-        :default: - no prefix
+        - If ``vpc`` is not supplied, no security groups are attached. Otherwise, a dedicated security
+        group is created for each function.
         '''
-        result = self._values.get("prefix")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
+        result = self._values.get("security_groups")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
 
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "S3LoggingConfiguration(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
-@jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.SaslAuthProps",
-    jsii_struct_bases=[],
-    name_mapping={"iam": "iam"},
-)
-class SaslAuthProps:
-    def __init__(self, *, iam: typing.Optional[builtins.bool] = None) -> None:
-        '''SASL authentication properties.
+    @builtins.property
+    def source_bucket_prefix(self) -> typing.Optional[builtins.str]:
+        '''The source bucket prefix with a slash at the end.
 
-        :param iam: Enable IAM access control. Default: true
+        :default: - No prefix is used
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a69cfaf96dab720314a86b2aba1a3764d5dad9597e92d15b07c21a58a886d884)
-            check_type(argname="argument iam", value=iam, expected_type=type_hints["iam"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if iam is not None:
-            self._values["iam"] = iam
+        result = self._values.get("source_bucket_prefix")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def iam(self) -> typing.Optional[builtins.bool]:
-        '''Enable IAM access control.
+    def subnets(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection]:
+        '''The subnets to deploy the custom resource in.
 
-        :default: true
+        :default: - The Custom Resource is executed in VPCs owned by AWS Lambda service.
         '''
-        result = self._values.get("iam")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "SaslAuthProps(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
-@jsii.enum(jsii_type="@cdklabs/aws-data-solutions-framework.streaming.StorageMode")
-class StorageMode(enum.Enum):
-    '''The storage mode for the cluster brokers.'''
-
-    LOCAL = "LOCAL"
-    '''Local storage mode utilizes network attached EBS storage.'''
-    TIERED = "TIERED"
-    '''Tiered storage mode utilizes EBS storage and Tiered storage.'''
-
+        result = self._values.get("subnets")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection], result)
 
-@jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.TlsAuthProps",
-    jsii_struct_bases=[],
-    name_mapping={"certificate_authorities": "certificateAuthorities"},
-)
-class TlsAuthProps:
-    def __init__(
-        self,
-        *,
-        certificate_authorities: typing.Optional[typing.Sequence[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]] = None,
-    ) -> None:
-        '''TLS authentication properties.
+    @builtins.property
+    def target_bucket_prefix(self) -> typing.Optional[builtins.str]:
+        '''The target S3 Bucket prefix with a slash at the end.
 
-        :param certificate_authorities: List of ACM Certificate Authorities to enable TLS authentication. Default: - none
+        :default: - No prefix is used
         '''
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b75ace651f25eb081badf2271fb655bc4c0850e36bafe6b474f39e00935bb0c7)
-            check_type(argname="argument certificate_authorities", value=certificate_authorities, expected_type=type_hints["certificate_authorities"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if certificate_authorities is not None:
-            self._values["certificate_authorities"] = certificate_authorities
+        result = self._values.get("target_bucket_prefix")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def certificate_authorities(
-        self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]]:
-        '''List of ACM Certificate Authorities to enable TLS authentication.
+    def vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
+        '''The VPC to deploy the custom resource in.
 
-        :default: - none
+        :default: - The Custom Resource is executed in VPCs owned by AWS Lambda service.
         '''
-        result = self._values.get("certificate_authorities")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]], result)
+        result = self._values.get("vpc")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "TlsAuthProps(%s)" % ", ".join(
+        return "S3DataCopyProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class VpcClientAuthentication(
+class StepFunctionUtils(
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.VpcClientAuthentication",
+    jsii_type="@cdklabs/aws-data-solutions-framework.utils.StepFunctionUtils",
 ):
-    '''Configuration properties for VPC client authentication.'''
-
-    @jsii.member(jsii_name="sasl")
-    @builtins.classmethod
-    def sasl(
-        cls,
-        *,
-        iam: typing.Optional[builtins.bool] = None,
-    ) -> "VpcClientAuthentication":
-        '''SASL authentication.
+    '''Utils for working with AWS Step Functions.'''
 
-        :param iam: Enable IAM access control. Default: true
-        '''
-        props = SaslAuthProps(iam=iam)
+    def __init__(self) -> None:
+        jsii.create(self.__class__, self, [])
 
-        return typing.cast("VpcClientAuthentication", jsii.sinvoke(cls, "sasl", [props]))
-
-    @jsii.member(jsii_name="saslTls")
+    @jsii.member(jsii_name="camelToPascal")
     @builtins.classmethod
-    def sasl_tls(
+    def camel_to_pascal(
         cls,
-        *,
-        iam: typing.Optional[builtins.bool] = None,
-        tls: typing.Optional[builtins.bool] = None,
-    ) -> "VpcClientAuthentication":
-        '''SASL + TLS authentication.
-
-        :param iam: Enable IAM access control. Default: true
-        :param tls: enable TLS authentication. Default: - none
-        '''
-        sasl_tls_props = SaslVpcTlsAuthProps(iam=iam, tls=tls)
-
-        return typing.cast("VpcClientAuthentication", jsii.sinvoke(cls, "saslTls", [sasl_tls_props]))
+        config: typing.Mapping[builtins.str, typing.Any],
+    ) -> typing.Mapping[builtins.str, typing.Any]:
+        '''Convert camel case properties to pascal case as required by AWS Step Functions API.
 
-    @jsii.member(jsii_name="tls")
-    @builtins.classmethod
-    def tls(
-        cls,
-        *,
-        tls: typing.Optional[builtins.bool] = None,
-    ) -> "VpcClientAuthentication":
-        '''TLS authentication.
+        :param config: -
 
-        :param tls: enable TLS authentication. Default: - none
+        :return: config converted to pascal case.
         '''
-        props = VpcTlsAuthProps(tls=tls)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8900956bb9a5e837ad18d5f562d4d1129e080f940075a87fdda2f93cb4467b66)
+            check_type(argname="argument config", value=config, expected_type=type_hints["config"])
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.sinvoke(cls, "camelToPascal", [config]))
 
-        return typing.cast("VpcClientAuthentication", jsii.sinvoke(cls, "tls", [props]))
 
-    @builtins.property
-    @jsii.member(jsii_name="saslProps")
-    def sasl_props(self) -> typing.Optional[SaslAuthProps]:
-        '''- properties for SASL authentication.'''
-        return typing.cast(typing.Optional[SaslAuthProps], jsii.get(self, "saslProps"))
+class Utils(
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdklabs/aws-data-solutions-framework.utils.Utils",
+):
+    '''Utilities class used across the different resources.'''
 
-    @builtins.property
-    @jsii.member(jsii_name="tlsProps")
-    def tls_props(self) -> typing.Optional["VpcTlsAuthProps"]:
-        '''- properties for TLS authentication.'''
-        return typing.cast(typing.Optional["VpcTlsAuthProps"], jsii.get(self, "tlsProps"))
+    def __init__(self) -> None:
+        jsii.create(self.__class__, self, [])
 
+    @jsii.member(jsii_name="generateHash")
+    @builtins.classmethod
+    def generate_hash(cls, text: builtins.str) -> builtins.str:
+        '''Generate an 8 character hash from a string based on HMAC algorithm.
 
-@jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.VpcTlsAuthProps",
-    jsii_struct_bases=[],
-    name_mapping={"tls": "tls"},
-)
-class VpcTlsAuthProps:
-    def __init__(self, *, tls: typing.Optional[builtins.bool] = None) -> None:
-        '''TLS authentication properties.
+        :param text: the text to hash.
 
-        :param tls: enable TLS authentication. Default: - none
+        :return: the hash
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bfa989fad1cbc8518acad9bce75e30465e418b0228fe1dd3da8649e86a493beb)
-            check_type(argname="argument tls", value=tls, expected_type=type_hints["tls"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if tls is not None:
-            self._values["tls"] = tls
-
-    @builtins.property
-    def tls(self) -> typing.Optional[builtins.bool]:
-        '''enable TLS authentication.
-
-        :default: - none
-        '''
-        result = self._values.get("tls")
-        return typing.cast(typing.Optional[builtins.bool], result)
+            type_hints = typing.get_type_hints(_typecheckingstub__a4e130c83849df0af7b3beb5e50b0f00a681650d748a723d6c81079ec6f34336)
+            check_type(argname="argument text", value=text, expected_type=type_hints["text"])
+        return typing.cast(builtins.str, jsii.sinvoke(cls, "generateHash", [text]))
 
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "VpcTlsAuthProps(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
+    @jsii.member(jsii_name="generateUniqueHash")
+    @builtins.classmethod
+    def generate_unique_hash(
+        cls,
+        scope: _constructs_77d1e7e8.Construct,
+        id: typing.Optional[builtins.str] = None,
+    ) -> builtins.str:
+        '''Generate a unique hash of 8 characters from the CDK scope using its path and the stack name.
 
+        :param scope: the CDK construct scope.
+        :param id: the CDK ID of the construct.
 
-@jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.SaslTlsAuthProps",
-    jsii_struct_bases=[SaslAuthProps, TlsAuthProps],
-    name_mapping={"iam": "iam", "certificate_authorities": "certificateAuthorities"},
-)
-class SaslTlsAuthProps(SaslAuthProps, TlsAuthProps):
-    def __init__(
-        self,
-        *,
-        iam: typing.Optional[builtins.bool] = None,
-        certificate_authorities: typing.Optional[typing.Sequence[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]] = None,
-    ) -> None:
-        '''SASL + TLS authentication properties.
-
-        :param iam: Enable IAM access control. Default: true
-        :param certificate_authorities: List of ACM Certificate Authorities to enable TLS authentication. Default: - none
+        :return: the hash
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b540b95307fdb73492eba61e5c3ad3f2ea64ba068d1b2d8d32d407a1f8dd7d37)
-            check_type(argname="argument iam", value=iam, expected_type=type_hints["iam"])
-            check_type(argname="argument certificate_authorities", value=certificate_authorities, expected_type=type_hints["certificate_authorities"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if iam is not None:
-            self._values["iam"] = iam
-        if certificate_authorities is not None:
-            self._values["certificate_authorities"] = certificate_authorities
-
-    @builtins.property
-    def iam(self) -> typing.Optional[builtins.bool]:
-        '''Enable IAM access control.
-
-        :default: true
-        '''
-        result = self._values.get("iam")
-        return typing.cast(typing.Optional[builtins.bool], result)
+            type_hints = typing.get_type_hints(_typecheckingstub__f70aa0e068d4cfe35caac3551a2937a15c623193142ac0abb9ea73184612ded3)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        return typing.cast(builtins.str, jsii.sinvoke(cls, "generateUniqueHash", [scope, id]))
 
-    @builtins.property
-    def certificate_authorities(
-        self,
-    ) -> typing.Optional[typing.List[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]]:
-        '''List of ACM Certificate Authorities to enable TLS authentication.
+    @jsii.member(jsii_name="loadYaml")
+    @builtins.classmethod
+    def load_yaml(cls, document: builtins.str) -> typing.Any:
+        '''Take a document stored as string and load it as YAML.
 
-        :default: - none
+        :param document: the document stored as string.
         '''
-        result = self._values.get("certificate_authorities")
-        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "SaslTlsAuthProps(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__f08bfe619a6fde71b5609a00f036443fb3dcf2ab30d09c795dbe0f7f0475a43d)
+            check_type(argname="argument document", value=document, expected_type=type_hints["document"])
+        return typing.cast(typing.Any, jsii.sinvoke(cls, "loadYaml", [document]))
 
-@jsii.data_type(
-    jsii_type="@cdklabs/aws-data-solutions-framework.streaming.SaslVpcTlsAuthProps",
-    jsii_struct_bases=[SaslAuthProps, VpcTlsAuthProps],
-    name_mapping={"iam": "iam", "tls": "tls"},
-)
-class SaslVpcTlsAuthProps(SaslAuthProps, VpcTlsAuthProps):
-    def __init__(
-        self,
-        *,
-        iam: typing.Optional[builtins.bool] = None,
-        tls: typing.Optional[builtins.bool] = None,
-    ) -> None:
-        '''SASL + TLS authentication properties.
+    @jsii.member(jsii_name="randomize")
+    @builtins.classmethod
+    def randomize(cls, name: builtins.str) -> builtins.str:
+        '''Create a random string to be used as a seed for IAM User password.
 
-        :param iam: Enable IAM access control. Default: true
-        :param tls: enable TLS authentication. Default: - none
+        :param name: the string to which to append a random string.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f0dd164ca1ef03c7ef58c6ede71291df119a9209e2a306b7a115179da71da707)
-            check_type(argname="argument iam", value=iam, expected_type=type_hints["iam"])
-            check_type(argname="argument tls", value=tls, expected_type=type_hints["tls"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
-        if iam is not None:
-            self._values["iam"] = iam
-        if tls is not None:
-            self._values["tls"] = tls
+            type_hints = typing.get_type_hints(_typecheckingstub__1e46f5024bfd2dc86af961c4cd184819afa4b4f01044da9ca6940bee2c2dcc0b)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+        return typing.cast(builtins.str, jsii.sinvoke(cls, "randomize", [name]))
 
-    @builtins.property
-    def iam(self) -> typing.Optional[builtins.bool]:
-        '''Enable IAM access control.
+    @jsii.member(jsii_name="readYamlDocument")
+    @builtins.classmethod
+    def read_yaml_document(cls, path: builtins.str) -> builtins.str:
+        '''Read a YAML file from the path provided and return it.
 
-        :default: true
+        :param path: the path to the file.
         '''
-        result = self._values.get("iam")
-        return typing.cast(typing.Optional[builtins.bool], result)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b8fc6dd438a6c31ad0cb5346cde32a499294a5ff963bf4c6bdfaa41fc70c2db4)
+            check_type(argname="argument path", value=path, expected_type=type_hints["path"])
+        return typing.cast(builtins.str, jsii.sinvoke(cls, "readYamlDocument", [path]))
 
-    @builtins.property
-    def tls(self) -> typing.Optional[builtins.bool]:
-        '''enable TLS authentication.
+    @jsii.member(jsii_name="stringSanitizer")
+    @builtins.classmethod
+    def string_sanitizer(cls, to_sanitize: builtins.str) -> builtins.str:
+        '''Sanitize a string by removing upper case and replacing special characters except underscore.
 
-        :default: - none
+        :param to_sanitize: the string to sanitize.
         '''
-        result = self._values.get("tls")
-        return typing.cast(typing.Optional[builtins.bool], result)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__025e16c10d80d5bc5e52559e8abad325d61eab41c0f9f27dff7670f8cc0ddb1a)
+            check_type(argname="argument to_sanitize", value=to_sanitize, expected_type=type_hints["to_sanitize"])
+        return typing.cast(builtins.str, jsii.sinvoke(cls, "stringSanitizer", [to_sanitize]))
 
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
+    @jsii.member(jsii_name="toPascalCase")
+    @builtins.classmethod
+    def to_pascal_case(cls, text: builtins.str) -> builtins.str:
+        '''Convert a string to PascalCase.
 
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
+        :param text: the string to convert to PascalCase.
 
-    def __repr__(self) -> str:
-        return "SaslVpcTlsAuthProps(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
+        :return: the string in Pascal case
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0331f7f31994294da6d4af34e71088170ba59a4c2a25908dab263b4710f4408a)
+            check_type(argname="argument text", value=text, expected_type=type_hints["text"])
+        return typing.cast(builtins.str, jsii.sinvoke(cls, "toPascalCase", [text]))
 
 
 __all__ = [
-    "Acl",
-    "AclOperationTypes",
-    "AclPermissionTypes",
-    "AclResourceTypes",
-    "Authentication",
-    "BrokerLogging",
-    "ClientAuthentication",
-    "ClusterConfigurationInfo",
-    "ClusterMonitoringLevel",
-    "EbsStorageInfo",
-    "KafkaApi",
-    "KafkaApiProps",
-    "KafkaClientLogLevel",
-    "KafkaVersion",
-    "MonitoringConfiguration",
-    "MskBrokerInstanceType",
-    "MskClusterType",
-    "MskTopic",
-    "ResourcePatternTypes",
-    "S3LoggingConfiguration",
-    "SaslAuthProps",
-    "SaslTlsAuthProps",
-    "SaslVpcTlsAuthProps",
-    "StorageMode",
-    "TlsAuthProps",
-    "VpcClientAuthentication",
-    "VpcTlsAuthProps",
+    "ApplicationStackFactory",
+    "ApplicationStage",
+    "ApplicationStageProps",
+    "Architecture",
+    "BucketUtils",
+    "CICDStage",
+    "DataVpc",
+    "DataVpcClientVpnEndpointProps",
+    "DataVpcProps",
+    "S3DataCopy",
+    "S3DataCopyProps",
+    "StepFunctionUtils",
+    "Utils",
 ]
 
 publication.publish()
 
-def _typecheckingstub__3b2c45eeb82912583d0e203bcc5f7cfa5d4679f4aa75359733b6a3b6d15aaa09(
-    *,
-    host: builtins.str,
-    operation: AclOperationTypes,
-    permission_type: AclPermissionTypes,
-    principal: builtins.str,
-    resource_name: builtins.str,
-    resource_pattern_type: ResourcePatternTypes,
-    resource_type: AclResourceTypes,
+def _typecheckingstub__4eef9172971b514785a6ce2346308753b3a0e87079b7ff4a145e5bb81378146a(
+    scope: _constructs_77d1e7e8.Construct,
+    stage: CICDStage,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__bcf29df229d45be6f58cf96f7c79a3fd20c67254205e0d4bf24c15fc1917467f(
+def _typecheckingstub__d5b5ac3de86725230614eaa05d4d588181e4795f348801b8e9846f7a8ade6698(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
     *,
-    cloudwatch_log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
-    firehose_delivery_stream_name: typing.Optional[builtins.str] = None,
-    s3: typing.Optional[typing.Union[S3LoggingConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
+    application_stack_factory: ApplicationStackFactory,
+    stage: CICDStage,
+    outputs_env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+    outdir: typing.Optional[builtins.str] = None,
+    permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
+    policy_validation_beta1: typing.Optional[typing.Sequence[_aws_cdk_ceddda9d.IPolicyValidationPluginBeta1]] = None,
+    stage_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__3836211b99f5c6335752911fac90a01a7d51a80694071ca21e83d6ed9e4ccd6e(
+def _typecheckingstub__0d0cd7bb2c6f89ceae419e95586371f2db805a9f35f0aa2ec97dcf48aa8c0209(
     *,
-    arn: builtins.str,
-    revision: jsii.Number,
+    env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
+    outdir: typing.Optional[builtins.str] = None,
+    permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
+    policy_validation_beta1: typing.Optional[typing.Sequence[_aws_cdk_ceddda9d.IPolicyValidationPluginBeta1]] = None,
+    stage_name: typing.Optional[builtins.str] = None,
+    application_stack_factory: ApplicationStackFactory,
+    stage: CICDStage,
+    outputs_env: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__3425efae5f0d6400892f5926740e3aa84485ca386ae41ba733ecaca3e0d2825d(
-    *,
-    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
-    volume_size: typing.Optional[jsii.Number] = None,
+def _typecheckingstub__88bcefb5e5ed5389168d4178ba329d512cd1938b816b8cfe7bc44a5b3124986f(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    name: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__11acb7f10ba2c540e3c133ed7f79f6ef73b1fa3e856e07fb966b40a1ffd34dc4(
+def _typecheckingstub__9563cd6cefb38ed980d4672a429ac3bfb7e0fdf90feea5a4f416b4ff13b018a7(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
-    broker_security_group: _aws_cdk_aws_ec2_ceddda9d.ISecurityGroup,
-    client_authentication: ClientAuthentication,
-    cluster_arn: builtins.str,
-    cluster_type: MskClusterType,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-    certficate_secret: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-    iam_handler_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    kafka_client_log_level: typing.Optional[KafkaClientLogLevel] = None,
-    mtls_handler_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+    vpc_cidr: builtins.str,
+    client_vpn_endpoint_props: typing.Optional[typing.Union[DataVpcClientVpnEndpointProps, typing.Dict[builtins.str, typing.Any]]] = None,
+    flow_log_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+    flow_log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
+    flow_log_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+    nat_gateways: typing.Optional[jsii.Number] = None,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b17087c46184134a6bdd689601d720ab914b7b56ad32b934fcad3f4c51f29dd0(
-    id: builtins.str,
-    topic_name: builtins.str,
-    client_authentication: Authentication,
-    principal: typing.Union[builtins.str, _aws_cdk_aws_iam_ceddda9d.IPrincipal],
-    host: typing.Optional[builtins.str] = None,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+def _typecheckingstub__006cefc76fdc1dca834321b036a66ceab95669c6f8f2eb4389a95b6405c5ca3a(
+    key: builtins.str,
+    value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__9c253515c374085f1ae8c19e0362e4924e1a2b781d754123dce2804908888e67(
-    id: builtins.str,
-    topic_name: builtins.str,
-    client_authentication: Authentication,
-    principal: typing.Union[builtins.str, _aws_cdk_aws_iam_ceddda9d.IPrincipal],
-    host: typing.Optional[builtins.str] = None,
-    removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+def _typecheckingstub__9f9e02adbd79c0e13152c12f983d4f942b325d9b511985bec14c1b11b1ad7cb9(
+    *,
+    saml_metadata_document: builtins.str,
+    server_certificate_arn: builtins.str,
+    authorize_all_users_to_vpc_cidr: typing.Optional[builtins.bool] = None,
+    dns_servers: typing.Optional[typing.Sequence[builtins.str]] = None,
+    logging: typing.Optional[builtins.bool] = None,
+    log_group: typing.Optional[_aws_cdk_aws_logs_ceddda9d.ILogGroup] = None,
+    port: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.VpnPort] = None,
+    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+    self_service_portal: typing.Optional[builtins.bool] = None,
+    session_timeout: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.ClientVpnSessionTimeout] = None,
+    split_tunnel: typing.Optional[builtins.bool] = None,
+    transport_protocol: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.TransportProtocol] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__0d1c462aeb2582babda671003a454ea0e7a7fec802c2e877a39480d04de2a004(
-    id: builtins.str,
-    acl_definition: typing.Union[Acl, typing.Dict[builtins.str, typing.Any]],
+def _typecheckingstub__39f5bd0a66c070362158feeb021d04ddf2268154575ded55b8382334b30740e6(
+    *,
+    vpc_cidr: builtins.str,
+    client_vpn_endpoint_props: typing.Optional[typing.Union[DataVpcClientVpnEndpointProps, typing.Dict[builtins.str, typing.Any]]] = None,
+    flow_log_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+    flow_log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
+    flow_log_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+    nat_gateways: typing.Optional[jsii.Number] = None,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__0906adf996cc3e4500527d7cc602db45099025693a3968a806f5ecab7596d1bf(
+def _typecheckingstub__517cea3b12f758ad38d48578dca87a1f97c700253daf18d0fa4f1079fa3b310b(
+    scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
-    client_authentication: Authentication,
-    topic_definition: typing.Union[MskTopic, typing.Dict[builtins.str, typing.Any]],
+    *,
+    source_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+    source_bucket_region: builtins.str,
+    target_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+    execution_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
-    wait_for_leaders: typing.Optional[builtins.bool] = None,
-    timeout: typing.Optional[jsii.Number] = None,
+    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+    source_bucket_prefix: typing.Optional[builtins.str] = None,
+    subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+    target_bucket_prefix: typing.Optional[builtins.str] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__8aa63759ad33545334567b3e848b5b426d5233e0f36e975fdd69080066c10ef2(
+def _typecheckingstub__b0f1736d011e3dabe341959f89b9b95889c7c24aa7cdfa70fa1893401fa55286(
     *,
-    broker_security_group: _aws_cdk_aws_ec2_ceddda9d.ISecurityGroup,
-    client_authentication: ClientAuthentication,
-    cluster_arn: builtins.str,
-    cluster_type: MskClusterType,
-    vpc: _aws_cdk_aws_ec2_ceddda9d.IVpc,
-    certficate_secret: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
-    iam_handler_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
-    kafka_client_log_level: typing.Optional[KafkaClientLogLevel] = None,
-    mtls_handler_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+    source_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+    source_bucket_region: builtins.str,
+    target_bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+    execution_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
     removal_policy: typing.Optional[_aws_cdk_ceddda9d.RemovalPolicy] = None,
+    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+    source_bucket_prefix: typing.Optional[builtins.str] = None,
     subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+    target_bucket_prefix: typing.Optional[builtins.str] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e0e8e81d0dac96cf7234f1a61b30d53c9a3d1a4d97fb2c0e99ddf481ddfdef08(
-    version: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__e2cbd7fca2428428959aa1e6b26222a5eda1ac49ca65e935d98c608d20e95b2a(
-    *,
-    cluster_monitoring_level: typing.Optional[ClusterMonitoringLevel] = None,
-    enable_prometheus_jmx_exporter: typing.Optional[builtins.bool] = None,
-    enable_prometheus_node_exporter: typing.Optional[builtins.bool] = None,
+def _typecheckingstub__8900956bb9a5e837ad18d5f562d4d1129e080f940075a87fdda2f93cb4467b66(
+    config: typing.Mapping[builtins.str, typing.Any],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__50999f64b2bf57e9a21df87c98a154cffadc71c2285baeebf0f8689e1e777429(
-    *,
-    num_partitions: jsii.Number,
-    topic: builtins.str,
-    replication_factor: typing.Optional[jsii.Number] = None,
+def _typecheckingstub__a4e130c83849df0af7b3beb5e50b0f00a681650d748a723d6c81079ec6f34336(
+    text: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__82ca97be2f9081adbed88410b7981d2cc7bbd6145b59a319f25c899a33c1587f(
-    *,
-    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
-    prefix: typing.Optional[builtins.str] = None,
+def _typecheckingstub__f70aa0e068d4cfe35caac3551a2937a15c623193142ac0abb9ea73184612ded3(
+    scope: _constructs_77d1e7e8.Construct,
+    id: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a69cfaf96dab720314a86b2aba1a3764d5dad9597e92d15b07c21a58a886d884(
-    *,
-    iam: typing.Optional[builtins.bool] = None,
+def _typecheckingstub__f08bfe619a6fde71b5609a00f036443fb3dcf2ab30d09c795dbe0f7f0475a43d(
+    document: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b75ace651f25eb081badf2271fb655bc4c0850e36bafe6b474f39e00935bb0c7(
-    *,
-    certificate_authorities: typing.Optional[typing.Sequence[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]] = None,
+def _typecheckingstub__1e46f5024bfd2dc86af961c4cd184819afa4b4f01044da9ca6940bee2c2dcc0b(
+    name: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__bfa989fad1cbc8518acad9bce75e30465e418b0228fe1dd3da8649e86a493beb(
-    *,
-    tls: typing.Optional[builtins.bool] = None,
+def _typecheckingstub__b8fc6dd438a6c31ad0cb5346cde32a499294a5ff963bf4c6bdfaa41fc70c2db4(
+    path: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b540b95307fdb73492eba61e5c3ad3f2ea64ba068d1b2d8d32d407a1f8dd7d37(
-    *,
-    iam: typing.Optional[builtins.bool] = None,
-    certificate_authorities: typing.Optional[typing.Sequence[_aws_cdk_aws_acmpca_ceddda9d.ICertificateAuthority]] = None,
+def _typecheckingstub__025e16c10d80d5bc5e52559e8abad325d61eab41c0f9f27dff7670f8cc0ddb1a(
+    to_sanitize: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__f0dd164ca1ef03c7ef58c6ede71291df119a9209e2a306b7a115179da71da707(
-    *,
-    iam: typing.Optional[builtins.bool] = None,
-    tls: typing.Optional[builtins.bool] = None,
+def _typecheckingstub__0331f7f31994294da6d4af34e71088170ba59a4c2a25908dab263b4710f4408a(
+    text: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/PKG-INFO` & `cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs.aws_data_solutions_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.aws-data-solutions-framework
-Version: 1.7.0
+Version: 1.8.0
 Summary: L3 CDK Constructs used to build data solutions with AWS
 Home-page: https://awslabs.github.io/data-solutions-framework-on-aws/
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/data-solutions-framework-on-aws.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.aws_data_solutions_framework-1.7.0/src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt` & `cdklabs.aws_data_solutions_framework-1.8.0/src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt
 src/cdklabs.aws_data_solutions_framework.egg-info/dependency_links.txt
 src/cdklabs.aws_data_solutions_framework.egg-info/requires.txt
 src/cdklabs.aws_data_solutions_framework.egg-info/top_level.txt
 src/cdklabs/aws_data_solutions_framework/__init__.py
 src/cdklabs/aws_data_solutions_framework/py.typed
 src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py
-src/cdklabs/aws_data_solutions_framework/_jsii/aws-data-solutions-framework@1.7.0.jsii.tgz
+src/cdklabs/aws_data_solutions_framework/_jsii/aws-data-solutions-framework@1.8.0.jsii.tgz
 src/cdklabs/aws_data_solutions_framework/consumption/__init__.py
 src/cdklabs/aws_data_solutions_framework/governance/__init__.py
 src/cdklabs/aws_data_solutions_framework/processing/__init__.py
 src/cdklabs/aws_data_solutions_framework/storage/__init__.py
 src/cdklabs/aws_data_solutions_framework/streaming/__init__.py
 src/cdklabs/aws_data_solutions_framework/utils/__init__.py
```

