# Comparing `tmp/pulumi-aws-tags-0.7.0.tar.gz` & `tmp/pulumi_aws_tags-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi-aws-tags-0.7.0.tar", last modified: Tue Mar 19 15:00:11 2024, max compression
+gzip compressed data, was "pulumi_aws_tags-0.7.1.tar", last modified: Mon May 27 12:23:53 2024, max compression
```

## Comparing `pulumi-aws-tags-0.7.0.tar` & `pulumi_aws_tags-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:11.676603 pulumi-aws-tags-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-19 15:00:11.676603 pulumi-aws-tags-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-19 14:59:56.000000 pulumi-aws-tags-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:11.676603 pulumi-aws-tags-0.7.0/pulumi_aws_tags/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-19 14:59:56.000000 pulumi-aws-tags-0.7.0/pulumi_aws_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-19 14:59:56.000000 pulumi-aws-tags-0.7.0/pulumi_aws_tags/autotag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-19 14:59:56.000000 pulumi-aws-tags-0.7.0/pulumi_aws_tags/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:11.676603 pulumi-aws-tags-0.7.0/pulumi_aws_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-19 15:00:11.000000 pulumi-aws-tags-0.7.0/pulumi_aws_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-19 15:00:11.000000 pulumi-aws-tags-0.7.0/pulumi_aws_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 15:00:11.000000 pulumi-aws-tags-0.7.0/pulumi_aws_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-19 15:00:11.000000 pulumi-aws-tags-0.7.0/pulumi_aws_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-19 15:00:11.000000 pulumi-aws-tags-0.7.0/pulumi_aws_tags.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 15:00:11.676603 pulumi-aws-tags-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-19 14:59:56.000000 pulumi-aws-tags-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:00:11.676603 pulumi-aws-tags-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-19 14:59:56.000000 pulumi-aws-tags-0.7.0/tests/test_autotag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:23:53.108017 pulumi_aws_tags-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-27 12:23:53.108017 pulumi_aws_tags-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-27 12:23:38.000000 pulumi_aws_tags-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:23:53.108017 pulumi_aws_tags-0.7.1/pulumi_aws_tags/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-27 12:23:38.000000 pulumi_aws_tags-0.7.1/pulumi_aws_tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-27 12:23:38.000000 pulumi_aws_tags-0.7.1/pulumi_aws_tags/autotag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-27 12:23:38.000000 pulumi_aws_tags-0.7.1/pulumi_aws_tags/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:23:53.108017 pulumi_aws_tags-0.7.1/pulumi_aws_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-27 12:23:53.000000 pulumi_aws_tags-0.7.1/pulumi_aws_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-27 12:23:53.000000 pulumi_aws_tags-0.7.1/pulumi_aws_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:23:53.000000 pulumi_aws_tags-0.7.1/pulumi_aws_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 12:23:53.000000 pulumi_aws_tags-0.7.1/pulumi_aws_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 12:23:53.000000 pulumi_aws_tags-0.7.1/pulumi_aws_tags.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-27 12:23:38.000000 pulumi_aws_tags-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:23:53.108017 pulumi_aws_tags-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:23:53.108017 pulumi_aws_tags-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-27 12:23:38.000000 pulumi_aws_tags-0.7.1/tests/test_autotag.py
```

### Comparing `pulumi-aws-tags-0.7.0/PKG-INFO` & `pulumi_aws_tags-0.7.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
-Name: pulumi-aws-tags
-Version: 0.7.0
+Name: pulumi_aws_tags
+Version: 0.7.1
 Summary: Pulumi package that helps manage tags for AWS resources
-Home-page: https://github.com/tlinhart/pulumi-aws-tags
-Author: Tomáš Linhart
-Author-email: pasmen@gmail.com
-License: MIT
-Keywords: pulumi aws tags
-Classifier: Programming Language :: Python :: 3
+Author-email: Tomáš Linhart <pasmen@gmail.com>
+Project-URL: Homepage, https://github.com/tlinhart/pulumi-aws-tags
+Keywords: pulumi,aws,tags
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pulumi<4.0.0,>=3.0.0
-Requires-Dist: pulumi-aws<7.0.0,>=4.0.0
+Requires-Dist: pulumi_aws<7.0.0,>=4.0.0
 
 # Pulumi AWS Tags
 
 Pulumi package that helps manage tags for AWS resources.
 
 ## Installation
```

### Comparing `pulumi-aws-tags-0.7.0/pulumi_aws_tags/autotag.py` & `pulumi_aws_tags-0.7.1/pulumi_aws_tags/autotag.py`

 * *Files identical despite different names*

### Comparing `pulumi-aws-tags-0.7.0/pulumi_aws_tags/taggable.py` & `pulumi_aws_tags-0.7.1/pulumi_aws_tags/taggable.py`

 * *Files identical despite different names*

### Comparing `pulumi-aws-tags-0.7.0/pulumi_aws_tags.egg-info/PKG-INFO` & `pulumi_aws_tags-0.7.1/pulumi_aws_tags.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
-Name: pulumi-aws-tags
-Version: 0.7.0
+Name: pulumi_aws_tags
+Version: 0.7.1
 Summary: Pulumi package that helps manage tags for AWS resources
-Home-page: https://github.com/tlinhart/pulumi-aws-tags
-Author: Tomáš Linhart
-Author-email: pasmen@gmail.com
-License: MIT
-Keywords: pulumi aws tags
-Classifier: Programming Language :: Python :: 3
+Author-email: Tomáš Linhart <pasmen@gmail.com>
+Project-URL: Homepage, https://github.com/tlinhart/pulumi-aws-tags
+Keywords: pulumi,aws,tags
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pulumi<4.0.0,>=3.0.0
-Requires-Dist: pulumi-aws<7.0.0,>=4.0.0
+Requires-Dist: pulumi_aws<7.0.0,>=4.0.0
 
 # Pulumi AWS Tags
 
 Pulumi package that helps manage tags for AWS resources.
 
 ## Installation
```

### Comparing `pulumi-aws-tags-0.7.0/tests/test_autotag.py` & `pulumi_aws_tags-0.7.1/tests/test_autotag.py`

 * *Files identical despite different names*

