# Comparing `tmp/makepyz-0.0.1b25.tar.gz` & `tmp/makepyz-0.0.1b28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makepyz-0.0.1b25.tar", last modified: Mon May 27 00:39:25 2024, max compression
+gzip compressed data, was "makepyz-0.0.1b28.tar", last modified: Mon May 27 01:02:35 2024, max compression
```

## Comparing `makepyz-0.0.1b25.tar` & `makepyz-0.0.1b28.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:25.029845 makepyz-0.0.1b25/
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-27 00:39:25.029845 makepyz-0.0.1b25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-27 00:39:22.000000 makepyz-0.0.1b25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 00:39:25.029845 makepyz-0.0.1b25/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:25.021845 makepyz-0.0.1b25/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:25.025845 makepyz-0.0.1b25/src/makepyz/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 00:39:22.000000 makepyz-0.0.1b25/src/makepyz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/fileops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/scm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:25.025845 makepyz-0.0.1b25/src/makepyz/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/scripts/makepyzui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/tasks_gh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/src/makepyz/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:25.029845 makepyz-0.0.1b25/src/makepyz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-27 00:39:25.000000 makepyz-0.0.1b25/src/makepyz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-27 00:39:25.000000 makepyz-0.0.1b25/src/makepyz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 00:39:25.000000 makepyz-0.0.1b25/src/makepyz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-27 00:39:25.000000 makepyz-0.0.1b25/src/makepyz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 00:39:25.000000 makepyz-0.0.1b25/src/makepyz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 00:39:25.000000 makepyz-0.0.1b25/src/makepyz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:39:25.029845 makepyz-0.0.1b25/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_fileops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_makepyx.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-27 00:39:00.000000 makepyz-0.0.1b25/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:02:35.064021 makepyz-0.0.1b28/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-27 01:02:35.064021 makepyz-0.0.1b28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-27 01:02:32.000000 makepyz-0.0.1b28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 01:02:35.064021 makepyz-0.0.1b28/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:02:35.056021 makepyz-0.0.1b28/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:02:35.060021 makepyz-0.0.1b28/src/makepyz/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 01:02:32.000000 makepyz-0.0.1b28/src/makepyz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/scm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:02:35.060021 makepyz-0.0.1b28/src/makepyz/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/scripts/makepyzui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/tasks_gh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/src/makepyz/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:02:35.064021 makepyz-0.0.1b28/src/makepyz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-27 01:02:35.000000 makepyz-0.0.1b28/src/makepyz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-27 01:02:35.000000 makepyz-0.0.1b28/src/makepyz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 01:02:35.000000 makepyz-0.0.1b28/src/makepyz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-27 01:02:35.000000 makepyz-0.0.1b28/src/makepyz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-27 01:02:35.000000 makepyz-0.0.1b28/src/makepyz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 01:02:35.000000 makepyz-0.0.1b28/src/makepyz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 01:02:35.064021 makepyz-0.0.1b28/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/tests/test_fileops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/tests/test_makepyx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-27 01:02:13.000000 makepyz-0.0.1b28/tests/test_tree.py
```

### Comparing `makepyz-0.0.1b25/PKG-INFO` & `makepyz-0.0.1b28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makepyz
-Version: 0.0.1b25
+Version: 0.0.1b28
 Summary: a new kind of make tool
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 Project-URL: Issues, https://github.com/cav71/makepyz/issues
 Project-URL: Source, https://github.com/cav71/makepyz
 Keywords: git,scm,version
 Classifier: Development Status :: 4 - Beta
```

### Comparing `makepyz-0.0.1b25/README.md` & `makepyz-0.0.1b28/README.md`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/pyproject.toml` & `makepyz-0.0.1b28/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "makepyz"
-version = "0.0.1b25"
+version = "0.0.1b28"
 description = "a new kind of make tool"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">= 3.8"
 keywords = [
   "git",
   "scm",
```

### Comparing `makepyz-0.0.1b25/src/makepyz/cli.py` & `makepyz-0.0.1b28/src/makepyz/cli.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/src/makepyz/exceptions.py` & `makepyz-0.0.1b28/src/makepyz/exceptions.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/src/makepyz/fileops.py` & `makepyz-0.0.1b28/src/makepyz/fileops.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/src/makepyz/github.py` & `makepyz-0.0.1b28/src/makepyz/github.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/src/makepyz/misc.py` & `makepyz-0.0.1b28/src/makepyz/misc.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/src/makepyz/packaging.py` & `makepyz-0.0.1b28/src/makepyz/packaging.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/src/makepyz/scm.py` & `makepyz-0.0.1b28/src/makepyz/scm.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/src/makepyz/scripts/makepyzui.py` & `makepyz-0.0.1b28/src/makepyz/scripts/makepyzui.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/src/makepyz/tasks.py` & `makepyz-0.0.1b28/src/makepyz/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,26 @@
                 params = inspect.signature(function).parameters
                 if "workdir" in params:
                     kwargs["workdir"] = oldcd
                 return function(*args, **kwargs)
             finally:
                 os.chdir(oldcd)
 
