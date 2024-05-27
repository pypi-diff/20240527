# Comparing `tmp/launch_generator-0.5.0.tar.gz` & `tmp/launch_generator-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launch_generator-0.5.0.tar", last modified: Sat Feb 17 01:56:04 2024, max compression
+gzip compressed data, was "launch_generator-0.5.1.tar", last modified: Mon May 27 14:00:56 2024, max compression
```

## Comparing `launch_generator-0.5.0.tar` & `launch_generator-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-17 01:56:04.125964 launch_generator-0.5.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-02-17 01:55:57.000000 launch_generator-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      357 2024-02-17 01:56:04.125964 launch_generator-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10634 2024-02-17 01:55:57.000000 launch_generator-0.5.0/README.md
--rw-r--r--   0 root         (0) root         (0)      482 2024-02-17 01:55:57.000000 launch_generator-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-17 01:56:04.125964 launch_generator-0.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1072 2024-02-17 01:55:57.000000 launch_generator-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-17 01:56:04.121964 launch_generator-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-17 01:56:04.125964 launch_generator-0.5.0/src/launch_generator/
--rw-r--r--   0 root         (0) root         (0)     1048 2024-02-17 01:55:57.000000 launch_generator-0.5.0/src/launch_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1070 2024-02-17 01:55:57.000000 launch_generator-0.5.0/src/launch_generator/base_generator.py
--rw-r--r--   0 root         (0) root         (0)    12654 2024-02-17 01:55:57.000000 launch_generator-0.5.0/src/launch_generator/common_generator.py
--rw-r--r--   0 root         (0) root         (0)     4304 2024-02-17 01:55:57.000000 launch_generator-0.5.0/src/launch_generator/container_generator.py
--rw-r--r--   0 root         (0) root         (0)     4975 2024-02-17 01:55:57.000000 launch_generator-0.5.0/src/launch_generator/event_handler_generator.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-02-17 01:55:57.000000 launch_generator-0.5.0/src/launch_generator/generator.py
--rw-r--r--   0 root         (0) root         (0)     1711 2024-02-17 01:55:57.000000 launch_generator-0.5.0/src/launch_generator/group_generator.py
--rw-r--r--   0 root         (0) root         (0)     1630 2024-02-17 01:55:57.000000 launch_generator-0.5.0/src/launch_generator/timer_generator.py
--rw-r--r--   0 root         (0) root         (0)     5487 2024-02-17 01:55:57.000000 launch_generator-0.5.0/src/launch_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-17 01:56:04.125964 launch_generator-0.5.0/src/launch_generator.egg-info/
--rw-r--r--   0 root         (0) root         (0)      357 2024-02-17 01:56:04.000000 launch_generator-0.5.0/src/launch_generator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      632 2024-02-17 01:56:04.000000 launch_generator-0.5.0/src/launch_generator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-17 01:56:04.000000 launch_generator-0.5.0/src/launch_generator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-17 01:56:04.000000 launch_generator-0.5.0/src/launch_generator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-17 01:56:04.000000 launch_generator-0.5.0/src/launch_generator.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-17 01:56:04.125964 launch_generator-0.5.0/test/
--rw-r--r--   0 root         (0) root         (0)     3451 2024-02-17 01:55:57.000000 launch_generator-0.5.0/test/test_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:00:56.073166 launch_generator-0.5.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-27 14:00:49.000000 launch_generator-0.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      357 2024-05-27 14:00:56.073166 launch_generator-0.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10634 2024-05-27 14:00:49.000000 launch_generator-0.5.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      482 2024-05-27 14:00:49.000000 launch_generator-0.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 14:00:56.073166 launch_generator-0.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-05-27 14:00:49.000000 launch_generator-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:00:56.069166 launch_generator-0.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:00:56.073166 launch_generator-0.5.1/src/launch_generator/
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-05-27 14:00:49.000000 launch_generator-0.5.1/src/launch_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-27 14:00:49.000000 launch_generator-0.5.1/src/launch_generator/base_generator.py
+-rw-r--r--   0 root         (0) root         (0)    12660 2024-05-27 14:00:49.000000 launch_generator-0.5.1/src/launch_generator/common_generator.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2024-05-27 14:00:49.000000 launch_generator-0.5.1/src/launch_generator/container_generator.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2024-05-27 14:00:49.000000 launch_generator-0.5.1/src/launch_generator/event_handler_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-05-27 14:00:49.000000 launch_generator-0.5.1/src/launch_generator/generator.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2024-05-27 14:00:49.000000 launch_generator-0.5.1/src/launch_generator/group_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2024-05-27 14:00:49.000000 launch_generator-0.5.1/src/launch_generator/timer_generator.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2024-05-27 14:00:49.000000 launch_generator-0.5.1/src/launch_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:00:56.073166 launch_generator-0.5.1/src/launch_generator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      357 2024-05-27 14:00:56.000000 launch_generator-0.5.1/src/launch_generator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-27 14:00:56.000000 launch_generator-0.5.1/src/launch_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 14:00:56.000000 launch_generator-0.5.1/src/launch_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-27 14:00:56.000000 launch_generator-0.5.1/src/launch_generator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-27 14:00:56.000000 launch_generator-0.5.1/src/launch_generator.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 14:00:56.073166 launch_generator-0.5.1/test/
+-rw-r--r--   0 root         (0) root         (0)     3451 2024-05-27 14:00:49.000000 launch_generator-0.5.1/test/test_generator.py
```

### Comparing `launch_generator-0.5.0/LICENSE` & `launch_generator-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `launch_generator-0.5.0/README.md` & `launch_generator-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `launch_generator-0.5.0/setup.py` & `launch_generator-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 #
 
 import setuptools
 
 setuptools.setup(
     name='launch_generator',
-    version='0.5.0',
+    version='0.5.1',
     author='Tatsuro Sakaguchi',
     author_email='tatsuro.sakaguchi@g.softbank.co.jp',
     description='The package `launch-generator` is a tool to easily generate launch descriptions for ROS 2.',
     url='https://github.com/Tacha-S/launch_generator',
     package_dir={'': 'src'},
     packages=setuptools.find_packages('src', include=['launch_generator']),
     install_requires=['pyyaml'],
```

### Comparing `launch_generator-0.5.0/src/launch_generator/__init__.py` & `launch_generator-0.5.1/src/launch_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `launch_generator-0.5.0/src/launch_generator/base_generator.py` & `launch_generator-0.5.1/src/launch_generator/base_generator.py`

 * *Files identical despite different names*

### Comparing `launch_generator-0.5.0/src/launch_generator/common_generator.py` & `launch_generator-0.5.1/src/launch_generator/common_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 
 from launch_generator.base_generator import BaseGenerator
 from launch_generator.container_generator import ContainerGenerator
 
 
 class CommonGenerator(BaseGenerator):
     """Group generator."""
-    event_action_type = (launch.some_actions_type.SomeActionsType
+    event_action_type = (launch.some_entities_type.SomeEntitiesType
                          | typing.Callable[
                              [launch.events.process.ProcessExited, launch.launch_context.LaunchContext],
-                             launch.some_actions_type.SomeActionsType | None,
+                             launch.some_entities_type.SomeEntitiesType | None,
                          ]
                          | None)
     event_io_type = (typing.Callable[[launch.events.process.ProcessIO],
-                                     launch.some_actions_type.SomeActionsType | None] | None)
+                                     launch.some_entities_type.SomeEntitiesType | None] | None)
 
     def __init__(self) -> None:
         """Initialize.
 
         Args:
             namespace: Group namespace. Defaults to None.
         """
