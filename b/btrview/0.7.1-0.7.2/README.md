# Comparing `tmp/btrview-0.7.1.tar.gz` & `tmp/btrview-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrview-0.7.1.tar", last modified: Thu May  9 03:57:34 2024, max compression
+gzip compressed data, was "btrview-0.7.2.tar", last modified: Mon May 27 14:56:52 2024, max compression
```

## Comparing `btrview-0.7.1.tar` & `btrview-0.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-09 03:57:34.010752 btrview-0.7.1/
--rw-r--r--   0 chris     (1000) chris     (1000)     1069 2024-04-18 05:35:32.000000 btrview-0.7.1/LICENSE.md
--rw-r--r--   0 chris     (1000) chris     (1000)     6364 2024-05-09 03:57:34.010752 btrview-0.7.1/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     4352 2024-05-09 03:55:16.000000 btrview-0.7.1/README.md
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-09 03:57:34.010752 btrview-0.7.1/btrview/
--rw-r--r--   0 chris     (1000) chris     (1000)       88 2024-05-09 03:57:22.000000 btrview-0.7.1/btrview/__init__.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.7.1/btrview/__main__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7839 2024-05-09 03:38:00.000000 btrview-0.7.1/btrview/btrfs.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6906 2024-05-09 03:00:04.000000 btrview-0.7.1/btrview/rich_output.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-09 03:57:34.010752 btrview-0.7.1/btrview/scripts/
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.7.1/btrview/scripts/btrview.py
--rw-r--r--   0 chris     (1000) chris     (1000)     4534 2024-05-09 03:38:00.000000 btrview-0.7.1/btrview/subvolume.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3217 2024-05-09 03:38:00.000000 btrview-0.7.1/btrview/typed_info.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-05-07 01:01:20.000000 btrview-0.7.1/btrview/utils.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-09 03:57:34.010752 btrview-0.7.1/btrview.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     6364 2024-05-09 03:57:34.000000 btrview-0.7.1/btrview.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      390 2024-05-09 03:57:34.000000 btrview-0.7.1/btrview.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-09 03:57:34.000000 btrview-0.7.1/btrview.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-05-09 03:57:34.000000 btrview-0.7.1/btrview.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-05-09 03:57:34.000000 btrview-0.7.1/btrview.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-05-09 03:57:34.000000 btrview-0.7.1/btrview.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)     1215 2024-05-09 03:57:22.000000 btrview-0.7.1/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-05-09 03:57:34.010752 btrview-0.7.1/setup.cfg
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-27 14:56:52.147232 btrview-0.7.2/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1069 2024-04-18 05:35:32.000000 btrview-0.7.2/LICENSE.md
+-rw-r--r--   0 chris     (1000) chris     (1000)     6364 2024-05-27 14:56:52.147232 btrview-0.7.2/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     4352 2024-05-09 03:55:16.000000 btrview-0.7.2/README.md
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-27 14:56:52.147232 btrview-0.7.2/btrview/
+-rw-r--r--   0 chris     (1000) chris     (1000)       88 2024-05-27 14:56:48.000000 btrview-0.7.2/btrview/__init__.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-05-27 14:31:17.000000 btrview-0.7.2/btrview/__main__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7839 2024-05-27 14:55:48.000000 btrview-0.7.2/btrview/btrfs.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6906 2024-05-27 14:31:17.000000 btrview-0.7.2/btrview/rich_output.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-27 14:56:52.147232 btrview-0.7.2/btrview/scripts/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-05-27 14:31:17.000000 btrview-0.7.2/btrview/scripts/btrview.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4534 2024-05-27 14:31:17.000000 btrview-0.7.2/btrview/subvolume.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3462 2024-05-27 14:31:17.000000 btrview-0.7.2/btrview/typed_info.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1278 2024-05-27 14:31:43.000000 btrview-0.7.2/btrview/utils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-27 14:56:52.147232 btrview-0.7.2/btrview.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     6364 2024-05-27 14:56:52.000000 btrview-0.7.2/btrview.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      390 2024-05-27 14:56:52.000000 btrview-0.7.2/btrview.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-27 14:56:52.000000 btrview-0.7.2/btrview.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-05-27 14:56:52.000000 btrview-0.7.2/btrview.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-05-27 14:56:52.000000 btrview-0.7.2/btrview.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-05-27 14:56:52.000000 btrview-0.7.2/btrview.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)     1215 2024-05-27 14:56:48.000000 btrview-0.7.2/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-05-27 14:56:52.147232 btrview-0.7.2/setup.cfg
```

### Comparing `btrview-0.7.1/LICENSE.md` & `btrview-0.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `btrview-0.7.1/PKG-INFO` & `btrview-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.7.1
+Version: 0.7.2
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2024 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `btrview-0.7.1/README.md` & `btrview-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `btrview-0.7.1/btrview/__main__.py` & `btrview-0.7.2/btrview/__main__.py`

 * *Files identical despite different names*

### Comparing `btrview-0.7.1/btrview/btrfs.py` & `btrview-0.7.2/btrview/btrfs.py`

 * *Files identical despite different names*

### Comparing `btrview-0.7.1/btrview/rich_output.py` & `btrview-0.7.2/btrview/rich_output.py`

 * *Files identical despite different names*

### Comparing `btrview-0.7.1/btrview/scripts/btrview.py` & `btrview-0.7.2/btrview/scripts/btrview.py`

 * *Files identical despite different names*

