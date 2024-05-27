# Comparing `tmp/pulumiverse_doppler-0.7.0.tar.gz` & `tmp/pulumiverse_doppler-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_doppler-0.7.0.tar", last modified: Thu May  2 08:29:34 2024, max compression
+gzip compressed data, was "pulumiverse_doppler-0.7.1.tar", last modified: Mon May 27 09:17:38 2024, max compression
```

## Comparing `pulumiverse_doppler-0.7.0.tar` & `pulumiverse_doppler-0.7.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:29:34.489793 pulumiverse_doppler-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-02 08:29:34.489793 pulumiverse_doppler-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:29:34.485793 pulumiverse_doppler-0.7.0/pulumiverse_doppler/
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/branch_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:29:34.485793 pulumiverse_doppler-0.7.0/pulumiverse_doppler/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/get_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/group_member.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:29:34.485793 pulumiverse_doppler-0.7.0/pulumiverse_doppler/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/integration/aws_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/integration/aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/integration/terraform_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:29:34.485793 pulumiverse_doppler-0.7.0/pulumiverse_doppler/projectmember/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/projectmember/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/projectmember/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/projectmember/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:29:34.489793 pulumiverse_doppler-0.7.0/pulumiverse_doppler/secretssync/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/secretssync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21335 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/secretssync/aws_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18377 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/secretssync/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/secretssync/terraform_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler/service_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:29:34.485793 pulumiverse_doppler-0.7.0/pulumiverse_doppler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/pulumiverse_doppler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:29:34.489793 pulumiverse_doppler-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-02 08:29:34.000000 pulumiverse_doppler-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:17:38.116553 pulumiverse_doppler-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-27 09:17:38.116553 pulumiverse_doppler-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:17:38.116553 pulumiverse_doppler-0.7.1/pulumiverse_doppler/
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/branch_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:17:38.116553 pulumiverse_doppler-0.7.1/pulumiverse_doppler/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/get_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/group_member.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:17:38.116553 pulumiverse_doppler-0.7.1/pulumiverse_doppler/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/integration/aws_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/integration/aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/integration/terraform_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:17:38.116553 pulumiverse_doppler-0.7.1/pulumiverse_doppler/projectmember/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/projectmember/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/projectmember/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/projectmember/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:17:38.116553 pulumiverse_doppler-0.7.1/pulumiverse_doppler/secretssync/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/secretssync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21335 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/secretssync/aws_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/secretssync/aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18377 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/secretssync/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18219 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/secretssync/terraform_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12701 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler/service_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 09:17:38.116553 pulumiverse_doppler-0.7.1/pulumiverse_doppler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-27 09:17:38.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-27 09:17:38.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:17:38.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 09:17:38.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 09:17:38.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 09:17:38.000000 pulumiverse_doppler-0.7.1/pulumiverse_doppler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 09:17:38.120553 pulumiverse_doppler-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-27 09:17:37.000000 pulumiverse_doppler-0.7.1/setup.py
```

### Comparing `pulumiverse_doppler-0.7.0/PKG-INFO` & `pulumiverse_doppler-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_doppler
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.7.0/README.md` & `pulumiverse_doppler-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/__init__.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/_utilities.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/branch_config.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/branch_config.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/config/vars.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/environment.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/environment.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/get_secrets.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/get_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/get_user.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/group.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/group_member.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/group_member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/integration/aws_parameter_store.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/integration/aws_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/integration/aws_secrets_manager.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/integration/aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/integration/terraform_cloud.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/integration/terraform_cloud.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,26 +14,22 @@
 @pulumi.input_type
 class TerraformCloudArgs:
     def __init__(__self__, *,
                  api_key: pulumi.Input[str],
                  name: pulumi.Input[str]):
         """
         The set of arguments for constructing a TerraformCloud resource.
-        :param pulumi.Input[str] api_key: A Terraform Cloud API key.
         :param pulumi.Input[str] name: The name of the integration
         """
         pulumi.set(__self__, "api_key", api_key)
         pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter(name="apiKey")
     def api_key(self) -> pulumi.Input[str]:
-        """
-        A Terraform Cloud API key.
-        """
         return pulumi.get(self, "api_key")
 
     @api_key.setter
     def api_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "api_key", value)
 
     @property
