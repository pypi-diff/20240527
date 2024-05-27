# Comparing `tmp/req-update-2.5.1.tar.gz` & `tmp/req_update-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "req-update-2.5.1.tar", last modified: Tue Feb 20 09:32:21 2024, max compression
+gzip compressed data, was "req_update-2.6.0.tar", last modified: Mon May 27 00:43:25 2024, max compression
```

## Comparing `req-update-2.5.1.tar` & `req_update-2.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:32:21.540825 req-update-2.5.1/
--rw-r--r--   0 root         (0) root         (0)     6114 2024-02-20 09:31:16.000000 req-update-2.5.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1068 2024-02-20 09:31:16.000000 req-update-2.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2024-02-20 09:31:16.000000 req-update-2.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3427 2024-02-20 09:32:21.536825 req-update-2.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2291 2024-02-20 09:31:16.000000 req-update-2.5.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1742 2024-02-20 09:31:16.000000 req-update-2.5.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:32:21.536825 req-update-2.5.1/req_update/
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 09:31:16.000000 req-update-2.5.1/req_update/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4442 2024-02-20 09:31:16.000000 req-update-2.5.1/req_update/docker.py
--rw-r--r--   0 root         (0) root         (0)      154 2024-02-20 09:31:16.000000 req-update-2.5.1/req_update/drone.py
--rw-r--r--   0 root         (0) root         (0)     5340 2024-02-20 09:31:16.000000 req-update-2.5.1/req_update/gitsubmodule.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-02-20 09:31:16.000000 req-update-2.5.1/req_update/go.py
--rw-r--r--   0 root         (0) root         (0)     5953 2024-02-20 09:31:16.000000 req-update-2.5.1/req_update/node.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 09:31:16.000000 req-update-2.5.1/req_update/py.typed
--rw-r--r--   0 root         (0) root         (0)     8578 2024-02-20 09:31:16.000000 req-update-2.5.1/req_update/python.py
--rwxr-xr-x   0 root         (0) root         (0)     3860 2024-02-20 09:31:16.000000 req-update-2.5.1/req_update/req_update.py
--rw-r--r--   0 root         (0) root         (0)     7536 2024-02-20 09:31:16.000000 req-update-2.5.1/req_update/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:32:21.536825 req-update-2.5.1/req_update.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3427 2024-02-20 09:32:21.000000 req-update-2.5.1/req_update.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      475 2024-02-20 09:32:21.000000 req-update-2.5.1/req_update.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 09:32:21.000000 req-update-2.5.1/req_update.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-02-20 09:32:21.000000 req-update-2.5.1/req_update.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-02-20 09:32:21.000000 req-update-2.5.1/req_update.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-02-20 09:32:21.000000 req-update-2.5.1/req_update.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-20 09:32:21.540825 req-update-2.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 00:43:25.524181 req_update-2.6.0/
+-rw-r--r--   0 root         (0) root         (0)     6337 2024-05-27 00:41:46.000000 req_update-2.6.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-05-27 00:41:46.000000 req_update-2.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-27 00:41:46.000000 req_update-2.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3428 2024-05-27 00:43:25.520181 req_update-2.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-05-27 00:41:46.000000 req_update-2.6.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-05-27 00:41:46.000000 req_update-2.6.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 00:43:25.520181 req_update-2.6.0/req_update/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4359 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/docker.py
+-rw-r--r--   0 root         (0) root         (0)      154 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/drone.py
+-rw-r--r--   0 root         (0) root         (0)     5343 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/gitsubmodule.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/go.py
+-rw-r--r--   0 root         (0) root         (0)     5800 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/node.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/py.typed
+-rw-r--r--   0 root         (0) root         (0)     8506 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/python.py
+-rwxr-xr-x   0 root         (0) root         (0)     4362 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/req_update.py
+-rw-r--r--   0 root         (0) root         (0)     7610 2024-05-27 00:41:46.000000 req_update-2.6.0/req_update/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 00:43:25.520181 req_update-2.6.0/req_update.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3428 2024-05-27 00:43:25.000000 req_update-2.6.0/req_update.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      475 2024-05-27 00:43:25.000000 req_update-2.6.0/req_update.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 00:43:25.000000 req_update-2.6.0/req_update.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-27 00:43:25.000000 req_update-2.6.0/req_update.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-27 00:43:25.000000 req_update-2.6.0/req_update.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-27 00:43:25.000000 req_update-2.6.0/req_update.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 00:43:25.524181 req_update-2.6.0/setup.cfg
```

### Comparing `req-update-2.5.1/CHANGELOG.md` & `req_update-2.6.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGELOG
 =========
 
