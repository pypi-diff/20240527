# Comparing `tmp/cook_builder-0.1.4.tar.gz` & `tmp/cook_builder-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cook_builder-0.1.4.tar", last modified: Wed Apr 24 06:55:37 2024, max compression
+gzip compressed data, was "cook_builder-0.1.5.tar", last modified: Mon May 27 15:04:17 2024, max compression
```

## Comparing `cook_builder-0.1.4.tar` & `cook_builder-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-24 06:55:37.498247 cook_builder-0.1.4/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.1.4/LICENSE
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3040 2024-04-24 06:55:37.498247 cook_builder-0.1.4/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      877 2024-04-19 18:55:28.000000 cook_builder-0.1.4/README.md
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-24 06:55:37.498247 cook_builder-0.1.4/cook/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       36 2024-04-23 18:58:25.000000 cook_builder-0.1.4/cook/__init__.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1204 2024-04-20 08:24:26.000000 cook_builder-0.1.4/cook/build.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3023 2024-04-23 18:57:39.000000 cook_builder-0.1.4/cook/cli.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     4851 2024-04-20 08:51:37.000000 cook_builder-0.1.4/cook/configuration.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3050 2024-04-22 20:22:09.000000 cook_builder-0.1.4/cook/cook.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      150 2024-04-16 14:39:30.000000 cook_builder-0.1.4/cook/exception.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2417 2024-04-24 06:54:24.000000 cook_builder-0.1.4/cook/executors.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      985 2024-04-23 18:19:22.000000 cook_builder-0.1.4/cook/logger.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2170 2024-04-23 18:36:05.000000 cook_builder-0.1.4/cook/main.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1030 2024-04-22 19:33:15.000000 cook_builder-0.1.4/cook/recipe.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2310 2024-04-22 20:00:03.000000 cook_builder-0.1.4/cook/rsync.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1383 2024-04-20 08:25:29.000000 cook_builder-0.1.4/cook/sync.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      381 2024-04-20 09:09:37.000000 cook_builder-0.1.4/cook/watchers.py
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-24 06:55:37.498247 cook_builder-0.1.4/cook_builder.egg-info/
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3040 2024-04-24 06:55:37.000000 cook_builder-0.1.4/cook_builder.egg-info/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      451 2024-04-24 06:55:37.000000 cook_builder-0.1.4/cook_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-04-24 06:55:37.000000 cook_builder-0.1.4/cook_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-24 06:55:37.000000 cook_builder-0.1.4/cook_builder.egg-info/entry_points.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       46 2024-04-24 06:55:37.000000 cook_builder-0.1.4/cook_builder.egg-info/requires.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-04-24 06:55:37.000000 cook_builder-0.1.4/cook_builder.egg-info/top_level.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1165 2024-04-24 06:55:11.000000 cook_builder-0.1.4/pyproject.toml
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-24 06:55:37.498247 cook_builder-0.1.4/setup.cfg
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-05-27 15:04:17.759513 cook_builder-0.1.5/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.1.5/LICENSE
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3083 2024-05-27 15:04:17.759513 cook_builder-0.1.5/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      920 2024-05-27 15:04:12.000000 cook_builder-0.1.5/README.md
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-05-27 15:04:17.759513 cook_builder-0.1.5/cook/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       36 2024-04-23 18:58:25.000000 cook_builder-0.1.5/cook/__init__.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1204 2024-04-20 08:24:26.000000 cook_builder-0.1.5/cook/build.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3870 2024-05-24 17:06:46.000000 cook_builder-0.1.5/cook/cli.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     4851 2024-04-20 08:51:37.000000 cook_builder-0.1.5/cook/configuration.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2915 2024-05-24 16:57:07.000000 cook_builder-0.1.5/cook/cook.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      150 2024-04-16 14:39:30.000000 cook_builder-0.1.5/cook/exception.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2390 2024-05-24 16:59:53.000000 cook_builder-0.1.5/cook/executors.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      981 2024-05-24 16:59:49.000000 cook_builder-0.1.5/cook/logger.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2455 2024-05-24 16:50:34.000000 cook_builder-0.1.5/cook/main.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1065 2024-05-24 16:30:49.000000 cook_builder-0.1.5/cook/recipe.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2310 2024-04-22 20:00:03.000000 cook_builder-0.1.5/cook/rsync.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1383 2024-04-20 08:25:29.000000 cook_builder-0.1.5/cook/sync.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      381 2024-04-20 09:09:37.000000 cook_builder-0.1.5/cook/watchers.py
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-05-27 15:04:17.759513 cook_builder-0.1.5/cook_builder.egg-info/
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3083 2024-05-27 15:04:17.000000 cook_builder-0.1.5/cook_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      451 2024-05-27 15:04:17.000000 cook_builder-0.1.5/cook_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-05-27 15:04:17.000000 cook_builder-0.1.5/cook_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-05-27 15:04:17.000000 cook_builder-0.1.5/cook_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       46 2024-05-27 15:04:17.000000 cook_builder-0.1.5/cook_builder.egg-info/requires.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-05-27 15:04:17.000000 cook_builder-0.1.5/cook_builder.egg-info/top_level.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1165 2024-05-27 15:02:54.000000 cook_builder-0.1.5/pyproject.toml
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-05-27 15:04:17.759513 cook_builder-0.1.5/setup.cfg
```

### Comparing `cook_builder-0.1.4/LICENSE` & `cook_builder-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.4/PKG-INFO` & `cook_builder-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.1.4
+Version: 0.1.5
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -78,12 +78,13 @@
 cd cook
 pip install -e .
 ```
 
 <!-- RELEASING
 1. Update version in pyproject.toml
 2. Build and upload wheels to PyPI:
+    python3 -m pip install --upgrade build
     python3 -m build
     twine upload dist/*
 -->
 
 <!-- TODO: add tests -->
```

