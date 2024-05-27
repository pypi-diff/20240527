# Comparing `tmp/semantic_versioning-0.1.5.tar.gz` & `tmp/semantic-versioning-0.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_versioning-0.1.5.tar", last modified: Mon May 27 12:49:41 2024, max compression
+gzip compressed data, was "semantic-versioning-0.2.0.dev0.tar", last modified: Sun Dec 10 21:50:13 2023, max compression
```

## Comparing `semantic_versioning-0.1.5.tar` & `semantic-versioning-0.2.0.dev0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:49:41.712797 semantic_versioning-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-27 12:49:36.000000 semantic_versioning-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-27 12:49:41.712797 semantic_versioning-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-27 12:49:36.000000 semantic_versioning-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-27 12:49:36.000000 semantic_versioning-0.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:49:41.712797 semantic_versioning-0.1.5/semantic_versioning/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 12:49:36.000000 semantic_versioning-0.1.5/semantic_versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 12:49:36.000000 semantic_versioning-0.1.5/semantic_versioning/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-27 12:49:36.000000 semantic_versioning-0.1.5/semantic_versioning/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-27 12:49:36.000000 semantic_versioning-0.1.5/semantic_versioning/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-27 12:49:36.000000 semantic_versioning-0.1.5/semantic_versioning/semantic_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-27 12:49:36.000000 semantic_versioning-0.1.5/semantic_versioning/specifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-27 12:49:36.000000 semantic_versioning-0.1.5/semantic_versioning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:49:41.712797 semantic_versioning-0.1.5/semantic_versioning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-27 12:49:41.000000 semantic_versioning-0.1.5/semantic_versioning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-27 12:49:41.000000 semantic_versioning-0.1.5/semantic_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:49:41.000000 semantic_versioning-0.1.5/semantic_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-27 12:49:41.000000 semantic_versioning-0.1.5/semantic_versioning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 12:49:41.000000 semantic_versioning-0.1.5/semantic_versioning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:49:41.712797 semantic_versioning-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:49:41.712797 semantic_versioning-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-05-27 12:49:36.000000 semantic_versioning-0.1.5/tests/test_semantic_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 21:50:13.297934 semantic-versioning-0.2.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-12-10 21:50:05.000000 semantic-versioning-0.2.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2023-12-10 21:50:13.297934 semantic-versioning-0.2.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2023-12-10 21:50:05.000000 semantic-versioning-0.2.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-12-10 21:50:05.000000 semantic-versioning-0.2.0.dev0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 21:50:13.293934 semantic-versioning-0.2.0.dev0/semantic_versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-10 21:50:05.000000 semantic-versioning-0.2.0.dev0/semantic_versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-10 21:50:05.000000 semantic-versioning-0.2.0.dev0/semantic_versioning/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-10 21:50:05.000000 semantic-versioning-0.2.0.dev0/semantic_versioning/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2023-12-10 21:50:05.000000 semantic-versioning-0.2.0.dev0/semantic_versioning/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2023-12-10 21:50:05.000000 semantic-versioning-0.2.0.dev0/semantic_versioning/semantic_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2023-12-10 21:50:05.000000 semantic-versioning-0.2.0.dev0/semantic_versioning/specifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2023-12-10 21:50:05.000000 semantic-versioning-0.2.0.dev0/semantic_versioning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 21:50:13.297934 semantic-versioning-0.2.0.dev0/semantic_versioning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2023-12-10 21:50:13.000000 semantic-versioning-0.2.0.dev0/semantic_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2023-12-10 21:50:13.000000 semantic-versioning-0.2.0.dev0/semantic_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 21:50:13.000000 semantic-versioning-0.2.0.dev0/semantic_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-10 21:50:13.000000 semantic-versioning-0.2.0.dev0/semantic_versioning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-10 21:50:13.000000 semantic-versioning-0.2.0.dev0/semantic_versioning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-10 21:50:13.297934 semantic-versioning-0.2.0.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 21:50:13.297934 semantic-versioning-0.2.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2023-12-10 21:50:05.000000 semantic-versioning-0.2.0.dev0/tests/test_semantic_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2023-12-10 21:50:05.000000 semantic-versioning-0.2.0.dev0/tests/test_specifier.py
```

### Comparing `semantic_versioning-0.1.5/LICENSE` & `semantic-versioning-0.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic_versioning-0.1.5/PKG-INFO` & `semantic-versioning-0.2.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-versioning
-Version: 0.1.5
+Version: 0.2.0.dev0
 Summary: A package for easily managing Semantic versions as described in PEP440.
 Maintainer-email: Jesse de Ruijter <jessederuijter@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `semantic_versioning-0.1.5/README.md` & `semantic-versioning-0.2.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `semantic_versioning-0.1.5/pyproject.toml` & `semantic-versioning-0.2.0.dev0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -18,22 +18,25 @@
 packages.find.include = ["semantic_versioning*"]
 dynamic.version.attr = "semantic_versioning._version.__version__"
 
 [tool.black]
 line-length = 99
 
 [tool.ruff]
