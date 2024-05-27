# Comparing `tmp/gdextension_cli-0.0.2b1.tar.gz` & `tmp/gdextension_cli-0.0.2b3.tar.gz`

## Comparing `gdextension_cli-0.0.2b1.tar` & `gdextension_cli-0.0.2b3.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/.pylintrc
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/requirements-publish.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/requirements.txt
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/.github/workflows/lint-and-test.yml
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/.idea/.gitignore
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/.idea/gdextension-cli.iml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/.idea/misc.xml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/.idea/vcs.xml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/src/main.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/src/gdextension_cli/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/src/gdextension_cli/__version__.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/src/gdextension_cli/command_line_args.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/src/gdextension_cli/template_renderer.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/src/gdextension_cli/commands/new_project_from_local.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/tests/test_command_line_arguments.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/README.md
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/pyproject.toml
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.pylintrc
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/requirements-publish.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/requirements.txt
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.github/workflows/lint-and-test.yml
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/.gitignore
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/gdextension-cli.iml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/misc.xml
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/vcs.xml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/main.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/gdextension_cli/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/gdextension_cli/__version__.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/gdextension_cli/command_line_args.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/gdextension_cli/template_renderer.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/gdextension_cli/commands/new_project_from_git.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/src/gdextension_cli/commands/new_project_from_local.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/tests/test_command_line_arguments.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/tests/test_template_renderer.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/LICENSE
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/README.md
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/pyproject.toml
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 gdextension_cli-0.0.2b3/PKG-INFO
```

### Comparing `gdextension_cli-0.0.2b1/.pylintrc` & `gdextension_cli-0.0.2b3/.pylintrc`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b1/.github/workflows/lint-and-test.yml` & `gdextension_cli-0.0.2b3/.github/workflows/lint-and-test.yml`

 * *Files 20% similar despite different names*

```diff
@@ -22,12 +22,10 @@
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
       - name: Analysing the code with pylint
-        run: |
-          pylint src/**/*.py tests/**/*.py
+        run: pylint src/**/*.py
       - name: Test with pytest
-        run: |
-          pytest
+        run: hatch test
```

### Comparing `gdextension_cli-0.0.2b1/.github/workflows/publish.yml` & `gdextension_cli-0.0.2b3/.github/workflows/publish.yml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 permissions:
   contents: read
 
 jobs:
   deploy:
 
-    environment: Production
+    environment: Release
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
 
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
@@ -30,15 +30,16 @@
           python -m pip install --upgrade pip
           if [ -f requirements-publish.txt ]; then pip install -r requirements-publish.txt; fi
 
       - name: Build package
         run: hatch build
 
       - name: Publish package to production
-        if: ${{ !startsWith(github.ref_name, 'release-') }}
+        if: ${{ startsWith(github.ref_name, 'release-') }}
         uses: pypa/gh-action-pypi-publish@release/v1
 
-      - name: Publish package to production
-        if: ${{ !startsWith(github.ref_name, 'test-release-') }}
+      - name: Publish package to testing
+        if: ${{ startsWith(github.ref_name, 'test-release-') }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
+          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
           repository-url: https://test.pypi.org/legacy/
```

### Comparing `gdextension_cli-0.0.2b1/.idea/gdextension-cli.iml` & `gdextension_cli-0.0.2b3/.idea/gdextension-cli.iml`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b1/.idea/inspectionProfiles/Project_Default.xml` & `gdextension_cli-0.0.2b3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b1/src/gdextension_cli/__init__.py` & `gdextension_cli-0.0.2b3/src/gdextension_cli/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 gdextension_cli entry point with callable function main_cli()
 """
 
 import logging
 
 from .command_line_args import CommandLineArgs
 from .commands.new_project_from_local import NewProjectFromLocalCommand
+from .commands.new_project_from_git import NewProjectFromGitCommand
 
 
 def main_cli():
     """gdextension-cli main entry point used in pyproject.toml"""
     command_line = CommandLineArgs()
     args = command_line.create().parse()
 
     initialize_logging(args.verbose if hasattr(args, "verbose") else logging.INFO)
 
     match args.subcommand:
         case "new":
             if args.from_local:
                 NewProjectFromLocalCommand.from_arguments(args).run()
             elif args.from_git:
-                print("from_git: not implemented")
+                NewProjectFromGitCommand.from_arguments(args).run()
             else:
                 raise AssertionError(
                     "Expected arguments '--from-local' or '--from-git'"
                 )
         case "build":
             print("BUILD")
         case _:
```

### Comparing `gdextension_cli-0.0.2b1/src/gdextension_cli/command_line_args.py` & `gdextension_cli-0.0.2b3/src/gdextension_cli/command_line_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,19 @@
     """
 
     HELP_OUTPUT_PATH = (
         "Output path of the project. "
         "Default: folder in current directory with name of the project"
     )
 
+    HELP_REPOSITORY_URL = (
+        "URL of a project template repository. "
+        "Default is https://github.com/3LK3/gdextension-template.git"
+    )
+
     def __init__(self):
         self._parser = argparse.ArgumentParser(prog="gdextension-cli")
         self._subcommands = self._parser.add_subparsers(dest="subcommand")
         self._parser.add_argument(
             "-v", "--version", action="version", version=__version__
         )
 
@@ -62,15 +67,15 @@
         from_group = new_parser.add_mutually_exclusive_group(required=False)
         from_group.add_argument(
             "--from-git",
             metavar="GIT_URL",
             type=str,
             required=False,
             default="https://github.com/3LK3/gdextension-template.git",
-            help="URL of a project template repository",
+            help=self.HELP_REPOSITORY_URL,
         )
         from_group.add_argument(
             "--from-local",
             metavar="PATH",
             type=pathlib.Path,
             required=False,
             help="Path to a local folder containing a project template",
```

### Comparing `gdextension_cli-0.0.2b1/src/gdextension_cli/template_renderer.py` & `gdextension_cli-0.0.2b3/src/gdextension_cli/template_renderer.py`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b1/src/gdextension_cli/commands/new_project_from_local.py` & `gdextension_cli-0.0.2b3/src/gdextension_cli/commands/new_project_from_local.py`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b1/.gitignore` & `gdextension_cli-0.0.2b3/.gitignore`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b1/LICENSE` & `gdextension_cli-0.0.2b3/LICENSE`

 * *Files identical despite different names*

### Comparing `gdextension_cli-0.0.2b1/pyproject.toml` & `gdextension_cli-0.0.2b3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     { name = "Sören Spindler", email = "soeren.s89@gmail.com" }
 ]
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "Jinja2==3.1.4"
+    "Jinja2==3.1.4",
+    "GitPython==3.1.43"
 ]
 dynamic = [
     "version"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/3LK3/gdextension-cli"
```