@@ -52,28 +48,24 @@
 @pulumi.input_type
 class _TerraformCloudState:
     def __init__(__self__, *,
                  api_key: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering TerraformCloud resources.
-        :param pulumi.Input[str] api_key: A Terraform Cloud API key.
         :param pulumi.Input[str] name: The name of the integration
         """
         if api_key is not None:
             pulumi.set(__self__, "api_key", api_key)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter(name="apiKey")
     def api_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        A Terraform Cloud API key.
-        """
         return pulumi.get(self, "api_key")
 
     @api_key.setter
     def api_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "api_key", value)
 
     @property
@@ -98,15 +90,14 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] api_key: A Terraform Cloud API key.
         :param pulumi.Input[str] name: The name of the integration
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TerraformCloudArgs,
@@ -163,31 +154,27 @@
         """
         Get an existing TerraformCloud resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] api_key: A Terraform Cloud API key.
         :param pulumi.Input[str] name: The name of the integration
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TerraformCloudState.__new__(_TerraformCloudState)
 
         __props__.__dict__["api_key"] = api_key
         __props__.__dict__["name"] = name
         return TerraformCloud(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="apiKey")
     def api_key(self) -> pulumi.Output[str]:
-        """
-        A Terraform Cloud API key.
-        """
         return pulumi.get(self, "api_key")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         The name of the integration
```

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/project.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/projectmember/group.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/projectmember/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/projectmember/service_account.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/projectmember/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/provider.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/secret.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/secret.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/secretssync/aws_parameter_store.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/secretssync/aws_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/secretssync/aws_secrets_manager.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/secretssync/aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/secretssync/github_actions.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/secretssync/github_actions.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/secretssync/terraform_cloud.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/secretssync/terraform_cloud.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,17 +25,14 @@
         """
         The set of arguments for constructing a TerraformCloud resource.
         :param pulumi.Input[str] config: The name of the Doppler config
         :param pulumi.Input[str] integration: The slug of the integration to use for this sync
         :param pulumi.Input[str] name_transform: A name transform to apply before syncing secrets: "none" or "lowercase"
         :param pulumi.Input[str] project: The name of the Doppler project
         :param pulumi.Input[str] sync_target: Either "workspace" or "variableSet", based on the resource type to sync to
-        :param pulumi.Input[str] variable_sync_type: Either "terraform" to sync secrets as Terraform variables or "env" to sync as environment variables
-        :param pulumi.Input[str] variable_set_id: The Terraform Cloud variable set ID to sync to
-        :param pulumi.Input[str] workspace_id: The Terraform Cloud workspace ID to sync to
         """
         pulumi.set(__self__, "config", config)
         pulumi.set(__self__, "integration", integration)
         pulumi.set(__self__, "name_transform", name_transform)
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "sync_target", sync_target)
         pulumi.set(__self__, "variable_sync_type", variable_sync_type)
@@ -103,41 +100,32 @@
     @sync_target.setter
     def sync_target(self, value: pulumi.Input[str]):
         pulumi.set(self, "sync_target", value)
 
     @property
     @pulumi.getter(name="variableSyncType")
     def variable_sync_type(self) -> pulumi.Input[str]:
-        """
-        Either "terraform" to sync secrets as Terraform variables or "env" to sync as environment variables
-        """
         return pulumi.get(self, "variable_sync_type")
 
     @variable_sync_type.setter
     def variable_sync_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "variable_sync_type", value)
 
     @property
     @pulumi.getter(name="variableSetId")
     def variable_set_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        The Terraform Cloud variable set ID to sync to
-        """
         return pulumi.get(self, "variable_set_id")
 
     @variable_set_id.setter
     def variable_set_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "variable_set_id", value)
 
     @property
     @pulumi.getter(name="workspaceId")
     def workspace_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        The Terraform Cloud workspace ID to sync to
-        """
         return pulumi.get(self, "workspace_id")
 
     @workspace_id.setter
     def workspace_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "workspace_id", value)
 
 
@@ -155,17 +143,14 @@
         """
         Input properties used for looking up and filtering TerraformCloud resources.
         :param pulumi.Input[str] config: The name of the Doppler config
         :param pulumi.Input[str] integration: The slug of the integration to use for this sync
         :param pulumi.Input[str] name_transform: A name transform to apply before syncing secrets: "none" or "lowercase"
         :param pulumi.Input[str] project: The name of the Doppler project
         :param pulumi.Input[str] sync_target: Either "workspace" or "variableSet", based on the resource type to sync to
