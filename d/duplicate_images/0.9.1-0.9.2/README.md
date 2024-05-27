# Comparing `tmp/duplicate_images-0.9.1.tar.gz` & `tmp/duplicate_images-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duplicate_images-0.9.1.tar", max compression
+gzip compressed data, was "duplicate_images-0.9.2.tar", max compression
```

## Comparing `duplicate_images-0.9.1.tar` & `duplicate_images-0.9.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1172 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/LICENSE
--rw-r--r--   0        0        0     9540 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/README.md
--rw-r--r--   0        0        0        0 2023-08-24 22:24:55.611681 duplicate_images-0.9.1/duplicate_images/__init__.py
--rw-r--r--   0        0        0      711 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/duplicate_images/common.py
--rwxr-xr-x   0        0        0     2947 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/duplicate_images/duplicate.py
--rw-r--r--   0        0        0      584 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/duplicate_images/function_types.py
--rw-r--r--   0        0        0      164 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/duplicate_images/hash_scanner/__init__.py
--rw-r--r--   0        0        0     2046 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/duplicate_images/hash_scanner/image_hash_scanner.py
--rw-r--r--   0        0        0     3301 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/duplicate_images/hash_store.py
--rw-r--r--   0        0        0     6415 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/duplicate_images/image_pair_finder.py
--rw-r--r--   0        0        0      439 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/duplicate_images/log.py
--rw-r--r--   0        0        0     3835 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/duplicate_images/methods.py
--rw-r--r--   0        0        0      557 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/duplicate_images/pair_finder_options.py
--rw-r--r--   0        0        0     2357 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/duplicate_images/parse_commandline.py
--rw-r--r--   0        0        0     1818 2023-08-24 22:24:55.528680 duplicate_images-0.9.1/duplicate_images/progress_bar_manager.py
--rw-r--r--   0        0        0     1084 2023-08-24 22:24:55.529680 duplicate_images-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    10611 1970-01-01 00:00:00.000000 duplicate_images-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1172 2023-08-26 09:02:50.578413 duplicate_images-0.9.2/LICENSE
+-rw-r--r--   0        0        0     9638 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/README.md
+-rw-r--r--   0        0        0        0 2023-08-26 09:02:50.658412 duplicate_images-0.9.2/duplicate_images/__init__.py
+-rw-r--r--   0        0        0      711 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/duplicate_images/common.py
+-rwxr-xr-x   0        0        0     2947 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/duplicate_images/duplicate.py
+-rw-r--r--   0        0        0      584 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/duplicate_images/function_types.py
+-rw-r--r--   0        0        0      164 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/duplicate_images/hash_scanner/__init__.py
+-rw-r--r--   0        0        0     2046 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/duplicate_images/hash_scanner/image_hash_scanner.py
+-rw-r--r--   0        0        0     3301 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/duplicate_images/hash_store.py
+-rw-r--r--   0        0        0     6415 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/duplicate_images/image_pair_finder.py
+-rw-r--r--   0        0        0      439 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/duplicate_images/log.py
+-rw-r--r--   0        0        0     3659 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/duplicate_images/methods.py
+-rw-r--r--   0        0        0      557 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/duplicate_images/pair_finder_options.py
+-rw-r--r--   0        0        0     2357 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/duplicate_images/parse_commandline.py
+-rw-r--r--   0        0        0     1818 2023-08-26 09:02:50.579413 duplicate_images-0.9.2/duplicate_images/progress_bar_manager.py
+-rw-r--r--   0        0        0     1084 2023-08-26 09:02:50.580413 duplicate_images-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    10709 1970-01-01 00:00:00.000000 duplicate_images-0.9.2/PKG-INFO
```

### Comparing `duplicate_images-0.9.1/LICENSE` & `duplicate_images-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `duplicate_images-0.9.1/README.md` & `duplicate_images-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,17 @@
 
 ### Actions for matching image groups
 
 Use the `--on-equal` option to select what to do to pairs of equal images. The default action is 
 `print`.
 - `delete-first` or `d1`: deletes the first of the files in the group
 - `delete-last` or `dl`: deletes the last of the files in the group
-- `delete-bigger` or `d>`: deletes the file with the biggest size
-- `delete-smaller` or `d<`: deletes the file with the smallest size
+- `delete-biggest` or `d>`: deletes the file with the biggest size
+- `delete-smallest` or `d<`: deletes the file with the smallest size
+- `symlink-smaller`: delete the smaller files and replace them to a symlink to the biggest file
 - `eog`: launches the `eog` image viewer to compare the files in the group (*deprecated* by `exec`)
 - `xv`: launches the `xv` image viewer to compare the files in the group (*deprecated* by `exec`)
 - `print`: prints the files in the group
 - `print_inline`: like `print` but without newline
 - `quote`: prints the files in the group quoted for POSIX shells
 - `quote_inline`: like `quote` but without newline
 - `exec`: executes a command (see `--exec` argument below)
```

