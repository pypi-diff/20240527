# Comparing `tmp/beancount_multitool-0.4.1.tar.gz` & `tmp/beancount_multitool-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_multitool-0.4.1.tar", max compression
+gzip compressed data, was "beancount_multitool-0.5.0.tar", max compression
```

## Comparing `beancount_multitool-0.4.1.tar` & `beancount_multitool-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1052 2024-05-13 10:19:52.000000 beancount_multitool-0.4.1/LICENSE
--rw-r--r--   0        0        0     1277 2024-05-25 12:35:01.002912 beancount_multitool-0.4.1/README.md
--rw-r--r--   0        0        0     1834 2024-05-25 12:32:16.709954 beancount_multitool-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      182 2024-05-23 01:27:44.241769 beancount_multitool-0.4.1/src/beancount_multitool/Institution.py
--rw-r--r--   0        0        0     5284 2024-05-24 04:10:42.855202 beancount_multitool-0.4.1/src/beancount_multitool/JABank.py
--rw-r--r--   0        0        0     2268 2024-05-25 12:26:23.651681 beancount_multitool-0.4.1/src/beancount_multitool/MappingDatabase.py
--rw-r--r--   0        0        0     4480 2024-05-24 03:32:40.768342 beancount_multitool-0.4.1/src/beancount_multitool/RakutenBank.py
--rw-r--r--   0        0        0     4781 2024-05-24 03:32:40.768228 beancount_multitool-0.4.1/src/beancount_multitool/RakutenCard.py
--rw-r--r--   0        0        0     5154 2024-05-24 04:06:12.816630 beancount_multitool-0.4.1/src/beancount_multitool/ShinseiBank.py
--rw-r--r--   0        0        0      454 2024-05-19 23:39:41.029470 beancount_multitool-0.4.1/src/beancount_multitool/__init__.py
--rw-r--r--   0        0        0      120 2024-05-20 00:15:30.523620 beancount_multitool-0.4.1/src/beancount_multitool/__main__.py
--rw-r--r--   0        0        0       22 2024-05-25 12:32:24.421178 beancount_multitool-0.4.1/src/beancount_multitool/__version__.py
--rw-r--r--   0        0        0     1567 2024-05-25 09:42:51.099454 beancount_multitool-0.4.1/src/beancount_multitool/as_transaction.py
--rw-r--r--   0        0        0     1684 2024-05-23 14:57:04.901452 beancount_multitool-0.4.1/src/beancount_multitool/cli.py
--rw-r--r--   0        0        0      421 2024-05-24 04:13:04.378795 beancount_multitool-0.4.1/src/beancount_multitool/get_beancount_config.py
--rw-r--r--   0        0        0      557 2024-05-24 03:18:42.671213 beancount_multitool-0.4.1/src/beancount_multitool/get_value.py
--rw-r--r--   0        0        0      654 2024-05-24 03:57:41.742099 beancount_multitool-0.4.1/src/beancount_multitool/read_config.py
--rw-r--r--   0        0        0      387 2024-05-24 07:53:23.172781 beancount_multitool-0.4.1/src/beancount_multitool/tests/test_get_beancount_config.py
--rw-r--r--   0        0        0      553 2024-05-24 07:53:56.206848 beancount_multitool-0.4.1/src/beancount_multitool/tests/test_get_value.py
--rw-r--r--   0        0        0      237 2024-05-24 07:53:33.405873 beancount_multitool-0.4.1/src/beancount_multitool/tests/test_read_config.py
--rw-r--r--   0        0        0     2633 1970-01-01 00:00:00.000000 beancount_multitool-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1052 2024-05-13 10:19:52.000000 beancount_multitool-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1356 2024-05-27 09:15:15.602690 beancount_multitool-0.5.0/README.md
+-rw-r--r--   0        0        0     1895 2024-05-27 09:47:21.240177 beancount_multitool-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      182 2024-05-23 01:27:44.241769 beancount_multitool-0.5.0/src/beancount_multitool/Institution.py
+-rw-r--r--   0        0        0     5284 2024-05-24 04:10:42.855202 beancount_multitool-0.5.0/src/beancount_multitool/JABank.py
+-rw-r--r--   0        0        0     2268 2024-05-25 12:26:23.651681 beancount_multitool-0.5.0/src/beancount_multitool/MappingDatabase.py
+-rw-r--r--   0        0        0     4480 2024-05-24 03:32:40.768342 beancount_multitool-0.5.0/src/beancount_multitool/RakutenBank.py
+-rw-r--r--   0        0        0     4781 2024-05-24 03:32:40.768228 beancount_multitool-0.5.0/src/beancount_multitool/RakutenCard.py
+-rw-r--r--   0        0        0     5154 2024-05-24 04:06:12.816630 beancount_multitool-0.5.0/src/beancount_multitool/ShinseiBank.py
+-rw-r--r--   0        0        0     5365 2024-05-27 08:52:37.416123 beancount_multitool-0.5.0/src/beancount_multitool/SumishinNetBank.py
+-rw-r--r--   0        0        0      545 2024-05-27 08:46:57.774005 beancount_multitool-0.5.0/src/beancount_multitool/__init__.py
+-rw-r--r--   0        0        0      120 2024-05-20 00:15:30.523620 beancount_multitool-0.5.0/src/beancount_multitool/__main__.py
+-rw-r--r--   0        0        0       22 2024-05-27 09:32:57.618008 beancount_multitool-0.5.0/src/beancount_multitool/__version__.py
+-rw-r--r--   0        0        0     1567 2024-05-25 09:42:51.099454 beancount_multitool-0.5.0/src/beancount_multitool/as_transaction.py
+-rw-r--r--   0        0        0     1864 2024-05-27 09:51:27.393341 beancount_multitool-0.5.0/src/beancount_multitool/cli.py
+-rw-r--r--   0        0        0      421 2024-05-24 04:13:04.378795 beancount_multitool-0.5.0/src/beancount_multitool/get_beancount_config.py
+-rw-r--r--   0        0        0      557 2024-05-24 03:18:42.671213 beancount_multitool-0.5.0/src/beancount_multitool/get_value.py
+-rw-r--r--   0        0        0      654 2024-05-24 03:57:41.742099 beancount_multitool-0.5.0/src/beancount_multitool/read_config.py
+-rw-r--r--   0        0        0      387 2024-05-24 07:53:23.172781 beancount_multitool-0.5.0/src/beancount_multitool/tests/test_get_beancount_config.py
+-rw-r--r--   0        0        0      553 2024-05-24 07:53:56.206848 beancount_multitool-0.5.0/src/beancount_multitool/tests/test_get_value.py
+-rw-r--r--   0        0        0      237 2024-05-24 07:53:33.405873 beancount_multitool-0.5.0/src/beancount_multitool/tests/test_read_config.py
+-rw-r--r--   0        0        0     2712 1970-01-01 00:00:00.000000 beancount_multitool-0.5.0/PKG-INFO
```

### Comparing `beancount_multitool-0.4.1/LICENSE` & `beancount_multitool-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.1/README.md` & `beancount_multitool-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,11 +11,12 @@
 The following financial institutions are supported:
 
 * Japan
   * [JA Bank ＪＡネットバンク](https://www.jabank.jp/)
   * [Rakuten Card 楽天カード](https://www.rakuten-card.co.jp/)
   * [Rakuten Bank 楽天銀行](https://www.rakuten-bank.co.jp/)
   * [SBI Shinsei Bank 新生銀行](https://www.sbishinseibank.co.jp/)
+  * [SBI Sumishin Net Bank 住信SBIネット銀行](https://www.netbk.co.jp/)
 
 To get started, see the [documentation](https://rlan.github.io/beancount-multitool).
 
 License: [MIT](LICENSE)
```

### Comparing `beancount_multitool-0.4.1/pyproject.toml` & `beancount_multitool-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "beancount-multitool"
-version = "0.4.1"
+version = "0.5.0"
 description = "A CLI tool that converts financial data to Beancount files"
 authors = ["Rick Lan <rlan@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
+packages = [{include = "beancount_multitool", from = "src"}]
 repository = "https://github.com/rlan/beancount-multitool"
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
   "Intended Audience :: Financial and Insurance Industry",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
```

### Comparing `beancount_multitool-0.4.1/src/beancount_multitool/JABank.py` & `beancount_multitool-0.5.0/src/beancount_multitool/JABank.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.1/src/beancount_multitool/MappingDatabase.py` & `beancount_multitool-0.5.0/src/beancount_multitool/MappingDatabase.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.1/src/beancount_multitool/RakutenBank.py` & `beancount_multitool-0.5.0/src/beancount_multitool/RakutenBank.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.1/src/beancount_multitool/RakutenCard.py` & `beancount_multitool-0.5.0/src/beancount_multitool/RakutenCard.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.1/src/beancount_multitool/ShinseiBank.py` & `beancount_multitool-0.5.0/src/beancount_multitool/ShinseiBank.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.1/src/beancount_multitool/as_transaction.py` & `beancount_multitool-0.5.0/src/beancount_multitool/as_transaction.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.1/src/beancount_multitool/cli.py` & `beancount_multitool-0.5.0/src/beancount_multitool/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 # Get available finanicial institutions
 from beancount_multitool import __INSTITUTIONS__
 
 from beancount_multitool import JABank
 from beancount_multitool import RakutenBank
 from beancount_multitool import RakutenCard
 from beancount_multitool import ShinseiBank
+from beancount_multitool import SumishinNetBank
 
 
 def validate_name(ctx, param, value):
     """Check given name is one of supported financial institutions."""
     if value in __INSTITUTIONS__:
         return value
     else:
         raise click.BadParameter(f"Name must be one of: {__INSTITUTIONS__}")
 
 
 @click.command(
-    epilog=f"Note: supported names of financial institutions: {__INSTITUTIONS__}"
+    epilog=f"Note: supported financial institutions are {__INSTITUTIONS__}"
 )
 @click.argument("name", type=str, callback=validate_name)
 @click.argument("config", type=click.Path(exists=True))
 @click.argument("data", type=click.Path(exists=True))
 @click.option(
     "--output",
     default="output.bean",
@@ -45,13 +46,17 @@
         tool = JABank(config)
     elif name == RakutenBank.NAME:
         tool = RakutenBank(config)
     elif name == RakutenCard.NAME:
         tool = RakutenCard(config)
     elif name == ShinseiBank.NAME:
         tool = ShinseiBank(config)
+    elif name == SumishinNetBank.NAME:
+        tool = SumishinNetBank(config)
+    else:
+        raise ValueError(f"Unknown name: {name}")
 
     return tool.convert(data, output)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `beancount_multitool-0.4.1/src/beancount_multitool/get_value.py` & `beancount_multitool-0.5.0/src/beancount_multitool/get_value.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.1/src/beancount_multitool/read_config.py` & `beancount_multitool-0.5.0/src/beancount_multitool/read_config.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.1/src/beancount_multitool/tests/test_get_value.py` & `beancount_multitool-0.5.0/src/beancount_multitool/tests/test_get_value.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.1/PKG-INFO` & `beancount_multitool-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-multitool
-Version: 0.4.1
+Version: 0.5.0
 Summary: A CLI tool that converts financial data to Beancount files
 Home-page: https://github.com/rlan/beancount-multitool
 License: MIT
 Author: Rick Lan
 Author-email: rlan@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -43,12 +43,13 @@
 The following financial institutions are supported:
 
 * Japan
   * [JA Bank ＪＡネットバンク](https://www.jabank.jp/)
   * [Rakuten Card 楽天カード](https://www.rakuten-card.co.jp/)
   * [Rakuten Bank 楽天銀行](https://www.rakuten-bank.co.jp/)
   * [SBI Shinsei Bank 新生銀行](https://www.sbishinseibank.co.jp/)
+  * [SBI Sumishin Net Bank 住信SBIネット銀行](https://www.netbk.co.jp/)
 
 To get started, see the [documentation](https://rlan.github.io/beancount-multitool).
 
 License: [MIT](LICENSE)
```

