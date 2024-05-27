# Comparing `tmp/python_text_cleaning-0.1.6.tar.gz` & `tmp/python_text_cleaning-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_text_cleaning-0.1.6.tar", max compression
+gzip compressed data, was "python_text_cleaning-0.1.7.tar", max compression
```

## Comparing `python_text_cleaning-0.1.6.tar` & `python_text_cleaning-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2024-04-30 09:27:20.046862 python_text_cleaning-0.1.6/LICENSE
--rw-r--r--   0        0        0      759 2024-04-30 09:27:20.046862 python_text_cleaning-0.1.6/README.md
--rw-r--r--   0        0        0      765 2024-04-30 09:27:31.211032 python_text_cleaning-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       73 2024-04-30 09:27:20.046862 python_text_cleaning-0.1.6/python_text_cleaning/__init__.py
--rw-r--r--   0        0        0     3883 2024-04-30 09:27:20.046862 python_text_cleaning-0.1.6/python_text_cleaning/asr_text_cleaning.py
--rw-r--r--   0        0        0      281 2024-04-30 09:27:20.046862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/__init__.py
--rw-r--r--   0        0        0      872 2024-04-30 09:27:20.046862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/cyrillic_character_maps.py
--rw-r--r--   0        0        0      954 2024-04-30 09:27:20.050862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/german_text_cleaners.py
--rw-r--r--   0        0        0     2111 2024-04-30 09:27:20.050862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/latin_character_maps.py
--rw-r--r--   0        0        0     2182 2024-04-30 09:27:20.050862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/misc_language_text_cleaners.py
--rw-r--r--   0        0        0      219 2024-04-30 09:27:20.050862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/not_str_translatable_maps.py
--rw-r--r--   0        0        0     3305 2024-04-30 09:27:20.050862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/text_cleaning.py
--rw-r--r--   0        0        0     1346 2024-04-30 09:27:20.050862 python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/todo.md
--rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 python_text_cleaning-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-27 15:45:15.146285 python_text_cleaning-0.1.7/LICENSE
+-rw-r--r--   0        0        0      759 2024-05-27 15:45:15.146285 python_text_cleaning-0.1.7/README.md
+-rw-r--r--   0        0        0      765 2024-05-27 15:45:26.494305 python_text_cleaning-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-05-27 15:45:15.146285 python_text_cleaning-0.1.7/python_text_cleaning/__init__.py
+-rw-r--r--   0        0        0     4018 2024-05-27 15:45:15.146285 python_text_cleaning-0.1.7/python_text_cleaning/asr_text_cleaning.py
+-rw-r--r--   0        0        0      281 2024-05-27 15:45:15.146285 python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-27 15:45:15.146285 python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/cyrillic_character_maps.py
+-rw-r--r--   0        0        0      954 2024-05-27 15:45:15.146285 python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/german_text_cleaners.py
+-rw-r--r--   0        0        0     2111 2024-05-27 15:45:15.146285 python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/latin_character_maps.py
+-rw-r--r--   0        0        0     2182 2024-05-27 15:45:15.146285 python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/misc_language_text_cleaners.py
+-rw-r--r--   0        0        0      219 2024-05-27 15:45:15.146285 python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/not_str_translatable_maps.py
+-rw-r--r--   0        0        0     3305 2024-05-27 15:45:15.146285 python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/text_cleaning.py
+-rw-r--r--   0        0        0     1346 2024-05-27 15:45:15.146285 python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/todo.md
+-rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 python_text_cleaning-0.1.7/PKG-INFO
```

### Comparing `python_text_cleaning-0.1.6/LICENSE` & `python_text_cleaning-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.6/README.md` & `python_text_cleaning-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.6/pyproject.toml` & `python_text_cleaning-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-text-cleaning"
-version = "0.1.6"
+version = "0.1.7"
 description = "mostly mapping characters"
 authors = ["Tilo Himmelsbach <dertilo@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/dertilo/python-text-cleaning"
 
 packages = [{ include = "python_text_cleaning" }]
```

### Comparing `python_text_cleaning-0.1.6/python_text_cleaning/asr_text_cleaning.py` & `python_text_cleaning-0.1.7/python_text_cleaning/asr_text_cleaning.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import re
 from collections.abc import Callable
 from dataclasses import dataclass
-from enum import Enum, auto
-from typing import TypeVar
+from enum import Enum
+
+from typing_extensions import Self
 
 from python_text_cleaning.character_mappings.text_cleaning import (
     TEXT_CLEANERS,
     NeStr,
     TextCleaner,
 )
 
-TCasing = TypeVar("TCasing", bound="Casing")  # is this really the recommended way?
-
 
-class Casing(str, Enum):
-    lower = auto()
-    upper = auto()
-    original = auto()
+class Casing(Enum):
+    LOWER = "LOWER"
+    UPPER = "UPPER"
+    original = "ORIGINAL"
 
-    def _to_dict(self, skip_keys: list[str] | None = None) -> dict:
+    def _to_dict(self, skip_keys: list[str] | None = None) -> dict[str, str]:
         obj = self
         module = obj.__class__.__module__
         _target_ = f"{module}.{obj.__class__.__name__}"
         # TODO: WTF? why _target_ and _id_ stuff here?
         d = {"_target_": _target_, "value": self.value, "_id_": str(id(self))}
         skip_keys = skip_keys if skip_keys is not None else []
         return {k: v for k, v in d.items() if k not in skip_keys}
@@ -31,25 +30,26 @@
         if self in CASING_FUNS.keys():
             fun = CASING_FUNS[self](text)
         else:  # noqa: RET505
             msg = "unknown Casing"
             raise AssertionError(msg)
         return fun
 
-    @staticmethod
-    def create(value: str | int) -> TCasing:
-        """
-        # TODO: this is only necessary if someone else mis-interprets "1" as an integer! pythons json lib does it correctly -> somewhere in jina??
-        """
-        return Casing(str(value))
+    @classmethod
+    def create(cls, value: str | dict[str, str]) -> Self:
+        if isinstance(value, dict):
+            value = value["value"]
+        elif value.startswith("Casing."):
+            value = value.split(".")[1]
+        return cls(value)
 
 
-CASING_FUNS: dict[Casing, Callable] = {
-    Casing.upper: lambda s: s.upper(),
-    Casing.lower: lambda s: s.lower(),
+CASING_FUNS: dict[Casing, Callable[[str], str]] = {
+    Casing.UPPER: lambda s: s.upper(),
+    Casing.LOWER: lambda s: s.lower(),
     Casing.original: lambda s: s,
 }
 
 
 Letters = NeStr
 
 
@@ -63,37 +63,38 @@
 #     text: str, vocab_letters: list[str], casing: Casing = Casing.original
 # ) -> str:
 #     return filter_by_lettervocab(casing.apply(text), vocab_letters)
 
 
 @dataclass
 class VocabCasingAwareTextCleaner(TextCleaner):
-    casing: str | dict | Casing
+    casing: str | dict[str, str] | Casing
     text_cleaner_name: str
     letter_vocab: Letters
 
     @property
     def name(self) -> NeStr:
+        assert isinstance(self.casing, Casing)
         return f"{self.casing.name}-{self.text_cleaner_name}"
 
     def __post_init__(self) -> None:
         if isinstance(self.casing, str):
             self.casing = Casing(self.casing)
         elif isinstance(
-            self.casing,
-            dict,
+            self.casing, dict  # noqa: COM812
         ):  # TODO: somehow Casing gets not deserialized properly!
-            self.casing = Casing.create(int(self.casing["value"]))
+            self.casing = Casing.create(self.casing["value"])
 
     def __call__(self, text: str) -> str:
+        assert isinstance(self.casing, Casing)
         text = clean_and_filter_text(
-            text,
-            self.letter_vocab,
-            TEXT_CLEANERS[self.text_cleaner_name],
-            self.casing,
+            text=text,
+            vocab_letters=self.letter_vocab,
+            text_cleaner=TEXT_CLEANERS[self.text_cleaner_name],
+            casing=self.casing,
         )
         assert "  " not in text, f"{text=}"
         return text
 
 
 def clean_and_filter_text(
     text: str,
@@ -125,8 +126,12 @@
     return casing.apply(text)
 
 
 def determine_casing(letter_vocab: Letters) -> Casing:
     more_than_half_is_upper = (
         sum([1 if c.upper() == c else 0 for c in letter_vocab]) > len(letter_vocab) / 2
     )
-    return Casing.upper if more_than_half_is_upper else Casing.lower
+    return Casing.UPPER if more_than_half_is_upper else Casing.LOWER
+
+
+if __name__ == "__main__":
+    print(Casing.LOWER)  # noqa: T201
```

### Comparing `python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/cyrillic_character_maps.py` & `python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/cyrillic_character_maps.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/german_text_cleaners.py` & `python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/german_text_cleaners.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/latin_character_maps.py` & `python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/latin_character_maps.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/misc_language_text_cleaners.py` & `python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/misc_language_text_cleaners.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/text_cleaning.py` & `python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/text_cleaning.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.6/python_text_cleaning/character_mappings/todo.md` & `python_text_cleaning-0.1.7/python_text_cleaning/character_mappings/todo.md`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.6/PKG-INFO` & `python_text_cleaning-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-text-cleaning
-Version: 0.1.6
+Version: 0.1.7
 Summary: mostly mapping characters
 Home-page: https://github.com/dertilo/python-text-cleaning
 Author: Tilo Himmelsbach
 Author-email: dertilo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

