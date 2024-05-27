# Comparing `tmp/bleuscore-0.1.2.tar.gz` & `tmp/bleuscore-0.1.3.tar.gz`

## Comparing `bleuscore-0.1.2.tar` & `bleuscore-0.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 bleuscore-0.1.2/Cargo.toml
--rw-r--r--   0     1001      127      575 2024-04-29 15:13:40.000000 bleuscore-0.1.2/.github/workflows/bench_base.yml
--rw-r--r--   0     1001      127     1044 2024-04-29 15:13:40.000000 bleuscore-0.1.2/.github/workflows/bench_pr.yml
--rw-r--r--   0     1001      127      900 2024-04-29 15:13:40.000000 bleuscore-0.1.2/.github/workflows/doc.yml
--rw-r--r--   0     1001      127     5153 2024-04-29 15:13:40.000000 bleuscore-0.1.2/.github/workflows/maturin.yml
--rw-r--r--   0     1001      127     1374 2024-04-29 15:13:40.000000 bleuscore-0.1.2/.github/workflows/rust.yml
--rw-r--r--   0     1001      127      456 2024-04-29 15:13:40.000000 bleuscore-0.1.2/.gitignore
--rw-r--r--   0     1001      127      768 2024-04-29 15:13:40.000000 bleuscore-0.1.2/CHANGELOG.md
--rw-r--r--   0     1001      127     1068 2024-04-29 15:13:40.000000 bleuscore-0.1.2/LICENSE
--rw-r--r--   0     1001      127     4837 2024-04-29 15:13:40.000000 bleuscore-0.1.2/README.md
--rw-r--r--   0     1001      127   302127 2024-04-29 15:13:40.000000 bleuscore-0.1.2/asset/benchmark/n_1.png
--rw-r--r--   0     1001      127   110049 2024-04-29 15:13:40.000000 bleuscore-0.1.2/asset/benchmark/n_100.png
--rw-r--r--   0     1001      127   136288 2024-04-29 15:13:40.000000 bleuscore-0.1.2/asset/benchmark/n_10000.png
--rw-r--r--   0     1001      127   117831 2024-04-29 15:13:40.000000 bleuscore-0.1.2/asset/benchmark/n_100000.png
--rw-r--r--   0     1001      127   351628 2024-04-29 15:13:40.000000 bleuscore-0.1.2/asset/benchmark/simple.png
--rw-r--r--   0     1001      127     4687 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/README.md
--rw-r--r--   0     1001      127   102651 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/bench.png
--rw-r--r--   0     1001      127      624 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/bench.sh
--rw-r--r--   0     1001      127     1742 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/bench_plot.py
--rw-r--r--   0     1001      127     4239 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/result.json
--rw-r--r--   0     1001      127      311 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/simple/hf_evaluate.py
--rw-r--r--   0     1001      127     8385 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/simple/local_hf_bleu.py
--rw-r--r--   0     1001      127      284 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/simple/rs_bleuscore.py
--rw-r--r--   0     1001      127      352 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/simple/sacre_bleu.py
--rw-r--r--   0     1001      127      473 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/simple/util.py
--rw-r--r--   0     1001      127      146 2024-04-29 15:13:40.000000 bleuscore-0.1.2/python/bleuscore/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-29 15:13:40.000000 bleuscore-0.1.2/python/bleuscore/py.typed
--rw-r--r--   0     1001      127       31 2024-04-29 15:13:40.000000 bleuscore-0.1.2/rust-toolchain.toml
--rw-r--r--   0     1001      127     7450 2024-04-29 15:13:40.000000 bleuscore-0.1.2/src/bleu.rs
--rw-r--r--   0     1001      127     2892 2024-04-29 15:13:40.000000 bleuscore-0.1.2/src/lib.rs
--rw-r--r--   0     1001      127     3640 2024-04-29 15:13:40.000000 bleuscore-0.1.2/src/ngram.rs
--rw-r--r--   0     1001      127     4343 2024-04-29 15:13:40.000000 bleuscore-0.1.2/src/tokenizer.rs
--rw-r--r--   0     1001      127      484 2024-04-29 15:13:40.000000 bleuscore-0.1.2/tests/conftest.py
--rw-r--r--   0     1001      127     4897 2024-04-29 15:13:40.000000 bleuscore-0.1.2/tests/py_bleu.py
--rw-r--r--   0     1001      127     3488 2024-04-29 15:13:40.000000 bleuscore-0.1.2/tests/py_token.py
--rw-r--r--   0     1001      127     4463 2024-04-29 15:13:40.000000 bleuscore-0.1.2/tests/test_bleu_score.py
--rw-r--r--   0     1001      127     1318 2024-04-29 15:13:40.000000 bleuscore-0.1.2/tests/test_tokenizer.py
--rw-r--r--   0     1001      127     1074 2024-04-29 15:13:40.000000 bleuscore-0.1.2/tests/util.py
--rw-r--r--   0     1001      127    16044 2024-04-29 15:13:53.000000 bleuscore-0.1.2/Cargo.lock
--rw-r--r--   0     1001      127     1983 2024-04-29 15:13:40.000000 bleuscore-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6362 1970-01-01 00:00:00.000000 bleuscore-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 bleuscore-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      127      575 2024-05-27 03:25:55.000000 bleuscore-0.1.3/.github/workflows/bench_base.yml
+-rw-r--r--   0     1001      127     1044 2024-05-27 03:25:55.000000 bleuscore-0.1.3/.github/workflows/bench_pr.yml
+-rw-r--r--   0     1001      127      900 2024-05-27 03:25:55.000000 bleuscore-0.1.3/.github/workflows/doc.yml
+-rw-r--r--   0     1001      127     5153 2024-05-27 03:25:55.000000 bleuscore-0.1.3/.github/workflows/maturin.yml
+-rw-r--r--   0     1001      127     1374 2024-05-27 03:25:55.000000 bleuscore-0.1.3/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127      456 2024-05-27 03:25:55.000000 bleuscore-0.1.3/.gitignore
+-rw-r--r--   0     1001      127      925 2024-05-27 03:25:55.000000 bleuscore-0.1.3/CHANGELOG.md
+-rw-r--r--   0     1001      127     1068 2024-05-27 03:25:55.000000 bleuscore-0.1.3/LICENSE
+-rw-r--r--   0     1001      127     4837 2024-05-27 03:25:55.000000 bleuscore-0.1.3/README.md
+-rw-r--r--   0     1001      127   302127 2024-05-27 03:25:55.000000 bleuscore-0.1.3/asset/benchmark/n_1.png
+-rw-r--r--   0     1001      127   110049 2024-05-27 03:25:55.000000 bleuscore-0.1.3/asset/benchmark/n_100.png
+-rw-r--r--   0     1001      127   136288 2024-05-27 03:25:55.000000 bleuscore-0.1.3/asset/benchmark/n_10000.png
+-rw-r--r--   0     1001      127   117831 2024-05-27 03:25:55.000000 bleuscore-0.1.3/asset/benchmark/n_100000.png
+-rw-r--r--   0     1001      127   351628 2024-05-27 03:25:55.000000 bleuscore-0.1.3/asset/benchmark/simple.png
+-rw-r--r--   0     1001      127     4687 2024-05-27 03:25:55.000000 bleuscore-0.1.3/benchmark/README.md
+-rw-r--r--   0     1001      127   102651 2024-05-27 03:25:55.000000 bleuscore-0.1.3/benchmark/bench.png
+-rw-r--r--   0     1001      127      624 2024-05-27 03:25:55.000000 bleuscore-0.1.3/benchmark/bench.sh
+-rw-r--r--   0     1001      127     1742 2024-05-27 03:25:55.000000 bleuscore-0.1.3/benchmark/bench_plot.py
+-rw-r--r--   0     1001      127     4239 2024-05-27 03:25:55.000000 bleuscore-0.1.3/benchmark/result.json
+-rw-r--r--   0     1001      127      311 2024-05-27 03:25:55.000000 bleuscore-0.1.3/benchmark/simple/hf_evaluate.py
+-rw-r--r--   0     1001      127     8385 2024-05-27 03:25:55.000000 bleuscore-0.1.3/benchmark/simple/local_hf_bleu.py
+-rw-r--r--   0     1001      127      284 2024-05-27 03:25:55.000000 bleuscore-0.1.3/benchmark/simple/rs_bleuscore.py
+-rw-r--r--   0     1001      127      352 2024-05-27 03:25:55.000000 bleuscore-0.1.3/benchmark/simple/sacre_bleu.py
+-rw-r--r--   0     1001      127      473 2024-05-27 03:25:55.000000 bleuscore-0.1.3/benchmark/simple/util.py
+-rw-r--r--   0     1001      127      146 2024-05-27 03:25:55.000000 bleuscore-0.1.3/python/bleuscore/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-27 03:25:55.000000 bleuscore-0.1.3/python/bleuscore/py.typed
+-rw-r--r--   0     1001      127       31 2024-05-27 03:25:55.000000 bleuscore-0.1.3/rust-toolchain.toml
+-rw-r--r--   0     1001      127     7433 2024-05-27 03:25:55.000000 bleuscore-0.1.3/src/bleu.rs
+-rw-r--r--   0     1001      127     2892 2024-05-27 03:25:55.000000 bleuscore-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      127     2477 2024-05-27 03:25:55.000000 bleuscore-0.1.3/src/ngram.rs
+-rw-r--r--   0     1001      127     4343 2024-05-27 03:25:55.000000 bleuscore-0.1.3/src/tokenizer.rs
+-rw-r--r--   0     1001      127      484 2024-05-27 03:25:55.000000 bleuscore-0.1.3/tests/conftest.py
+-rw-r--r--   0     1001      127     4897 2024-05-27 03:25:55.000000 bleuscore-0.1.3/tests/py_bleu.py
+-rw-r--r--   0     1001      127     3488 2024-05-27 03:25:55.000000 bleuscore-0.1.3/tests/py_token.py
+-rw-r--r--   0     1001      127     4463 2024-05-27 03:25:55.000000 bleuscore-0.1.3/tests/test_bleu_score.py
+-rw-r--r--   0     1001      127     1318 2024-05-27 03:25:55.000000 bleuscore-0.1.3/tests/test_tokenizer.py
+-rw-r--r--   0     1001      127     1074 2024-05-27 03:25:55.000000 bleuscore-0.1.3/tests/util.py
+-rw-r--r--   0     1001      127    15581 2024-05-27 03:26:10.000000 bleuscore-0.1.3/Cargo.lock
+-rw-r--r--   0     1001      127     1982 2024-05-27 03:25:55.000000 bleuscore-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6407 1970-01-01 00:00:00.000000 bleuscore-0.1.3/PKG-INFO
```

### Comparing `bleuscore-0.1.2/.github/workflows/bench_base.yml` & `bleuscore-0.1.3/.github/workflows/bench_base.yml`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/.github/workflows/bench_pr.yml` & `bleuscore-0.1.3/.github/workflows/bench_pr.yml`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/.github/workflows/doc.yml` & `bleuscore-0.1.3/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/.github/workflows/maturin.yml` & `bleuscore-0.1.3/.github/workflows/maturin.yml`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/.github/workflows/rust.yml` & `bleuscore-0.1.3/.github/workflows/rust.yml`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/CHANGELOG.md` & `bleuscore-0.1.3/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.3] - 2024-05-27
+
+### Fixed
+- `ngram` bench use counter lib's function rather than the truly used function.
+
+### Changed
+- Use AHash in ngram module
+
 ## [0.1.2] - 2024-04-29
 
 
 ### Changed
 - Implement ngram counts with a better way (#33)
 - Rust `compute_score` function signature changed to use references (#34)
 - Use rayon to run every prediction-references statistics calculation parallely (#38)
```

### Comparing `bleuscore-0.1.2/LICENSE` & `bleuscore-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/README.md` & `bleuscore-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/asset/benchmark/n_1.png` & `bleuscore-0.1.3/asset/benchmark/n_1.png`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/asset/benchmark/n_100.png` & `bleuscore-0.1.3/asset/benchmark/n_100.png`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/asset/benchmark/n_10000.png` & `bleuscore-0.1.3/asset/benchmark/n_10000.png`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/asset/benchmark/n_100000.png` & `bleuscore-0.1.3/asset/benchmark/n_100000.png`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/asset/benchmark/simple.png` & `bleuscore-0.1.3/asset/benchmark/simple.png`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/benchmark/README.md` & `bleuscore-0.1.3/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/benchmark/bench.png` & `bleuscore-0.1.3/benchmark/bench.png`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/benchmark/bench.sh` & `bleuscore-0.1.3/benchmark/bench.sh`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/benchmark/bench_plot.py` & `bleuscore-0.1.3/benchmark/bench_plot.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/benchmark/result.json` & `bleuscore-0.1.3/benchmark/result.json`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/benchmark/simple/local_hf_bleu.py` & `bleuscore-0.1.3/benchmark/simple/local_hf_bleu.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/src/bleu.rs` & `bleuscore-0.1.3/src/bleu.rs`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             Stat(
                 translation_length,
                 reference_length,
                 possible_matches_by_order,
                 matches_by_order,
             )
         })
-        .reduce_with(|s1, s2| agg_stat(s1, s2));
+        .reduce_with(agg_stat);
 
     let Stat(translation_length, reference_length, possible_matches_by_order, matches_by_order) =
         match stat_result {
             None => panic!("Pair statistics calculation got empty result"),
             Some(stats) => stats,
         };
```

### Comparing `bleuscore-0.1.2/src/lib.rs` & `bleuscore-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/src/tokenizer.rs` & `bleuscore-0.1.3/src/tokenizer.rs`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/tests/py_bleu.py` & `bleuscore-0.1.3/tests/py_bleu.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/tests/py_token.py` & `bleuscore-0.1.3/tests/py_token.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/tests/test_bleu_score.py` & `bleuscore-0.1.3/tests/test_bleu_score.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/tests/test_tokenizer.py` & `bleuscore-0.1.3/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/tests/util.py` & `bleuscore-0.1.3/tests/util.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.2/Cargo.lock` & `bleuscore-0.1.3/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -28,42 +28,41 @@
 name = "allocator-api2"
 version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bleuscore"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "ahash",
  "cached",
- "counter",
  "lazy_static",
  "pyo3",
  "rayon",
  "regex",
 ]
 
 [[package]]
 name = "cached"
-version = "0.50.0"
+version = "0.51.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10a7d38ed2761b8a13ce42bc44b09d5a052b88da2f9fead624c779f31ac0729a"
+checksum = "dd93a9f06ec296ca66b4c26fafa9ed63f32c473d7a708a5f28563ee64c948515"
 dependencies = [
  "ahash",
  "cached_proc_macro",
  "cached_proc_macro_types",
  "hashbrown",
  "instant",
  "once_cell",
@@ -91,23 +90,14 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
-name = "counter"
-version = "0.5.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2d458e66999348f56fd3ffcfbb7f7951542075ca8359687c703de6500c1ddccd"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
 dependencies = [
  "crossbeam-epoch",
  "crossbeam-utils",
@@ -120,70 +110,70 @@
 checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "darling"
-version = "0.20.8"
+version = "0.20.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
+checksum = "83b2eb4d90d12bdda5ed17de686c2acb4c57914f8f921b8da7e112b5a36f3fe1"
 dependencies = [
  "darling_core",
  "darling_macro",
 ]
 
 [[package]]
 name = "darling_core"
-version = "0.20.8"
+version = "0.20.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
+checksum = "622687fe0bac72a04e5599029151f5796111b90f1baaa9b544d807a5e31cd120"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
  "syn",
 ]
 
 [[package]]
 name = "darling_macro"
-version = "0.20.8"
+version = "0.20.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
+checksum = "733cabb43482b1a1b53eee8583c2b9e8684d592215ea83efd305dd31bc2f0178"
 dependencies = [
  "darling_core",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "either"
-version = "1.11.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -212,32 +202,32 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "instant"
-version = "0.1.12"
+version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
+checksum = "e0242819d153cba4b4b05a5a8f2a7e9bbf97b6055b2a002b395c96b5ff3c0222"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
@@ -257,33 +247,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "num-traits"
-version = "0.2.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.2"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
@@ -302,17 +283,17 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.21.2"
@@ -453,49 +434,49 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "strsim"
-version = "0.10.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.59"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.59"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -584,24 +565,24 @@
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "zerocopy"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
```

### Comparing `bleuscore-0.1.2/pyproject.toml` & `bleuscore-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 authors = [
     {name = 'Mathew Shen', email = 'datahonor@gmail.com'},
 ]
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
-#    "Development Status :: 5 - Production/Stable",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `bleuscore-0.1.2/PKG-INFO` & `bleuscore-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.3
 Name: bleuscore
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,15 +21,15 @@
 Requires-Dist: evaluate ; extra == 'test'
 Requires-Dist: sacrebleu ; extra == 'test'
 Requires-Dist: black ; extra == 'lint'
 Requires-Dist: ruff ~=0.3.7 ; extra == 'lint'
 Provides-Extra: test
 Provides-Extra: lint
 License-File: LICENSE
-Summary: A fast(not yet :) bleu score calculator
+Summary: A fast bleu score calculator
 Keywords: NLP,Tokenizer,BLEU,DeepLearning
 Author: Mathew Shen <datahonor@gmail.com>
 Author-email: Mathew Shen <datahonor@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://github.com/shenxiangzhuang/bleuscore
```