+2.6.0 (2024-05-26)
+------------------
+
+ - Change check_repository_cleanliness to return a bool rather than raise an exception
+ - Add a ignore-cleanliness CLI flag
+ - Fix update warnings in dry-mode
+ - Update dependencies
+
+
 2.5.1 (2024-02-20)
 ------------------
 
  - Fix docker writing updates to the wrong path
  - Fix erroring out on docker hub errors
  - Update and clean up dependencies
```

### Comparing `req-update-2.5.1/LICENSE` & `req_update-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `req-update-2.5.1/PKG-INFO` & `req_update-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: req-update
-Version: 2.5.1
+Version: 2.6.0
 Summary: Update python, node, go, docker, and other dependencies
 Author-email: Albert Wang <git@albertyw.com>
 License: MIT
 Project-URL: Homepage, https://github.com/albertyw/req-update
 Keywords: dependencies
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,17 +19,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: test
-Requires-Dist: coverage==7.4.1; extra == "test"
-Requires-Dist: ruff==0.2.2; extra == "test"
-Requires-Dist: mypy==1.8.0; extra == "test"
+Requires-Dist: coverage==7.5.2; extra == "test"
+Requires-Dist: ruff==0.4.5; extra == "test"
+Requires-Dist: mypy==1.10.0; extra == "test"
 
 # req-update
 
 [![PyPI](https://img.shields.io/pypi/v/req-update)](https://pypi.org/project/req-update/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/req-update)
 ![PyPI - License](https://img.shields.io/pypi/l/req-update)
```