### Comparing `btrview-0.7.1/btrview/subvolume.py` & `btrview-0.7.2/btrview/subvolume.py`

 * *Files identical despite different names*

### Comparing `btrview-0.7.1/btrview/typed_info.py` & `btrview-0.7.2/btrview/typed_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,61 +5,66 @@
 from uuid import UUID
 from dataclasses import dataclass
 
 from btrfsutil import SubvolumeInfo
 
 UUIDS = {"uuid": "UUID",
          "parent_uuid": "Parent UUID",
-         "received_uuid": "Received UUID"}
+         "received_uuid": "Received UUID",}
 
 TIMES = {"otime": "Creation time",
          "rtime": "Receieve time",
          "stime": "Send time",
-         "ctime": None}
+         "ctime": None,}
 
 GENS = {"generation": "Generation",
         "otransid": "Gen at creation",
         "rtransid": "Receive transid",
         "stransid": "Send transid",
-        "ctransid": None}
+        "ctransid": None,}
 
 INTS = {"id": "Subvolume ID",
         "parent_id": "Parent ID",
-        "dir_id": None,
-        "flags": "Flags"}
+        "flags": "Flags",
+        "dir_id": None,}
 
 OTHER = {"name": "Name",
-         "path": "Path"}
+         "path": "Path",}
 
 BTRDICT = {v:k for k,v in (UUIDS | TIMES | GENS | INTS | OTHER).items() if v}
 BASE = {k:v for k,v in BTRDICT.items() if v in ("name","id","uuid")}
 
 @dataclass
 class Generation:
     """A class representing a btrfs generation"""
     generation: int
 
     def __lt__(self, other: Self):
         return self.generation < other.generation
 
 @dataclass(frozen=True)
 class BaseInfo:
+    """Base class for TypedInfo, mainly used to facilitate creating
+    subvolume and snapshot trees for subvolumes not on the filesystem"""
     name: str
     id: int
     uuid: UUID
 
     @classmethod
     def from_deleted(cls, suuid: str) -> "BaseInfo":
+        """Returns a BaseInfo instance from a uuid"""
         uuid = UUID(suuid)
         bi = BaseInfo(suuid, uuid.int, uuid)
         return bi
 
-    def __getitem__(self, key):
-        if key in BASE:
-            return getattr(self, BTRDICT[key])
+    def __getitem__(self, key: str):
+        """Returns the attribute corresponding to the key in BTRDICT"""
+        attr = BTRDICT.get(key)
+        if attr in self.__dataclass_fields__:
+            return getattr(self, attr)
         else:
             return None
 
 @dataclass(frozen=True)
 class TypedInfo(BaseInfo):
     """A wrapper around SubvolumeInfo that adds type hints and convenience methods"""
     name: str
@@ -74,20 +79,25 @@
     generation: Generation
     ctransid: Generation
     otransid: Generation
     stransid: Generation
     rtransid: Generation
     ctime: datetime
     otime: datetime
+    rtime: datetime
+    stime: datetime
 
     @classmethod
     def from_info(cls, path: str, info: SubvolumeInfo):
+        """Returns a TypeInfo instance from a SubvolumeInfo instance"""
         kw_args = {}
         kw_args["path"] = PurePath("/" + path)
         kw_args["name"] = kw_args["path"].name or "<FS_TREE>"
+        kw_args["rtime"] = info.rtime
+        kw_args["stime"] = info.stime
         for attr in info.__match_args__:
             val = getattr(info, attr)
             kw_args[attr] = cls._cast(attr, val)
         return cls(**kw_args)
 
     @classmethod
     def _cast(cls, key: str, value: str|int|bytes) -> None | datetime | UUID | Generation | str:
@@ -99,16 +109,7 @@
             return UUID(value) if value != "0"*32 else None
         elif key in GENS:
             return Generation(value) if value else None
         elif key in INTS:
             return int(value)
         else:
             raise KeyError(f"{key = } can't be cast")
-
-    def __getitem__(self, key: str):
-        if key in BTRDICT:
-            return getattr(self, BTRDICT[key])
-        else:
-            #returns None instead of raising an error
-            #makes it slightly easier to use with Subvolume
-            return None 
-
```

### Comparing `btrview-0.7.1/btrview/utils.py` & `btrview-0.7.2/btrview/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 def run(command: str, **kwargs) -> subprocess.CompletedProcess[str]:
     """Split a string command into tokens, run it, and return its output."""
     tokens = shlex.split(command)
     try:
         out = subprocess.run(tokens, check=True, capture_output=True, 
                              text=True, **kwargs)
     except subprocess.CalledProcessError as e:
+        print(e.stderr)
         raise e
     return out
 
 def get_UUIDs(path: Path) -> set[str]:
     """Return a set of UUIDs on a BTRFS filesystem"""
     UUIDs: set[str] = set()
     out = run(f"btrfs subvolume list -u '{path}'")
```

### Comparing `btrview-0.7.1/btrview.egg-info/PKG-INFO` & `btrview-0.7.2/btrview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.7.1
+Version: 0.7.2
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2024 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `btrview-0.7.1/pyproject.toml` & `btrview-0.7.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btrview"
-version = "0.7.1"
+version = "0.7.2"
 description = "View btrfs snapshot trees"
 readme = "README.md"
 authors = [{name = "Chris Copley"}]
 license = {file = "LICENSE.md"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,15 +29,15 @@
 Issues = "https://github.com/CopOnTheRun/btrview/issues"
 
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.7.1"
+current_version = "0.7.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
```