```

### Comparing `launch_generator-0.5.0/src/launch_generator/container_generator.py` & `launch_generator-0.5.1/src/launch_generator/container_generator.py`

 * *Files identical despite different names*

### Comparing `launch_generator-0.5.0/src/launch_generator/event_handler_generator.py` & `launch_generator-0.5.1/src/launch_generator/event_handler_generator.py`

 * *Files identical despite different names*

### Comparing `launch_generator-0.5.0/src/launch_generator/generator.py` & `launch_generator-0.5.1/src/launch_generator/generator.py`

 * *Files identical despite different names*

### Comparing `launch_generator-0.5.0/src/launch_generator/group_generator.py` & `launch_generator-0.5.1/src/launch_generator/group_generator.py`

 * *Files identical despite different names*

### Comparing `launch_generator-0.5.0/src/launch_generator/timer_generator.py` & `launch_generator-0.5.1/src/launch_generator/timer_generator.py`

 * *Files identical despite different names*

### Comparing `launch_generator-0.5.0/src/launch_generator/utils.py` & `launch_generator-0.5.1/src/launch_generator/utils.py`

 * *Files identical despite different names*

### Comparing `launch_generator-0.5.0/src/launch_generator.egg-info/SOURCES.txt` & `launch_generator-0.5.1/src/launch_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `launch_generator-0.5.0/test/test_generator.py` & `launch_generator-0.5.1/test/test_generator.py`

 * *Files identical despite different names*

