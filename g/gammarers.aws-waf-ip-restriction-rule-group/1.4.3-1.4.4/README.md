# Comparing `tmp/gammarers.aws-waf-ip-restriction-rule-group-1.4.3.tar.gz` & `tmp/gammarers.aws-waf-ip-restriction-rule-group-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-waf-ip-restriction-rule-group-1.4.3.tar", last modified: Mon May 20 19:20:08 2024, max compression
+gzip compressed data, was "gammarers.aws-waf-ip-restriction-rule-group-1.4.4.tar", last modified: Mon May 27 19:20:50 2024, max compression
```

## Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.3.tar` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:08.578527 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-20 19:19:58.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 19:19:58.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-20 19:20:08.578527 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-20 19:19:58.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-20 19:19:58.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:20:08.578527 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-20 19:19:58.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:08.574526 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:08.574526 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:08.578527 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers/aws_waf_ip_restriction_rule_group/
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-05-20 19:19:58.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers/aws_waf_ip_restriction_rule_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:08.578527 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-20 19:19:58.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23967 2024-05-20 19:19:58.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/aws-waf-ip-restriction-rule-group@1.4.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:19:58.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers/aws_waf_ip_restriction_rule_group/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:08.578527 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-20 19:20:08.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-20 19:20:08.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:20:08.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-20 19:20:08.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 19:20:08.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:50.084214 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-27 19:20:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 19:20:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-27 19:20:50.084214 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-27 19:20:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-27 19:20:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:20:50.084214 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-27 19:20:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:50.084214 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:50.084214 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:50.084214 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers/aws_waf_ip_restriction_rule_group/
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-05-27 19:20:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers/aws_waf_ip_restriction_rule_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:50.084214 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-27 19:20:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23982 2024-05-27 19:20:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/aws-waf-ip-restriction-rule-group@1.4.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:20:39.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers/aws_waf_ip_restriction_rule_group/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:20:50.084214 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-27 19:20:50.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-27 19:20:50.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:20:50.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-27 19:20:50.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 19:20:50.000000 gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/top_level.txt
```

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.3/LICENSE` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.3/PKG-INFO` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-waf-ip-restriction-rule-group
-Version: 1.4.3
+Version: 1.4.4
 Summary: This is an AWS CDK Construct for IP Restriction Rule Group on WAF V2
 Home-page: https://github.com/gammarers/aws-waf-ip-restriction-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-waf-ip-restriction-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.3/README.md` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.3/setup.py` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-waf-ip-restriction-rule-group",
-    "version": "1.4.3",
+    "version": "1.4.4",
     "description": "This is an AWS CDK Construct for IP Restriction Rule Group on WAF V2",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-waf-ip-restriction-rule-group.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarers.aws_waf_ip_restriction_rule_group",
         "gammarers.aws_waf_ip_restriction_rule_group._jsii"
     ],
     "package_data": {
         "gammarers.aws_waf_ip_restriction_rule_group._jsii": [
-            "aws-waf-ip-restriction-rule-group@1.4.3.jsii.tgz"
+            "aws-waf-ip-restriction-rule-group@1.4.4.jsii.tgz"
         ],
         "gammarers.aws_waf_ip_restriction_rule_group": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers/aws_waf_ip_restriction_rule_group/__init__.py` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers/aws_waf_ip_restriction_rule_group/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/__init__.py` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-waf-ip-restriction-rule-group",
-    "1.4.3",
+    "1.4.4",
     __name__[0:-6],
-    "aws-waf-ip-restriction-rule-group@1.4.3.jsii.tgz",
+    "aws-waf-ip-restriction-rule-group@1.4.4.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/PKG-INFO` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-waf-ip-restriction-rule-group
-Version: 1.4.3
+Version: 1.4.4
 Summary: This is an AWS CDK Construct for IP Restriction Rule Group on WAF V2
 Home-page: https://github.com/gammarers/aws-waf-ip-restriction-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-waf-ip-restriction-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-waf-ip-restriction-rule-group-1.4.3/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/SOURCES.txt` & `gammarers.aws-waf-ip-restriction-rule-group-1.4.4/src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/SOURCES.txt
 src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/dependency_links.txt
 src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/requires.txt
 src/gammarers.aws_waf_ip_restriction_rule_group.egg-info/top_level.txt
 src/gammarers/aws_waf_ip_restriction_rule_group/__init__.py
 src/gammarers/aws_waf_ip_restriction_rule_group/py.typed
 src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/__init__.py
-src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/aws-waf-ip-restriction-rule-group@1.4.3.jsii.tgz
+src/gammarers/aws_waf_ip_restriction_rule_group/_jsii/aws-waf-ip-restriction-rule-group@1.4.4.jsii.tgz
```