-target-version = "py310"
 line-length = 99
+target-version = "py310"
+select = ["ALL"]
+ignore = ["ANN101", "ANN102", "D100", "D101", "PERF203"]
+ignore-init-module-imports = true
 
 [tool.ruff.mccabe]
 max-complexity = 10
 
 [tool.ruff.per-file-ignores]
-"tests/*" = ["D102", "PLR2004", "S101"]
+"tests/*" = ["ANN201", "D101", "D102", "D104", "PLR2004", "S101"]
 "semantic_versioning/patterns.py" = ["E501"]
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore",
     "default:::semantic_versioning.*",
 ]
```

### Comparing `semantic_versioning-0.1.5/semantic_versioning/patterns.py` & `semantic-versioning-0.2.0.dev0/semantic_versioning/patterns.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .flags import Operator
 
 POS_NUM = r"(0|[1-9]\d*)"
 VERSION_PATTERN = rf"(?P<major>{POS_NUM})(\.(?P<minor>{POS_NUM}))?(\.(?P<patch>{POS_NUM}))?(?P<versions>(\.{POS_NUM})*)?"
 RELEASE_PATTERN = rf"((?P<pre_release_type>a|b|rc)(?P<pre_release>{POS_NUM}))?((\.|-|_)post(?P<post_release>{POS_NUM}))?((\.|-|_)dev(?P<dev_release>{POS_NUM}))?"
 FULL_VERSION_PATTERN = rf"{VERSION_PATTERN}{RELEASE_PATTERN}"
 
-OPERATOR_PATTERN = " | ".join(str(Operator))
-EXPRESSION_PATTERN = rf"(?P<operator>{OPERATOR_PATTERN})(?P<version>{FULL_VERSION_PATTERN})"
+OPERATOR_PATTERN = "|".join([operator.value for operator in Operator])
+EXPRESSION_PATTERN = rf"(?P<operator>{(OPERATOR_PATTERN)})(?P<version>{FULL_VERSION_PATTERN})"
```

### Comparing `semantic_versioning-0.1.5/semantic_versioning/semantic_version.py` & `semantic-versioning-0.2.0.dev0/semantic_versioning/semantic_version.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,72 +11,77 @@
 
 INT_TYPES = ["major", "minor", "patch", "pre_release", "post_release", "dev_release"]
 
 
 @dataclass
 @total_ordering
 class SemanticVersion:
+    """A version object."""
+
     major: int
-    minor: int | None = None
-    patch: int | None = None
+    minor: int | Literal["*"] | None = None
+    patch: int | Literal["*"] | None = None
     versions: list[int] = field(default_factory=list)
     pre_release_type: Literal["a", "b", "rc"] | None = None
-    pre_release: int | None = None
-    post_release: int | None = None
-    dev_release: int | None = None
+    pre_release: int | Literal["*"] | None = None
+    post_release: int | Literal["*"] | None = None
+    dev_release: int | Literal["*"] | None = None
 
     @classmethod
     def parse(cls: type[SemanticVersion], version: str, separator: str = ".") -> SemanticVersion:
         """Initialize a Semanticversion parsed from a string.
 
-        Args:
+        Attributes
+        ----------
             cls (type[SemanticVersion]): the SemanticVersion class.
             version (str): the version string to parse.
             separator (str): the charachter between the major, minor and patch versions.
 
-        Raises:
+        Raises
+        ------
             ValueError: Couldn't parse the version.
 
-        Returns:
+        Returns
+        -------
             SemanticVersion: a SemanticVersion object.
         """
         if separator != ".":
-            version = version.replace(separator, ".")
+            version.replace(separator, ".")
 
         if not (match := re.fullmatch(re.compile(FULL_VERSION_PATTERN), version)):
             msg = (
                 f"Invalid format for semantic version {version!r}.",
                 "Only X.X.X(.devX) or with other separator allowed.",
             )
             raise AssertionError(msg)
 
         version_dict = {}
         for k, v in match.groupdict().items():
             if not v:
                 continue
-
             if k in INT_TYPES:
-                v = int(v)
+                version_dict[k] = int(v)
             elif k == "versions":
-                v = [int(w) for w in v.split(".") if w]
-            version_dict[k] = v
+                version_dict[k] = [int(w) for w in v.split(".") if w]
 
         return cls(**version_dict)
 