### Comparing `cook_builder-0.1.4/README.md` & `cook_builder-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,12 +32,13 @@
 cd cook
 pip install -e .
 ```
 
 <!-- RELEASING
 1. Update version in pyproject.toml
 2. Build and upload wheels to PyPI:
+    python3 -m pip install --upgrade build
     python3 -m build
     twine upload dist/*
 -->
 
 <!-- TODO: add tests -->
```

### Comparing `cook_builder-0.1.4/cook/build.py` & `cook_builder-0.1.5/cook/build.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.4/cook/configuration.py` & `cook_builder-0.1.5/cook/configuration.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.4/cook/cook.py` & `cook_builder-0.1.5/cook/cook.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,16 +30,15 @@
         else:
             raise RuntimeError(f'Unknown build type: {build_type}')
 
     def _local_build(self):
         build_steps = self.configuration.get_build_steps()
 
         if build_steps:
-            self.logger.print('local', 'Running local build')
-            executor = LocalExecutor('local', self.logger)
+            executor = LocalExecutor('log', self.logger)
             executor.set_dry_run(self.dry_run)
             executor.run_multiple(build_steps)
 
     def _remote_build(self):
         build_steps = self.configuration.get_build_steps()
         local_base, remote_base = self.configuration.get_base_paths()
         files_to_send = self.configuration.get_files_to_send()
@@ -47,37 +46,36 @@
 
         setup_rsync = files_to_send or files_to_receive
         if setup_rsync:
             rsync = Rsync(self.build_server, local_base, remote_base, self.logger)
             rsync.set_dry_run(self.dry_run)
 
         if files_to_send:
-            self.logger.print('remote', 'Sending Files')
+            self.logger.print('log', 'Sending Files')
             rsync.send(files_to_send)
 
         if build_steps:
-            self.logger.print('remote', 'Running Remote Build')
             executor = RemoteExecutor(self.build_server, self.logger)
             executor.set_dry_run(self.dry_run)
             executor.run_multiple(build_steps)
 
         if files_to_receive:
-            self.logger.print('remote', 'Receiving Files')
+            self.logger.print('log', 'Receiving Files')
             rsync.receive(files_to_receive)
 
     def _composite_build(self):
         components = self.configuration.get_components()
 
         if not components:  # TODO required?
             return
 
-        self.logger.print('local', 'Executing Components')
+        self.logger.print('log', 'Running Composite Build')
 
         for component in components:
-            self.logger.print('local', f'Component: {component}')
+            self.logger.print('log', f'Component: {component}')
             self._run_component(component)
 
     def _run_component(self, component):
         try:
             sub_configuration = Configuration(self.recipe)
             sub_configuration.setup(component, self.build_server)