-        :param pulumi.Input[str] variable_set_id: The Terraform Cloud variable set ID to sync to
-        :param pulumi.Input[str] variable_sync_type: Either "terraform" to sync secrets as Terraform variables or "env" to sync as environment variables
-        :param pulumi.Input[str] workspace_id: The Terraform Cloud workspace ID to sync to
         """
         if config is not None:
             pulumi.set(__self__, "config", config)
         if integration is not None:
             pulumi.set(__self__, "integration", integration)
         if name_transform is not None:
             pulumi.set(__self__, "name_transform", name_transform)
@@ -239,41 +224,32 @@
     @sync_target.setter
     def sync_target(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "sync_target", value)
 
     @property
     @pulumi.getter(name="variableSetId")
     def variable_set_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        The Terraform Cloud variable set ID to sync to
-        """
         return pulumi.get(self, "variable_set_id")
 
     @variable_set_id.setter
     def variable_set_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "variable_set_id", value)
 
     @property
     @pulumi.getter(name="variableSyncType")
     def variable_sync_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        Either "terraform" to sync secrets as Terraform variables or "env" to sync as environment variables
-        """
         return pulumi.get(self, "variable_sync_type")
 
     @variable_sync_type.setter
     def variable_sync_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "variable_sync_type", value)
 
     @property
     @pulumi.getter(name="workspaceId")
     def workspace_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        The Terraform Cloud workspace ID to sync to
-        """
         return pulumi.get(self, "workspace_id")
 
     @workspace_id.setter
     def workspace_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "workspace_id", value)
 
 
@@ -297,17 +273,14 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] config: The name of the Doppler config
         :param pulumi.Input[str] integration: The slug of the integration to use for this sync
         :param pulumi.Input[str] name_transform: A name transform to apply before syncing secrets: "none" or "lowercase"
         :param pulumi.Input[str] project: The name of the Doppler project
         :param pulumi.Input[str] sync_target: Either "workspace" or "variableSet", based on the resource type to sync to
-        :param pulumi.Input[str] variable_set_id: The Terraform Cloud variable set ID to sync to
-        :param pulumi.Input[str] variable_sync_type: Either "terraform" to sync secrets as Terraform variables or "env" to sync as environment variables
-        :param pulumi.Input[str] workspace_id: The Terraform Cloud workspace ID to sync to
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TerraformCloudArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -392,17 +365,14 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] config: The name of the Doppler config
         :param pulumi.Input[str] integration: The slug of the integration to use for this sync
         :param pulumi.Input[str] name_transform: A name transform to apply before syncing secrets: "none" or "lowercase"
         :param pulumi.Input[str] project: The name of the Doppler project
         :param pulumi.Input[str] sync_target: Either "workspace" or "variableSet", based on the resource type to sync to
-        :param pulumi.Input[str] variable_set_id: The Terraform Cloud variable set ID to sync to
-        :param pulumi.Input[str] variable_sync_type: Either "terraform" to sync secrets as Terraform variables or "env" to sync as environment variables
-        :param pulumi.Input[str] workspace_id: The Terraform Cloud workspace ID to sync to
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TerraformCloudState.__new__(_TerraformCloudState)
 
         __props__.__dict__["config"] = config
         __props__.__dict__["integration"] = integration
@@ -453,28 +423,19 @@
         Either "workspace" or "variableSet", based on the resource type to sync to
         """
         return pulumi.get(self, "sync_target")
 
     @property
     @pulumi.getter(name="variableSetId")
     def variable_set_id(self) -> pulumi.Output[Optional[str]]:
-        """
-        The Terraform Cloud variable set ID to sync to
-        """
         return pulumi.get(self, "variable_set_id")
 
     @property
     @pulumi.getter(name="variableSyncType")
     def variable_sync_type(self) -> pulumi.Output[str]:
-        """
-        Either "terraform" to sync secrets as Terraform variables or "env" to sync as environment variables
-        """
         return pulumi.get(self, "variable_sync_type")
 
     @property
     @pulumi.getter(name="workspaceId")
     def workspace_id(self) -> pulumi.Output[Optional[str]]:
-        """
-        The Terraform Cloud workspace ID to sync to
-        """
         return pulumi.get(self, "workspace_id")
```

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/service_account.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler/service_token.py` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler/service_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler.egg-info/PKG-INFO` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-doppler
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Pulumi package for creating and managing doppler cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-doppler
 Keywords: pulumi doppler category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_doppler-0.7.0/pulumiverse_doppler.egg-info/SOURCES.txt` & `pulumiverse_doppler-0.7.1/pulumiverse_doppler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_doppler-0.7.0/setup.py` & `pulumiverse_doppler-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.7.0"
+VERSION = "0.7.1"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "doppler Pulumi Package - Development Version"
```