-    def to_string(self, separator=".") -> str:
+    def to_string(self, separator: str = ".") -> str:
         """Convert version to a string separated with dots.
 
-        Args:
+        Attributes
+        ----------
             separator (str): the charachter between the major, minor and patch versions.
 
-        Returns:
+        Returns
+        -------
             str: version string.
         """
         version = str(self.major)
-        for v in [self.minor, self.patch] + self.versions:
+        for v in [self.minor, self.patch, *self.versions]:
             if v or v == 0:
                 version += f".{v}"
         if self.pre_release is not None:
             version += f"{self.pre_release_type}{self.pre_release}"
         if self.post_release is not None:
             version += f".post{self.post_release}"
         if self.dev_release is not None:
@@ -85,80 +90,85 @@
         if separator != ".":
             version = version.replace(".", separator)
         return version
 
     def __str__(self) -> str:
         """Convert to string, will choose dotted version.
 
-        Returns:
+        Returns
+        -------
             str: dot-separated version string.
         """
         return self.to_string()
 
     @staticmethod
     def validate(version: str) -> bool:
         """Validate if a string complies to semantic version form.
 
-        Args:
+        Attributes
+        ----------
             version (str): version to validate.
 
-        Returns:
+        Returns
+        -------
             bool: if it is a valid semantic version.
         """
         pattern = re.compile(FULL_VERSION_PATTERN)
         return bool(re.fullmatch(pattern, version))
 
     def __eq__(self, other: SemanticVersion) -> bool:
         """Compare with another SemanticVersion if equal.
 
-        Args:
-            other (Any): version to compare with.
+        Attributes
+        ----------
+            other (SemanticVersion): version to compare with.
 
-        Returns:
+        Returns
+        -------
             bool: if the versions are equal.
         """