### Comparing `duplicate_images-0.9.1/duplicate_images/common.py` & `duplicate_images-0.9.2/duplicate_images/common.py`

 * *Files identical despite different names*

### Comparing `duplicate_images-0.9.1/duplicate_images/duplicate.py` & `duplicate_images-0.9.2/duplicate_images/duplicate.py`

 * *Files identical despite different names*

### Comparing `duplicate_images-0.9.1/duplicate_images/function_types.py` & `duplicate_images-0.9.2/duplicate_images/function_types.py`

 * *Files identical despite different names*

### Comparing `duplicate_images-0.9.1/duplicate_images/hash_scanner/image_hash_scanner.py` & `duplicate_images-0.9.2/duplicate_images/hash_scanner/image_hash_scanner.py`

 * *Files identical despite different names*

### Comparing `duplicate_images-0.9.1/duplicate_images/hash_store.py` & `duplicate_images-0.9.2/duplicate_images/hash_store.py`

 * *Files identical despite different names*

### Comparing `duplicate_images-0.9.1/duplicate_images/image_pair_finder.py` & `duplicate_images-0.9.2/duplicate_images/image_pair_finder.py`

 * *Files identical despite different names*

### Comparing `duplicate_images-0.9.1/duplicate_images/methods.py` & `duplicate_images-0.9.2/duplicate_images/methods.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 __author__ = 'Lene Preuss <lene.preuss@gmail.com>'
 
 import logging
 from argparse import Namespace
-from functools import lru_cache
-from hashlib import sha256
 from pathlib import Path
 from shlex import quote
 from subprocess import call  # nosec
 from typing import Any, Callable, Dict, List, Optional
 
 import imagehash
 
@@ -16,38 +14,31 @@
 
 __all__ = [
     'call', 'quote', 'get_hash_size_kwargs', 'IMAGE_HASH_ALGORITHM', 'ALGORITHM_DEFAULTS',
     'ACTIONS_ON_EQUALITY'
 ]
 
 
-@lru_cache(maxsize=None)
-def get_size(file: Path) -> int:
-    return file.stat().st_size
-
-
-@lru_cache(maxsize=None)
-def get_hash(file: Path) -> str:
-    return sha256(file.open('rb').read()).hexdigest()
-
-
-def compare_exactly(file: Path, other_file: Path) -> bool:
-    """Returns True if file and other_file are exactly exactly_equal"""
-    return get_size(other_file) == get_size(file) and get_hash(file) == get_hash(other_file)
-
-
 def ascending_by_size(group: ImageGroup) -> List[Path]:
-    return sorted(group, key=lambda path: path.stat().st_size)
+    return sorted(group, key=lambda path: (path.stat().st_size, str(path)))
 
 
 def delete_with_log_message(file: Path) -> None:
     file.unlink()
     logging.info('Deleted %s', path_with_parent(file))
 
 
+def symlink_to_biggest_file(group: ImageGroup):
+    biggest = ascending_by_size(group)[-1]
+    others = set(group) - {biggest}
+    for file in others:
+        delete_with_log_message(file)
+        file.symlink_to(biggest)
+
+
 def shell_exec(args: Namespace, group: ImageGroup) -> None:
     cmd = args.exec
     for num, path in enumerate(group):
         cmd = cmd.replace(f"{'{'}{num+1}{'}'}", f'{quote(str(path))}')
     cmd = cmd.replace('{*}', ' '.join([quote(str(path)) for path in group]))
     call(cmd, shell=True)  # nosec
 
