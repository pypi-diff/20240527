# Comparing `tmp/lam_cli-0.0.6.tar.gz` & `tmp/lam_cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lam_cli-0.0.6.tar", last modified: Wed May 22 21:01:58 2024, max compression
+gzip compressed data, was "lam_cli-0.0.7.tar", last modified: Mon May 27 14:37:41 2024, max compression
```

## Comparing `lam_cli-0.0.6.tar` & `lam_cli-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:01:58.058709 lam_cli-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-22 21:01:54.000000 lam_cli-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-22 21:01:58.058709 lam_cli-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-22 21:01:54.000000 lam_cli-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:01:58.058709 lam_cli-0.0.6/lam/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:01:54.000000 lam_cli-0.0.6/lam/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7269 2024-05-22 21:01:54.000000 lam_cli-0.0.6/lam/lam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:01:58.058709 lam_cli-0.0.6/lam_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-22 21:01:58.000000 lam_cli-0.0.6/lam_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-22 21:01:58.000000 lam_cli-0.0.6/lam_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:01:58.000000 lam_cli-0.0.6/lam_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 21:01:58.000000 lam_cli-0.0.6/lam_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 21:01:58.000000 lam_cli-0.0.6/lam_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 21:01:58.000000 lam_cli-0.0.6/lam_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:01:58.058709 lam_cli-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-22 21:01:54.000000 lam_cli-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:41.339978 lam_cli-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-27 14:37:37.000000 lam_cli-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-27 14:37:41.339978 lam_cli-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-27 14:37:37.000000 lam_cli-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:41.339978 lam_cli-0.0.7/lam/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:37.000000 lam_cli-0.0.7/lam/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7383 2024-05-27 14:37:37.000000 lam_cli-0.0.7/lam/lam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:37:41.339978 lam_cli-0.0.7/lam_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-27 14:37:41.000000 lam_cli-0.0.7/lam_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-27 14:37:41.000000 lam_cli-0.0.7/lam_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:37:41.000000 lam_cli-0.0.7/lam_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 14:37:41.000000 lam_cli-0.0.7/lam_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 14:37:41.000000 lam_cli-0.0.7/lam_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 14:37:41.000000 lam_cli-0.0.7/lam_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:37:41.339978 lam_cli-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-27 14:37:37.000000 lam_cli-0.0.7/setup.py
```

### Comparing `lam_cli-0.0.6/LICENSE` & `lam_cli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lam_cli-0.0.6/README.md` & `lam_cli-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lam_cli-0.0.6/lam/lam.py` & `lam_cli-0.0.7/lam/lam.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,19 +100,20 @@
     pass
 
 @lam.command()
 @click.argument('program_file', type=click.Path(exists=True))
 @click.argument('input', type=str)
 @click.option('--workspace_id', default="local", help="Workspace ID")
 @click.option('--flow_id', default="local", help="Flow ID")
+@click.option('--execution_id', default="local", help="Execution ID")
 @click.option('--as-json', is_flag=True, default=True, help="Output as JSON")
-def run(program_file, input, workspace_id, flow_id, as_json):
+def run(program_file, input, workspace_id, flow_id, execution_id, as_json):
     timestamp = datetime.now().strftime('%Y%m%d_%H%M%S')
-    log_file = f"lam_run_{workspace_id}_{flow_id}_{timestamp}.log"
-    result_file = f"lam_result_{workspace_id}_{flow_id}_{timestamp}.json"
+    log_file = f"lam_run_{workspace_id}_{flow_id}_{execution_id}_{timestamp}.log"
+    result_file = f"lam_result_{workspace_id}_{flow_id}_{execution_id}_{timestamp}.json"
 
     file_handler = logging.FileHandler(log_file, 'w')
     file_handler.setFormatter(logging.Formatter('%(asctime)s - %(levelname)s - %(message)s'))
     logger.addHandler(file_handler)
 
     logger.info(f"Logging to {log_file}")
     logger.info(f"Running command with program file: {program_file}, input: {truncate_long_strings(input)}, workspace_id: {workspace_id}, flow_id: {flow_id}, as_json: {as_json}")
```

### Comparing `lam_cli-0.0.6/setup.py` & `lam_cli-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='lam-cli',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     install_requires=[
         'click',
         'posthog',
         'logtail-python',
     ],
     entry_points={
```