```

### Comparing `cook_builder-0.1.4/cook/executors.py` & `cook_builder-0.1.5/cook/executors.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,23 +57,23 @@
 
 
 class LocalExecutor(Executor):
     def run_multiple(self, steps):
         context = invoke.context.Context()
         for step in steps:
             if self.logger:
-                self.logger.print('local', f'Local Workdir/Command: {step.workdir}: {step.command}')
+                self.logger.print('log', f'Local Step: {step.workdir}: {step.command}')
 
             self.run(context, step)
 
 
 class RemoteExecutor(Executor):
     def _execute_step(self, context, step):
         if self.logger:
-            self.logger.print('remote', f'Remote Workdir/Command: {self.name}:{step.workdir}: {step.command}')
+            self.logger.print('log', f'Remote Step: {self.name}:{step.workdir}: {step.command}')
 
         try:
             self.run(context, step)
         except gaierror as e:
             raise ExecutorError(e.strerror, self.name, e.errno)
 
     def run_multiple(self, steps):
```

### Comparing `cook_builder-0.1.4/cook/logger.py` & `cook_builder-0.1.5/cook/logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 class Logger:
     GREEN = '#00cc52'
     PURPLE = '#d849ff'
 
     def __init__(self, rich_output, quiet):
         cook_console_theme = Theme(
             {
-                'local': Logger.GREEN,
-                'remote': Logger.PURPLE,
+                'log': Logger.GREEN,
+                'info': Logger.PURPLE,
                 'warning': 'dark_orange',
                 'error': 'red',
             }
         )
         self.console = Console(theme=cook_console_theme)
         self.rich_output = rich_output
         self.quiet = quiet
```

### Comparing `cook_builder-0.1.4/cook/main.py` & `cook_builder-0.1.5/cook/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         return (self.recipe.base_path / "recipe.py").as_posix()
 
     def get_projects(self):
         projects = list(self.recipe.projects.keys())
         default_project = self.recipe.default_project
         return projects, default_project
 
+    def get_build_servers(self):
+        return self.recipe.build_servers, self.recipe.default_build_server
+
     def configure(self, project, build_server):
         self.project = project
         self.build_server = build_server
 
     def set_output(self, rich=False, quiet=False):
         self.rich_output = rich
         self.quiet = quiet
@@ -63,7 +66,12 @@
         except ProcessError as e:
             self.logger.print('error', e)
             exit(e.return_code)
 
         except ExecutorError as e:
             self.logger.print('error', f'{e.name}: {e}')
             exit(e.return_code)
+
+        self.logger.print('info', f'Finished running {self.project} on {self.build_server}')
+
+        if dry_run:
+            self.logger.print('warning', 'Dry run finished')
```

### Comparing `cook_builder-0.1.4/cook/recipe.py` & `cook_builder-0.1.5/cook/recipe.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     pass
 
 
 class Recipe:
     default_project: str
     default_build_server: str
     projects: dict[dict[Any]]
+    build_servers: list[str]
 
     def __init__(self, base_path: Path):
         self.base_path = base_path
 
     def load(self):
         recipes = list(self.base_path.glob('recipe.py'))
 
@@ -35,9 +36,10 @@
         self.update(vars(recipe))
 
     def update(self, settings):
         for key in self.__annotations__.keys():
             try:
                 value = settings[key]
             except KeyError:
-                raise RecipeError(f'{key} entry not found in recipe.')
+                # TODO: add separate validation
+                value = None
             setattr(self, key, value)
```

### Comparing `cook_builder-0.1.4/cook/rsync.py` & `cook_builder-0.1.5/cook/rsync.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.4/cook/sync.py` & `cook_builder-0.1.5/cook/sync.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.4/cook_builder.egg-info/PKG-INFO` & `cook_builder-0.1.5/cook_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.1.4
+Version: 0.1.5
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -78,12 +78,13 @@
 cd cook
 pip install -e .
 ```
 
 <!-- RELEASING
 1. Update version in pyproject.toml
 2. Build and upload wheels to PyPI:
+    python3 -m pip install --upgrade build
     python3 -m build
     twine upload dist/*
 -->
 
 <!-- TODO: add tests -->
```

### Comparing `cook_builder-0.1.4/pyproject.toml` & `cook_builder-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cook_builder"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
   "fabric==3.2.2",
   "rich==13.7.1",
   "questionary==2.0.1",
 ]
 requires-python = ">=3.10"
 authors = [
```