-        _fn1.task = name or function.__name__  # type: ignore
+        _fn1.task = (  # type: ignore
+            name or (function.func if hasattr(function, "func") else function).__name__
+        )
         return _fn1
 
     return _fn
 
 
+def add_task(function, **kwargs):
+    return task()(functools.partial(function, **kwargs))
+
+
 def info(arguments: list[str], mod: types.ModuleType | None = None):
     """this is the hello world"""
     from makepyz import api
 
     print(  # noqa: T201
         f"""
 Hi!
@@ -59,15 +65,15 @@
     names = [f"[{i}]" for i in range(len(arguments))]
     width = max(len(n) for n in names)
     head = f"  {{name:{width + 1}}}{{sep}} '{{value}}'"
     for name, argument in zip(names, arguments) or []:  # type: ignore
         print(head.format(name=name, value=argument, sep=":"))
 
 
-def tests(arguments: list[str], mod: types.ModuleType):
+def tests(arguments: list[str], mod: types.ModuleType, package: str = "makepyz"):
     """run all tests"""
 
     # def parse_arguments(arguments: list[str]):
     #     parser = argparse.ArgumentParser()
     #     parser.add_argument("--json", action="store_true")
     #     return parser.parse_args(arguments)
     #
@@ -79,15 +85,15 @@
     env = os.environ.copy()
     env["PYTHONPATH"] = str(Path.cwd() / "src")
     fileops.check_call(
         [
             "pytest",
             "-vvs",
             "--cov",
-            "makepyz",
+            package,
             "--cov-report",
             f"html:{builddir / 'coverage'}",
             "--cov-report",
             f"json:{builddir / 'coverage.json'}",
             str(workdir / "tests"),
         ],
         env=env,
```

### Comparing `makepyz-0.0.1b25/src/makepyz/tasks_gh.py` & `makepyz-0.0.1b28/src/makepyz/tasks_gh.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     if old != "" and old != gdata["sha"]:
         raise RuntimeError(f"found in {initfile} __hash__ {old} != {gdata['sha']}")
     misc.set_variable_def(initfile, "__hash__", lineno, gdata["sha"], quote)
 
     return initfile
 
 
-def build(arguments: list[str]):
+def build(arguments: list[str], package: str = "makepyz"):
     """create beta and release packages for makepyz (only in github)"""
     from . import cli, fileops, github
 
     global DRYRUN
 
     def parse_arguments(arguments: list[str]):
         parser = argparse.ArgumentParser()
@@ -75,11 +75,11 @@
     with contextlib.ExitStack() as stack:
         save = stack.enter_context(fileops.backups())
 
         # pyproject.toml
         _, version, current = process_pyproject(save("pyproject.toml"), gdata, release)
 
         # __init__.py
-        _ = process_init(save("src/makepyz/__init__.py"), gdata, version, current)
+        _ = process_init(save(f"src/{package}/__init__.py"), gdata, version, current)
 
         if not options.dryrun:
             subprocess.check_call([sys.executable, "-m", "build"])  # noqa: S603
```

### Comparing `makepyz-0.0.1b25/src/makepyz/text.py` & `makepyz-0.0.1b28/src/makepyz/text.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/src/makepyz/tree.py` & `makepyz-0.0.1b28/src/makepyz/tree.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/src/makepyz.egg-info/PKG-INFO` & `makepyz-0.0.1b28/src/makepyz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makepyz
-Version: 0.0.1b25
+Version: 0.0.1b28
 Summary: a new kind of make tool
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 Project-URL: Issues, https://github.com/cav71/makepyz/issues
 Project-URL: Source, https://github.com/cav71/makepyz
 Keywords: git,scm,version
 Classifier: Development Status :: 4 - Beta
```

### Comparing `makepyz-0.0.1b25/src/makepyz.egg-info/SOURCES.txt` & `makepyz-0.0.1b28/src/makepyz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/tests/test_cli.py` & `makepyz-0.0.1b28/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/tests/test_fileops.py` & `makepyz-0.0.1b28/tests/test_fileops.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/tests/test_github.py` & `makepyz-0.0.1b28/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/tests/test_packaging.py` & `makepyz-0.0.1b28/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/tests/test_scm.py` & `makepyz-0.0.1b28/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/tests/test_text.py` & `makepyz-0.0.1b28/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b25/tests/test_tree.py` & `makepyz-0.0.1b28/tests/test_tree.py`

 * *Files identical despite different names*