-        return (
-            isinstance(other, SemanticVersion)
-            and self.major == other.major
-            and self.minor == other.minor
-            and self.patch == other.patch
-            and self.versions == other.versions
-            and self.pre_release_type == other.pre_release_type
-            and self.pre_release == other.pre_release
-            and self.post_release == other.post_release
-            and self.dev_release == other.dev_release
+        return isinstance(other, SemanticVersion) and all(
+            self._equal_attribute(other, attribute)
+            for attribute in [*INT_TYPES, "versions", "pre_release_type"]
         )
 
+    def _equal_attribute(self, other: SemanticVersion, attribute: str) -> bool:
+        self_attribute = getattr(self, attribute)
+        other_attribute = getattr(other, attribute)
+        if self_attribute == "*" or other_attribute == "*":
+            return True
+        return self_attribute == other_attribute
+
     def __lt__(self, other: SemanticVersion) -> bool:
         """Compare with another SemanticVersion if smaller.
 
-        Args:
+        Attributes
+        ----------
             other (Any): version to compare with.
 
-        Returns:
+        Returns
+        -------
             bool: if the version is smaller than other.
         """
         versions_length = max(len(self.versions or []), len(other.versions or []))
         return self.__compare_tuple(self, versions_length) < self.__compare_tuple(
-            other, versions_length
+            other,
+            versions_length,
         )
 
     @staticmethod
     def __compare_tuple(v: SemanticVersion, v_length: int) -> tuple:
-        ct = (
+        pre_release_version = pre_release_type_to_int(v.pre_release_type)
+        return (
             v.major,
             v.minor if v.minor is not None else math.inf,
             v.patch if v.patch is not None else math.inf,
             *pad(v.versions, v_length, math.inf),
-            pre_release_type_to_int(v.pre_release_type) or math.inf
-            if not v.post_release and not v.dev_release
-            else -1,
+            pre_release_version or math.inf if not v.post_release and not v.dev_release else -1,
             v.pre_release or math.inf if not v.post_release and not v.dev_release else -1,
             v.post_release or math.inf if not v.dev_release else -1,
             v.dev_release or math.inf,
         )
-        print(ct)
-        return ct
 
     def __hash__(self) -> int:
         """Override hash to show version dotted notation."""
         return hash(self.to_string())
```

### Comparing `semantic_versioning-0.1.5/semantic_versioning.egg-info/PKG-INFO` & `semantic-versioning-0.2.0.dev0/semantic_versioning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-versioning
-Version: 0.1.5
+Version: 0.2.0.dev0
 Summary: A package for easily managing Semantic versions as described in PEP440.
 Maintainer-email: Jesse de Ruijter <jessederuijter@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `semantic_versioning-0.1.5/tests/test_semantic_version.py` & `semantic-versioning-0.2.0.dev0/tests/test_semantic_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,25 +4,46 @@
 
 
 class TestEqualsSemanticVersion(unittest.TestCase):
     def test_equals_correct(self):
         assert SemanticVersion(1, 2, 3) == SemanticVersion(1, 2, 3)
         assert SemanticVersion(1, 2, 3, [1, 2]) == SemanticVersion(1, 2, 3, [1, 2])
         assert SemanticVersion(1, 2, 3, [1, 2], "a", 4, 5, 6) == SemanticVersion(
-            1, 2, 3, [1, 2], "a", 4, 5, 6
+            1,
+            2,
+            3,
+            [1, 2],
+            "a",
+            4,
+            5,
+            6,
         )
 
     def test_equals_incorrect(self):
         assert SemanticVersion(1, 5, 3) != SemanticVersion(1, 2, 3)
         assert SemanticVersion(1, 2, 3, [1, 2]) != SemanticVersion(1, 2, 3, [3, 2])
         assert SemanticVersion(1, 2, 3, [1, 2], "a", 4, 5, 6) != SemanticVersion(
-            1, 2, 3, [1, 2], "b", 4, 5, 6
+            1,
+            2,
+            3,
+            [1, 2],
+            "b",
+            4,
+            5,
+            6,
         )
         assert SemanticVersion(1, 2, 3, [1, 2], "a", 4, 5, 6) != SemanticVersion(
-            1, 2, 3, [1, 2], "a", 7, 5, 6
+            1,
+            2,
+            3,
+            [1, 2],
+            "a",
+            7,
+            5,
+            6,
         )
 
 
 class TestParseSemanticVersion(unittest.TestCase):
     def test_parse_simple_correct(self):
         assert SemanticVersion.parse("1") == SemanticVersion(1)
         assert SemanticVersion.parse("1.0") == SemanticVersion(1, 0)
@@ -30,18 +51,26 @@
         assert SemanticVersion.parse("3.4.1.4") == SemanticVersion(3, 4, 1, [4])
         assert SemanticVersion.parse("3.4.1.4.6") == SemanticVersion(3, 4, 1, [4, 6])
 
     def test_parse_release_correct(self):
         assert SemanticVersion.parse("1-dev1") == SemanticVersion(1, dev_release=1)
         assert SemanticVersion.parse("1.post12") == SemanticVersion(1, post_release=12)
         assert SemanticVersion.parse("1.3a3") == SemanticVersion(
-            1, 3, pre_release_type="a", pre_release=3
+            1,
+            3,
+            pre_release_type="a",
+            pre_release=3,
         )
         assert SemanticVersion.parse("1.3.5a3_dev1") == SemanticVersion(
-            1, 3, 5, pre_release_type="a", pre_release=3, dev_release=1
+            1,
+            3,
+            5,
+            pre_release_type="a",
+            pre_release=3,
+            dev_release=1,
         )
 
 
 class TestValidateSemanticVersion(unittest.TestCase):
     def test_validate_correct(self):
         assert SemanticVersion.validate("0")
         assert SemanticVersion.validate("0.5")
@@ -75,26 +104,36 @@
         assert SemanticVersion(1, 1, 1, [1]) < SemanticVersion(1, 1, 2)
         assert SemanticVersion(1, 1, 1, [1, 1]) < SemanticVersion(1, 1, 1, [2])
         assert SemanticVersion(1, 1, 1, [1, 1]) < SemanticVersion(1, 1, 1, [1, 2])
 
     def test_compare_release_correct(self):
         assert SemanticVersion(1, pre_release_type="a", pre_release=1) < SemanticVersion(1)
         assert SemanticVersion(1, pre_release_type="a", pre_release=1) < SemanticVersion(
-            1, pre_release_type="b", pre_release=1
+            1,
+            pre_release_type="b",
+            pre_release=1,
         )
         assert SemanticVersion(1, pre_release_type="a", pre_release=1) < SemanticVersion(
-            1, pre_release_type="a", pre_release=2
+            1,
+            pre_release_type="a",
+            pre_release=2,
         )
         assert SemanticVersion(1, post_release=1) < SemanticVersion(
-            1, pre_release_type="a", pre_release=1
+            1,
+            pre_release_type="a",
+            pre_release=1,
         )
         assert SemanticVersion(1, dev_release=1) < SemanticVersion(1, post_release=1)
         assert SemanticVersion(1, 0, 0, dev_release=1) < SemanticVersion(1, 0, 0, dev_release=2)
         assert SemanticVersion(1, 0, 0, [1, 1], dev_release=1) < SemanticVersion(
-            1, 0, 0, [1, 1], dev_release=2
+            1,
+            0,
+            0,
+            [1, 1],
+            dev_release=2,
         )
 
 
 class TestStringifySemanticVersion(unittest.TestCase):
     def test_stringify_simple_correct(self):
         assert str(SemanticVersion(1)) == "1"
         assert str(SemanticVersion(1, 12)) == "1.12"
```