### Comparing `req-update-2.5.1/README.md` & `req_update-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `req-update-2.5.1/pyproject.toml` & `req_update-2.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 ]
 dependencies = []
 dynamic = ["version", "readme"]
 
 [project.optional-dependencies]
 test = [
     # Testing
-    "coverage==7.4.1",                  # Test coverage
-    "ruff==0.2.2",                      # Python linter
+    "coverage==7.5.2",                  # Test coverage
+    "ruff==0.4.5",                      # Python linter
 
     # Types
-    "mypy==1.8.0",                      # Static typing
+    "mypy==1.10.0",                     # Static typing
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/albertyw/req-update"
 
 [project.scripts]
 req_update = "req_update.req_update:main"
@@ -45,15 +45,15 @@
 version = {attr = "req_update.req_update.__version__"}
 readme = {file = "README.md", content-type="text/markdown"}
 
 [options.package_data]
 req_update = ["py.typed"]
 
 [tool.ruff]
-lint.select = ["E", "F", "B"]
+lint.select = ["E", "F", "W", "A", "B", "COM", "N", "PLC", "PLE", "PLW"]
 lint.ignore = ["B010"]
 
 [tool.mypy]
 strict = true
 exclude = [
     "build",
 ]
@@ -65,9 +65,8 @@
 omit = [
     ".virtualenv",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
-    'if __name__ == "__main__":',
 ]
```

### Comparing `req-update-2.5.1/req_update/docker.py` & `req_update-2.6.0/req_update/docker.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,14 @@
             line = dockerfile_lines[i]
             new_line, dependency, version = self.attempt_update_image(line)
             if not dependency or not version:
                 continue
             updates = True
             dockerfile_lines[i] = new_line
             self.commit_dockerfile(update_file, dockerfile_lines, dependency, version)
-        if not updates:
-            self.util.warn('No %s updates' % self.language)
         return updates
 
     def read_update_file(self, update_file: Path) -> list[str]:
         with open(update_file, 'r') as handle:
             lines = handle.readlines()
         lines = [line.strip('\n') for line in lines]
         return lines
@@ -109,13 +107,13 @@
         else:
             return new_version
 
     def commit_dockerfile(self,
         update_file: Path,
         dockerfile: list[str],
         dependency: str,
-        version: str
+        version: str,
     ) -> None:
         if not self.util.dry_run:
             with open(update_file, 'w') as handle:
                 handle.write('\n'.join(dockerfile))
         self.util.commit_dependency_update(self.language, dependency, version)
```

### Comparing `req-update-2.5.1/req_update/gitsubmodule.py` & `req_update-2.6.0/req_update/gitsubmodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,22 @@
         return len(result.stdout) > 0
 
     def update_dependencies(self) -> bool:
         submodules = self.get_submodule_info()
         clean = True
         for submodule in submodules:
             self.util.log('Checking dependency: %s' % submodule.path)
-            submodule = self.annotate_submodule(submodule)
-            version = self.update_submodule(submodule)
+            annotated_submodule = self.annotate_submodule(submodule)
+            version = self.update_submodule(annotated_submodule)
             if version:
-                try:
-                    # Not easy to tell if a git submodule has changed
-                    self.util.check_repository_cleanliness()
-                except RuntimeError:
+                # Not easy to tell if a git submodule has changed
+                clean = self.util.check_repository_cleanliness()
+                if not clean:
                     self.util.commit_dependency_update(
-                        self.language, str(submodule.path), version
+                        self.language, str(annotated_submodule.path), version,
                     )
                     clean = False
         return not clean
 
     # TODO: Make this a method on Submodule
     def get_submodule_info(self) -> List[Submodule]:
         command = ['git', 'submodule']
```

### Comparing `req-update-2.5.1/req_update/go.py` & `req_update-2.6.0/req_update/go.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,11 @@
         """
         command = ['go', 'get', '-u', 'all']
         self.util.log('Updating go packages')
         self.util.execute_shell(command, False)
         command = ['go', 'mod', 'tidy']
         self.util.log('Tidying go packages')
         self.util.execute_shell(command, False)
-        try:
-            self.util.check_repository_cleanliness()
-            self.util.warn('No %s updates' % self.language)
-            return False  # repository is clean so nothing to commit or push
-        except RuntimeError:
+        clean = self.util.check_repository_cleanliness()
+        if not clean:
             self.util.commit_git('Update go packages')
-            return True
+        return not clean
```

### Comparing `req-update-2.5.1/req_update/node.py` & `req_update-2.6.0/req_update/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,28 +31,25 @@
         """
         Update dependencies
         Return if updates were made
         """
         updated_unpinned = self.update_unpinned_dependencies()
         updated_pinned = self.update_pinned_dependencies()
         updated = updated_unpinned or updated_pinned
-        if not updated:
-            self.util.warn('No %s updates' % self.language)
         return updated
 
     def update_unpinned_dependencies(self) -> bool:
         command = ['npm', 'update']
         self.util.log('Updating npm packages')
         self.util.execute_shell(command, False)
-        try:
-            self.util.check_repository_cleanliness()
-            return False  # repository is clean so nothing to commit or push
-        except RuntimeError:
+        clean = self.util.check_repository_cleanliness()
+        if not clean:
             self.util.commit_git('Update npm packages')
             return True
+        return False
 
     def update_pinned_dependencies(self) -> bool:
         packages = self.get_outdated()
         if not packages:
             return False
         any_updated = False
         for package_name, package in packages.items():
@@ -66,15 +63,15 @@
         result = self.util.execute_shell(command, True, ignore_exit_code=True)
         packages = json.loads(result.stdout)
         if TYPE_CHECKING:
             return cast(dict[str, dict[str, str]], packages)
         return packages
 
     def update_package(
-        self, package_name: str, package: dict[str, str]
+        self, package_name: str, package: dict[str, str],
     ) -> bool:
         self.util.log('Updating dependency: %s' % package_name)
         with open('package.json', 'r') as handle:
             package_json_string = handle.read()
         package_json = json.loads(package_json_string)
         if package_name in package_json.get('dependencies', {}):
             old_version = package_json['dependencies'][package_name]
@@ -98,20 +95,20 @@
         package_json_string += '\n'  # Add the traditional EOF newline
         if not self.util.dry_run:
             with open('package.json', 'w') as handle:
                 handle.write(package_json_string)
         success = self.install_dependencies()
         if not success:
             self.util.warn(
-                'Dependency conflict; rolling back: %s' % package_name
+                'Dependency conflict; rolling back: %s' % package_name,
             )
             self.util.reset_changes()
             return False
         self.util.check_major_version_update(
-            package_name, old_version, new_version
+            package_name, old_version, new_version,
         )
         self.util.commit_dependency_update(self.language, package_name, new_version)
         return True
 
     def update_package_dependencies(
         self,
         dependencies: dict[str, str],
```

### Comparing `req-update-2.5.1/req_update/python.py` & `req_update-2.6.0/req_update/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         super().__init__(util)
 
     def check_applicable(self) -> bool:
         # Make sure pip is recent enough
         command = ['pip', '--version']
         try:
             result = self.util.execute_shell(
-                command, True, suppress_output=True
+                command, True, suppress_output=True,
             )
         except (subprocess.CalledProcessError, FileNotFoundError):
             # Cannot find pip
             return False
         try:
             pip_version = result.stdout.split(' ')
             pip_major_version = int(pip_version[1].split('.')[0])
@@ -74,16 +74,14 @@
         """
         Update dependencies
         Return if updates were made.
         """
         updates_made = self.update_dependencies_file()
         if updates_made:
             self.install_updates()
-        else:
-            self.util.warn('No %s updates' % self.language)
         return updates_made
 
     def update_dependencies_file(self) -> bool:
         """
         Update and commit a list of dependency updates.
         Return if updates were made.
         """
@@ -187,15 +185,15 @@
                 new_line = line_regex.sub(
                     r'"\g<1>\g<2>%s"%s' % (version, spacer),
                     line,
                 )
             if line == new_line:
                 continue
             self.util.check_major_version_update(
-                dependency, old_version, version
+                dependency, old_version, version,
             )
             lines[i] = new_line
             return True
         return False
 
     def install_updates(self) -> None:
         """Install requirements updates"""
```

### Comparing `req-update-2.5.1/req_update/req_update.py` & `req_update-2.6.0/req_update/req_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from req_update.gitsubmodule import GitSubmodule  # NOQA
 from req_update.go import Go  # NOQA
 from req_update.node import Node  # NOQA
 from req_update.python import Python  # NOQA
 from req_update.util import Updater, Util  # NOQA
 
 
-VERSION = (2, 5, 1)
+VERSION = (2, 6, 0)
 __version__ = '.'.join(map(str, VERSION))
 
 
 DESCRIPTION = (
     'Update python, go, node, and git submodule dependencies for your '
     'project with git integration\n\n'
     'https://github.com/albertyw/req-update'
@@ -56,32 +56,37 @@
     def main(self) -> bool:
         """
         Update all dependencies
         Return if updates were made
         """
         self.get_args()
         branch_created = False
-        self.util.check_repository_cleanliness()
+        if not self.util.ignore_cleanliness:
+            clean = self.util.check_repository_cleanliness()
+            if not clean:
+                raise RuntimeError('Repository is not clean')
         updates_made = False
         for updater in self.updaters:
             if self.language:
-                if self.language != updater.__class__.__name__.lower():
+                if self.language != updater.language.lower():
                     continue
             if not updater.check_applicable():
                 if self.language:
                     warn = (
                         'Selected language %s but language not applicable'
                         % self.language
                     )
                     self.util.warn(warn)
                 continue
             if not branch_created:
                 self.util.create_branch()
                 branch_created = True
             updates = updater.update_dependencies()
+            if not updates:
+                self.util.warn('No %s updates' % updater.language)
             updates_made = updates_made or updates
         if branch_created and not updates_made:
             self.util.rollback_branch()
         return updates_made
 
     def get_args(self) -> argparse.Namespace:
         parser = argparse.ArgumentParser(
@@ -99,14 +104,20 @@
         parser.add_argument(
             '-p',
             '--push',
             action='store_true',
             help='Push commits individually to remote origin',
         )
         parser.add_argument(
+            '-i',
+            '--ignore-cleanliness',
+            action='store_true',
+            help='Ignore checking if the repository is clean',
+        )
+        parser.add_argument(
             '-d',
             '--dryrun',
             action='store_true',
             help='Dry run',
         )
         parser.add_argument(
             '-v',
@@ -119,20 +130,21 @@
             action='version',
             version=__version__,
         )
         args = parser.parse_args()
         self.language = args.language
         self.util.push = args.push
         self.util.verbose = args.verbose
+        self.util.ignore_cleanliness = args.ignore_cleanliness
         self.util.dry_run = args.dryrun
         return args
 
     @staticmethod
     def updater_names() -> list[str]:
         return [u.__name__.lower() for u in UPDATERS]
 
 
-if __name__ == '__main__':
+if __name__ == '__main__':  # pragma: no cover
     try:
         main()
     except subprocess.CalledProcessError:
         pass
```

### Comparing `req-update-2.5.1/req_update/util.py` & `req_update-2.6.0/req_update/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,45 +39,46 @@
         return type(self).__name__
 
 
 class Util:
     def __init__(self) -> None:
         self.push = False
         self.verbose = False
+        self.ignore_cleanliness = True
         self.dry_run = True
         self.branch_exists = False
 
-    def check_repository_cleanliness(self) -> None:
+    def check_repository_cleanliness(self) -> bool:
         """
         Check that the repository is ready for updating dependencies.
-        Non-clean repositories will raise a RuntimeError
+        Returns a bool for if a repository is clean.
+        Raises a runtimeError if not being run within a git repository.
         """
         # Make sure there are no uncommitted files
         if self.dry_run:
-            return
+            return True
         command = ['git', 'status', '--porcelain']
         try:
             result = self.execute_shell(command, True)
         except subprocess.CalledProcessError as error:
             raise RuntimeError('Must run within a git repository') from error
         lines = result.stdout.split('\n')
         # Do not count untracked files when checking for repository cleanliness
         lines = [line for line in lines if line and line[:2] != '??']
-        if lines:
-            raise RuntimeError('Repository not clean')
+        return len(lines) == 0
 
     def commit_git(self, commit_message: str) -> None:
         """Create a git commit of all changed files"""
         self.log(commit_message)
         command = ['git', 'commit', '-am', commit_message]
         self.execute_shell(command, False)
         self.push_dependency_update()
 
     def commit_dependency_update(
-        self, language: str, dependency: str, version: str
+        self, language: str, dependency: str, version: str,
     ) -> None:
         """Create a commit with a dependency update"""
         commit_message = COMMIT_MESSAGE.format(
             language=language,
             package=dependency,
             version=version,
         )
@@ -137,15 +138,15 @@
             if int(compares[0]) < int(compares[1]):
                 return True
             if int(compares[0]) > int(compares[1]):
                 return False
         return False
 
     def check_major_version_update(
-        self, dependency: str, old_version: str, new_version: str
+        self, dependency: str, old_version: str, new_version: str,
     ) -> Optional[bool]:
         """
         Try to parse versions as semver and compare major version numbers.
         Log a warning if the major version numbers are different.
         Returns True if there is a major version bump
         Returns False if there is not a major version bump
         Returns None if versions are not semver
@@ -162,15 +163,15 @@
             new_version_major = int(new_version_parsed[0])
         except ValueError:
             return None
         if old_version_major == new_version_major:
             return False
         self.warn(
             'Warning: Major version change on %s: %s updated to %s'
-            % (dependency, old_version, new_version)
+            % (dependency, old_version, new_version),
         )
         return True
 
     def execute_shell(
         self,
         command: list[str],
         readonly: bool,
@@ -179,15 +180,15 @@
         ignore_exit_code: bool = False,
     ) -> SubprocessOutput:
         """Helper method to execute commands in a shell and return output"""
         if self.verbose:
             self.log(' '.join(command))
         if self.dry_run and not readonly:
             return subprocess.CompletedProcess(
-                command, 0, stdout='', stderr=''
+                command, 0, stdout='', stderr='',
             )
         try:
             result = subprocess.run(
                 command,
                 cwd=cwd,
                 capture_output=True,
                 check=True,
```

### Comparing `req-update-2.5.1/req_update.egg-info/PKG-INFO` & `req_update-2.6.0/req_update.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: req-update
-Version: 2.5.1
+Version: 2.6.0
 Summary: Update python, node, go, docker, and other dependencies
 Author-email: Albert Wang <git@albertyw.com>
 License: MIT
 Project-URL: Homepage, https://github.com/albertyw/req-update
 Keywords: dependencies
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,17 +19,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: test
-Requires-Dist: coverage==7.4.1; extra == "test"
-Requires-Dist: ruff==0.2.2; extra == "test"
-Requires-Dist: mypy==1.8.0; extra == "test"
+Requires-Dist: coverage==7.5.2; extra == "test"
+Requires-Dist: ruff==0.4.5; extra == "test"
+Requires-Dist: mypy==1.10.0; extra == "test"
 
 # req-update
 
 [![PyPI](https://img.shields.io/pypi/v/req-update)](https://pypi.org/project/req-update/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/req-update)
 ![PyPI - License](https://img.shields.io/pypi/l/req-update)
```