@@ -80,18 +71,19 @@
 }
 
 ACTIONS_ON_EQUALITY: Dict[str, ActionFunction] = {
     'delete-first': lambda args, group: delete_with_log_message(group[0]),
     'd1': lambda args, group: delete_with_log_message(group[0]),
     'delete-last': lambda args, group: delete_with_log_message(group[-1]),
     'dl': lambda args, group: delete_with_log_message(group[-1]),
-    'delete-bigger': lambda args, group: delete_with_log_message(ascending_by_size(group)[-1]),
+    'delete-biggest': lambda args, group: delete_with_log_message(ascending_by_size(group)[-1]),
     'd>': lambda args, group: delete_with_log_message(ascending_by_size(group)[-1]),
-    'delete-smaller': lambda args, group: delete_with_log_message(ascending_by_size(group)[0]),
+    'delete-smallest': lambda args, group: delete_with_log_message(ascending_by_size(group)[0]),
     'd<': lambda args, group: delete_with_log_message(ascending_by_size(group)[0]),
+    'symlink-smaller': lambda args, group: symlink_to_biggest_file(group),
     'eog': lambda args, group: call(['eog'] + [str(pic) for pic in group]),  # nosec
     'xv': lambda args, group: call(['xv', '-nolim'] + [str(pic) for pic in group]),  # nosec
     'print': lambda args, group: print(*group),
     'print_inline': lambda args, group: print(*group, end=' '),
     'quote': lambda args, group: print(' '.join([quote(str(pic)) for pic in group])),
     'quote_inline': lambda args, group: print(
         ' '.join([quote(str(pic)) for pic in group]), end=' '
```

### Comparing `duplicate_images-0.9.1/duplicate_images/pair_finder_options.py` & `duplicate_images-0.9.2/duplicate_images/pair_finder_options.py`

 * *Files identical despite different names*

### Comparing `duplicate_images-0.9.1/duplicate_images/parse_commandline.py` & `duplicate_images-0.9.2/duplicate_images/parse_commandline.py`

 * *Files identical despite different names*

### Comparing `duplicate_images-0.9.1/duplicate_images/progress_bar_manager.py` & `duplicate_images-0.9.2/duplicate_images/progress_bar_manager.py`

 * *Files identical despite different names*

### Comparing `duplicate_images-0.9.1/pyproject.toml` & `duplicate_images-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "duplicate_images"
-version = "0.9.1"
+version = "0.9.2"
 description = "Finds equal or similar images in a directory containing (many) image files"
 authors = ["Lene Preuss <lene.preuss@gmail.com>"]
 repository = "https://github.com/lene/DuplicateImages.git"
 homepage = "https://github.com/lene/DuplicateImages"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `duplicate_images-0.9.1/PKG-INFO` & `duplicate_images-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplicate_images
-Version: 0.9.1
+Version: 0.9.2
 Summary: Finds equal or similar images in a directory containing (many) image files
 Home-page: https://github.com/lene/DuplicateImages
 Author: Lene Preuss
 Author-email: lene.preuss@gmail.com
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -118,16 +118,17 @@
 
 ### Actions for matching image groups
 
 Use the `--on-equal` option to select what to do to pairs of equal images. The default action is 
 `print`.
 - `delete-first` or `d1`: deletes the first of the files in the group
 - `delete-last` or `dl`: deletes the last of the files in the group
-- `delete-bigger` or `d>`: deletes the file with the biggest size
-- `delete-smaller` or `d<`: deletes the file with the smallest size
+- `delete-biggest` or `d>`: deletes the file with the biggest size
+- `delete-smallest` or `d<`: deletes the file with the smallest size
+- `symlink-smaller`: delete the smaller files and replace them to a symlink to the biggest file
 - `eog`: launches the `eog` image viewer to compare the files in the group (*deprecated* by `exec`)
 - `xv`: launches the `xv` image viewer to compare the files in the group (*deprecated* by `exec`)
 - `print`: prints the files in the group
 - `print_inline`: like `print` but without newline
 - `quote`: prints the files in the group quoted for POSIX shells
 - `quote_inline`: like `quote` but without newline
 - `exec`: executes a command (see `--exec` argument below)
```

