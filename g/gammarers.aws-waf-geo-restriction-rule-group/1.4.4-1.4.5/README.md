# Comparing `tmp/gammarers.aws-waf-geo-restriction-rule-group-1.4.4.tar.gz` & `tmp/gammarers.aws-waf-geo-restriction-rule-group-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-waf-geo-restriction-rule-group-1.4.4.tar", last modified: Mon May 20 19:20:41 2024, max compression
+gzip compressed data, was "gammarers.aws-waf-geo-restriction-rule-group-1.4.5.tar", last modified: Mon May 27 19:21:51 2024, max compression
```

## Comparing `gammarers.aws-waf-geo-restriction-rule-group-1.4.4.tar` & `gammarers.aws-waf-geo-restriction-rule-group-1.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:41.626744 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-20 19:20:30.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 19:20:30.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-20 19:20:41.626744 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-20 19:20:30.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-20 19:20:30.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:20:41.626744 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-20 19:20:30.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:41.622744 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:41.622744 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:41.626744 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers/aws_waf_geo_restriction_rule_group/
--rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-05-20 19:20:30.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers/aws_waf_geo_restriction_rule_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:41.626744 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers/aws_waf_geo_restriction_rule_group/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-20 19:20:30.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers/aws_waf_geo_restriction_rule_group/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26670 2024-05-20 19:20:30.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers/aws_waf_geo_restriction_rule_group/_jsii/aws-waf-geo-restriction-rule-group@1.4.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:20:30.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers/aws_waf_geo_restriction_rule_group/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:41.626744 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-20 19:20:41.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-20 19:20:41.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:20:41.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-20 19:20:41.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 19:20:41.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:51.115413 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-27 19:21:39.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 19:21:39.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-27 19:21:51.115413 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-27 19:21:39.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-27 19:21:39.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 19:21:51.115413 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-27 19:21:39.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:51.111413 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:51.111413 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:51.115413 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers/aws_waf_geo_restriction_rule_group/
+-rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-05-27 19:21:39.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers/aws_waf_geo_restriction_rule_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:51.115413 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers/aws_waf_geo_restriction_rule_group/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-27 19:21:39.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers/aws_waf_geo_restriction_rule_group/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26687 2024-05-27 19:21:39.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers/aws_waf_geo_restriction_rule_group/_jsii/aws-waf-geo-restriction-rule-group@1.4.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:21:39.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers/aws_waf_geo_restriction_rule_group/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 19:21:51.115413 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-27 19:21:51.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-27 19:21:51.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 19:21:51.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-27 19:21:51.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 19:21:51.000000 gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/top_level.txt
```

### Comparing `gammarers.aws-waf-geo-restriction-rule-group-1.4.4/LICENSE` & `gammarers.aws-waf-geo-restriction-rule-group-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-waf-geo-restriction-rule-group-1.4.4/PKG-INFO` & `gammarers.aws-waf-geo-restriction-rule-group-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-waf-geo-restriction-rule-group
-Version: 1.4.4
+Version: 1.4.5
 Summary: This is an AWS CDK Construct for Geo Restriction Rule Group on WAF V2
 Home-page: https://github.com/gammarers/aws-waf-geo-restriction-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-waf-geo-restriction-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-waf-geo-restriction-rule-group-1.4.4/README.md` & `gammarers.aws-waf-geo-restriction-rule-group-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-waf-geo-restriction-rule-group-1.4.4/setup.py` & `gammarers.aws-waf-geo-restriction-rule-group-1.4.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-waf-geo-restriction-rule-group",
-    "version": "1.4.4",
+    "version": "1.4.5",
     "description": "This is an AWS CDK Construct for Geo Restriction Rule Group on WAF V2",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-waf-geo-restriction-rule-group.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarers.aws_waf_geo_restriction_rule_group",
         "gammarers.aws_waf_geo_restriction_rule_group._jsii"
     ],
     "package_data": {
         "gammarers.aws_waf_geo_restriction_rule_group._jsii": [
-            "aws-waf-geo-restriction-rule-group@1.4.4.jsii.tgz"
+            "aws-waf-geo-restriction-rule-group@1.4.5.jsii.tgz"
         ],
         "gammarers.aws_waf_geo_restriction_rule_group": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers/aws_waf_geo_restriction_rule_group/__init__.py` & `gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers/aws_waf_geo_restriction_rule_group/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers/aws_waf_geo_restriction_rule_group/_jsii/__init__.py` & `gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers/aws_waf_geo_restriction_rule_group/_jsii/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-waf-geo-restriction-rule-group",
-    "1.4.4",
+    "1.4.5",
     __name__[0:-6],
-    "aws-waf-geo-restriction-rule-group@1.4.4.jsii.tgz",
+    "aws-waf-geo-restriction-rule-group@1.4.5.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/PKG-INFO` & `gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-waf-geo-restriction-rule-group
-Version: 1.4.4
+Version: 1.4.5
 Summary: This is an AWS CDK Construct for Geo Restriction Rule Group on WAF V2
 Home-page: https://github.com/gammarers/aws-waf-geo-restriction-rule-group.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-waf-geo-restriction-rule-group.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-waf-geo-restriction-rule-group-1.4.4/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt` & `gammarers.aws-waf-geo-restriction-rule-group-1.4.5/src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/SOURCES.txt
 src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/dependency_links.txt
 src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/requires.txt
 src/gammarers.aws_waf_geo_restriction_rule_group.egg-info/top_level.txt
 src/gammarers/aws_waf_geo_restriction_rule_group/__init__.py
 src/gammarers/aws_waf_geo_restriction_rule_group/py.typed
 src/gammarers/aws_waf_geo_restriction_rule_group/_jsii/__init__.py
-src/gammarers/aws_waf_geo_restriction_rule_group/_jsii/aws-waf-geo-restriction-rule-group@1.4.4.jsii.tgz
+src/gammarers/aws_waf_geo_restriction_rule_group/_jsii/aws-waf-geo-restriction-rule-group@1.4.5.jsii.tgz
```

