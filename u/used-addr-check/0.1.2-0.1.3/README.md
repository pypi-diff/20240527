# Comparing `tmp/used_addr_check-0.1.2.tar.gz` & `tmp/used_addr_check-0.1.3.tar.gz`

## Comparing `used_addr_check-0.1.2.tar` & `used_addr_check-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/.cspell/custom-dictionary-workspace.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/.vscode/extensions.json
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/.vscode/settings.json
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/__main__.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/cli.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/download_list.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/index_create.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/index_search.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/index_types.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/scan_file.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/tests/test_1.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/tests/test_scan_file.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/tests/test_data/scan_file_sample_1.txt
--rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/tests/test_data/scan_file_sample_2.txt
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/LICENSE
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/.cspell/custom-dictionary-workspace.txt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/.vscode/extensions.json
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/__main__.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/cli.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/download_list.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/index_create.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/index_search.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/index_types.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/scan_file.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/tests/test_1.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/tests/test_scan_file.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/tests/test_data/scan_file_sample_1.txt
+-rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/tests/test_data/scan_file_sample_2.txt
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/PKG-INFO
```

### Comparing `used_addr_check-0.1.2/.vscode/settings.json` & `used_addr_check-0.1.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.2/src/used_addr_check/cli.py` & `used_addr_check-0.1.3/src/used_addr_check/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 # from used_addr_check.download_list import download_list, BITCOIN_LIST_URL
+from used_addr_check import __VERSION__
 from used_addr_check.index_create import load_or_generate_index
 from used_addr_check.index_search import search_multiple_in_file
 from used_addr_check.scan_file import scan_file_for_used_addresses
 
 import argparse
+import sys
 from pathlib import Path
 
 
 def main_cli():
     parser = argparse.ArgumentParser(
         description="CLI for file processing and searching"
     )
+    parser.add_argument(
+        "-V",
+        "--version",
+        dest="version",
+        action="store_true",
+        help="Print version to stdout and exit",
+    )
     subparsers = parser.add_subparsers(dest="command")
 
     # # Subparser for the 'download' command
     # download_parser = subparsers.add_parser(
     #     "download", help="Download the file"
     # )
     # download_parser.add_argument(
@@ -28,14 +37,20 @@
     #     "-u",
     #     "--url",
     #     dest="url",
     #     default=BITCOIN_LIST_URL,
     #     help="URL to download the file from",
     # )
 
+    # Subparser for the 'version' command (subparser not really used)
+    subparsers.add_parser(
+        "version",
+        help="Print version to stdout and exit",
+    )
+
     # Subparser for the 'index' command
     index_parser = subparsers.add_parser(
         "index",
         help="Index a haystack 'used addresses' file, save it to orig_name.txt.index.json",  # noqa
     )
     index_parser.add_argument(
         "-f",
@@ -82,15 +97,18 @@
         required=True,
         help="Needle file path, with list of addresses. Addresses will be "
         "extracted from this file",
     )
 
     args = parser.parse_args()
 
-    if args.command == "index":
+    if args.command == "version" or args.version:
+        print(f"used_addr_scan version v{__VERSION__}")
+        sys.exit(0)
+    elif args.command == "index":
         load_or_generate_index(
             haystack_file_path=Path(args.haystack_file_path),
             force_recreate=True,
         )
     elif args.command == "search":
         search_multiple_in_file(Path(args.haystack_file_path), args.needles)
     # elif args.command == "download":
```

### Comparing `used_addr_check-0.1.2/src/used_addr_check/download_list.py` & `used_addr_check-0.1.3/src/used_addr_check/download_list.py`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.2/src/used_addr_check/index_create.py` & `used_addr_check-0.1.3/src/used_addr_check/index_create.py`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.2/src/used_addr_check/index_search.py` & `used_addr_check-0.1.3/src/used_addr_check/index_search.py`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.2/src/used_addr_check/scan_file.py` & `used_addr_check-0.1.3/src/used_addr_check/scan_file.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from used_addr_check.index_search import search_multiple_in_file
 
 
 # BITCOIN_ADDR_REGEX = r"[13][a-km-zA-HJ-NP-Z1-9]{25,34}"
 
 # Source: https://ihateregex.io/expr/bitcoin-address/
-BITCOIN_ADDR_REGEX = r"((bc1|[13])[a-zA-HJ-NP-Z0-9]{25,39})"
+BITCOIN_ADDR_REGEX = r"\b((bc1|[13])[a-zA-HJ-NP-Z0-9]{25,39})\b"
 
 
 def _extract_addresses_from_file_python_re(text_file_path: Path) -> List[str]:
     """
     Extracts bitcoin addresses from a file using Python regex.
 
     Args:
@@ -101,15 +101,17 @@
 
         elif searcher == "python_re":
             return _extract_addresses_from_file_python_re(text_file_path)
 
         else:
             raise ValueError(f"Invalid searcher provided: {searcher}")
 
-    raise Exception("This should never be reached.")
+    raise Exception(
+        "This should never be reached. Address extraction has failed."
+    )
 
 
 def scan_file_for_used_addresses(
     haystack_file_path: Path, needle_file_path: Path
 ):
     """
     Scans a file for bitcoin addresses, and see which one have been used.
@@ -122,11 +124,24 @@
     assert isinstance(haystack_file_path, Path)
     assert isinstance(needle_file_path, Path)
 
     needle_addresses = extract_addresses_from_file(needle_file_path)
     logger.info(
         f"Extracted {len(needle_addresses):,} addresses from the needle file"
     )
+
+    # remove duplicates (get distinct addresses)
+    count_before_distinct = len(needle_addresses)
+    needle_addresses = list(set(needle_addresses))
+    count_after_distinct = len(needle_addresses)
+    addr_count_change = count_after_distinct - count_before_distinct  # neg
+    if addr_count_change != 0:
+        logger.info(
+            "By removing duplicates, address count changed "
+            f"from {count_before_distinct:,} to {count_after_distinct:,}"
+            f" ({addr_count_change:,} addresses)."
+        )
+
     matched_addresses = search_multiple_in_file(
         haystack_file_path, needle_addresses
     )
     logger.info(f"Found {len(matched_addresses):,} used addresses in the file")
```

### Comparing `used_addr_check-0.1.2/tests/test_scan_file.py` & `used_addr_check-0.1.3/tests/test_scan_file.py`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.2/tests/test_data/scan_file_sample_1.txt` & `used_addr_check-0.1.3/tests/test_data/scan_file_sample_1.txt`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.2/tests/test_data/scan_file_sample_2.txt` & `used_addr_check-0.1.3/tests/test_data/scan_file_sample_2.txt`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.2/.gitignore` & `used_addr_check-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.2/LICENSE` & `used_addr_check-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.2/README.md` & `used_addr_check-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.2/pyproject.toml` & `used_addr_check-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "used_addr_check"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     { name="RecRanger", email="RecRanger+package@proton.me" },
 ]
 description = "A tool to efficiently check if a Bitcoin Address has ever been used before"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `used_addr_check-0.1.2/PKG-INFO` & `used_addr_check-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: used_addr_check
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool to efficiently check if a Bitcoin Address has ever been used before
 Project-URL: Homepage, https://github.com/RecRanger/used-addr-check
 Project-URL: Issues, https://github.com/RecRanger/used-addr-check/issues
 Author-email: RecRanger <RecRanger+package@proton.me>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

