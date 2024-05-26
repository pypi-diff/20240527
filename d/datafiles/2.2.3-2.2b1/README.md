# Comparing `tmp/datafiles-2.2.3.tar.gz` & `tmp/datafiles-2.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafiles-2.2.3.tar", max compression
+gzip compressed data, was "datafiles-2.2b1.tar", max compression
```

## Comparing `datafiles-2.2.3.tar` & `datafiles-2.2b1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1088 2019-06-09 21:33:24.000000 datafiles-2.2.3/LICENSE.md
--rw-r--r--   0        0        0     3654 2024-05-19 19:41:42.566877 datafiles-2.2.3/README.md
--rw-r--r--   0        0        0      236 2023-07-23 20:04:24.607458 datafiles-2.2.3/datafiles/__init__.py
--rw-r--r--   0        0        0      928 2024-05-04 18:07:52.074321 datafiles-2.2.3/datafiles/config.py
--rw-r--r--   0        0        0     6817 2022-11-23 17:08:26.552083 datafiles-2.2.3/datafiles/converters/__init__.py
--rw-r--r--   0        0        0     1605 2022-02-02 22:35:04.726189 datafiles-2.2.3/datafiles/converters/_bases.py
--rw-r--r--   0        0        0     1369 2022-02-02 22:35:04.726539 datafiles-2.2.3/datafiles/converters/builtins.py
--rw-r--r--   0        0        0     7671 2023-05-05 12:00:14.196700 datafiles-2.2.3/datafiles/converters/containers.py
--rw-r--r--   0        0        0      605 2022-02-02 22:35:04.727351 datafiles-2.2.3/datafiles/converters/enumerations.py
--rw-r--r--   0        0        0     1038 2022-02-02 22:35:04.727646 datafiles-2.2.3/datafiles/converters/extensions.py
--rw-r--r--   0        0        0     2334 2023-07-23 20:04:24.607703 datafiles-2.2.3/datafiles/decorators.py
--rw-r--r--   0        0        0     3643 2022-11-09 21:15:25.993928 datafiles-2.2.3/datafiles/formats.py
--rw-r--r--   0        0        0     4688 2022-04-22 23:18:12.443625 datafiles-2.2.3/datafiles/hooks.py
--rw-r--r--   0        0        0     5915 2024-03-16 19:42:53.212280 datafiles-2.2.3/datafiles/manager.py
--rw-r--r--   0        0        0    10552 2024-05-04 18:07:52.189629 datafiles-2.2.3/datafiles/mapper.py
--rw-r--r--   0        0        0     2402 2023-07-23 20:04:24.608029 datafiles-2.2.3/datafiles/model.py
--rw-r--r--   0        0        0     2373 2023-05-28 18:10:33.298224 datafiles-2.2.3/datafiles/plugins.py
--rw-r--r--   0        0        0        0 2023-03-26 23:55:27.144248 datafiles-2.2.3/datafiles/py.typed
--rw-r--r--   0        0        0      133 2021-05-26 11:50:47.865164 datafiles-2.2.3/datafiles/settings.py
--rw-r--r--   0        0        0      362 2022-07-29 16:35:41.394659 datafiles-2.2.3/datafiles/tests/__init__.py
--rw-r--r--   0        0        0    16339 2022-08-20 17:08:29.835977 datafiles-2.2.3/datafiles/tests/test_converters.py
--rw-r--r--   0        0        0     1255 2023-07-23 20:04:24.608283 datafiles-2.2.3/datafiles/tests/test_decorators.py
--rw-r--r--   0        0        0     1789 2022-02-02 22:35:04.730640 datafiles-2.2.3/datafiles/tests/test_formats.py
--rw-r--r--   0        0        0     2006 2022-02-02 22:35:04.730913 datafiles-2.2.3/datafiles/tests/test_generics.py
--rw-r--r--   0        0        0     1585 2022-04-22 23:06:52.609396 datafiles-2.2.3/datafiles/tests/test_hooks.py
--rw-r--r--   0        0        0     6215 2024-03-16 19:42:53.212931 datafiles-2.2.3/datafiles/tests/test_manager.py
--rw-r--r--   0        0        0     3849 2022-10-11 11:26:59.046450 datafiles-2.2.3/datafiles/tests/test_mapper.py
--rw-r--r--   0        0        0      609 2023-02-13 17:48:23.612872 datafiles-2.2.3/datafiles/tests/test_model.py
--rw-r--r--   0        0        0     2790 2022-03-07 14:07:43.245444 datafiles-2.2.3/datafiles/tests/test_utils.py
--rw-r--r--   0        0        0      743 2022-04-16 23:56:46.724770 datafiles-2.2.3/datafiles/types.py
--rw-r--r--   0        0        0     4363 2024-05-26 22:10:32.206806 datafiles-2.2.3/datafiles/utils.py
--rw-r--r--   0        0        0     2049 2024-05-26 22:17:22.716150 datafiles-2.2.3/pyproject.toml
--rw-r--r--   0        0        0     5061 1970-01-01 00:00:00.000000 datafiles-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1088 2019-06-09 21:33:24.000000 datafiles-2.2b1/LICENSE.md
+-rw-r--r--   0        0        0     3591 2023-07-21 15:51:12.989466 datafiles-2.2b1/README.md
+-rw-r--r--   0        0        0      236 2023-07-21 15:53:49.187973 datafiles-2.2b1/datafiles/__init__.py
+-rw-r--r--   0        0        0      929 2022-10-11 11:26:59.042300 datafiles-2.2b1/datafiles/config.py
+-rw-r--r--   0        0        0     6817 2022-11-23 17:08:26.552083 datafiles-2.2b1/datafiles/converters/__init__.py
+-rw-r--r--   0        0        0     1605 2022-02-02 22:35:04.726189 datafiles-2.2b1/datafiles/converters/_bases.py
+-rw-r--r--   0        0        0     1369 2022-02-02 22:35:04.726539 datafiles-2.2b1/datafiles/converters/builtins.py
+-rw-r--r--   0        0        0     7671 2023-05-05 12:00:14.196700 datafiles-2.2b1/datafiles/converters/containers.py
+-rw-r--r--   0        0        0      605 2022-02-02 22:35:04.727351 datafiles-2.2b1/datafiles/converters/enumerations.py
+-rw-r--r--   0        0        0     1038 2022-02-02 22:35:04.727646 datafiles-2.2b1/datafiles/converters/extensions.py
+-rw-r--r--   0        0        0     2334 2023-07-23 04:01:33.922645 datafiles-2.2b1/datafiles/decorators.py
+-rw-r--r--   0        0        0     3643 2022-11-09 21:15:25.993928 datafiles-2.2b1/datafiles/formats.py
+-rw-r--r--   0        0        0     4688 2022-04-22 23:18:12.443625 datafiles-2.2b1/datafiles/hooks.py
+-rw-r--r--   0        0        0     6011 2023-02-13 17:48:23.609765 datafiles-2.2b1/datafiles/manager.py
+-rw-r--r--   0        0        0    10496 2023-07-21 16:16:07.783884 datafiles-2.2b1/datafiles/mapper.py
+-rw-r--r--   0        0        0     2402 2023-07-23 04:01:33.922788 datafiles-2.2b1/datafiles/model.py
+-rw-r--r--   0        0        0     2373 2023-05-28 18:10:33.298224 datafiles-2.2b1/datafiles/plugins.py
+-rw-r--r--   0        0        0        0 2023-03-26 23:55:27.144248 datafiles-2.2b1/datafiles/py.typed
+-rw-r--r--   0        0        0      133 2021-05-26 11:50:47.865164 datafiles-2.2b1/datafiles/settings.py
+-rw-r--r--   0        0        0      362 2022-07-29 16:35:41.394659 datafiles-2.2b1/datafiles/tests/__init__.py
+-rw-r--r--   0        0        0    16339 2022-08-20 17:08:29.835977 datafiles-2.2b1/datafiles/tests/test_converters.py
+-rw-r--r--   0        0        0     1255 2023-07-23 04:01:33.923084 datafiles-2.2b1/datafiles/tests/test_decorators.py
+-rw-r--r--   0        0        0     1789 2022-02-02 22:35:04.730640 datafiles-2.2b1/datafiles/tests/test_formats.py
+-rw-r--r--   0        0        0     2006 2022-02-02 22:35:04.730913 datafiles-2.2b1/datafiles/tests/test_generics.py
+-rw-r--r--   0        0        0     1585 2022-04-22 23:06:52.609396 datafiles-2.2b1/datafiles/tests/test_hooks.py
+-rw-r--r--   0        0        0     5555 2023-02-11 00:35:02.076274 datafiles-2.2b1/datafiles/tests/test_manager.py
+-rw-r--r--   0        0        0     3849 2022-10-11 11:26:59.046450 datafiles-2.2b1/datafiles/tests/test_mapper.py
+-rw-r--r--   0        0        0      609 2023-02-13 17:48:23.612872 datafiles-2.2b1/datafiles/tests/test_model.py
+-rw-r--r--   0        0        0     2790 2022-03-07 14:07:43.245444 datafiles-2.2b1/datafiles/tests/test_utils.py
+-rw-r--r--   0        0        0      743 2022-04-16 23:56:46.724770 datafiles-2.2b1/datafiles/types.py
+-rw-r--r--   0        0        0     4242 2022-04-16 23:57:40.170785 datafiles-2.2b1/datafiles/utils.py
+-rw-r--r--   0        0        0     2013 2023-07-23 04:01:33.924992 datafiles-2.2b1/pyproject.toml
+-rw-r--r--   0        0        0     5197 1970-01-01 00:00:00.000000 datafiles-2.2b1/PKG-INFO
```

### Comparing `datafiles-2.2.3/LICENSE.md` & `datafiles-2.2b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/README.md` & `datafiles-2.2b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # Datafiles: A file-based ORM for Python dataclasses
 
 Datafiles is a bidirectional serialization library for Python [dataclasses](https://docs.python.org/3/library/dataclasses.html) to synchronize objects to the filesystem using type annotations. It supports a variety of file formats with round-trip preservation of formatting and comments, where possible. Object changes are automatically saved to disk and only include the minimum data needed to restore each object.
 
-[![Linux Build](https://img.shields.io/github/actions/workflow/status/jacebrowning/datafiles/main.yml?branch=main&label=linux)](https://github.com/jacebrowning/datafiles/actions)
-[![Windows Build](https://img.shields.io/appveyor/ci/jacebrowning/datafiles/main.svg?label=windows)](https://ci.appveyor.com/project/jacebrowning/datafiles)
-[![Code Coverage](https://img.shields.io/codecov/c/github/jacebrowning/datafiles)
-](https://codecov.io/gh/jacebrowning/datafiles)
+[![Travis CI](https://img.shields.io/travis/com/jacebrowning/datafiles/main.svg?label=unix)](https://app.travis-ci.com/jacebrowning/datafiles)
+[![AppVeyor](https://img.shields.io/appveyor/ci/jacebrowning/datafiles/main.svg?label=windows)](https://ci.appveyor.com/project/jacebrowning/datafiles)
+[![Coveralls](https://img.shields.io/coveralls/jacebrowning/datafiles.svg)](https://coveralls.io/r/jacebrowning/datafiles)
 [![PyPI License](https://img.shields.io/pypi/l/datafiles.svg)](https://pypi.org/project/datafiles)
-[![PyPI Version](https://img.shields.io/pypi/v/datafiles.svg?label=version)](https://pypi.org/project/datafiles)
+[![PyPI Version](https://img.shields.io/pypi/v/datafiles.svg)](https://pypi.org/project/datafiles)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/datafiles.svg?color=orange)](https://pypistats.org/packages/datafiles)
 [![Gitter](https://img.shields.io/gitter/room/jacebrowning/datafiles?color=D0164E)](https://gitter.im/jacebrowning/datafiles)
 
 Some common use cases include:
 
 - Coercing user-editable files into the proper Python types
-- Storing program configuration and state in version control
+- Storing program configuration and data in version control
 - Loading data fixtures for demonstration or testing purposes
 - Synchronizing application state using file sharing services
 - Prototyping data models agnostic of persistence backends
 
 Watch [my lightning talk](https://www.youtube.com/watch?v=moYkuNrmc1I&feature=youtu.be&t=1225) for a demo of this in action!
 
 ## Overview
```

### Comparing `datafiles-2.2.3/datafiles/config.py` & `datafiles-2.2b1/datafiles/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Configuration defaults for each model."""
 
+
 from contextlib import suppress
 from dataclasses import dataclass
 from typing import Dict, Optional
 
 from .converters import Converter
```

### Comparing `datafiles-2.2.3/datafiles/converters/__init__.py` & `datafiles-2.2b1/datafiles/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/converters/_bases.py` & `datafiles-2.2b1/datafiles/converters/_bases.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/converters/builtins.py` & `datafiles-2.2b1/datafiles/converters/builtins.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/converters/containers.py` & `datafiles-2.2b1/datafiles/converters/containers.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/converters/enumerations.py` & `datafiles-2.2b1/datafiles/converters/enumerations.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/converters/extensions.py` & `datafiles-2.2b1/datafiles/converters/extensions.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/decorators.py` & `datafiles-2.2b1/datafiles/decorators.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/formats.py` & `datafiles-2.2b1/datafiles/formats.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/hooks.py` & `datafiles-2.2b1/datafiles/hooks.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/manager.py` & `datafiles-2.2b1/datafiles/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 from . import hooks, model
 
 if TYPE_CHECKING:
     from .model import Model
 
 
 Trilean = Optional[bool]
-Missing = dataclasses._MISSING_TYPE  # sentinel value for arguments to be loaded
-Absent = object()  # sentinel value for required arguments not passed
+Missing = dataclasses._MISSING_TYPE
+_NOT_PASSED = object()  # sentinel
 
 
 class Splats:
     def __getattr__(self, name):
         return "*"
 
 
@@ -34,45 +34,48 @@
     def __init__(self, cls):
         self.model = cls
 
     def get(self, *args, **kwargs) -> Model:
         with hooks.disabled():
             instance = self.model.__new__(self.model)
 
-            # Set initial values for all passed arguments
+            # We **must** initialize with a value all fields on the uninitialized
+            # instance which play a role in loading, e.g., those with placeholders
+            # in the pattern. Other init fields of the instance which are not passed
+            # as args or kwargs will be set to `dataclasses._MISSING_TYPE` and their
+            # values will be loaded over.
             fields = [field for field in dataclasses.fields(self.model) if field.init]
             pattern = self.model.Meta.datafile_pattern
             args_iter = iter(args)
             for field in fields:
                 placeholder = f"{{self.{field.name}}}"
 
                 try:
+                    # we always need to consume an arg if it exists,
+                    # even if it's not one with a placeholder
                     value = next(args_iter)
                 except StopIteration:
-                    value = kwargs.get(field.name, Absent)
+                    value = kwargs.get(field.name, _NOT_PASSED)
 
-                if (
-                    placeholder in pattern
-                    and value is Absent
-                    and isinstance(field.default, Missing)
-                ):
-                    raise TypeError(
-                        f"Manager.get() missing required placeholder field argument: '{field.name}'"
-                    )
+                if placeholder in pattern:
+                    if value is _NOT_PASSED:
+                        raise TypeError(
+                            f"Manager.get() missing required placeholder field argument: '{field.name}'"
+                        )
 
-                if value is Absent:
+                if value is _NOT_PASSED:
                     if not isinstance(field.default, Missing):
                         value = field.default
                     elif not isinstance(field.default_factory, Missing):
                         value = field.default_factory()
                     else:
                         value = Missing
                 object.__setattr__(instance, field.name, value)
 
-            # Bypass calling load() because hooks are disabled currently
+            # NOTE: the following doesn't call instance.datafile.load because hooks are disabled currently
             model.Model.__post_init__(instance)
 
             try:
                 instance.datafile.load(_first_load=True)
             except MarkedYAMLError as e:
                 log.critical(
                     f"Deleting invalid YAML: {instance.datafile.path} ({e.problem})"
@@ -115,30 +118,28 @@
             except (TypeError, OSError):
                 level = log.DEBUG if "__main__" in str(self.model) else log.WARNING
                 log.log(level, f"Unable to determine module for {self.model}")
                 root = Path.cwd()
             path = root / self.model.Meta.datafile_pattern
             log.debug(f"Detected dynamic pattern: {path}")
 
-        pattern = alt_pattern = str(path.resolve())
-        for field in dataclasses.fields(self.model):
-            if not isinstance(field.default, Missing):
-                alt_pattern = alt_pattern.replace("{self." + field.name + "}", "")
+        pattern = str(path.resolve())
         splatted = pattern.format(self=Splats()).replace(
             f"{os.sep}*{os.sep}", f"{os.sep}**{os.sep}"
         )
 
         log.info(f"Finding files matching pattern: {splatted}")
         for index, filename in enumerate(iglob(splatted, recursive=True)):
+
             if Path(filename).is_dir():
                 log.debug(f"Skipped matching directory {index + 1}: {filename}")
                 continue
 
             log.debug(f"Found matching path {index + 1}: {filename}")
-            result = parse(pattern, filename) or parse(alt_pattern, filename)
+            result = parse(pattern, filename)
             if result:
                 values = list(result.named.values())
 
                 if len(values) > 1 and os.sep in values[-1]:
                     parts = values[-1].rsplit(os.sep, 1)
                     values[-2] = values[-2] + os.sep + parts[0]
                     values[-1] = parts[1]
```

### Comparing `datafiles-2.2.3/datafiles/mapper.py` & `datafiles-2.2b1/datafiles/mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,19 +127,17 @@
         for name, converter in self.attrs.items():
             value = data[name]
 
             if getattr(converter, "DATACLASS", None):
                 log.debug(f"Converting '{name}' dataclass with {converter}")
                 new_value = converter.to_preserialization_data(
                     value,
-                    default_to_skip=(
-                        Missing
-                        if include_default_values
-                        else get_default_field_value(self._instance, name)
-                    ),
+                    default_to_skip=Missing
+                    if include_default_values
+                    else get_default_field_value(self._instance, name),
                 )
                 data[name] = recursive_update(value, new_value)
 
             elif (
                 value == get_default_field_value(self._instance, name)
                 and not include_default_values
             ):
```

### Comparing `datafiles-2.2.3/datafiles/model.py` & `datafiles-2.2b1/datafiles/model.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/plugins.py` & `datafiles-2.2b1/datafiles/plugins.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/tests/test_converters.py` & `datafiles-2.2b1/datafiles/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/tests/test_decorators.py` & `datafiles-2.2b1/datafiles/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/tests/test_formats.py` & `datafiles-2.2b1/datafiles/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/tests/test_generics.py` & `datafiles-2.2b1/datafiles/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/tests/test_hooks.py` & `datafiles-2.2b1/datafiles/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/tests/test_manager.py` & `datafiles-2.2b1/datafiles/tests/test_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=unused-variable,unused-argument
+# pylint: disable=unused-variable
 
 import os
 import shutil
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional
 from unittest.mock import patch
@@ -21,147 +21,129 @@
 @dataclass
 class MyClass:
     foo: int
     bar: int
     nested: Optional[Nested] = None
 
 
-@dataclass
-class MyClassDefaults:
-    foo: int
-    bar: int = 2
-
-
 def describe_manager():
     @pytest.fixture
-    def files():
-        return Path(__file__).parent / "files"
-
-    @pytest.fixture
-    def manager(files: Path):
-        shutil.rmtree(files, ignore_errors=True)
+    def manager():
+        shutil.rmtree(Path(__file__).parent / "files", ignore_errors=True)
         model = create_model(MyClass, pattern="files/{self.foo}.yml")
         return Manager(model)
 
     @pytest.fixture
-    def manager_at_home():
+    def manager_home():
         model = create_model(Nested, pattern="~/.{self.name}.json")
         return Manager(model)
 
-    @pytest.fixture
-    def manager_with_files(files: Path):
-        files.mkdir(exist_ok=True)
+    @pytest.fixture()
+    def manager_with_files():
+        files_dir = Path(__file__).parent / "files"
+        shutil.rmtree(files_dir, ignore_errors=True)
+        files_dir.mkdir(exist_ok=True)
         model = create_model(MyClass, pattern="files/{self.foo}.yml")
         model(foo=1, bar=2).datafile.save()
         return Manager(model)
 
-    @pytest.fixture
-    def manager_with_defaults(files: Path):
-        shutil.rmtree(files, ignore_errors=True)
-        model = create_model(MyClassDefaults, pattern="files/{self.foo}/{self.bar}.yml")
-        return Manager(model)
-
     def describe_get():
         @patch("datafiles.mapper.Mapper.load")
         @patch("datafiles.mapper.Mapper.exists", True)
         @patch("datafiles.mapper.Mapper.modified", False)
-        def when_absent_pattern_arg(mock_load, expect, manager):
-            instance = manager.get(1)
-            expect(instance.foo) == 1
-            expect(instance.bar) is Missing
+        def when_partial_args_passed_init_args_missing(mock_load, expect, manager):
+            got = manager.get(1)
+            expect(got.foo) == 1
+            expect(got.bar) is Missing
             expect(mock_load.called).is_(True)
 
             with expect.raises(
                 TypeError,
                 "Manager.get() missing required placeholder field argument: 'foo'",
             ):
                 manager.get(bar=2)
 
-        @patch("datafiles.mapper.Mapper.load")
         @patch("datafiles.mapper.Mapper.exists", True)
         @patch("datafiles.mapper.Mapper.modified", False)
-        def when_absent_pattern_arg_has_default_value(
-            mock_load, expect, manager_with_defaults: Manager
+        def when_partial_args_passed_init_arg_missing_file_exists(
+            expect, manager_with_files
         ):
-            expect(manager_with_defaults.get(0, 1)) == MyClassDefaults(foo=0, bar=1)
-            expect(manager_with_defaults.get(1)) == MyClassDefaults(foo=1, bar=2)
-            expect(mock_load.called).is_(True)
-
-        @patch("datafiles.mapper.Mapper.exists", True)
-        @patch("datafiles.mapper.Mapper.modified", False)
-        def when_partial_args_match_file(expect, manager_with_files: Manager):
+            # demonstrates that `Manager.get` loads the value for bar, when it is not passed
             expect(manager_with_files.get(1)) == MyClass(foo=1, bar=2)
 
         @patch("datafiles.mapper.Mapper.exists", True)
         @patch("datafiles.mapper.Mapper.modified", False)
-        def when_partial_kwargs_match_file(expect, manager_with_files: Manager):
+        def when_partial_kwargs_passed_init_arg_missing_file_exists(
+            expect, manager_with_files
+        ):
+            # demonstrates that `Manager.get` loads the value for bar, when it is not passed
             expect(manager_with_files.get(foo=1)) == MyClass(foo=1, bar=2)
 
     def describe_get_or_none():
         @patch("datafiles.mapper.Mapper.load")
         @patch("datafiles.mapper.Mapper.exists", True)
         @patch("datafiles.mapper.Mapper.modified", False)
-        def when_file_exists(mock_load, expect, manager: Manager):
+        def when_file_exists(mock_load, expect, manager):
             expect(manager.get_or_none(foo=1, bar=2)) == MyClass(foo=1, bar=2)
             expect(mock_load.called).is_(True)
 
         @patch("datafiles.mapper.Mapper.exists", False)
-        def when_file_missing(expect, manager: Manager):
+        def when_file_missing(expect, manager):
             expect(manager.get_or_none(foo=3, bar=4)).is_(None)
 
-        def when_file_corrupt(expect, manager: Manager):
+        def when_file_corrupt(expect, manager):
             instance = manager.get_or_create(foo=2, bar=1)
             instance.datafile.path.write_text("{")
             instance2 = manager.get_or_none(foo=2, bar=2)
             expect(instance2).is_(None)
             expect(instance.datafile.path.is_file()).is_(False)
 
     def describe_get_or_create():
         @patch("datafiles.mapper.Mapper.save")
         @patch("datafiles.mapper.Mapper.load")
         @patch("datafiles.mapper.Mapper.exists", True)
         @patch("datafiles.mapper.Mapper.modified", False)
-        def when_file_exists(mock_save, mock_load, expect, manager: Manager):
+        def when_file_exists(mock_save, mock_load, expect, manager):
             expect(manager.get_or_create(foo=1, bar=2)) == MyClass(foo=1, bar=2)
             expect(mock_save.called).is_(True)
             expect(mock_load.called).is_(False)
 
         @patch("datafiles.mapper.Mapper.save")
         @patch("datafiles.mapper.Mapper.load")
         @patch("datafiles.mapper.Mapper.exists", False)
-        def when_file_missing(mock_save, mock_load, expect, manager: Manager):
+        def when_file_missing(mock_save, mock_load, expect, manager):
             expect(manager.get_or_create(foo=1, bar=2)) == MyClass(foo=1, bar=2)
             expect(mock_save.called).is_(True)
             expect(mock_load.called).is_(True)
 
-        def when_file_corrupt(expect, manager: Manager):
+        def when_file_corrupt(expect, manager):
             instance = manager.get_or_create(foo=2, bar=1)
             instance.datafile.path.write_text("{")
             instance2 = manager.get_or_create(foo=2, bar=2)
-            expect(instance2.bar) == 2  # type: ignore[attr-defined]
+            expect(instance2.bar) == 2
 
     def describe_all():
         @patch("datafiles.mapper.Mapper.exists", False)
-        def when_no_files_exist(expect, manager: Manager):
+        def when_no_files_exist(expect, manager):
             items = list(manager.all())
             expect(items) == []
 
-        def with_home_directory(expect, manager_at_home: Manager):
-            items = list(manager_at_home.all())
+        def with_home_directory(expect, manager_home):
+            items = list(manager_home.all())
             if "CI" not in os.environ:
                 expect(len(items)) > 0
 
     def describe_filter():
         @patch("datafiles.mapper.Mapper.exists", False)
-        def when_no_files_exist(expect, manager: Manager):
+        def when_no_files_exist(expect, manager):
             items = list(manager.filter())
             expect(items) == []
 
         @patch("datafiles.mapper.Mapper.exists", False)
-        def with_partial_positional_arguments(expect, manager: Manager):
+        def with_partial_positional_arguments(expect, manager):
             items = list(manager.filter(foo=1))
             expect(items) == []
 
         @patch("datafiles.mapper.Mapper.exists", False)
-        def with_nested_key_query(expect, manager: Manager):
+        def with_nested_key_query(expect, manager):
             items = list(manager.filter(nested__name="John Doe"))
             expect(items) == []
```

### Comparing `datafiles-2.2.3/datafiles/tests/test_mapper.py` & `datafiles-2.2b1/datafiles/tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/tests/test_model.py` & `datafiles-2.2b1/datafiles/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/tests/test_utils.py` & `datafiles-2.2b1/datafiles/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/types.py` & `datafiles-2.2b1/datafiles/types.py`

 * *Files identical despite different names*

### Comparing `datafiles-2.2.3/datafiles/utils.py` & `datafiles-2.2b1/datafiles/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Internal helper functions."""
 
 import dataclasses
 import time
 from contextlib import suppress
-from dataclasses import Field
 from functools import lru_cache
 from pathlib import Path
 from pprint import pformat
 from shutil import get_terminal_size
 from typing import Any, Dict, Union
 
 import log
@@ -27,27 +26,22 @@
 def get_default_field_value(instance, name):
     for field in dataclasses.fields(instance):
         if field.name == name:
             if not isinstance(field.default, Missing):
                 return field.default
 
             if not isinstance(field.default_factory, Missing):  # type: ignore
-                return _call_default_factory(field)
+                return field.default_factory()  # type: ignore
 
             if not field.init and hasattr(instance, "__post_init__"):
                 return getattr(instance, name)
 
     return Missing
 
 
-@cached
-def _call_default_factory(field: Field):
-    return field.default_factory()  # type: ignore
-
-
 def prettify(value) -> str:
     """Ensure value is a dictionary pretty-format it."""
     return pformat(dictify(value))
 
 
 def dictify(value):
     """Ensure value is a dictionary."""
```

### Comparing `datafiles-2.2.3/pyproject.toml` & `datafiles-2.2b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "datafiles"
-version = "2.2.3"
+version = "2.2b1"
 description = "File-based ORM for dataclasses."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
@@ -49,20 +49,20 @@
 
 # ORM
 parse = "^1.12"
 
 # Utilities
 cached_property = "^1.5"
 classproperties = "^0.2"
-minilog = "^2.3"
+minilog = "^2.1"
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
-black = "^24.3"
+black = "^22.1"
 isort = "^5.10"
 
 # Linters
 mypy = "^1.3"
 pylint = "~2.15"
 pydocstyle = "*"
 
@@ -83,17 +83,17 @@
 # Documentation
 mkdocs = "^1.4"
 pygments = "^2.15"
 
 # Notebooks
 idna = "^3.3" # papermill dependency
 ipython = "^8.10"
-notebook = { version = "^7.2", markers = "os.name != 'nt'" }
+jupyter = { version = "^1.0", markers = "sys_platform != 'win32'" }
 nbstripout ="~0.4"
-papermill = { version = "^2.3", markers = "os.name != 'nt'" }
+papermill = "^2.3"
 
 [tool.black]
 
 quiet = true
 
 [tool.isort]
```

### Comparing `datafiles-2.2.3/PKG-INFO` & `datafiles-2.2b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafiles
-Version: 2.2.3
+Version: 2.2b1
 Summary: File-based ORM for dataclasses.
 Home-page: https://pypi.org/project/datafiles
 License: MIT
 Keywords: dataclasses,serialization,type-annotations,object-relational mapping,YAML,JSON,TOML
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -15,44 +15,47 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Dist: cached_property (>=1.5,<2.0)
 Requires-Dist: classproperties (>=0.2,<0.3)
-Requires-Dist: minilog (>=2.3,<3.0)
+Requires-Dist: minilog (>=2.1,<3.0)
 Requires-Dist: parse (>=1.12,<2.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: tomlkit (>=0.10.1,<0.11.0)
 Project-URL: Documentation, https://datafiles.readthedocs.io
 Project-URL: Repository, https://github.com/jacebrowning/datafiles
 Description-Content-Type: text/markdown
 
 # Datafiles: A file-based ORM for Python dataclasses
 
 Datafiles is a bidirectional serialization library for Python [dataclasses](https://docs.python.org/3/library/dataclasses.html) to synchronize objects to the filesystem using type annotations. It supports a variety of file formats with round-trip preservation of formatting and comments, where possible. Object changes are automatically saved to disk and only include the minimum data needed to restore each object.
 
-[![Linux Build](https://img.shields.io/github/actions/workflow/status/jacebrowning/datafiles/main.yml?branch=main&label=linux)](https://github.com/jacebrowning/datafiles/actions)
-[![Windows Build](https://img.shields.io/appveyor/ci/jacebrowning/datafiles/main.svg?label=windows)](https://ci.appveyor.com/project/jacebrowning/datafiles)
-[![Code Coverage](https://img.shields.io/codecov/c/github/jacebrowning/datafiles)
-](https://codecov.io/gh/jacebrowning/datafiles)
+[![Travis CI](https://img.shields.io/travis/com/jacebrowning/datafiles/main.svg?label=unix)](https://app.travis-ci.com/jacebrowning/datafiles)
+[![AppVeyor](https://img.shields.io/appveyor/ci/jacebrowning/datafiles/main.svg?label=windows)](https://ci.appveyor.com/project/jacebrowning/datafiles)
+[![Coveralls](https://img.shields.io/coveralls/jacebrowning/datafiles.svg)](https://coveralls.io/r/jacebrowning/datafiles)
 [![PyPI License](https://img.shields.io/pypi/l/datafiles.svg)](https://pypi.org/project/datafiles)
-[![PyPI Version](https://img.shields.io/pypi/v/datafiles.svg?label=version)](https://pypi.org/project/datafiles)
+[![PyPI Version](https://img.shields.io/pypi/v/datafiles.svg)](https://pypi.org/project/datafiles)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/datafiles.svg?color=orange)](https://pypistats.org/packages/datafiles)
 [![Gitter](https://img.shields.io/gitter/room/jacebrowning/datafiles?color=D0164E)](https://gitter.im/jacebrowning/datafiles)
 
 Some common use cases include:
 
 - Coercing user-editable files into the proper Python types
-- Storing program configuration and state in version control
+- Storing program configuration and data in version control
 - Loading data fixtures for demonstration or testing purposes
 - Synchronizing application state using file sharing services
 - Prototyping data models agnostic of persistence backends
 
 Watch [my lightning talk](https://www.youtube.com/watch?v=moYkuNrmc1I&feature=youtu.be&t=1225) for a demo of this in action!
 
 ## Overview
```

